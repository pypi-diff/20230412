# Comparing `tmp/redis-metric-helper-0.1.tar.gz` & `tmp/redis-metric-helper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-metric-helper-0.1.tar", last modified: Wed Apr 12 08:10:53 2023, max compression
+gzip compressed data, was "redis-metric-helper-0.1.1.tar", last modified: Wed Apr 12 11:37:37 2023, max compression
```

## Comparing `redis-metric-helper-0.1.tar` & `redis-metric-helper-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 08:10:53.361383 redis-metric-helper-0.1/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.1/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1003 2023-04-12 08:10:53.361383 redis-metric-helper-0.1/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.1/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 08:10:53.357383 redis-metric-helper-0.1/metric_helper/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2487 2023-04-12 08:07:26.000000 redis-metric-helper-0.1/metric_helper/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6532 2023-04-12 08:07:44.000000 redis-metric-helper-0.1/metric_helper/base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      382 2023-04-04 10:58:15.000000 redis-metric-helper-0.1/metric_helper/conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      541 2023-04-12 08:07:01.000000 redis-metric-helper-0.1/metric_helper/connections.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.1/metric_helper/exceptions.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 08:10:53.361383 redis-metric-helper-0.1/redis_metric_helper.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1003 2023-04-12 08:10:53.000000 redis-metric-helper-0.1/redis_metric_helper.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      367 2023-04-12 08:10:53.000000 redis-metric-helper-0.1/redis_metric_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-12 08:10:53.000000 redis-metric-helper-0.1/redis_metric_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-12 08:10:53.000000 redis-metric-helper-0.1/redis_metric_helper.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-04-12 08:10:53.000000 redis-metric-helper-0.1/redis_metric_helper.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-12 08:10:53.361383 redis-metric-helper-0.1/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.1/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 11:37:37.428725 redis-metric-helper-0.1.1/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.1.1/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-12 11:37:37.428725 redis-metric-helper-0.1.1/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.1.1/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 11:37:37.428725 redis-metric-helper-0.1.1/metric_helper/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2489 2023-04-12 11:36:53.000000 redis-metric-helper-0.1.1/metric_helper/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6532 2023-04-12 08:54:36.000000 redis-metric-helper-0.1.1/metric_helper/base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      398 2023-04-12 11:36:36.000000 redis-metric-helper-0.1.1/metric_helper/conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      541 2023-04-12 08:07:01.000000 redis-metric-helper-0.1.1/metric_helper/connections.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.1.1/metric_helper/exceptions.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 11:37:37.428725 redis-metric-helper-0.1.1/redis_metric_helper.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-12 11:37:37.000000 redis-metric-helper-0.1.1/redis_metric_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      367 2023-04-12 11:37:37.000000 redis-metric-helper-0.1.1/redis_metric_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-12 11:37:37.000000 redis-metric-helper-0.1.1/redis_metric_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-12 11:37:37.000000 redis-metric-helper-0.1.1/redis_metric_helper.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-04-12 11:37:37.000000 redis-metric-helper-0.1.1/redis_metric_helper.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-12 11:37:37.428725 redis-metric-helper-0.1.1/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.1.1/setup.py
```

### Comparing `redis-metric-helper-0.1/LICENSE` & `redis-metric-helper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.1/PKG-INFO` & `redis-metric-helper-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.1
+Version: 0.1.1
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.1/metric_helper/__init__.py` & `redis-metric-helper-0.1.1/metric_helper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from metric_helper.conf import settings
 from metric_helper.base import Timeseries, Counter, Gauge, PositiveGauge
 from metric_helper.connections import get_redis_connection
 from metric_helper.exceptions import MetricNotFound
 
 
-__version__ = '0.1'
+__version__ = '0.1.1'
 
 
 
 
 metric_classes = [
     Timeseries,
     Counter,
```

### Comparing `redis-metric-helper-0.1/metric_helper/base.py` & `redis-metric-helper-0.1.1/metric_helper/base.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.1/metric_helper/connections.py` & `redis-metric-helper-0.1.1/metric_helper/connections.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.1/redis_metric_helper.egg-info/PKG-INFO` & `redis-metric-helper-0.1.1/redis_metric_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.1
+Version: 0.1.1
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.1/setup.py` & `redis-metric-helper-0.1.1/setup.py`

 * *Files identical despite different names*

