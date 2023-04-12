# Comparing `tmp/openfabric_pysdk-0.2.3.tar.gz` & `tmp/openfabric_pysdk-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfabric_pysdk-0.2.3.tar", max compression
+gzip compressed data, was "openfabric_pysdk-0.2.4.tar", max compression
```

## Comparing `openfabric_pysdk-0.2.3.tar` & `openfabric_pysdk-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2022-09-07 14:53:56.463341 openfabric_pysdk-0.2.3/README.md
--rw-r--r--   0        0        0        1 2023-03-14 13:31:02.159674 openfabric_pysdk-0.2.3/openfabric_pysdk/__init__.py
--rw-r--r--   0        0        0     5649 2023-03-30 07:45:52.716595 openfabric_pysdk-0.2.3/openfabric_pysdk/application.py
--rw-r--r--   0        0        0     3600 2023-03-30 07:45:52.768103 openfabric_pysdk-0.2.3/openfabric_pysdk/benchmark.py
--rw-r--r--   0        0        0      412 2023-03-14 13:25:56.167968 openfabric_pysdk-0.2.3/openfabric_pysdk/config.py
--rw-r--r--   0        0        0     5507 2023-03-14 13:25:56.168325 openfabric_pysdk-0.2.3/openfabric_pysdk/context.py
--rw-r--r--   0        0        0     7386 2023-03-30 07:45:52.744619 openfabric_pysdk-0.2.3/openfabric_pysdk/engine.py
--rw-r--r--   0        0        0     1993 2023-03-29 16:17:55.309405 openfabric_pysdk-0.2.3/openfabric_pysdk/loader.py
--rw-r--r--   0        0        0     1852 2023-03-30 07:45:52.736248 openfabric_pysdk-0.2.3/openfabric_pysdk/starter.py
--rw-r--r--   0        0        0     4463 2023-03-30 07:45:52.763114 openfabric_pysdk-0.2.3/openfabric_pysdk/store.py
--rw-r--r--   0        0        0     3114 2023-03-30 07:45:52.756404 openfabric_pysdk-0.2.3/openfabric_pysdk/task.py
--rw-r--r--   0        0        0    13433 2023-03-29 17:29:12.865670 openfabric_pysdk-0.2.3/openfabric_pysdk/templates/index.html
--rw-r--r--   0        0        0     3880 2023-03-16 19:44:08.374707 openfabric_pysdk-0.2.3/openfabric_pysdk/toolset.py
--rw-r--r--   0        0        0        0 2022-09-07 14:53:56.464562 openfabric_pysdk-0.2.3/openfabric_pysdk/transport/__init__.py
--rw-r--r--   0        0        0     2609 2023-03-15 16:39:57.524646 openfabric_pysdk-0.2.3/openfabric_pysdk/transport/queue.py
--rw-r--r--   0        0        0     1077 2023-03-15 16:31:53.418040 openfabric_pysdk-0.2.3/openfabric_pysdk/transport/rest.py
--rw-r--r--   0        0        0     6100 2023-03-30 07:45:52.749321 openfabric_pysdk-0.2.3/openfabric_pysdk/transport/socket.py
--rw-r--r--   0        0        0     2408 2023-03-14 13:25:56.172085 openfabric_pysdk-0.2.3/openfabric_pysdk/utility.py
--rw-r--r--   0        0        0      886 2023-04-02 06:31:33.287649 openfabric_pysdk-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 openfabric_pysdk-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-07 14:53:56.463341 openfabric_pysdk-0.2.4/README.md
+-rw-r--r--   0        0        0        1 2023-03-14 13:31:02.159674 openfabric_pysdk-0.2.4/openfabric_pysdk/__init__.py
+-rw-r--r--   0        0        0     5649 2023-03-30 07:45:52.716595 openfabric_pysdk-0.2.4/openfabric_pysdk/application.py
+-rw-r--r--   0        0        0     3600 2023-03-30 07:45:52.768103 openfabric_pysdk-0.2.4/openfabric_pysdk/benchmark.py
+-rw-r--r--   0        0        0      412 2023-03-14 13:25:56.167968 openfabric_pysdk-0.2.4/openfabric_pysdk/config.py
+-rw-r--r--   0        0        0     5578 2023-04-11 19:44:10.159542 openfabric_pysdk-0.2.4/openfabric_pysdk/context.py
+-rw-r--r--   0        0        0     7386 2023-03-30 07:45:52.744619 openfabric_pysdk-0.2.4/openfabric_pysdk/engine.py
+-rw-r--r--   0        0        0     1993 2023-03-29 16:17:55.309405 openfabric_pysdk-0.2.4/openfabric_pysdk/loader.py
+-rw-r--r--   0        0        0     1852 2023-03-30 07:45:52.736248 openfabric_pysdk-0.2.4/openfabric_pysdk/starter.py
+-rw-r--r--   0        0        0     4463 2023-03-30 07:45:52.763114 openfabric_pysdk-0.2.4/openfabric_pysdk/store.py
+-rw-r--r--   0        0        0     3114 2023-03-30 07:45:52.756404 openfabric_pysdk-0.2.4/openfabric_pysdk/task.py
+-rw-r--r--   0        0        0    13433 2023-03-29 17:29:12.865670 openfabric_pysdk-0.2.4/openfabric_pysdk/templates/index.html
+-rw-r--r--   0        0        0     3880 2023-03-16 19:44:08.374707 openfabric_pysdk-0.2.4/openfabric_pysdk/toolset.py
+-rw-r--r--   0        0        0        0 2022-09-07 14:53:56.464562 openfabric_pysdk-0.2.4/openfabric_pysdk/transport/__init__.py
+-rw-r--r--   0        0        0     2609 2023-03-15 16:39:57.524646 openfabric_pysdk-0.2.4/openfabric_pysdk/transport/queue.py
+-rw-r--r--   0        0        0     1077 2023-03-15 16:31:53.418040 openfabric_pysdk-0.2.4/openfabric_pysdk/transport/rest.py
+-rw-r--r--   0        0        0     6224 2023-04-11 18:21:33.475130 openfabric_pysdk-0.2.4/openfabric_pysdk/transport/socket.py
+-rw-r--r--   0        0        0     2408 2023-03-14 13:25:56.172085 openfabric_pysdk-0.2.4/openfabric_pysdk/utility.py
+-rw-r--r--   0        0        0      914 2023-04-11 14:42:48.562083 openfabric_pysdk-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 openfabric_pysdk-0.2.4/PKG-INFO
```

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/application.py` & `openfabric_pysdk-0.2.4/openfabric_pysdk/application.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/benchmark.py` & `openfabric_pysdk-0.2.4/openfabric_pysdk/benchmark.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/context.py` & `openfabric_pysdk-0.2.4/openfabric_pysdk/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from datetime import datetime
 from enum import Enum
 from typing import Dict, List, Set
 
 from marshmallow import Schema, fields, post_load
 from tqdm.asyncio import tqdm, tqdm_asyncio
 
@@ -55,15 +56,18 @@
     def __str__(self):
         return self.name
 
 
 class Message:
     type: MessageType = 0
     content: str = None
-    created_at: datetime = datetime.now()
+    created_at: datetime = None
+
+    def __init__(self):
+        self.created_at = datetime.now()
 
     # ------------------------------------------------------------------------
     def __eq__(self, other):
         if not isinstance(other, Message):
             return NotImplemented
         return self.type == other.type and self.content == other.content
```

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/engine.py` & `openfabric_pysdk-0.2.4/openfabric_pysdk/engine.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/loader.py` & `openfabric_pysdk-0.2.4/openfabric_pysdk/loader.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/starter.py` & `openfabric_pysdk-0.2.4/openfabric_pysdk/starter.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/store.py` & `openfabric_pysdk-0.2.4/openfabric_pysdk/store.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/task.py` & `openfabric_pysdk-0.2.4/openfabric_pysdk/task.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/templates/index.html` & `openfabric_pysdk-0.2.4/openfabric_pysdk/templates/index.html`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/toolset.py` & `openfabric_pysdk-0.2.4/openfabric_pysdk/toolset.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/transport/queue.py` & `openfabric_pysdk-0.2.4/openfabric_pysdk/transport/queue.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/transport/rest.py` & `openfabric_pysdk-0.2.4/openfabric_pysdk/transport/rest.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/transport/socket.py` & `openfabric_pysdk-0.2.4/openfabric_pysdk/transport/socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import logging
 import zlib
 from hashlib import md5
 
 from typing import Any, Set, Dict
 
-import eventlet
+import gevent
 from flask import Flask, request
 from flask_socketio import SocketIO, Namespace, emit
 
 from openfabric_pysdk.context import RaySchema, Ray, State, StateSchema
 from openfabric_pysdk.engine import foreground, background
 from openfabric_pysdk.loader import *
 from openfabric_pysdk.utility import ChangeDetector
@@ -28,16 +28,22 @@
     # ------------------------------------------------------------------------
     def __init__(self, socket_namespace, socket_session, app: Flask, state: State):
         super().__init__(socket_namespace)
         self.__session = socket_session
         # Set this variable to "threading", "eventlet" or "gevent" to test the
         # different async modes, or leave it set to None for the application to choose
         # the best option based on installed packages.
-        async_mode = "eventlet"
-        self.__socket_io = SocketIO(app, async_mode=async_mode, cors_allowed_origins='*')
+        async_mode = "gevent"
+        max_size = 10000000 * 100  # 100Mb
+        self.__socket_io = SocketIO(
+            app,
+            async_mode=async_mode,
+            cors_allowed_origins='*',
+            max_http_buffer_size=max_size
+        )
         self.__socket_io.on_namespace(self)
         self.__app = app
         self.__state = state
         self.__active_sessions = set()
 
     # ------------------------------------------------------------------------
     def run(self, debug, host, port):
@@ -85,15 +91,15 @@
                 ray_dump = RaySchema().dump(ray)
                 emit('progress', ray_dump)
                 if ray.finished is True:
                     # input = background.get(qid, 'in')
                     output = background.read(qid, 'out')
                     emit('response', dict(output=output, ray=ray_dump))
                     break
-                eventlet.sleep(0.1)
+                gevent.sleep(0.1)
 
     # ------------------------------------------------------------------------
     def on_resume(self, uid: str):
         sid = request.sid
         with MeasureBlockTime("OpenfabricSocket::restore"):
             def criteria(_ray: Ray):
                 # is deleted ?
@@ -123,15 +129,15 @@
     def on_state(self, uid: str):
         sid = request.sid
         with MeasureBlockTime("Socket::state"):
             while sid in self.__active_sessions:
                 changed = ChangeDetector.is_changed('app::state' + sid, self.__state, StateSchema().dump)
                 if changed is True:
                     emit('state', StateSchema().dump(self.__state))
-                eventlet.sleep(0.1)
+                gevent.sleep(0.1)
 
     # ------------------------------------------------------------------------
     def on_delete(self, qid: str):
         sid = request.sid
         with MeasureBlockTime("OpenfabricSocket::delete"):
             foreground.delete(qid)
             background.delete(qid)
```

