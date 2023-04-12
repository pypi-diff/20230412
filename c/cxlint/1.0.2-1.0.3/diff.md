# Comparing `tmp/cxlint-1.0.2.tar.gz` & `tmp/cxlint-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/pmarlow/eng/cxlint/dist/tmpyrhx8bfa/cxlint-1.0.2.tar", last modified: Wed Apr 12 02:57:34 2023, max compression
+gzip compressed data, was "/Users/pmarlow/eng/cxlint/dist/tmppx_0w9t4/cxlint-1.0.3.tar", last modified: Wed Apr 12 03:06:04 2023, max compression
```

## Comparing `cxlint-1.0.2.tar` & `cxlint-1.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 02:57:34.000000 cxlint-1.0.2/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3835 2023-04-12 02:57:34.000000 cxlint-1.0.2/PKG-INFO
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2978 2023-04-12 01:31:40.000000 cxlint-1.0.2/README.md
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1753 2023-04-12 02:57:08.000000 cxlint-1.0.2/setup.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       78 2023-04-12 02:57:34.000000 cxlint-1.0.2/setup.cfg
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11357 2023-03-01 20:47:23.000000 cxlint-1.0.2/LICENSE.txt
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 02:57:34.000000 cxlint-1.0.2/src/
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 02:57:34.000000 cxlint-1.0.2/src/cxlint/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8160 2023-04-12 02:56:48.000000 cxlint-1.0.2/src/cxlint/cxlint.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 02:57:34.000000 cxlint-1.0.2/src/cxlint/resources/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3441 2023-04-12 02:20:03.000000 cxlint-1.0.2/src/cxlint/resources/route_groups.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8793 2023-04-12 02:19:51.000000 cxlint-1.0.2/src/cxlint/resources/intents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6180 2023-04-12 02:19:29.000000 cxlint-1.0.2/src/cxlint/resources/entity_types.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2023-01-26 14:31:21.000000 cxlint-1.0.2/src/cxlint/resources/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7029 2023-04-12 02:20:20.000000 cxlint-1.0.2/src/cxlint/resources/types.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1348 2023-04-12 02:19:17.000000 cxlint-1.0.2/src/cxlint/resources/agents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5978 2023-04-12 02:19:59.000000 cxlint-1.0.2/src/cxlint/resources/pages.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    13432 2023-04-12 02:19:45.000000 cxlint-1.0.2/src/cxlint/resources/flows.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4160 2023-04-12 02:20:25.000000 cxlint-1.0.2/src/cxlint/resources/webhooks.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9825 2023-04-12 02:20:16.000000 cxlint-1.0.2/src/cxlint/resources/test_cases.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10560 2023-04-12 02:20:10.000000 cxlint-1.0.2/src/cxlint/resources/routes.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1420 2023-03-02 21:47:37.000000 cxlint-1.0.2/src/cxlint/graph.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2023-01-09 15:34:14.000000 cxlint-1.0.2/src/cxlint/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7541 2023-04-12 02:17:45.000000 cxlint-1.0.2/src/cxlint/common.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 02:57:34.000000 cxlint-1.0.2/src/cxlint/rules/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10503 2023-04-12 02:22:04.000000 cxlint-1.0.2/src/cxlint/rules/intents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6783 2023-04-12 02:21:53.000000 cxlint-1.0.2/src/cxlint/rules/entity_types.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2023-03-15 21:40:16.000000 cxlint-1.0.2/src/cxlint/rules/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2804 2023-04-12 02:20:42.000000 cxlint-1.0.2/src/cxlint/rules/logger.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8607 2023-04-12 02:21:44.000000 cxlint-1.0.2/src/cxlint/rules/pages.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6155 2023-04-12 02:21:30.000000 cxlint-1.0.2/src/cxlint/rules/flows.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2301 2023-04-12 02:22:14.000000 cxlint-1.0.2/src/cxlint/rules/webhooks.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5370 2023-04-12 02:20:52.000000 cxlint-1.0.2/src/cxlint/rules/response_messages.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4437 2023-04-12 02:20:58.000000 cxlint-1.0.2/src/cxlint/rules/test_cases.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2277 2023-03-02 21:47:37.000000 cxlint-1.0.2/src/cxlint/gcs_utils.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 02:57:34.000000 cxlint-1.0.2/src/cxlint.egg-info/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3835 2023-04-12 02:57:34.000000 cxlint-1.0.2/src/cxlint.egg-info/PKG-INFO
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      911 2023-04-12 02:57:34.000000 cxlint-1.0.2/src/cxlint.egg-info/SOURCES.txt
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        7 2023-04-12 02:57:34.000000 cxlint-1.0.2/src/cxlint.egg-info/top_level.txt
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        1 2023-04-12 02:57:34.000000 cxlint-1.0.2/src/cxlint.egg-info/dependency_links.txt
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:06:04.000000 cxlint-1.0.3/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3835 2023-04-12 03:06:04.000000 cxlint-1.0.3/PKG-INFO
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2978 2023-04-12 01:31:40.000000 cxlint-1.0.3/README.md
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1753 2023-04-12 03:05:33.000000 cxlint-1.0.3/setup.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       78 2023-04-12 03:06:04.000000 cxlint-1.0.3/setup.cfg
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11357 2023-03-01 20:47:23.000000 cxlint-1.0.3/LICENSE.txt
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8160 2023-04-12 03:05:27.000000 cxlint-1.0.3/src/cxlint/cxlint.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint/resources/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3441 2023-04-12 02:20:03.000000 cxlint-1.0.3/src/cxlint/resources/route_groups.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8793 2023-04-12 02:19:51.000000 cxlint-1.0.3/src/cxlint/resources/intents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6180 2023-04-12 02:19:29.000000 cxlint-1.0.3/src/cxlint/resources/entity_types.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2023-01-26 14:31:21.000000 cxlint-1.0.3/src/cxlint/resources/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7029 2023-04-12 02:20:20.000000 cxlint-1.0.3/src/cxlint/resources/types.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1348 2023-04-12 02:19:17.000000 cxlint-1.0.3/src/cxlint/resources/agents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5978 2023-04-12 02:19:59.000000 cxlint-1.0.3/src/cxlint/resources/pages.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    13432 2023-04-12 02:19:45.000000 cxlint-1.0.3/src/cxlint/resources/flows.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4160 2023-04-12 02:20:25.000000 cxlint-1.0.3/src/cxlint/resources/webhooks.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9825 2023-04-12 02:20:16.000000 cxlint-1.0.3/src/cxlint/resources/test_cases.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10560 2023-04-12 02:20:10.000000 cxlint-1.0.3/src/cxlint/resources/routes.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1420 2023-03-02 21:47:37.000000 cxlint-1.0.3/src/cxlint/graph.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2023-01-09 15:34:14.000000 cxlint-1.0.3/src/cxlint/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7541 2023-04-12 02:17:45.000000 cxlint-1.0.3/src/cxlint/common.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint/rules/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10503 2023-04-12 02:22:04.000000 cxlint-1.0.3/src/cxlint/rules/intents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6783 2023-04-12 02:21:53.000000 cxlint-1.0.3/src/cxlint/rules/entity_types.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2023-03-15 21:40:16.000000 cxlint-1.0.3/src/cxlint/rules/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2804 2023-04-12 02:20:42.000000 cxlint-1.0.3/src/cxlint/rules/logger.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8607 2023-04-12 02:21:44.000000 cxlint-1.0.3/src/cxlint/rules/pages.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6155 2023-04-12 02:21:30.000000 cxlint-1.0.3/src/cxlint/rules/flows.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2301 2023-04-12 02:22:14.000000 cxlint-1.0.3/src/cxlint/rules/webhooks.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5370 2023-04-12 02:20:52.000000 cxlint-1.0.3/src/cxlint/rules/response_messages.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4437 2023-04-12 02:20:58.000000 cxlint-1.0.3/src/cxlint/rules/test_cases.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2277 2023-03-02 21:47:37.000000 cxlint-1.0.3/src/cxlint/gcs_utils.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint.egg-info/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3835 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint.egg-info/PKG-INFO
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      911 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint.egg-info/SOURCES.txt
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        7 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint.egg-info/top_level.txt
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        1 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint.egg-info/dependency_links.txt
```

### Comparing `cxlint-1.0.2/PKG-INFO` & `cxlint-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxlint
-Version: 1.0.2
+Version: 1.0.3
 Summary: A static code analyzer that provides automated quality       control for Dialogflow CX Agents
 Home-page: https://github.com/GoogleCloudPlatform/cxlint
 Author: Patrick Marlow
 Author-email: pmarlow@google.com
 License: UNKNOWN
 Keywords: dialogflow,cx,google,bot,chatbot,linter,dfcx
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cxlint Version: 1.0.2 Summary: A static code
+Metadata-Version: 2.1 Name: cxlint Version: 1.0.3 Summary: A static code
 analyzer that provides automated quality control for Dialogflow CX Agents Home-
 page: https://github.com/GoogleCloudPlatform/cxlint Author: Patrick Marlow
 Author-email: pmarlow@google.com License: UNKNOWN Keywords:
 dialogflow,cx,google,bot,chatbot,linter,dfcx Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Communications :: Chat Classifier: Topic ::
