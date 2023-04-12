# Comparing `tmp/insightconnect-plugin-runtime-4.9.0.tar.gz` & `tmp/insightconnect-plugin-runtime-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insightconnect-plugin-runtime-4.9.0.tar", last modified: Tue Jan 24 18:53:01 2023, max compression
+gzip compressed data, was "insightconnect-plugin-runtime-5.0.0.tar", last modified: Wed Apr 12 14:16:39 2023, max compression
```

## Comparing `insightconnect-plugin-runtime-4.9.0.tar` & `insightconnect-plugin-runtime-5.0.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.880626 insightconnect-plugin-runtime-4.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-01-24 18:53:01.880626 insightconnect-plugin-runtime-4.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-01-24 18:52:23.000000 insightconnect-plugin-runtime-4.9.0/insightconnect-plugin-swagger.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.868626 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/action.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.868626 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26428 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.868626 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/clients/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/clients/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.868626 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/data/input_message_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/data/output_message_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13942 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.868626 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-01-24 18:53:01.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-01-24 18:53:01.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 18:53:01.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-01-24 18:53:01.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-24 18:53:01.000000 insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 18:53:01.880626 insightconnect-plugin-runtime-4.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.868626 insightconnect-plugin-runtime-4.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.868626 insightconnect-plugin-runtime-4.9.0/tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.872626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.872626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.872626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.872626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/
--rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.872626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.872626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.872626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.872626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.876626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.876626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.876626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.876626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.876626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.876626 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/tests/test_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/tests/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 18:53:01.880626 insightconnect-plugin-runtime-4.9.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/test_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/test_aws_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/test_custom_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/test_server_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-24 18:51:31.000000 insightconnect-plugin-runtime-4.9.0/tests/unit/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.675042 insightconnect-plugin-runtime-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-04-12 14:16:39.675042 insightconnect-plugin-runtime-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-04-12 14:15:48.000000 insightconnect-plugin-runtime-5.0.0/insightconnect-plugin-swagger.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.663042 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/action.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.663042 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26671 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.663042 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/clients/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/clients/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/data/input_message_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/data/output_message_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13942 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.663042 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-04-12 14:16:39.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-12 14:16:39.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:16:39.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-12 14:16:39.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 14:16:39.000000 insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:16:39.675042 insightconnect-plugin-runtime-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.667042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.671042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.671042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.671042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.671042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.671042 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/test_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:39.675042 insightconnect-plugin-runtime-5.0.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_aws_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_custom_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_server_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-12 14:14:33.000000 insightconnect-plugin-runtime-5.0.0/tests/unit/test_variables.py
```

### Comparing `insightconnect-plugin-runtime-4.9.0/PKG-INFO` & `insightconnect-plugin-runtime-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect-plugin-runtime
-Version: 4.9.0
+Version: 5.0.0
 Summary: InsightConnect Plugin Runtime
 Home-page: https://github.com/rapid7/komand-plugin-sdk-python
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -150,14 +150,17 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
+* 4.10.1 - Remove raising of exception if request id is not available in header
+* 4.10.0 - Add structlog for structured logging
 * 4.9.0 - Add current SDK version plugin is using to /info endpoint
 * 4.8.0 - Add `OAuth20ClientCredentialMixin` class to clients
 * 4.7.6 - Add `PaginationHelper` to the AWS Client | Refactored the `ActionHelper` | Add `region` handler for AWSAction 
 * 4.7.5 - Add AWS client for assuming role 
 * 4.7.4 - Convert data field to string in exception handling 
 * 4.7.3 - Add `measurement_time` property to plugin metrics collection
 * 4.7.2 - Fix incorrect status codes when handling PluginExceptions
```

### Comparing `insightconnect-plugin-runtime-4.9.0/README.md` & `insightconnect-plugin-runtime-5.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,17 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
+* 4.10.1 - Remove raising of exception if request id is not available in header
+* 4.10.0 - Add structlog for structured logging
 * 4.9.0 - Add current SDK version plugin is using to /info endpoint
 * 4.8.0 - Add `OAuth20ClientCredentialMixin` class to clients
 * 4.7.6 - Add `PaginationHelper` to the AWS Client | Refactored the `ActionHelper` | Add `region` handler for AWSAction 
 * 4.7.5 - Add AWS client for assuming role 
 * 4.7.4 - Convert data field to string in exception handling 
 * 4.7.3 - Add `measurement_time` property to plugin metrics collection
 * 4.7.2 - Fix incorrect status codes when handling PluginExceptions
