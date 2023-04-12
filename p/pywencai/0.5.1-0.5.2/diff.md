# Comparing `tmp/pywencai-0.5.1.tar.gz` & `tmp/pywencai-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywencai-0.5.1.tar", max compression
+gzip compressed data, was "pywencai-0.5.2.tar", max compression
```

## Comparing `pywencai-0.5.1.tar` & `pywencai-0.5.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-04-06 13:05:04.130357 pywencai-0.5.1/LICENSE
--rw-r--r--   0        0        0     1814 2023-04-06 13:05:04.130357 pywencai-0.5.1/README.md
--rw-r--r--   0        0        0      516 2023-04-06 13:05:04.134357 pywencai-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       23 2023-04-06 13:05:04.134357 pywencai-0.5.1/pywencai/__init__.py
--rw-r--r--   0        0        0    39677 2023-04-06 13:05:04.134357 pywencai-0.5.1/pywencai/hexin-v.js
--rw-r--r--   0        0        0     3964 2023-04-06 13:05:04.134357 pywencai-0.5.1/pywencai/wencai.py
--rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 pywencai-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-12 14:50:10.237392 pywencai-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1814 2023-04-12 14:50:10.237392 pywencai-0.5.2/README.md
+-rw-r--r--   0        0        0      516 2023-04-12 14:50:10.241392 pywencai-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-04-12 14:50:10.241392 pywencai-0.5.2/pywencai/__init__.py
+-rw-r--r--   0        0        0    39677 2023-04-12 14:50:10.241392 pywencai-0.5.2/pywencai/hexin-v.js
+-rw-r--r--   0        0        0     4049 2023-04-12 14:50:10.241392 pywencai-0.5.2/pywencai/wencai.py
+-rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 pywencai-0.5.2/PKG-INFO
```

### Comparing `pywencai-0.5.1/LICENSE` & `pywencai-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywencai-0.5.1/README.md` & `pywencai-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pywencai-0.5.1/pyproject.toml` & `pywencai-0.5.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywencai"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 authors = ["pluto <mayuanchi1029@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
```

### Comparing `pywencai-0.5.1/pywencai/hexin-v.js` & `pywencai-0.5.2/pywencai/hexin-v.js`

 * *Files identical despite different names*

### Comparing `pywencai-0.5.1/pywencai/wencai.py` & `pywencai-0.5.2/pywencai/wencai.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,20 @@
 
 # 获取condition
 def getCondition(**kwargs):
   retry = kwargs.get('retry', 10)
   sleep = kwargs.get('sleep', 0)
   question = kwargs.get('query')
   log = kwargs.get('log', False)
+  query_type = kwargs.get('query_type', 'stock')
   data = {
     'perpage': 10,
     'page': 1,
     'source': 'Ths_iwencai_Xuangu',
+    'secondary_intent': query_type,
     'question': question
   }
 
   count = 0
   log and logging.info(f'获取condition开始')
 
   while count < retry :
@@ -64,19 +66,19 @@
     }
     return key_map.get(key, key)
 
 # 获取comp_id和uuid
 def getIds(query_type):
   ids_map = {
     'stock': {
-      'comp_id': 6623802,
+      'comp_id': 6729244,
       'uuid': 24087
     },
     'zhishu': {
-      'comp_id': 5473251,
+      'comp_id': 6367801,
       'uuid': 24089
     },
     'fund': {
       'comp_id': 6546054,
       'uuid': 24088
     },
     'hkstock': {
```

### Comparing `pywencai-0.5.1/PKG-INFO` & `pywencai-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywencai
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

