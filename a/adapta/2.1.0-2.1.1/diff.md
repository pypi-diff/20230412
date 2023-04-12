# Comparing `tmp/adapta-2.1.0.tar.gz` & `tmp/adapta-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapta-2.1.0.tar", max compression
+gzip compressed data, was "adapta-2.1.1.tar", max compression
```

## Comparing `adapta-2.1.0.tar` & `adapta-2.1.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    10693 2023-04-03 15:20:32.551782 adapta-2.1.0/LICENSE
--rw-r--r--   0        0        0      666 2023-04-03 15:20:32.551782 adapta-2.1.0/README.md
--rw-r--r--   0        0        0      663 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/__init__.py
--rw-r--r--   0        0        0       22 2023-04-03 15:20:51.192235 adapta-2.1.0/adapta/_version.py
--rw-r--r--   0        0        0      598 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/connectors/__init__.py
--rw-r--r--   0        0        0      694 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/connectors/service_bus/__init__.py
--rw-r--r--   0        0        0     1914 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/connectors/service_bus/_connector.py
--rw-r--r--   0        0        0     4111 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/logs/README.md
--rw-r--r--   0        0        0      667 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/logs/__init__.py
--rw-r--r--   0        0        0    12390 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/logs/_base.py
--rw-r--r--   0        0        0     2950 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/logs/_internal.py
--rw-r--r--   0        0        0      598 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/logs/handlers/__init__.py
--rw-r--r--   0        0        0     9168 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/logs/handlers/datadog_api_handler.py
--rw-r--r--   0        0        0     2211 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/logs/handlers/safe_stream_handler.py
--rw-r--r--   0        0        0      741 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/logs/models/__init__.py
--rw-r--r--   0        0        0      794 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/logs/models/_log_level.py
--rw-r--r--   0        0        0      963 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/logs/models/_logs_metadata.py
--rw-r--r--   0        0        0      672 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/metrics/__init__.py
--rw-r--r--   0        0        0     3215 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/metrics/_base.py
--rw-r--r--   0        0        0     1930 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/metrics/providers/README.md
--rw-r--r--   0        0        0      598 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/metrics/providers/__init__.py
--rw-r--r--   0        0        0     4466 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/metrics/providers/datadog_provider.py
--rw-r--r--   0        0        0      653 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/ml/__init__.py
--rw-r--r--   0        0        0     1223 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/ml/_model.py
--rw-r--r--   0        0        0      699 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/ml/mlflow/__init__.py
--rw-r--r--   0        0        0     5319 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/ml/mlflow/_client.py
--rw-r--r--   0        0        0     3820 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/ml/mlflow/_functions.py
--rw-r--r--   0        0        0      674 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/process_communication/__init__.py
--rw-r--r--   0        0        0     3362 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/process_communication/_models.py
--rw-r--r--   0        0        0      598 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/security/__init__.py
--rw-r--r--   0        0        0     1303 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/security/clients/__init__.py
--rw-r--r--   0        0        0     7396 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/security/clients/_azure_client.py
--rw-r--r--   0        0        0     2396 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/security/clients/_base.py
--rw-r--r--   0        0        0     1787 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/security/clients/_local_client.py
--rw-r--r--   0        0        0      598 2023-04-03 15:20:32.551782 adapta-2.1.0/adapta/security/clients/hashicorp_vault/__init__.py
--rw-r--r--   0        0        0     2695 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
--rw-r--r--   0        0        0     2601 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/security/clients/hashicorp_vault/kubernetes_client.py
--rw-r--r--   0        0        0     3332 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/security/clients/hashicorp_vault/oidc_client.py
--rw-r--r--   0        0        0      598 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/__init__.py
--rw-r--r--   0        0        0     1208 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/blob/README.md
--rw-r--r--   0        0        0      622 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/blob/__init__.py
--rw-r--r--   0        0        0     9605 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/blob/azure_storage_client.py
--rw-r--r--   0        0        0     4791 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/blob/base.py
--rw-r--r--   0        0        0      665 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/cache/__init__.py
--rw-r--r--   0        0        0     3451 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/cache/_base.py
--rw-r--r--   0        0        0     3365 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/cache/redis_cache.py
--rw-r--r--   0        0        0     2451 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/database/README.md
--rw-r--r--   0        0        0      598 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/database/__init__.py
--rw-r--r--   0        0        0     4691 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/database/azure_sql.py
--rw-r--r--   0        0        0      675 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/database/models/__init__.py
--rw-r--r--   0        0        0     1447 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/database/models/_models.py
--rw-r--r--   0        0        0     7711 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/database/odbc.py
--rw-r--r--   0        0        0     4523 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/database/trino_sql.py
--rw-r--r--   0        0        0     2386 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/delta_lake/README.md
--rw-r--r--   0        0        0      721 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/delta_lake/__init__.py
--rw-r--r--   0        0        0    11493 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/delta_lake/_functions.py
--rw-r--r--   0        0        0     2247 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/delta_lake/_models.py
--rw-r--r--   0        0        0      598 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/models/__init__.py
--rw-r--r--   0        0        0     5302 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/models/azure.py
--rw-r--r--   0        0        0     2063 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/models/base.py
--rw-r--r--   0        0        0     5711 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/models/format.py
--rw-r--r--   0        0        0     6627 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/models/hive.py
--rw-r--r--   0        0        0     1519 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/models/local.py
--rw-r--r--   0        0        0      529 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/secrets/README.md
--rw-r--r--   0        0        0      666 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/secrets/__init__.py
--rw-r--r--   0        0        0     2216 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/secrets/_base.py
--rw-r--r--   0        0        0     2358 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/secrets/azure_secret_client.py
--rw-r--r--   0        0        0     2887 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
--rw-r--r--   0        0        0      668 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/utils/__init__.py
--rw-r--r--   0        0        0     3578 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/utils/_common.py
--rw-r--r--   0        0        0     3815 2023-04-03 15:20:32.555782 adapta-2.1.0/adapta/utils/concurrent_task_runner.py
--rw-r--r--   0        0        0     2185 2023-04-03 15:20:51.192235 adapta-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 adapta-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10693 2023-04-12 11:49:34.504297 adapta-2.1.1/LICENSE
+-rw-r--r--   0        0        0      666 2023-04-12 11:49:34.504297 adapta-2.1.1/README.md
+-rw-r--r--   0        0        0      663 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-12 11:49:54.497748 adapta-2.1.1/adapta/_version.py
+-rw-r--r--   0        0        0      598 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/connectors/__init__.py
+-rw-r--r--   0        0        0      694 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/connectors/service_bus/__init__.py
+-rw-r--r--   0        0        0     1914 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/connectors/service_bus/_connector.py
+-rw-r--r--   0        0        0     4111 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/README.md
+-rw-r--r--   0        0        0      667 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/__init__.py
+-rw-r--r--   0        0        0    12390 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/_base.py
+-rw-r--r--   0        0        0     2950 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/_internal.py
+-rw-r--r--   0        0        0      598 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/handlers/__init__.py
+-rw-r--r--   0        0        0     9168 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/handlers/datadog_api_handler.py
+-rw-r--r--   0        0        0     2211 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/handlers/safe_stream_handler.py
+-rw-r--r--   0        0        0      741 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/models/__init__.py
+-rw-r--r--   0        0        0      794 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/models/_log_level.py
+-rw-r--r--   0        0        0      963 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/models/_logs_metadata.py
+-rw-r--r--   0        0        0      672 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/metrics/__init__.py
+-rw-r--r--   0        0        0     3215 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/metrics/_base.py
+-rw-r--r--   0        0        0     1930 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/metrics/providers/README.md
+-rw-r--r--   0        0        0      598 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/metrics/providers/__init__.py
+-rw-r--r--   0        0        0     4466 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/metrics/providers/datadog_provider.py
+-rw-r--r--   0        0        0      653 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/ml/__init__.py
+-rw-r--r--   0        0        0     1223 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/ml/_model.py
+-rw-r--r--   0        0        0      699 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/ml/mlflow/__init__.py
+-rw-r--r--   0        0        0     5319 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/ml/mlflow/_client.py
+-rw-r--r--   0        0        0     3820 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/ml/mlflow/_functions.py
+-rw-r--r--   0        0        0      674 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/process_communication/__init__.py
+-rw-r--r--   0        0        0     3362 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/process_communication/_models.py
+-rw-r--r--   0        0        0      598 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/security/__init__.py
+-rw-r--r--   0        0        0     1303 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/security/clients/__init__.py
+-rw-r--r--   0        0        0     7396 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/security/clients/_azure_client.py
+-rw-r--r--   0        0        0     2396 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/security/clients/_base.py
+-rw-r--r--   0        0        0     1787 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/security/clients/_local_client.py
+-rw-r--r--   0        0        0      598 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/security/clients/hashicorp_vault/__init__.py
+-rw-r--r--   0        0        0     2695 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
+-rw-r--r--   0        0        0     2601 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/security/clients/hashicorp_vault/kubernetes_client.py
+-rw-r--r--   0        0        0     3454 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/security/clients/hashicorp_vault/oidc_client.py
+-rw-r--r--   0        0        0      598 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/__init__.py
+-rw-r--r--   0        0        0     1208 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/blob/README.md
+-rw-r--r--   0        0        0      622 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/blob/__init__.py
+-rw-r--r--   0        0        0     9605 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/blob/azure_storage_client.py
+-rw-r--r--   0        0        0     4791 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/blob/base.py
+-rw-r--r--   0        0        0      665 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/cache/__init__.py
+-rw-r--r--   0        0        0     3451 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/cache/_base.py
+-rw-r--r--   0        0        0     3365 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/cache/redis_cache.py
+-rw-r--r--   0        0        0     2451 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/README.md
+-rw-r--r--   0        0        0      598 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/__init__.py
+-rw-r--r--   0        0        0     4691 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/azure_sql.py
+-rw-r--r--   0        0        0      675 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/models/__init__.py
+-rw-r--r--   0        0        0     1447 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/models/_models.py
+-rw-r--r--   0        0        0     7711 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/odbc.py
+-rw-r--r--   0        0        0     4523 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/trino_sql.py
+-rw-r--r--   0        0        0     2386 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/delta_lake/README.md
+-rw-r--r--   0        0        0      721 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/delta_lake/__init__.py
+-rw-r--r--   0        0        0    11493 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/delta_lake/_functions.py
+-rw-r--r--   0        0        0     2247 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/delta_lake/_models.py
+-rw-r--r--   0        0        0      598 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/models/__init__.py
+-rw-r--r--   0        0        0     5302 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/models/azure.py
+-rw-r--r--   0        0        0     2063 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/models/base.py
+-rw-r--r--   0        0        0     5711 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/models/format.py
+-rw-r--r--   0        0        0     6627 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/models/hive.py
+-rw-r--r--   0        0        0     1519 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/models/local.py
+-rw-r--r--   0        0        0      529 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/secrets/README.md
+-rw-r--r--   0        0        0      666 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/secrets/__init__.py
+-rw-r--r--   0        0        0     2216 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/secrets/_base.py
+-rw-r--r--   0        0        0     2358 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/secrets/azure_secret_client.py
+-rw-r--r--   0        0        0     2887 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
+-rw-r--r--   0        0        0      668 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/utils/__init__.py
+-rw-r--r--   0        0        0     3578 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/utils/_common.py
+-rw-r--r--   0        0        0     3815 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/utils/concurrent_task_runner.py
+-rw-r--r--   0        0        0     2185 2023-04-12 11:49:54.497748 adapta-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 adapta-2.1.1/PKG-INFO
```

### Comparing `adapta-2.1.0/LICENSE` & `adapta-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/README.md` & `adapta-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/__init__.py` & `adapta-2.1.1/adapta/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/connectors/__init__.py` & `adapta-2.1.1/adapta/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/connectors/service_bus/__init__.py` & `adapta-2.1.1/adapta/connectors/service_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/connectors/service_bus/_connector.py` & `adapta-2.1.1/adapta/connectors/service_bus/_connector.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/logs/README.md` & `adapta-2.1.1/adapta/logs/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/logs/__init__.py` & `adapta-2.1.1/adapta/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/logs/_base.py` & `adapta-2.1.1/adapta/logs/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/logs/_internal.py` & `adapta-2.1.1/adapta/logs/_internal.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/logs/handlers/__init__.py` & `adapta-2.1.1/adapta/logs/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/logs/handlers/datadog_api_handler.py` & `adapta-2.1.1/adapta/logs/handlers/datadog_api_handler.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/logs/handlers/safe_stream_handler.py` & `adapta-2.1.1/adapta/logs/handlers/safe_stream_handler.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/logs/models/__init__.py` & `adapta-2.1.1/adapta/logs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/logs/models/_log_level.py` & `adapta-2.1.1/adapta/logs/models/_log_level.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/logs/models/_logs_metadata.py` & `adapta-2.1.1/adapta/logs/models/_logs_metadata.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/metrics/__init__.py` & `adapta-2.1.1/adapta/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/metrics/_base.py` & `adapta-2.1.1/adapta/metrics/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/metrics/providers/README.md` & `adapta-2.1.1/adapta/metrics/providers/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/metrics/providers/__init__.py` & `adapta-2.1.1/adapta/metrics/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/metrics/providers/datadog_provider.py` & `adapta-2.1.1/adapta/metrics/providers/datadog_provider.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/ml/__init__.py` & `adapta-2.1.1/adapta/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/ml/_model.py` & `adapta-2.1.1/adapta/ml/_model.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/ml/mlflow/__init__.py` & `adapta-2.1.1/adapta/ml/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/ml/mlflow/_client.py` & `adapta-2.1.1/adapta/ml/mlflow/_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/ml/mlflow/_functions.py` & `adapta-2.1.1/adapta/ml/mlflow/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/process_communication/__init__.py` & `adapta-2.1.1/adapta/process_communication/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/process_communication/_models.py` & `adapta-2.1.1/adapta/process_communication/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/security/__init__.py` & `adapta-2.1.1/adapta/security/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/security/clients/__init__.py` & `adapta-2.1.1/adapta/security/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/security/clients/_azure_client.py` & `adapta-2.1.1/adapta/security/clients/_azure_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/security/clients/_base.py` & `adapta-2.1.1/adapta/security/clients/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/security/clients/_local_client.py` & `adapta-2.1.1/adapta/security/clients/_local_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/security/clients/hashicorp_vault/__init__.py` & `adapta-2.1.1/adapta/security/clients/hashicorp_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py` & `adapta-2.1.1/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/security/clients/hashicorp_vault/kubernetes_client.py` & `adapta-2.1.1/adapta/security/clients/hashicorp_vault/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/security/clients/hashicorp_vault/oidc_client.py` & `adapta-2.1.1/adapta/security/clients/hashicorp_vault/oidc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,20 @@
         def do_GET(self):  # pylint: disable=C0103
             """Handles GET request and collects token"""
 
             params = parse.parse_qs(self.path.split("?")[1])
             self.server.token = params["code"][0]
             self.send_response(200)
             self.end_headers()
