# Comparing `tmp/metaflow-2.8.2.tar.gz` & `tmp/metaflow-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-2.8.2.tar", last modified: Wed Mar 29 19:01:28 2023, max compression
+gzip compressed data, was "metaflow-2.8.3.tar", last modified: Wed Apr 12 18:52:36 2023, max compression
```

## Comparing `metaflow-2.8.2.tar` & `metaflow-2.8.3.tar`

### file list

```diff
@@ -1,331 +1,331 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.154644 metaflow-2.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-03-29 19:01:15.000000 metaflow-2.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-29 19:01:15.000000 metaflow-2.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-03-29 19:01:28.154644 metaflow-2.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-03-29 19:01:15.000000 metaflow-2.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.126643 metaflow-2.8.2/metaflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/R.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.130643 metaflow-2.8.2/metaflow/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.130643 metaflow-2.8.2/metaflow/_vendor/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/_bashcomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/_termui_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/_textwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/_unicodefun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/_winconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.130643 metaflow-2.8.2/metaflow/_vendor/v3_5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.130643 metaflow-2.8.2/metaflow/_vendor/v3_5/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_5/zipp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.130643 metaflow-2.8.2/metaflow/_vendor/v3_6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.134643 metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_6/typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/_vendor/v3_6/zipp.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.134643 metaflow-2.8.2/metaflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63310 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/client/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/client/filecache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.134643 metaflow-2.8.2/metaflow/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31051 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/cmd/configure_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/cmd/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/cmd/tutorials_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/cmd/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/cmd_with_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.134643 metaflow-2.8.2/metaflow/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/datastore/content_addressed_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/datastore/datastore_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/datastore/datastore_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/datastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/datastore/flow_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/datastore/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/datastore/task_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/event_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.134643 metaflow-2.8.2/metaflow/extension_support/
--rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/extension_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/extension_support/_empty_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/extension_support/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/extension_support/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/extension_support/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/flowspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/includefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.134643 metaflow-2.8.2/metaflow/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/metadata/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/metadata/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17121 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/metaflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/metaflow_config_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/metaflow_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/metaflow_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/metaflow_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.134643 metaflow-2.8.2/metaflow/mflog/
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/mflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/mflog/mflog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/mflog/save_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/mflog/save_logs_periodically.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/mflog/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/multicore_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.138643 metaflow-2.8.2/metaflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.138643 metaflow-2.8.2/metaflow/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30230 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/airflow/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/airflow/airflow_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/airflow/airflow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/airflow/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/airflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/airflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.138643 metaflow-2.8.2/metaflow/plugins/airflow/plumbing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/airflow/plumbing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/airflow/plumbing/set_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.138643 metaflow-2.8.2/metaflow/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/airflow/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/airflow/sensors/base_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/airflow/sensors/external_task_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/airflow/sensors/s3_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.138643 metaflow-2.8.2/metaflow/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/argo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/argo/argo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57957 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/argo/argo_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    17737 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/argo/argo_workflows_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/argo/argo_workflows_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/argo/process_input_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.138643 metaflow-2.8.2/metaflow/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/aws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.142644 metaflow-2.8.2/metaflow/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/batch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/batch/batch_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    22700 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/batch/batch_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/batch/batch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.142644 metaflow-2.8.2/metaflow/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/secrets_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.142644 metaflow-2.8.2/metaflow/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/step_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/step_functions/dynamo_db_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/step_functions/event_bridge_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/step_functions/production_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/step_functions/schedule_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/step_functions/set_batch_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    41866 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/step_functions/step_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/step_functions/step_functions_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/step_functions/step_functions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/aws/step_functions/step_functions_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.142644 metaflow-2.8.2/metaflow/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/azure/azure_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/azure/azure_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/azure/azure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/azure/blob_service_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/azure/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.142644 metaflow-2.8.2/metaflow/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.146644 metaflow-2.8.2/metaflow/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.146644 metaflow-2.8.2/metaflow/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/chevron/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/chevron/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/chevron/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/chevron/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/convert_to_native_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/renderer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_modules/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/card_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/component_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/cards/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/catch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.146644 metaflow-2.8.2/metaflow/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/conda/batch_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/conda/conda_step_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.146644 metaflow-2.8.2/metaflow/plugins/datastores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/datastores/azure_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/datastores/gs_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/datastores/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/datastores/s3_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.146644 metaflow-2.8.2/metaflow/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/datatools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/datatools/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.150644 metaflow-2.8.2/metaflow/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/datatools/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62959 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/datatools/s3/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/datatools/s3/s3op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/datatools/s3/s3tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/datatools/s3/s3util.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/debug_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/debug_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.150644 metaflow-2.8.2/metaflow/plugins/env_escape/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/client_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.150644 metaflow-2.8.2/metaflow/plugins/env_escape/communication/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/communication/bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/communication/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/communication/socket_bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/communication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.150644 metaflow-2.8.2/metaflow/plugins/env_escape/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.150644 metaflow-2.8.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.150644 metaflow-2.8.2/metaflow/plugins/env_escape/configurations/test_lib_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/data_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/exception_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/override_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/env_escape/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/environment_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.150644 metaflow-2.8.2/metaflow/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/frameworks/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.150644 metaflow-2.8.2/metaflow/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/gcp/gs_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/gcp/gs_storage_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/gcp/gs_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/gcp/gs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/gcp/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.150644 metaflow-2.8.2/metaflow/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/kubernetes/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/kubernetes/kubernetes_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/kubernetes/kubernetes_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17152 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/kubernetes/kubernetes_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24217 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/kubernetes/kubernetes_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.154644 metaflow-2.8.2/metaflow/plugins/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/metadata/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    19987 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/metadata/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/package_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/parallel_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/project_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/resources_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/retry_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.154644 metaflow-2.8.2/metaflow/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/secrets/inline_secrets_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/secrets/secrets_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/storage_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/tag_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/test_unbounded_foreach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/plugins/timeout_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/procpoll.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/pylint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.154644 metaflow-2.8.2/metaflow/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/sidecar/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/sidecar/sidecar_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/sidecar/sidecar_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/sidecar/sidecar_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tagging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.122643 metaflow-2.8.2/metaflow/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.154644 metaflow-2.8.2/metaflow/tutorials/00-helloworld/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/00-helloworld/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/00-helloworld/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.154644 metaflow-2.8.2/metaflow/tutorials/01-playlist/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/01-playlist/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/01-playlist/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/01-playlist/playlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/01-playlist/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.154644 metaflow-2.8.2/metaflow/tutorials/02-statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/02-statistics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/02-statistics/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/02-statistics/stats.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/02-statistics/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.154644 metaflow-2.8.2/metaflow/tutorials/03-playlist-redux/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/03-playlist-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/03-playlist-redux/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.154644 metaflow-2.8.2/metaflow/tutorials/04-playlist-plus/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/04-playlist-plus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/04-playlist-plus/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.154644 metaflow-2.8.2/metaflow/tutorials/05-hello-cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/05-hello-cloud/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/05-hello-cloud/hello-cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.154644 metaflow-2.8.2/metaflow/tutorials/06-statistics-redux/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/06-statistics-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/06-statistics-redux/stats.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.154644 metaflow-2.8.2/metaflow/tutorials/07-worldview/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/07-worldview/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/07-worldview/worldview.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.154644 metaflow-2.8.2/metaflow/tutorials/08-autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/08-autopilot/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/tutorials/08-autopilot/autopilot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/unbounded_foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-03-29 19:01:15.000000 metaflow-2.8.2/metaflow/vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:01:28.130643 metaflow-2.8.2/metaflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-03-29 19:01:28.000000 metaflow-2.8.2/metaflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10861 2023-03-29 19:01:28.000000 metaflow-2.8.2/metaflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 19:01:28.000000 metaflow-2.8.2/metaflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-29 19:01:28.000000 metaflow-2.8.2/metaflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 19:01:28.000000 metaflow-2.8.2/metaflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-29 19:01:28.000000 metaflow-2.8.2/metaflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-29 19:01:28.158644 metaflow-2.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-29 19:01:15.000000 metaflow-2.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-12 18:52:25.000000 metaflow-2.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 18:52:25.000000 metaflow-2.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-12 18:52:36.890292 metaflow-2.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-12 18:52:25.000000 metaflow-2.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.866292 metaflow-2.8.3/metaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/R.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.866292 metaflow-2.8.3/metaflow/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/_vendor/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/_bashcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/_unicodefun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/_vendor/v3_5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/_vendor/v3_5/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_5/zipp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/_vendor/v3_6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/zipp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63753 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/client/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/client/filecache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31039 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cmd/configure_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cmd/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cmd/tutorials_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cmd/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cmd_with_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/content_addressed_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/datastore_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/datastore_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/flow_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/task_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/event_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/extension_support/
+-rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/extension_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/extension_support/_empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/extension_support/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/extension_support/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/extension_support/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/flowspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/includefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metadata/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metadata/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metaflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metaflow_config_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metaflow_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metaflow_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metaflow_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/mflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/mflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/mflog/mflog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/mflog/save_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/mflog/save_logs_periodically.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/mflog/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/multicore_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30229 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/airflow_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/airflow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/plugins/airflow/plumbing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/plumbing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/plumbing/set_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/sensors/base_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/sensors/external_task_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/sensors/s3_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/argo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/argo/argo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58089 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/argo/argo_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17737 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/argo/argo_workflows_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/argo/argo_workflows_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/argo/process_input_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/aws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16118 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/batch/batch_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23960 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/batch/batch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15590 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/batch/batch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/dynamo_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/event_bridge_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/production_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/schedule_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/set_batch_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42073 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/azure/azure_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/azure/azure_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/azure/azure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/azure/blob_service_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/azure/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/convert_to_native_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/renderer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/test_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/component_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/catch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/conda/batch_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/conda/conda_step_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/datastores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datastores/azure_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datastores/gs_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datastores/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datastores/s3_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62975 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/s3/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/s3/s3op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/s3/s3tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/s3/s3util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/debug_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/debug_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/env_escape/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/client_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/env_escape/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/communication/bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/communication/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/communication/socket_bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/communication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/test_lib_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/data_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/exception_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/override_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/environment_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/frameworks/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/gcp/gs_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/gcp/gs_storage_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/gcp/gs_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/gcp/gs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/gcp/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/metadata/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/metadata/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/package_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/parallel_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/project_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/resources_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/retry_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/secrets/inline_secrets_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/secrets/secrets_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/storage_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/tag_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/test_unbounded_foreach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/procpoll.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/pylint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/sidecar/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/sidecar/sidecar_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/sidecar/sidecar_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/sidecar/sidecar_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tagging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.862292 metaflow-2.8.3/metaflow/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/tutorials/00-helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/00-helloworld/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/00-helloworld/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/tutorials/01-playlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/01-playlist/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/01-playlist/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/01-playlist/playlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/01-playlist/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/02-statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/02-statistics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/02-statistics/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/02-statistics/stats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/02-statistics/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/03-playlist-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/03-playlist-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/03-playlist-redux/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/04-playlist-plus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/04-playlist-plus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/04-playlist-plus/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/hello-cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/06-statistics-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/06-statistics-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/06-statistics-redux/stats.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/07-worldview/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/07-worldview/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/07-worldview/worldview.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/08-autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/08-autopilot/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/08-autopilot/autopilot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/unbounded_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.866292 metaflow-2.8.3/metaflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-12 18:52:36.000000 metaflow-2.8.3/metaflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10861 2023-04-12 18:52:36.000000 metaflow-2.8.3/metaflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:52:36.000000 metaflow-2.8.3/metaflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 18:52:36.000000 metaflow-2.8.3/metaflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 18:52:36.000000 metaflow-2.8.3/metaflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 18:52:36.000000 metaflow-2.8.3/metaflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 18:52:36.890292 metaflow-2.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-12 18:52:25.000000 metaflow-2.8.3/setup.py
```

### Comparing `metaflow-2.8.2/LICENSE` & `metaflow-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/PKG-INFO` & `metaflow-2.8.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow
-Version: 2.8.2
+Version: 2.8.3
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
@@ -69,12 +69,7 @@
 * Open an issue at: https://github.com/Netflix/metaflow 
 * Email us at: help@metaflow.org
 * Chat with us on: http://chat.metaflow.org 
 
 ## Contributing
 
 We welcome contributions to Metaflow. Please see our [contribution guide](https://docs.metaflow.org/introduction/contributing-to-metaflow) for more details.
-
-### Code style
-
-We use [black](https://black.readthedocs.io/en/stable/) as a code formatter. The easiest way to ensure your commits are always formatted with the correct version of `black` it is to use [pre-commit](https://pre-commit.com/): install it and then run `pre-commit install` once in your local copy of the repo.
-
```

### Comparing `metaflow-2.8.2/README.md` & `metaflow-2.8.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -44,12 +44,7 @@
 * Open an issue at: https://github.com/Netflix/metaflow 
 * Email us at: help@metaflow.org
 * Chat with us on: http://chat.metaflow.org 
 
 ## Contributing
 
 We welcome contributions to Metaflow. Please see our [contribution guide](https://docs.metaflow.org/introduction/contributing-to-metaflow) for more details.
-
-### Code style
-
-We use [black](https://black.readthedocs.io/en/stable/) as a code formatter. The easiest way to ensure your commits are always formatted with the correct version of `black` it is to use [pre-commit](https://pre-commit.com/): install it and then run `pre-commit install` once in your local copy of the repo.
-
```

### Comparing `metaflow-2.8.2/metaflow/R.py` & `metaflow-2.8.3/metaflow/R.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/__init__.py` & `metaflow-2.8.3/metaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/__init__.py` & `metaflow-2.8.3/metaflow/_vendor/click/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/_bashcomplete.py` & `metaflow-2.8.3/metaflow/_vendor/click/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/_compat.py` & `metaflow-2.8.3/metaflow/_vendor/click/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/_termui_impl.py` & `metaflow-2.8.3/metaflow/_vendor/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/_textwrap.py` & `metaflow-2.8.3/metaflow/_vendor/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/_unicodefun.py` & `metaflow-2.8.3/metaflow/_vendor/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/_winconsole.py` & `metaflow-2.8.3/metaflow/_vendor/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/core.py` & `metaflow-2.8.3/metaflow/_vendor/click/core.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/decorators.py` & `metaflow-2.8.3/metaflow/_vendor/click/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/exceptions.py` & `metaflow-2.8.3/metaflow/_vendor/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/formatting.py` & `metaflow-2.8.3/metaflow/_vendor/click/formatting.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/globals.py` & `metaflow-2.8.3/metaflow/_vendor/click/globals.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/parser.py` & `metaflow-2.8.3/metaflow/_vendor/click/parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/termui.py` & `metaflow-2.8.3/metaflow/_vendor/click/termui.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/testing.py` & `metaflow-2.8.3/metaflow/_vendor/click/testing.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/types.py` & `metaflow-2.8.3/metaflow/_vendor/click/types.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/click/utils.py` & `metaflow-2.8.3/metaflow/_vendor/click/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/v3_5/importlib_metadata/__init__.py` & `metaflow-2.8.3/metaflow/_vendor/v3_5/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/v3_5/importlib_metadata/_compat.py` & `metaflow-2.8.3/metaflow/_vendor/v3_5/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/v3_5/zipp.py` & `metaflow-2.8.3/metaflow/_vendor/v3_5/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/__init__.py` & `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py` & `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_collections.py` & `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_compat.py` & `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_functools.py` & `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py` & `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_meta.py` & `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/v3_6/importlib_metadata/_text.py` & `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/v3_6/typing_extensions.py` & `metaflow-2.8.3/metaflow/_vendor/v3_6/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/_vendor/v3_6/zipp.py` & `metaflow-2.8.3/metaflow/_vendor/v3_6/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/cli.py` & `metaflow-2.8.3/metaflow/cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/cli_args.py` & `metaflow-2.8.3/metaflow/cli_args.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/client/core.py` & `metaflow-2.8.3/metaflow/client/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,14 +261,15 @@
         _parent: Optional["MetaflowObject"] = None,
         _namespace_check: bool = True,
     ):
         self._metaflow = Metaflow()
         self._parent = _parent
         self._path_components = None
         self._attempt = attempt
+        self._namespace_check = _namespace_check
 
         if self._attempt is not None:
             if self._NAME not in ["task", "artifact"]:
                 raise MetaflowNotFound(
                     "Attempts can only be specified for Task or DataArtifact"
                 )
             try:
@@ -311,38 +312,40 @@
 
         self._tags = frozenset(
             chain(self._object.get("system_tags") or [], self._object.get("tags") or [])
         )
         self._user_tags = frozenset(self._object.get("tags") or [])
         self._system_tags = frozenset(self._object.get("system_tags") or [])
 
-        if _namespace_check and not self.is_in_namespace():
+        if self._namespace_check and not self.is_in_namespace():
             raise MetaflowNamespaceMismatch(current_namespace)
 
     def _get_object(self, *path_components):
         result = self._metaflow.metadata.get_object(
             self._NAME, "self", None, self._attempt, *path_components
         )
         if not result:
             raise MetaflowNotFound("%s does not exist" % self)
         return result
 
     def __iter__(self) -> Iterable["MetaflowObject"]:
         """
         Iterate over all child objects of this object if any.
 
-        Note that only children present in the current namespace are returned.
+        Note that only children present in the current namespace are returned iff
+        _namespace_check is set.
 
         Returns
         -------
         Iterable[MetaflowObject]
             Iterator over all children
         """
         query_filter = {}
-        if current_namespace:
+        # skip namespace filtering if _namespace_check is False
+        if self._namespace_check and current_namespace:
             query_filter = {"any_tags": current_namespace}
 
         unfiltered_children = self._metaflow.metadata.get_object(
             self._NAME,
             _CLASSES[self._CHILD_CLASS]._NAME,
             query_filter,
             self._attempt,
@@ -377,14 +380,18 @@
         If tags are specified, only children associated with all specified tags
         are returned.
         """
         for child in self:
             if all(tag in child.tags for tag in tags):
                 yield child
 
+    def _ipython_key_completions_(self):
+        """Returns available options for ipython auto-complete."""
+        return [child.id for child in self._filtered_children()]
+
     @classmethod
     def _url_token(cls):
         return "%ss" % cls._NAME
 
     def is_in_namespace(self) -> bool:
         """
         Returns whether this object is in the current namespace.
@@ -440,15 +447,18 @@
         ------
         KeyError
             If the name does not identify a valid child object
         """
         obj = self._get_child(id)
         if obj:
             return _CLASSES[self._CHILD_CLASS](
-                attempt=self._attempt, _object=obj, _parent=self
+                attempt=self._attempt,
+                _object=obj,
+                _parent=self,
+                _namespace_check=self._namespace_check,
             )
         else:
             raise KeyError(id)
 
     def __contains__(self, id: str):
         """
         Tests whether a child named 'id' exists.
```

### Comparing `metaflow-2.8.2/metaflow/client/filecache.py` & `metaflow-2.8.3/metaflow/client/filecache.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/cmd/configure_cmd.py` & `metaflow-2.8.3/metaflow/cmd/configure_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,21 +245,21 @@
         cyan("[METAFLOW_DATASTORE_SYSROOT_S3]")
         + " Amazon S3 folder for Metaflow artifact storage "
         + "(s3://<bucket>/<prefix>).",
         default=existing_env.get("METAFLOW_DATASTORE_SYSROOT_S3"),
         show_default=True,
     )
     # Set Amazon S3 folder for datatools.
-    env["METAFLOW_DATATOOLS_SYSROOT_S3"] = click.prompt(
-        cyan("[METAFLOW_DATATOOLS_SYSROOT_S3]")
+    env["METAFLOW_DATATOOLS_S3ROOT"] = click.prompt(
+        cyan("[METAFLOW_DATATOOLS_S3ROOT]")
         + yellow(" (optional)")
         + " Amazon S3 folder for Metaflow datatools "
         + "(s3://<bucket>/<prefix>).",
         default=existing_env.get(
-            "METAFLOW_DATATOOLS_SYSROOT_S3",
+            "METAFLOW_DATATOOLS_S3ROOT",
             os.path.join(env["METAFLOW_DATASTORE_SYSROOT_S3"], "data"),
         ),
         show_default=True,
     )
     return env
```

### Comparing `metaflow-2.8.2/metaflow/cmd/main_cli.py` & `metaflow-2.8.3/metaflow/cmd/main_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 
 from metaflow._vendor import click
 
 from metaflow.extension_support.cmd import process_cmds, resolve_cmds
 from metaflow.plugins.datastores.local_storage import LocalStorage
-from metaflow.metaflow_config import DATASTORE_LOCAL_DIR
+from metaflow.metaflow_config import DATASTORE_LOCAL_DIR, CONTACT_INFO
+from metaflow.metaflow_version import get_version
 
 from .util import echo_always
 
 
 @click.group()
 def main():
     pass
@@ -76,31 +77,25 @@
     echo = echo_always
 
     import metaflow
 
     echo("Metaflow ", fg="magenta", bold=True, nl=False)
 
     if ctx.invoked_subcommand is None:
-        echo("(%s): " % metaflow.__version__, fg="magenta", bold=False, nl=False)
+        echo("(%s): " % get_version(), fg="magenta", bold=False, nl=False)
     else:
-        echo("(%s)\n" % metaflow.__version__, fg="magenta", bold=False)
+        echo("(%s)\n" % get_version(), fg="magenta", bold=False)
 
     if ctx.invoked_subcommand is None:
         echo("More data science, less engineering\n", fg="magenta")
 
-        # metaflow URL
-        echo("http://docs.metaflow.org", fg="cyan", nl=False)
-        echo(" - Read the documentation")
-
-        # metaflow chat
-        echo("http://chat.metaflow.org", fg="cyan", nl=False)
-        echo(" - Chat with us")
-
-        # metaflow help email
-        echo("help@metaflow.org", fg="cyan", nl=False)
-        echo("        - Get help by email\n")
+        lnk_sz = max(len(lnk) for lnk in CONTACT_INFO.values()) + 1
+        for what, lnk in CONTACT_INFO.items():
+            echo("%s%s" % (lnk, " " * (lnk_sz - len(lnk))), fg="cyan", nl=False)
+            echo("- %s" % what)
+        echo("")
 
         print(ctx.get_help())
 
 
 if __name__ == "__main__":
     start()
```

### Comparing `metaflow-2.8.2/metaflow/cmd/tutorials_cmd.py` & `metaflow-2.8.3/metaflow/cmd/tutorials_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/cmd_with_io.py` & `metaflow-2.8.3/metaflow/cmd_with_io.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/current.py` & `metaflow-2.8.3/metaflow/current.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from collections import namedtuple
 import os
 from typing import Any, Optional
 
+from metaflow.metaflow_config import TEMPDIR
+
 Parallel = namedtuple("Parallel", ["main_ip", "num_nodes", "node_index"])
 
 
 class Current(object):
     def __init__(self):
         self._flow_name = None
         self._run_id = None
@@ -13,14 +15,15 @@
         self._task_id = None
         self._retry_count = None
         self._origin_run_id = None
         self._namespace = None
         self._username = None
         self._metadata_str = None
         self._is_running = False
+        self._tempdir = TEMPDIR
 
         def _raise(ex):
             raise ex
 
         self.__class__.graph = property(
             fget=lambda _: _raise(RuntimeError("Graph is not available"))
         )
@@ -226,11 +229,23 @@
         """
         [Legacy function - do not use]
 
         Access tags through the Run object instead.
         """
         return self._tags
 
+    @property
+    def tempdir(self) -> str:
+        """
+        Currently configured temp dir.
+
+        Returns
+        -------
+        str
+            temp dir.
+        """
+        return self._tempdir
+
 
 # instantiate the Current singleton. This will be populated
 # by task.MetaflowTask before a task is executed.
 current = Current()
```

### Comparing `metaflow-2.8.2/metaflow/datastore/content_addressed_store.py` & `metaflow-2.8.3/metaflow/datastore/content_addressed_store.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/datastore/datastore_set.py` & `metaflow-2.8.3/metaflow/datastore/datastore_set.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/datastore/datastore_storage.py` & `metaflow-2.8.3/metaflow/datastore/datastore_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/datastore/flow_datastore.py` & `metaflow-2.8.3/metaflow/datastore/flow_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/datastore/task_datastore.py` & `metaflow-2.8.3/metaflow/datastore/task_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/debug.py` & `metaflow-2.8.3/metaflow/debug.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/decorators.py` & `metaflow-2.8.3/metaflow/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/event_logger.py` & `metaflow-2.8.3/metaflow/event_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/exception.py` & `metaflow-2.8.3/metaflow/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/extension_support/__init__.py` & `metaflow-2.8.3/metaflow/extension_support/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/extension_support/cmd.py` & `metaflow-2.8.3/metaflow/extension_support/cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/extension_support/integrations.py` & `metaflow-2.8.3/metaflow/extension_support/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/extension_support/plugins.py` & `metaflow-2.8.3/metaflow/extension_support/plugins.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/flowspec.py` & `metaflow-2.8.3/metaflow/flowspec.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/graph.py` & `metaflow-2.8.3/metaflow/graph.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/includefile.py` & `metaflow-2.8.3/metaflow/includefile.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/integrations.py` & `metaflow-2.8.3/metaflow/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/lint.py` & `metaflow-2.8.3/metaflow/lint.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/metadata/heartbeat.py` & `metaflow-2.8.3/metaflow/metadata/heartbeat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/metadata/metadata.py` & `metaflow-2.8.3/metaflow/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/metadata/util.py` & `metaflow-2.8.3/metaflow/metadata/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/metaflow_config.py` & `metaflow-2.8.3/metaflow/metaflow_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,16 @@
 DATATOOLS_S3ROOT = from_conf(
     "DATATOOLS_S3ROOT",
     os.path.join(DATASTORE_SYSROOT_S3, DATATOOLS_SUFFIX)
     if DATASTORE_SYSROOT_S3
     else None,
 )
 
+TEMPDIR = from_conf("TEMPDIR", ".")
+
 DATATOOLS_CLIENT_PARAMS = from_conf("DATATOOLS_CLIENT_PARAMS", {})
 if S3_ENDPOINT_URL:
     DATATOOLS_CLIENT_PARAMS["endpoint_url"] = S3_ENDPOINT_URL
 if S3_VERIFY_CERTIFICATE:
     DATATOOLS_CLIENT_PARAMS["verify"] = S3_VERIFY_CERTIFICATE
 
 DATATOOLS_SESSION_VARS = from_conf("DATATOOLS_SESSION_VARS", {})
@@ -189,16 +191,33 @@
 SERVICE_VERSION_CHECK = from_conf("SERVICE_VERSION_CHECK", True)
 
 # Default container image
 DEFAULT_CONTAINER_IMAGE = from_conf("DEFAULT_CONTAINER_IMAGE")
 # Default container registry
 DEFAULT_CONTAINER_REGISTRY = from_conf("DEFAULT_CONTAINER_REGISTRY")
 
+###
+# Organization customizations
+###
 UI_URL = from_conf("UI_URL")
 
+# Contact information displayed when running the `metaflow` command.
+# Value should be a dictionary where:
+#  - key is a string describing contact method
+#  - value is a string describing contact itself (email, web address, etc.)
+# The default value shows an example of this
+CONTACT_INFO = from_conf(
+    "CONTACT_INFO",
+    {
+        "Read the documentation": "http://docs.metaflow.org",
+        "Chat with us": "http://chat.metaflow.org",
+        "Get help by email": "help@metaflow.org",
+    },
+)
+
 ###
 # AWS Batch configuration
 ###
 # IAM role for AWS Batch container with Amazon S3 access
 # (and AWS DynamoDb access for AWS StepFunctions, if enabled)
 ECS_S3_ACCESS_IAM_ROLE = from_conf("ECS_S3_ACCESS_IAM_ROLE")
 # IAM role for AWS Batch container for AWS Fargate
@@ -256,14 +275,16 @@
 KUBERNETES_CONTAINER_IMAGE = from_conf(
     "KUBERNETES_CONTAINER_IMAGE", DEFAULT_CONTAINER_IMAGE
 )
 # Default container registry for K8S
 KUBERNETES_CONTAINER_REGISTRY = from_conf(
     "KUBERNETES_CONTAINER_REGISTRY", DEFAULT_CONTAINER_REGISTRY
 )
+# Toggle for trying to fetch EC2 instance metadata
+KUBERNETES_FETCH_EC2_METADATA = from_conf("KUBERNETES_FETCH_EC2_METADATA", False)
 
 ARGO_WORKFLOWS_KUBERNETES_SECRETS = from_conf("ARGO_WORKFLOWS_KUBERNETES_SECRETS", "")
 ARGO_WORKFLOWS_ENV_VARS_TO_SKIP = from_conf("ARGO_WORKFLOWS_ENV_VARS_TO_SKIP", "")
 
 ##
 # Airflow Configuration
 ##
```

### Comparing `metaflow-2.8.2/metaflow/metaflow_config_funcs.py` & `metaflow-2.8.3/metaflow/metaflow_config_funcs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/metaflow_environment.py` & `metaflow-2.8.3/metaflow/metaflow_environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             "after 6 tries. Exiting...' && exit 1; "
             "fi" % code_package_url,
             "TAR_OPTIONS='--warning=no-timestamp' tar xf job.tar",
             "mflog 'Task is starting.'",
         ]
         return cmds
 
-    def get_environment_info(self):
+    def get_environment_info(self, include_ext_info=False):
         global version_cache
         if version_cache is None:
             version_cache = metaflow_version.get_version()
 
         # note that this dict goes into the code package
         # so variables here should be relatively stable (no
         # timestamps) so the hash won't change all the time
@@ -183,17 +183,18 @@
             "metaflow_version": version_cache,
             "script": os.path.basename(os.path.abspath(sys.argv[0])),
         }
         if R.use_r():
             env["metaflow_r_version"] = R.metaflow_r_version()
             env["r_version"] = R.r_version()
             env["r_version_code"] = R.r_version_code()
-        # Information about extension modules (to load them in the proper order)
-        ext_key, ext_val = dump_module_info()
-        env[ext_key] = ext_val
+        if include_ext_info:
+            # Information about extension modules (to load them in the proper order)
+            ext_key, ext_val = dump_module_info()
+            env[ext_key] = ext_val
         return env
 
     def executable(self, step_name):
         return self._python()
 
     def _python(self):
         if R.use_r():
```

### Comparing `metaflow-2.8.2/metaflow/metaflow_version.py` & `metaflow-2.8.3/metaflow/metaflow_version.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/mflog/__init__.py` & `metaflow-2.8.3/metaflow/mflog/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/mflog/mflog.py` & `metaflow-2.8.3/metaflow/mflog/mflog.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/mflog/save_logs.py` & `metaflow-2.8.3/metaflow/mflog/save_logs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/mflog/save_logs_periodically.py` & `metaflow-2.8.3/metaflow/mflog/save_logs_periodically.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/mflog/tee.py` & `metaflow-2.8.3/metaflow/mflog/tee.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/monitor.py` & `metaflow-2.8.3/metaflow/monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/multicore_utils.py` & `metaflow-2.8.3/metaflow/multicore_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/package.py` & `metaflow-2.8.3/metaflow/package.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             # the user's working directory
             flowdir = os.path.dirname(os.path.abspath(sys.argv[0])) + "/"
             for path_tuple in self._walk(flowdir, suffixes=self.suffixes):
                 yield path_tuple
 
     def _add_info(self, tar):
         info = tarfile.TarInfo(os.path.basename(INFO_FILE))
-        env = self.environment.get_environment_info()
+        env = self.environment.get_environment_info(include_ext_info=True)
         buf = BytesIO()
         buf.write(json.dumps(env).encode("utf-8"))
         buf.seek(0)
         info.size = len(buf.getvalue())
         tar.addfile(info, buf)
 
     def _make(self):
```

### Comparing `metaflow-2.8.2/metaflow/parameters.py` & `metaflow-2.8.3/metaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/__init__.py` & `metaflow-2.8.3/metaflow/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/airflow/airflow.py` & `metaflow-2.8.3/metaflow/plugins/airflow/airflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 )
 from metaflow import current
 
 AIRFLOW_DEPLOY_TEMPLATE_FILE = os.path.join(os.path.dirname(__file__), "dag.py")
 
 
 class Airflow(object):
-
     TOKEN_STORAGE_ROOT = "mf.airflow"
 
     def __init__(
         self,
         name,
         graph,
         flow,
```

### Comparing `metaflow-2.8.2/metaflow/plugins/airflow/airflow_cli.py` & `metaflow-2.8.3/metaflow/plugins/airflow/airflow_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/airflow/airflow_decorator.py` & `metaflow-2.8.3/metaflow/plugins/airflow/airflow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/airflow/airflow_utils.py` & `metaflow-2.8.3/metaflow/plugins/airflow/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/airflow/plumbing/set_parameters.py` & `metaflow-2.8.3/metaflow/plugins/airflow/plumbing/set_parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/airflow/sensors/base_sensor.py` & `metaflow-2.8.3/metaflow/plugins/airflow/sensors/base_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/airflow/sensors/external_task_sensor.py` & `metaflow-2.8.3/metaflow/plugins/airflow/sensors/external_task_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/airflow/sensors/s3_sensor.py` & `metaflow-2.8.3/metaflow/plugins/airflow/sensors/s3_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/argo/argo_client.py` & `metaflow-2.8.3/metaflow/plugins/argo/argo_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/argo/argo_workflows.py` & `metaflow-2.8.3/metaflow/plugins/argo/argo_workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     DATASTORE_SYSROOT_S3,
     DATATOOLS_S3ROOT,
     DEFAULT_METADATA,
     KUBERNETES_NAMESPACE,
     KUBERNETES_NODE_SELECTOR,
     KUBERNETES_SANDBOX_INIT_SCRIPT,
     KUBERNETES_SECRETS,
+    KUBERNETES_FETCH_EC2_METADATA,
     S3_ENDPOINT_URL,
     AZURE_STORAGE_BLOB_SERVICE_ENDPOINT,
     DATASTORE_SYSROOT_AZURE,
     DATASTORE_SYSROOT_GS,
     CARD_AZUREROOT,
     CARD_GSROOT,
     DEFAULT_SECRETS_BACKEND_TYPE,
@@ -781,14 +782,15 @@
                         "METAFLOW_USER": "argo-workflows",
                         "METAFLOW_DATASTORE_SYSROOT_S3": DATASTORE_SYSROOT_S3,
                         "METAFLOW_DATATOOLS_S3ROOT": DATATOOLS_S3ROOT,
                         "METAFLOW_DEFAULT_DATASTORE": self.flow_datastore.TYPE,
                         "METAFLOW_DEFAULT_METADATA": DEFAULT_METADATA,
                         "METAFLOW_CARD_S3ROOT": CARD_S3ROOT,
                         "METAFLOW_KUBERNETES_WORKLOAD": 1,
+                        "METAFLOW_KUBERNETES_FETCH_EC2_METADATA": KUBERNETES_FETCH_EC2_METADATA,
                         "METAFLOW_RUNTIME_ENVIRONMENT": "kubernetes",
                         "METAFLOW_OWNER": self.username,
                     },
                     **{
                         # Some optional values for bookkeeping
                         "METAFLOW_FLOW_NAME": self.flow.name,
                         "METAFLOW_STEP_NAME": node.name,
```

### Comparing `metaflow-2.8.2/metaflow/plugins/argo/argo_workflows_cli.py` & `metaflow-2.8.3/metaflow/plugins/argo/argo_workflows_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/argo/argo_workflows_decorator.py` & `metaflow-2.8.3/metaflow/plugins/argo/argo_workflows_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/argo/process_input_paths.py` & `metaflow-2.8.3/metaflow/plugins/argo/process_input_paths.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/aws_client.py` & `metaflow-2.8.3/metaflow/plugins/aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/aws_utils.py` & `metaflow-2.8.3/metaflow/plugins/aws/aws_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,21 @@
     """
     meta = {}
     # Capture AWS instance identity metadata. This is best-effort only since
     # access to this end-point might be blocked on AWS and not available
     # for non-AWS deployments.
     # https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-identity-documents.html
     try:
+        # Set a very aggressive timeout, as the communication is happening in the same subnet,
+        # there should not be any significant delay in the response.
+        # Having a long default timeout here introduces unnecessary delay in launching tasks when the
+        # instance is unreachable.
         instance_meta = requests.get(
-            url="http://169.254.169.254/latest/dynamic/instance-identity/document"
+            url="http://169.254.169.254/latest/dynamic/instance-identity/document",
+            timeout=(1, 10),
         ).json()
         meta["ec2-instance-id"] = instance_meta.get("instanceId")
         meta["ec2-instance-type"] = instance_meta.get("instanceType")
         meta["ec2-region"] = instance_meta.get("region")
         meta["ec2-availability-zone"] = instance_meta.get("availabilityZone")
     except:
         pass
```

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/batch/batch.py` & `metaflow-2.8.3/metaflow/plugins/aws/batch/batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -175,14 +175,18 @@
         shared_memory=None,
         max_swap=None,
         swappiness=None,
         inferentia=None,
         env={},
         attrs={},
         host_volumes=None,
+        use_tmpfs=None,
+        tmpfs_tempdir=None,
+        tmpfs_size=None,
+        tmpfs_path=None,
         num_parallel=0,
     ):
         job_name = self._job_name(
             attrs.get("metaflow.user"),
             attrs.get("metaflow.flow_name"),
             attrs.get("metaflow.run_id"),
             attrs.get("metaflow.step_name"),
@@ -197,34 +201,39 @@
                 self._command(
                     self.environment, code_package_url, step_name, [step_cli], task_spec
                 )
             )
             .image(image)
             .iam_role(iam_role)
             .execution_role(execution_role)
+            .cpu(cpu)
+            .gpu(gpu)
+            .memory(memory)
+            .shared_memory(shared_memory)
+            .max_swap(max_swap)
+            .swappiness(swappiness)
+            .inferentia(inferentia)
+            .timeout_in_secs(run_time_limit)
             .job_def(
                 image,
                 iam_role,
                 queue,
                 execution_role,
                 shared_memory,
                 max_swap,
                 swappiness,
                 inferentia,
+                memory=memory,
                 host_volumes=host_volumes,
+                use_tmpfs=use_tmpfs,
+                tmpfs_tempdir=tmpfs_tempdir,
+                tmpfs_size=tmpfs_size,
+                tmpfs_path=tmpfs_path,
                 num_parallel=num_parallel,
             )
-            .cpu(cpu)
-            .gpu(gpu)
-            .memory(memory)
-            .shared_memory(shared_memory)
-            .max_swap(max_swap)
-            .swappiness(swappiness)
-            .inferentia(inferentia)
-            .timeout_in_secs(run_time_limit)
             .task_id(attrs.get("metaflow.task_id"))
             .environment_variable("AWS_DEFAULT_REGION", self._client.region())
             .environment_variable("METAFLOW_CODE_SHA", code_package_sha)
             .environment_variable("METAFLOW_CODE_URL", code_package_url)
             .environment_variable("METAFLOW_CODE_DS", code_package_ds)
             .environment_variable("METAFLOW_USER", attrs["metaflow.user"])
             .environment_variable("METAFLOW_SERVICE_URL", SERVICE_INTERNAL_URL)
@@ -244,14 +253,19 @@
             )
         if AWS_SECRETS_MANAGER_DEFAULT_REGION is not None:
             job.environment_variable(
                 "METAFLOW_AWS_SECRETS_MANAGER_DEFAULT_REGION",
                 AWS_SECRETS_MANAGER_DEFAULT_REGION,
             )
 
+        tmpfs_enabled = use_tmpfs or (tmpfs_size and use_tmpfs is None)
+
+        if tmpfs_enabled and tmpfs_tempdir:
+            job.environment_variable("METAFLOW_TEMPDIR", tmpfs_path)
+
         # Skip setting METAFLOW_DATASTORE_SYSROOT_LOCAL because metadata sync between the local user
         # instance and the remote AWS Batch instance assumes metadata is stored in DATASTORE_LOCAL_DIR
         # on the remote AWS Batch instance; this happens when METAFLOW_DATASTORE_SYSROOT_LOCAL
         # is NOT set (see get_datastore_root_from_config in datastore/local.py).
         # add METAFLOW_S3_ENDPOINT_URL
         if S3_ENDPOINT_URL is not None:
             job.environment_variable("METAFLOW_S3_ENDPOINT_URL", S3_ENDPOINT_URL)
@@ -296,14 +310,18 @@
         memory=None,
         run_time_limit=None,
         shared_memory=None,
         max_swap=None,
         swappiness=None,
         inferentia=None,
         host_volumes=None,
+        use_tmpfs=None,
+        tmpfs_tempdir=None,
+        tmpfs_size=None,
+        tmpfs_path=None,
         num_parallel=0,
         env={},
         attrs={},
     ):
         if queue is None:
             queue = next(self._client.active_job_queues(), None)
             if queue is None:
@@ -329,14 +347,18 @@
             shared_memory,
             max_swap,
             swappiness,
             inferentia,
             env=env,
             attrs=attrs,
             host_volumes=host_volumes,
+            use_tmpfs=use_tmpfs,
+            tmpfs_tempdir=tmpfs_tempdir,
+            tmpfs_size=tmpfs_size,
+            tmpfs_path=tmpfs_path,
             num_parallel=num_parallel,
         )
         self.num_parallel = num_parallel
         self.job = job.execute()
 
     def wait(self, stdout_location, stderr_location, echo=None):
         def wait_for_launch(job, child_jobs):
```

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/batch/batch_cli.py` & `metaflow-2.8.3/metaflow/plugins/aws/batch/batch_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -137,14 +137,18 @@
     default=5 * 24 * 60 * 60,
     help="Run time limit in seconds for the AWS Batch job. Default is 5 days.",
 )
 @click.option("--shared-memory", help="Shared Memory requirement for AWS Batch.")
 @click.option("--max-swap", help="Max Swap requirement for AWS Batch.")
 @click.option("--swappiness", help="Swappiness requirement for AWS Batch.")
 @click.option("--inferentia", help="Inferentia requirement for AWS Batch.")
+@click.option("--use-tmpfs", is_flag=True, help="tmpfs requirement for AWS Batch.")
+@click.option("--tmpfs-tempdir", is_flag=True, help="tmpfs requirement for AWS Batch.")
+@click.option("--tmpfs-size", help="tmpfs requirement for AWS Batch.")
+@click.option("--tmpfs-path", help="tmpfs requirement for AWS Batch.")
 # TODO: Maybe remove it altogether since it's not used here
 @click.option("--ubf-context", default=None, type=click.Choice([None, "ubf_control"]))
 @click.option("--host-volumes", multiple=True)
 @click.option(
     "--num-parallel",
     default=0,
     type=int,
@@ -165,14 +169,18 @@
     memory=None,
     queue=None,
     run_time_limit=None,
     shared_memory=None,
     max_swap=None,
     swappiness=None,
     inferentia=None,
+    use_tmpfs=None,
+    tmpfs_tempdir=None,
+    tmpfs_size=None,
+    tmpfs_path=None,
     host_volumes=None,
     num_parallel=None,
     **kwargs
 ):
     def echo(msg, stream="stderr", batch_id=None, **kwargs):
         msg = util.to_unicode(msg)
         if batch_id:
@@ -292,14 +300,18 @@
                 shared_memory=shared_memory,
                 max_swap=max_swap,
                 swappiness=swappiness,
                 inferentia=inferentia,
                 env=env,
                 attrs=attrs,
                 host_volumes=host_volumes,
+                use_tmpfs=use_tmpfs,
+                tmpfs_tempdir=tmpfs_tempdir,
+                tmpfs_size=tmpfs_size,
+                tmpfs_path=tmpfs_path,
                 num_parallel=num_parallel,
             )
     except Exception as e:
         traceback.print_exc()
         _sync_metadata()
         sys.exit(METAFLOW_EXIT_DISALLOW_RETRY)
     try:
```

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/batch/batch_client.py` & `metaflow-2.8.3/metaflow/plugins/aws/batch/batch_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,15 +145,20 @@
         job_role,
         job_queue,
         execution_role,
         shared_memory,
         max_swap,
         swappiness,
         inferentia,
+        memory,
         host_volumes,
+        use_tmpfs,
+        tmpfs_tempdir,
+        tmpfs_size,
+        tmpfs_path,
         num_parallel,
     ):
         # identify platform from any compute environment associated with the
         # queue
         if AWS_SANDBOX_ENABLED:
             # within the Metaflow sandbox, we can't execute the
             # describe_job_queues directive for AWS Batch to detect compute
@@ -247,15 +252,15 @@
                     job_definition["containerProperties"]["linuxParameters"][
                         "maxSwap"
                     ] = int(max_swap)
 
         if inferentia:
             if not (isinstance(inferentia, (int, unicode, basestring))):
                 raise BatchJobException(
-                    "invalid inferentia value: ({}) (should be 0 or greater)".format(
+                    "Invalid inferentia value: ({}) (should be 0 or greater)".format(
                         inferentia
                     )
                 )
             else:
                 job_definition["containerProperties"]["linuxParameters"]["devices"] = []
                 for i in range(int(inferentia)):
                     job_definition["containerProperties"]["linuxParameters"][
@@ -278,14 +283,37 @@
                 job_definition["containerProperties"]["volumes"].append(
                     {"name": name, "host": {"sourcePath": host_path}}
                 )
                 job_definition["containerProperties"]["mountPoints"].append(
                     {"sourceVolume": name, "containerPath": host_path}
                 )
 
+        if use_tmpfs or (tmpfs_size and use_tmpfs is None):
+            if tmpfs_size:
+                if not (isinstance(tmpfs_size, (int, unicode, basestring))):
+                    raise BatchJobException(
+                        "Invalid tmpfs value: ({}) (should be 0 or greater)".format(
+                            tmpfs_size
+                        )
+                    )
+            else:
+                # default tmpfs behavior - https://man7.org/linux/man-pages/man5/tmpfs.5.html
+                tmpfs_size = int(memory) / 2
+
+            job_definition["containerProperties"]["linuxParameters"]["tmpfs"] = [
+                {
+                    "containerPath": tmpfs_path,
+                    "size": int(tmpfs_size),
+                    "mountOptions": [
+                        # should map to rw, suid, dev, exec, auto, nouser, and async
+                        "defaults"
+                    ],
+                }
+            ]
+
         self.num_parallel = num_parallel or 0
         if self.num_parallel >= 1:
             job_definition["type"] = "multinode"
             job_definition["nodeProperties"] = {
                 "numNodes": self.num_parallel,
                 "mainNode": 0,
             }
@@ -339,27 +367,37 @@
         iam_role,
         job_queue,
         execution_role,
         shared_memory,
         max_swap,
         swappiness,
         inferentia,
+        memory,
         host_volumes,
+        use_tmpfs,
+        tmpfs_tempdir,
+        tmpfs_size,
+        tmpfs_path,
         num_parallel,
     ):
         self.payload["jobDefinition"] = self._register_job_definition(
             image,
             iam_role,
             job_queue,
             execution_role,
             shared_memory,
             max_swap,
             swappiness,
             inferentia,
+            memory,
             host_volumes,
+            use_tmpfs,
+            tmpfs_tempdir,
+            tmpfs_size,
+            tmpfs_path,
             num_parallel,
         )
         return self
 
     def job_name(self, job_name):
         self.payload["jobName"] = job_name
         return self
@@ -518,15 +556,14 @@
 
 class TriableException(Exception):
     def __init__(self, ex):
         self.ex = ex
 
 
 class RunningJob(object):
-
     NUM_RETRIES = 8
 
     def __init__(self, id, client):
         self._id = id
         self._client = client
         self._data = {}
```

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/batch/batch_decorator.py` & `metaflow-2.8.3/metaflow/plugins/aws/batch/batch_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,24 @@
         Docker where the value is the sum of the container memory plus the
         `max_swap` value.
     swappiness : int, optional
         This allows you to tune memory swappiness behavior for this step.
         A swappiness value of 0 causes swapping not to happen unless absolutely
         necessary. A swappiness value of 100 causes pages to be swapped very
         aggressively. Accepted values are whole numbers between 0 and 100.
+    use_tmpfs: bool, default: False
+        This enables an explicit tmpfs mount for this step.
+    tmpfs_tempdir: bool, default: True
+        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
+    tmpfs_size: int, optional
+        The value for the size (in MiB) of the tmpfs mount for this step.
+        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
+        memory allocated for this step.
+    tmpfs_path: string, optional
+        Path to tmpfs mount for this step. Defaults to /metaflow_temp.
     inferentia : int, default: 0
         Number of Inferentia chips required for this step.
     """
 
     name = "batch"
     defaults = {
         "cpu": None,
@@ -85,14 +95,18 @@
         "iam_role": ECS_S3_ACCESS_IAM_ROLE,
         "execution_role": ECS_FARGATE_EXECUTION_ROLE,
         "shared_memory": None,
         "max_swap": None,
         "swappiness": None,
         "inferentia": None,
         "host_volumes": None,
+        "use_tmpfs": False,
+        "tmpfs_tempdir": True,
+        "tmpfs_size": None,
+        "tmpfs_path": "/metaflow_temp",
     }
     resource_defaults = {
         "cpu": "1",
         "gpu": "0",
         "memory": "4096",
     }
     package_url = None
@@ -149,14 +163,18 @@
         self.run_time_limit = get_run_time_limit_for_task(decos)
         if self.run_time_limit < 60:
             raise BatchException(
                 "The timeout for step *{step}* should be at "
                 "least 60 seconds for execution on AWS Batch.".format(step=step)
             )
 
+        # Validate tmpfs_path. Batch requires this to be an absolute path
+        if self.attributes["tmpfs_path"] and self.attributes["tmpfs_path"][0] != "/":
+            raise BatchException("'tmpfs_path' needs to be an absolute path")
+
     def runtime_init(self, flow, graph, package, run_id):
         # Set some more internal state.
         self.flow = flow
         self.graph = graph
         self.package = package
         self.run_id = run_id
 
@@ -194,14 +212,19 @@
         max_retries,
         ubf_context,
         inputs,
     ):
         self.metadata = metadata
         self.task_datastore = task_datastore
 
+        # current.tempdir reflects the value of METAFLOW_TEMPDIR (the current working
+        # directory by default), or the value of tmpfs_path if tmpfs_tempdir=False.
+        if not self.attributes["tmpfs_tempdir"]:
+            current._update_env({"tempdir": self.attributes["tmpfs_path"]})
+
         # task_pre_step may run locally if fallback is activated for @catch
         # decorator. In that scenario, we skip collecting AWS Batch execution
         # metadata. A rudimentary way to detect non-local execution is to
         # check for the existence of AWS_BATCH_JOB_ID environment variable.
 
         if "AWS_BATCH_JOB_ID" in os.environ:
             meta = {}
```

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py` & `metaflow-2.8.3/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/step_functions/dynamo_db_client.py` & `metaflow-2.8.3/metaflow/plugins/aws/step_functions/dynamo_db_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/step_functions/event_bridge_client.py` & `metaflow-2.8.3/metaflow/plugins/aws/step_functions/event_bridge_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/step_functions/production_token.py` & `metaflow-2.8.3/metaflow/plugins/aws/step_functions/production_token.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/step_functions/schedule_decorator.py` & `metaflow-2.8.3/metaflow/plugins/aws/step_functions/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/step_functions/set_batch_environment.py` & `metaflow-2.8.3/metaflow/plugins/aws/step_functions/set_batch_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/step_functions/step_functions.py` & `metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,14 @@
                     "name of this flow or delete your "
                     "existing workflow on AWS Step "
                     "Functions." % name
                 )
         return None
 
     def _compile(self):
-
         # Visit every node of the flow and recursively build the state machine.
         def _visit(node, workflow, exit_node=None):
             if node.parallel_foreach:
                 raise StepFunctionsException(
                     "Deploying flows with @parallel decorator(s) "
                     "to AWS Step Functions is not supported currently."
                 )
@@ -633,16 +632,15 @@
                     "re-configure Metaflow using "
                     "*metaflow configure aws* on your "
                     "terminal."
                 )
             env["METAFLOW_SFN_DYNAMO_DB_TABLE"] = SFN_DYNAMO_DB_TABLE
 
         # It makes no sense to set env vars to None (shows up as "None" string)
-        env_without_none_values = {k: v for k, v in env.items() if v is not None}
-        del env
+        env = {k: v for k, v in env.items() if v is not None}
 
         # Resolve AWS Batch resource requirements.
         batch_deco = [deco for deco in node.decorators if deco.name == "batch"][0]
         resources = {}
         resources.update(batch_deco.attributes)
         resources.update(
             compute_resource_attributes(
@@ -682,15 +680,20 @@
                 cpu=resources["cpu"],
                 gpu=resources["gpu"],
                 memory=resources["memory"],
                 run_time_limit=batch_deco.run_time_limit,
                 shared_memory=resources["shared_memory"],
                 max_swap=resources["max_swap"],
                 swappiness=resources["swappiness"],
-                env=env_without_none_values,
+                use_tmpfs=resources["use_tmpfs"],
+                tmpfs_tempdir=resources["tmpfs_tempdir"],
+                tmpfs_size=resources["tmpfs_size"],
+                tmpfs_path=resources["tmpfs_path"],
+                inferentia=resources["inferentia"],
+                env=env,
                 attrs=attrs,
                 host_volumes=resources["host_volumes"],
             )
             .attempts(total_retries + 1)
         )
 
     def _get_retries(self, node):
```

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/step_functions/step_functions_cli.py` & `metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,14 @@
         is_project=is_project,
     )
 
 
 def resolve_token(
     name, token_prefix, obj, authorize, given_token, generate_new_token, is_project
 ):