```

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect-plugin-swagger.json` & `insightconnect-plugin-runtime-5.0.0/insightconnect-plugin-swagger.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -450,112 +450,112 @@
     "definitions": {
         "PluginInfo": {
             "type": "object",
             "properties": {
                 "plugin_spec_version": {
                     "type": "string"
                 },
-                "enable_cache": {
-                    "type": "boolean"
-                },
-                "support": {
+                "description": {
                     "type": "string"
                 },
-                "title": {
+                "version": {
                     "type": "string"
                 },
-                "version": {
+                "vendor": {
                     "type": "string"
                 },
                 "name": {
                     "type": "string"
                 },
-                "vendor": {
+                "title": {
                     "type": "string"
                 },
-                "tags": {
-                    "type": "array",
-                    "items": {
-                        "type": "string"
-                    }
-                },
                 "number_of_workers": {
                     "type": "integer",
                     "format": "int32"
                 },
                 "threads": {
                     "type": "integer",
                     "format": "int32"
                 },
-                "sdk_version": {
+                "tags": {
+                    "type": "array",
+                    "items": {
+                        "type": "string"
+                    }
+                },
+                "enable_cache": {
+                    "type": "boolean"
+                },
+                "support": {
                     "type": "string"
                 },
-                "description": {
+                "sdk_version": {
                     "type": "string"
                 }
             }
         },
         "ActionTriggerOutputBody": {
             "type": "object",
             "properties": {
-                "output": {
-                    "type": "object"
-                },
-                "meta": {
-                    "type": "object"
+                "status": {
+                    "type": "string"
                 },
                 "log": {
                     "type": "string"
                 },
-                "status": {
-                    "type": "string"
+                "meta": {
+                    "type": "object"
+                },
+                "output": {
+                    "type": "object"
                 }
             },
             "required": [
                 "log",
                 "meta",
                 "output",
                 "status"
             ]
         },
         "ActionTriggerOutput": {
             "type": "object",
             "properties": {
+                "body": {
+                    "$ref": "#/definitions/ActionTriggerOutputBody"
+                },
                 "version": {
                     "type": "string"
                 },
                 "type": {
                     "type": "string",
                     "enum": [
                         "action_event",
                         "trigger_event"
                     ]
-                },
-                "body": {
-                    "$ref": "#/definitions/ActionTriggerOutputBody"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "TaskOutputBody": {
             "type": "object",
             "properties": {
-                "log": {
-                    "type": "string"
-                },
                 "status": {
                     "type": "string"
                 },
                 "output": {
                     "type": "object"
                 },
+                "log": {
+                    "type": "string"
+                },
                 "meta": {
                     "type": "object"
                 },
                 "state": {
                     "type": "object"
                 }
             },
@@ -566,183 +566,183 @@
                 "state",
                 "status"
             ]
         },
         "TaskOutput": {
             "type": "object",
             "properties": {
+                "body": {
+                    "$ref": "#/definitions/TaskOutputBody"
+                },
                 "version": {
                     "type": "string"
                 },
                 "type": {
                     "type": "string",
                     "enum": [
                         "task_event"
                     ]
-                },
-                "body": {
-                    "$ref": "#/definitions/TaskOutputBody"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "ActionTriggerInputBody": {
             "type": "object",
             "properties": {
-                "connection": {
-                    "type": "object"
-                },
                 "input": {
                     "type": "object"
                 },
                 "action": {
                     "type": "string"
+                },
+                "connection": {
+                    "type": "object"
                 }
             },
             "required": [
                 "action",
                 "connection",
                 "input"
             ]
         },
         "ActionTriggerInput": {
             "type": "object",
             "properties": {
+                "body": {
+                    "$ref": "#/definitions/ActionTriggerInputBody"
+                },
                 "version": {
                     "type": "string"
                 },
                 "type": {
                     "type": "string",
                     "enum": [
                         "action_event",
                         "trigger_event"
                     ]
-                },
-                "body": {
-                    "$ref": "#/definitions/ActionTriggerInputBody"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "TaskInputBody": {
             "type": "object",
             "properties": {
-                "connection": {
+                "state": {
                     "type": "object"
                 },
                 "input": {
                     "type": "object"
                 },
+                "connection": {
+                    "type": "object"
+                },
                 "task": {
                     "type": "string"
-                },
-                "state": {
-                    "type": "object"
                 }
             },
             "required": [
                 "connection",
                 "input",
                 "state",
                 "task"
             ]
         },
         "TaskInput": {
             "type": "object",
             "properties": {
+                "body": {
+                    "$ref": "#/definitions/TaskInputBody"
+                },
                 "version": {
                     "type": "string"
                 },
                 "type": {
                     "type": "string",
                     "enum": [
                         "task_event"
                     ]
-                },
-                "body": {
-                    "$ref": "#/definitions/TaskInputBody"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "ActionTriggerDetails": {
             "type": "object",
             "properties": {
-                "input": {
+                "output": {
                     "type": "object"
                 },
                 "title": {
                     "type": "string"
                 },
-                "output": {
+                "input": {
                     "type": "object"
                 },
                 "description": {
                     "type": "string"
                 }
             }
         },
         "ConnectionDetails": {
             "type": "object",
             "properties": {
-                "properties": {
-                    "type": "object"
-                },
-                "type": {
-                    "type": "string"
-                },
                 "title": {
                     "type": "string"
                 },
                 "required": {
                     "type": "array",
                     "items": {
                         "type": "string"
                     }
+                },
+                "type": {
+                    "type": "string"
+                },
+                "properties": {
+                    "type": "object"
                 }
             }
         },
         "ConnectionTestOutput": {
             "type": "object",
             "properties": {
                 "message": {
                     "type": "object"
                 }
             }
         },
         "TaskDetails": {
             "type": "object",
             "properties": {
-                "input": {
+                "output": {
                     "type": "object"
                 },
-                "title": {
-                    "type": "string"
-                },
-                "output": {
+                "schedule": {
                     "type": "object"
                 },
                 "description": {
                     "type": "string"
                 },
-                "state": {
+                "title": {
+                    "type": "string"
+                },
+                "input": {
                     "type": "object"
                 },
-                "schedule": {
+                "state": {
                     "type": "object"
                 }
             }
         }
     }
 }
```

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/__init__.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import insightconnect_plugin_runtime.task
 import insightconnect_plugin_runtime.variables
 import insightconnect_plugin_runtime.helper
 import insightconnect_plugin_runtime.dispatcher
 import insightconnect_plugin_runtime.exceptions
 import certifi
 import os
