# Comparing `tmp/chaostoolkit-opentracing-0.9.0.tar.gz` & `tmp/chaostoolkit-opentracing-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chaostoolkit-opentracing-0.9.0.tar", last modified: Tue Feb 21 21:15:20 2023, max compression
+gzip compressed data, was "dist/chaostoolkit-opentracing-0.9.1.tar", last modified: Wed Feb 22 07:18:36 2023, max compression
```

## Comparing `chaostoolkit-opentracing-0.9.0.tar` & `chaostoolkit-opentracing-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:15:20.000000 chaostoolkit-opentracing-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-02-21 21:15:07.000000 chaostoolkit-opentracing-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-21 21:15:07.000000 chaostoolkit-opentracing-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-21 21:15:07.000000 chaostoolkit-opentracing-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-02-21 21:15:20.000000 chaostoolkit-opentracing-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-02-21 21:15:07.000000 chaostoolkit-opentracing-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:15:20.000000 chaostoolkit-opentracing-0.9.0/chaostoolkit_opentracing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-02-21 21:15:20.000000 chaostoolkit-opentracing-0.9.0/chaostoolkit_opentracing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-02-21 21:15:20.000000 chaostoolkit-opentracing-0.9.0/chaostoolkit_opentracing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 21:15:20.000000 chaostoolkit-opentracing-0.9.0/chaostoolkit_opentracing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-21 21:15:20.000000 chaostoolkit-opentracing-0.9.0/chaostoolkit_opentracing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-21 21:15:20.000000 chaostoolkit-opentracing-0.9.0/chaostoolkit_opentracing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:15:20.000000 chaostoolkit-opentracing-0.9.0/chaostracing/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-21 21:15:07.000000 chaostoolkit-opentracing-0.9.0/chaostracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-02-21 21:15:07.000000 chaostoolkit-opentracing-0.9.0/chaostracing/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-21 21:15:07.000000 chaostoolkit-opentracing-0.9.0/chaostracing/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-02-21 21:15:07.000000 chaostoolkit-opentracing-0.9.0/chaostracing/oltp.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-21 21:15:07.000000 chaostoolkit-opentracing-0.9.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-21 21:15:07.000000 chaostoolkit-opentracing-0.9.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-21 21:15:07.000000 chaostoolkit-opentracing-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-21 21:15:20.000000 chaostoolkit-opentracing-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-02-21 21:15:07.000000 chaostoolkit-opentracing-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:15:20.000000 chaostoolkit-opentracing-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-21 21:15:07.000000 chaostoolkit-opentracing-0.9.0/tests/test_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 07:18:36.000000 chaostoolkit-opentracing-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-02-22 07:18:25.000000 chaostoolkit-opentracing-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-22 07:18:25.000000 chaostoolkit-opentracing-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-22 07:18:25.000000 chaostoolkit-opentracing-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-02-22 07:18:36.000000 chaostoolkit-opentracing-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-02-22 07:18:25.000000 chaostoolkit-opentracing-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 07:18:36.000000 chaostoolkit-opentracing-0.9.1/chaostoolkit_opentracing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-02-22 07:18:36.000000 chaostoolkit-opentracing-0.9.1/chaostoolkit_opentracing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-02-22 07:18:36.000000 chaostoolkit-opentracing-0.9.1/chaostoolkit_opentracing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 07:18:36.000000 chaostoolkit-opentracing-0.9.1/chaostoolkit_opentracing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-22 07:18:36.000000 chaostoolkit-opentracing-0.9.1/chaostoolkit_opentracing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 07:18:36.000000 chaostoolkit-opentracing-0.9.1/chaostoolkit_opentracing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 07:18:36.000000 chaostoolkit-opentracing-0.9.1/chaostracing/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-22 07:18:25.000000 chaostoolkit-opentracing-0.9.1/chaostracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-02-22 07:18:25.000000 chaostoolkit-opentracing-0.9.1/chaostracing/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-22 07:18:25.000000 chaostoolkit-opentracing-0.9.1/chaostracing/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-02-22 07:18:25.000000 chaostoolkit-opentracing-0.9.1/chaostracing/oltp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-22 07:18:25.000000 chaostoolkit-opentracing-0.9.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-22 07:18:25.000000 chaostoolkit-opentracing-0.9.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-22 07:18:25.000000 chaostoolkit-opentracing-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-22 07:18:36.000000 chaostoolkit-opentracing-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-02-22 07:18:25.000000 chaostoolkit-opentracing-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 07:18:36.000000 chaostoolkit-opentracing-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-22 07:18:25.000000 chaostoolkit-opentracing-0.9.1/tests/test_control.py
```

### Comparing `chaostoolkit-opentracing-0.9.0/CHANGELOG.md` & `chaostoolkit-opentracing-0.9.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 # Changelog
 
 ## [Unreleased][]
 
