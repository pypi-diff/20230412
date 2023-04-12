# Comparing `tmp/inspector-python-0.1.8.tar.gz` & `tmp/inspector-python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspector-python-0.1.8.tar", last modified: Wed Nov 16 13:04:14 2022, max compression
+gzip compressed data, was "inspector-python-0.1.9.tar", last modified: Fri Nov 18 17:35:57 2022, max compression
```

## Comparing `inspector-python-0.1.8.tar` & `inspector-python-0.1.9.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxrwx   0        0        0        0 2022-11-16 13:04:14.684188 inspector-python-0.1.8/
--rw-rw-rw-   0        0        0     1092 2022-09-26 17:00:05.000000 inspector-python-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1524 2022-11-16 13:04:14.684188 inspector-python-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      933 2022-11-15 14:49:17.000000 inspector-python-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2022-11-16 13:04:14.684188 inspector-python-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      961 2022-11-16 13:03:28.000000 inspector-python-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-16 13:04:14.631466 inspector-python-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2022-11-16 13:04:14.638018 inspector-python-0.1.8/src/inspector/
--rw-rw-rw-   0        0        0       76 2022-09-26 17:00:05.000000 inspector-python-0.1.8/src/inspector/__init__.py
--rw-rw-rw-   0        0        0     5116 2022-11-16 13:02:42.000000 inspector-python-0.1.8/src/inspector/configuration.py
-drwxrwxrwx   0        0        0        0 2022-11-16 13:04:14.641695 inspector-python-0.1.8/src/inspector/exceptions/
--rw-rw-rw-   0        0        0       52 2022-09-26 17:00:05.000000 inspector-python-0.1.8/src/inspector/exceptions/__init__.py
--rw-rw-rw-   0        0        0      145 2022-09-26 17:00:05.000000 inspector-python-0.1.8/src/inspector/exceptions/inspector_exception.py
--rw-rw-rw-   0        0        0     4520 2022-11-16 13:02:42.000000 inspector-python-0.1.8/src/inspector/inspector.py
-drwxrwxrwx   0        0        0        0 2022-11-16 13:04:14.651617 inspector-python-0.1.8/src/inspector/models/
--rw-rw-rw-   0        0        0      203 2022-11-15 11:43:57.000000 inspector-python-0.1.8/src/inspector/models/__init__.py
--rw-rw-rw-   0        0        0     1902 2022-10-05 12:59:26.000000 inspector-python-0.1.8/src/inspector/models/arrayable.py
-drwxrwxrwx   0        0        0        0 2022-11-16 13:04:14.656137 inspector-python-0.1.8/src/inspector/models/enums/
--rw-rw-rw-   0        0        0      125 2022-10-05 12:59:26.000000 inspector-python-0.1.8/src/inspector/models/enums/__init__.py
--rw-rw-rw-   0        0        0      179 2022-11-15 11:43:57.000000 inspector-python-0.1.8/src/inspector/models/enums/model_type.py
--rw-rw-rw-   0        0        0      107 2022-10-05 12:59:26.000000 inspector-python-0.1.8/src/inspector/models/enums/transaction_type.py
--rw-rw-rw-   0        0        0       95 2022-10-05 12:59:26.000000 inspector-python-0.1.8/src/inspector/models/enums/transport_type.py
--rw-rw-rw-   0        0        0     2448 2022-11-15 13:48:45.000000 inspector-python-0.1.8/src/inspector/models/error.py
--rw-rw-rw-   0        0        0     1451 2022-11-15 11:43:57.000000 inspector-python-0.1.8/src/inspector/models/has_context.py
-drwxrwxrwx   0        0        0        0 2022-11-16 13:04:14.661647 inspector-python-0.1.8/src/inspector/models/partials/
--rw-rw-rw-   0        0        0      152 2022-10-05 12:59:26.000000 inspector-python-0.1.8/src/inspector/models/partials/__init__.py
--rw-rw-rw-   0        0        0     1463 2022-11-16 13:02:42.000000 inspector-python-0.1.8/src/inspector/models/partials/host.py
--rw-rw-rw-   0        0        0      474 2022-11-15 13:48:45.000000 inspector-python-0.1.8/src/inspector/models/partials/http.py
--rw-rw-rw-   0        0        0     1190 2022-11-15 13:48:45.000000 inspector-python-0.1.8/src/inspector/models/partials/request.py
--rw-rw-rw-   0        0        0      604 2022-11-15 13:48:45.000000 inspector-python-0.1.8/src/inspector/models/partials/socket.py
--rw-rw-rw-   0        0        0     1093 2022-11-15 13:48:45.000000 inspector-python-0.1.8/src/inspector/models/partials/url.py
--rw-rw-rw-   0        0        0      552 2022-11-15 13:48:45.000000 inspector-python-0.1.8/src/inspector/models/partials/user.py
--rw-rw-rw-   0        0        0     1145 2022-11-15 13:48:45.000000 inspector-python-0.1.8/src/inspector/models/performance.py
--rw-rw-rw-   0        0        0      970 2022-11-15 13:48:45.000000 inspector-python-0.1.8/src/inspector/models/segment.py
--rw-rw-rw-   0        0        0     2821 2022-11-16 13:02:42.000000 inspector-python-0.1.8/src/inspector/models/transaction.py
-drwxrwxrwx   0        0        0        0 2022-11-16 13:04:14.661647 inspector-python-0.1.8/src/inspector/transports/
--rw-rw-rw-   0        0        0      177 2022-11-15 11:43:57.000000 inspector-python-0.1.8/src/inspector/transports/__init__.py
--rw-rw-rw-   0        0        0     1039 2022-11-15 13:48:45.000000 inspector-python-0.1.8/src/inspector/transports/async_transport.py
--rw-rw-rw-   0        0        0      793 2022-11-15 13:48:45.000000 inspector-python-0.1.8/src/inspector/transports/sync_transport.py
--rw-rw-rw-   0        0        0     3531 2022-11-15 13:52:46.000000 inspector-python-0.1.8/src/inspector/transports/transport.py
--rw-rw-rw-   0        0        0      488 2022-11-15 13:48:45.000000 inspector-python-0.1.8/src/inspector/transports/transport_interface.py
-drwxrwxrwx   0        0        0        0 2022-11-16 13:04:14.671856 inspector-python-0.1.8/src/inspector_python.egg-info/
--rw-rw-rw-   0        0        0     1524 2022-11-16 13:04:14.000000 inspector-python-0.1.8/src/inspector_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2022-11-16 13:04:14.000000 inspector-python-0.1.8/src/inspector_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-16 13:04:14.000000 inspector-python-0.1.8/src/inspector_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-11-16 13:04:14.000000 inspector-python-0.1.8/src/inspector_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-11-16 13:04:14.000000 inspector-python-0.1.8/src/inspector_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-16 13:04:14.682121 inspector-python-0.1.8/src/tests/
--rw-rw-rw-   0        0        0        0 2022-09-26 17:00:05.000000 inspector-python-0.1.8/src/tests/__init__.py
--rw-rw-rw-   0        0        0     1196 2022-11-16 13:02:42.000000 inspector-python-0.1.8/src/tests/test_inspector.py
+drwxrwxrwx   0        0        0        0 2022-11-18 17:35:57.784078 inspector-python-0.1.9/
+-rw-rw-rw-   0        0        0     1092 2022-09-26 17:00:05.000000 inspector-python-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1524 2022-11-18 17:35:57.784078 inspector-python-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      933 2022-11-15 14:49:17.000000 inspector-python-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-11-18 17:35:57.784078 inspector-python-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      961 2022-11-18 17:34:49.000000 inspector-python-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-18 17:35:57.724420 inspector-python-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2022-11-18 17:35:57.733326 inspector-python-0.1.9/src/inspector/
+-rw-rw-rw-   0        0        0       76 2022-09-26 17:00:05.000000 inspector-python-0.1.9/src/inspector/__init__.py
+-rw-rw-rw-   0        0        0     5116 2022-11-16 13:02:42.000000 inspector-python-0.1.9/src/inspector/configuration.py
+drwxrwxrwx   0        0        0        0 2022-11-18 17:35:57.735319 inspector-python-0.1.9/src/inspector/exceptions/
+-rw-rw-rw-   0        0        0       53 2022-11-18 17:34:49.000000 inspector-python-0.1.9/src/inspector/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      145 2022-09-26 17:00:05.000000 inspector-python-0.1.9/src/inspector/exceptions/inspector_exception.py
+-rw-rw-rw-   0        0        0     4531 2022-11-18 17:34:49.000000 inspector-python-0.1.9/src/inspector/inspector.py
+drwxrwxrwx   0        0        0        0 2022-11-18 17:35:57.741201 inspector-python-0.1.9/src/inspector/models/
+-rw-rw-rw-   0        0        0      203 2022-11-15 11:43:57.000000 inspector-python-0.1.9/src/inspector/models/__init__.py
+-rw-rw-rw-   0        0        0     1902 2022-10-05 12:59:26.000000 inspector-python-0.1.9/src/inspector/models/arrayable.py
+drwxrwxrwx   0        0        0        0 2022-11-18 17:35:57.741201 inspector-python-0.1.9/src/inspector/models/enums/
+-rw-rw-rw-   0        0        0      125 2022-10-05 12:59:26.000000 inspector-python-0.1.9/src/inspector/models/enums/__init__.py
+-rw-rw-rw-   0        0        0      179 2022-11-15 11:43:57.000000 inspector-python-0.1.9/src/inspector/models/enums/model_type.py
+-rw-rw-rw-   0        0        0      107 2022-10-05 12:59:26.000000 inspector-python-0.1.9/src/inspector/models/enums/transaction_type.py
+-rw-rw-rw-   0        0        0       95 2022-10-05 12:59:26.000000 inspector-python-0.1.9/src/inspector/models/enums/transport_type.py
+-rw-rw-rw-   0        0        0     2448 2022-11-15 13:48:45.000000 inspector-python-0.1.9/src/inspector/models/error.py
+-rw-rw-rw-   0        0        0     1451 2022-11-15 11:43:57.000000 inspector-python-0.1.9/src/inspector/models/has_context.py
+drwxrwxrwx   0        0        0        0 2022-11-18 17:35:57.752341 inspector-python-0.1.9/src/inspector/models/partials/
+-rw-rw-rw-   0        0        0      152 2022-10-05 12:59:26.000000 inspector-python-0.1.9/src/inspector/models/partials/__init__.py
+-rw-rw-rw-   0        0        0     1463 2022-11-16 13:02:42.000000 inspector-python-0.1.9/src/inspector/models/partials/host.py
+-rw-rw-rw-   0        0        0      474 2022-11-15 13:48:45.000000 inspector-python-0.1.9/src/inspector/models/partials/http.py
+-rw-rw-rw-   0        0        0     1190 2022-11-15 13:48:45.000000 inspector-python-0.1.9/src/inspector/models/partials/request.py
+-rw-rw-rw-   0        0        0      604 2022-11-15 13:48:45.000000 inspector-python-0.1.9/src/inspector/models/partials/socket.py
+-rw-rw-rw-   0        0        0     1093 2022-11-15 13:48:45.000000 inspector-python-0.1.9/src/inspector/models/partials/url.py
+-rw-rw-rw-   0        0        0      552 2022-11-15 13:48:45.000000 inspector-python-0.1.9/src/inspector/models/partials/user.py
+-rw-rw-rw-   0        0        0     1145 2022-11-15 13:48:45.000000 inspector-python-0.1.9/src/inspector/models/performance.py
+-rw-rw-rw-   0        0        0      997 2022-11-18 17:34:49.000000 inspector-python-0.1.9/src/inspector/models/segment.py
+-rw-rw-rw-   0        0        0     2821 2022-11-16 13:02:42.000000 inspector-python-0.1.9/src/inspector/models/transaction.py
+drwxrwxrwx   0        0        0        0 2022-11-18 17:35:57.758847 inspector-python-0.1.9/src/inspector/transports/
+-rw-rw-rw-   0        0        0      177 2022-11-15 11:43:57.000000 inspector-python-0.1.9/src/inspector/transports/__init__.py
+-rw-rw-rw-   0        0        0     1039 2022-11-15 13:48:45.000000 inspector-python-0.1.9/src/inspector/transports/async_transport.py
+-rw-rw-rw-   0        0        0      793 2022-11-15 13:48:45.000000 inspector-python-0.1.9/src/inspector/transports/sync_transport.py
+-rw-rw-rw-   0        0        0     3531 2022-11-15 13:52:46.000000 inspector-python-0.1.9/src/inspector/transports/transport.py
+-rw-rw-rw-   0        0        0      488 2022-11-15 13:48:45.000000 inspector-python-0.1.9/src/inspector/transports/transport_interface.py
+drwxrwxrwx   0        0        0        0 2022-11-18 17:35:57.780063 inspector-python-0.1.9/src/inspector_python.egg-info/
+-rw-rw-rw-   0        0        0     1524 2022-11-18 17:35:57.000000 inspector-python-0.1.9/src/inspector_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1389 2022-11-18 17:35:57.000000 inspector-python-0.1.9/src/inspector_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-18 17:35:57.000000 inspector-python-0.1.9/src/inspector_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2022-11-18 17:35:57.000000 inspector-python-0.1.9/src/inspector_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2022-11-18 17:35:57.000000 inspector-python-0.1.9/src/inspector_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-11-18 17:35:57.784078 inspector-python-0.1.9/src/tests/
+-rw-rw-rw-   0        0        0        0 2022-09-26 17:00:05.000000 inspector-python-0.1.9/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     1837 2022-11-18 17:34:49.000000 inspector-python-0.1.9/src/tests/test_agent.py
+-rw-rw-rw-   0        0        0     1213 2022-11-18 17:34:49.000000 inspector-python-0.1.9/src/tests/test_exception_encoder.py
```

### Comparing `inspector-python-0.1.8/LICENSE` & `inspector-python-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/PKG-INFO` & `inspector-python-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspector-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: Real-time Code Execution Monitoring of your Python scripts.
 Home-page: https://inspector.dev/
 Author: Antonio Bruno
 Author-email: antoniobruno82@gmail.com
 License: MIT
 Project-URL: Documentation, https://docs.inspector.dev/guides/python/
 Project-URL: Source Code, https://github.com/inspector-apm/inspector-python
