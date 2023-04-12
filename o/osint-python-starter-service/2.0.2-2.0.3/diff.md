# Comparing `tmp/osint-python-starter-service-2.0.2.tar.gz` & `tmp/osint-python-starter-service-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-starter-service-2.0.2.tar", last modified: Fri Apr  7 12:41:23 2023, max compression
+gzip compressed data, was "osint-python-starter-service-2.0.3.tar", last modified: Wed Apr 12 12:38:30 2023, max compression
```

## Comparing `osint-python-starter-service-2.0.2.tar` & `osint-python-starter-service-2.0.3.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-07 12:41:23.670373 osint-python-starter-service-2.0.2/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.2/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2173 2023-04-07 12:41:23.670373 osint-python-starter-service-2.0.2/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1702 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.2/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-07 12:41:23.670373 osint-python-starter-service-2.0.2/osint_python_starter_service.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2173 2023-04-07 12:41:23.000000 osint-python-starter-service-2.0.2/osint_python_starter_service.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      745 2023-04-07 12:41:23.000000 osint-python-starter-service-2.0.2/osint_python_starter_service.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-07 12:41:23.000000 osint-python-starter-service-2.0.2/osint_python_starter_service.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-04-07 12:41:23.000000 osint-python-starter-service-2.0.2/osint_python_starter_service.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-04-07 12:41:23.000000 osint-python-starter-service-2.0.2/osint_python_starter_service.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-07 12:41:23.670373 osint-python-starter-service-2.0.2/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-04-07 12:40:14.000000 osint-python-starter-service-2.0.2/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-07 12:41:23.670373 osint-python-starter-service-2.0.2/starter_service/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.2/starter_service/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      177 2023-04-07 11:36:44.000000 osint-python-starter-service-2.0.2/starter_service/aaaa.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.2/starter_service/api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6814 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.2/starter_service/api_server.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4731 2023-04-06 18:13:23.000000 osint-python-starter-service-2.0.2/starter_service/avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2767 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.2/starter_service/base_service.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1275 2023-04-04 14:58:16.000000 osint-python-starter-service-2.0.2/starter_service/env.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-07 12:41:23.670373 osint-python-starter-service-2.0.2/starter_service/examples/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.2/starter_service/examples/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      716 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.2/starter_service/examples/error.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      927 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.2/starter_service/examples/manual_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1313 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.2/starter_service/examples/multi.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1062 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.2/starter_service/examples/single.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6887 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.2/starter_service/kafka_adapter.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.2/starter_service/messages.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6552 2023-04-07 12:39:21.000000 osint-python-starter-service-2.0.2/starter_service/schemas.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.3/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1713 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.3/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-12 12:38:30.000000 osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      790 2023-04-12 12:38:30.000000 osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-12 12:38:30.000000 osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-04-12 12:38:30.000000 osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-04-12 12:38:30.000000 osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-04-12 12:22:32.000000 osint-python-starter-service-2.0.3/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/starter_service/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.3/starter_service/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      177 2023-04-07 11:36:44.000000 osint-python-starter-service-2.0.3/starter_service/aaaa.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.3/starter_service/api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6814 2023-04-12 12:36:49.000000 osint-python-starter-service-2.0.3/starter_service/api_server.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4731 2023-04-06 18:13:23.000000 osint-python-starter-service-2.0.3/starter_service/avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2757 2023-04-12 12:21:36.000000 osint-python-starter-service-2.0.3/starter_service/base_service.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1275 2023-04-04 14:58:16.000000 osint-python-starter-service-2.0.3/starter_service/env.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/starter_service/examples/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.3/starter_service/examples/__init__.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/starter_service/examples/classes/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.3/starter_service/examples/classes/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      716 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.3/starter_service/examples/error.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      927 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.3/starter_service/examples/manual_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1313 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.3/starter_service/examples/multi.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1062 2023-04-12 12:35:48.000000 osint-python-starter-service-2.0.3/starter_service/examples/single.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6887 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.3/starter_service/kafka_adapter.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.3/starter_service/messages.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6406 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.3/starter_service/schemas.py
```

### Comparing `osint-python-starter-service-2.0.2/LICENSE` & `osint-python-starter-service-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.2/PKG-INFO` & `osint-python-starter-service-2.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -23,19 +23,22 @@
 First you need to provide ENV variables for the service to run.
 
 ### ENV variables
 
 Main ENV variables:
 
 - `CLIENT_ID` - client id of the service