-[Unreleased]: https://github.com/chaostoolkit-incubator/chaostoolkit-opentracing/compare/0.9.0...HEAD
+[Unreleased]: https://github.com/chaostoolkit-incubator/chaostoolkit-opentracing/compare/0.9.1...HEAD
+
+## [0.9.1][] - 2023-02-22
+
+[0.9.1]: https://github.com/chaostoolkit-incubator/chaostoolkit-opentracing/compare/0.9.0...0.9.1
+
+### Fixed
+
+- Missing variable declaration for GCP
+
+### Added
+
+- The `CHAOSTOOLKIT_OTEL_GCP_SA` and `CHAOSTOOLKIT_OTEL_GCP_PROJECT_ID`
+  environment variables to pass the information of the target project
 
 ## [0.9.0][] - 2023-02-21
 
 [0.9.0]: https://github.com/chaostoolkit-incubator/chaostoolkit-opentracing/compare/0.8.2...0.9.0
 
 ### Added
```

### Comparing `chaostoolkit-opentracing-0.9.0/LICENSE` & `chaostoolkit-opentracing-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-opentracing-0.9.0/PKG-INFO` & `chaostoolkit-opentracing-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-opentracing
-Version: 0.9.0
+Version: 0.9.1
 Summary: Chaos Toolkit OpenTracing Extension
 Home-page: http://chaostoolkit.org
 Author: chaostoolkit Team
 Author-email: contact@chaostoolkit.org
 License: Apache License Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: Freely Distributable
@@ -116,31 +116,34 @@
       }
     ]
 }
 ```
 
 This will enable the according instrumentation automatically.
 
+#### Google Cloud Platform Traces
+
 If you intend on using Google Cloud Platform to export your traces to, please
 consider also installing the followings:
 
 ```
 $ pip install opentelemetry-exporter-gcp-trace \
     opentelemetry-resourcedetector-gcp \
     opentelemetry-propagator-gcp
 ```
 
 To authenticate the client, you can either:
 
-* set `GOOGLE_APPLICATION_CREDENTIALS` 
+* set `GOOGLE_APPLICATION_CREDENTIALS` environment variable
 * pass the `otel_gcp_service_account` and `otel_gcp_project_id` variables
   in the configuration block
+* set the `CHAOSTOOLKIT_OTEL_GCP_SA` and `CHAOSTOOLKIT_OTEL_GCP_PROJECT_ID` environment variables
 
-In both cases, point to a service account which has
-the `roles/cloudtrace.agent` role.
+In all cases, point to a service account which has
+the `roles/cloudtrace.agent` role as nthe name of the target project.
 
 ### Legacy Open Tracing
 
 This extensions supports the [Open Tracing](https://opentracing.io/) export
 format but highly recommends you to switch to Open Telemetry instead. There will
 be no support for Open Tracing support.
```

### Comparing `chaostoolkit-opentracing-0.9.0/README.md` & `chaostoolkit-opentracing-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,31 +92,34 @@
       }
     ]
 }
 ```
 
 This will enable the according instrumentation automatically.
 
+#### Google Cloud Platform Traces
+
 If you intend on using Google Cloud Platform to export your traces to, please
 consider also installing the followings:
 
 ```
 $ pip install opentelemetry-exporter-gcp-trace \
     opentelemetry-resourcedetector-gcp \
     opentelemetry-propagator-gcp
 ```
 
 To authenticate the client, you can either:
 
-* set `GOOGLE_APPLICATION_CREDENTIALS` 
+* set `GOOGLE_APPLICATION_CREDENTIALS` environment variable
 * pass the `otel_gcp_service_account` and `otel_gcp_project_id` variables
   in the configuration block
+* set the `CHAOSTOOLKIT_OTEL_GCP_SA` and `CHAOSTOOLKIT_OTEL_GCP_PROJECT_ID` environment variables
 
-In both cases, point to a service account which has
-the `roles/cloudtrace.agent` role.
+In all cases, point to a service account which has
+the `roles/cloudtrace.agent` role as nthe name of the target project.
 
 ### Legacy Open Tracing
 
 This extensions supports the [Open Tracing](https://opentracing.io/) export
 format but highly recommends you to switch to Open Telemetry instead. There will
 be no support for Open Tracing support.
```

