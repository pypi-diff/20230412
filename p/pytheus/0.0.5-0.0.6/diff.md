# Comparing `tmp/pytheus-0.0.5.tar.gz` & `tmp/pytheus-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytheus-0.0.5.tar", last modified: Sun Apr  9 01:13:41 2023, max compression
+gzip compressed data, was "pytheus-0.0.6.tar", last modified: Wed Apr 12 19:37:37 2023, max compression
```

## Comparing `pytheus-0.0.5.tar` & `pytheus-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-09 01:13:41.662736 pytheus-0.0.5/
--rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.0.5/LICENSE
--rw-r--r--   0 llandy     (501) staff       (20)    12214 2023-04-09 01:13:41.662497 pytheus-0.0.5/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)    11813 2023-04-09 00:43:25.000000 pytheus-0.0.5/README.md
--rw-r--r--   0 llandy     (501) staff       (20)     1037 2023-04-09 01:11:17.000000 pytheus-0.0.5/pyproject.toml
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-09 01:13:41.659371 pytheus-0.0.5/pytheus/
--rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.0.5/pytheus/__init__.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-09 01:13:41.661125 pytheus-0.0.5/pytheus/backends/
--rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.0.5/pytheus/backends/__init__.py
--rw-r--r--   0 llandy     (501) staff       (20)     4148 2023-04-04 00:38:41.000000 pytheus-0.0.5/pytheus/backends/base.py
--rw-r--r--   0 llandy     (501) staff       (20)     3142 2023-04-04 00:38:41.000000 pytheus-0.0.5/pytheus/backends/redis.py
--rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.0.5/pytheus/exceptions.py
--rw-r--r--   0 llandy     (501) staff       (20)     2058 2023-04-02 20:13:46.000000 pytheus-0.0.5/pytheus/exposition.py
--rw-r--r--   0 llandy     (501) staff       (20)    17904 2023-04-08 18:15:41.000000 pytheus-0.0.5/pytheus/metrics.py
--rw-r--r--   0 llandy     (501) staff       (20)     3051 2023-04-03 00:08:23.000000 pytheus-0.0.5/pytheus/registry.py
--rw-r--r--   0 llandy     (501) staff       (20)      173 2023-04-01 23:52:48.000000 pytheus-0.0.5/pytheus/utils.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-09 01:13:41.660329 pytheus-0.0.5/pytheus.egg-info/
--rw-r--r--   0 llandy     (501) staff       (20)    12214 2023-04-09 01:13:41.000000 pytheus-0.0.5/pytheus.egg-info/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)      465 2023-04-09 01:13:41.000000 pytheus-0.0.5/pytheus.egg-info/SOURCES.txt
--rw-r--r--   0 llandy     (501) staff       (20)        1 2023-04-09 01:13:41.000000 pytheus-0.0.5/pytheus.egg-info/dependency_links.txt
--rw-r--r--   0 llandy     (501) staff       (20)      164 2023-04-09 01:13:41.000000 pytheus-0.0.5/pytheus.egg-info/requires.txt
--rw-r--r--   0 llandy     (501) staff       (20)        8 2023-04-09 01:13:41.000000 pytheus-0.0.5/pytheus.egg-info/top_level.txt
--rw-r--r--   0 llandy     (501) staff       (20)       38 2023-04-09 01:13:41.662786 pytheus-0.0.5/setup.cfg
--rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.0.5/setup.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-09 01:13:41.662047 pytheus-0.0.5/tests/
--rw-r--r--   0 llandy     (501) staff       (20)     5852 2023-03-30 23:54:35.000000 pytheus-0.0.5/tests/test_exposition.py
--rw-r--r--   0 llandy     (501) staff       (20)    21760 2023-04-03 00:00:50.000000 pytheus-0.0.5/tests/test_metrics.py
--rw-r--r--   0 llandy     (501) staff       (20)     2892 2023-04-01 00:46:20.000000 pytheus-0.0.5/tests/test_registry.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 19:37:37.113518 pytheus-0.0.6/
+-rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.0.6/LICENSE
+-rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-12 19:37:37.113332 pytheus-0.0.6/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)    12050 2023-04-12 19:36:26.000000 pytheus-0.0.6/README.md
+-rw-r--r--   0 llandy     (501) staff       (20)     1070 2023-04-12 19:37:03.000000 pytheus-0.0.6/pyproject.toml
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 19:37:37.110728 pytheus-0.0.6/pytheus/
+-rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.0.6/pytheus/__init__.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 19:37:37.112212 pytheus-0.0.6/pytheus/backends/
+-rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.0.6/pytheus/backends/__init__.py
+-rw-r--r--   0 llandy     (501) staff       (20)     4148 2023-04-04 00:38:41.000000 pytheus-0.0.6/pytheus/backends/base.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3142 2023-04-04 00:38:41.000000 pytheus-0.0.6/pytheus/backends/redis.py
+-rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.0.6/pytheus/exceptions.py
+-rw-r--r--   0 llandy     (501) staff       (20)     2058 2023-04-11 21:40:44.000000 pytheus-0.0.6/pytheus/exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    18563 2023-04-12 19:31:40.000000 pytheus-0.0.6/pytheus/metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3051 2023-04-03 00:08:23.000000 pytheus-0.0.6/pytheus/registry.py
+-rw-r--r--   0 llandy     (501) staff       (20)      173 2023-04-01 23:52:48.000000 pytheus-0.0.6/pytheus/utils.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 19:37:37.111532 pytheus-0.0.6/pytheus.egg-info/
+-rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-12 19:37:37.000000 pytheus-0.0.6/pytheus.egg-info/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)      465 2023-04-12 19:37:37.000000 pytheus-0.0.6/pytheus.egg-info/SOURCES.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        1 2023-04-12 19:37:37.000000 pytheus-0.0.6/pytheus.egg-info/dependency_links.txt
+-rw-r--r--   0 llandy     (501) staff       (20)      164 2023-04-12 19:37:37.000000 pytheus-0.0.6/pytheus.egg-info/requires.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        8 2023-04-12 19:37:37.000000 pytheus-0.0.6/pytheus.egg-info/top_level.txt
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2023-04-12 19:37:37.113564 pytheus-0.0.6/setup.cfg
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.0.6/setup.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 19:37:37.112750 pytheus-0.0.6/tests/
+-rw-r--r--   0 llandy     (501) staff       (20)     5852 2023-03-30 23:54:35.000000 pytheus-0.0.6/tests/test_exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    22327 2023-04-12 19:31:40.000000 pytheus-0.0.6/tests/test_metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     2892 2023-04-01 00:46:20.000000 pytheus-0.0.6/tests/test_registry.py
```

### Comparing `pytheus-0.0.5/LICENSE` & `pytheus-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.5/PKG-INFO` & `pytheus-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: pytheus
-Version: 0.0.5
+Version: 0.0.6
 Summary: playing with metrics
 Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
