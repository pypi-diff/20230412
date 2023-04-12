# Comparing `tmp/honeycomb_opentelemetry-0.1.2b0.tar.gz` & `tmp/honeycomb_opentelemetry-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honeycomb_opentelemetry-0.1.2b0.tar", max compression
+gzip compressed data, was "honeycomb_opentelemetry-0.2.0b0.tar", max compression
```

## Comparing `honeycomb_opentelemetry-0.1.2b0.tar` & `honeycomb_opentelemetry-0.2.0b0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-03-30 10:42:05.410160 honeycomb_opentelemetry-0.1.2b0/LICENSE
--rw-r--r--   0        0        0     1390 2023-03-30 10:42:05.410160 honeycomb_opentelemetry-0.1.2b0/README.md
--rw-r--r--   0        0        0      840 2023-03-30 10:42:05.414160 honeycomb_opentelemetry-0.1.2b0/pyproject.toml
--rw-r--r--   0        0        0      128 2023-03-30 10:42:05.414160 honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/__init__.py
--rw-r--r--   0        0        0     1416 2023-03-30 10:42:05.414160 honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/baggage.py
--rw-r--r--   0        0        0     2665 2023-03-30 10:42:05.414160 honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/distro.py
--rw-r--r--   0        0        0     3161 2023-03-30 10:42:05.414160 honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/local_exporter.py
--rw-r--r--   0        0        0     1664 2023-03-30 10:42:05.414160 honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/metrics.py
--rw-r--r--   0        0        0    15162 2023-03-30 10:42:05.414160 honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/options.py
--rw-r--r--   0        0        0      842 2023-03-30 10:42:05.414160 honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/resource.py
--rw-r--r--   0        0        0     3127 2023-03-30 10:42:05.414160 honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/sampler.py
--rw-r--r--   0        0        0     2223 2023-03-30 10:42:05.414160 honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/trace.py
--rw-r--r--   0        0        0      101 2023-03-30 10:42:05.414160 honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/version.py
--rw-r--r--   0        0        0     2472 1970-01-01 00:00:00.000000 honeycomb_opentelemetry-0.1.2b0/setup.py
--rw-r--r--   0        0        0     2110 1970-01-01 00:00:00.000000 honeycomb_opentelemetry-0.1.2b0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-12 10:22:34.666372 honeycomb_opentelemetry-0.2.0b0/LICENSE
+-rw-r--r--   0        0        0     1612 2023-04-12 10:22:34.666372 honeycomb_opentelemetry-0.2.0b0/README.md
+-rw-r--r--   0        0        0      836 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/__init__.py
+-rw-r--r--   0        0        0     1416 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/baggage.py
+-rw-r--r--   0        0        0     2665 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/distro.py
+-rw-r--r--   0        0        0     3161 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/local_exporter.py
+-rw-r--r--   0        0        0     1664 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/metrics.py
+-rw-r--r--   0        0        0    15162 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/options.py
+-rw-r--r--   0        0        0      842 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/resource.py
+-rw-r--r--   0        0        0     3127 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/sampler.py
+-rw-r--r--   0        0        0     2223 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/trace.py
+-rw-r--r--   0        0        0      101 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/version.py
+-rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 honeycomb_opentelemetry-0.2.0b0/PKG-INFO
```

### Comparing `honeycomb_opentelemetry-0.1.2b0/LICENSE` & `honeycomb_opentelemetry-0.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.1.2b0/README.md` & `honeycomb_opentelemetry-0.2.0b0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Honeycomb OpenTelemetry Distro for Python
 
 [![OSS Lifecycle](https://img.shields.io/osslifecycle/honeycombio/honeycomb-opentelemetry-python)](https://github.com/honeycombio/home/blob/main/honeycomb-oss-lifecycle-and-practices.md)
 [![CircleCI](https://circleci.com/gh/honeycombio/honeycomb-opentelemetry-python.svg?style=shield)](https://circleci.com/gh/honeycombio/honeycomb-opentelemetry-python)
+[![PyPi](https://img.shields.io/pypi/v/honeycomb-opentelemetry)](https://pypi.org/project/honeycomb-opentelemetry/)
+
+**STATUS: this library is BETA.**
+You're welcome to try it, and let us know your feedback in the issues!
 
 This is Honeycomb's Distribution of OpenTelemetry for Python.
 It makes getting started with OpenTelemetry and Honeycomb easier!
 
 Latest release built with:
 
-- [OpenTelemetry version 1.16.0/0.37b0](https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.16.0)
+- [OpenTelemetry version 1.17.0/0.38b0](https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.17.0)
 
 ## Requirements
 
 - Python 3.7 or higher
 
 ## Getting Started
```

### Comparing `honeycomb_opentelemetry-0.1.2b0/pyproject.toml` & `honeycomb_opentelemetry-0.2.0b0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "honeycomb-opentelemetry"
-version = "0.1.2b0"
+version = "0.2.0b0"
 description = "Honeycomb OpenTelemetry Distro for Python"
 authors = ["Honeycomb <support@honeycomb.io>"]
 readme = "README.md"
 packages = [{include = "honeycomb", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.7, >= 3.7.2"
-opentelemetry-api = "^1.16.0"
-opentelemetry-sdk = "^1.16.0"
-opentelemetry-exporter-otlp = "^1.16.0"
-opentelemetry-instrumentation = "^0.37b0"
+opentelemetry-api = "1.17.0"
+opentelemetry-sdk = "1.17.0"
+opentelemetry-exporter-otlp = "1.17.0"
+opentelemetry-instrumentation = "0.38b0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = ">=6.5,<8.0"
 pytest = "^7.2.0"
 pylint = "^2.16.0"
 pycodestyle = "^2.10.0"
 importlib-metadata = { version = ">=0.12", python = "<3.8" }
```

### Comparing `honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/baggage.py` & `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/baggage.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/distro.py` & `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/distro.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/local_exporter.py` & `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/local_exporter.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/metrics.py` & `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/metrics.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/options.py` & `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/options.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/resource.py` & `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/resource.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/sampler.py` & `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/sampler.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.1.2b0/src/honeycomb/opentelemetry/trace.py` & `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/trace.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.1.2b0/PKG-INFO` & `honeycomb_opentelemetry-0.2.0b0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: honeycomb-opentelemetry
-Version: 0.1.2b0
+Version: 0.2.0b0
 Summary: Honeycomb OpenTelemetry Distro for Python
 Author: Honeycomb
 Author-email: support@honeycomb.io
 Requires-Python: >=3.7.2,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: opentelemetry-api (>=1.16.0,<2.0.0)
-Requires-Dist: opentelemetry-exporter-otlp (>=1.16.0,<2.0.0)
-Requires-Dist: opentelemetry-instrumentation (>=0.37b0,<0.38)
-Requires-Dist: opentelemetry-sdk (>=1.16.0,<2.0.0)
+Requires-Dist: opentelemetry-api (==1.17.0)
+Requires-Dist: opentelemetry-exporter-otlp (==1.17.0)
+Requires-Dist: opentelemetry-instrumentation (==0.38b0)
+Requires-Dist: opentelemetry-sdk (==1.17.0)
 Description-Content-Type: text/markdown
 
 # Honeycomb OpenTelemetry Distro for Python
 
 [![OSS Lifecycle](https://img.shields.io/osslifecycle/honeycombio/honeycomb-opentelemetry-python)](https://github.com/honeycombio/home/blob/main/honeycomb-oss-lifecycle-and-practices.md)
 [![CircleCI](https://circleci.com/gh/honeycombio/honeycomb-opentelemetry-python.svg?style=shield)](https://circleci.com/gh/honeycombio/honeycomb-opentelemetry-python)
+[![PyPi](https://img.shields.io/pypi/v/honeycomb-opentelemetry)](https://pypi.org/project/honeycomb-opentelemetry/)
+
+**STATUS: this library is BETA.**
+You're welcome to try it, and let us know your feedback in the issues!
 
 This is Honeycomb's Distribution of OpenTelemetry for Python.
 It makes getting started with OpenTelemetry and Honeycomb easier!
 
 Latest release built with:
 
-- [OpenTelemetry version 1.16.0/0.37b0](https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.16.0)
+- [OpenTelemetry version 1.17.0/0.38b0](https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.17.0)
 
 ## Requirements
 
 - Python 3.7 or higher
 
 ## Getting Started
```

