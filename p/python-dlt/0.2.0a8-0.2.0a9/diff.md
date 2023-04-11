# Comparing `tmp/python_dlt-0.2.0a8.tar.gz` & `tmp/python_dlt-0.2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dlt-0.2.0a8.tar", max compression
+gzip compressed data, was "python_dlt-0.2.0a9.tar", max compression
```

## Comparing `python_dlt-0.2.0a8.tar` & `python_dlt-0.2.0a9.tar`

### file list

```diff
@@ -1,195 +1,195 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 python_dlt-0.2.0a8/LICENSE.txt
--rw-r--r--   0        0        0     4222 2022-09-15 12:13:36.104313 python_dlt-0.2.0a8/QUICKSTART.md
--rw-r--r--   0        0        0     1555 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/__init__.py
--rw-r--r--   0        0        0       21 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/__version__.py
--rw-r--r--   0        0        0       31 2022-11-27 12:55:51.874732 python_dlt-0.2.0a8/dlt/cli/__init__.py
--rw-r--r--   0        0        0     7512 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     1961 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    15801 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0      162 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/cli/echo.py
--rw-r--r--   0        0        0      259 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    13790 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/cli/init_command.py
--rw-r--r--   0        0        0      106 2022-11-27 12:56:10.734732 python_dlt-0.2.0a8/dlt/cli/typing.py
--rw-r--r--   0        0        0     2490 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/cli/utils.py
--rw-r--r--   0        0        0      245 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 python_dlt-0.2.0a8/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      451 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     4489 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     2630 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     5694 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     5816 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0      252 2022-12-02 14:59:55.574492 python_dlt-0.2.0a8/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0     1095 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1199 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     2068 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0      762 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0     3170 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    16225 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0      837 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     8648 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0      503 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/specs/config_namespace_context.py
--rw-r--r--   0        0        0     1683 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     1196 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0     2918 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/specs/gcp_client_credentials.py
--rw-r--r--   0        0        0      556 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/specs/load_volume_configuration.py
--rw-r--r--   0        0        0      417 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/specs/normalize_volume_configuration.py
--rw-r--r--   0        0        0     1062 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/specs/pool_runner_configuration.py
--rw-r--r--   0        0        0     2313 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/specs/postgres_credentials.py
--rw-r--r--   0        0        0     1812 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0      944 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/specs/schema_volume_configuration.py
--rw-r--r--   0        0        0     4926 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      260 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     5149 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     1696 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     5235 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0     6567 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/common/destination.py
--rw-r--r--   0        0        0     4545 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/common/exceptions.py
--rw-r--r--   0        0        0     2220 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/git.py
--rw-r--r--   0        0        0     4184 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/common/json.py
--rw-r--r--   0        0        0     8725 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/common/logger.py
--rw-r--r--   0        0        0        0 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0      472 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0      691 2022-12-02 14:59:55.584492 python_dlt-0.2.0a8/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    10510 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0      300 2022-06-27 16:30:05.091379 python_dlt-0.2.0a8/dlt/common/normalizers/names/__init__.py
--rw-r--r--   0        0        0     2600 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/common/normalizers/names/snake_case.py
--rw-r--r--   0        0        0      406 2022-06-03 17:49:47.664600 python_dlt-0.2.0a8/dlt/common/pendulum.py
--rw-r--r--   0        0        0     6055 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4644 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     2517 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      154 2022-08-26 15:28:07.203730 python_dlt-0.2.0a8/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      768 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/runners/init.py
--rw-r--r--   0        0        0     7529 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4041 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0      728 2022-06-28 10:52:24.103559 python_dlt-0.2.0a8/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     3629 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/runners/venv.py
--rw-r--r--   0        0        0      369 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0      772 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/schema/configuration.py
--rw-r--r--   0        0        0     1939 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2977 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    24247 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3010 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    24569 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1277 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/common/signals.py
--rw-r--r--   0        0        0      410 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1713 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     2582 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0     7767 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2527 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    12318 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2387 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8505 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     2465 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2054 2022-06-28 10:52:24.103559 python_dlt-0.2.0a8/dlt/common/telemetry.py
--rw-r--r--   0        0        0     1108 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/common/time.py
--rw-r--r--   0        0        0     3816 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/typing.py
--rw-r--r--   0        0        0     6708 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/common/wei.py
--rw-r--r--   0        0        0      876 2022-06-03 13:18:25.174600 python_dlt-0.2.0a8/dlt/dbt_runner/README.md
--rw-r--r--   0        0        0        0 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/dbt_runner/__init__.py
--rw-r--r--   0        0        0     2748 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/dbt_runner/configuration.py
--rw-r--r--   0        0        0      159 2022-06-03 13:18:25.174600 python_dlt-0.2.0a8/dlt/dbt_runner/exceptions.py
--rw-r--r--   0        0        0     8129 2022-12-02 14:59:55.594492 python_dlt-0.2.0a8/dlt/dbt_runner/runner.py
--rw-r--r--   0        0        0     3197 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/dbt_runner/utils.py
--rw-r--r--   0        0        0        0 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1725 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    11216 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      382 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0     6249 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1587 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      625 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4667 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     2939 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     7151 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0      251 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1847 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0      400 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0    10352 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     4768 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1191 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1778 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      306 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     3651 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     3478 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0      564 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 python_dlt-0.2.0a8/dlt/extract/__init__.py
--rw-r--r--   0        0        0    10674 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/extract/decorators.py
--rw-r--r--   0        0        0    10604 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     5430 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/extract/extract.py
--rw-r--r--   0        0        0    24256 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/extract/pipe.py
--rw-r--r--   0        0        0    22304 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/extract/source.py
--rw-r--r--   0        0        0     1500 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/extract/typing.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 python_dlt-0.2.0a8/dlt/helpers/__init__.py
--rw-r--r--   0        0        0     2373 2022-12-02 14:59:55.604492 python_dlt-0.2.0a8/dlt/helpers/pandas.py
--rw-r--r--   0        0        0     7360 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/helpers/streamlit.py
--rw-r--r--   0        0        0       31 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/load/__init__.py
--rw-r--r--   0        0        0      905 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/load/configuration.py
--rw-r--r--   0        0        0     1109 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/load/exceptions.py
--rw-r--r--   0        0        0    13834 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/load/load.py
--rw-r--r--   0        0        0       32 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1138 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 python_dlt-0.2.0a8/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    14328 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/normalize/normalize.py
--rw-r--r--   0        0        0     1880 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/pipeline/README.md
--rw-r--r--   0        0        0     3800 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1235 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0     3291 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0    44977 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0     5917 2022-12-04 21:46:36.159175 python_dlt-0.2.0a8/dlt/pipeline/state.py
--rw-r--r--   0        0        0     2803 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/pipeline/trace.py
--rw-r--r--   0        0        0       92 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 python_dlt-0.2.0a8/dlt/py.typed
--rw-r--r--   0        0        0        0 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/reflection/names.py
--rw-r--r--   0        0        0     2141 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     4605 2022-12-02 14:59:55.614492 python_dlt-0.2.0a8/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      745 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/.dlt/example.secrets.toml
--rw-r--r--   0        0        0     3777 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/README.md
--rw-r--r--   0        0        0        0 2022-05-20 13:04:18.202424 python_dlt-0.2.0a8/examples/__init__.py
--rw-r--r--   0        0        0     2859 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/_helpers.py
--rw-r--r--   0        0        0       91 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/chess/.dlt/config.toml
--rw-r--r--   0        0        0       75 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/chess/.dlt/secrets.toml
--rw-r--r--   0        0        0        0 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/chess/__init__.py
--rw-r--r--   0        0        0     1971 2022-12-02 15:00:00.154492 python_dlt-0.2.0a8/examples/chess/chess.py
--rw-r--r--   0        0        0    23882 2022-05-20 13:04:18.272424 python_dlt-0.2.0a8/examples/data/channels.json
--rw-r--r--   0        0        0      530 2022-05-31 08:33:39.199428 python_dlt-0.2.0a8/examples/data/demo_example.json
--rw-r--r--   0        0        0    71730 2022-05-20 13:04:18.602424 python_dlt-0.2.0a8/examples/data/messages.json
--rw-r--r--   0        0        0   386829 2022-06-26 22:03:48.615163 python_dlt-0.2.0a8/examples/data/rasa_trackers/2888158124550630_tracker.jsonl
--rw-r--r--   0        0        0   213456 2022-06-26 22:03:45.545163 python_dlt-0.2.0a8/examples/data/rasa_trackers/8629c904-0c26-4f0b-927b-14d48db43c28_tracker.jsonl
--rw-r--r--   0        0        0     2669 2022-06-23 14:46:53.157751 python_dlt-0.2.0a8/examples/data/singer_taps/csv_catalog.json
--rw-r--r--   0        0        0      210 2022-06-23 14:46:53.157751 python_dlt-0.2.0a8/examples/data/singer_taps/model_annotations.csv
--rw-r--r--   0        0        0     8010 2022-06-23 14:46:53.157751 python_dlt-0.2.0a8/examples/data/singer_taps/tap_google_sheet.jsonl
--rw-r--r--   0        0        0  4458258 2022-06-23 14:46:53.167751 python_dlt-0.2.0a8/examples/data/singer_taps/tap_hubspot.jsonl
--rw-r--r--   0        0        0     6429 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/demo_example.py
--rw-r--r--   0        0        0     3748 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/discord_iterator.py
--rw-r--r--   0        0        0     3371 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/google_drive_csv.py
--rw-r--r--   0        0        0      311 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/google_sheets.py
--rw-r--r--   0        0        0     6832 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/quickstart.py
--rw-r--r--   0        0        0     1358 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/rasa_example.py
--rw-r--r--   0        0        0     1467 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/read_table.py
--rw-r--r--   0        0        0     1068 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/restore_pipeline.py
--rw-r--r--   0        0        0        0 2022-06-09 15:05:08.450657 python_dlt-0.2.0a8/examples/schemas/__init__.py
--rw-r--r--   0        0        0    12510 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/schemas/discord.schema.yml
--rw-r--r--   0        0        0     1933 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/schemas/dlt_quickstart.schema.yaml
--rw-r--r--   0        0        0     1208 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/schemas/hubspot.schema.yaml
--rw-r--r--   0        0        0     4492 2022-12-02 14:59:55.624492 python_dlt-0.2.0a8/examples/schemas/inferred_demo.schema.yml
--rw-r--r--   0        0        0     1346 2022-12-02 14:59:55.634492 python_dlt-0.2.0a8/examples/singer_tap_example.py
--rw-r--r--   0        0        0      731 2022-12-02 14:59:55.634492 python_dlt-0.2.0a8/examples/singer_tap_jsonl_example.py
--rw-r--r--   0        0        0        0 2022-06-09 15:05:08.450657 python_dlt-0.2.0a8/examples/sources/__init__.py
--rw-r--r--   0        0        0     1969 2022-12-02 14:59:55.634492 python_dlt-0.2.0a8/examples/sources/google_sheets.py
--rw-r--r--   0        0        0     1029 2022-12-02 14:59:55.634492 python_dlt-0.2.0a8/examples/sources/jsonl.py
--rw-r--r--   0        0        0       22 2022-12-02 14:59:55.634492 python_dlt-0.2.0a8/examples/sources/rasa/__init__.py
--rw-r--r--   0        0        0     3287 2022-12-02 14:59:55.634492 python_dlt-0.2.0a8/examples/sources/rasa/rasa.py
--rw-r--r--   0        0        0     1959 2022-12-02 14:59:55.634492 python_dlt-0.2.0a8/examples/sources/rasa/rasa.schema.yaml
--rw-r--r--   0        0        0     3702 2022-12-02 14:59:55.634492 python_dlt-0.2.0a8/examples/sources/singer_tap.py
--rw-r--r--   0        0        0     2461 2022-12-02 14:59:55.634492 python_dlt-0.2.0a8/examples/sources/sql_query.py
--rw-r--r--   0        0        0      869 2022-12-02 14:59:55.634492 python_dlt-0.2.0a8/examples/sources/stdout.py
--rw-r--r--   0        0        0      807 2022-12-02 14:59:55.634492 python_dlt-0.2.0a8/examples/sync_schema_example.py
--rw-r--r--   0        0        0     3493 2022-12-04 21:47:06.439175 python_dlt-0.2.0a8/pyproject.toml
--rw-r--r--   0        0        0     7812 1970-01-01 00:00:00.000000 python_dlt-0.2.0a8/setup.py
--rw-r--r--   0        0        0     7444 1970-01-01 00:00:00.000000 python_dlt-0.2.0a8/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 python_dlt-0.2.0a9/LICENSE.txt
+-rw-r--r--   0        0        0     4222 2022-09-15 12:13:36.104313 python_dlt-0.2.0a9/QUICKSTART.md
+-rw-r--r--   0        0        0     1555 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/__init__.py
+-rw-r--r--   0        0        0       21 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/__version__.py
+-rw-r--r--   0        0        0       31 2022-11-27 12:55:51.874732 python_dlt-0.2.0a9/dlt/cli/__init__.py
+-rw-r--r--   0        0        0     7512 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     1961 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    15801 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0      162 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/cli/echo.py
+-rw-r--r--   0        0        0      259 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    14921 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/cli/init_command.py
+-rw-r--r--   0        0        0      106 2022-11-27 12:56:10.734732 python_dlt-0.2.0a9/dlt/cli/typing.py
+-rw-r--r--   0        0        0     2497 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/cli/utils.py
+-rw-r--r--   0        0        0      245 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 python_dlt-0.2.0a9/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      451 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     4489 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     2630 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     5694 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     5816 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0      252 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0     1095 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1199 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     2068 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0      762 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0     3170 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    16225 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0      837 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     8648 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0      503 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/config_namespace_context.py
+-rw-r--r--   0        0        0     1683 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     1196 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0     2918 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/gcp_client_credentials.py
+-rw-r--r--   0        0        0      556 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/load_volume_configuration.py
+-rw-r--r--   0        0        0      417 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/normalize_volume_configuration.py
+-rw-r--r--   0        0        0     1062 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/pool_runner_configuration.py
+-rw-r--r--   0        0        0     2313 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/postgres_credentials.py
+-rw-r--r--   0        0        0     1812 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0      944 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/schema_volume_configuration.py
+-rw-r--r--   0        0        0     4926 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      260 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     5149 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     1696 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     5235 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0     6567 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/destination.py
+-rw-r--r--   0        0        0     4545 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     2220 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/git.py
+-rw-r--r--   0        0        0     4184 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/json.py
+-rw-r--r--   0        0        0     8725 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/logger.py
+-rw-r--r--   0        0        0        0 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0      472 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0      691 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    10510 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0      300 2022-06-27 16:30:05.091379 python_dlt-0.2.0a9/dlt/common/normalizers/names/__init__.py
+-rw-r--r--   0        0        0     2600 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/normalizers/names/snake_case.py
+-rw-r--r--   0        0        0      406 2022-06-03 17:49:47.664600 python_dlt-0.2.0a9/dlt/common/pendulum.py
+-rw-r--r--   0        0        0     6055 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4644 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     2517 2022-12-05 21:04:23.672896 python_dlt-0.2.0a9/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      154 2022-08-26 15:28:07.203730 python_dlt-0.2.0a9/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      768 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/runners/init.py
+-rw-r--r--   0        0        0     7529 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4041 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0      728 2022-06-28 10:52:24.103559 python_dlt-0.2.0a9/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     3629 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0      369 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0      772 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/schema/configuration.py
+-rw-r--r--   0        0        0     1939 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2977 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    24247 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3010 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    24569 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1277 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/signals.py
+-rw-r--r--   0        0        0      410 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1713 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     2582 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0     7767 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2527 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    12318 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2387 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8505 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     2465 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2054 2022-06-28 10:52:24.103559 python_dlt-0.2.0a9/dlt/common/telemetry.py
+-rw-r--r--   0        0        0     1108 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/time.py
+-rw-r--r--   0        0        0     3816 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/typing.py
+-rw-r--r--   0        0        0     6708 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/wei.py
+-rw-r--r--   0        0        0      876 2022-06-03 13:18:25.174600 python_dlt-0.2.0a9/dlt/dbt_runner/README.md
+-rw-r--r--   0        0        0        0 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/dbt_runner/__init__.py
+-rw-r--r--   0        0        0     2748 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/dbt_runner/configuration.py
+-rw-r--r--   0        0        0      159 2022-06-03 13:18:25.174600 python_dlt-0.2.0a9/dlt/dbt_runner/exceptions.py
+-rw-r--r--   0        0        0     8129 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/dbt_runner/runner.py
+-rw-r--r--   0        0        0     3197 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/dbt_runner/utils.py
+-rw-r--r--   0        0        0        0 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     1725 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    11216 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0      382 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0     6283 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1587 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      625 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4667 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     3604 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     7151 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0      251 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     1847 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0      400 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0    10352 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     4830 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1191 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     1778 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      306 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     3651 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     3863 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0      564 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 python_dlt-0.2.0a9/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    10674 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    10604 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     5430 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/extract/extract.py
+-rw-r--r--   0        0        0    24256 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/extract/pipe.py
+-rw-r--r--   0        0        0    22304 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/extract/source.py
+-rw-r--r--   0        0        0     1500 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/extract/typing.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 python_dlt-0.2.0a9/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0     2373 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/helpers/pandas.py
+-rw-r--r--   0        0        0     7360 2022-12-05 22:14:32.612895 python_dlt-0.2.0a9/dlt/helpers/streamlit.py
+-rw-r--r--   0        0        0       31 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/load/__init__.py
+-rw-r--r--   0        0        0      905 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1109 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    13834 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1138 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 python_dlt-0.2.0a9/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    14328 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0     1880 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/pipeline/README.md
+-rw-r--r--   0        0        0     3800 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     1235 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0     3291 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0    44978 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0     5917 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/pipeline/state.py
+-rw-r--r--   0        0        0     2803 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0       92 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 python_dlt-0.2.0a9/dlt/py.typed
+-rw-r--r--   0        0        0        0 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/reflection/names.py
+-rw-r--r--   0        0        0     2141 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      745 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/.dlt/example.secrets.toml
+-rw-r--r--   0        0        0     3777 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/README.md
+-rw-r--r--   0        0        0        0 2022-05-20 13:04:18.202424 python_dlt-0.2.0a9/examples/__init__.py
+-rw-r--r--   0        0        0     2859 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/_helpers.py
+-rw-r--r--   0        0        0       91 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/chess/.dlt/config.toml
+-rw-r--r--   0        0        0       75 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/chess/.dlt/secrets.toml
+-rw-r--r--   0        0        0        0 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/chess/__init__.py
+-rw-r--r--   0        0        0     1971 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/examples/chess/chess.py
+-rw-r--r--   0        0        0    23882 2022-05-20 13:04:18.272424 python_dlt-0.2.0a9/examples/data/channels.json
+-rw-r--r--   0        0        0      530 2022-05-31 08:33:39.199428 python_dlt-0.2.0a9/examples/data/demo_example.json
+-rw-r--r--   0        0        0    71730 2022-05-20 13:04:18.602424 python_dlt-0.2.0a9/examples/data/messages.json
+-rw-r--r--   0        0        0   386829 2022-06-26 22:03:48.615163 python_dlt-0.2.0a9/examples/data/rasa_trackers/2888158124550630_tracker.jsonl
+-rw-r--r--   0        0        0   213456 2022-06-26 22:03:45.545163 python_dlt-0.2.0a9/examples/data/rasa_trackers/8629c904-0c26-4f0b-927b-14d48db43c28_tracker.jsonl
+-rw-r--r--   0        0        0     2669 2022-06-23 14:46:53.157751 python_dlt-0.2.0a9/examples/data/singer_taps/csv_catalog.json
+-rw-r--r--   0        0        0      210 2022-06-23 14:46:53.157751 python_dlt-0.2.0a9/examples/data/singer_taps/model_annotations.csv
+-rw-r--r--   0        0        0     8010 2022-06-23 14:46:53.157751 python_dlt-0.2.0a9/examples/data/singer_taps/tap_google_sheet.jsonl
+-rw-r--r--   0        0        0  4458258 2022-06-23 14:46:53.167751 python_dlt-0.2.0a9/examples/data/singer_taps/tap_hubspot.jsonl
+-rw-r--r--   0        0        0     6429 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/demo_example.py
+-rw-r--r--   0        0        0     3748 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/discord_iterator.py
+-rw-r--r--   0        0        0     3371 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/google_drive_csv.py
+-rw-r--r--   0        0        0      311 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/google_sheets.py
+-rw-r--r--   0        0        0     6832 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/quickstart.py
+-rw-r--r--   0        0        0     1358 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/rasa_example.py
+-rw-r--r--   0        0        0     1467 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/read_table.py
+-rw-r--r--   0        0        0     1068 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/restore_pipeline.py
+-rw-r--r--   0        0        0        0 2022-06-09 15:05:08.450657 python_dlt-0.2.0a9/examples/schemas/__init__.py
+-rw-r--r--   0        0        0    12510 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/schemas/discord.schema.yml
+-rw-r--r--   0        0        0     1933 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/schemas/dlt_quickstart.schema.yaml
+-rw-r--r--   0        0        0     1208 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/schemas/hubspot.schema.yaml
+-rw-r--r--   0        0        0     4492 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/schemas/inferred_demo.schema.yml
+-rw-r--r--   0        0        0     1346 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/singer_tap_example.py
+-rw-r--r--   0        0        0      731 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/singer_tap_jsonl_example.py
+-rw-r--r--   0        0        0        0 2022-06-09 15:05:08.450657 python_dlt-0.2.0a9/examples/sources/__init__.py
+-rw-r--r--   0        0        0     1969 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/google_sheets.py
+-rw-r--r--   0        0        0     1029 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/jsonl.py
+-rw-r--r--   0        0        0       22 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/rasa/__init__.py
+-rw-r--r--   0        0        0     3287 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/rasa/rasa.py
+-rw-r--r--   0        0        0     1959 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/rasa/rasa.schema.yaml
+-rw-r--r--   0        0        0     3702 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/singer_tap.py
+-rw-r--r--   0        0        0     2461 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/sql_query.py
+-rw-r--r--   0        0        0      869 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/stdout.py
+-rw-r--r--   0        0        0      807 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sync_schema_example.py
+-rw-r--r--   0        0        0     3493 2022-12-05 22:54:08.432896 python_dlt-0.2.0a9/pyproject.toml
+-rw-r--r--   0        0        0     7812 1970-01-01 00:00:00.000000 python_dlt-0.2.0a9/setup.py
+-rw-r--r--   0        0        0     7444 1970-01-01 00:00:00.000000 python_dlt-0.2.0a9/PKG-INFO
```

### Comparing `python_dlt-0.2.0a8/LICENSE.txt` & `python_dlt-0.2.0a9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/QUICKSTART.md` & `python_dlt-0.2.0a9/QUICKSTART.md`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/__init__.py` & `python_dlt-0.2.0a9/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/cli/_dlt.py` & `python_dlt-0.2.0a9/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/cli/config_toml_writer.py` & `python_dlt-0.2.0a9/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/cli/deploy_command.py` & `python_dlt-0.2.0a9/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/cli/init_command.py` & `python_dlt-0.2.0a9/dlt/cli/init_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import inspect
 import os
 import ast
 import click
 import shutil
+from astunparse import unparse
 from types import ModuleType
 from typing import Dict, List, Tuple
 from importlib.metadata import version as pkg_version
 
 from dlt.common.configuration import is_secret_hint, DOT_DLT, make_dot_dlt_path
 from dlt.common.configuration.providers import CONFIG_TOML, SECRETS_TOML, ConfigTomlProvider, SecretsTomlProvider
 from dlt.common.logger import DLT_PKG_NAME
@@ -23,46 +24,64 @@
 
 import dlt.cli.echo as fmt
 from dlt.cli import utils
 from dlt.cli.config_toml_writer import WritableConfigValue, write_values
 from dlt.cli.exceptions import CliCommandException
 
 
-def _find_argument_nodes_to_replace(visitor: PipelineScriptVisitor, replace_nodes: List[Tuple[str, str]], init_script_name: str) -> List[Tuple[ast.Constant, str, str]]:
+def _find_call_arguments_to_replace(visitor: PipelineScriptVisitor, replace_nodes: List[Tuple[str, str]], init_script_name: str) -> List[Tuple[ast.AST, ast.AST, str]]:
     # the input tuple (call argument name, replacement value)
     # the returned tuple (node, replacement value, node type)
-    transformed_nodes: List[Tuple[ast.Constant, str, str]] = []
+    transformed_nodes: List[Tuple[ast.AST, ast.AST, str]] = []
     known_calls: Dict[str, List[inspect.BoundArguments]] = visitor.known_calls
     for arg_name, calls in known_calls.items():
         for args in calls:
             for t_arg_name, t_value in replace_nodes:
                 dn_node: ast.AST = args.arguments.get(t_arg_name)
                 if dn_node is not None:
                     if not isinstance(dn_node, ast.Constant) or not isinstance(dn_node.value, str):
                         raise CliCommandException("init", f"The pipeline script {init_script_name} must pass the {t_arg_name} as string to '{arg_name}' function in line {dn_node.lineno}")
                     else:
-                        transformed_nodes.append((dn_node, t_value, t_arg_name))
+                        transformed_nodes.append((dn_node, ast.Constant(value=t_value, kind=None), t_arg_name))
 
     # there was at least one replacement
     for t_arg_name, _ in replace_nodes:
         if len(list(filter(lambda tn: tn[2] == t_arg_name, transformed_nodes))) == 0:
             raise CliCommandException("init", f"The pipeline script {init_script_name} is not explicitly passing the '{t_arg_name}' argument to 'pipeline' or 'run' function. In init script the default and configured values are not accepted.")
     return transformed_nodes
 
 
-def _detect_required_configs(visitor: PipelineScriptVisitor, script_module: ModuleType, init_script_name: str) -> Tuple[Dict[str, WritableConfigValue], Dict[str, WritableConfigValue]]:
+def _find_source_calls_to_replace(visitor: PipelineScriptVisitor, pipeline_name: str) -> List[Tuple[ast.AST, ast.AST, str]]:
+    transformed_nodes: List[Tuple[ast.AST, ast.AST, str]] = []
+    for source_def in visitor.known_sources_resources.values():
+        # recreate function name as a ast.Name with known source code location
+        func_name = ast.Name(source_def.name)
+        func_name.lineno = func_name.end_lineno = source_def.lineno
+        func_name.col_offset = visitor.source_lines[func_name.lineno - 1].index(source_def.name)  # find where function name starts
+        func_name.end_col_offset = func_name.col_offset + len(source_def.name)
+        # append function name to be replaces
+        transformed_nodes.append((func_name, ast.Name(id=pipeline_name + "_" + source_def.name), ""))
+
+    for calls in visitor.known_sources_resources_calls.values():
+        for call in calls:
+            transformed_nodes.append((call.func, ast.Name(id=pipeline_name + "_" + unparse(call.func)), ""))
+
+    return transformed_nodes
+
+
+def _detect_required_configs(visitor: PipelineScriptVisitor) -> Tuple[Dict[str, WritableConfigValue], Dict[str, WritableConfigValue]]:
     # all detected secrets with namespaces
     required_secrets: Dict[str, WritableConfigValue] = {}
     # all detected configs with namespaces
     required_config: Dict[str, WritableConfigValue] = {}
 
     # skip sources without spec. those are not imported and most probably are inner functions. also skip the sources that are not called
     # also skip the sources that are called from functions, the parent of call object to the source must be None (no outer function)
-    known_imported_sources = {name: _SOURCES[name] for name in visitor.known_sources
-        if name in _SOURCES and name in visitor.known_source_calls and any(call.parent is None for call in visitor.known_source_calls[name])}  # type: ignore
+    known_imported_sources = {name: _SOURCES[name] for name in visitor.known_sources_resources
+        if name in _SOURCES and name in visitor.known_sources_resources_calls and any(call.parent is None for call in visitor.known_sources_resources_calls[name])}  # type: ignore
 
     for source_name, source_info in known_imported_sources.items():
         source_config = source_info.SPEC()
         spec_fields = source_config.get_resolvable_fields()
         for field_name, field_type in spec_fields.items():
             val_store = None
             # all secrets must go to secrets.toml
@@ -76,43 +95,42 @@
                 # we are sure that all resources come from single file so we can put them in single namespace
                 # namespaces = () if len(known_imported_sources) == 1 else ("sources", source_name)
                 val_store[source_name + ":" + field_name] = WritableConfigValue(field_name, field_type, ())
 
     return required_secrets, required_config
 
 
-def _rewrite_script(script_source: str, transformed_nodes: List[Tuple[ast.Constant, str, str]]) -> str:
-    module_source_lines: List[str] = ast._splitlines_no_ff(script_source)  # type: ignore
+def _rewrite_script(source_script_lines: List[str], transformed_nodes: List[Tuple[ast.AST, ast.AST, str]]) -> str:
     script_lines: List[str] = []
     last_line = -1
     last_offset = -1
     # sort transformed nodes by line and offset
     for node, t_value, _ in sorted(transformed_nodes, key=lambda n: (n[0].lineno, n[0].col_offset)):
         # do we have a line changed
         if last_line != node.lineno - 1:
             # add remainder from the previous line
             if last_offset >= 0:
-                script_lines.append(module_source_lines[last_line][last_offset:])
+                script_lines.append(source_script_lines[last_line][last_offset:])
             # add all new lines from previous line to current
-            script_lines.extend(module_source_lines[last_line+1:node.lineno-1])
+            script_lines.extend(source_script_lines[last_line+1:node.lineno-1])
             # add trailing characters until node in current line starts
-            script_lines.append(module_source_lines[node.lineno-1][:node.col_offset])
+            script_lines.append(source_script_lines[node.lineno-1][:node.col_offset])
         elif last_offset >= 0:
             # no line change, add the characters from the end of previous node to the current
-            script_lines.append(module_source_lines[last_line][last_offset:node.col_offset])
+            script_lines.append(source_script_lines[last_line][last_offset:node.col_offset])
 
         # replace node value
-        script_lines.append(f'"{t_value}"')
+        script_lines.append(unparse(t_value).strip())
         last_line = node.end_lineno - 1
         last_offset = node.end_col_offset
 
     # add all that was missing
     if last_offset >= 0:
-        script_lines.append(module_source_lines[last_line][last_offset:])
-    script_lines.extend(module_source_lines[last_line+1:])
+        script_lines.append(source_script_lines[last_line][last_offset:])
+    script_lines.extend(source_script_lines[last_line+1:])
 
     dest_script = "".join(script_lines)
     # validate by parsing
     ast.parse(source=dest_script)
     return dest_script
 
 
@@ -134,16 +152,16 @@
     clone_storage = utils.clone_command_repo("init", branch)
     # clone_storage = FileStorage("/home/rudolfix/src/python-dlt-init-template")
     command_module = utils.load_command_module(clone_storage.storage_path)
     pipeline_script, template_files = _get_template_files(command_module, use_generic_template)
 
     # get init script variant or the default
     init_script_name = os.path.join("variants", pipeline_name + ".py")
-    if clone_storage.has_file(init_script_name):
-        # use variant
+    is_variant = clone_storage.has_file(init_script_name)
+    if is_variant:
         dest_pipeline_script = pipeline_name + ".py"
         click.echo(f"Using a verified pipeline {fmt.bold(dest_pipeline_script)}")
         if use_generic_template:
             fmt.warning("--generic parameter is meaningless if verified pipeline is used")
     else:
         # use default
         init_script_name = pipeline_script
@@ -172,38 +190,42 @@
     visitor = utils.parse_init_script("init", clone_storage.load(init_script_name), init_script_name)
     if visitor.is_destination_imported:
         raise CliCommandException("init", f"The pipeline script {init_script_name} import a destination from dlt.destinations. You should specify destinations by name when calling dlt.pipeline or dlt.run in init scripts.")
     if n.PIPELINE not in visitor.known_calls:
         raise CliCommandException("init", f"The pipeline script {init_script_name} does not seem to initialize pipeline with dlt.pipeline. Please initialize pipeline explicitly in init scripts.")
 
     # find all arguments in all calls to replace
-    transformed_nodes = _find_argument_nodes_to_replace(
+    transformed_nodes = _find_call_arguments_to_replace(
         visitor,
         [("destination", destination_name), ("pipeline_name", pipeline_name), ("dataset_name", pipeline_name + "_data")],
         init_script_name
     )
 
     # inspect the script
-    script_module = inspect_pipeline_script(clone_storage.storage_path, clone_storage.to_relative_path(init_script_name))
+    inspect_pipeline_script(clone_storage.storage_path, clone_storage.to_relative_path(init_script_name))
 
     if len(_SOURCES) == 0:
         raise CliCommandException("init", f"The pipeline script {init_script_name} is not creating or importing any sources or resources")
 
     for source_q_name, source_config in _SOURCES.items():
-        if source_q_name not in visitor.known_sources:
+        if source_q_name not in visitor.known_sources_resources:
             raise CliCommandException("init", f"The pipeline script {init_script_name} imports a source/resource {source_config.f.__name__} from module {source_config.module.__name__}. In init scripts you must declare all sources and resources in single file.")
 
+    # rename sources and resources
+    if not is_variant:
+        transformed_nodes.extend(_find_source_calls_to_replace(visitor, pipeline_name))
+
     # detect all the required secrets and configs that should go into tomls files
-    required_secrets, required_config = _detect_required_configs(visitor, script_module, init_script_name)
+    required_secrets, required_config = _detect_required_configs(visitor)
     # add destination spec to required secrets
     credentials_type = destination_spec().get_resolvable_fields()["credentials"]
     required_secrets["destinations:" + destination_name] = WritableConfigValue("credentials", credentials_type, ("destination", destination_name))
 
     # modify the script
-    dest_script_source = _rewrite_script(visitor.source, transformed_nodes)
+    dest_script_source = _rewrite_script(visitor.source_lines, transformed_nodes)
 
     # welcome message
     click.echo()
     click.echo("Your new pipeline %s is ready to be customized!" % fmt.bold(pipeline_name))
     click.echo("* Review and change how dlt loads your data in %s" % fmt.bold(dest_pipeline_script))
     click.echo("* Add credentials to %s and other secrets in %s" % (fmt.bold(destination_name), fmt.bold(toml_files[1])))
     click.echo("* Configure your pipeline in %s" % fmt.bold(toml_files[0]))
```

