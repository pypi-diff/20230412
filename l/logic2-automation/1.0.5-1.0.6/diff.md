# Comparing `tmp/logic2_automation-1.0.5.tar.gz` & `tmp/logic2_automation-1.0.6.tar.gz`

## Comparing `logic2_automation-1.0.5.tar` & `logic2_automation-1.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 logic2_automation-1.0.5/grpc_build_hook.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 logic2_automation-1.0.5/saleae/automation/__init__.py
--rw-r--r--   0        0        0    16332 2020-02-02 00:00:00.000000 logic2_automation-1.0.5/saleae/automation/capture.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 logic2_automation-1.0.5/saleae/automation/errors.py
--rw-r--r--   0        0        0    24206 2020-02-02 00:00:00.000000 logic2_automation-1.0.5/saleae/automation/manager.py
--rw-r--r--   0        0        0    17678 2020-02-02 00:00:00.000000 logic2_automation-1.0.5/proto/saleae/grpc/saleae.proto
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logic2_automation-1.0.5/.gitignore
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 logic2_automation-1.0.5/README.md
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 logic2_automation-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 logic2_automation-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 logic2_automation-1.0.6/grpc_build_hook.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 logic2_automation-1.0.6/saleae/automation/__init__.py
+-rw-r--r--   0        0        0    16332 2020-02-02 00:00:00.000000 logic2_automation-1.0.6/saleae/automation/capture.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 logic2_automation-1.0.6/saleae/automation/errors.py
+-rw-r--r--   0        0        0    24206 2020-02-02 00:00:00.000000 logic2_automation-1.0.6/saleae/automation/manager.py
+-rw-r--r--   0        0        0    17678 2020-02-02 00:00:00.000000 logic2_automation-1.0.6/proto/saleae/grpc/saleae.proto
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logic2_automation-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 logic2_automation-1.0.6/README.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 logic2_automation-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 logic2_automation-1.0.6/PKG-INFO
```

### Comparing `logic2_automation-1.0.5/grpc_build_hook.py` & `logic2_automation-1.0.6/grpc_build_hook.py`

 * *Files identical despite different names*

### Comparing `logic2_automation-1.0.5/saleae/automation/__init__.py` & `logic2_automation-1.0.6/saleae/automation/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 try:
     from saleae.grpc import saleae_pb2, saleae_pb2_grpc
 except Exception as exc:
     import sys
     sys.stderr.write('''There was an error that occurred while importing grpc/pb modules.
 This can be caused by pb files that were generated using an incompatible version of protobuf.
-You can regenerate these files by reinstalling logic2-automaation:
+You can regenerate these files by reinstalling logic2-automation:
 
-     pip --force-reinstall logic2-automation
+     pip install logic2-automation --force-reinstall
 
  ''')
     raise exc from None
 
 from .manager import *
 from .capture import *
 from .errors import *
```

### Comparing `logic2_automation-1.0.5/saleae/automation/capture.py` & `logic2_automation-1.0.6/saleae/automation/capture.py`

 * *Files identical despite different names*

### Comparing `logic2_automation-1.0.5/saleae/automation/errors.py` & `logic2_automation-1.0.6/saleae/automation/errors.py`

 * *Files identical despite different names*

### Comparing `logic2_automation-1.0.5/saleae/automation/manager.py` & `logic2_automation-1.0.6/saleae/automation/manager.py`

 * *Files identical despite different names*

### Comparing `logic2_automation-1.0.5/proto/saleae/grpc/saleae.proto` & `logic2_automation-1.0.6/proto/saleae/grpc/saleae.proto`

 * *Files identical despite different names*

### Comparing `logic2_automation-1.0.5/README.md` & `logic2_automation-1.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 `logic2-automation` implements a Python client for the [Logic 2 Automation API](https://www.saleae.com/automation/).
 
 Documentation can be found at https://saleae.github.io/logic2-automation/
 
 
 ## Changelog
 
+### 1.0.6
+
+- Moved `grpcio-tools` to build dependencies.
+
 ### 1.0.5
 
 - The .whl build has been fixed, and now includes the generate protobuf/grpc files.
 
 ### 1.0.4
 
 - YANKED!
```

### Comparing `logic2_automation-1.0.5/pyproject.toml` & `logic2_automation-1.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "logic2-automation"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
     { name="Saleae, Inc.", email="support@saleae.com" },
 ]
 description = "Library for using the Saleae Logic 2 Automation API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
    "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "grpcio>=1.13.0",
-    "grpcio-tools>=1.13.0",
+    "protobuf>=3.5.0.post1",
     "pywin32; platform_system == 'Windows'"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/saleae/logic2-automation"
 "Bug Tracker" = "https://github.com/saleae/logic2-automation/issues"
 
@@ -43,8 +43,11 @@
 [tool.hatch.build.force-include]
 "../proto/saleae/grpc/saleae.proto" = "proto/saleae/grpc/saleae.proto"
 
 # The gRPC/protobuf files are only generated when building a wheel
 [tool.hatch.build.targets.wheel.hooks.custom]
 require-runtime-dependencies = true
 path = "grpc_build_hook.py"
+dependencies = [
+    "grpcio-tools>=1.13.0",
+]
```

### Comparing `logic2_automation-1.0.5/PKG-INFO` & `logic2_automation-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: logic2-automation
-Version: 1.0.5
+Version: 1.0.6
 Summary: Library for using the Saleae Logic 2 Automation API
 Project-URL: Homepage, https://github.com/saleae/logic2-automation
 Project-URL: Bug Tracker, https://github.com/saleae/logic2-automation/issues
 Author-email: "Saleae, Inc." <support@saleae.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: grpcio-tools>=1.13.0
 Requires-Dist: grpcio>=1.13.0
+Requires-Dist: protobuf>=3.5.0.post1
 Requires-Dist: pywin32; platform_system == 'Windows'
 Description-Content-Type: text/markdown
 
 # Saleae Logic 2 Automation
 
 `logic2-automation` implements a Python client for the [Logic 2 Automation API](https://www.saleae.com/automation/).
 
 Documentation can be found at https://saleae.github.io/logic2-automation/
 
 
 ## Changelog
 
+### 1.0.6
+
+- Moved `grpcio-tools` to build dependencies.
+
 ### 1.0.5
 
 - The .whl build has been fixed, and now includes the generate protobuf/grpc files.
 
 ### 1.0.4
 
 - YANKED!
```