-
     # 1) retrieve the previous deployment, if one exists
     workflow = StepFunctions.get_existing_deployment(name)
     if workflow is None:
         obj.echo(
             "It seems this is the first time you are deploying *%s* to "
             "AWS Step Functions." % name
         )
```

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/step_functions/step_functions_client.py` & `metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/aws/step_functions/step_functions_decorator.py` & `metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/azure/azure_tail.py` & `metaflow-2.8.3/metaflow/plugins/azure/azure_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/azure/azure_utils.py` & `metaflow-2.8.3/metaflow/plugins/azure/azure_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/azure/blob_service_client_factory.py` & `metaflow-2.8.3/metaflow/plugins/azure/blob_service_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/azure/includefile_support.py` & `metaflow-2.8.3/metaflow/plugins/azure/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_cli.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_client.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_datastore.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_decorator.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_modules/__init__.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_modules/base.html` & `metaflow-2.8.3/metaflow/plugins/cards/card_modules/base.html`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_modules/basic.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_modules/basic.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_modules/bundle.css` & `metaflow-2.8.3/metaflow/plugins/cards/card_modules/bundle.css`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_modules/card.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_modules/card.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_modules/chevron/main.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/main.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_modules/chevron/renderer.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/renderer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_modules/chevron/tokenizer.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_modules/components.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_modules/components.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_modules/convert_to_native_type.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_modules/convert_to_native_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -291,33 +291,95 @@
 
     def _parse_type(self, data_object):
         return data_object.__name__
 
     def _parse_range(self, data_object):
         return self._get_repr().repr(data_object)
 
+    @staticmethod
+    def _parse_pandas_column(column_object):
+        # There are two types of parsing we do here.
+        # 1. We explicitly parse the types we know how to parse
+        # 2. We try to partially match a type name to the column's type.
+        #   - We do this because `datetime64` can match `datetime64[ns]` and `datetime64[ns, UTC]`
+        #   - We do this because period can match `period[D]` and `period[2D]` etc.
+        #   - There are just too many types to explicitly parse so we go by this heuristic
+        # We have a default parser called `truncate_long_objects` which type casts any column to string
+        # and truncates it to 30 characters.
+        # If there is any form of TypeError or ValueError we set the column value to "Unsupported Type"
+        # We also set columns which are have null values to "null" strings
+        time_format = "%Y-%m-%dT%H:%M:%SZ"
+        truncate_long_objects = (
+            lambda x: x.astype("string").str.slice(0, 30) + "..."
+            if x.astype("string").str.len().max() > 30
+            else x.astype("string")
+        )
+        type_parser = {
+            "int64": lambda x: x,
+            "float64": lambda x: x,
+            "bool": lambda x: x,
+            "object": lambda x: truncate_long_objects(x.fillna("null")),
+            "category": truncate_long_objects,
+        }
+
+        partial_type_name_match_parsers = {
+            "complex": {
+                "complex": lambda x: x.astype("string"),
+            },
+            "datetime": {
+                "datetime64": lambda x: x.dt.strftime(time_format),
+                "timedelta": lambda x: x.dt.total_seconds(),
+            },
+            "interval": {
+                "interval": lambda x: x.astype("string"),
+            },
+            "period": {
+                "period": lambda x: x.astype("string"),
+            },
+        }
+
+        def _match_partial_type():
+            col_type = column_object.dtype
+            for _, type_parsers in partial_type_name_match_parsers.items():
+                for type_name, parser in type_parsers.items():
+                    if type_name in str(col_type):
+                        return parser(column_object)
+            return None
+
+        try:
+            col_type = str(column_object.dtype)
+            if col_type in type_parser:
+                return type_parser[col_type](column_object)
+            else:
+                parsed_col = _match_partial_type()
+                if parsed_col is not None:
+                    return parsed_col
+            return truncate_long_objects(column_object)
+        except ValueError as e:
+            return "Unsupported type: {0}".format(col_type)
+        except TypeError as e:
+            return "Unsupported type: {0}".format(col_type)
+
     def _parse_pandas_dataframe(self, data_object, truncate=True):
         headers = list(data_object.columns)
         data = data_object
         if truncate:
             data = data_object.head()
         index_column = data.index
         time_format = "%Y-%m-%dT%H:%M:%SZ"
-        if index_column.dtype == "datetime64[ns]":
+
+        if "datetime64" in str(index_column.dtype):
             if index_column.__class__.__name__ == "DatetimeIndex":
                 index_column = index_column.strftime(time_format)
             else:
                 index_column = index_column.dt.strftime(time_format)
 
         for col in data.columns:
-            # we convert datetime columns to strings
-            if data[col].dtype == "datetime64[ns]":
-                data[col] = data[col].dt.strftime(time_format)
+            data[col] = self._parse_pandas_column(data[col])
 
-        data = data.astype(object).where(data.notnull(), None)
         data_vals = data.values.tolist()
         for row, idx in zip(data_vals, index_column.values.tolist()):
             row.insert(0, idx)
         return dict(
             full_size=(
                 # full_size is a tuple of (num_rows,num_columns)
                 len(data_object),
```

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_modules/main.js` & `metaflow-2.8.3/metaflow/plugins/cards/card_modules/main.js`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_modules/renderer_tools.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_modules/renderer_tools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_modules/test_cards.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_modules/test_cards.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/card_resolver.py` & `metaflow-2.8.3/metaflow/plugins/cards/card_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/component_serializer.py` & `metaflow-2.8.3/metaflow/plugins/cards/component_serializer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/cards/exception.py` & `metaflow-2.8.3/metaflow/plugins/cards/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/catch_decorator.py` & `metaflow-2.8.3/metaflow/plugins/catch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/conda/__init__.py` & `metaflow-2.8.3/metaflow/plugins/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/conda/batch_bootstrap.py` & `metaflow-2.8.3/metaflow/plugins/conda/batch_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/conda/conda.py` & `metaflow-2.8.3/metaflow/plugins/conda/conda.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/conda/conda_environment.py` & `metaflow-2.8.3/metaflow/plugins/conda/conda_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,9 +128,9 @@
             "deps": info[env_id]["deps"],
         }
         return new_info
 
     def get_package_commands(self, code_package_url, datastore_type):
         return self.base_env.get_package_commands(code_package_url, datastore_type)
 
-    def get_environment_info(self):
-        return self.base_env.get_environment_info()
+    def get_environment_info(self, include_ext_info=False):
+        return self.base_env.get_environment_info(include_ext_info)
```