### Comparing `python_dlt-0.2.0a8/dlt/cli/utils.py` & `python_dlt-0.2.0a9/dlt/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 def parse_init_script(command: str, script_source: str, init_script_name: str) -> PipelineScriptVisitor:
     # parse the script first
     tree = ast.parse(source=script_source)
     set_ast_parents(tree)
     visitor = PipelineScriptVisitor(script_source)
-    visitor.visit(tree)
+    visitor.visit_passes(tree)
     if len(visitor.mod_aliases) == 0:
         raise CliCommandException(command, f"The pipeline script {init_script_name} does not import dlt and does not seem to run any pipelines")
 
     return visitor
 
 
 def ensure_git_command(command: str) -> None:
```

### Comparing `python_dlt-0.2.0a8/dlt/common/arithmetics.py` & `python_dlt-0.2.0a9/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/accessors.py` & `python_dlt-0.2.0a9/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/container.py` & `python_dlt-0.2.0a9/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/exceptions.py` & `python_dlt-0.2.0a9/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/inject.py` & `python_dlt-0.2.0a9/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/providers/context.py` & `python_dlt-0.2.0a9/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/providers/dictionary.py` & `python_dlt-0.2.0a9/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/providers/environ.py` & `python_dlt-0.2.0a9/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/providers/provider.py` & `python_dlt-0.2.0a9/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/providers/toml.py` & `python_dlt-0.2.0a9/dlt/common/configuration/providers/toml.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/resolve.py` & `python_dlt-0.2.0a9/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/specs/__init__.py` & `python_dlt-0.2.0a9/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/specs/base_configuration.py` & `python_dlt-0.2.0a9/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/specs/config_providers_context.py` & `python_dlt-0.2.0a9/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/specs/exceptions.py` & `python_dlt-0.2.0a9/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/specs/gcp_client_credentials.py` & `python_dlt-0.2.0a9/dlt/common/configuration/specs/gcp_client_credentials.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/specs/load_volume_configuration.py` & `python_dlt-0.2.0a9/dlt/common/configuration/specs/load_volume_configuration.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/specs/pool_runner_configuration.py` & `python_dlt-0.2.0a9/dlt/common/configuration/specs/pool_runner_configuration.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/specs/postgres_credentials.py` & `python_dlt-0.2.0a9/dlt/common/configuration/specs/postgres_credentials.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/specs/run_configuration.py` & `python_dlt-0.2.0a9/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/specs/schema_volume_configuration.py` & `python_dlt-0.2.0a9/dlt/common/configuration/specs/schema_volume_configuration.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/configuration/utils.py` & `python_dlt-0.2.0a9/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/data_writers/buffered.py` & `python_dlt-0.2.0a9/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/data_writers/escape.py` & `python_dlt-0.2.0a9/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/data_writers/exceptions.py` & `python_dlt-0.2.0a9/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/data_writers/writers.py` & `python_dlt-0.2.0a9/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/destination.py` & `python_dlt-0.2.0a9/dlt/common/destination.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/exceptions.py` & `python_dlt-0.2.0a9/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/git.py` & `python_dlt-0.2.0a9/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/json.py` & `python_dlt-0.2.0a9/dlt/common/json.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/logger.py` & `python_dlt-0.2.0a9/dlt/common/logger.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/normalizers/json/__init__.py` & `python_dlt-0.2.0a9/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/normalizers/json/relational.py` & `python_dlt-0.2.0a9/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/normalizers/names/snake_case.py` & `python_dlt-0.2.0a9/dlt/common/normalizers/names/snake_case.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/pipeline.py` & `python_dlt-0.2.0a9/dlt/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/reflection/spec.py` & `python_dlt-0.2.0a9/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/reflection/utils.py` & `python_dlt-0.2.0a9/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/runners/init.py` & `python_dlt-0.2.0a9/dlt/common/runners/init.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/runners/pool_runner.py` & `python_dlt-0.2.0a9/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/runners/runnable.py` & `python_dlt-0.2.0a9/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/runners/stdout.py` & `python_dlt-0.2.0a9/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/runners/venv.py` & `python_dlt-0.2.0a9/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/schema/configuration.py` & `python_dlt-0.2.0a9/dlt/common/schema/configuration.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/schema/detections.py` & `python_dlt-0.2.0a9/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/schema/exceptions.py` & `python_dlt-0.2.0a9/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/schema/schema.py` & `python_dlt-0.2.0a9/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/schema/typing.py` & `python_dlt-0.2.0a9/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/schema/utils.py` & `python_dlt-0.2.0a9/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/signals.py` & `python_dlt-0.2.0a9/dlt/common/signals.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/storages/data_item_storage.py` & `python_dlt-0.2.0a9/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/storages/exceptions.py` & `python_dlt-0.2.0a9/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/storages/file_storage.py` & `python_dlt-0.2.0a9/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/storages/live_schema_storage.py` & `python_dlt-0.2.0a9/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/storages/load_storage.py` & `python_dlt-0.2.0a9/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/storages/normalize_storage.py` & `python_dlt-0.2.0a9/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/storages/schema_storage.py` & `python_dlt-0.2.0a9/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/storages/versioned_storage.py` & `python_dlt-0.2.0a9/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/telemetry.py` & `python_dlt-0.2.0a9/dlt/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/time.py` & `python_dlt-0.2.0a9/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/typing.py` & `python_dlt-0.2.0a9/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/utils.py` & `python_dlt-0.2.0a9/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/validation.py` & `python_dlt-0.2.0a9/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/common/wei.py` & `python_dlt-0.2.0a9/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/dbt_runner/README.md` & `python_dlt-0.2.0a9/dlt/dbt_runner/README.md`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/dbt_runner/configuration.py` & `python_dlt-0.2.0a9/dlt/dbt_runner/configuration.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/dbt_runner/runner.py` & `python_dlt-0.2.0a9/dlt/dbt_runner/runner.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/dbt_runner/utils.py` & `python_dlt-0.2.0a9/dlt/dbt_runner/utils.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/destinations/bigquery/__init__.py` & `python_dlt-0.2.0a9/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/destinations/bigquery/bigquery.py` & `python_dlt-0.2.0a9/dlt/destinations/bigquery/bigquery.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/destinations/bigquery/sql_client.py` & `python_dlt-0.2.0a9/dlt/destinations/bigquery/sql_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from google.cloud.bigquery.dbapi import exceptions as dbapi_exceptions
 from google.api_core import exceptions as api_core_exceptions
 
 from dlt.common import logger
 from dlt.common.configuration.specs import GcpClientCredentials
 
 from dlt.destinations.typing import DBCursor
-from dlt.destinations.sql_client import SqlClientBase, raise_database_error
+from dlt.destinations.sql_client import SqlClientBase, raise_database_error, raise_open_connection_error
 
 # terminal reasons as returned in BQ gRPC error response
 # https://cloud.google.com/bigquery/docs/error-messages
 BQ_TERMINAL_REASONS = ["billingTierLimitExceeded", "duplicate", "invalid", "notFound", "notImplemented", "stopped", "tableUnavailable"]
 # invalidQuery is an transient error -> must be fixed by programmer
 
 
@@ -26,14 +26,15 @@
         self._client: bigquery.Client = None
         self.credentials: GcpClientCredentials = credentials
         super().__init__(dataset_name)
 
         self.default_retry = bigquery.DEFAULT_RETRY.with_deadline(credentials.retry_deadline)
         self.default_query = bigquery.QueryJobConfig(default_dataset=self.fully_qualified_dataset_name())
 
+    @raise_open_connection_error
     def open_connection(self) -> None:
         self._client = bigquery.Client(
             self.credentials.project_id,
             credentials=self.credentials.to_service_account_credentials(),
             location=self.credentials.location
         )
 
@@ -80,15 +81,14 @@
             self.fully_qualified_dataset_name(),
             not_found_ok=True,
             delete_contents=True,
             retry=self.default_retry,
             timeout=self.credentials.http_timeout
         )
 
-    # @raise_database_error
     def execute_sql(self, sql: AnyStr, *args: Any, **kwargs: Any) -> Optional[Sequence[Sequence[Any]]]:
         with self.execute_query(sql, *args, **kwargs) as curr:
             if not curr.description:
                 return None
             else:
                 try:
                     f = curr.fetchall()
```