```

### Comparing `inspector-python-0.1.8/README.md` & `inspector-python-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/setup.py` & `inspector-python-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='inspector-python',
-    version='0.1.8',
+    version='0.1.9',
     description='Real-time Code Execution Monitoring of your Python scripts.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Antonio Bruno',
     author_email='antoniobruno82@gmail.com',
     url='https://inspector.dev/',
     project_urls={
```

### Comparing `inspector-python-0.1.8/src/inspector/configuration.py` & `inspector-python-0.1.9/src/inspector/configuration.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector/inspector.py` & `inspector-python-0.1.9/src/inspector/inspector.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     # Disable recording.
     # return: Inspector
     def stop_recording(self) -> Inspector:
         self._configuration.set_enabled(False)
         return self
 
-    def start_segment(self, type_str=TransactionType.PROCESS.value, label=None):
+    def start_segment(self, type_str=TransactionType.PROCESS.value, label=None) -> Segment:
         self._segment = Segment(self._transaction, type_str, label)
         self._segment.start()
         self.add_entries(self._segment)
         return self._segment
 
     def add_segment(self, callback, type_str, label=None, throw=False):
         self.start_segment(type_str, label)
```

### Comparing `inspector-python-0.1.8/src/inspector/models/arrayable.py` & `inspector-python-0.1.9/src/inspector/models/arrayable.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector/models/error.py` & `inspector-python-0.1.9/src/inspector/models/error.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector/models/has_context.py` & `inspector-python-0.1.9/src/inspector/models/has_context.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector/models/partials/host.py` & `inspector-python-0.1.9/src/inspector/models/partials/host.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector/models/partials/request.py` & `inspector-python-0.1.9/src/inspector/models/partials/request.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector/models/partials/socket.py` & `inspector-python-0.1.9/src/inspector/models/partials/socket.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector/models/partials/url.py` & `inspector-python-0.1.9/src/inspector/models/partials/url.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector/models/partials/user.py` & `inspector-python-0.1.9/src/inspector/models/partials/user.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector/models/performance.py` & `inspector-python-0.1.9/src/inspector/models/performance.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector/models/segment.py` & `inspector-python-0.1.9/src/inspector/models/segment.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     timestamp = None
 
     def __init__(self, transaction, type, label=None):
         Performance.__init__(self)
         self.model = self.MODEL_NAME
         self.type = type
         self.label = label
+        self.context = {}
         self.transaction = transaction
         self.timestamp = self.get_microtime()
 
     def start(self, timestamp=None) -> Performance:
         initial = self.get_microtime() if timestamp is None else timestamp
         self.start = round((initial - self.transaction.timestamp) * 1000, 4)
         return self
```

### Comparing `inspector-python-0.1.8/src/inspector/models/transaction.py` & `inspector-python-0.1.9/src/inspector/models/transaction.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector/transports/async_transport.py` & `inspector-python-0.1.9/src/inspector/transports/async_transport.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector/transports/sync_transport.py` & `inspector-python-0.1.9/src/inspector/transports/sync_transport.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector/transports/transport.py` & `inspector-python-0.1.9/src/inspector/transports/transport.py`

 * *Files identical despite different names*

### Comparing `inspector-python-0.1.8/src/inspector_python.egg-info/PKG-INFO` & `inspector-python-0.1.9/src/inspector_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspector-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: Real-time Code Execution Monitoring of your Python scripts.
 Home-page: https://inspector.dev/
 Author: Antonio Bruno
 Author-email: antoniobruno82@gmail.com
 License: MIT
 Project-URL: Documentation, https://docs.inspector.dev/guides/python/
 Project-URL: Source Code, https://github.com/inspector-apm/inspector-python
```

### Comparing `inspector-python-0.1.8/src/inspector_python.egg-info/SOURCES.txt` & `inspector-python-0.1.9/src/inspector_python.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -31,8 +31,9 @@
 src/inspector/transports/transport_interface.py
 src/inspector_python.egg-info/PKG-INFO
 src/inspector_python.egg-info/SOURCES.txt
 src/inspector_python.egg-info/dependency_links.txt
 src/inspector_python.egg-info/requires.txt
 src/inspector_python.egg-info/top_level.txt
 src/tests/__init__.py
-src/tests/test_inspector.py
+src/tests/test_agent.py
+src/tests/test_exception_encoder.py
```

