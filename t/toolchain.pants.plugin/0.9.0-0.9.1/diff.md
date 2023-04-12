# Comparing `tmp/toolchain.pants.plugin-0.9.0.tar.gz` & `tmp/toolchain.pants.plugin-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toolchain.pants.plugin-0.9.0.tar", last modified: Thu Apr 29 16:37:09 2021, max compression
+gzip compressed data, was "dist/toolchain.pants.plugin-0.9.1.tar", last modified: Thu Apr 29 22:47:41 2021, max compression
```

## Comparing `toolchain.pants.plugin-0.9.0.tar` & `toolchain.pants.plugin-0.9.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 16:37:09.658689 toolchain.pants.plugin-0.9.0/
--rw-r--r--   0 asher      (501) staff       (20)       12 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/MANIFEST.in
--rw-r--r--   0 asher      (501) staff       (20)     1197 2021-04-29 16:37:09.658378 toolchain.pants.plugin-0.9.0/PKG-INFO
--rw-r--r--   0 asher      (501) staff       (20)       38 2021-04-29 16:37:09.658844 toolchain.pants.plugin-0.9.0/setup.cfg
--rw-r--r--   0 asher      (501) staff       (20)     2049 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/setup.py
-drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 16:37:09.645605 toolchain.pants.plugin-0.9.0/src/
-drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 16:37:09.647461 toolchain.pants.plugin-0.9.0/src/toolchain/
--rw-r--r--   0 asher      (501) staff       (20)        0 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/__init__.py
-drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 16:37:09.650272 toolchain.pants.plugin-0.9.0/src/toolchain/base/
--rw-r--r--   0 asher      (501) staff       (20)     1480 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/base/datetime_tools.py
-drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 16:37:09.650831 toolchain.pants.plugin-0.9.0/src/toolchain/pants/
-drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 16:37:09.654114 toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/
--rw-r--r--   0 asher      (501) staff       (20)        0 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/__init__.py
--rw-r--r--   0 asher      (501) staff       (20)    10726 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/client.py
--rw-r--r--   0 asher      (501) staff       (20)    51965 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/error.html
--rw-r--r--   0 asher      (501) staff       (20)     2579 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/favicon.png
--rw-r--r--   0 asher      (501) staff       (20)     2514 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/plugin.py
--rw-r--r--   0 asher      (501) staff       (20)      544 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/register.py
--rw-r--r--   0 asher      (501) staff       (20)    11498 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/rules.py
--rw-r--r--   0 asher      (501) staff       (20)     5851 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/server.py
--rw-r--r--   0 asher      (501) staff       (20)     2473 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/store.py
--rw-r--r--   0 asher      (501) staff       (20)    53298 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/success.html
-drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 16:37:09.657183 toolchain.pants.plugin-0.9.0/src/toolchain/pants/buildsense/
--rw-r--r--   0 asher      (501) staff       (20)     9452 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/buildsense/client.py
--rw-r--r--   0 asher      (501) staff       (20)      871 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/buildsense/common.py
--rw-r--r--   0 asher      (501) staff       (20)    10113 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/buildsense/converter.py
--rw-r--r--   0 asher      (501) staff       (20)     5807 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/buildsense/local_store.py
--rw-r--r--   0 asher      (501) staff       (20)    12709 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/buildsense/reporter.py
--rw-r--r--   0 asher      (501) staff       (20)    10077 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/buildsense/state.py
-drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 16:37:09.657822 toolchain.pants.plugin-0.9.0/src/toolchain/pants/common/
--rw-r--r--   0 asher      (501) staff       (20)      727 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/common/network.py
--rw-r--r--   0 asher      (501) staff       (20)     1306 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/common/toolchain_setup.py
--rw-r--r--   0 asher      (501) staff       (20)      763 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/register.py
--rw-r--r--   0 asher      (501) staff       (20)      528 2021-04-29 16:37:08.000000 toolchain.pants.plugin-0.9.0/src/toolchain/pants/version.py
-drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 16:37:09.649997 toolchain.pants.plugin-0.9.0/src/toolchain.pants.plugin.egg-info/
--rw-r--r--   0 asher      (501) staff       (20)     1197 2021-04-29 16:37:09.000000 toolchain.pants.plugin-0.9.0/src/toolchain.pants.plugin.egg-info/PKG-INFO
--rw-r--r--   0 asher      (501) staff       (20)     1249 2021-04-29 16:37:09.000000 toolchain.pants.plugin-0.9.0/src/toolchain.pants.plugin.egg-info/SOURCES.txt
--rw-r--r--   0 asher      (501) staff       (20)        1 2021-04-29 16:37:09.000000 toolchain.pants.plugin-0.9.0/src/toolchain.pants.plugin.egg-info/dependency_links.txt
--rw-r--r--   0 asher      (501) staff       (20)       60 2021-04-29 16:37:09.000000 toolchain.pants.plugin-0.9.0/src/toolchain.pants.plugin.egg-info/entry_points.txt
--rw-r--r--   0 asher      (501) staff       (20)        1 2021-04-29 16:37:09.000000 toolchain.pants.plugin-0.9.0/src/toolchain.pants.plugin.egg-info/namespace_packages.txt
--rw-r--r--   0 asher      (501) staff       (20)       50 2021-04-29 16:37:09.000000 toolchain.pants.plugin-0.9.0/src/toolchain.pants.plugin.egg-info/requires.txt
--rw-r--r--   0 asher      (501) staff       (20)       10 2021-04-29 16:37:09.000000 toolchain.pants.plugin-0.9.0/src/toolchain.pants.plugin.egg-info/top_level.txt
--rw-r--r--   0 asher      (501) staff       (20)        1 2021-04-29 16:37:09.000000 toolchain.pants.plugin-0.9.0/src/toolchain.pants.plugin.egg-info/zip-safe
+drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 22:47:41.972519 toolchain.pants.plugin-0.9.1/
+-rw-r--r--   0 asher      (501) staff       (20)       12 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/MANIFEST.in
+-rw-r--r--   0 asher      (501) staff       (20)     1197 2021-04-29 22:47:41.972196 toolchain.pants.plugin-0.9.1/PKG-INFO
+-rw-r--r--   0 asher      (501) staff       (20)       38 2021-04-29 22:47:41.972631 toolchain.pants.plugin-0.9.1/setup.cfg
+-rw-r--r--   0 asher      (501) staff       (20)     2049 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/setup.py
+drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 22:47:41.957657 toolchain.pants.plugin-0.9.1/src/
+drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 22:47:41.959821 toolchain.pants.plugin-0.9.1/src/toolchain/
+-rw-r--r--   0 asher      (501) staff       (20)        0 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/__init__.py
+drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 22:47:41.963291 toolchain.pants.plugin-0.9.1/src/toolchain/base/
+-rw-r--r--   0 asher      (501) staff       (20)     1480 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/base/datetime_tools.py
+drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 22:47:41.964210 toolchain.pants.plugin-0.9.1/src/toolchain/pants/
+drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 22:47:41.968382 toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/
+-rw-r--r--   0 asher      (501) staff       (20)        0 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/__init__.py
+-rw-r--r--   0 asher      (501) staff       (20)    10938 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/client.py
+-rw-r--r--   0 asher      (501) staff       (20)    51965 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/error.html
+-rw-r--r--   0 asher      (501) staff       (20)     2579 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/favicon.png
+-rw-r--r--   0 asher      (501) staff       (20)     2514 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/plugin.py
+-rw-r--r--   0 asher      (501) staff       (20)      544 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/register.py
+-rw-r--r--   0 asher      (501) staff       (20)    11498 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/rules.py
+-rw-r--r--   0 asher      (501) staff       (20)     5851 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/server.py
+-rw-r--r--   0 asher      (501) staff       (20)     2473 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/store.py
+-rw-r--r--   0 asher      (501) staff       (20)    53298 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/success.html
+drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 22:47:41.970868 toolchain.pants.plugin-0.9.1/src/toolchain/pants/buildsense/
+-rw-r--r--   0 asher      (501) staff       (20)     9452 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/buildsense/client.py
+-rw-r--r--   0 asher      (501) staff       (20)      871 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/buildsense/common.py
+-rw-r--r--   0 asher      (501) staff       (20)    10113 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/buildsense/converter.py
+-rw-r--r--   0 asher      (501) staff       (20)     5807 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/buildsense/local_store.py
+-rw-r--r--   0 asher      (501) staff       (20)    12709 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/buildsense/reporter.py
+-rw-r--r--   0 asher      (501) staff       (20)    10077 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/buildsense/state.py
+drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 22:47:41.971585 toolchain.pants.plugin-0.9.1/src/toolchain/pants/common/
+-rw-r--r--   0 asher      (501) staff       (20)      727 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/common/network.py
+-rw-r--r--   0 asher      (501) staff       (20)     1306 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/common/toolchain_setup.py
+-rw-r--r--   0 asher      (501) staff       (20)      763 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/register.py
+-rw-r--r--   0 asher      (501) staff       (20)      528 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain/pants/version.py
+drwxr-xr-x   0 asher      (501) staff       (20)        0 2021-04-29 22:47:41.962708 toolchain.pants.plugin-0.9.1/src/toolchain.pants.plugin.egg-info/
+-rw-r--r--   0 asher      (501) staff       (20)     1197 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain.pants.plugin.egg-info/PKG-INFO
+-rw-r--r--   0 asher      (501) staff       (20)     1249 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain.pants.plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 asher      (501) staff       (20)        1 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain.pants.plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 asher      (501) staff       (20)       60 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain.pants.plugin.egg-info/entry_points.txt
+-rw-r--r--   0 asher      (501) staff       (20)        1 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain.pants.plugin.egg-info/namespace_packages.txt
+-rw-r--r--   0 asher      (501) staff       (20)       50 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain.pants.plugin.egg-info/requires.txt
+-rw-r--r--   0 asher      (501) staff       (20)       10 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain.pants.plugin.egg-info/top_level.txt
+-rw-r--r--   0 asher      (501) staff       (20)        1 2021-04-29 22:47:41.000000 toolchain.pants.plugin-0.9.1/src/toolchain.pants.plugin.egg-info/zip-safe
```

### Comparing `toolchain.pants.plugin-0.9.0/PKG-INFO` & `toolchain.pants.plugin-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolchain.pants.plugin
-Version: 0.9.0
+Version: 0.9.1
 Summary: Toolchain Pants plugin.
 Home-page: https://toolchain.com
 Author: Toolchain Inc
 Author-email: info@toolchain.com
 License: Proprietary
 Description: # Toolchain Pants plugin
