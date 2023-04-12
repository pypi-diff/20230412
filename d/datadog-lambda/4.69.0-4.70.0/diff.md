# Comparing `tmp/datadog_lambda-4.69.0.tar.gz` & `tmp/datadog_lambda-4.70.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog_lambda-4.69.0.tar", max compression
+gzip compressed data, was "datadog_lambda-4.70.0.tar", max compression
```

## Comparing `datadog_lambda-4.69.0.tar` & `datadog_lambda-4.70.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11379 2022-09-22 18:30:00.504292 datadog_lambda-4.69.0/LICENSE
--rw-r--r--   0        0        0      394 2022-09-22 18:30:00.504380 datadog_lambda-4.69.0/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0     3416 2022-09-22 18:30:00.504557 datadog_lambda-4.69.0/README.md
--rw-r--r--   0        0        0      538 2023-02-13 20:46:09.160997 datadog_lambda-4.69.0/datadog_lambda/__init__.py
--rw-r--r--   0        0        0     3653 2022-09-22 18:30:00.504778 datadog_lambda-4.69.0/datadog_lambda/api.py
--rw-r--r--   0        0        0     7062 2023-02-13 20:46:09.161235 datadog_lambda-4.69.0/datadog_lambda/cold_start.py
--rw-r--r--   0        0        0     1669 2023-01-25 19:31:51.675529 datadog_lambda-4.69.0/datadog_lambda/constants.py
--rw-r--r--   0        0        0     4769 2022-09-22 18:30:00.505031 datadog_lambda-4.69.0/datadog_lambda/dogstatsd.py
--rw-r--r--   0        0        0     1199 2022-09-22 18:30:00.505121 datadog_lambda-4.69.0/datadog_lambda/extension.py
--rw-r--r--   0        0        0      994 2022-09-22 18:30:00.505207 datadog_lambda-4.69.0/datadog_lambda/handler.py
--rw-r--r--   0        0        0     4707 2022-09-22 18:30:00.505343 datadog_lambda-4.69.0/datadog_lambda/metric.py
--rw-r--r--   0        0        0      139 2022-09-22 18:30:00.505417 datadog_lambda-4.69.0/datadog_lambda/module_name.py
--rw-r--r--   0        0        0     4641 2022-09-22 18:30:00.505516 datadog_lambda-4.69.0/datadog_lambda/patch.py
--rw-r--r--   0        0        0      243 2022-09-22 18:30:00.505686 datadog_lambda-4.69.0/datadog_lambda/stats_writer.py
--rw-r--r--   0        0        0      403 2022-09-22 18:30:00.505792 datadog_lambda-4.69.0/datadog_lambda/statsd_writer.py
--rw-r--r--   0        0        0     1751 2022-09-22 18:30:00.505884 datadog_lambda-4.69.0/datadog_lambda/tag_object.py
--rw-r--r--   0        0        0     3240 2022-09-22 18:30:00.505984 datadog_lambda-4.69.0/datadog_lambda/tags.py
--rw-r--r--   0        0        0     2522 2022-09-22 18:30:00.506089 datadog_lambda-4.69.0/datadog_lambda/thread_stats_writer.py
--rw-r--r--   0        0        0    43679 2023-02-13 15:23:17.991523 datadog_lambda-4.69.0/datadog_lambda/tracing.py
--rw-r--r--   0        0        0    11912 2022-12-07 18:46:50.567807 datadog_lambda-4.69.0/datadog_lambda/trigger.py
--rw-r--r--   0        0        0    13237 2023-02-13 20:46:09.161471 datadog_lambda-4.69.0/datadog_lambda/wrapper.py
--rw-r--r--   0        0        0     3449 2023-03-22 12:07:02.672991 datadog_lambda-4.69.0/datadog_lambda/xray.py
--rw-r--r--   0        0        0     1205 2023-03-22 12:11:31.681692 datadog_lambda-4.69.0/pyproject.toml
--rw-r--r--   0        0        0     4549 1970-01-01 00:00:00.000000 datadog_lambda-4.69.0/setup.py
--rw-r--r--   0        0        0     4912 1970-01-01 00:00:00.000000 datadog_lambda-4.69.0/PKG-INFO
+-rw-r--r--   0        0        0    11379 2022-08-04 20:47:28.483033 datadog_lambda-4.70.0/LICENSE
+-rw-r--r--   0        0        0      394 2023-02-13 18:56:36.618770 datadog_lambda-4.70.0/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0     3416 2023-02-13 18:56:36.619028 datadog_lambda-4.70.0/README.md
+-rw-r--r--   0        0        0      538 2023-02-17 16:21:55.265937 datadog_lambda-4.70.0/datadog_lambda/__init__.py
+-rw-r--r--   0        0        0     3653 2023-02-13 18:56:36.619460 datadog_lambda-4.70.0/datadog_lambda/api.py
+-rw-r--r--   0        0        0     7232 2023-04-12 18:23:27.980925 datadog_lambda-4.70.0/datadog_lambda/cold_start.py
+-rw-r--r--   0        0        0     1669 2023-02-13 18:56:36.620125 datadog_lambda-4.70.0/datadog_lambda/constants.py
+-rw-r--r--   0        0        0     4769 2023-02-13 18:56:36.620241 datadog_lambda-4.70.0/datadog_lambda/dogstatsd.py
+-rw-r--r--   0        0        0     1199 2023-02-13 18:56:36.620396 datadog_lambda-4.70.0/datadog_lambda/extension.py
+-rw-r--r--   0        0        0      994 2022-08-04 20:47:28.483885 datadog_lambda-4.70.0/datadog_lambda/handler.py
+-rw-r--r--   0        0        0     4707 2023-03-15 15:25:33.105333 datadog_lambda-4.70.0/datadog_lambda/metric.py
+-rw-r--r--   0        0        0      139 2023-02-13 18:56:36.620660 datadog_lambda-4.70.0/datadog_lambda/module_name.py
+-rw-r--r--   0        0        0     4641 2023-02-13 18:56:36.620808 datadog_lambda-4.70.0/datadog_lambda/patch.py
+-rw-r--r--   0        0        0      243 2023-02-13 18:56:36.620890 datadog_lambda-4.70.0/datadog_lambda/stats_writer.py
+-rw-r--r--   0        0        0      403 2023-02-13 18:56:36.620968 datadog_lambda-4.70.0/datadog_lambda/statsd_writer.py
+-rw-r--r--   0        0        0     1751 2023-02-13 18:56:36.621061 datadog_lambda-4.70.0/datadog_lambda/tag_object.py
+-rw-r--r--   0        0        0     3240 2023-02-13 18:56:36.621201 datadog_lambda-4.70.0/datadog_lambda/tags.py
+-rw-r--r--   0        0        0     2522 2023-02-13 18:56:36.621290 datadog_lambda-4.70.0/datadog_lambda/thread_stats_writer.py
+-rw-r--r--   0        0        0    45292 2023-04-12 18:23:27.981500 datadog_lambda-4.70.0/datadog_lambda/tracing.py
+-rw-r--r--   0        0        0    12082 2023-04-12 18:23:27.981977 datadog_lambda-4.70.0/datadog_lambda/trigger.py
+-rw-r--r--   0        0        0    13237 2023-03-15 15:25:33.105870 datadog_lambda-4.70.0/datadog_lambda/wrapper.py
+-rw-r--r--   0        0        0     3449 2023-04-12 15:37:46.255654 datadog_lambda-4.70.0/datadog_lambda/xray.py
+-rw-r--r--   0        0        0     1205 2023-04-12 18:30:35.665688 datadog_lambda-4.70.0/pyproject.toml
+-rw-r--r--   0        0        0     4549 1970-01-01 00:00:00.000000 datadog_lambda-4.70.0/setup.py
+-rw-r--r--   0        0        0     4912 1970-01-01 00:00:00.000000 datadog_lambda-4.70.0/PKG-INFO
```

### Comparing `datadog_lambda-4.69.0/LICENSE` & `datadog_lambda-4.70.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/README.md` & `datadog_lambda-4.70.0/README.md`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/datadog_lambda/__init__.py` & `datadog_lambda-4.70.0/datadog_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/datadog_lambda/api.py` & `datadog_lambda-4.70.0/datadog_lambda/api.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/datadog_lambda/cold_start.py` & `datadog_lambda-4.70.0/datadog_lambda/cold_start.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,36 +130,41 @@
 
 
 class ColdStartTracer(object):
     def __init__(
         self,
         tracer,
         function_name,
-        cold_start_span_finish_time_ns,
+        current_span_start_time_ns,
         trace_ctx,
         min_duration_ms: int,
-        ignored_libs: List[str] = [],
+        ignored_libs: List[str] = None,
     ):
+        if ignored_libs is None:
+            ignored_libs = []
         self._tracer = tracer
         self.function_name = function_name
-        self.cold_start_span_finish_time_ns = cold_start_span_finish_time_ns
+        self.current_span_start_time_ns = current_span_start_time_ns
         self.min_duration_ms = min_duration_ms
         self.trace_ctx = trace_ctx
         self.ignored_libs = ignored_libs
         self.need_to_reactivate_context = True
 
     def trace(self, root_nodes: List[ImportNode] = root_nodes):
         if not root_nodes:
             return
         cold_start_span_start_time_ns = root_nodes[0].start_time_ns
+        cold_start_span_end_time_ns = min(
+            root_nodes[-1].end_time_ns, self.current_span_start_time_ns
+        )
         cold_start_span = self.create_cold_start_span(cold_start_span_start_time_ns)
         while root_nodes:
             root_node = root_nodes.pop()
             self.trace_tree(root_node, cold_start_span)
-        self.finish_span(cold_start_span, self.cold_start_span_finish_time_ns)
+        self.finish_span(cold_start_span, cold_start_span_end_time_ns)
 
     def trace_tree(self, import_node: ImportNode, parent_span):
         if (
             import_node.end_time_ns - import_node.start_time_ns
             < self.min_duration_ms * 1e6
             or import_node.module_name in self.ignored_libs
         ):
```

