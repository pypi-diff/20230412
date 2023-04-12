# Comparing `tmp/pytest-inmanta-extensions-8.2.0.tar.gz` & `tmp/pytest-inmanta-extensions-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-inmanta-extensions-8.2.0.tar", last modified: Thu Feb  9 10:00:42 2023, max compression
+gzip compressed data, was "pytest-inmanta-extensions-8.3.0.tar", last modified: Wed Apr 12 07:26:49 2023, max compression
```

## Comparing `pytest-inmanta-extensions-8.2.0.tar` & `pytest-inmanta-extensions-8.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:42.246691 pytest-inmanta-extensions-8.2.0/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      199 2023-02-09 09:57:10.000000 pytest-inmanta-extensions-8.2.0/MANIFEST.in
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-02-09 10:00:42.246691 pytest-inmanta-extensions-8.2.0/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      467 2023-02-09 09:57:10.000000 pytest-inmanta-extensions-8.2.0/README.md
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       59 2023-02-09 10:00:42.247691 pytest-inmanta-extensions-8.2.0/setup.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2481 2023-02-09 09:57:10.000000 pytest-inmanta-extensions-8.2.0/setup.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:42.244691 pytest-inmanta-extensions-8.2.0/src/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:42.244691 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-02-09 09:57:10.000000 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    68061 2023-02-09 10:00:18.000000 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/conftest.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:42.245690 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:42.243690 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/ca/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:42.245690 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/ca/enduser-certs/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6223 2023-02-09 09:57:10.000000 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/ca/enduser-certs/server.chain
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2069 2023-02-09 09:57:10.000000 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/ca/enduser-certs/server.crt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-02-09 09:57:10.000000 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/ca/enduser-certs/server.key
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-02-09 09:57:10.000000 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1237 2023-02-09 10:00:18.000000 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/server.crt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1679 2023-02-09 10:00:18.000000 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/server.open.key
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:42.245690 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/db/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      980 2023-02-09 10:00:18.000000 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/db/common.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:42.246691 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/db/simple_project/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      212 2023-02-09 09:57:10.000000 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/db/simple_project/main.cf
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      185 2023-02-09 09:57:10.000000 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/db/simple_project/project.yml
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      685 2023-02-09 09:57:10.000000 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/plugin.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    25435 2023-02-09 10:00:18.000000 pytest-inmanta-extensions-8.2.0/src/inmanta_tests/utils.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:42.246691 pytest-inmanta-extensions-8.2.0/src/pytest_inmanta_extensions.egg-info/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-02-09 10:00:42.000000 pytest-inmanta-extensions-8.2.0/src/pytest_inmanta_extensions.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      882 2023-02-09 10:00:42.000000 pytest-inmanta-extensions-8.2.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-02-09 10:00:42.000000 pytest-inmanta-extensions-8.2.0/src/pytest_inmanta_extensions.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       55 2023-02-09 10:00:42.000000 pytest-inmanta-extensions-8.2.0/src/pytest_inmanta_extensions.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      122 2023-02-09 10:00:42.000000 pytest-inmanta-extensions-8.2.0/src/pytest_inmanta_extensions.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       14 2023-02-09 10:00:42.000000 pytest-inmanta-extensions-8.2.0/src/pytest_inmanta_extensions.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.465607 pytest-inmanta-extensions-8.3.0/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      199 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/MANIFEST.in
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-04-12 07:26:49.465607 pytest-inmanta-extensions-8.3.0/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      467 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/README.md
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       59 2023-04-12 07:26:49.466607 pytest-inmanta-extensions-8.3.0/setup.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2481 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/setup.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.463606 pytest-inmanta-extensions-8.3.0/src/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.464607 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    68790 2023-04-12 07:26:26.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/conftest.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.464607 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.462607 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.464607 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6223 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.chain
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2069 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.crt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1237 2023-04-12 07:26:26.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/server.crt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1679 2023-04-12 07:26:26.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/server.open.key
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.464607 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/db/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      980 2023-04-12 07:26:26.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/db/common.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.465607 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/db/simple_project/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      212 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/db/simple_project/main.cf
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      185 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/db/simple_project/project.yml
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      685 2023-04-12 07:23:21.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/plugin.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    25441 2023-04-12 07:26:26.000000 pytest-inmanta-extensions-8.3.0/src/inmanta_tests/utils.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:49.465607 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-04-12 07:26:49.000000 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      882 2023-04-12 07:26:49.000000 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-04-12 07:26:49.000000 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       55 2023-04-12 07:26:49.000000 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      122 2023-04-12 07:26:49.000000 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       14 2023-04-12 07:26:49.000000 pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/top_level.txt
```

### Comparing `pytest-inmanta-extensions-8.2.0/PKG-INFO` & `pytest-inmanta-extensions-8.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-inmanta-extensions
-Version: 8.2.0
+Version: 8.3.0
 Summary: Inmanta tests package
 Home-page: https://github.com/inmanta/inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Keywords: pytest inmanta tests