### Comparing `openfabric_pysdk-0.2.3/openfabric_pysdk/utility.py` & `openfabric_pysdk-0.2.4/openfabric_pysdk/utility.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.3/pyproject.toml` & `openfabric_pysdk-0.2.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openfabric-pysdk"
-version = "0.2.3"
+version = "0.2.4"
 description = "Openfabric Python SDK"
 authors = ["Andrei Tara <andrei@openfabric.ai>"]
 readme = "README.md"
 homepage = "https://openfabric.ai"
 repository = "https://github.com/Openfabric/openfabic-pysdk"
 keywords = ["openfabric", "SDK", "IoAI"]
 classifiers = [
@@ -15,21 +15,22 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Flask = "^2.0.1"
 Flask-RESTful = "^0.3.9"
 Flask-SocketIO = "^4.3.2"
 flask-apispec = "0.11.0"
-eventlet = "^0.31.1"
 Flask-Cors = "^3.0.10"
 pickleDB = "^0.9.2"
 runstats = "^2.0.0"
 tqdm = "^4.62.3"
 Werkzeug = "2.0.3"
 marshmallow-enum = "^1.5.1"
+gevent = "^22.10.2"
+gevent-websocket = "^0.10.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openfabric_pysdk-0.2.3/PKG-INFO` & `openfabric_pysdk-0.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfabric-pysdk
-Version: 0.2.3
+Version: 0.2.4
 Summary: Openfabric Python SDK
 Home-page: https://openfabric.ai
 Keywords: openfabric,SDK,IoAI
 Author: Andrei Tara
 Author-email: andrei@openfabric.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -16,16 +16,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Flask (>=2.0.1,<3.0.0)
 Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0)
 Requires-Dist: Flask-RESTful (>=0.3.9,<0.4.0)
 Requires-Dist: Flask-SocketIO (>=4.3.2,<5.0.0)
 Requires-Dist: Werkzeug (==2.0.3)
-Requires-Dist: eventlet (>=0.31.1,<0.32.0)
 Requires-Dist: flask-apispec (==0.11.0)
+Requires-Dist: gevent (>=22.10.2,<23.0.0)
+Requires-Dist: gevent-websocket (>=0.10.1,<0.11.0)
 Requires-Dist: marshmallow-enum (>=1.5.1,<2.0.0)
 Requires-Dist: pickleDB (>=0.9.2,<0.10.0)
 Requires-Dist: runstats (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Project-URL: Repository, https://github.com/Openfabric/openfabic-pysdk
 Description-Content-Type: text/markdown
```