-import logging
 
 Plugin = insightconnect_plugin_runtime.plugin.Plugin
 Action = insightconnect_plugin_runtime.action.Action
 Trigger = insightconnect_plugin_runtime.trigger.Trigger
 Task = insightconnect_plugin_runtime.task.Task
 Connection = insightconnect_plugin_runtime.connection.Connection
 Input = insightconnect_plugin_runtime.variables.Input
@@ -52,11 +51,7 @@
     except Exception as ex:
         # old certifi value
         return old_certifi_value
 
 
 # and here's the monkey-patch itself.
 certifi.where = where
-
-root_logger = logging.getLogger()
-root_logger.setLevel("DEBUG")
-root_logger.addHandler(logging.StreamHandler())
```

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/api/endpoints.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/api/endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 import subprocess
 import yaml
 import os
 import pkg_resources
 import signal
 from flask import jsonify, request, abort, make_response, Blueprint
+import structlog
+
 from insightconnect_plugin_runtime.exceptions import (
     ClientException,
     ServerException,
     LoggedException,
     ConnectionTestException,
     PluginException,
 )
@@ -19,15 +21,15 @@
     ConnectionDetailsSchema,
 )
 
 
 class Endpoints:
     def __init__(self, logger, plugin, spec, debug, workers, threads, master_pid):
         self.plugin = plugin
-        self.logger = logger
+        self.logger = structlog.get_logger("plugin")
         self.spec = spec
         self.debug = debug
         self.workers = workers
         self.threads = threads
         self.master_pid = master_pid
 
     def create_endpoints(self):
@@ -486,59 +488,59 @@
 
         @v1.route("/workers/add", methods=["POST"])
         def add_worker():
             """
             Adds a worker (another process)
             :return: Json Response
             """
-            r = {}
+            response = {}
 
             # Linux signal examples here:
             # https://docs.gunicorn.org/en/stable/signals.html#master-process
             try:
                 self.logger.info("Adding a worker")
                 self.logger.info("Current process is: %s" % self.master_pid)
                 os.kill(self.master_pid, signal.SIGTTIN)
-            except Exception as e:
-                r.status_code = 500
-                r.error = e
-                return jsonify(r)
+            except Exception as error:
+                response.status_code = 500
+                response.error = error
+                return jsonify(response)
 
-            r["num_workers"] = Endpoints._number_of_workers()
-            return jsonify(r)
+            response["num_workers"] = Endpoints._number_of_workers()
+            return jsonify(response)
 
         @v1.route("/workers/remove", methods=["POST"])
         def remove_worker():
             """
             Shuts down a worker (another process)
             If there is only 1 worker, nothing happens
 
             :return: Json Response
             """
 
-            r = {}
+            response = {}
 
             # Linux signal examples here:
             # https://docs.gunicorn.org/en/stable/signals.html#master-process
             try:
                 self.logger.info("Removing a worker")
                 self.logger.info("Current process is: %s" % self.master_pid)
                 os.kill(self.master_pid, signal.SIGTTOU)
-            except Exception as e:
-                r = {}
-                r.status_code = 500
-                r.error = e
-                return jsonify(r)
+            except Exception as error:
+                response = {}
+                response.status_code = 500
+                response.error = error
+                return jsonify(response)
 
-            return jsonify(r)  # Flask or Gunicorn expect a return
+            return jsonify(response)  # Flask or Gunicorn expect a return
 
         @v1.route("/workers", methods=["GET"])
         def num_workers():
-            r = {"num_workers": Endpoints._number_of_workers()}
-            return jsonify(r)
+            response = {"num_workers": Endpoints._number_of_workers()}
+            return jsonify(response)
 
         @v1.route("/connection", methods=["GET"])
         def connection():
             """Plugin connection details endpoint
             ---
             get:
               summary: Get plugin connection details
@@ -581,24 +583,24 @@
 
             try:
                 output = self.plugin.handle_step(
                     input_message, is_debug=self.debug, is_test=True
                 )
                 if output.get("body", {}).get("output") is None:
                     status_code = 204
-            except LoggedException as e:
-                wrapped_exception = e.ex
+            except LoggedException as error:
+                wrapped_exception = error.ex
                 self.logger.exception(wrapped_exception)
 
-                output = e.output
+                output = error.output
                 status_code = Endpoints.handle_wrapped_exception(wrapped_exception)
             finally:
-                r = jsonify(output)
-                r.status_code = status_code
-                return r
+                response = jsonify(output)
+                response.status_code = status_code
+                return response
 
         blueprints = [legacy, v1]
         return blueprints
 
     def _create_action_definitions_payload(self):
         """
         Creates a payload containing definitions for all actions within a given plugin
@@ -634,28 +636,28 @@
         return num_workers - 1
 
     @staticmethod
     def action_trigger_task_exists(plugin_spec_json, p_type, p_name):
         actions_triggers_tasks = plugin_spec_json.get(p_type)
         if actions_triggers_tasks is None or actions_triggers_tasks.get(p_name) is None:
             msg = f"{p_type[:-1].capitalize()} {p_name} does not exist"
-            resp = make_response(jsonify({"error": msg}), 400)
-            abort(resp)
+            response = make_response(jsonify({"error": msg}), 400)
+            abort(response)
         return actions_triggers_tasks.get(p_name)
 
     @staticmethod
     def load_file_json_format(filename):
-        with open(filename, "r") as p_spec:
-            return yaml.safe_load(p_spec.read())
+        with open(filename, "r") as plugin_spec:
+            return yaml.safe_load(plugin_spec.read())
 
     @staticmethod
     def validate_action_trigger_task_empty_input(input_message):
         if not input_message:
-            resp = make_response(jsonify({"error": "Empty input provided"}), 400)
-            abort(resp)
+            response = make_response(jsonify({"error": "Empty input provided"}), 400)
+            abort(response)
 
     @staticmethod
     def validate_action_trigger_task_name(input_message, name, p_type):
         name_in_input_msg = input_message.get("body", {}).get(p_type, None)
         if name_in_input_msg != name:
             msg = f"{p_type.capitalize()} name ({name_in_input_msg}) in input body is not matching with name ({name}) in route"
             resp = make_response(jsonify({"error": msg}), 400)
@@ -667,49 +669,49 @@
         for field in fields:
             plugin_info.update({field: plugin_spec_json.get(field)})
         return plugin_info
 
     def get_plugin_sdk_version(self):
         try:
             version = pkg_resources.require("insightconnect-plugin-runtime")[0].version
-        except Exception as e:
+        except Exception:
             self.logger.warn("Unable to get SDK version")
             version = "0.0.0"
 
         return version
 
     def run_action_trigger_task(self, input_message, test=False):
         status_code = 200
         output = None
         try:
             output = self.plugin.handle_step(
                 input_message, is_debug=self.debug, is_test=test
             )
-        except LoggedException as e:
-            wrapped_exception = e.ex
+        except LoggedException as error:
+            wrapped_exception = error.ex
             self.logger.exception(wrapped_exception)
 
-            output = e.output
+            output = error.output
             if isinstance(wrapped_exception, ClientException):
                 status_code = 400
             elif (
                 isinstance(wrapped_exception, PluginException)
                 and wrapped_exception.preset is PluginException.Preset.BAD_REQUEST
             ):
                 status_code = 400
             elif isinstance(wrapped_exception, ServerException):
                 # I'm unsure about this
                 status_code = 500
             else:
                 status_code = 500
         finally:
             self.logger.debug("Request output: %s", output)
-            r = jsonify(output)
-            r.status_code = status_code
-            return r
+            response = jsonify(output)
+            response.status_code = status_code
+            return response
 
     @staticmethod
     def handle_wrapped_exception(wrapped_exception):
         if isinstance(wrapped_exception, (ConnectionTestException, ClientException)):
             return 400
         elif (
             isinstance(wrapped_exception, PluginException)
```

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/api/schemas.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/api/schemas.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/cli.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/cli.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/clients/aws_client.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/clients/aws_client.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/clients/oauth.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/clients/oauth.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/connection.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/connection.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/data/input_message_schema.json` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/data/input_message_schema.json`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/data/output_message_schema.json` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/data/output_message_schema.json`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/dispatcher.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/dispatcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,16 +47,16 @@
         self.custom_encoder = config.get("custom_encoder")
         self.custom_decoder = config.get("custom_decoder")
 
         logging.info("Using dispatcher config: %s", config)
 
     def write(self, msg):
         try:
-            r = requests.post(self.url, json=msg, verify=os.environ["SSL_CERT_FILE"])
-            logging.info("POST %s returned %s", self.url, r.content)
-        except Exception as ex:
+            response = requests.post(self.url, json=msg, verify=os.environ["SSL_CERT_FILE"])
+            logging.info("POST %s returned %s", self.url, response.content)
+        except Exception as exception:
             logging.error(
                 "ERROR: POST to %s failed. CA bundle path: %s Exception %s",
                 self.url,
                 os.environ["SSL_CERT_FILE"],
-                str(ex),
+                str(exception),
             )
```

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/exceptions.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/exceptions.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/helper.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/helper.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/metrics.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/metrics.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/plugin.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # -*- coding: utf-8 -*-
 import copy
 import inspect
 import io
 import json
 import logging
-import os
-import uuid
 
 import jsonschema
+import structlog
 
-from .connection import ConnectionCache
-from .dispatcher import Stdout, Http
-from .exceptions import (
+from insightconnect_plugin_runtime.connection import ConnectionCache
+from insightconnect_plugin_runtime.dispatcher import Stdout, Http
+from insightconnect_plugin_runtime.exceptions import (
     ClientException,
     ServerException,
     LoggedException,
     ConnectionTestException,
     PluginException,
 )
-from .metrics import MetricsBuilder
+from insightconnect_plugin_runtime.metrics import MetricsBuilder
+from insightconnect_plugin_runtime.util import is_running_in_cloud
 
 message_output_type = {
     "action_start": "action_event",
     "trigger_start": "trigger_event",
     "task_start": "task_event",
     "connection_test": "connection_test",
 }
 
 
 class Workflow(object):
     def __init__(
-            self,
-            shortOrgId=None,
-            orgProductToken=None,
-            uiHostUrl=None,
-            jobId=None,
-            stepId=None,
-            versionId=None,
-            nextStepId=None,
-            nextEdgeId=None,
-            triggerId=None,
-            jobExecutionContextId=None,
-            time=None,
-            connectionTestId=None,
-            connectionTestTimeout=None,
-            workflowId=None,
+        self,
+        shortOrgId=None,
+        orgProductToken=None,
+        uiHostUrl=None,
+        jobId=None,
+        stepId=None,
+        versionId=None,
+        nextStepId=None,
+        nextEdgeId=None,
+        triggerId=None,
+        jobExecutionContextId=None,
+        time=None,
+        connectionTestId=None,
+        connectionTestTimeout=None,
+        workflowId=None,
     ):
         """
         Worflow object for the Meta Class
         :param shortOrgId: Short version of the Organization ID
         :param orgProductToken: Organization Product Token
         :param uiHostUrl: Job URL for triggers
         :param jobId: Job UUID
@@ -104,15 +104,15 @@
             time=input_message.get("time", None),
             connectionTestId=input_message.get("connectionTestId", None),
             connectionTestTimeout=input_message.get("connectionTestTimeout", None),
         )
 
 
 class Meta(object):
-    """ Meta properties for a plugin """
+    """Meta properties for a plugin"""
 
     def __init__(self, name="", vendor="", description="", version="", workflow=None):
         self.name, self.vendor, self.description, self.version, self.workflow = (
             name,
             vendor,
             description,
             version,
@@ -131,22 +131,22 @@
             self.workflow = Workflow.from_insight_connect(input_message)
 
 
 class Plugin(object):
     """A Komand Plugin."""
 
     def __init__(
-            self,
-            name="",
-            vendor="",
-            description="",
-            version="",
-            connection=None,
-            custom_encoder=None,
-            custom_decoder=None,
+        self,
+        name="",
+        vendor="",
+        description="",
+        version="",
+        connection=None,
+        custom_encoder=None,
+        custom_decoder=None,
     ):
         self.name = name
         self.vendor = vendor
         self.description = description
         self.version = version
         self.connection = connection
 
@@ -159,61 +159,66 @@
         self.actions = {}
         self.tasks = {}
         self.debug = False
         self.custom_decoder = custom_decoder
         self.custom_encoder = custom_encoder
 
     def add_trigger(self, trigger):
-        """ add a new trigger """
+        """add a new trigger"""
         self.triggers[trigger.name] = trigger
 
     def add_action(self, action):
-        """ add a new action """
+        """add a new action"""
         self.actions[action.name] = action
 
     def add_task(self, task):
-        """ add a new task"""
+        """add a new task"""
         self.tasks[task.name] = task
 
     def envelope(
-            self,
-            message_type,
-            input_message,
-            log,
-            success,
-            output,
-            error_message,
-            state,
-            ex: None,
-            is_test: False
+        self,
+        message_type,
+        input_message,
+        log,
+        success,
+        output,
+        error_message,
+        state,
+        has_more_pages,
+        ex: None,
+        is_test: False,
     ):
         """
         Creates an output message of a step's execution.
 
         :param message_type: The message type
         :param input_message: The input message
         :param log: The log of the step, as a single string
         :param success: whether or not the step was successful
         :param output: The step data output
         :param error_message: An error message if an error was thrown
         :param state: The state of task_event. Only applicable to tasks.
+        :param has_more_pages: Whether or not a task_event has more pages to be consumed. Only applicable to tasks.
         :param ex: An error that was thrown
         :param is_test: whether or not the step is part of a Connection Test
         :return: An output message
         """
 
         output_message = {
             "log": log,
             "status": "ok" if success else "error",
             "meta": input_message["body"].get("meta", None),
         }
 
-        if state:
+        if state is not None:
             output_message["state"] = state
 
+        if has_more_pages is not None:
+            output_message["has_more_pages"] = has_more_pages
+
         if success:
             output_message["output"] = output
         else:
             output_message["error"] = error_message
 
             if ex:
                 if isinstance(ex, ConnectionTestException):
@@ -223,42 +228,44 @@
                         "data": ex.data,
                     }
 
                 if is_test and not isinstance(ex, ConnectionTestException):
                     output_message["exception"] = {
                         "cause": "Plugin connection test failed.",
                         "assistance": "See error log for more details.",
-                        "data": ex.__repr__()
+                        "data": ex.__repr__(),
                     }
 
                 # Build the metrics blob to attach to the output payload
                 # Only supported in cloud environments right now
-                if os.environ.get("PLUGIN_RUNTIME_ENVIRONMENT") == "cloud":
-                    metrics_builder = MetricsBuilder(plugin_name=self.name,
-                                                     plugin_version=self.version,
-                                                     plugin_vendor=self.vendor,
-                                                     input_message=input_message,
-                                                     exception_=ex,
-                                                     workflow_id=self.connection.meta.workflow.workflowId,
-                                                     org_id=self.connection.meta.workflow.shortOrgId)
+                if is_running_in_cloud():
+                    metrics_builder = MetricsBuilder(
+                        plugin_name=self.name,
+                        plugin_version=self.version,
+                        plugin_vendor=self.vendor,
+                        input_message=input_message,
+                        exception_=ex,
+                        workflow_id=self.connection.meta.workflow.workflowId,
+                        org_id=self.connection.meta.workflow.shortOrgId,
+                    )
                     output_message["metrics"] = metrics_builder.build()
 
         return {"body": output_message, "version": "v1", "type": message_type}
 
     def marshal(self, msg, fd):
-        """ Marshal a message to fd. """
+        """Marshal a message to fd."""
 
         if self.custom_encoder is None:
             json.dump(msg, fd)
         else:
             json.dump(msg, fd, cls=self.custom_encoder)
         fd.flush()
 
     def unmarshal(self, fd):
-        """ Unmarshal a message. """
+        """Unmarshal a message."""
 
         if self.custom_decoder is None:
             msg = json.load(fd)
         else:
             msg = json.load(fd, cls=self.custom_decoder)
         return msg
 
@@ -343,32 +350,42 @@
         :return:
         """
         input_message_meta = input_message["body"].get("meta", {})
 
         if input_message_meta is None:
             input_message_meta = {}
         self.connection.meta.set_workflow(input_message_meta)
-        request_id = uuid.uuid4()
+
+        # Add StreamHandler to record plugin action/trigger/task logs for output back to consumer
+        # log_stream will record logs via StreamHandler and be included in the plugin output
         log_stream = io.StringIO()
         stream_handler = logging.StreamHandler(log_stream)
-        logger = logging.getLogger("step_handler_{}".format(request_id))
-        logger.setLevel("DEBUG" if is_debug else "INFO")
-        logger.addHandler(stream_handler)
+        stream_handler.setLevel(logging.DEBUG if is_debug else logging.INFO)
+        logging.getLogger("plugin").addHandler(stream_handler)
+        logger = structlog.get_logger("plugin")
 
         success = True
         caught_exception = None
         output = None
         out_type = None
+
+        # Properties specific to tasks
         state = None
+        has_more_pages = None
 
         try:
             # Attempt to grab message type first
             message_type = input_message.get("type")
             out_type = message_output_type.get(message_type)
-            if message_type not in ["action_start", "trigger_start", "task_start", "connection_test"]:
+            if message_type not in [
+                "action_start",
+                "trigger_start",
+                "task_start",
+                "connection_test",
+            ]:
                 raise ClientException(
                     'Unsupported message type "{}"'.format(message_type)
                 )
 
             Plugin.validate_input_message(input_message)
 
             if message_type == "action_start":
@@ -400,16 +417,15 @@
                         "task",
                         logger,
                         log_stream,
                         is_test,
                         is_debug,
                     )
                 else:
-                    # state will be returned by task's run method along with output
-                    output, state = self.start_step(
+                    output, state, has_more_pages = self.start_step(
                         input_message["body"],
                         "task",
                         logger,
                         log_stream,
                         is_test,
                         is_debug,
                     )
@@ -418,39 +434,46 @@
                 output = self.start_step(
                     input_message["body"],
                     "connection_test",
                     logger,
                     log_stream,
                     is_test,
                     is_debug,
-                    is_connection_test=True
+                    is_connection_test=True,
                 )
         except (ClientException, ServerException, PluginException, Exception) as e:
             success = False
             caught_exception = e
             logger.exception(e)
         finally:
             output = self.envelope(
                 out_type,
                 input_message,
                 log_stream.getvalue(),
                 success,
                 output,
                 str(caught_exception),
                 state,
+                has_more_pages,
                 caught_exception,
-                is_test
+                is_test,
             )
-            print(f"Output is: {output}")
             if not success:
                 raise LoggedException(caught_exception, output)
             return output
 
     def start_step(
-            self, message_body, step_key, logger, log_stream, is_test=False, is_debug=False, is_connection_test=False
+        self,
+        message_body,
+        step_key,
+        logger,
+        log_stream,
+        is_test=False,
+        is_debug=False,
+        is_connection_test=False,
     ):
         """
         Starts an action.
         :param message_body: The action_start message.
         :param step_key: The type of step to execute
         :param logger the logger for logging
         :param log_stream the raw stream for the log
@@ -471,15 +494,15 @@
                 func = connection.test
             else:
                 raise NotImplementedError(
                     "The server successfully processed the request and is not "
                     "returning any content (no connection test function)"
                 )
             output = func()
-            
+
             return output
 
         else:
             action_name = message_body[step_key]
             dictionary = getattr(self, step_key + "s")
             if action_name not in dictionary:
                 raise ClientException('Unknown {} "{}"'.format(step_key, action_name))
@@ -504,68 +527,73 @@
                     if step.debug:
                         step.dispatcher = Stdout(message_body["dispatcher"])
                     else:
                         step.dispatcher = Http(message_body["dispatcher"])
 
             params = message_body["input"]
             state = {}
-    
+            has_more_pages = None
+
             if not is_test:
                 # Validate input message
                 try:
                     step.input.validate(params)
                     if step_key == "task":
                         state = message_body["state"]
                         step.state.validate(state)
-    
+
                     # Validate required inputs
                     # Step inputs will be checked against schema for required properties existence
                     # This is needed to prevent null/empty string values from being passed as output to input of steps
                     step.input.validate_required(params)
                 except jsonschema.exceptions.ValidationError as e:
-                    raise ClientException("{} input JSON was invalid".format(step_key), e)
+                    raise ClientException(
+                        "{} input JSON was invalid".format(step_key), e
+                    )
                 except Exception as e:
-                    raise Exception("Unable to validate {} input JSON".format(step_key), e)
+                    raise Exception(
+                        "Unable to validate {} input JSON".format(step_key), e
+                    )
 
             # Log step information for improved debugging with users
             step.logger.info(
                 "{vendor}/{plugin_name}:{plugin_version}. Step name: {step_name}".format(
                     vendor=step.connection.meta.vendor,
                     plugin_name=step.connection.meta.name,
                     plugin_version=step.connection.meta.version,
                     step_name=step.name,
                 )
             )
-        
+
             if is_test:
                 # Check if connection test func available. If so - use it (preferred). Else fallback to action/trigger test
                 if hasattr(step.connection, "test"):
                     func = step.connection.test
                 else:
                     func = step.test
             else:
                 func = step.run
-    
+
             # Backward compatibility with steps with missing argument params
             # The SDK has always defined the signature of the run/test methods to include the params dictionary.
             # However, the code generation generates the test method without the params argument.
             parameters = inspect.signature(func)
             if len(parameters.parameters) > 0:
                 if step_key == "task" and not is_test:
-                    output, state = func(params, state)
+                    output, state, has_more_pages = func(params, state)
                 else:
                     output = func(params)
             else:
                 if step_key == "task" and not is_test:
-                    output, state = func()
+                    output, state, has_more_pages = func()
                 else:
                     output = func()
-    
+
             # Don't validate output for any test functions - action/trigger tests shouldn't be validated due to them
             # not providing value and a connection test shouldn't be validated due to it being generic/universal
             if not is_test:
                 step.output.validate(output)
-    
+
             if step_key == "task" and not is_test:
-                return output, state
-        
+                return output, state, has_more_pages
+
             return output
```

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/schema.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/step.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/step.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/trigger.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/util.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 import copy
-import sys
 import logging