```

### Comparing `cxlint-1.0.2/README.md` & `cxlint-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/setup.py` & `cxlint-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='cxlint',
-    version='1.0.2',
+    version='1.0.3',
     description='A static code analyzer that provides automated quality \
       control for Dialogflow CX Agents',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/GoogleCloudPlatform/cxlint',
     author='Patrick Marlow',
     author_email='pmarlow@google.com',
```

### Comparing `cxlint-1.0.2/LICENSE.txt` & `cxlint-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/cxlint.py` & `cxlint-1.0.3/src/cxlint/cxlint.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/resources/route_groups.py` & `cxlint-1.0.3/src/cxlint/resources/route_groups.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/resources/intents.py` & `cxlint-1.0.3/src/cxlint/resources/intents.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/resources/entity_types.py` & `cxlint-1.0.3/src/cxlint/resources/entity_types.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/resources/types.py` & `cxlint-1.0.3/src/cxlint/resources/types.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/resources/agents.py` & `cxlint-1.0.3/src/cxlint/resources/agents.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/resources/pages.py` & `cxlint-1.0.3/src/cxlint/resources/pages.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/resources/flows.py` & `cxlint-1.0.3/src/cxlint/resources/flows.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/resources/webhooks.py` & `cxlint-1.0.3/src/cxlint/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/resources/test_cases.py` & `cxlint-1.0.3/src/cxlint/resources/test_cases.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/resources/routes.py` & `cxlint-1.0.3/src/cxlint/resources/routes.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/graph.py` & `cxlint-1.0.3/src/cxlint/graph.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/common.py` & `cxlint-1.0.3/src/cxlint/common.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/rules/intents.py` & `cxlint-1.0.3/src/cxlint/rules/intents.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/rules/entity_types.py` & `cxlint-1.0.3/src/cxlint/rules/entity_types.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/rules/logger.py` & `cxlint-1.0.3/src/cxlint/rules/logger.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/rules/pages.py` & `cxlint-1.0.3/src/cxlint/rules/pages.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/rules/flows.py` & `cxlint-1.0.3/src/cxlint/rules/flows.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/rules/webhooks.py` & `cxlint-1.0.3/src/cxlint/rules/webhooks.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/rules/response_messages.py` & `cxlint-1.0.3/src/cxlint/rules/response_messages.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/rules/test_cases.py` & `cxlint-1.0.3/src/cxlint/rules/test_cases.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint/gcs_utils.py` & `cxlint-1.0.3/src/cxlint/gcs_utils.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.2/src/cxlint.egg-info/PKG-INFO` & `cxlint-1.0.3/src/cxlint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxlint
-Version: 1.0.2
+Version: 1.0.3
 Summary: A static code analyzer that provides automated quality       control for Dialogflow CX Agents
 Home-page: https://github.com/GoogleCloudPlatform/cxlint
 Author: Patrick Marlow
 Author-email: pmarlow@google.com
 License: UNKNOWN
 Keywords: dialogflow,cx,google,bot,chatbot,linter,dfcx
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cxlint Version: 1.0.2 Summary: A static code
+Metadata-Version: 2.1 Name: cxlint Version: 1.0.3 Summary: A static code
 analyzer that provides automated quality control for Dialogflow CX Agents Home-
 page: https://github.com/GoogleCloudPlatform/cxlint Author: Patrick Marlow
 Author-email: pmarlow@google.com License: UNKNOWN Keywords:
 dialogflow,cx,google,bot,chatbot,linter,dfcx Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Communications :: Chat Classifier: Topic ::
```

### Comparing `cxlint-1.0.2/src/cxlint.egg-info/SOURCES.txt` & `cxlint-1.0.3/src/cxlint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