### Comparing `datadog_lambda-4.69.0/datadog_lambda/constants.py` & `datadog_lambda-4.70.0/datadog_lambda/constants.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/datadog_lambda/dogstatsd.py` & `datadog_lambda-4.70.0/datadog_lambda/dogstatsd.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/datadog_lambda/extension.py` & `datadog_lambda-4.70.0/datadog_lambda/extension.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/datadog_lambda/handler.py` & `datadog_lambda-4.70.0/datadog_lambda/handler.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/datadog_lambda/metric.py` & `datadog_lambda-4.70.0/datadog_lambda/metric.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/datadog_lambda/patch.py` & `datadog_lambda-4.70.0/datadog_lambda/patch.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/datadog_lambda/tag_object.py` & `datadog_lambda-4.70.0/datadog_lambda/tag_object.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/datadog_lambda/tags.py` & `datadog_lambda-4.70.0/datadog_lambda/tags.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/datadog_lambda/thread_stats_writer.py` & `datadog_lambda-4.70.0/datadog_lambda/thread_stats_writer.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/datadog_lambda/tracing.py` & `datadog_lambda-4.70.0/datadog_lambda/tracing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Unless explicitly stated otherwise all files in this repository are licensed
 # under the Apache License Version 2.0.
 # This product includes software developed at Datadog (https://www.datadoghq.com/).
 # Copyright 2019 Datadog, Inc.