### Comparing `metaflow-2.8.2/metaflow/plugins/conda/conda_flow_decorator.py` & `metaflow-2.8.3/metaflow/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/conda/conda_step_decorator.py` & `metaflow-2.8.3/metaflow/plugins/conda/conda_step_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,21 @@
             # EXT_PKG extensions are PYTHONPATH extensions. Instead of re-resolving,
             # we use the resolved information that is written out to the INFO file.
             with open(
                 os.path.join(self.metaflow_home, info_file_name),
                 mode="wt",
                 encoding="utf-8",
             ) as f:
-                f.write(json.dumps(self._cur_environment.get_environment_info()))
+                f.write(
+                    json.dumps(
+                        self._cur_environment.get_environment_info(
+                            include_ext_info=True
+                        )
+                    )
+                )
 
         # Do the same for EXT_PKG
         try:
             m = importlib.import_module(EXT_PKG)
         except ImportError:
             # No additional check needed because if we are here, we already checked
             # for other issues when loading at the toplevel
```

### Comparing `metaflow-2.8.2/metaflow/plugins/datastores/azure_storage.py` & `metaflow-2.8.3/metaflow/plugins/datastores/azure_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/datastores/gs_storage.py` & `metaflow-2.8.3/metaflow/plugins/datastores/gs_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/datastores/local_storage.py` & `metaflow-2.8.3/metaflow/plugins/datastores/local_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/datastores/s3_storage.py` & `metaflow-2.8.3/metaflow/plugins/datastores/s3_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/datatools/__init__.py` & `metaflow-2.8.3/metaflow/plugins/datatools/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/datatools/local.py` & `metaflow-2.8.3/metaflow/plugins/datatools/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/datatools/s3/s3.py` & `metaflow-2.8.3/metaflow/plugins/datatools/s3/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from metaflow import FlowSpec
 from metaflow.current import current
 from metaflow.metaflow_config import (
     DATATOOLS_S3ROOT,
     S3_RETRY_COUNT,
     S3_TRANSIENT_RETRY_COUNT,
+    TEMPDIR,
 )
 from metaflow.util import (
     namedtuple_with_defaults,
     is_stringish,
     to_bytes,
     to_unicode,
     to_fileobj,
@@ -138,15 +139,14 @@
         path: str,
         size: Optional[int] = None,
         content_type: Optional[str] = None,
         metadata: Optional[Dict[str, str]] = None,
         range_info: Optional[RangeInfo] = None,
         last_modified: int = None,
     ):
