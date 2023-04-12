# Comparing `tmp/redis-metric-helper-0.1.1.tar.gz` & `tmp/redis-metric-helper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-metric-helper-0.1.1.tar", last modified: Wed Apr 12 11:37:37 2023, max compression
+gzip compressed data, was "redis-metric-helper-0.1.2.tar", last modified: Wed Apr 12 14:02:26 2023, max compression
```

## Comparing `redis-metric-helper-0.1.1.tar` & `redis-metric-helper-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 11:37:37.428725 redis-metric-helper-0.1.1/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.1.1/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-12 11:37:37.428725 redis-metric-helper-0.1.1/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.1.1/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 11:37:37.428725 redis-metric-helper-0.1.1/metric_helper/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2489 2023-04-12 11:36:53.000000 redis-metric-helper-0.1.1/metric_helper/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6532 2023-04-12 08:54:36.000000 redis-metric-helper-0.1.1/metric_helper/base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      398 2023-04-12 11:36:36.000000 redis-metric-helper-0.1.1/metric_helper/conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      541 2023-04-12 08:07:01.000000 redis-metric-helper-0.1.1/metric_helper/connections.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.1.1/metric_helper/exceptions.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 11:37:37.428725 redis-metric-helper-0.1.1/redis_metric_helper.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-12 11:37:37.000000 redis-metric-helper-0.1.1/redis_metric_helper.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      367 2023-04-12 11:37:37.000000 redis-metric-helper-0.1.1/redis_metric_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-12 11:37:37.000000 redis-metric-helper-0.1.1/redis_metric_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-12 11:37:37.000000 redis-metric-helper-0.1.1/redis_metric_helper.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-04-12 11:37:37.000000 redis-metric-helper-0.1.1/redis_metric_helper.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-12 11:37:37.428725 redis-metric-helper-0.1.1/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.1.1/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:02:26.787831 redis-metric-helper-0.1.2/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.1.2/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-12 14:02:26.787831 redis-metric-helper-0.1.2/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.1.2/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:02:26.783831 redis-metric-helper-0.1.2/metric_helper/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2489 2023-04-12 14:01:46.000000 redis-metric-helper-0.1.2/metric_helper/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6532 2023-04-12 08:54:36.000000 redis-metric-helper-0.1.2/metric_helper/base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      464 2023-04-12 14:01:26.000000 redis-metric-helper-0.1.2/metric_helper/conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      587 2023-04-12 14:01:20.000000 redis-metric-helper-0.1.2/metric_helper/connections.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.1.2/metric_helper/exceptions.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:02:26.787831 redis-metric-helper-0.1.2/redis_metric_helper.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-12 14:02:26.000000 redis-metric-helper-0.1.2/redis_metric_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      367 2023-04-12 14:02:26.000000 redis-metric-helper-0.1.2/redis_metric_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-12 14:02:26.000000 redis-metric-helper-0.1.2/redis_metric_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-12 14:02:26.000000 redis-metric-helper-0.1.2/redis_metric_helper.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-04-12 14:02:26.000000 redis-metric-helper-0.1.2/redis_metric_helper.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-12 14:02:26.787831 redis-metric-helper-0.1.2/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.1.2/setup.py
```

### Comparing `redis-metric-helper-0.1.1/LICENSE` & `redis-metric-helper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.1.1/PKG-INFO` & `redis-metric-helper-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.1.1/metric_helper/__init__.py` & `redis-metric-helper-0.1.2/metric_helper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from metric_helper.conf import settings
 from metric_helper.base import Timeseries, Counter, Gauge, PositiveGauge
 from metric_helper.connections import get_redis_connection
 from metric_helper.exceptions import MetricNotFound
 
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 
 
 
 metric_classes = [
     Timeseries,
     Counter,
```

### Comparing `redis-metric-helper-0.1.1/metric_helper/base.py` & `redis-metric-helper-0.1.2/metric_helper/base.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.1.1/metric_helper/connections.py` & `redis-metric-helper-0.1.2/metric_helper/connections.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 class RedisWrapper:
 
     def __init__(self):
         self.redis = StrictRedis(
             host=settings.REDIS_HOST,
             port=settings.REDIS_PORT,
+            password=settings.REDIS_PASSWORD,
             db=0,
             decode_responses=True,
         )
 
 
     def get_connection(self):
         return self.redis
```

### Comparing `redis-metric-helper-0.1.1/redis_metric_helper.egg-info/PKG-INFO` & `redis-metric-helper-0.1.2/redis_metric_helper.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.1.1/setup.py` & `redis-metric-helper-0.1.2/setup.py`

 * *Files identical despite different names*