+- `REST_API_ENABLED` - enable/disable REST API
+
+## Kafka
+
 - `CONSUME` - comma separated list of topics to consume
 - `PRODUCE` - comma separated list of topics to produce
 - `KAFKA_HOST` - kafka host
 - `SCHEMA_REGISTRY` - schema registry host
-- `REST_API_ENABLED` - enable/disable REST API
 
 ## Usage
 
 Check the provided examples in the `examples` folder.
 
 ## Example
```

### Comparing `osint-python-starter-service-2.0.2/README.md` & `osint-python-starter-service-2.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,22 @@
 First you need to provide ENV variables for the service to run.
 
 ### ENV variables
 
 Main ENV variables:
 
 - `CLIENT_ID` - client id of the service
+- `REST_API_ENABLED` - enable/disable REST API
+
+## Kafka
+
 - `CONSUME` - comma separated list of topics to consume
 - `PRODUCE` - comma separated list of topics to produce
 - `KAFKA_HOST` - kafka host
 - `SCHEMA_REGISTRY` - schema registry host
-- `REST_API_ENABLED` - enable/disable REST API
 
 ## Usage
 
 Check the provided examples in the `examples` folder.
 
 ## Example
```

### Comparing `osint-python-starter-service-2.0.2/osint_python_starter_service.egg-info/PKG-INFO` & `osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -23,19 +23,22 @@
 First you need to provide ENV variables for the service to run.
 
 ### ENV variables
 
 Main ENV variables:
 
 - `CLIENT_ID` - client id of the service
+- `REST_API_ENABLED` - enable/disable REST API
+
+## Kafka
+
 - `CONSUME` - comma separated list of topics to consume
 - `PRODUCE` - comma separated list of topics to produce
 - `KAFKA_HOST` - kafka host
 - `SCHEMA_REGISTRY` - schema registry host
-- `REST_API_ENABLED` - enable/disable REST API
 
 ## Usage
 
 Check the provided examples in the `examples` folder.
 
 ## Example
```

### Comparing `osint-python-starter-service-2.0.2/osint_python_starter_service.egg-info/SOURCES.txt` & `osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 starter_service/kafka_adapter.py
 starter_service/messages.py
 starter_service/schemas.py
 starter_service/examples/__init__.py
 starter_service/examples/error.py
 starter_service/examples/manual_kafka.py
 starter_service/examples/multi.py