+import os
+import sys
 
 import python_jsonschema_objects as pjs
 
 
 def default_for_object(obj, defs):
     defaults = {}
 
@@ -102,7 +103,11 @@
 
     return o.as_dict()
 
 
 def trace():
     """Returns the trace from an exception"""
     return sys.exc_info()[2]
+
+
+def is_running_in_cloud():
+    return os.environ.get("PLUGIN_RUNTIME_ENVIRONMENT") == "cloud"
```

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime/variables.py` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime/variables.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime.egg-info/PKG-INFO` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect-plugin-runtime
-Version: 4.9.0
+Version: 5.0.0
 Summary: InsightConnect Plugin Runtime
 Home-page: https://github.com/rapid7/komand-plugin-sdk-python
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -150,14 +150,17 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
+* 4.10.1 - Remove raising of exception if request id is not available in header
+* 4.10.0 - Add structlog for structured logging
 * 4.9.0 - Add current SDK version plugin is using to /info endpoint
 * 4.8.0 - Add `OAuth20ClientCredentialMixin` class to clients
 * 4.7.6 - Add `PaginationHelper` to the AWS Client | Refactored the `ActionHelper` | Add `region` handler for AWSAction 
 * 4.7.5 - Add AWS client for assuming role 
 * 4.7.4 - Convert data field to string in exception handling 
 * 4.7.3 - Add `measurement_time` property to plugin metrics collection
 * 4.7.2 - Fix incorrect status codes when handling PluginExceptions
```