```

### Comparing `pytest-inmanta-extensions-8.2.0/setup.py` & `pytest-inmanta-extensions-8.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     Contact: code@inmanta.com
 """
 from os import path
 
 from setuptools import find_namespace_packages, setup
 
-version = "8.2.0"
+version = "8.3.0"
 
 requires = [
     "asyncpg",
     "click",
     f"inmanta-core~={version}.dev",
     "pip2pi",
     "pyformance",
```

### Comparing `pytest-inmanta-extensions-8.2.0/src/inmanta_tests/__init__.py` & `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.2.0/src/inmanta_tests/conftest.py` & `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     limitations under the License.
 
     Contact: code@inmanta.com
 """
 import warnings
 
 import toml
+from inmanta.config import AuthJWTConfig
 
 """
 About the use of @parametrize_any and @slowtest:
 
 For parametrized tests:
 - if the test is fast and tests different things for each parameter, use @parametrize
 - if the parameters only slightly increase the coverage of the test (some different exception path,...), use @parametrize_any.
@@ -99,14 +100,15 @@
 import build.env
 import inmanta
 import inmanta.agent
 import inmanta.app
 import inmanta.compiler as compiler
 import inmanta.compiler.config
 import inmanta.main
+import inmanta.user_setup
 from inmanta import config, const, data, env, loader, protocol, resources
 from inmanta.agent import handler
 from inmanta.agent.agent import Agent
 from inmanta.ast import CompilerException
 from inmanta.data.schema import SCHEMA_VERSION_TABLE
 from inmanta.db import util as db_util
 from inmanta.env import LocalPackagePath, VirtualEnv, mock_process_env
@@ -114,14 +116,15 @@
 from inmanta.module import InmantaModuleRequirement, InstallMode, Project, RelationPrecedenceRule
 from inmanta.moduletool import IsolatedEnvBuilderCached, ModuleTool, V2ModuleBuilder
 from inmanta.parser.plyInmantaParser import cache_manager
 from inmanta.protocol import VersionMatch
 from inmanta.server import SLICE_AGENT_MANAGER, SLICE_COMPILER
 from inmanta.server.bootloader import InmantaBootloader
 from inmanta.server.protocol import Server, SliceStartupException
+from inmanta.server.services import orchestrationservice
 from inmanta.server.services.compilerservice import CompilerService, CompileRun
 from inmanta.types import JsonType
 from inmanta.warnings import WarningsManager
 from libpip2pi.commands import dir2pi
 from packaging.version import Version
 
 # Import test modules differently when conftest is put into the inmanta_tests packages
@@ -507,14 +510,15 @@
     # command.Commander.reset()
     handler.Commander.reset()
     Project._project = None
     unknown_parameters.clear()
     InmantaBootloader.AVAILABLE_EXTENSIONS = None
     V2ModuleBuilder.DISABLE_ISOLATED_ENV_BUILDER_CACHE = False
     compiler.Finalizers.reset_finalizers()
+    AuthJWTConfig.reset()
 
 
 @pytest.fixture()
 def disable_isolated_env_builder_cache() -> None:
     V2ModuleBuilder.DISABLE_ISOLATED_ENV_BUILDER_CACHE = True
 
 
@@ -550,15 +554,15 @@
 
 
 @pytest.fixture(scope="function", autouse=True)
 def inmanta_config() -> Iterator[ConfigParser]:
     config.Config.load_config()
     config.Config.set("auth_jwt_default", "algorithm", "HS256")
     config.Config.set("auth_jwt_default", "sign", "true")
-    config.Config.set("auth_jwt_default", "client_types", "agent,compiler")
+    config.Config.set("auth_jwt_default", "client_types", "agent,compiler,api")
     config.Config.set("auth_jwt_default", "key", "rID3kG4OwGpajIsxnGDhat4UFcMkyFZQc1y3oKQTPRs")
     config.Config.set("auth_jwt_default", "expire", "0")
     config.Config.set("auth_jwt_default", "issuer", "https://localhost:8888/")
     config.Config.set("auth_jwt_default", "audience", "https://localhost:8888/")
 
     yield config.Config._get_instance()
 
@@ -1742,7 +1746,20 @@
             utils.create_python_package(
                 name=pkg_name,
                 pkg_version=Version("1.0.0"),
                 path=os.path.join(tmpdirname, pkg_name),
                 publish_index=pip_index,
             )
         yield pip_index.url
+
+
+@pytest.fixture(scope="session", autouse=True)
+def disable_version_and_agent_cleanup_job():
+    """
+    Disable the cleanup job ran by the Inmanta server that cleans up old model version and agent records that are no longer
+    used. Enabling this cleanup for the test suite causes race conditions in tests cases that create agent records without an
+    associated model version.
+    """
+    old_perform_cleanup = orchestrationservice.PERFORM_CLEANUP
+    orchestrationservice.PERFORM_CLEANUP = False
+    yield
+    orchestrationservice.PERFORM_CLEANUP = old_perform_cleanup
```

### Comparing `pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/ca/enduser-certs/server.chain` & `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.chain`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/ca/enduser-certs/server.crt` & `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.crt`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/ca/enduser-certs/server.key` & `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open` & `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/server.crt` & `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/server.crt`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.2.0/src/inmanta_tests/data/server.open.key` & `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/data/server.open.key`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.2.0/src/inmanta_tests/db/common.py` & `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/db/common.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.2.0/src/inmanta_tests/plugin.py` & `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.2.0/src/inmanta_tests/utils.py` & `pytest-inmanta-extensions-8.3.0/src/inmanta_tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 if not isinstance(val, dict):
                     return val
                 key = [str(val[x]) for x in sortby if x in val]
                 return "_".join(key)
 
             minimal = sorted(minimal, key=keyfunc)
             actual = sorted(actual, key=keyfunc)
-        for (m, a) in zip(minimal, actual):
+        for m, a in zip(minimal, actual):
             assert_equal_ish(m, a, sortby)
     elif minimal is UNKWN:
         return
     else:
         assert minimal == actual, f"Minimal value expected is '{minimal}' but got '{actual}'"
 
 
@@ -233,15 +233,15 @@
 
 
 def assert_no_warning(caplog, loggers_to_allow: list[str] = NOISY_LOGGERS):
     """
     Assert there are no warning, except from the list of loggers to allow
     """
     for record in caplog.records:
-        assert record.levelname != "WARNING" or (record.name in loggers_to_allow)
+        assert record.levelname != "WARNING" or (record.name in loggers_to_allow), record
 
 
 def configure(unused_tcp_port, database_name, database_port):
     import inmanta.agent.config  # noqa: F401
     import inmanta.server.config  # noqa: F401
     from inmanta.config import Config
```

### Comparing `pytest-inmanta-extensions-8.2.0/src/pytest_inmanta_extensions.egg-info/PKG-INFO` & `pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-inmanta-extensions
-Version: 8.2.0
+Version: 8.3.0
 Summary: Inmanta tests package
 Home-page: https://github.com/inmanta/inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Keywords: pytest inmanta tests
```

### Comparing `pytest-inmanta-extensions-8.2.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt` & `pytest-inmanta-extensions-8.3.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