-starter_service/examples/single.py
+starter_service/examples/single.py
+starter_service/examples/classes/__init__.py
```

### Comparing `osint-python-starter-service-2.0.2/setup.py` & `osint-python-starter-service-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 setuptools.setup(
     name="osint-python-starter-service",
-    version="2.0.2",
+    version="2.0.3",
     author="mindpetk",
     author_email="petkeviciusm@gmail.com",
     description="Python starter service",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-starter-service",
     include_package_data=True,
```

### Comparing `osint-python-starter-service-2.0.2/starter_service/api.py` & `osint-python-starter-service-2.0.3/starter_service/api.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.2/starter_service/api_server.py` & `osint-python-starter-service-2.0.3/starter_service/api_server.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.2/starter_service/avro_parser.py` & `osint-python-starter-service-2.0.3/starter_service/avro_parser.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.2/starter_service/base_service.py` & `osint-python-starter-service-2.0.3/starter_service/base_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s %(levelname)s %(name)s %(message)s')
 
 
 class StarterService(ABC):
 
     def __init__(self):
-        self._logger = logging.getLogger(__name__)
+        self.logger = logging.getLogger(__name__)
         self._kafka = None
         self._api = None
         self._schemas = None
         self._functions = None
         self._initialize()
 
     @abstractmethod
@@ -29,52 +29,52 @@
         pass
 
     def _initialize(self):
         """Initialize services"""
 
         def _schema_callback():
             """Callback for Schema Registry, called when Schema Registry is ready or when an error occurs"""
-            self._logger.info("Schema callback")
+            self.logger.info("Schema callback")
             self._register_api(_kafka_status)
 
         def _kafka_callback():
             """Callback for Kafka Adapter, called when Kafka Adapter is ready or when an error occurs"""
-            self._logger.info("Kafka callback")
+            self.logger.info("Kafka callback")
             self._register_schemas(_schema_callback)
 
         """Initialize services"""
         _kafka_status = "ok"
-        self._logger.info("Initializing kafka")
+        self.logger.info("Initializing kafka")
         try:
             self._kafka = KafkaAdapter(callback=_kafka_callback, base_service=self)
             self._kafka.start()
-            self._logger.info(f"Kafka initialized.")
+            self.logger.info(f"Kafka initialized.")
         except Exception as e:
             _kafka_status = f"Error: {e}"
             _kafka_callback()
-            self._logger.error(f'Error initializing kafka: {e}')
+            self.logger.error(f'Error initializing kafka: {e}')
 
     def _register_schemas(self, callback):
         try:
             callback()
         except Exception as e:
-            self._logger.error(f'Error initializing schema registry: {e}')
+            self.logger.error(f'Error initializing schema registry: {e}')
 
     def _register_api(self, _kafka_status):
         try:
             self._api = APIServer(ready=self.ready, health=self.health, kafka_status=_kafka_status,
                                   base_service=self)
             self._api.start()
-            self._logger.info(f"REST API initialized.")
+            self.logger.info(f"REST API initialized.")
         except Exception as e:
-            self._logger.error(f'Error initializing api: {e}')
+            self.logger.error(f'Error initializing api: {e}')
             traceback.print_exc()
 
         if self._kafka is None and self._api is None:
-            self._logger.error('No services initialized. Shutting down.')
+            self.logger.error('No services initialized. Shutting down.')
             exit(1)
 
     def send_message(self, message, topic):
         """Send message to Kafka"""
         if self._kafka is None:
             raise Exception("Kafka is not initialized")
         self._kafka.send_message(message, topics=topic, testing=True)
```

### Comparing `osint-python-starter-service-2.0.2/starter_service/env.py` & `osint-python-starter-service-2.0.3/starter_service/env.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.2/starter_service/examples/error.py` & `osint-python-starter-service-2.0.3/starter_service/examples/error.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.2/starter_service/examples/manual_kafka.py` & `osint-python-starter-service-2.0.3/starter_service/examples/manual_kafka.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.2/starter_service/examples/multi.py` & `osint-python-starter-service-2.0.3/starter_service/examples/multi.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.2/starter_service/examples/single.py` & `osint-python-starter-service-2.0.3/starter_service/examples/single.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.2/starter_service/kafka_adapter.py` & `osint-python-starter-service-2.0.3/starter_service/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.2/starter_service/messages.py` & `osint-python-starter-service-2.0.3/starter_service/messages.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.2/starter_service/schemas.py` & `osint-python-starter-service-2.0.3/starter_service/schemas.py`

 * *Files 9% similar despite different names*

```diff
@@ -156,17 +156,15 @@
                 raise e
 
         if not os.path.exists(f"{_path}/schemas"):
             try:
                 os.makedirs(f"{_path}/schemas")
                 with open(f"{_path}/schemas/readme.txt", "w") as f:
                     f.write(
-                        "Use this folder to provide AVRO schemas\n"
-                        "Consume schemas are used to consume messages\n"
-                        "Produce schemas are used to produce messages"
+                        "Use this folder to provide AVRO schemas"
                     )
             except Exception as e:
                 self._logger.error(f"Error creating schema folder {e}")
                 raise e
 
     def get_schema(self, topic) -> object or dict:
         with self._lock:
```