-Project-URL: repository, https://github.com/Llandy3d/pytheus
+Project-URL: Homepage, https://github.com/Llandy3d/pytheus
+Project-URL: Documentation, https://pythe.us
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: redis
 Provides-Extra: docs
 License-File: LICENSE
 
 <img src="https://user-images.githubusercontent.com/16627175/185823115-b33905c3-f389-40e1-b830-2197889a936a.png" height="400">
 
 # pytheus
 
-playing with metrics
+*playing with metrics*
+
+---
+
+**Documentation**: https://pythe.us
 
 ---
 
 pytheus is a modern python library for collecting [prometheus](https://prometheus.io/docs/introduction/overview/) metrics built with multiprocessing in mind.
 
 Some of the features are:
 
@@ -245,14 +250,19 @@
 with gauge.time():
     do_something()
 
 # tracking time can also be done as a decorator
 @gauge
 def do_something():
     ...
+
+# tracking progress is also available via decorator with a flag
+@gauge(track_inprogress=True)
+def do_something():
+    ...
 ```
 
 ---
 
 ### Histogram
 
 A histogram samples observations (usually things like request durations or response sizes) and counts them in configurable buckets. It also provides a sum of all observed values. ([taken from prometheus docs](https://prometheus.io/docs/concepts/metric_types/#histogram))
@@ -311,57 +321,59 @@
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.SingleProcessBackend'>
+# <class 'pytheus.backends.base.SingleProcessBackend'>
 print(counter._metric_value_backend.config)
 # {}
 ```
 
 You can define environment configuration to have different defaults, using two environment variables:
 
 ```bash
-export PYTHEUS_BACKEND_CLASS="pytheus.backends.MultiProcessFileBackend"
+export PYTHEUS_BACKEND_CLASS="pytheus.backends.redis.MultiProcessRedisBackend"
 export PYTHEUS_BACKEND_CONFIG="./config.json"
 ```
 
 Now, create the config file, `./config.json`:
 
 ```json
 {
-  "pytheus_file_directory": "./"
+  "host": "127.0.0.1",
+  "port":  6379
 }
 ```
 
 Now we can try the same snippet as above:
 
 ```python
 from pytheus.metrics import Counter
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.MultiProcessFileBackend'>
+# <class 'pytheus.backends.redis.MultiProcessRedisBackend'>
 print(counter._metric_value_backend.config)
-# {'pytheus_file_directory': "./"}
+# {"host": "127.0.0.1", "port":  6379}
 ```
 
 You can also pass the values directly in Python, which would take precedence over the environment
 setup we have just described:
 
 ```python
 
 from pytheus.metrics import Counter
-from pytheus.backends import MultiProcessRedisBackend, load_backend
+from pytheus.backends import load_backend
+from pytheus.backends.redis import MultiProcessRedisBackend
 
 load_backend(
     backend_class=MultiProcessRedisBackend,
     backend_config={
       "host": "127.0.0.1",
       "port":  6379
     }
@@ -373,15 +385,15 @@
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.MultiProcessRedisBackend'>
+# <class 'pytheus.backends.redis.MultiProcessRedisBackend'>
 print(counter._metric_value_backend.config)
 # {'host': '127.0.0.1', 'port': 6379}
 ```
 
 ## Create your own Backend
 
 ### Custom Backend
@@ -409,15 +421,15 @@
 
     def get(self) -> float:
         ...
 ```
 
 ### Initialization hook
 
-It's possible that you want to initialize your custom backed or there are one time steps that you want to happen on import.
+It's possible that you want to initialize your custom backend or there are one time steps that you want to happen on import.
 
 To achieve that you can use the class method hook called `_initialize` that accepts a `BackendConfig` parameter.
 
 ```python
 @classmethod
 def _initialize(cls, config: "BackendConfig") -> None:
     # initialization steps
```

### Comparing `pytheus-0.0.5/README.md` & `pytheus-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 <img src="https://user-images.githubusercontent.com/16627175/185823115-b33905c3-f389-40e1-b830-2197889a936a.png" height="400">
 
 # pytheus
 
-playing with metrics
+*playing with metrics*
+
+---
+
+**Documentation**: https://pythe.us
 
 ---
 
 pytheus is a modern python library for collecting [prometheus](https://prometheus.io/docs/introduction/overview/) metrics built with multiprocessing in mind.
 
 Some of the features are:
 
@@ -231,14 +235,19 @@
 with gauge.time():
     do_something()
 
 # tracking time can also be done as a decorator
 @gauge
 def do_something():
     ...
+
+# tracking progress is also available via decorator with a flag
+@gauge(track_inprogress=True)
+def do_something():
+    ...
 ```
 
 ---
 
 ### Histogram
 
 A histogram samples observations (usually things like request durations or response sizes) and counts them in configurable buckets. It also provides a sum of all observed values. ([taken from prometheus docs](https://prometheus.io/docs/concepts/metric_types/#histogram))
@@ -297,57 +306,59 @@
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.SingleProcessBackend'>
+# <class 'pytheus.backends.base.SingleProcessBackend'>
 print(counter._metric_value_backend.config)
 # {}
 ```
 
 You can define environment configuration to have different defaults, using two environment variables:
 
 ```bash
-export PYTHEUS_BACKEND_CLASS="pytheus.backends.MultiProcessFileBackend"
+export PYTHEUS_BACKEND_CLASS="pytheus.backends.redis.MultiProcessRedisBackend"
 export PYTHEUS_BACKEND_CONFIG="./config.json"
 ```
 
 Now, create the config file, `./config.json`:
 
 ```json
 {
-  "pytheus_file_directory": "./"
+  "host": "127.0.0.1",
+  "port":  6379
 }
 ```
 
 Now we can try the same snippet as above:
 
 ```python
 from pytheus.metrics import Counter
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.MultiProcessFileBackend'>
+# <class 'pytheus.backends.redis.MultiProcessRedisBackend'>
 print(counter._metric_value_backend.config)
-# {'pytheus_file_directory': "./"}
+# {"host": "127.0.0.1", "port":  6379}
 ```
 
 You can also pass the values directly in Python, which would take precedence over the environment
 setup we have just described:
 
 ```python
 
 from pytheus.metrics import Counter
-from pytheus.backends import MultiProcessRedisBackend, load_backend
+from pytheus.backends import load_backend
+from pytheus.backends.redis import MultiProcessRedisBackend
 
 load_backend(
     backend_class=MultiProcessRedisBackend,
     backend_config={
       "host": "127.0.0.1",
       "port":  6379
     }
@@ -359,15 +370,15 @@
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.MultiProcessRedisBackend'>
+# <class 'pytheus.backends.redis.MultiProcessRedisBackend'>
 print(counter._metric_value_backend.config)
 # {'host': '127.0.0.1', 'port': 6379}
 ```
 
 ## Create your own Backend
 
 ### Custom Backend
@@ -395,15 +406,15 @@
 
     def get(self) -> float:
         ...
 ```
 
 ### Initialization hook
 
-It's possible that you want to initialize your custom backed or there are one time steps that you want to happen on import.
+It's possible that you want to initialize your custom backend or there are one time steps that you want to happen on import.
 
 To achieve that you can use the class method hook called `_initialize` that accepts a `BackendConfig` parameter.
 
 ```python
 @classmethod
 def _initialize(cls, config: "BackendConfig") -> None:
     # initialization steps
```

### Comparing `pytheus-0.0.5/pyproject.toml` & `pytheus-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [project]
 name = "pytheus"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Llandy Riveron Del Risco", email="llandy3d@gmail.com" },
 ]
 description = "playing with metrics"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 
 [project.urls]
-repository = "https://github.com/Llandy3d/pytheus"
+Homepage = "https://github.com/Llandy3d/pytheus"
+Documentation = "https://pythe.us"
 
 [project.optional-dependencies]
 test = [
   "pytest >= 7.0.0",
   "mypy == 1.1.1",
   "ruff == 0.0.260",
   "black == 23.3.0",
```

### Comparing `pytheus-0.0.5/pytheus/backends/base.py` & `pytheus-0.0.6/pytheus/backends/base.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.5/pytheus/backends/redis.py` & `pytheus-0.0.6/pytheus/backends/redis.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.5/pytheus/exposition.py` & `pytheus-0.0.6/pytheus/exposition.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.5/pytheus/metrics.py` & `pytheus-0.0.6/pytheus/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,18 @@
     @name.setter
     def name(self, value: str) -> None:
         pass
 
 
 class _MetricCollector:
     """
-    #TODO
+    This handles the core logic for a specific named metric.
+    It will do label validation, it will have the metric name and most importantly it will keep
+    track of all the Child instances so that when `collect()` is called it will retrieve all
+    the correct samples from all the possible observable Childrens.
     _labeled_metrics contains all observable metrics when required_labels is set.
     """
 
     def __init__(
         self,
         name: str,
         description: str,
@@ -371,26 +374,33 @@
         Will increase the gauge value when entered and decrease it when exited.
         """
         self._raise_if_cannot_observe()
         self.inc()
         yield
         self.dec()
 
-    # TODO: this could be configured to allow the decoration to be used
-    # with track_inprogress giving more flexibility.
-    def __call__(self, func: Callable) -> Callable:
+    def __call__(self, func: Callable | None = None, track_inprogress: bool = False) -> Callable:
         """
         When called acts as a decorator tracking the time taken by
         the wrapped function.
+
+        If passing the parameter `track_inprogress` as `True` it will instead increase while the
+        function is running and will decrease when it's finished.
         """
+        if func is None:
+            return functools.partial(self.__call__, track_inprogress=track_inprogress)
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):  # type: ignore
-            with self.time():
-                return func(*args, **kwargs)
+            if track_inprogress:
+                with self.track_inprogress():
+                    return func(*args, **kwargs)
+            else:
+                with self.time():
+                    return func(*args, **kwargs)
 
         return wrapper
 
     @contextmanager
     def time(self) -> Generator[None, None, None]:
         """
         Times the duration inside of it and sets the value.
```

### Comparing `pytheus-0.0.5/pytheus/registry.py` & `pytheus-0.0.6/pytheus/registry.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.5/pytheus.egg-info/PKG-INFO` & `pytheus-0.0.6/pytheus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: pytheus
-Version: 0.0.5
+Version: 0.0.6
 Summary: playing with metrics
 Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
-Project-URL: repository, https://github.com/Llandy3d/pytheus
+Project-URL: Homepage, https://github.com/Llandy3d/pytheus
+Project-URL: Documentation, https://pythe.us
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: redis
 Provides-Extra: docs
 License-File: LICENSE
 
 <img src="https://user-images.githubusercontent.com/16627175/185823115-b33905c3-f389-40e1-b830-2197889a936a.png" height="400">
 
 # pytheus
 
-playing with metrics
+*playing with metrics*
+
+---
+
+**Documentation**: https://pythe.us
 
 ---
 
 pytheus is a modern python library for collecting [prometheus](https://prometheus.io/docs/introduction/overview/) metrics built with multiprocessing in mind.
 
 Some of the features are:
 
@@ -245,14 +250,19 @@
 with gauge.time():
     do_something()
 
 # tracking time can also be done as a decorator
 @gauge
 def do_something():
     ...
+
+# tracking progress is also available via decorator with a flag
+@gauge(track_inprogress=True)
+def do_something():
+    ...
 ```
 
 ---
 
 ### Histogram
 
 A histogram samples observations (usually things like request durations or response sizes) and counts them in configurable buckets. It also provides a sum of all observed values. ([taken from prometheus docs](https://prometheus.io/docs/concepts/metric_types/#histogram))
@@ -311,57 +321,59 @@
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.SingleProcessBackend'>
+# <class 'pytheus.backends.base.SingleProcessBackend'>
 print(counter._metric_value_backend.config)
 # {}
 ```
 
 You can define environment configuration to have different defaults, using two environment variables:
 
 ```bash
-export PYTHEUS_BACKEND_CLASS="pytheus.backends.MultiProcessFileBackend"
+export PYTHEUS_BACKEND_CLASS="pytheus.backends.redis.MultiProcessRedisBackend"
 export PYTHEUS_BACKEND_CONFIG="./config.json"
 ```
 
 Now, create the config file, `./config.json`:
 
 ```json
 {
-  "pytheus_file_directory": "./"
+  "host": "127.0.0.1",
+  "port":  6379
 }
 ```
 
 Now we can try the same snippet as above:
 
 ```python
 from pytheus.metrics import Counter
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.MultiProcessFileBackend'>
+# <class 'pytheus.backends.redis.MultiProcessRedisBackend'>
 print(counter._metric_value_backend.config)
-# {'pytheus_file_directory': "./"}
+# {"host": "127.0.0.1", "port":  6379}
 ```
 
 You can also pass the values directly in Python, which would take precedence over the environment
 setup we have just described:
 
 ```python
 
 from pytheus.metrics import Counter
-from pytheus.backends import MultiProcessRedisBackend, load_backend
+from pytheus.backends import load_backend
+from pytheus.backends.redis import MultiProcessRedisBackend
 
 load_backend(
     backend_class=MultiProcessRedisBackend,
     backend_config={
       "host": "127.0.0.1",
       "port":  6379
     }
@@ -373,15 +385,15 @@
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.MultiProcessRedisBackend'>
+# <class 'pytheus.backends.redis.MultiProcessRedisBackend'>
 print(counter._metric_value_backend.config)
 # {'host': '127.0.0.1', 'port': 6379}
 ```
 
 ## Create your own Backend
 
 ### Custom Backend
@@ -409,15 +421,15 @@
 
     def get(self) -> float:
         ...
 ```
 
 ### Initialization hook
 
-It's possible that you want to initialize your custom backed or there are one time steps that you want to happen on import.
+It's possible that you want to initialize your custom backend or there are one time steps that you want to happen on import.
 
 To achieve that you can use the class method hook called `_initialize` that accepts a `BackendConfig` parameter.
 
 ```python
 @classmethod
 def _initialize(cls, config: "BackendConfig") -> None:
     # initialization steps
```

### Comparing `pytheus-0.0.5/tests/test_exposition.py` & `pytheus-0.0.6/tests/test_exposition.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.5/tests/test_metrics.py` & `pytheus-0.0.6/tests/test_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+from unittest import mock
 
 import pytest
 
 from pytheus.exceptions import (
     BucketException,
     LabelValidationException,
     UnobservableMetricException,
@@ -444,14 +445,34 @@
         @gauge
         def test():
             pass
 
         test()
         assert gauge._metric_value_backend.get() != 0
 
+    def test_as_decorator_with_track_inprogress(self, gauge):
+        backend_mock = mock.Mock()
+        gauge._metric_value_backend = backend_mock
+
+        @gauge(track_inprogress=True)
+        def test():
+            pass
+
+        test()
+        backend_mock.inc.assert_called()
+        backend_mock.dec.assert_called()
+
+    def test_as_decorator_with_track_inprogress_as_false(self, gauge):
+        @gauge(track_inprogress=False)
+        def test():
+            pass
+
+        test()
+        assert gauge._metric_value_backend.get() != 0
+
 
 class TestHistogram:
     @pytest.fixture
     def histogram(self):
         return Histogram("name", "desc")
 
     def test_metric_type(self, histogram):
```

### Comparing `pytheus-0.0.5/tests/test_registry.py` & `pytheus-0.0.6/tests/test_registry.py`

 * *Files identical despite different names*

