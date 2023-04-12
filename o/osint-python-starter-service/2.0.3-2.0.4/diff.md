# Comparing `tmp/osint-python-starter-service-2.0.3.tar.gz` & `tmp/osint-python-starter-service-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-starter-service-2.0.3.tar", last modified: Wed Apr 12 12:38:30 2023, max compression
+gzip compressed data, was "osint-python-starter-service-2.0.4.tar", last modified: Wed Apr 12 13:18:24 2023, max compression
```

## Comparing `osint-python-starter-service-2.0.3.tar` & `osint-python-starter-service-2.0.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.3/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1713 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.3/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-12 12:38:30.000000 osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      790 2023-04-12 12:38:30.000000 osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-12 12:38:30.000000 osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-04-12 12:38:30.000000 osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-04-12 12:38:30.000000 osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-04-12 12:22:32.000000 osint-python-starter-service-2.0.3/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/starter_service/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.3/starter_service/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      177 2023-04-07 11:36:44.000000 osint-python-starter-service-2.0.3/starter_service/aaaa.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.3/starter_service/api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6814 2023-04-12 12:36:49.000000 osint-python-starter-service-2.0.3/starter_service/api_server.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4731 2023-04-06 18:13:23.000000 osint-python-starter-service-2.0.3/starter_service/avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2757 2023-04-12 12:21:36.000000 osint-python-starter-service-2.0.3/starter_service/base_service.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1275 2023-04-04 14:58:16.000000 osint-python-starter-service-2.0.3/starter_service/env.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/starter_service/examples/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.3/starter_service/examples/__init__.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:38:30.434693 osint-python-starter-service-2.0.3/starter_service/examples/classes/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.3/starter_service/examples/classes/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      716 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.3/starter_service/examples/error.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      927 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.3/starter_service/examples/manual_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1313 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.3/starter_service/examples/multi.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1062 2023-04-12 12:35:48.000000 osint-python-starter-service-2.0.3/starter_service/examples/single.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6887 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.3/starter_service/kafka_adapter.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.3/starter_service/messages.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6406 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.3/starter_service/schemas.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:18:24.833377 osint-python-starter-service-2.0.4/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.4/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-12 13:18:24.830044 osint-python-starter-service-2.0.4/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1713 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.4/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:18:24.830044 osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-12 13:18:24.000000 osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      874 2023-04-12 13:18:24.000000 osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-12 13:18:24.000000 osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-04-12 13:18:24.000000 osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-04-12 13:18:24.000000 osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-12 13:18:24.833377 osint-python-starter-service-2.0.4/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-04-12 13:16:20.000000 osint-python-starter-service-2.0.4/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:18:24.830044 osint-python-starter-service-2.0.4/starter_service/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.4/starter_service/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.4/starter_service/api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6814 2023-04-12 12:36:49.000000 osint-python-starter-service-2.0.4/starter_service/api_server.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4731 2023-04-06 18:13:23.000000 osint-python-starter-service-2.0.4/starter_service/avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2980 2023-04-12 13:10:08.000000 osint-python-starter-service-2.0.4/starter_service/base_service.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1275 2023-04-04 14:58:16.000000 osint-python-starter-service-2.0.4/starter_service/env.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:18:24.830044 osint-python-starter-service-2.0.4/starter_service/examples/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.4/starter_service/examples/__init__.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 13:18:24.830044 osint-python-starter-service-2.0.4/starter_service/examples/classes/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.4/starter_service/examples/classes/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2569 2023-04-12 13:08:09.000000 osint-python-starter-service-2.0.4/starter_service/examples/classes/article_raw_en.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      637 2023-04-12 13:08:09.000000 osint-python-starter-service-2.0.4/starter_service/examples/classes/metadata_item_key_en.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      708 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.4/starter_service/examples/error.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      912 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.4/starter_service/examples/manual_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1298 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.4/starter_service/examples/multi.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1047 2023-04-12 13:12:02.000000 osint-python-starter-service-2.0.4/starter_service/examples/single.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6887 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.4/starter_service/kafka_adapter.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.4/starter_service/messages.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6406 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.4/starter_service/schemas.py
```

### Comparing `osint-python-starter-service-2.0.3/LICENSE` & `osint-python-starter-service-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.3/PKG-INFO` & `osint-python-starter-service-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.0.3/README.md` & `osint-python-starter-service-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/PKG-INFO` & `osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.0.3/osint_python_starter_service.egg-info/SOURCES.txt` & `osint-python-starter-service-2.0.4/osint_python_starter_service.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 setup.py
 osint_python_starter_service.egg-info/PKG-INFO
 osint_python_starter_service.egg-info/SOURCES.txt
 osint_python_starter_service.egg-info/dependency_links.txt
 osint_python_starter_service.egg-info/requires.txt
 osint_python_starter_service.egg-info/top_level.txt
 starter_service/__init__.py
-starter_service/aaaa.py
 starter_service/api.py
 starter_service/api_server.py
 starter_service/avro_parser.py
 starter_service/base_service.py
 starter_service/env.py
 starter_service/kafka_adapter.py
 starter_service/messages.py
 starter_service/schemas.py
 starter_service/examples/__init__.py
 starter_service/examples/error.py
 starter_service/examples/manual_kafka.py
 starter_service/examples/multi.py
 starter_service/examples/single.py