-
         # all fields of S3Object should return a unicode object
         prefix, url, path = map(ensure_unicode, (prefix, url, path))
 
         self._size = size
         self._url = url
         self._path = path
         self._key = None
@@ -477,15 +477,15 @@
 
     @classmethod
     def get_root_from_config(cls, echo, create_on_absent=True):
         return DATATOOLS_S3ROOT
 
     def __init__(
         self,
-        tmproot: str = ".",
+        tmproot: str = TEMPDIR,
         bucket: Optional[str] = None,
         prefix: Optional[str] = None,
         run: Optional[Union[FlowSpec, "Run"]] = None,
         s3root: Optional[str] = None,
         **kwargs
     ):
         if not boto_found:
```

### Comparing `metaflow-2.8.2/metaflow/plugins/datatools/s3/s3op.py` & `metaflow-2.8.3/metaflow/plugins/datatools/s3/s3op.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/datatools/s3/s3tail.py` & `metaflow-2.8.3/metaflow/plugins/datatools/s3/s3tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/datatools/s3/s3util.py` & `metaflow-2.8.3/metaflow/plugins/datatools/s3/s3util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/debug_logger.py` & `metaflow-2.8.3/metaflow/plugins/debug_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/debug_monitor.py` & `metaflow-2.8.3/metaflow/plugins/debug_monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/__init__.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/client.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/client_modules.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/client_modules.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/communication/bytestream.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/communication/bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/communication/channel.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/communication/channel.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def recv(self, timeout=None):
         # To receive, we first receive the size of the object and then the object itself
         try:
             sz_bytes = self._stream.read(self._fmt.size, timeout)
             msg_sz = self._fmt.unpack(sz_bytes)[0]
             obj_bytes = self._stream.read(msg_sz, timeout)
