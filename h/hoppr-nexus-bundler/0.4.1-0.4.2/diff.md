# Comparing `tmp/hoppr_nexus_bundler-0.4.1.tar.gz` & `tmp/hoppr_nexus_bundler-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_nexus_bundler-0.4.1.tar", max compression
+gzip compressed data, was "hoppr_nexus_bundler-0.4.2.tar", max compression
```

## Comparing `hoppr_nexus_bundler-0.4.1.tar` & `hoppr_nexus_bundler-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1084 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/LICENSE
--rw-r--r--   0        0        0     1694 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/README.md
--rw-r--r--   0        0        0       89 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/__init__.py
--rw-r--r--   0        0        0     7091 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/bundler.py
--rw-r--r--   0        0        0     1998 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/nexus_instance.py
--rw-r--r--   0        0        0        0 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/__init__.py
--rw-r--r--   0        0        0     4431 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/apt_publisher.py
--rw-r--r--   0        0        0     9523 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/base_publisher.py
--rw-r--r--   0        0        0     6269 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/docker_publisher.py
--rw-r--r--   0        0        0     2321 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/git_publisher.py
--rw-r--r--   0        0        0      876 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/helm_publisher.py
--rw-r--r--   0        0        0     1916 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/maven_publisher.py
--rw-r--r--   0        0        0        0 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/py.typed
--rw-r--r--   0        0        0      875 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/pypi_publisher.py
--rw-r--r--   0        0        0     1904 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/raw_publisher.py
--rw-r--r--   0        0        0     5711 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/yum_publisher.py
--rw-r--r--   0        0        0        0 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/nexus_bundler/py.typed
--rw-r--r--   0        0        0      999 2023-01-26 23:09:29.000000 hoppr_nexus_bundler-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 hoppr_nexus_bundler-0.4.1/setup.py
--rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 hoppr_nexus_bundler-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1694 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/README.md
+-rw-r--r--   0        0        0       89 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/__init__.py
+-rw-r--r--   0        0        0     7034 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/bundler.py
+-rw-r--r--   0        0        0     1998 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/nexus_instance.py
+-rw-r--r--   0        0        0        0 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/__init__.py
+-rw-r--r--   0        0        0     4373 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/apt_publisher.py
+-rw-r--r--   0        0        0     9569 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/base_publisher.py
+-rw-r--r--   0        0        0     6265 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/docker_publisher.py
+-rw-r--r--   0        0        0     2278 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/git_publisher.py
+-rw-r--r--   0        0        0      833 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/helm_publisher.py
+-rw-r--r--   0        0        0     1873 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/maven_publisher.py
+-rw-r--r--   0        0        0        0 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/py.typed
+-rw-r--r--   0        0        0      832 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/pypi_publisher.py
+-rw-r--r--   0        0        0     1861 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/raw_publisher.py
+-rw-r--r--   0        0        0     5741 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/yum_publisher.py
+-rw-r--r--   0        0        0        0 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/nexus_bundler/py.typed
+-rw-r--r--   0        0        0     1164 2023-04-12 04:07:21.000000 hoppr_nexus_bundler-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 hoppr_nexus_bundler-0.4.2/PKG-INFO
```

### Comparing `hoppr_nexus_bundler-0.4.1/LICENSE` & `hoppr_nexus_bundler-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.1/README.md` & `hoppr_nexus_bundler-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.1/nexus_bundler/bundler.py` & `hoppr_nexus_bundler-0.4.2/nexus_bundler/bundler.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 """
 
 from concurrent.futures import Future, ProcessPoolExecutor
 import os
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
 
-from hoppr.base_plugins.hoppr import HopprPlugin, hoppr_process
+from hoppr import HopprContext, HopprPlugin, Result, hoppr_process
 from hoppr.exceptions import HopprPluginError
-from hoppr.context import Context
-from hoppr.result import Result
+
 from nexus_bundler import __version__
 from nexus_bundler.publishers.apt_publisher import AptPublisher
 from nexus_bundler.publishers.base_publisher import Publisher
 from nexus_bundler.publishers.maven_publisher import MavenPublisher
 from nexus_bundler.publishers.git_publisher import GitPublisher
 from nexus_bundler.publishers.raw_publisher import RawPublisher
 from nexus_bundler.publishers.pypi_publisher import PypiPublisher
@@ -37,15 +36,15 @@
     """
 
     publishers: Dict[str, Publisher] = {}
 
     def get_version(self) -> str:
         return __version__
 
