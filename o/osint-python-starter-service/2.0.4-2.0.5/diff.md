# Comparing `tmp/osint-python-starter-service-2.0.4.tar.gz` & `tmp/osint-python-starter-service-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-starter-service-2.0.4.tar", last modified: Wed Apr 12 13:18:24 2023, max compression
+gzip compressed data, was "osint-python-starter-service-2.0.5.tar", last modified: Wed Apr 12 13:50:00 2023, max compression
```

## Comparing `osint-python-starter-service-2.0.4.tar` & `osint-python-starter-service-2.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:18:24.833377 osint-python-starter-service-2.0.4/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.4/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-12 13:18:24.830044 osint-python-starter-service-2.0.4/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1713 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.4/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:18:24.830044 osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-12 13:18:24.000000 osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      874 2023-04-12 13:18:24.000000 osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-12 13:18:24.000000 osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-04-12 13:18:24.000000 osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-04-12 13:18:24.000000 osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-12 13:18:24.833377 osint-python-starter-service-2.0.4/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-04-12 13:16:20.000000 osint-python-starter-service-2.0.4/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:18:24.830044 osint-python-starter-service-2.0.4/starter_service/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.4/starter_service/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.4/starter_service/api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6814 2023-04-12 12:36:49.000000 osint-python-starter-service-2.0.4/starter_service/api_server.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4731 2023-04-06 18:13:23.000000 osint-python-starter-service-2.0.4/starter_service/avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2980 2023-04-12 13:10:08.000000 osint-python-starter-service-2.0.4/starter_service/base_service.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1275 2023-04-04 14:58:16.000000 osint-python-starter-service-2.0.4/starter_service/env.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:18:24.830044 osint-python-starter-service-2.0.4/starter_service/examples/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.4/starter_service/examples/__init__.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:18:24.830044 osint-python-starter-service-2.0.4/starter_service/examples/classes/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.4/starter_service/examples/classes/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2569 2023-04-12 13:08:09.000000 osint-python-starter-service-2.0.4/starter_service/examples/classes/article_raw_en.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      637 2023-04-12 13:08:09.000000 osint-python-starter-service-2.0.4/starter_service/examples/classes/metadata_item_key_en.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      708 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.4/starter_service/examples/error.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      912 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.4/starter_service/examples/manual_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1298 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.4/starter_service/examples/multi.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1047 2023-04-12 13:12:02.000000 osint-python-starter-service-2.0.4/starter_service/examples/single.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6887 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.4/starter_service/kafka_adapter.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.4/starter_service/messages.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6406 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.4/starter_service/schemas.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.5/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1713 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.5/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-12 13:50:00.000000 osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      874 2023-04-12 13:50:00.000000 osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-12 13:50:00.000000 osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-04-12 13:50:00.000000 osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-04-12 13:50:00.000000 osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-04-12 13:49:34.000000 osint-python-starter-service-2.0.5/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/starter_service/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.5/starter_service/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.5/starter_service/api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6814 2023-04-12 12:36:49.000000 osint-python-starter-service-2.0.5/starter_service/api_server.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4731 2023-04-06 18:13:23.000000 osint-python-starter-service-2.0.5/starter_service/avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2980 2023-04-12 13:10:08.000000 osint-python-starter-service-2.0.5/starter_service/base_service.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1274 2023-04-12 13:48:58.000000 osint-python-starter-service-2.0.5/starter_service/env.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/starter_service/examples/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.5/starter_service/examples/__init__.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:50:00.921250 osint-python-starter-service-2.0.5/starter_service/examples/classes/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.5/starter_service/examples/classes/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2569 2023-04-12 13:43:03.000000 osint-python-starter-service-2.0.5/starter_service/examples/classes/article_raw_en.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      637 2023-04-12 13:43:03.000000 osint-python-starter-service-2.0.5/starter_service/examples/classes/metadata_item_key_en.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      708 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.5/starter_service/examples/error.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      912 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.5/starter_service/examples/manual_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1298 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.5/starter_service/examples/multi.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1047 2023-04-12 13:49:22.000000 osint-python-starter-service-2.0.5/starter_service/examples/single.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6887 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.5/starter_service/kafka_adapter.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.5/starter_service/messages.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6239 2023-04-12 13:42:48.000000 osint-python-starter-service-2.0.5/starter_service/schemas.py
```

### Comparing `osint-python-starter-service-2.0.4/LICENSE` & `osint-python-starter-service-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/PKG-INFO` & `osint-python-starter-service-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.0.4/README.md` & `osint-python-starter-service-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/PKG-INFO` & `osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/SOURCES.txt` & `osint-python-starter-service-2.0.5/osint_python_starter_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/setup.py` & `osint-python-starter-service-2.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 setuptools.setup(
     name="osint-python-starter-service",
-    version="2.0.4",
+    version="2.0.5",
     author="mindpetk",
     author_email="petkeviciusm@gmail.com",
     description="Python starter service",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-starter-service",
     include_package_data=True,
```

### Comparing `osint-python-starter-service-2.0.4/starter_service/api.py` & `osint-python-starter-service-2.0.5/starter_service/api.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/starter_service/api_server.py` & `osint-python-starter-service-2.0.5/starter_service/api_server.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/starter_service/avro_parser.py` & `osint-python-starter-service-2.0.5/starter_service/avro_parser.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/starter_service/base_service.py` & `osint-python-starter-service-2.0.5/starter_service/base_service.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/starter_service/env.py` & `osint-python-starter-service-2.0.5/starter_service/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     PARTITIONER = _env("PARTITIONER", "random")
     MESSAGE_MAX_BYTES = _env.int('MESSAGE_MAX_BYTES', 1000000)
     HEARTBEAT_INTERVAL = _env.int('HEARTBEAT_INTERVAL', 10)
     OFFSET_TYPE = _env('OFFSET_TYPE', 'earliest')
     STRING_BASED_KEYS = _env.bool('STRING_BASED_KEYS', True)
 
     # REST API
-    REST_API_ENABLED = _env.bool('REST_API_ENABLED', False)
+    REST_API_ENABLED = _env.bool('REST_API_ENABLED', True)
     REST_API_PORT = _env.int('REST_API_PORT', 8080)
     REST_API_HOST = _env('REST_API_HOST', '0.0.0.0')
     REST_LOG_MESSAGES = _env.bool('REST_LOG_MESSAGES', False)
 
     # OTHER
     LOCAL_SCHEMA_REGISTRY_ENABLED = _env.bool('LOCAL_SCHEMA_REGISTRY_ENABLED', True)
```

### Comparing `osint-python-starter-service-2.0.4/starter_service/examples/classes/article_raw_en.py` & `osint-python-starter-service-2.0.5/starter_service/examples/classes/article_raw_en.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/starter_service/examples/classes/metadata_item_key_en.py` & `osint-python-starter-service-2.0.5/starter_service/examples/classes/metadata_item_key_en.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/starter_service/examples/error.py` & `osint-python-starter-service-2.0.5/starter_service/examples/error.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/starter_service/examples/manual_kafka.py` & `osint-python-starter-service-2.0.5/starter_service/examples/manual_kafka.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/starter_service/examples/multi.py` & `osint-python-starter-service-2.0.5/starter_service/examples/multi.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/starter_service/examples/single.py` & `osint-python-starter-service-2.0.5/starter_service/examples/single.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/starter_service/kafka_adapter.py` & `osint-python-starter-service-2.0.5/starter_service/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/starter_service/messages.py` & `osint-python-starter-service-2.0.5/starter_service/messages.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.4/starter_service/schemas.py` & `osint-python-starter-service-2.0.5/starter_service/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,45 +24,40 @@
         return f"{self.class_name} from {self.filename}"
 
     def __repr__(self):
         return f"{self.class_name} from {self.filename}"
 
 
 class SchemaRegistry:
-    _instance = None
     _lock = Lock()
+    _instance = None
+    _logger = logging.getLogger(__name__)
+
+    _schemas = {}
+    _classes = {}
 
     def __new__(self):
         with self._lock:
             if self._instance is None:
                 self._instance = super().__new__(self)
         return self._instance
 
-    def __init__(self):
-        self._logger = logging.getLogger(__name__)
-        self._initialized = False
-        self._schemas = {}
-        self._classes = {}
-
     def get_schemas(self):
         return self._schemas
 
     def get_schemas_dict(self):
         return {schema.topic: schema.class_name for class_name, schema in self._schemas.items()}
 
     def initialize(self):
-        if self._initialized:
-            return
         # create schema folder if not exists
         self._init_dir()
         # load schemas from folder
         self._load_local_schemas()
         # load classes from folder
         self._load_local_classes()
-        self._initialized = True
 
     def _load_local_schemas(self):
         # load avro schemas from local folder
         _schemas = []
         for file in os.listdir(f"{_path}/schemas"):
             if file.endswith(".avsc") or file.endswith("-value.avsc") or file.endswith("-key.avsc"):
                 _schemas.append(file)
```