-
+import hashlib
 import logging
 import os
 import json
 import base64
 from datetime import datetime, timezone
 from typing import Optional, Dict
 
@@ -324,14 +324,47 @@
         sampling_priority = dd_ctx.get(TraceHeader.SAMPLING_PRIORITY)
         return trace_id, parent_id, sampling_priority
     except Exception as e:
         logger.debug("The trace extractor returned with error %s", e)
         return extract_context_from_lambda_context(lambda_context)
 
 
+def _deterministic_md5_hash(s: str) -> str:
+    """MD5 here is to generate trace_id, not for any encryption."""
+    hex_number = hashlib.md5(s.encode("ascii")).hexdigest()
+    binary = bin(int(hex_number, 16))
+    binary_str = str(binary)
+    binary_str_remove_0b = binary_str[2:].rjust(128, "0")
+    most_significant_64_bits_without_leading_1 = "0" + binary_str_remove_0b[1:-64]
+    result = str(int(most_significant_64_bits_without_leading_1, 2))
+    if result == "0" * 64:
+        return "1"
+    return result
+
+
+def extract_context_from_step_functions(event, lambda_context):
+    """
+    Only extract datadog trace context when Step Functions Context Object is injected
+    into lambda's event dict.
+    """
+    try:
+        execution_id = event.get("Execution").get("Id")
+        state_name = event.get("State").get("Name")
+        state_entered_time = event.get("State").get("EnteredTime")
+        trace_id = _deterministic_md5_hash(execution_id)
+        parent_id = _deterministic_md5_hash(
+            execution_id + "#" + state_name + "#" + state_entered_time
+        )
+        sampling_priority = SamplingPriority.AUTO_KEEP
+        return trace_id, parent_id, sampling_priority
+    except Exception as e:
+        logger.debug("The Step Functions trace extractor returned with error %s", e)
+        return extract_context_from_lambda_context(lambda_context)
+
+
 def extract_context_custom_extractor(extractor, event, lambda_context):
     """
     Extract Datadog trace context using a custom trace extractor function
     """
     try:
         (
             trace_id,
@@ -348,15 +381,15 @@
 def is_authorizer_response(response) -> bool:
     try:
         return (
             response is not None
             and response["principalId"]
             and response["policyDocument"]
         )
-    except KeyError:
+    except (KeyError, AttributeError):
         pass
     except Exception as e:
         logger.debug("unknown error while checking is_authorizer_response %s", e)
     return False
 
 
 def get_injected_authorizer_data(event, is_http_api) -> dict:
@@ -436,14 +469,20 @@
         ) = extract_context_from_eventbridge_event(event, lambda_context)
     elif event_source.equals(EventTypes.KINESIS):
         (
             trace_id,
             parent_id,
             sampling_priority,
         ) = extract_context_from_kinesis_event(event, lambda_context)