### Comparing `python_dlt-0.2.0a8/dlt/destinations/dummy/__init__.py` & `python_dlt-0.2.0a9/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/destinations/dummy/configuration.py` & `python_dlt-0.2.0a9/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/destinations/dummy/dummy.py` & `python_dlt-0.2.0a9/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/destinations/exceptions.py` & `python_dlt-0.2.0a9/dlt/destinations/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,18 +27,26 @@
 
 
 class DatabaseTransientException(DestinationTransientException, DatabaseException):
     def __init__(self, dbapi_exception: Exception) -> None:
         super().__init__(dbapi_exception)
 
 
-class LoadClientNoConnection(DestinationTransientException):
-    def __init__(self, client_type: str) -> None:
+class DestinationConnectionError(DestinationTransientException):
+    def __init__(self, client_type: str, dataset_name: str, reason: str, inner_exc: Exception) -> None:
         self.client_type = client_type
-        super().__init__(f"Connection in sql client {client_type} is closed. Open the connection with 'client.open_connection' or with the 'with client:' statement")
+        self.dataset_name = dataset_name
+        self.inner_exc = inner_exc
+        super().__init__(f"Connection with {client_type} to dataset name {dataset_name} failed. Please check if you configured the credentials at all and provided the right credentials values. You can be also denied access or your internet connection may be down. The actual reason given is: {reason}")
+
+class LoadClientNotConnected(DestinationTransientException):
+    def __init__(self, client_type: str, dataset_name: str) -> None:
+        self.client_type = client_type
+        self.dataset_name = dataset_name
+        super().__init__(f"Connection with {client_type} to dataset {dataset_name} is closed. Open the connection with 'client.open_connection' or with the 'with client:' statement")
 
 
 class DestinationSchemaWillNotUpdate(DestinationTerminalException):
     def __init__(self, table_name: str, columns: Sequence[str], msg: str) -> None:
         self.table_name = table_name
         self.columns = columns
         super().__init__(f"Schema for table {table_name} column(s) {columns} will not update: {msg}")