### Comparing `insightconnect-plugin-runtime-4.9.0/insightconnect_plugin_runtime.egg-info/SOURCES.txt` & `insightconnect-plugin-runtime-5.0.0/insightconnect_plugin_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/setup.py` & `insightconnect-plugin-runtime-5.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="insightconnect-plugin-runtime",
-    version="4.9.0",
+    version="5.0.0",
     description="InsightConnect Plugin Runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rapid7 Integrations Alliance",
     author_email="integrationalliance@rapid7.com",
     url="https://github.com/rapid7/komand-plugin-sdk-python",
     packages=find_packages(),
@@ -21,14 +21,17 @@
         "Flask==2.0.3",
         "gunicorn==20.0.4",
         "greenlet>=0.4.17, <=1.1.2",
         "gevent==20.9.0",
         "marshmallow==3.4.0",
         "apispec==3.2.0",
         "apispec-webframeworks==0.5.2",
+        "blinker==1.5",
+        "structlog==22.3.0",
+        "python-json-logger==2.0.7",
     ],
     tests_require=[
         "pytest",
         "docker",
         "dockerpty",
         "swagger-spec-validator",
     ],
```

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/__init__.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/__init__.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/tests/conftest.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/tests/test_cli.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/tests/test_hello_world.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/plugin/hello_world/tests/test_server.py` & `insightconnect-plugin-runtime-5.0.0/tests/plugin/hello_world/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/unit/test_action.py` & `insightconnect-plugin-runtime-5.0.0/tests/unit/test_action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/unit/test_aws_action.py` & `insightconnect-plugin-runtime-5.0.0/tests/unit/test_aws_action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/unit/test_custom_encoder.py` & `insightconnect-plugin-runtime-5.0.0/tests/unit/test_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/unit/test_endpoints.py` & `insightconnect-plugin-runtime-5.0.0/tests/unit/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/unit/test_exceptions.py` & `insightconnect-plugin-runtime-5.0.0/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/unit/test_helpers.py` & `insightconnect-plugin-runtime-5.0.0/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/unit/test_metrics.py` & `insightconnect-plugin-runtime-5.0.0/tests/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/unit/test_oauth.py` & `insightconnect-plugin-runtime-5.0.0/tests/unit/test_oauth.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/unit/test_plugin.py` & `insightconnect-plugin-runtime-5.0.0/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/unit/test_schema.py` & `insightconnect-plugin-runtime-5.0.0/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/unit/test_server_spec.py` & `insightconnect-plugin-runtime-5.0.0/tests/unit/test_server_spec.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-4.9.0/tests/unit/test_trigger.py` & `insightconnect-plugin-runtime-5.0.0/tests/unit/test_trigger.py`

 * *Files identical despite different names*