+    elif event_source.equals(EventTypes.STEPFUNCTIONS):
+        (
+            trace_id,
+            parent_id,
+            sampling_priority,
+        ) = extract_context_from_step_functions(event, lambda_context)
     else:
         trace_id, parent_id, sampling_priority = extract_context_from_lambda_context(
             lambda_context
         )
 
     if trace_id and parent_id and sampling_priority:
         logger.debug("Extracted Datadog trace context from event or context")
```

### Comparing `datadog_lambda-4.69.0/datadog_lambda/trigger.py` & `datadog_lambda-4.70.0/datadog_lambda/trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,21 @@
     API_GATEWAY = "api-gateway"
     APPSYNC = "appsync"
     ALB = "application-load-balancer"
     CLOUDWATCH_LOGS = "cloudwatch-logs"
     CLOUDWATCH_EVENTS = "cloudwatch-events"
     CLOUDFRONT = "cloudfront"
     DYNAMODB = "dynamodb"
+    EVENTBRIDGE = "eventbridge"
     KINESIS = "kinesis"
     LAMBDA_FUNCTION_URL = "lambda-function-url"
     S3 = "s3"
     SNS = "sns"
     SQS = "sqs"
-    EVENTBRIDGE = "eventbridge"
+    STEPFUNCTIONS = "states"
 
 
 class EventSubtypes(_stringTypedEnum):
     """
     EventSubtypes is an enum of Lambda event subtypes.
     Currently, API Gateway events subtypes are supported,
     e.g. HTTP-API and Websocket events vs vanilla API-Gateway events.
@@ -141,14 +142,17 @@
     has_event_categories = (
         isinstance(event_detail, dict)
         and event_detail.get("EventCategories") is not None
     )
     if event.get("source") == "aws.events" or has_event_categories:
         event_source = _EventSource(EventTypes.CLOUDWATCH_EVENTS)
 
+    if "Execution" in event and "StateMachine" in event and "State" in event:
+        event_source = _EventSource(EventTypes.STEPFUNCTIONS)
+
     event_record = get_first_record(event)
     if event_record:
         aws_event_source = event_record.get(
             "eventSource", event_record.get("EventSource")
         )
 
         if aws_event_source == "aws:dynamodb":
```

### Comparing `datadog_lambda-4.69.0/datadog_lambda/wrapper.py` & `datadog_lambda-4.70.0/datadog_lambda/wrapper.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/datadog_lambda/xray.py` & `datadog_lambda-4.70.0/datadog_lambda/xray.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.69.0/pyproject.toml` & `datadog_lambda-4.70.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datadog_lambda"
-version = "4.69.0"
+version = "4.70.0"
 description = "The Datadog AWS Lambda Library"
 authors = ["Datadog, Inc. <dev@datadoghq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/DataDog/datadog-lambda-python"
 keywords = [
     "datadog",
```

### Comparing `datadog_lambda-4.69.0/setup.py` & `datadog_lambda-4.70.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
          'requests>=2.22.0,<3.0.0',
          'nose2>=0.9.1,<0.10.0',
          'flake8>=3.7.9,<4.0.0',
          'httpretty>=0.9.7,<0.10.0']}
 
 setup_kwargs = {
     'name': 'datadog-lambda',
-    'version': '4.69.0',
+    'version': '4.70.0',
     'description': 'The Datadog AWS Lambda Library',
     'long_description': "# datadog-lambda-python\n\n![build](https://github.com/DataDog/datadog-lambda-python/workflows/build/badge.svg)\n[![PyPI](https://img.shields.io/pypi/v/datadog-lambda)](https://pypi.org/project/datadog-lambda/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datadog-lambda)\n[![Slack](https://chat.datadoghq.com/badge.svg?bg=632CA6)](https://chat.datadoghq.com/)\n[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-lambda-python/blob/main/LICENSE)\n\nDatadog Lambda Library for Python (3.7, 3.8, and 3.9) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.\n\n## Installation\n\nFollow the [installation instructions](https://docs.datadoghq.com/serverless/installation/python/), and view your function's enhanced metrics, traces and logs in Datadog.\n\n## Configuration\n\nFollow the [configuration instructions](https://docs.datadoghq.com/serverless/configuration) to tag your telemetry, capture request/response payloads, filter or scrub sensitive information from logs or traces, and more.\n\n## Opening Issues\n\nIf you encounter a bug with this package, we want to hear about it. Before opening a new issue, search the existing issues to avoid duplicates.\n\nWhen opening an issue, include the Datadog Lambda Library version, Python version, and stack trace if available. In addition, include the steps to reproduce when appropriate.\n\nYou can also open an issue for a feature request.\n\n## Lambda Profiling Beta\n\nDatadog's [Continuous Profiler](https://www.datadoghq.com/product/code-profiling/) is now available in beta for Python in version 4.62.0 and layer version 62 and above. This optional feature is enabled by setting the `DD_PROFILING_ENABLED` environment variable to `true`. During the beta period, profiling is available at no additional cost.\n\nThe Continuous Profiler works by spawning a thread which periodically wakes up and takes a snapshot of the CPU and Heap of all running python code. This can include the profiler itself. If you want the Profiler to ignore itself, set `DD_PROFILING_IGNORE_PROFILER` to `true`.\n\n## Major Version Notes\n\n### 4.x / Layer version 61+\n\n- Python3.6 support has been [deprecated](https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html) by AWS, and support removed from this library.\n- `dd-trace` upgraded from 0.61 to 1.4, full release notes are available [here](https://ddtrace.readthedocs.io/en/stable/release_notes.html#v1-0-0)\n  - `get_correlation_ids()` has been changed to `get_log_correlation_context()`, which now returns a dictionary containing the active `span_id`, `trace_id`, as well as `service` and `env`.\n\n## Contributing\n\nIf you find an issue with this package and have a fix, please feel free to open a pull request following the [procedures](CONTRIBUTING.md).\n\n## Community\n\nFor product feedback and questions, join the `#serverless` channel in the [Datadog community on Slack](https://chat.datadoghq.com/).\n\n## License\n\nUnless explicitly stated otherwise all files in this repository are licensed under the Apache License Version 2.0.\n\nThis product includes software developed at Datadog (https://www.datadoghq.com/). Copyright 2019 Datadog, Inc.\n",
     'author': 'Datadog, Inc.',
     'author_email': 'dev@datadoghq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DataDog/datadog-lambda-python',
```

### Comparing `datadog_lambda-4.69.0/PKG-INFO` & `datadog_lambda-4.70.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-lambda
-Version: 4.69.0
+Version: 4.70.0
 Summary: The Datadog AWS Lambda Library
 Home-page: https://github.com/DataDog/datadog-lambda-python
 License: Apache-2.0
 Keywords: datadog,aws,lambda,layer
 Author: Datadog, Inc.
 Author-email: dev@datadoghq.com
 Requires-Python: >=3.7.0,<4
```