```

### Comparing `python_dlt-0.2.0a8/dlt/destinations/job_client_impl.py` & `python_dlt-0.2.0a9/dlt/destinations/job_client_impl.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/destinations/postgres/__init__.py` & `python_dlt-0.2.0a9/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/destinations/postgres/postgres.py` & `python_dlt-0.2.0a9/dlt/destinations/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/destinations/postgres/sql_client.py` & `python_dlt-0.2.0a9/dlt/destinations/postgres/sql_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from contextlib import contextmanager
 from typing import Any, AnyStr, Iterator, Optional, Sequence
 
 from dlt.common.configuration.specs import PostgresCredentials
 
 from dlt.destinations.exceptions import DatabaseTerminalException, DatabaseTransientException, DatabaseUndefinedRelation
 from dlt.destinations.typing import DBCursor
-from dlt.destinations.sql_client import SqlClientBase, raise_database_error
+from dlt.destinations.sql_client import SqlClientBase, raise_database_error, raise_open_connection_error
 
 
 class Psycopg2SqlClient(SqlClientBase["psycopg2.connection"]):
 
     def __init__(self, dataset_name: str, credentials: PostgresCredentials) -> None:
         super().__init__(dataset_name)
         self._conn: psycopg2.connection = None
@@ -28,14 +28,15 @@
         self._conn = psycopg2.connect(
                              dsn=self.credentials.to_native_representation(),
                              options=f"-c search_path={self.fully_qualified_dataset_name()},public"
                              )
         # we'll provide explicit transactions see _reset
         self._reset_connection()
 
