# Comparing `tmp/redis-metric-helper-0.1.2.tar.gz` & `tmp/redis-metric-helper-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-metric-helper-0.1.2.tar", last modified: Wed Apr 12 14:02:26 2023, max compression
+gzip compressed data, was "redis-metric-helper-0.2.tar", last modified: Wed Apr 12 14:11:12 2023, max compression
```

## Comparing `redis-metric-helper-0.1.2.tar` & `redis-metric-helper-0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:02:26.787831 redis-metric-helper-0.1.2/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.1.2/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-12 14:02:26.787831 redis-metric-helper-0.1.2/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.1.2/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:02:26.783831 redis-metric-helper-0.1.2/metric_helper/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2489 2023-04-12 14:01:46.000000 redis-metric-helper-0.1.2/metric_helper/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6532 2023-04-12 08:54:36.000000 redis-metric-helper-0.1.2/metric_helper/base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      464 2023-04-12 14:01:26.000000 redis-metric-helper-0.1.2/metric_helper/conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      587 2023-04-12 14:01:20.000000 redis-metric-helper-0.1.2/metric_helper/connections.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.1.2/metric_helper/exceptions.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:02:26.787831 redis-metric-helper-0.1.2/redis_metric_helper.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-12 14:02:26.000000 redis-metric-helper-0.1.2/redis_metric_helper.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      367 2023-04-12 14:02:26.000000 redis-metric-helper-0.1.2/redis_metric_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-12 14:02:26.000000 redis-metric-helper-0.1.2/redis_metric_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-12 14:02:26.000000 redis-metric-helper-0.1.2/redis_metric_helper.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-04-12 14:02:26.000000 redis-metric-helper-0.1.2/redis_metric_helper.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-12 14:02:26.787831 redis-metric-helper-0.1.2/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.1.2/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:11:12.480736 redis-metric-helper-0.2/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.2/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1003 2023-04-12 14:11:12.480736 redis-metric-helper-0.2/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.2/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:11:12.476736 redis-metric-helper-0.2/metric_helper/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       20 2023-04-12 14:10:31.000000 redis-metric-helper-0.2/metric_helper/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     6532 2023-04-12 08:54:36.000000 redis-metric-helper-0.2/metric_helper/base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      464 2023-04-12 14:01:26.000000 redis-metric-helper-0.2/metric_helper/conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      587 2023-04-12 14:01:20.000000 redis-metric-helper-0.2/metric_helper/connections.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.2/metric_helper/exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2463 2023-04-12 14:09:16.000000 redis-metric-helper-0.2/metric_helper/registry.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-12 14:11:12.480736 redis-metric-helper-0.2/redis_metric_helper.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1003 2023-04-12 14:11:12.000000 redis-metric-helper-0.2/redis_metric_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      393 2023-04-12 14:11:12.000000 redis-metric-helper-0.2/redis_metric_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-12 14:11:12.000000 redis-metric-helper-0.2/redis_metric_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-12 14:11:12.000000 redis-metric-helper-0.2/redis_metric_helper.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-04-12 14:11:12.000000 redis-metric-helper-0.2/redis_metric_helper.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-12 14:11:12.480736 redis-metric-helper-0.2/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.2/setup.py
```

### Comparing `redis-metric-helper-0.1.2/LICENSE` & `redis-metric-helper-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.1.2/PKG-INFO` & `redis-metric-helper-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.1.2
+Version: 0.2
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.1.2/metric_helper/__init__.py` & `redis-metric-helper-0.2/metric_helper/registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 from metric_helper.conf import settings
 from metric_helper.base import Timeseries, Counter, Gauge, PositiveGauge
 from metric_helper.connections import get_redis_connection
 from metric_helper.exceptions import MetricNotFound
 
 
-__version__ = '0.1.2'
-
-
-
-
 metric_classes = [
     Timeseries,
     Counter,
     Gauge,
     PositiveGauge,
 ]
 # These string names may not change unless extreme caution is used
```

### Comparing `redis-metric-helper-0.1.2/metric_helper/base.py` & `redis-metric-helper-0.2/metric_helper/base.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.1.2/metric_helper/connections.py` & `redis-metric-helper-0.2/metric_helper/connections.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.1.2/redis_metric_helper.egg-info/PKG-INFO` & `redis-metric-helper-0.2/redis_metric_helper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.1.2
+Version: 0.2
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.1.2/setup.py` & `redis-metric-helper-0.2/setup.py`

 * *Files identical despite different names*