-            return json.loads(obj_bytes, encoding="utf-8")
+            return json.loads(obj_bytes)
         except EOFError as e:
             raise RuntimeError("Cannot receive object over streaming interface: %s" % e)
         except BaseException as e:
             raise ValueError("Cannot deserialize object: %s" % traceback.format_exc())
 
     def fileno(self):
         return self._stream.fileno()
```

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/communication/socket_bytestream.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/communication/socket_bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/communication/utils.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/communication/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/consts.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/consts.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/data_transferer.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/data_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/exception_transferer.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/exception_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/override_decorators.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/override_decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/server.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/server.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/stub.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/stub.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/env_escape/utils.py` & `metaflow-2.8.3/metaflow/plugins/env_escape/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/environment_decorator.py` & `metaflow-2.8.3/metaflow/plugins/environment_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/frameworks/pytorch.py` & `metaflow-2.8.3/metaflow/plugins/frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/gcp/gs_storage_client_factory.py` & `metaflow-2.8.3/metaflow/plugins/gcp/gs_storage_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/gcp/gs_tail.py` & `metaflow-2.8.3/metaflow/plugins/gcp/gs_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/gcp/gs_utils.py` & `metaflow-2.8.3/metaflow/plugins/gcp/gs_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/gcp/includefile_support.py` & `metaflow-2.8.3/metaflow/plugins/gcp/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/kubernetes/kubernetes.py` & `metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     SERVICE_INTERNAL_URL,
     CARD_S3ROOT,
     DATASTORE_SYSROOT_S3,
     DATATOOLS_S3ROOT,
     DEFAULT_AWS_CLIENT_PROVIDER,
     DEFAULT_METADATA,
     KUBERNETES_SANDBOX_INIT_SCRIPT,
+    KUBERNETES_FETCH_EC2_METADATA,
     S3_ENDPOINT_URL,
     AZURE_STORAGE_BLOB_SERVICE_ENDPOINT,
     DATASTORE_SYSROOT_AZURE,
     CARD_AZUREROOT,
     CARD_GSROOT,
     DATASTORE_SYSROOT_GS,
     DEFAULT_SECRETS_BACKEND_TYPE,
@@ -195,14 +196,17 @@
                 json.dumps(SERVICE_HEADERS),
             )
             .environment_variable("METAFLOW_DATASTORE_SYSROOT_S3", DATASTORE_SYSROOT_S3)
             .environment_variable("METAFLOW_DATATOOLS_S3ROOT", DATATOOLS_S3ROOT)
             .environment_variable("METAFLOW_DEFAULT_DATASTORE", self._datastore.TYPE)
             .environment_variable("METAFLOW_DEFAULT_METADATA", DEFAULT_METADATA)
             .environment_variable("METAFLOW_KUBERNETES_WORKLOAD", 1)
+            .environment_variable(
+                "METAFLOW_KUBERNETES_FETCH_EC2_METADATA", KUBERNETES_FETCH_EC2_METADATA
+            )
             .environment_variable("METAFLOW_RUNTIME_ENVIRONMENT", "kubernetes")
             .environment_variable(
                 "METAFLOW_DEFAULT_SECRETS_BACKEND_TYPE", DEFAULT_SECRETS_BACKEND_TYPE
             )
             .environment_variable("METAFLOW_CARD_S3ROOT", CARD_S3ROOT)
             .environment_variable(
                 "METAFLOW_DEFAULT_AWS_CLIENT_PROVIDER", DEFAULT_AWS_CLIENT_PROVIDER
```

