# Comparing `tmp/snyk-metrics-0.0.3.tar.gz` & `tmp/snyk_metrics-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snyk-metrics-0.0.3.tar", max compression
+gzip compressed data, was "snyk_metrics-0.0.4.tar", max compression
```

## Comparing `snyk-metrics-0.0.3.tar` & `snyk_metrics-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      550 2022-08-11 13:47:07.208047 snyk-metrics-0.0.3/LICENSE
--rw-r--r--   0        0        0     2113 2022-08-11 13:47:07.208047 snyk-metrics-0.0.3/README.md
--rw-r--r--   0        0        0     1039 2022-08-11 13:47:07.208047 snyk-metrics-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2242 2022-08-11 13:47:07.208047 snyk-metrics-0.0.3/snyk_metrics/__init__.py
--rw-r--r--   0        0        0     5779 2022-08-11 13:47:07.208047 snyk-metrics-0.0.3/snyk_metrics/client.py
--rw-r--r--   0        0        0        0 2022-08-11 13:47:07.208047 snyk-metrics-0.0.3/snyk_metrics/clients/__init__.py
--rw-r--r--   0        0        0      719 2022-08-11 13:47:07.208047 snyk-metrics-0.0.3/snyk_metrics/clients/base.py
--rw-r--r--   0        0        0     1009 2022-08-11 13:47:07.208047 snyk-metrics-0.0.3/snyk_metrics/clients/dogstatsd.py
--rw-r--r--   0        0        0     4113 2022-08-11 13:47:07.208047 snyk-metrics-0.0.3/snyk_metrics/clients/prometheus.py
--rw-r--r--   0        0        0      587 2022-08-11 13:47:07.208047 snyk-metrics-0.0.3/snyk_metrics/exceptions.py
--rw-r--r--   0        0        0     1784 2022-08-11 13:47:07.208047 snyk-metrics-0.0.3/snyk_metrics/metrics.py
--rw-r--r--   0        0        0     2993 2022-08-11 13:47:15.448847 snyk-metrics-0.0.3/setup.py
--rw-r--r--   0        0        0     2979 2022-08-11 13:47:15.449151 snyk-metrics-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      550 2023-04-12 11:10:18.506756 snyk_metrics-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2113 2023-04-12 11:10:18.506756 snyk_metrics-0.0.4/README.md
+-rw-r--r--   0        0        0     1039 2023-04-12 11:10:18.506756 snyk_metrics-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2242 2023-04-12 11:10:18.506756 snyk_metrics-0.0.4/snyk_metrics/__init__.py
+-rw-r--r--   0        0        0     6118 2023-04-12 11:10:18.506756 snyk_metrics-0.0.4/snyk_metrics/client.py
+-rw-r--r--   0        0        0        0 2023-04-12 11:10:18.506756 snyk_metrics-0.0.4/snyk_metrics/clients/__init__.py
+-rw-r--r--   0        0        0      903 2023-04-12 11:10:18.506756 snyk_metrics-0.0.4/snyk_metrics/clients/base.py
+-rw-r--r--   0        0        0     1288 2023-04-12 11:10:18.506756 snyk_metrics-0.0.4/snyk_metrics/clients/dogstatsd.py
+-rw-r--r--   0        0        0     4584 2023-04-12 11:10:18.506756 snyk_metrics-0.0.4/snyk_metrics/clients/prometheus.py
+-rw-r--r--   0        0        0      587 2023-04-12 11:10:18.506756 snyk_metrics-0.0.4/snyk_metrics/exceptions.py
+-rw-r--r--   0        0        0     2563 2023-04-12 11:10:18.506756 snyk_metrics-0.0.4/snyk_metrics/metrics.py
+-rw-r--r--   0        0        0     2997 1970-01-01 00:00:00.000000 snyk_metrics-0.0.4/setup.py
+-rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 snyk_metrics-0.0.4/PKG-INFO
```

### Comparing `snyk-metrics-0.0.3/LICENSE` & `snyk_metrics-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snyk-metrics-0.0.3/README.md` & `snyk_metrics-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `snyk-metrics-0.0.3/pyproject.toml` & `snyk_metrics-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snyk-metrics"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python library to interact transparently with Prometheus, Pushgateway and Dogstatsd."
 authors = ["Snyk Security R&D <security-engineering@snyk.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/snyk/python-metrics"
 repository = "https://github.com/snyk/python-metrics"
 keywords = ["prometheus", "datadog", "metrics"]
```

### Comparing `snyk-metrics-0.0.3/snyk_metrics/__init__.py` & `snyk_metrics-0.0.4/snyk_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `snyk-metrics-0.0.3/snyk_metrics/client.py` & `snyk_metrics-0.0.4/snyk_metrics/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         dogstatsd_enabled: bool = False,
         dogstatsd_agent_host: str = "datadog",
         dogstatsd_port: int = 8125,
         prometheus_registry: CollectorRegistry = REGISTRY,
         raise_exceptions: bool = True,
         lock_registry: bool = False,
     ):
