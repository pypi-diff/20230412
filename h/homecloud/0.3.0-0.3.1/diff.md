# Comparing `tmp/homecloud-0.3.0.tar.gz` & `tmp/homecloud-0.3.1.tar.gz`

## Comparing `homecloud-0.3.0.tar` & `homecloud-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 homecloud-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/__init__.py
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/client_settings.toml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/client_subclass.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/get_routes.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/homecloud_config.toml
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/homecloud_generator.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/homecloud_logging.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/homecloud_utils.py
--rw-r--r--   0        0        0    10837 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/module_to_api.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/post_routes.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/request_models.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/router_template.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 homecloud-0.3.0/src/homecloud/server.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 homecloud-0.3.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 homecloud-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 homecloud-0.3.0/README.md
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 homecloud-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 homecloud-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 homecloud-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/__init__.py
+-rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/client_settings.toml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/client_subclass.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/get_routes.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/homecloud_config.toml
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/homecloud_generator.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/homecloud_logging.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/homecloud_utils.py
+-rw-r--r--   0        0        0    10837 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/module_to_api.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/post_routes.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/request_models.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/router_template.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 homecloud-0.3.1/src/homecloud/server.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 homecloud-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 homecloud-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 homecloud-0.3.1/README.md
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 homecloud-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 homecloud-0.3.1/PKG-INFO
```

### Comparing `homecloud-0.3.0/CHANGELOG.md` & `homecloud-0.3.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 # Changelog
 
-## 0.2.0 (2023-04-03)
+## 0.3.0 (2023-04-10)
+
+#### Refactorings
+
+* move push_logs check and call from on_fail decorator to client.send_request()
+
+
+## v0.2.0 (2023-04-03)
 
 #### New Features
 
 * add log_path param to client and logging files to override default behavior
 #### Refactorings
 
 * replace pathlib.Path with pathier.Pathier
 #### Others
 
+* build v0.2.0
+* update changelog
 * remove unused imports from client.py
 
 
 ## v0.1.1 (2023-03-22)
 
 #### Others
```

### Comparing `homecloud-0.3.0/src/homecloud/client.py` & `homecloud-0.3.1/src/homecloud/client.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.3.0/src/homecloud/client_subclass.py` & `homecloud-0.3.1/src/homecloud/client_subclass.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-import json
-
 import requests
+from pathier import Pathier
 
 from homecloud import HomeCloudClient, on_fail
 
 
 class app_nameClient(HomeCloudClient):
     def __init__(
         self,
         app_name: str = "$app_name",
         send_logs: bool = True,
         log_send_thresh: int = 10,
         log_level: str = "INFO",
+        log_path: Pathier | str = None,
         timeout: int = 10,
     ):
-        super().__init__(app_name, send_logs, log_send_thresh, log_level, timeout)
+        super().__init__(
+            app_name, send_logs, log_send_thresh, log_level, log_path, timeout
+        )
 
     @on_fail
     def hello(self) -> str:
         """Contacts the server and returns the app name."""
         self.logger.debug(f"Saying hello to the {self.app_name} server.")
-        return json.loads(self.send_request("get", "/homecloud").text)["app_name"]
+        return self.send_request("get", "/homecloud").json()["app_name"]
```

### Comparing `homecloud-0.3.0/src/homecloud/get_routes.py` & `homecloud-0.3.1/src/homecloud/get_routes.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.3.0/src/homecloud/homecloud_generator.py` & `homecloud-0.3.1/src/homecloud/homecloud_generator.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.3.0/src/homecloud/homecloud_logging.py` & `homecloud-0.3.1/src/homecloud/homecloud_logging.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.3.0/src/homecloud/homecloud_utils.py` & `homecloud-0.3.1/src/homecloud/homecloud_utils.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.3.0/src/homecloud/module_to_api.py` & `homecloud-0.3.1/src/homecloud/module_to_api.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.3.0/src/homecloud/server.py` & `homecloud-0.3.1/src/homecloud/server.py`

 * *Files identical despite different names*

### Comparing `homecloud-0.3.0/LICENSE.txt` & `homecloud-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `homecloud-0.3.0/README.md` & `homecloud-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `homecloud-0.3.0/pyproject.toml` & `homecloud-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 000000a0: 7468 6520 7465 6d70 6c61 7465 2066 696c  the template fil
 000000b0: 6573 206e 6565 6465 6420 746f 2069 6e74  es needed to int
 000000c0: 6567 7261 7465 2066 6173 7461 7069 2c20  egrate fastapi, 
 000000d0: 7576 6963 6f72 6e2c 2061 6e64 2061 2072  uvicorn, and a r
 000000e0: 6571 7565 7374 7320 6261 7365 6420 636c  equests based cl
 000000f0: 6965 6e74 2069 6e74 6f20 6120 5079 7468  ient into a Pyth
 00000100: 6f6e 2070 726f 6a65 6374 2e22 0d0a 7665  on project."..ve
-00000110: 7273 696f 6e20 3d20 2230 2e33 2e30 220d  rsion = "0.3.0".
+00000110: 7273 696f 6e20 3d20 2230 2e33 2e31 220d  rsion = "0.3.1".
 00000120: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 00000130: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 00000140: 656e 6465 6e63 6965 7320 3d20 5b22 7265  endencies = ["re
 00000150: 7175 6573 7473 222c 2022 746f 6d6c 6b69  quests", "tomlki
 00000160: 7422 2c20 2270 7964 616e 7469 6322 2c20  t", "pydantic", 
 00000170: 2262 6c61 636b 222c 2022 6661 7374 6170  "black", "fastap
 00000180: 6922 2c20 226c 616e 7574 696c 7322 2c20  i", "lanutils",
```

### Comparing `homecloud-0.3.0/PKG-INFO` & `homecloud-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homecloud
-Version: 0.3.0
+Version: 0.3.1
 Summary: A command line tool for generating the template files needed to integrate fastapi, uvicorn, and a requests based client into a Python project.
 Project-URL: Homepage, https://github.com/matt-manes/homecloud
 Project-URL: Documentation, https://github.com/matt-manes/homecloud/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/homecloud/tree/main/src/homecloud
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: api,client,fastapi,network,server
```