+    @raise_open_connection_error
     def close_connection(self) -> None:
         if self._conn:
             self._conn.close()
             self._conn = None
 
     @property
     def native_connection(self) -> "psycopg2.connection":
```

### Comparing `python_dlt-0.2.0a8/dlt/destinations/redshift/README.md` & `python_dlt-0.2.0a9/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/destinations/redshift/__init__.py` & `python_dlt-0.2.0a9/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/destinations/redshift/redshift.py` & `python_dlt-0.2.0a9/dlt/destinations/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/destinations/sql_client.py` & `python_dlt-0.2.0a9/dlt/destinations/sql_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from functools import wraps
 import inspect
 from types import TracebackType
 from typing import Any, ContextManager, Generic, Iterator, Optional, Sequence, Type, AnyStr
 from dlt.common.typing import TFun
-from dlt.destinations.exceptions import LoadClientNoConnection
+from dlt.destinations.exceptions import DestinationConnectionError, LoadClientNotConnected
 
 from dlt.destinations.typing import TNativeConn, DBCursor
 
 
 class SqlClientBase(ABC, Generic[TNativeConn]):
     def __init__(self, dataset_name: str) -> None:
         if not dataset_name:
@@ -71,15 +71,15 @@
             yield self
         finally:
             # restore previous dataset name
             self.dataset_name = current_dataset_name
 
     def _ensure_native_conn(self) -> None:
         if not self.native_connection:
-            raise LoadClientNoConnection(type(self).__name__ + ":" + self.dataset_name)
+            raise LoadClientNotConnected(type(self).__name__ , self.dataset_name)
 
     @staticmethod
     @abstractmethod
     def _make_database_exception(ex: Exception) -> Exception:
         pass
 
     @staticmethod
@@ -107,7 +107,19 @@
         except Exception as ex:
             raise self._make_database_exception(ex)
 
     if inspect.isgeneratorfunction(f):
         return _wrap_gen  # type: ignore
     else:
         return _wrap  # type: ignore
+
+
+def raise_open_connection_error(f: TFun) -> TFun:
+
+    @wraps(f)
+    def _wrap(self: SqlClientBase[Any], *args: Any, **kwargs: Any) -> Any:
+        try:
+            return f(self, *args, **kwargs)
+        except Exception as ex:
+            raise DestinationConnectionError(type(self).__name__, self.dataset_name, str(ex), ex)
+
+    return _wrap  # type: ignore
```

### Comparing `python_dlt-0.2.0a8/dlt/destinations/typing.py` & `python_dlt-0.2.0a9/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/extract/decorators.py` & `python_dlt-0.2.0a9/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/extract/exceptions.py` & `python_dlt-0.2.0a9/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/extract/extract.py` & `python_dlt-0.2.0a9/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/extract/pipe.py` & `python_dlt-0.2.0a9/dlt/extract/pipe.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/extract/source.py` & `python_dlt-0.2.0a9/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/extract/typing.py` & `python_dlt-0.2.0a9/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/helpers/pandas.py` & `python_dlt-0.2.0a9/dlt/helpers/pandas.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/helpers/streamlit.py` & `python_dlt-0.2.0a9/dlt/helpers/streamlit.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/load/configuration.py` & `python_dlt-0.2.0a9/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/load/exceptions.py` & `python_dlt-0.2.0a9/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/load/load.py` & `python_dlt-0.2.0a9/dlt/load/load.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/normalize/configuration.py` & `python_dlt-0.2.0a9/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/normalize/normalize.py` & `python_dlt-0.2.0a9/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/pipeline/README.md` & `python_dlt-0.2.0a9/dlt/pipeline/README.md`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/pipeline/__init__.py` & `python_dlt-0.2.0a9/dlt/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/pipeline/configuration.py` & `python_dlt-0.2.0a9/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/pipeline/exceptions.py` & `python_dlt-0.2.0a9/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/pipeline/pipeline.py` & `python_dlt-0.2.0a9/dlt/pipeline/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     STATE_FILE: ClassVar[str] = "state.json"
     STATE_PROPS: ClassVar[List[str]] = list(get_type_hints(TPipelineState).keys())
     LOCAL_STATE_PROPS: ClassVar[List[str]] = list(get_type_hints(TPipelineLocalState).keys())
 
     pipeline_name: str
     default_schema_name: str = None
     schema_names: List[str] = []
-    first_run: bool = None
+    first_run: bool = False
     """Indicates a first run of the pipeline, where run ends with successful loading of data"""
     full_refresh: bool
     must_attach_to_local_pipeline: bool
     pipelines_dir: str
     working_dir: str
     destination: DestinationReference = None
     dataset_name: str = None
```