-
         self._raise_exceptions = raise_exceptions
         self._prometheus_client = (
             PrometheusClient(
                 pushgateway_enabled=pushgateway_enabled,
                 pushgateway_host=pushgateway_host,
                 pushgateway_port=pushgateway_port,
                 pushgateway_job_name=pushgateway_job_name,
@@ -163,7 +162,15 @@
     @_exception_handler
     def set_gauge_value(
         self, metric: Metric, labels: Optional[Dict[str, Any]] = None, value: float = 0.0
     ) -> None:
         self._validate_metric(metric, MetricTypes.GAUGE, labels)
         for client in self._enabled_clients:
             client.set_gauge_value(metric.name, labels, value)
+
+    @_exception_handler
+    def set_histogram_value(
+        self, metric: Metric, labels: Optional[Dict[str, Any]] = None, value: float = 0.0
+    ) -> None:
+        self._validate_metric(metric, MetricTypes.HISTOGRAM, labels)
+        for client in self._enabled_clients:
+            client.set_histogram_value(metric.name, labels, value)
```

### Comparing `snyk-metrics-0.0.3/snyk_metrics/clients/base.py` & `snyk_metrics-0.0.4/snyk_metrics/clients/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,20 @@
     @abstractmethod
     def set_gauge_value(
         self, name: str, labels: Optional[Dict[str, Any]] = None, value: float = 0.0
     ) -> None:
         raise NotImplementedError
 
     @abstractmethod
+    def set_histogram_value(
+        self, name: str, labels: Optional[Dict[str, Any]] = None, value: float = 0.0
+    ) -> None:
+        raise NotImplementedError
+
+    @abstractmethod
     def register_metric(
         self,
         metric_type: str,
         name: str,
         documentation: str,
         label_names: Optional[Tuple[str, ...]] = None,
     ) -> None:
```

### Comparing `snyk-metrics-0.0.3/snyk_metrics/clients/dogstatsd.py` & `snyk_metrics-0.0.4/snyk_metrics/clients/dogstatsd.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 
     def set_gauge_value(
         self, name: str, labels: Optional[Dict[str, str]] = None, value: float = 0.0
     ) -> None:
         tags = [f"{key}:{value}" for key, value in labels.items()] if labels else None
         statsd.gauge(metric=name, tags=tags, value=value)
 
+    def set_histogram_value(
+        self, name: str, labels: Optional[Dict[str, str]] = None, value: float = 0.0
+    ) -> None:
+        tags = [f"{key}:{value}" for key, value in labels.items()] if labels else None
+        statsd.histogram(metric=name, tags=tags, value=value)
+
     def register_metric(
         self,
         metric_type: str,
         name: str,
         documentation: str,
         label_names: Optional[Tuple[str, ...]] = None,
     ) -> None:
```

### Comparing `snyk-metrics-0.0.3/snyk_metrics/clients/prometheus.py` & `snyk_metrics-0.0.4/snyk_metrics/clients/prometheus.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     def register_metric(
         self,
         metric_type: str,
         name: str,
         documentation: str,
         label_names: Optional[Tuple[str, ...]] = None,
     ) -> PrometheusMetric:
-
         metric = PROMETHEUS_METRIC_CLASS_MAP[metric_type](
             name=name,
             documentation=documentation,
             labelnames=label_names or (),
             registry=self._registry,
         )
         if self.pushgateway_enabled:
@@ -122,7 +121,19 @@
         gauge = self._get_registered_metric("gauge", name, label_names)
         gauge.labels(**labels).set(value) if labels else gauge.set(value)
 
         if self.pushgateway_enabled:
             self._push_to_gateway()
 
         return
+
+    def set_histogram_value(
+        self, name: str, labels: Optional[Dict[str, Any]] = None, value: float = 0.0
+    ) -> None:
+        label_names: Optional[Tuple[str, ...]] = tuple(labels.keys()) if labels else None
+        histogram = self._get_registered_metric("histogram", name, label_names)
+        histogram.labels(**labels).set(value) if labels else histogram.set(value)
+
+        if self.pushgateway_enabled:
+            self._push_to_gateway()
+
+        return
```

### Comparing `snyk-metrics-0.0.3/snyk_metrics/exceptions.py` & `snyk_metrics-0.0.4/snyk_metrics/exceptions.py`

 * *Files identical despite different names*

### Comparing `snyk-metrics-0.0.3/snyk_metrics/metrics.py` & `snyk_metrics-0.0.4/snyk_metrics/metrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 logger = logging.getLogger(__name__)
 
 
 class Counter(Metric):
     def __init__(
         self, name: str, documentation: str, label_names: Optional[Tuple[str, ...]] = None
     ):
-
         super().__init__(
             metric_type=MetricTypes.COUNTER,
             name=name,
             documentation=documentation,
             label_names=label_names,
         )
 
@@ -36,15 +35,14 @@
         self._client.increment_counter(self, value=value, labels=labels)
 
 
 class Gauge(Metric):
     def __init__(
         self, name: str, documentation: str, label_names: Optional[Tuple[str, ...]] = None
     ):
-
         super().__init__(
             metric_type=MetricTypes.GAUGE,
             name=name,
             documentation=documentation,
             label_names=label_names,
         )
 
@@ -57,7 +55,33 @@
             pass
 
     def set_value(self, value: float = 0.0, labels: Optional[Dict[str, Any]] = None) -> None:
         if not self._client:
             self._client = get_client()
 
         self._client.set_gauge_value(self, value=value, labels=labels)
+
+
+class Histogram(Metric):
+    def __init__(
+        self, name: str, documentation: str, label_names: Optional[Tuple[str, ...]] = None
+    ):
+        super().__init__(
+            metric_type=MetricTypes.HISTOGRAM,
+            name=name,
+            documentation=documentation,
+            label_names=label_names,
+        )
+
+        self._client: Optional[MetricsClient] = None
+
+        try:
+            self._client = get_client()
+            self._client.register_metric(self)
+        except ClientNotInitialisedError:
+            pass
+
+    def set_value(self, value: float = 0.0, labels: Optional[Dict[str, Any]] = None) -> None:
+        if not self._client:
+            self._client = get_client()
+
+        self._client.set_histogram_value(self, value=value, labels=labels)
```

### Comparing `snyk-metrics-0.0.3/setup.py` & `snyk_metrics-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 {'': ['*']}
 
 install_requires = \
 ['datadog>=0.43.0,<0.44.0', 'prometheus-client>=0.12.0,<0.13.0']
 
 setup_kwargs = {
     'name': 'snyk-metrics',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Python library to interact transparently with Prometheus, Pushgateway and Dogstatsd.',
     'long_description': '# snyk-python-metrics\n\nPython library to interact transparently with Prometheus, Pushgateway and\nDogstatsd.\n\n## Usage\n\nThe client can be used with two different approaches, one more opinionated and\nstructured, with all the metrics created and registered at the creation of the\nclient, and one more flexible, where metrics can be registered at any time.\n\nThe first approach should help keeping the application using this client cleaner\nand the metrics management in a centralised place.\n\n### Example 1 - "Locked Registry"\n\nIn this example all the metrics used by the application are registered as part\nof the client initialisation.\n\nExample:\n\n```python\n# my_app/settings.py\nfrom snyk_metrics import initialise, Counter\n\ncounter_1 = Counter(\n    name="my_app_counter",\n    documentation="Simple example counter",\n    label_names=None,\n)\ncounter_2 = Counter(\n    name="my_app_requests",\n    documentation="Requests per endpoint and method",\n    label_names=("endpoint", "method"),\n)\n\nmetrics = [counter_1, counter_2]\n\ninitialise(metrics=metrics, prometheus_enabled=True)\n```\n\n```python\n# my_app/api/endpoints.py\nfrom my_app.metrics import counter_1, counter_2\n\n\ndef my_function():\n    counter_1.increment()\n\n\ndef foo_get_endpoint():\n    counter_2.increment()\n```\n\n### Example 2 - "Unstructured flexibility"\n\nIn this example metrics are created and used within the same file. It could make\nit harder to keep track of all the metrics in the application, but it can also\nhelp in keeping them closer to the part of the project where the metrics are\nused.\n\n```python\n# my_app/settings.py\nfrom snyk_metrics import initialise\n\ninitialise(prometheus_enabled=True, lock_registry=False)\n```\n\n```python\n# my_app/api/endpoints.py\nfrom snyk_metrics import Counter\n\ncounter_1 = Counter(\n    name="my_app_counter",\n    documentation="Simple example counter",\n    label_names=None,\n)\ncounter_2 = Counter(\n    name="my_app_requests",\n    documentation="Requests per endpoint and method",\n    label_names=("endpoint", "method"),\n)\n\n\ndef my_function():\n    counter_1.increment()\n\n\ndef foo_get_endpoint():\n    counter_2.increment()\n```\n',
     'author': 'Snyk Security R&D',
     'author_email': 'security-engineering@snyk.io',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/snyk/python-metrics',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `snyk-metrics-0.0.3/PKG-INFO` & `snyk_metrics-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: snyk-metrics
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library to interact transparently with Prometheus, Pushgateway and Dogstatsd.
 Home-page: https://github.com/snyk/python-metrics
 License: Apache-2.0
 Keywords: prometheus,datadog,metrics
 Author: Snyk Security R&D
 Author-email: security-engineering@snyk.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: datadog (>=0.43.0,<0.44.0)
 Requires-Dist: prometheus-client (>=0.12.0,<0.13.0)
 Project-URL: Repository, https://github.com/snyk/python-metrics
 Description-Content-Type: text/markdown
 
 # snyk-python-metrics
```