### Comparing `metaflow-2.8.2/metaflow/plugins/kubernetes/kubernetes_cli.py` & `metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/kubernetes/kubernetes_client.py` & `metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/kubernetes/kubernetes_decorator.py` & `metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     KUBERNETES_CONTAINER_REGISTRY,
     KUBERNETES_GPU_VENDOR,
     KUBERNETES_NAMESPACE,
     KUBERNETES_NODE_SELECTOR,
     KUBERNETES_TOLERATIONS,
     KUBERNETES_SERVICE_ACCOUNT,
     KUBERNETES_SECRETS,
+    KUBERNETES_FETCH_EC2_METADATA,
 )
 from metaflow.plugins.resources_decorator import ResourcesDecorator
 from metaflow.plugins.timeout_decorator import get_run_time_limit_for_task
 from metaflow.sidecar import Sidecar
 
 from ..aws.aws_utils import get_docker_registry, get_ec2_instance_metadata
 
@@ -323,16 +324,19 @@
             meta["kubernetes-pod-service-account-name"] = os.environ[
                 "METAFLOW_KUBERNETES_SERVICE_ACCOUNT_NAME"
             ]
             meta["kubernetes-node-ip"] = os.environ["METAFLOW_KUBERNETES_NODE_IP"]
 
             # TODO (savin): Introduce equivalent support for Microsoft Azure and
             #               Google Cloud Platform