### Comparing `chaostoolkit-opentracing-0.9.0/chaostoolkit_opentracing.egg-info/PKG-INFO` & `chaostoolkit-opentracing-0.9.1/chaostoolkit_opentracing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-opentracing
-Version: 0.9.0
+Version: 0.9.1
 Summary: Chaos Toolkit OpenTracing Extension
 Home-page: http://chaostoolkit.org
 Author: chaostoolkit Team
 Author-email: contact@chaostoolkit.org
 License: Apache License Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: Freely Distributable
@@ -116,31 +116,34 @@
       }
     ]
 }
 ```
 
 This will enable the according instrumentation automatically.
 
+#### Google Cloud Platform Traces
+
 If you intend on using Google Cloud Platform to export your traces to, please
 consider also installing the followings:
 
 ```
 $ pip install opentelemetry-exporter-gcp-trace \
     opentelemetry-resourcedetector-gcp \
     opentelemetry-propagator-gcp
 ```
 
 To authenticate the client, you can either:
 
-* set `GOOGLE_APPLICATION_CREDENTIALS` 
+* set `GOOGLE_APPLICATION_CREDENTIALS` environment variable
 * pass the `otel_gcp_service_account` and `otel_gcp_project_id` variables
   in the configuration block
+* set the `CHAOSTOOLKIT_OTEL_GCP_SA` and `CHAOSTOOLKIT_OTEL_GCP_PROJECT_ID` environment variables
 
-In both cases, point to a service account which has
-the `roles/cloudtrace.agent` role.
+In all cases, point to a service account which has
+the `roles/cloudtrace.agent` role as nthe name of the target project.
 
 ### Legacy Open Tracing
 
 This extensions supports the [Open Tracing](https://opentracing.io/) export
 format but highly recommends you to switch to Open Telemetry instead. There will
 be no support for Open Tracing support.
```

### Comparing `chaostoolkit-opentracing-0.9.0/chaostoolkit_opentracing.egg-info/requires.txt` & `chaostoolkit-opentracing-0.9.1/chaostoolkit_opentracing.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `chaostoolkit-opentracing-0.9.0/chaostracing/control.py` & `chaostoolkit-opentracing-0.9.1/chaostracing/control.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-opentracing-0.9.0/chaostracing/metrics.py` & `chaostoolkit-opentracing-0.9.1/chaostracing/metrics.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-opentracing-0.9.0/chaostracing/oltp.py` & `chaostoolkit-opentracing-0.9.1/chaostracing/oltp.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,28 +63,24 @@
     "before_activity_control",
     "after_activity_control",
 ]
 
 REGISTRY_HANDLER = None
 
 
-logger.info("KABOOOM")
-
-
 def configure_control(
     experiment: Experiment,
     event_registry: EventHandlerRegistry,
     trace_request: bool = False,
     trace_httpx: bool = False,
     trace_botocore: bool = False,
     configuration: Configuration = None,
     secrets: Secrets = None,
     **kwargs: Any,
 ) -> None:
-    logger.info("BOOOM")
     configure_traces(configuration)
     configure_instrumentations(trace_request, trace_httpx, trace_botocore)
 
     global REGISTRY_HANDLER
     REGISTRY_HANDLER = OLTPRunEventHandler()
     event_registry.register(REGISTRY_HANDLER)
 
@@ -355,17 +351,23 @@
     elif vendor == "gcp":
         if not HAS_GCP_EXPORTER:
             raise RuntimeError(
                 "missing Google Cloud Platform Open Telemetry dependencies. "
                 "See: https://google-cloud-opentelemetry.readthedocs.io/"
             )
 
+        tsc = None
+
         configuration = configuration or {}
-        service_account = configuration.get("otel_gcp_service_account")
-        project_id = configuration.get("otel_gcp_project_id")
+        service_account = configuration.get(
+            "otel_gcp_service_account", os.getenv("CHAOSTOOLKIT_OTEL_GCP_SA")
+        )
+        project_id = configuration.get(
+            "otel_gcp_project_id", os.getenv("CHAOSTOOLKIT_OTEL_GCP_PROJECT_ID")
+        )
         if service_account and os.path.isfile(service_account):
             credentials = Credentials.from_service_account_file(service_account)
             project_id = credentials.project_id
             tsc = TraceServiceClient(
                 credentials=credentials,
                 transport=TraceServiceGrpcTransport(
                     channel=TraceServiceGrpcTransport.create_channel(
```

### Comparing `chaostoolkit-opentracing-0.9.0/requirements.txt` & `chaostoolkit-opentracing-0.9.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `chaostoolkit-opentracing-0.9.0/setup.py` & `chaostoolkit-opentracing-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-opentracing-0.9.0/tests/test_control.py` & `chaostoolkit-opentracing-0.9.1/tests/test_control.py`

 * *Files identical despite different names*