-starter_service/examples/classes/__init__.py
+starter_service/examples/classes/__init__.py
+starter_service/examples/classes/article_raw_en.py
+starter_service/examples/classes/metadata_item_key_en.py
```

### Comparing `osint-python-starter-service-2.0.3/setup.py` & `osint-python-starter-service-2.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 setuptools.setup(
     name="osint-python-starter-service",
-    version="2.0.3",
+    version="2.0.4",
     author="mindpetk",
     author_email="petkeviciusm@gmail.com",
     description="Python starter service",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-starter-service",
     include_package_data=True,
```

### Comparing `osint-python-starter-service-2.0.3/starter_service/api.py` & `osint-python-starter-service-2.0.4/starter_service/api.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.3/starter_service/api_server.py` & `osint-python-starter-service-2.0.4/starter_service/api_server.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.3/starter_service/avro_parser.py` & `osint-python-starter-service-2.0.4/starter_service/avro_parser.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.3/starter_service/base_service.py` & `osint-python-starter-service-2.0.4/starter_service/base_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import logging
 import traceback
 from abc import ABC, abstractmethod
 
 from starter_service.api_server import APIServer
+from starter_service.env import ENV
 from starter_service.kafka_adapter import KafkaAdapter
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s %(levelname)s %(name)s %(message)s')
 
 
 class StarterService(ABC):
+    """Base class for all services."""
+    name = None  # Change this to the name of your service or use CLIENT_ID environment variable
 
     def __init__(self):
         self.logger = logging.getLogger(__name__)
         self._kafka = None
         self._api = None
         self._schemas = None
         self._functions = None
@@ -26,14 +29,15 @@
     @abstractmethod
     def health(self) -> str:
         """Return service health status."""
         pass
 
     def _initialize(self):
         """Initialize services"""
+        ENV.CLIENT_ID = ENV.CLIENT_ID or self.name
 
         def _schema_callback():
             """Callback for Schema Registry, called when Schema Registry is ready or when an error occurs"""
             self.logger.info("Schema callback")
             self._register_api(_kafka_status)
 
         def _kafka_callback():
```

### Comparing `osint-python-starter-service-2.0.3/starter_service/env.py` & `osint-python-starter-service-2.0.4/starter_service/env.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.3/starter_service/examples/error.py` & `osint-python-starter-service-2.0.4/starter_service/examples/error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import sys
 
 sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
-os.environ['CLIENT_ID'] = 'error'
 os.environ['CONSUME'] = 'article_raw_en'
 os.environ['PRODUCE'] = 'metadata_item_key_en'
 os.environ['REST_API_ENABLED'] = 'True'
 
 from starter_service.base_service import StarterService
 from starter_service.api import API
 
 
 class SingleRoute(StarterService):
+    name = "single_error"
 
     def health(self):
         return "OK"
 
     def ready(self):
         return True
```

### Comparing `osint-python-starter-service-2.0.3/starter_service/examples/manual_kafka.py` & `osint-python-starter-service-2.0.4/starter_service/examples/manual_kafka.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import sys
 
 sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
-os.environ['CLIENT_ID'] = 'manual_kafka'
 os.environ['CONSUME'] = 'article_raw_xx'
 os.environ['PRODUCE'] = 'article_raw_en,article_raw_lt'
 os.environ['REST_API_ENABLED'] = 'True'
 
 from starter_service.base_service import StarterService
 from starter_service.api import API
 
 
 class ManualKafka(StarterService):
+    name = "manual_kafka"
 
     def __init__(self):
         super().__init__()
 
     def health(self):
         return
```

### Comparing `osint-python-starter-service-2.0.3/starter_service/examples/multi.py` & `osint-python-starter-service-2.0.4/starter_service/examples/multi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import sys
 
 sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
-os.environ['CLIENT_ID'] = 'multi'
 os.environ['CONSUME'] = 'article_raw_xx'
 os.environ['PRODUCE'] = 'article_raw_en,article_raw_lt,article_raw_nl'
 os.environ['REST_API_ENABLED'] = 'True'
 
 from starter_service.base_service import StarterService
 from starter_service.api import API
 
 
 class MultiRoutes(StarterService):
+    name = "multi"
 
     def __init__(self):
         super().__init__()
 
     def health(self):
         return
```

### Comparing `osint-python-starter-service-2.0.3/starter_service/examples/single.py` & `osint-python-starter-service-2.0.4/starter_service/examples/single.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import sys
 
 sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
-os.environ['CLIENT_ID'] = 'single'
 os.environ['CONSUME'] = 'article_raw_en'
 os.environ['PRODUCE'] = 'metadata_item_key_en'
 os.environ['REST_API_ENABLED'] = 'True'
 
 from starter_service.base_service import StarterService
 from starter_service.api import API
 
 
 class SingleRoute(StarterService):
+    name = "single"
 
     def health(self):
         return "OK"
 
     def ready(self):
         return True
```

### Comparing `osint-python-starter-service-2.0.3/starter_service/kafka_adapter.py` & `osint-python-starter-service-2.0.4/starter_service/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.3/starter_service/messages.py` & `osint-python-starter-service-2.0.4/starter_service/messages.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.3/starter_service/schemas.py` & `osint-python-starter-service-2.0.4/starter_service/schemas.py`

 * *Files identical despite different names*