-            self.wfile.write(str.encode("<div>Authentication successful, you can close the browser now.</div>"))
+            self.wfile.write(
+                str.encode(
+                    "<script>window.close()</script><div>Authentication successful,"
+                    " you can close the browser now.</div>"
+                )
+            )
 
     server_address = ("127.0.0.1", 8250)
     httpd = HttpServ(server_address, AuthHandler)
     httpd.handle_request()
     return httpd.token
```

### Comparing `adapta-2.1.0/adapta/storage/__init__.py` & `adapta-2.1.1/adapta/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/blob/README.md` & `adapta-2.1.1/adapta/storage/blob/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/blob/__init__.py` & `adapta-2.1.1/adapta/storage/blob/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/blob/azure_storage_client.py` & `adapta-2.1.1/adapta/storage/blob/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/blob/base.py` & `adapta-2.1.1/adapta/storage/blob/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/cache/__init__.py` & `adapta-2.1.1/adapta/storage/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/cache/_base.py` & `adapta-2.1.1/adapta/storage/cache/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/cache/redis_cache.py` & `adapta-2.1.1/adapta/storage/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/database/README.md` & `adapta-2.1.1/adapta/storage/database/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/database/__init__.py` & `adapta-2.1.1/adapta/storage/database/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/database/azure_sql.py` & `adapta-2.1.1/adapta/storage/database/azure_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/database/models/__init__.py` & `adapta-2.1.1/adapta/storage/database/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/database/models/_models.py` & `adapta-2.1.1/adapta/storage/database/models/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/database/odbc.py` & `adapta-2.1.1/adapta/storage/database/odbc.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/database/trino_sql.py` & `adapta-2.1.1/adapta/storage/database/trino_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/delta_lake/README.md` & `adapta-2.1.1/adapta/storage/delta_lake/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/delta_lake/__init__.py` & `adapta-2.1.1/adapta/storage/delta_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/delta_lake/_functions.py` & `adapta-2.1.1/adapta/storage/delta_lake/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/delta_lake/_models.py` & `adapta-2.1.1/adapta/storage/delta_lake/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/models/__init__.py` & `adapta-2.1.1/adapta/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/models/azure.py` & `adapta-2.1.1/adapta/storage/models/azure.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/models/base.py` & `adapta-2.1.1/adapta/storage/models/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/models/format.py` & `adapta-2.1.1/adapta/storage/models/format.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/models/hive.py` & `adapta-2.1.1/adapta/storage/models/hive.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/models/local.py` & `adapta-2.1.1/adapta/storage/models/local.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/secrets/README.md` & `adapta-2.1.1/adapta/storage/secrets/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/secrets/__init__.py` & `adapta-2.1.1/adapta/storage/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/secrets/_base.py` & `adapta-2.1.1/adapta/storage/secrets/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/secrets/azure_secret_client.py` & `adapta-2.1.1/adapta/storage/secrets/azure_secret_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py` & `adapta-2.1.1/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/utils/__init__.py` & `adapta-2.1.1/adapta/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/utils/_common.py` & `adapta-2.1.1/adapta/utils/_common.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/adapta/utils/concurrent_task_runner.py` & `adapta-2.1.1/adapta/utils/concurrent_task_runner.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.0/pyproject.toml` & `adapta-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adapta"
-version = "2.1.0"
+version = "2.1.1"
 description = "Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier."
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>']
 license = 'Apache 2.0'
 readme = "README.md"
 repository = 'https://github.com/SneaksAndData/adapta'
```

### Comparing `adapta-2.1.0/PKG-INFO` & `adapta-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapta
-Version: 2.1.0
+Version: 2.1.1
 Summary: Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier.
 Home-page: https://github.com/SneaksAndData/adapta
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

