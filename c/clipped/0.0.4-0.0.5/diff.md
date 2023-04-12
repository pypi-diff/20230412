# Comparing `tmp/clipped-0.0.4.tar.gz` & `tmp/clipped-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipped-0.0.4.tar", last modified: Tue Apr 11 19:09:48 2023, max compression
+gzip compressed data, was "clipped-0.0.5.tar", last modified: Wed Apr 12 15:59:28 2023, max compression
```

## Comparing `clipped-0.0.4.tar` & `clipped-0.0.5.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-11 19:09:48.442724 clipped-0.0.4/
--rw-r--r--   0 mourad     (501) staff       (20)      174 2023-04-11 19:09:05.000000 clipped-0.0.4/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-11 19:09:48.442838 clipped-0.0.4/PKG-INFO
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-11 19:09:48.441827 clipped-0.0.4/clipped/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/bool_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/cached_property.py
--rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/click_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/cmd.py
--rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/coroutine.py
--rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/csv_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/date_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     4349 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/deprecated_decorators.py
--rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/dict_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/encoding.py
--rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/enums_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     1995 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/env.py
--rw-r--r--   0 mourad     (501) staff       (20)     6222 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/formatting.py
--rw-r--r--   0 mourad     (501) staff       (20)     4731 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/git_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     1825 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/hashing.py
--rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/http_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     3367 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/humanize.py
--rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/imports.py
--rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/indentation.py
--rw-r--r--   0 mourad     (501) staff       (20)      442 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/json_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      894 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/list_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/logging_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/manager_interface.py
--rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/memoize_decorators.py
--rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/np_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     8482 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/path_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/pkg.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/py.typed
--rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/query_params.py
--rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/requests_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/response_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      559 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/sanitizers.py
--rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/serialization.py
--rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/signal_decorators.py
--rw-r--r--   0 mourad     (501) staff       (20)     2339 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/string_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/tz_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/units_processors.py
--rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/urls_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      613 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/validation.py
--rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/versions.py
--rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/workers_utils.py
--rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-11 19:09:05.000000 clipped-0.0.4/clipped/yaml_utils.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-11 19:09:48.442567 clipped-0.0.4/clipped.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     2012 2023-04-11 19:09:48.000000 clipped-0.0.4/clipped.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1164 2023-04-11 19:09:48.000000 clipped-0.0.4/clipped.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-11 19:09:48.000000 clipped-0.0.4/clipped.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-11 19:09:48.000000 clipped-0.0.4/clipped.egg-info/top_level.txt
--rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-11 19:09:48.443381 clipped-0.0.4/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-11 19:09:05.000000 clipped-0.0.4/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-12 15:59:28.127670 clipped-0.0.5/
+-rw-r--r--   0 mourad     (501) staff       (20)       60 2023-04-12 15:56:47.000000 clipped-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 mourad     (501) staff       (20)    11351 2023-04-12 15:56:47.000000 clipped-0.0.5/LICENSE
+-rw-r--r--   0 mourad     (501) staff       (20)      165 2023-04-12 15:56:47.000000 clipped-0.0.5/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     1482 2023-04-12 15:59:28.127741 clipped-0.0.5/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)      551 2023-04-12 15:56:47.000000 clipped-0.0.5/README.md
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-12 15:59:28.127054 clipped-0.0.5/clipped/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1004 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/bool_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      646 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/cached_property.py
+-rw-r--r--   0 mourad     (501) staff       (20)      143 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/click_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      665 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/cmd.py
+-rw-r--r--   0 mourad     (501) staff       (20)      570 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/coroutine.py
+-rw-r--r--   0 mourad     (501) staff       (20)      755 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/csv_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     7568 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/date_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4349 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/deprecated_decorators.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3354 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/dict_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      496 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/encoding.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1093 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/enums_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1995 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/env.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6222 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/formatting.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4731 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/git_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1825 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/hashing.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1175 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/http_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3367 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/humanize.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1327 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/imports.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1695 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/indentation.py
+-rw-r--r--   0 mourad     (501) staff       (20)      287 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/json_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      894 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/list_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      113 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/logging_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      824 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/manager_interface.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1923 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/memoize_decorators.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1280 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/np_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     8482 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/path_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      203 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/pkg.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/py.typed
+-rw-r--r--   0 mourad     (501) staff       (20)      674 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/query_params.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1134 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/requests_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1041 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/response_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      559 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/sanitizers.py
+-rw-r--r--   0 mourad     (501) staff       (20)      676 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/serialization.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2686 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/signal_decorators.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2339 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/string_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1115 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/tz_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4040 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/units_processors.py
+-rw-r--r--   0 mourad     (501) staff       (20)      269 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/urls_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      613 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/validation.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1128 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/versions.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1068 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/workers_utils.py
+-rw-r--r--   0 mourad     (501) staff       (20)      546 2023-04-12 15:56:47.000000 clipped-0.0.5/clipped/yaml_utils.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-12 15:59:28.127522 clipped-0.0.5/clipped.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     1482 2023-04-12 15:59:28.000000 clipped-0.0.5/clipped.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1155 2023-04-12 15:59:28.000000 clipped-0.0.5/clipped.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-12 15:59:28.000000 clipped-0.0.5/clipped.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        8 2023-04-12 15:59:28.000000 clipped-0.0.5/clipped.egg-info/top_level.txt
+-rw-r--r--   0 mourad     (501) staff       (20)     1033 2023-04-12 15:59:28.128131 clipped-0.0.5/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2345 2023-04-12 15:56:47.000000 clipped-0.0.5/setup.py
```

### Comparing `clipped-0.0.4/clipped/bool_utils.py` & `clipped-0.0.5/clipped/bool_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/cached_property.py` & `clipped-0.0.5/clipped/cached_property.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/cmd.py` & `clipped-0.0.5/clipped/cmd.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/coroutine.py` & `clipped-0.0.5/clipped/coroutine.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/csv_utils.py` & `clipped-0.0.5/clipped/csv_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/date_utils.py` & `clipped-0.0.5/clipped/date_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/deprecated_decorators.py` & `clipped-0.0.5/clipped/deprecated_decorators.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/dict_utils.py` & `clipped-0.0.5/clipped/dict_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/enums_utils.py` & `clipped-0.0.5/clipped/enums_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/env.py` & `clipped-0.0.5/clipped/env.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/formatting.py` & `clipped-0.0.5/clipped/formatting.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/git_utils.py` & `clipped-0.0.5/clipped/git_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/hashing.py` & `clipped-0.0.5/clipped/hashing.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/http_utils.py` & `clipped-0.0.5/clipped/http_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/humanize.py` & `clipped-0.0.5/clipped/humanize.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/imports.py` & `clipped-0.0.5/clipped/imports.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/indentation.py` & `clipped-0.0.5/clipped/indentation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/list_utils.py` & `clipped-0.0.5/clipped/list_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/manager_interface.py` & `clipped-0.0.5/clipped/manager_interface.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/memoize_decorators.py` & `clipped-0.0.5/clipped/memoize_decorators.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/np_utils.py` & `clipped-0.0.5/clipped/np_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/path_utils.py` & `clipped-0.0.5/clipped/path_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/query_params.py` & `clipped-0.0.5/clipped/query_params.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/requests_utils.py` & `clipped-0.0.5/clipped/requests_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/response_utils.py` & `clipped-0.0.5/clipped/response_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/sanitizers.py` & `clipped-0.0.5/clipped/sanitizers.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/serialization.py` & `clipped-0.0.5/clipped/serialization.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/signal_decorators.py` & `clipped-0.0.5/clipped/signal_decorators.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/string_utils.py` & `clipped-0.0.5/clipped/string_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/tz_utils.py` & `clipped-0.0.5/clipped/tz_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/units_processors.py` & `clipped-0.0.5/clipped/units_processors.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/validation.py` & `clipped-0.0.5/clipped/validation.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/versions.py` & `clipped-0.0.5/clipped/versions.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/workers_utils.py` & `clipped-0.0.5/clipped/workers_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped/yaml_utils.py` & `clipped-0.0.5/clipped/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/clipped.egg-info/SOURCES.txt` & `clipped-0.0.5/clipped.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+CONTRIBUTING.md
+LICENSE
 MANIFEST.in
+README.md
 setup.cfg
 setup.py
-../CONTRIBUTING.md
-../LICENSE
-../README.md
 clipped/__init__.py
 clipped/bool_utils.py
 clipped/cached_property.py
 clipped/click_utils.py
 clipped/cmd.py
 clipped/coroutine.py
 clipped/csv_utils.py
```

### Comparing `clipped-0.0.4/setup.cfg` & `clipped-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `clipped-0.0.4/setup.py` & `clipped-0.0.5/setup.py`

 * *Files identical despite different names*