```

### Comparing `toolchain.pants.plugin-0.9.0/setup.py` & `toolchain.pants.plugin-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 Speed up your builds dramatically through shared execution and caching.
 View and search your team's entire build history. Use data to find
 bottlenecks and optimize your development cycle.
 """,
     'long_description_content_type': 'text/markdown',
     'name': 'toolchain.pants.plugin',
     'url': 'https://toolchain.com',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'zip_safe': True,
     'package_dir': {
         '': 'src',
     },
     'packages': (
         'toolchain',
         'toolchain.base',
```

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/base/datetime_tools.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/base/datetime_tools.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/client.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,17 +217,19 @@
         # TODO build a better string/error message
         errors = resp_json.get("errors") or "N/A"
         raise AuthError(f"API Errors: {errors}", request_id=request_id, server_failure=True)
 
     def _should_disable(self, complete_env: Mapping[str, str]) -> bool:
         for env_var, expression in self.restricted_token_matches.items():
             if env_var not in complete_env:
+                _logger.debug(f"{env_var} not in env: {complete_env.keys()}")
                 return True
-            if not re.match(expression, complete_env[env_var]):
-                return True
+            match = re.match(expression, complete_env[env_var]) is not None
+            _logger.debug(f"expression match={match} for {env_var}: expected={expression}  got={complete_env[env_var]}")
+            return not match
         return False
 
     def _load_refresh_token(self, complete_env: Mapping[str, str]) -> Optional[AuthToken]:
         if self.env_var:
             token = _load_from_env(complete_env, self.env_var)
             if token:
                 return token
```

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/error.html` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/error.html`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/favicon.png` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/favicon.png`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/plugin.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/plugin.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/register.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/register.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/rules.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/rules.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/server.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/server.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/store.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/store.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/auth/success.html` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/auth/success.html`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/buildsense/client.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/buildsense/client.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/buildsense/common.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/buildsense/common.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/buildsense/converter.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/buildsense/converter.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/buildsense/local_store.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/buildsense/local_store.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/buildsense/reporter.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/buildsense/reporter.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/buildsense/state.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/buildsense/state.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/common/network.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/common/network.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/common/toolchain_setup.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/common/toolchain_setup.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/register.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/register.py`

 * *Files identical despite different names*

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain/pants/version.py` & `toolchain.pants.plugin-0.9.1/src/toolchain/pants/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,8 +4,8 @@
 #
 # This file includes unpublished proprietary source code of Toolchain Labs, Inc.
 # The copyright notice above does not evidence any actual or intended publication of such source code.
 # Disclosure of this source code or any related proprietary information is strictly prohibited without
 # the express written permission of Toolchain Labs, Inc.
 
 # The version to use when publishing artifacts from this repo.
-VERSION = "0.9.0"
+VERSION = "0.9.1"
```

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain.pants.plugin.egg-info/PKG-INFO` & `toolchain.pants.plugin-0.9.1/src/toolchain.pants.plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolchain.pants.plugin
-Version: 0.9.0
+Version: 0.9.1
 Summary: Toolchain Pants plugin.
 Home-page: https://toolchain.com
 Author: Toolchain Inc
 Author-email: info@toolchain.com
 License: Proprietary
 Description: # Toolchain Pants plugin
```

### Comparing `toolchain.pants.plugin-0.9.0/src/toolchain.pants.plugin.egg-info/SOURCES.txt` & `toolchain.pants.plugin-0.9.1/src/toolchain.pants.plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

