# Comparing `tmp/redis-metric-helper-0.2.tar.gz` & `tmp/redis-metric-helper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-metric-helper-0.2.tar", last modified: Wed Apr 12 14:11:12 2023, max compression
+gzip compressed data, was "redis-metric-helper-0.2.1.tar", last modified: Wed Apr 12 14:39:03 2023, max compression
```

## Comparing `redis-metric-helper-0.2.tar` & `redis-metric-helper-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:11:12.480736 redis-metric-helper-0.2/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.2/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1003 2023-04-12 14:11:12.480736 redis-metric-helper-0.2/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.2/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:11:12.476736 redis-metric-helper-0.2/metric_helper/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       20 2023-04-12 14:10:31.000000 redis-metric-helper-0.2/metric_helper/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6532 2023-04-12 08:54:36.000000 redis-metric-helper-0.2/metric_helper/base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      464 2023-04-12 14:01:26.000000 redis-metric-helper-0.2/metric_helper/conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      587 2023-04-12 14:01:20.000000 redis-metric-helper-0.2/metric_helper/connections.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.2/metric_helper/exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2463 2023-04-12 14:09:16.000000 redis-metric-helper-0.2/metric_helper/registry.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:11:12.480736 redis-metric-helper-0.2/redis_metric_helper.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1003 2023-04-12 14:11:12.000000 redis-metric-helper-0.2/redis_metric_helper.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      393 2023-04-12 14:11:12.000000 redis-metric-helper-0.2/redis_metric_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-12 14:11:12.000000 redis-metric-helper-0.2/redis_metric_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-12 14:11:12.000000 redis-metric-helper-0.2/redis_metric_helper.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-04-12 14:11:12.000000 redis-metric-helper-0.2/redis_metric_helper.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-12 14:11:12.480736 redis-metric-helper-0.2/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.2/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:39:03.271892 redis-metric-helper-0.2.1/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.2.1/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-12 14:39:03.267892 redis-metric-helper-0.2.1/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.2.1/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:39:03.267892 redis-metric-helper-0.2.1/metric_helper/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-12 14:37:07.000000 redis-metric-helper-0.2.1/metric_helper/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6649 2023-04-12 14:36:53.000000 redis-metric-helper-0.2.1/metric_helper/base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      464 2023-04-12 14:01:26.000000 redis-metric-helper-0.2.1/metric_helper/conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      587 2023-04-12 14:01:20.000000 redis-metric-helper-0.2.1/metric_helper/connections.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.2.1/metric_helper/exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2463 2023-04-12 14:09:16.000000 redis-metric-helper-0.2.1/metric_helper/registry.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:39:03.267892 redis-metric-helper-0.2.1/redis_metric_helper.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-12 14:39:03.000000 redis-metric-helper-0.2.1/redis_metric_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      393 2023-04-12 14:39:03.000000 redis-metric-helper-0.2.1/redis_metric_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-12 14:39:03.000000 redis-metric-helper-0.2.1/redis_metric_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-12 14:39:03.000000 redis-metric-helper-0.2.1/redis_metric_helper.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-04-12 14:39:03.000000 redis-metric-helper-0.2.1/redis_metric_helper.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-12 14:39:03.271892 redis-metric-helper-0.2.1/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.2.1/setup.py
```

### Comparing `redis-metric-helper-0.2/LICENSE` & `redis-metric-helper-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.2/PKG-INFO` & `redis-metric-helper-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.2
+Version: 0.2.1
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.2/metric_helper/base.py` & `redis-metric-helper-0.2.1/metric_helper/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 
     def __init__(self, name):
         self.key = name
         self.name = name
         self.redis = get_redis_connection()
         self.ts = self.redis.ts()
-        self.retention_msecs = settings.TIMESERIES_RETENTION_MSECS
-        self.retention_seconds = self.retention_msecs / 1000
+        self.retention_msecs = int(settings.TIMESERIES_RETENTION_MSECS)
+        self.retention_seconds = int(self.retention_msecs / 1000)
 
 
     def handle_write_kwargs(self, **kwargs):
         value = kwargs.get('value', None)
         if not value:
             raise ValueError('You must provide a value for the metric write method.')
         labels = kwargs.get('labels', {})
@@ -242,14 +242,19 @@
             amount=amount,
         )
         self.expire()
 
 
     def decr(self, amount=1, **kwargs):
         current_value = self.redis.get(self.key)
+        try:
+            current_value = int(current_value)
+        except:
+            current_value = 0
+
         if current_value <= 0:
             # Don't decrement this value.
             # A positive gauge cannot be smaller than 0.
             return
         self.redis.decr(
             self.key,
             amount=amount,
```

### Comparing `redis-metric-helper-0.2/metric_helper/connections.py` & `redis-metric-helper-0.2.1/metric_helper/connections.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.2/metric_helper/registry.py` & `redis-metric-helper-0.2.1/metric_helper/registry.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.2/redis_metric_helper.egg-info/PKG-INFO` & `redis-metric-helper-0.2.1/redis_metric_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.2
+Version: 0.2.1
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.2/setup.py` & `redis-metric-helper-0.2.1/setup.py`

 * *Files identical despite different names*