-            instance_meta = get_ec2_instance_metadata()
-            meta.update(instance_meta)
+            # TODO: Introduce a way to detect Cloud Provider, so unnecessary requests (and delays)
+            # can be avoided by not having to try out all providers.
+            if KUBERNETES_FETCH_EC2_METADATA:
+                instance_meta = get_ec2_instance_metadata()
+                meta.update(instance_meta)
 
             # Unfortunately, there doesn't seem to be any straight forward way right
             # now to attach the Batch/v1 name - While we can rely on a hacky approach
             # given we know that the pod name is simply a unique suffix with a hyphen
             # delimiter to the Batch/v1 name - this approach will fail if the Batch/v1
             # name is closer to 63 chars where the pod name will truncate the Batch/v1
             # name.
```

### Comparing `metaflow-2.8.2/metaflow/plugins/kubernetes/kubernetes_job.py` & `metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -409,16 +409,31 @@
                         stdin=False,
                         stdout=True,
                         tty=False,
                     )
                 except:
                     # Best effort. It's likely that this API call could be
                     # blocked for the user.
-                    pass
-                    # raise
+                    # --------------------------------------------------------
+                    # We try patching Job parallelism anyway. Stopping any runaway
+                    # jobs (and their pods) is secondary to correctly showing
+                    # "Killed" status on the Kubernetes pod.
+                    #
+                    # This has the effect of pausing the job.
+                    try:
+                        client.BatchV1Api().patch_namespaced_job(
+                            name=self._name,
+                            namespace=self._namespace,
+                            field_manager="metaflow",
+                            body={"spec": {"parallelism": 0}},
+                        )
+                    except:
+                        # Best effort.
+                        pass
+                        # raise
             else:
                 # Case 2.
                 # This has the effect of pausing the job.
                 try:
                     client.BatchV1Api().patch_namespaced_job(
                         name=self._name,
                         namespace=self._namespace,
```

### Comparing `metaflow-2.8.2/metaflow/plugins/metadata/local.py` & `metaflow-2.8.3/metaflow/plugins/metadata/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/metadata/service.py` & `metaflow-2.8.3/metaflow/plugins/metadata/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,17 +133,18 @@
         elif heartbeat_type == HeartbeatTypes.RUN:
             # create run heartbeat
             data = {"flow_id": flow_id, "run_number": run_id}
 
             payload[HB_URL_KEY] = self.url_run_template.format(**data)
         else:
             raise Exception("invalid heartbeat type")
-        payload["service_version"] = self.version()
+        service_version = self.version()
+        payload["service_version"] = service_version
         # start sidecar
-        if self.version() is None or LooseVersion(self.version()) < LooseVersion(
+        if service_version is None or LooseVersion(service_version) < LooseVersion(
             "2.0.4"
         ):
             # if old version of the service is running
             # then avoid running real heartbeat sidecar process
             self.sidecar = Sidecar("none")
         else:
             self.sidecar = Sidecar("heartbeat")
```

### Comparing `metaflow-2.8.2/metaflow/plugins/package_cli.py` & `metaflow-2.8.3/metaflow/plugins/package_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/parallel_decorator.py` & `metaflow-2.8.3/metaflow/plugins/parallel_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/project_decorator.py` & `metaflow-2.8.3/metaflow/plugins/project_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/resources_decorator.py` & `metaflow-2.8.3/metaflow/plugins/resources_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/retry_decorator.py` & `metaflow-2.8.3/metaflow/plugins/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/secrets/secrets_decorator.py` & `metaflow-2.8.3/metaflow/plugins/secrets/secrets_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/storage_executor.py` & `metaflow-2.8.3/metaflow/plugins/storage_executor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/tag_cli.py` & `metaflow-2.8.3/metaflow/plugins/tag_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/test_unbounded_foreach_decorator.py` & `metaflow-2.8.3/metaflow/plugins/test_unbounded_foreach_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/plugins/timeout_decorator.py` & `metaflow-2.8.3/metaflow/plugins/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/procpoll.py` & `metaflow-2.8.3/metaflow/procpoll.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/pylint_wrapper.py` & `metaflow-2.8.3/metaflow/pylint_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/runtime.py` & `metaflow-2.8.3/metaflow/runtime.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/sidecar/sidecar.py` & `metaflow-2.8.3/metaflow/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/sidecar/sidecar_messages.py` & `metaflow-2.8.3/metaflow/sidecar/sidecar_messages.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/sidecar/sidecar_subprocess.py` & `metaflow-2.8.3/metaflow/sidecar/sidecar_subprocess.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/sidecar/sidecar_worker.py` & `metaflow-2.8.3/metaflow/sidecar/sidecar_worker.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tagging_util.py` & `metaflow-2.8.3/metaflow/tagging_util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/task.py` & `metaflow-2.8.3/metaflow/task.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/00-helloworld/helloworld.py` & `metaflow-2.8.3/metaflow/tutorials/00-helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/01-playlist/README.md` & `metaflow-2.8.3/metaflow/tutorials/01-playlist/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/01-playlist/movies.csv` & `metaflow-2.8.3/metaflow/tutorials/01-playlist/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/01-playlist/playlist.ipynb` & `metaflow-2.8.3/metaflow/tutorials/01-playlist/playlist.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/01-playlist/playlist.py` & `metaflow-2.8.3/metaflow/tutorials/01-playlist/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/02-statistics/README.md` & `metaflow-2.8.3/metaflow/tutorials/02-statistics/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/02-statistics/movies.csv` & `metaflow-2.8.3/metaflow/tutorials/02-statistics/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/02-statistics/stats.ipynb` & `metaflow-2.8.3/metaflow/tutorials/02-statistics/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/02-statistics/stats.py` & `metaflow-2.8.3/metaflow/tutorials/02-statistics/stats.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/03-playlist-redux/README.md` & `metaflow-2.8.3/metaflow/tutorials/03-playlist-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/03-playlist-redux/playlist.py` & `metaflow-2.8.3/metaflow/tutorials/03-playlist-redux/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/04-playlist-plus/README.md` & `metaflow-2.8.3/metaflow/tutorials/04-playlist-plus/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/04-playlist-plus/playlist.py` & `metaflow-2.8.3/metaflow/tutorials/04-playlist-plus/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/05-hello-cloud/README.md` & `metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb` & `metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/05-hello-cloud/hello-cloud.py` & `metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/hello-cloud.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/06-statistics-redux/README.md` & `metaflow-2.8.3/metaflow/tutorials/06-statistics-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/06-statistics-redux/stats.ipynb` & `metaflow-2.8.3/metaflow/tutorials/06-statistics-redux/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/07-worldview/worldview.ipynb` & `metaflow-2.8.3/metaflow/tutorials/07-worldview/worldview.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/08-autopilot/README.md` & `metaflow-2.8.3/metaflow/tutorials/08-autopilot/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/tutorials/08-autopilot/autopilot.ipynb` & `metaflow-2.8.3/metaflow/tutorials/08-autopilot/autopilot.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/util.py` & `metaflow-2.8.3/metaflow/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow/vendor.py` & `metaflow-2.8.3/metaflow/vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/metaflow.egg-info/PKG-INFO` & `metaflow-2.8.3/metaflow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow
-Version: 2.8.2
+Version: 2.8.3
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
@@ -69,12 +69,7 @@
 * Open an issue at: https://github.com/Netflix/metaflow 
 * Email us at: help@metaflow.org
 * Chat with us on: http://chat.metaflow.org 
 
 ## Contributing
 
 We welcome contributions to Metaflow. Please see our [contribution guide](https://docs.metaflow.org/introduction/contributing-to-metaflow) for more details.
-
-### Code style
-
-We use [black](https://black.readthedocs.io/en/stable/) as a code formatter. The easiest way to ensure your commits are always formatted with the correct version of `black` it is to use [pre-commit](https://pre-commit.com/): install it and then run `pre-commit install` once in your local copy of the repo.
-
```

### Comparing `metaflow-2.8.2/metaflow.egg-info/SOURCES.txt` & `metaflow-2.8.3/metaflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.2/setup.py` & `metaflow-2.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "2.8.2"
+version = "2.8.3"
 
 setup(
     include_package_data=True,
     name="metaflow",
     version=version,
     description="Metaflow: More Data Science, Less Engineering",
     long_description=open("README.md").read(),
```