### Comparing `python_dlt-0.2.0a8/dlt/pipeline/state.py` & `python_dlt-0.2.0a9/dlt/pipeline/state.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/pipeline/trace.py` & `python_dlt-0.2.0a9/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/reflection/names.py` & `python_dlt-0.2.0a9/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/dlt/reflection/script_inspector.py` & `python_dlt-0.2.0a9/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/.dlt/example.secrets.toml` & `python_dlt-0.2.0a9/examples/.dlt/example.secrets.toml`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/README.md` & `python_dlt-0.2.0a9/examples/README.md`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/_helpers.py` & `python_dlt-0.2.0a9/examples/_helpers.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/chess/chess.py` & `python_dlt-0.2.0a9/examples/chess/chess.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/data/channels.json` & `python_dlt-0.2.0a9/examples/data/channels.json`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/data/demo_example.json` & `python_dlt-0.2.0a9/examples/data/demo_example.json`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/data/messages.json` & `python_dlt-0.2.0a9/examples/data/messages.json`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/data/rasa_trackers/2888158124550630_tracker.jsonl` & `python_dlt-0.2.0a9/examples/data/rasa_trackers/2888158124550630_tracker.jsonl`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/data/rasa_trackers/8629c904-0c26-4f0b-927b-14d48db43c28_tracker.jsonl` & `python_dlt-0.2.0a9/examples/data/rasa_trackers/8629c904-0c26-4f0b-927b-14d48db43c28_tracker.jsonl`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/data/singer_taps/csv_catalog.json` & `python_dlt-0.2.0a9/examples/data/singer_taps/csv_catalog.json`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/data/singer_taps/tap_google_sheet.jsonl` & `python_dlt-0.2.0a9/examples/data/singer_taps/tap_google_sheet.jsonl`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/data/singer_taps/tap_hubspot.jsonl` & `python_dlt-0.2.0a9/examples/data/singer_taps/tap_hubspot.jsonl`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/demo_example.py` & `python_dlt-0.2.0a9/examples/demo_example.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/discord_iterator.py` & `python_dlt-0.2.0a9/examples/discord_iterator.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/google_drive_csv.py` & `python_dlt-0.2.0a9/examples/google_drive_csv.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/quickstart.py` & `python_dlt-0.2.0a9/examples/quickstart.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/rasa_example.py` & `python_dlt-0.2.0a9/examples/rasa_example.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/read_table.py` & `python_dlt-0.2.0a9/examples/read_table.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/restore_pipeline.py` & `python_dlt-0.2.0a9/examples/restore_pipeline.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/schemas/discord.schema.yml` & `python_dlt-0.2.0a9/examples/schemas/discord.schema.yml`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/schemas/dlt_quickstart.schema.yaml` & `python_dlt-0.2.0a9/examples/schemas/dlt_quickstart.schema.yaml`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/schemas/hubspot.schema.yaml` & `python_dlt-0.2.0a9/examples/schemas/hubspot.schema.yaml`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/schemas/inferred_demo.schema.yml` & `python_dlt-0.2.0a9/examples/schemas/inferred_demo.schema.yml`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/singer_tap_example.py` & `python_dlt-0.2.0a9/examples/singer_tap_example.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/singer_tap_jsonl_example.py` & `python_dlt-0.2.0a9/examples/singer_tap_jsonl_example.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/sources/google_sheets.py` & `python_dlt-0.2.0a9/examples/sources/google_sheets.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/sources/jsonl.py` & `python_dlt-0.2.0a9/examples/sources/jsonl.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/sources/rasa/rasa.py` & `python_dlt-0.2.0a9/examples/sources/rasa/rasa.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/sources/rasa/rasa.schema.yaml` & `python_dlt-0.2.0a9/examples/sources/rasa/rasa.schema.yaml`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/sources/singer_tap.py` & `python_dlt-0.2.0a9/examples/sources/singer_tap.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/sources/sql_query.py` & `python_dlt-0.2.0a9/examples/sources/sql_query.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/sources/stdout.py` & `python_dlt-0.2.0a9/examples/sources/stdout.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/examples/sync_schema_example.py` & `python_dlt-0.2.0a9/examples/sync_schema_example.py`

 * *Files identical despite different names*