-    def __init__(self, context: Context, config: Any = None) -> None:
+    def __init__(self, context: HopprContext, config: Any = None) -> None:
         super().__init__(context, config)
 
         use_config = {}
         if config is not None:
             use_config = config
 
         self.nexus_instance = NexusInstance(
```

### Comparing `hoppr_nexus_bundler-0.4.1/nexus_bundler/nexus_instance.py` & `hoppr_nexus_bundler-0.4.2/nexus_bundler/nexus_instance.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/apt_publisher.py` & `hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/apt_publisher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """
 Nexus publisher for docker artifacts
 """
 from pathlib import Path
 import time
 from typing import Any, Dict, Optional
 
-from hoppr.base_plugins.hoppr import hoppr_rerunner
-from hoppr.context import Context
-from hoppr.result import Result
+from hoppr import HopprContext, Result, hoppr_rerunner
 from hoppr.exceptions import HopprError
 
 from nexus_bundler.publishers.base_publisher import Publisher
 from nexus_bundler.nexus_instance import NexusInstance
 
 
 class AptPublisher(Publisher):
@@ -23,15 +21,15 @@
     See https://issues.sonatype.org/browse/NEXUS-28889
     """
 
     nexus_repository_type = "apt"
     required_tools = ["gpg"]
 
     def __init__(
-        self, nexus_instance: NexusInstance, context: Context, config: Any = None
+        self, nexus_instance: NexusInstance, context: HopprContext, config: Any = None
     ) -> None:
         super().__init__(nexus_instance, context, config)
 
         if self.config is not None:
             if "gpg_command" in self.config:
                 self.required_tools = [self.config["gpg_command"]]
```

### Comparing `hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/base_publisher.py` & `hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/base_publisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 import json
 import os
 from pathlib import Path
 import re
 import subprocess
 from typing import Any, Dict, List, Optional
 import requests
-from hoppr.base_plugins.hoppr import hoppr_rerunner
+from hoppr import HopprContext, Result, hoppr_rerunner
 from hoppr.exceptions import HopprError
-from hoppr.context import Context
 from hoppr.mem_logger import MemoryLogger
-from hoppr.result import Result
 from hoppr.plugin_utils import check_for_missing_commands, repo_url_from_dir_name
 from hoppr.utils import obscure_passwords
 from nexus_bundler.nexus_instance import NexusInstance
 
 
 class Publisher(ABC):
     """
@@ -29,24 +27,24 @@
     id_iter = itertools.count()
 
     nexus_repository_type = "raw"
     nexus_repository_format = None
     required_tools: List[str] = []
 
     def __init__(
-        self, nexus_instance: NexusInstance, context: Context, config: Any = None
+        self, nexus_instance: NexusInstance, context: HopprContext, config: Any = None
     ) -> None:
         self.instance_id = next(self.id_iter)
         self.nexus_instance = nexus_instance
         if self.nexus_repository_format is None:
             self.nexus_repository_format = self.nexus_repository_type
         log_name = f"pub--{self.__class__.__name__}--{os.getpid()}-{self.instance_id}"
         self.context = context
         self._logger = MemoryLogger(
-            self.context.logfile_location, self.context.logfile_lock, log_name
+            str(context.logfile_location), context.logfile_lock, log_name  # type: ignore[arg-type]
         )
         self.root_dir = Path(context.collect_root_dir).absolute()
         self.config = config
 
     def get_logger(self) -> MemoryLogger:
         """
         Returns the logger for this publisher (needed by hoppr_rerunner)
@@ -120,14 +118,15 @@
 
                 response = requests.post(
                     f"{self.nexus_instance.get_repository_api()}/"
                     + f"{self.nexus_repository_type}/hosted",
                     auth=(self.nexus_instance.userid, self.nexus_instance.password),
                     data=json.dumps(data),
                     headers=headers,
+                    timeout=600,
                 )
 
                 if response.status_code != 201:
                     msg = (
                         f"Response code {response.status_code} returned from nexus API call to "
                         + f"create {self.nexus_repository_type} repository '{repo_name}'.\n"
                         + f"Response text: {response.text}"
@@ -179,14 +178,15 @@
         """
 
         ### Get existing repos, and see if the requested repo name is already created
 
         repo_list = requests.get(
             f"{self.nexus_instance.get_repository_api()}/",
             auth=(self.nexus_instance.userid, self.nexus_instance.password),
+            timeout=600,
         )
 
         if repo_list.status_code != 200:
             msg = (
                 f"Error code retrieving list of repositories: {repo_list.status_code}\n"
                 + f"Reason: {repo_list.reason}"
             )
@@ -263,14 +263,15 @@
         response = requests.post(
             f"{self.nexus_instance.get_component_api()}?repository={repository}",
             files=files,
             data=data,
             auth=(self.nexus_instance.userid, self.nexus_instance.password),
             allow_redirects=True,
             verify=verify,
+            timeout=600,
         )
 
         return Result.from_http_response(response)
 
     def run_command(self, command, password_list=None, cwd=None):
         """
         Run a command and log any errors
```

### Comparing `hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/docker_publisher.py` & `hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/docker_publisher.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 """
 import json
 from pathlib import Path
 import re
 from typing import Any, Dict
 import requests
 
-from hoppr.base_plugins.hoppr import hoppr_rerunner
-from hoppr.context import Context
-from hoppr.result import Result
+from hoppr import HopprContext, Result, hoppr_rerunner
 from hoppr.exceptions import HopprError
 
 from nexus_bundler.publishers.base_publisher import Publisher
 from nexus_bundler.nexus_instance import NexusInstance
 
 
 class DockerPublisher(Publisher):
@@ -21,15 +19,15 @@
     Nexus publisher for docker artifacts
     """
 
     nexus_repository_type = "docker"
     required_tools = ["skopeo"]
 
     def __init__(
-        self, nexus_instance: NexusInstance, context: Context, config: Any = None
+        self, nexus_instance: NexusInstance, context: HopprContext, config: Any = None
     ) -> None:
         super().__init__(nexus_instance, context, config)
 
         if self.config is not None:
             if "skopeo_command" in self.config:
                 self.required_tools = [self.config["skopeo_command"]]
 
@@ -85,14 +83,15 @@
 
         address = f"{self.nexus_instance.url}service/rest/beta/security/realms/active"
 
         response = requests.get(
             address,
             auth=(self.nexus_instance.userid, self.nexus_instance.password),
             headers=headers,
+            timeout=600,
         )
 
         if response.status_code != 200:
             msg = (
                 f"Response code {response.status_code} returned from nexus API to retrieve "
                 + "active realms.\n"
                 + f"Response text: {response.text}"
@@ -105,14 +104,15 @@
         if "DockerToken" not in realms:
             realms.append("DockerToken")
             response = requests.put(
                 address,
                 auth=(self.nexus_instance.userid, self.nexus_instance.password),
                 data=json.dumps(realms),
                 headers=headers,
+                timeout=600,
             )
             if response.status_code != 204:
                 msg = (
                     f"Response code {response.status_code} returned from "
                     + "Nexus API call to add DockerToken realm.\n"
                     + f"Response text: {response.text}"
                 )
```

### Comparing `hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/git_publisher.py` & `hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/git_publisher.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 Nexus publisher for git artifacts
 """
 
 from contextlib import ExitStack
 import os
 from pathlib import Path
 from typing import Dict
-from hoppr.base_plugins.hoppr import hoppr_rerunner
-from hoppr.result import Result
+from hoppr import Result, hoppr_rerunner
 from nexus_bundler.publishers.base_publisher import Publisher
 
 
 class GitPublisher(Publisher):
     """
     Nexus publisher for git artifacts
     """
```

### Comparing `hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/helm_publisher.py` & `hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/helm_publisher.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Nexus publisher for helm artifacts
 """
 from pathlib import Path
-from hoppr.base_plugins.hoppr import hoppr_rerunner
-from hoppr.result import Result
+from hoppr import Result, hoppr_rerunner
 
 from nexus_bundler.publishers.base_publisher import Publisher
 
 
 class HelmPublisher(Publisher):
     """
     Nexus publisher for helm artifacts
```

### Comparing `hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/pypi_publisher.py` & `hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/pypi_publisher.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Nexus publisher for pypi artifacts
 """
 
 from pathlib import Path
-from hoppr.base_plugins.hoppr import hoppr_rerunner
-from hoppr.result import Result
+from hoppr import Result, hoppr_rerunner
 from nexus_bundler.publishers.base_publisher import Publisher
 
 
 class PypiPublisher(Publisher):
     """
     Nexus publisher for pypi artifacts
     """
```

### Comparing `hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/raw_publisher.py` & `hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/raw_publisher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Nexus publisher for raw artifacts
 """
 
 from pathlib import Path
 from typing import Dict
-from hoppr.base_plugins.hoppr import hoppr_rerunner
-from hoppr.result import Result
+from hoppr import Result, hoppr_rerunner
 from nexus_bundler.publishers.base_publisher import Publisher
 
 
 class RawPublisher(Publisher):
     """
     Nexus publisher for raw artifacts
     """
```

### Comparing `hoppr_nexus_bundler-0.4.1/nexus_bundler/publishers/yum_publisher.py` & `hoppr_nexus_bundler-0.4.2/nexus_bundler/publishers/yum_publisher.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,29 @@
 """
 
 import json
 from pathlib import Path
 import re
 from typing import Any, Dict, List
 import requests
-from hoppr.base_plugins.hoppr import hoppr_rerunner
-from hoppr.context import Context
+from hoppr import HopprContext, Result, hoppr_rerunner
 from hoppr.exceptions import HopprPluginError
-from hoppr.result import Result
 from nexus_bundler.publishers.base_publisher import Publisher
 from nexus_bundler.nexus_instance import NexusInstance
 
 
 class YumPublisher(Publisher):
     """
     Nexus publisher for yum artifacts
     """
 
     nexus_repository_type = "yum"
 
     def __init__(
-        self, nexus_instance: NexusInstance, context: Context, config: Any = None
+        self, nexus_instance: NexusInstance, context: HopprContext, config: Any = None
     ) -> None:
         super().__init__(nexus_instance, context, config)
         self.yum_data_depth = -1
 
     @hoppr_rerunner
     def push_artifact(self, path: Path) -> Result:
         """
@@ -59,14 +57,15 @@
         """
         Group yum repositories of different data depths
         """
 
         repository_list = requests.get(
             f"{self.nexus_instance.get_repository_api()}/",
             auth=(self.nexus_instance.userid, self.nexus_instance.password),
+            timeout=600,
         )
 
         if repository_list.status_code != 200:
             msg = (
                 f"Error code retrieving list of yum repositories: {repository_list.status_code}\n"
                 + f"Reason: {repository_list.reason}"
             )
@@ -105,16 +104,17 @@
 
             response = requests.post(
                 f"{self.nexus_instance.get_repository_api()}/yum/group",
                 auth=(
                     self.nexus_instance.userid,
                     self.nexus_instance.password,
                 ),
-                data=json.dumps(data),
+                data=json.dumps(data),  # pylint: disable=duplicate-code
                 headers=headers,
+                timeout=600,
             )
 
             if response.status_code != 201:
                 msg = (
                     f"Failed to create yum group repo {group_name}. "
                     + f"Response code: {response.status_code}. "
                     + f"Response message: {response.text}"
```

### Comparing `hoppr_nexus_bundler-0.4.1/pyproject.toml` & `hoppr_nexus_bundler-0.4.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr_nexus_bundler"
-version = "0.4.1"
+version = "0.4.2"
 description = "Plug-in for Hoppr to bundle artifacts into a Nexus Repository"
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev/"
 repository = "https://gitlab.com/-/ide/project/lmco/hoppr/plugins/hoppr-nexus-bundler"
 
@@ -25,19 +25,26 @@
 packages = [
     { include = "nexus_bundler" },
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
+hoppr = "^1.8.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 pylint = "^2.14.4"
 mypy = "^0.961"
-coverage = "^6.4.1"
+coverage = "^7.0.0"
 pytest = "^7.1.2"
-hoppr = ">=0.20.0"
+
+[[tool.mypy.overrides]]
+module = ["test.*", "ruamel"]
+allow_untyped_defs = true
+allow_incomplete_defs = true
+allow_untyped_calls = true
+ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hoppr_nexus_bundler-0.4.1/PKG-INFO` & `hoppr_nexus_bundler-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr-nexus-bundler
-Version: 0.4.1
+Version: 0.4.2
 Summary: Plug-in for Hoppr to bundle artifacts into a Nexus Repository
 Home-page: https://hoppr.dev/
 License: MIT
 Keywords: hoppr,plugin,nexus
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: System :: Software Distribution
+Requires-Dist: hoppr (>=1.8.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/-/ide/project/lmco/hoppr/plugins/hoppr-nexus-bundler
 Description-Content-Type: text/markdown
 
 # Nexus Bundler for Hoppr
 
 The Nexus Bundler is a plug-in for [Hoppr](https://gitlab.com/lmco/hoppr/hoppr) to package the collected artifacts into an existing Nexus instance.
```