### Comparing `python_dlt-0.2.0a8/pyproject.toml` & `python_dlt-0.2.0a9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-dlt"
-version = "0.2.0a8"
+version = "0.2.0a9"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>",]
 readme = "QUICKSTART.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
```

### Comparing `python_dlt-0.2.0a8/setup.py` & `python_dlt-0.2.0a9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
  'redshift:platform_python_implementation == "PyPy"': ['psycopg2cffi>=2.9.0,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:main']}
 
 setup_kwargs = {
     'name': 'python-dlt',
-    'version': '0.2.0a8',
+    'version': '0.2.0a9',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
     'long_description': '# Quickstart Guide: Data Load Tool (DLT)\n\n## **TL;DR: This guide shows you how to load a JSON document into Google BigQuery using DLT.**\n\n![](docs/DLT-Pacman-Big.gif)\n\n*Please open a pull request [here](https://github.com/scale-vector/dlt/edit/master/QUICKSTART.md) if there is something you can improve about this quickstart.*\n\n## Grab the demo\n\nClone the example repository:\n```\ngit clone https://github.com/scale-vector/dlt-quickstart-example.git\n```\n\nEnter the directory:\n```\ncd dlt-quickstart-example\n```\n\nOpen the files in your favorite IDE / text editor:\n- `data.json` (i.e. the JSON document you will load)\n- `credentials.json` (i.e. contains the credentials to our demo Google BigQuery warehouse)\n- `quickstart.py` (i.e. the script that uses DLT)\n\n## Set up a virtual environment\n\nEnsure you are using either Python 3.8 or 3.9:\n```\npython3 --version\n```\n\nCreate a new virtual environment:\n```\npython3 -m venv ./env\n```\n\nActivate the virtual environment:\n```\nsource ./env/bin/activate\n```\n\n## Install DLT and support for the target data warehouse\n\nInstall DLT using pip:\n```\npip3 install -U python-dlt\n```\n\nInstall support for Google BigQuery:\n```\npip3 install -U python-dlt[gcp]\n```\n\n## Understanding the code\n\n1. Configure DLT\n\n2. Create a DLT pipeline\n\n3. Load the data from the JSON document\n\n4. Pass the data to the DLT pipeline\n\n5. Use DLT to load the data\n\n## Running the code\n\nRun the quickstart script in `/examples` folder:\n\n```\npython3 quickstart.py\n```\n\nInspect `schema.yml` that has been printed by the script or the generated file:\n```\nvim schema.yml\n```\n\nSee results of querying the Google BigQuery table:\n\n`json_doc` table\n\n```\nSELECT * FROM `{schema_prefix}_example.json_doc`\n```\n```\n{  "name": "Ana",  "age": "30",  "id": "456",  "_dlt_load_id": "1654787700.406905",  "_dlt_id": "5b018c1ba3364279a0ca1a231fbd8d90"}\n{  "name": "Bob",  "age": "30",  "id": "455",  "_dlt_load_id": "1654787700.406905",  "_dlt_id": "afc8506472a14a529bf3e6ebba3e0a9e"}\n```\n\n`json_doc__children` table\n\n```\nSELECT * FROM `{schema_prefix}_example.json_doc__children` LIMIT 1000\n```\n```\n    # {"name": "Bill", "id": "625", "_dlt_parent_id": "5b018c1ba3364279a0ca1a231fbd8d90", "_dlt_list_idx": "0", "_dlt_root_id": "5b018c1ba3364279a0ca1a231fbd8d90",\n    #   "_dlt_id": "7993452627a98814cc7091f2c51faf5c"}\n    # {"name": "Bill", "id": "625", "_dlt_parent_id": "afc8506472a14a529bf3e6ebba3e0a9e", "_dlt_list_idx": "0", "_dlt_root_id": "afc8506472a14a529bf3e6ebba3e0a9e",\n    #   "_dlt_id": "9a2fd144227e70e3aa09467e2358f934"}\n    # {"name": "Dave", "id": "621", "_dlt_parent_id": "afc8506472a14a529bf3e6ebba3e0a9e", "_dlt_list_idx": "1", "_dlt_root_id": "afc8506472a14a529bf3e6ebba3e0a9e",\n    #   "_dlt_id": "28002ed6792470ea8caf2d6b6393b4f9"}\n    # {"name": "Elli", "id": "591", "_dlt_parent_id": "5b018c1ba3364279a0ca1a231fbd8d90", "_dlt_list_idx": "1", "_dlt_root_id": "5b018c1ba3364279a0ca1a231fbd8d90",\n    #   "_dlt_id": "d18172353fba1a492c739a7789a786cf"}\n```\n\nJoining the two tables above on autogenerated keys (i.e. `p._record_hash = c._parent_hash`)\n\n```\nselect p.name, p.age, p.id as parent_id,\n            c.name as child_name, c.id as child_id, c._dlt_list_idx as child_order_in_list\n        from `{schema_prefix}_example.json_doc` as p\n        left join `{schema_prefix}_example.json_doc__children`  as c\n            on p._dlt_id = c._dlt_parent_id\n```\n```\n    # {  "name": "Ana",  "age": "30",  "parent_id": "456",  "child_name": "Bill",  "child_id": "625",  "child_order_in_list": "0"}\n    # {  "name": "Ana",  "age": "30",  "parent_id": "456",  "child_name": "Elli",  "child_id": "591",  "child_order_in_list": "1"}\n    # {  "name": "Bob",  "age": "30",  "parent_id": "455",  "child_name": "Bill",  "child_id": "625",  "child_order_in_list": "0"}\n    # {  "name": "Bob",  "age": "30",  "parent_id": "455",  "child_name": "Dave",  "child_id": "621",  "child_order_in_list": "1"}\n```\n\n## Next steps\n\n1. Replace `data.json` with data you want to explore\n\n2. Check that the inferred types are correct in `schema.yml`\n\n3. Set up your own Google BigQuery warehouse (and replace the credentials)\n\n4. Use this new clean staging layer as the starting point for a semantic layer / analytical model (e.g. using dbt)',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
```

### Comparing `python_dlt-0.2.0a8/PKG-INFO` & `python_dlt-0.2.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dlt
-Version: 0.2.0a8
+Version: 0.2.0a9
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
```

