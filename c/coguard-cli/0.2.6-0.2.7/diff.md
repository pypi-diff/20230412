# Comparing `tmp/coguard-cli-0.2.6.tar.gz` & `tmp/coguard-cli-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coguard-cli-0.2.6.tar", last modified: Fri Mar 31 15:08:51 2023, max compression
+gzip compressed data, was "coguard-cli-0.2.7.tar", last modified: Wed Apr 12 16:13:13 2023, max compression
```

## Comparing `coguard-cli-0.2.6.tar` & `coguard-cli-0.2.7.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.360187 coguard-cli-0.2.6/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1071 2022-06-21 06:40:28.000000 coguard-cli-0.2.6/LICENSE
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9303 2023-03-31 15:08:51.360187 coguard-cli-0.2.6/PKG-INFO
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8931 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/README.md
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8748 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/README_PYPI.md
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)       84 2022-06-21 06:40:28.000000 coguard-cli-0.2.6/pyproject.toml
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      980 2023-03-31 15:08:51.360187 coguard-cli-0.2.6/setup.cfg
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.346853 coguard-cli-0.2.6/src/
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.350187 coguard-cli-0.2.6/src/coguard_cli/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    22785 2023-03-30 03:21:13.000000 coguard-cli-0.2.6/src/coguard_cli/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6592 2023-03-30 03:21:13.000000 coguard-cli-0.2.6/src/coguard_cli/__main__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7702 2023-02-01 14:06:40.000000 coguard-cli-0.2.6/src/coguard_cli/api_connection.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.353520 coguard-cli-0.2.6/src/coguard_cli/auth/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8534 2023-02-01 14:06:40.000000 coguard-cli-0.2.6/src/coguard_cli/auth/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1860 2022-07-03 06:44:40.000000 coguard-cli-0.2.6/src/coguard_cli/auth/auth_config.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6313 2023-02-24 03:10:28.000000 coguard-cli-0.2.6/src/coguard_cli/auth/token.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      269 2023-02-01 14:06:40.000000 coguard-cli-0.2.6/src/coguard_cli/auth/util.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.353520 coguard-cli-0.2.6/src/coguard_cli/ci_cd/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/ci_cd/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1011 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/ci_cd/ci_cd_provider_abc.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      502 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/ci_cd/ci_cd_provider_factory.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.353520 coguard-cli-0.2.6/src/coguard_cli/ci_cd/ci_cd_providers/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/ci_cd/ci_cd_providers/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2193 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/ci_cd/ci_cd_providers/ci_cd_provider_github.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.346853 coguard-cli-0.2.6/src/coguard_cli/ci_cd/ci_cd_scripts/
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.353520 coguard-cli-0.2.6/src/coguard_cli/ci_cd/ci_cd_scripts/github/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      485 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/ci_cd/ci_cd_scripts/github/github_coguard_action.yml
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.353520 coguard-cli-0.2.6/src/coguard_cli/discovery/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-22 20:18:10.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/__init__.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.353520 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-01 14:06:40.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1431 2023-03-30 03:21:13.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/cloud_provider_abc.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      799 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/cloud_provider_factory.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.353520 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/cloud_providers/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-24 03:43:49.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/cloud_providers/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5713 2023-03-30 03:21:13.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_aws.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2078 2023-03-30 03:21:13.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_azure.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7364 2023-03-30 03:21:13.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.353520 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2716 2023-03-31 15:08:41.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/Dockerfile
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.353520 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/data/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      232 2023-02-01 14:06:40.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/data/versions.tf
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.353520 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4492 2023-03-31 15:08:41.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/cmd_for_dfile
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7608 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finder_abc.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2518 2023-02-01 14:06:40.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finder_factory.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.356854 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    25095 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6096 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_apache.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4258 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_docker_compose.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4176 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_dockerfile.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3668 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_elasticsearch.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6197 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_helm.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3615 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_kafka.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6035 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_kerberos.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3490 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_kubernetes.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5011 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_mongodb.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7401 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_mysql.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7047 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_netlify.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5979 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_nginx.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8137 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_open_telemetry_collector.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9482 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_postgres.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9241 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_redis.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3849 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_terraform.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11379 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_tomcat.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11573 2023-03-31 15:08:41.000000 coguard-cli-0.2.6/src/coguard_cli/docker_dao.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.356854 coguard-cli-0.2.6/src/coguard_cli/folder_scan/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9227 2023-02-19 03:22:05.000000 coguard-cli-0.2.6/src/coguard_cli/folder_scan/__init__.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.356854 coguard-cli-0.2.6/src/coguard_cli/image_check/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8557 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/image_check/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      239 2022-06-21 06:45:38.000000 coguard-cli-0.2.6/src/coguard_cli/print_colors.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.356854 coguard-cli-0.2.6/src/coguard_cli/tests/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.6/src/coguard_cli/tests/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13023 2023-02-01 14:06:40.000000 coguard-cli-0.2.6/src/coguard_cli/tests/api_connection_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.356854 coguard-cli-0.2.6/src/coguard_cli/tests/auth/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.6/src/coguard_cli/tests/auth/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      675 2022-06-21 06:45:38.000000 coguard-cli-0.2.6/src/coguard_cli/tests/auth/auth_config_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4927 2023-02-01 14:06:40.000000 coguard-cli-0.2.6/src/coguard_cli/tests/auth/common_auth_function_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8441 2023-02-01 14:06:40.000000 coguard-cli-0.2.6/src/coguard_cli/tests/auth/token_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.356854 coguard-cli-0.2.6/src/coguard_cli/tests/ci_cd/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/tests/ci_cd/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      595 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/tests/ci_cd/ci_cd_provider_factory_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.356854 coguard-cli-0.2.6/src/coguard_cli/tests/ci_cd/ci_cd_providers/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/tests/ci_cd/ci_cd_providers/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2099 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/tests/ci_cd/ci_cd_providers/ci_cd_provider_github_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11605 2023-02-24 03:10:28.000000 coguard-cli-0.2.6/src/coguard_cli/tests/common_functions_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.356854 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-25 15:30:38.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/__init__.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.356854 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/cloud_discovery/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-02 14:16:57.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/cloud_discovery/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      640 2023-02-02 14:16:57.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/cloud_discovery/cloud_provider_factory_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.356854 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-02 14:16:57.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8905 2023-02-02 14:16:57.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_aws_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4269 2023-02-02 14:16:57.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_azure_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11454 2023-03-30 03:21:13.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3339 2023-01-25 15:30:38.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finder_abc_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      637 2023-01-25 15:30:38.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finder_factory_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.360187 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-25 15:30:38.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13736 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/common_functions_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6934 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_apache_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6597 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_docker_compose_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5465 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_dockerfile_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5865 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_elasticsearch_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5736 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_helm_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5634 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kafka_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7029 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kerberos_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5883 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kubernetes_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6248 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mongodb_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6932 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mysql_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6899 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_nginx_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6005 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_opentelemetry_collector_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8168 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_postgres_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7506 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_redis_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5657 2023-02-14 11:54:29.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_terraform_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9100 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_tomcat_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.360187 coguard-cli-0.2.6/src/coguard_cli/tests/folder_scan/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-23 19:31:49.000000 coguard-cli-0.2.6/src/coguard_cli/tests/folder_scan/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13956 2023-02-19 03:22:05.000000 coguard-cli-0.2.6/src/coguard_cli/tests/folder_scan/common_functions_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.360187 coguard-cli-0.2.6/src/coguard_cli/tests/image_check/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.6/src/coguard_cli/tests/image_check/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    10470 2023-02-24 03:10:28.000000 coguard-cli-0.2.6/src/coguard_cli/tests/image_check/common_functions_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13136 2023-02-01 14:06:40.000000 coguard-cli-0.2.6/src/coguard_cli/tests/image_check/docker_dao_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6243 2023-02-23 02:56:51.000000 coguard-cli-0.2.6/src/coguard_cli/tests/util_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5506 2023-03-05 05:26:44.000000 coguard-cli-0.2.6/src/coguard_cli/util.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-03-31 15:08:51.350187 coguard-cli-0.2.6/src/coguard_cli.egg-info/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9303 2023-03-31 15:08:51.000000 coguard-cli-0.2.6/src/coguard_cli.egg-info/PKG-INFO
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6340 2023-03-31 15:08:51.000000 coguard-cli-0.2.6/src/coguard_cli.egg-info/SOURCES.txt
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        1 2023-03-31 15:08:51.000000 coguard-cli-0.2.6/src/coguard_cli.egg-info/dependency_links.txt
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)       54 2023-03-31 15:08:51.000000 coguard-cli-0.2.6/src/coguard_cli.egg-info/entry_points.txt
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)       62 2023-03-31 15:08:51.000000 coguard-cli-0.2.6/src/coguard_cli.egg-info/requires.txt
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)       12 2023-03-31 15:08:51.000000 coguard-cli-0.2.6/src/coguard_cli.egg-info/top_level.txt
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.836614 coguard-cli-0.2.7/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1071 2022-06-21 06:40:28.000000 coguard-cli-0.2.7/LICENSE
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9303 2023-04-12 16:13:13.836614 coguard-cli-0.2.7/PKG-INFO
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8931 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/README.md
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8748 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/README_PYPI.md
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)       84 2022-06-21 06:40:28.000000 coguard-cli-0.2.7/pyproject.toml
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      980 2023-04-12 16:13:13.836614 coguard-cli-0.2.7/setup.cfg
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.823281 coguard-cli-0.2.7/src/
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    23004 2023-04-12 16:13:07.000000 coguard-cli-0.2.7/src/coguard_cli/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6592 2023-03-30 03:21:13.000000 coguard-cli-0.2.7/src/coguard_cli/__main__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7702 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/api_connection.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/auth/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8534 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/auth/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1860 2022-07-03 06:44:40.000000 coguard-cli-0.2.7/src/coguard_cli/auth/auth_config.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6313 2023-02-24 03:10:28.000000 coguard-cli-0.2.7/src/coguard_cli/auth/token.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      269 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/auth/util.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/ci_cd/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/ci_cd/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1011 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_provider_abc.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      502 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_provider_factory.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_providers/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_providers/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2193 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_providers/ci_cd_provider_github.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.823281 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_scripts/
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_scripts/github/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      485 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_scripts/github/github_coguard_action.yml
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/discovery/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-22 20:18:10.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/__init__.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1431 2023-03-30 03:21:13.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_provider_abc.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      799 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_provider_factory.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-24 03:43:49.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5713 2023-03-30 03:21:13.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_aws.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2078 2023-03-30 03:21:13.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_azure.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7364 2023-03-30 03:21:13.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2716 2023-03-31 15:08:41.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/Dockerfile
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/data/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      232 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/data/versions.tf
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4492 2023-03-31 15:08:41.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/cmd_for_dfile
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7608 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finder_abc.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2518 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finder_factory.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    25095 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6096 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_apache.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4258 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_docker_compose.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4176 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_dockerfile.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3668 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_elasticsearch.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6197 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_helm.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3615 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_kafka.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6035 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_kerberos.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3490 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_kubernetes.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5011 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_mongodb.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7401 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_mysql.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7047 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_netlify.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5979 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_nginx.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8639 2023-04-12 16:13:07.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_open_telemetry_collector.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9482 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_postgres.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9241 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_redis.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3849 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_terraform.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11379 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_tomcat.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11573 2023-03-31 15:08:41.000000 coguard-cli-0.2.7/src/coguard_cli/docker_dao.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/folder_scan/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9227 2023-02-19 03:22:05.000000 coguard-cli-0.2.7/src/coguard_cli/folder_scan/__init__.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/image_check/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8557 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/image_check/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      239 2022-06-21 06:45:38.000000 coguard-cli-0.2.7/src/coguard_cli/print_colors.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.829947 coguard-cli-0.2.7/src/coguard_cli/tests/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13023 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/tests/api_connection_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/auth/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/auth/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      675 2022-06-21 06:45:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/auth/auth_config_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4927 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/tests/auth/common_auth_function_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8441 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/tests/auth/token_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      595 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/ci_cd_provider_factory_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/ci_cd_providers/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/ci_cd_providers/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2099 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/ci_cd_providers/ci_cd_provider_github_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11605 2023-02-24 03:10:28.000000 coguard-cli-0.2.7/src/coguard_cli/tests/common_functions_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-25 15:30:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/__init__.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-02 14:16:57.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      640 2023-02-02 14:16:57.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_provider_factory_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-02 14:16:57.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8905 2023-02-02 14:16:57.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_aws_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4269 2023-02-02 14:16:57.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_azure_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11454 2023-03-30 03:21:13.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3339 2023-01-25 15:30:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finder_abc_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      637 2023-01-25 15:30:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finder_factory_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-25 15:30:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13736 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/common_functions_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6934 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_apache_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6597 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_docker_compose_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5465 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_dockerfile_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5865 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_elasticsearch_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5736 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_helm_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5634 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kafka_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7029 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kerberos_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5883 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kubernetes_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6248 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mongodb_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6932 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mysql_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6899 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_nginx_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6324 2023-04-12 16:13:07.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_opentelemetry_collector_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8168 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_postgres_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7506 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_redis_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5657 2023-02-14 11:54:29.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_terraform_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9100 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_tomcat_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.833281 coguard-cli-0.2.7/src/coguard_cli/tests/folder_scan/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-23 19:31:49.000000 coguard-cli-0.2.7/src/coguard_cli/tests/folder_scan/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13956 2023-02-19 03:22:05.000000 coguard-cli-0.2.7/src/coguard_cli/tests/folder_scan/common_functions_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.836614 coguard-cli-0.2.7/src/coguard_cli/tests/image_check/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.7/src/coguard_cli/tests/image_check/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    10470 2023-02-24 03:10:28.000000 coguard-cli-0.2.7/src/coguard_cli/tests/image_check/common_functions_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13136 2023-02-01 14:06:40.000000 coguard-cli-0.2.7/src/coguard_cli/tests/image_check/docker_dao_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6243 2023-02-23 02:56:51.000000 coguard-cli-0.2.7/src/coguard_cli/tests/util_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5506 2023-03-05 05:26:44.000000 coguard-cli-0.2.7/src/coguard_cli/util.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-04-12 16:13:13.826614 coguard-cli-0.2.7/src/coguard_cli.egg-info/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9303 2023-04-12 16:13:13.000000 coguard-cli-0.2.7/src/coguard_cli.egg-info/PKG-INFO
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6340 2023-04-12 16:13:13.000000 coguard-cli-0.2.7/src/coguard_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        1 2023-04-12 16:13:13.000000 coguard-cli-0.2.7/src/coguard_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)       54 2023-04-12 16:13:13.000000 coguard-cli-0.2.7/src/coguard_cli.egg-info/entry_points.txt
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)       62 2023-04-12 16:13:13.000000 coguard-cli-0.2.7/src/coguard_cli.egg-info/requires.txt
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)       12 2023-04-12 16:13:13.000000 coguard-cli-0.2.7/src/coguard_cli.egg-info/top_level.txt
```

### Comparing `coguard-cli-0.2.6/LICENSE` & `coguard-cli-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/PKG-INFO` & `coguard-cli-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coguard-cli
-Version: 0.2.6
+Version: 0.2.7
 Summary: A command line interface for scanning configuration files with CoGuard
 Home-page: https://github.com/coguardio/coguard-cli
 Author: Heinle Solutions Inc.
 Author-email: albert@coguard.io
 Project-URL: Bug Tracker, https://github.com/coguardio/coguard-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `coguard-cli-0.2.6/README.md` & `coguard-cli-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/README_PYPI.md` & `coguard-cli-0.2.7/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/setup.cfg` & `coguard-cli-0.2.7/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = coguard-cli
-version = 0.2.6
+version = 0.2.7
 author = Heinle Solutions Inc.
 author_email = albert@coguard.io
 description = A command line interface for scanning configuration files with CoGuard
 long_description = file: README_PYPI.md
 long_description_content_type = text/markdown
 url = https://github.com/coguardio/coguard-cli
 project_urls =
```

### Comparing `coguard-cli-0.2.6/src/coguard_cli/__init__.py` & `coguard-cli-0.2.7/src/coguard_cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,47 +279,51 @@
             coguard_api_url,
             image,
             output_format,
             fail_level,
             organization
         )
 
+# pylint: disable=bare-except
 def _find_and_merge_included_docker_images(
         collected_config_file_tuple: Tuple[str, Dict],
         auth_config: auth.CoGuardCliConfig):
     docker_images_extracted = folder_scan.extract_included_docker_images(
         collected_config_file_tuple
     )
     for image, location in docker_images_extracted:
         print(
             f"{COLOR_CYAN}Found referenced docker image "
             f"{image} in configuration file {location}."
             f"{COLOR_TERMINATION}"
         )
-        temp_folder, temp_inspection, temp_image = image_check.extract_image_to_file_system(
-            image
-        ) or (None, None, None)
-        if temp_folder is None or temp_inspection is None or temp_image is None:
-            continue
-        collected_docker_config_file_tuple = image_check.find_configuration_files_and_collect(
-            image,
-            auth_config.get_username(),
-            temp_folder,
-            temp_inspection
-        )
-        util.merge_coguard_infrastructure_description_folders(
-            "included_docker_image",
-            collected_config_file_tuple,
-            collected_docker_config_file_tuple
-        )
-        # cleanup
-        collected_location, _ = collected_docker_config_file_tuple
-        shutil.rmtree(collected_location, ignore_errors=True)
-        shutil.rmtree(temp_folder, ignore_errors=True)
-        docker_dao.rm_temporary_container_name(temp_image)
+        try:
+            temp_folder, temp_inspection, temp_image = image_check.extract_image_to_file_system(
+                image
+            ) or (None, None, None)
+            if temp_folder is None or temp_inspection is None or temp_image is None:
+                continue
+            collected_docker_config_file_tuple = image_check.find_configuration_files_and_collect(
+                image,
+                auth_config.get_username(),
+                temp_folder,
+                temp_inspection
+            )
+            util.merge_coguard_infrastructure_description_folders(
+                "included_docker_image",
+                collected_config_file_tuple,
+                collected_docker_config_file_tuple
+            )
+            # cleanup
+            collected_location, _ = collected_docker_config_file_tuple
+            shutil.rmtree(collected_location, ignore_errors=True)
+            shutil.rmtree(temp_folder, ignore_errors=True)
+            docker_dao.rm_temporary_container_name(temp_image)
+        except:
+            logging.error("Failed to extract the referenced Docker image.")
 
 def perform_folder_scan(
         folder_name: Optional[str],
         deal_type: auth.util.DealEnum,
         auth_config: auth.CoGuardCliConfig,
         token: auth.token.Token,
         organization: str,
```

### Comparing `coguard-cli-0.2.6/src/coguard_cli/__main__.py` & `coguard-cli-0.2.7/src/coguard_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/api_connection.py` & `coguard-cli-0.2.7/src/coguard_cli/api_connection.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/auth/__init__.py` & `coguard-cli-0.2.7/src/coguard_cli/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/auth/auth_config.py` & `coguard-cli-0.2.7/src/coguard_cli/auth/auth_config.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/auth/token.py` & `coguard-cli-0.2.7/src/coguard_cli/auth/token.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/ci_cd/ci_cd_provider_abc.py` & `coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_provider_abc.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/ci_cd/ci_cd_providers/ci_cd_provider_github.py` & `coguard-cli-0.2.7/src/coguard_cli/ci_cd/ci_cd_providers/ci_cd_provider_github.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/cloud_provider_abc.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_provider_abc.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/cloud_provider_factory.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_provider_factory.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_aws.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_aws.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_azure.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_azure.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/Dockerfile` & `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/Dockerfile`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/cmd_for_dfile` & `coguard-cli-0.2.7/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/cmd_for_dfile`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finder_abc.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finder_abc.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finder_factory.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finder_factory.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/__init__.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/__init__.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_apache.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_apache.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_docker_compose.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_docker_compose.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_dockerfile.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_dockerfile.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_elasticsearch.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_helm.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_helm.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_kafka.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_kafka.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_kerberos.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_kerberos.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_kubernetes.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_kubernetes.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_mongodb.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_mongodb.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_mysql.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_mysql.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_netlify.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_netlify.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_nginx.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_nginx.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_open_telemetry_collector.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_open_telemetry_collector.py`

 * *Files 10% similar despite different names*

```diff
@@ -154,18 +154,27 @@
         keys_to_look_for = [
             "receivers",
             "exporters",
             "service"
         ]
         results = []
         for file_candidate in file_candidates:
-            with open(file_candidate, 'r', encoding='utf-8') as f_handle:
+            file_candidate_without_symlink = cff_util.get_path_behind_symlinks(
+                '',
+                file_candidate
+            )
+            if not os.path.exists(file_candidate_without_symlink) or \
+               not file_candidate_without_symlink.startswith(path_to_file_system):
+                logging.error("The symlink of `%s` did not lead to a valid file inside the folder",
+                              file_candidate)
+                continue
+            with open(file_candidate_without_symlink, 'r', encoding='utf-8') as f_handle:
                 f_content = f_handle.read()
             if all(key in f_content for key in keys_to_look_for):
-                result_files.append(file_candidate)
+                result_files.append(file_candidate_without_symlink)
         for result_file in result_files:
             print(
                 f"{COLOR_CYAN}Found file "
                 f"{result_file.replace(path_to_file_system, '')}"
                 f"{COLOR_TERMINATION}"
             )
             append_candidate = self._create_temp_location_and_manifest_entry(
```

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_postgres.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_postgres.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_redis.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_redis.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_terraform.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_terraform.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/discovery/config_file_finders/config_file_finder_tomcat.py` & `coguard-cli-0.2.7/src/coguard_cli/discovery/config_file_finders/config_file_finder_tomcat.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/docker_dao.py` & `coguard-cli-0.2.7/src/coguard_cli/docker_dao.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/folder_scan/__init__.py` & `coguard-cli-0.2.7/src/coguard_cli/folder_scan/__init__.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/image_check/__init__.py` & `coguard-cli-0.2.7/src/coguard_cli/image_check/__init__.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/api_connection_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/api_connection_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/auth/auth_config_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/auth/auth_config_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/auth/common_auth_function_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/auth/common_auth_function_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/auth/token_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/auth/token_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/ci_cd/ci_cd_provider_factory_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/ci_cd_provider_factory_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/ci_cd/ci_cd_providers/ci_cd_provider_github_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/ci_cd/ci_cd_providers/ci_cd_provider_github_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/common_functions_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/common_functions_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/cloud_discovery/cloud_provider_factory_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_provider_factory_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_aws_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_aws_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_azure_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_azure_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finder_abc_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finder_abc_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finder_factory_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finder_factory_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/common_functions_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/common_functions_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_apache_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_apache_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_docker_compose_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_docker_compose_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_dockerfile_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_dockerfile_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_elasticsearch_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_elasticsearch_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_helm_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_helm_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kafka_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kafka_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kerberos_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kerberos_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kubernetes_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kubernetes_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mongodb_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mongodb_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mysql_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mysql_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_nginx_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_nginx_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_opentelemetry_collector_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_opentelemetry_collector_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,21 @@
     def test_check_for_config_files_filesystem_search_existing(self):
         """
         This checks for the standard location test and sees if the file is
         existent or not.
         """
         with unittest.mock.patch(
                 "os.walk",
-                new_callable=lambda: lambda location: [("etc", [], ["server.yaml"])]), \
+                new_callable=lambda: lambda location: [("foo/etc", [], ["server.yaml"])]), \
+                unittest.mock.patch(
+                "os.path.exists",
+                new_callable=lambda: lambda location: True), \
+                unittest.mock.patch(
+                "coguard_cli.discovery.config_file_finders.get_path_behind_symlinks",
+                new_callable = lambda: lambda p, q: q), \
                 unittest.mock.patch(
                 'builtins.open',
                 unittest.mock.mock_open(
                     read_data="receiversprocessorsexportersextensionsservice")
                 ), \
                 unittest.mock.patch(
                     ("coguard_cli.discovery.config_file_finders.config_file_"
```

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_postgres_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_postgres_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_redis_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_redis_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_terraform_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_terraform_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_tomcat_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_tomcat_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/folder_scan/common_functions_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/folder_scan/common_functions_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/image_check/common_functions_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/image_check/common_functions_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/image_check/docker_dao_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/image_check/docker_dao_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/tests/util_test.py` & `coguard-cli-0.2.7/src/coguard_cli/tests/util_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli/util.py` & `coguard-cli-0.2.7/src/coguard_cli/util.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.6/src/coguard_cli.egg-info/PKG-INFO` & `coguard-cli-0.2.7/src/coguard_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coguard-cli
-Version: 0.2.6
+Version: 0.2.7
 Summary: A command line interface for scanning configuration files with CoGuard
 Home-page: https://github.com/coguardio/coguard-cli
 Author: Heinle Solutions Inc.
 Author-email: albert@coguard.io
 Project-URL: Bug Tracker, https://github.com/coguardio/coguard-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `coguard-cli-0.2.6/src/coguard_cli.egg-info/SOURCES.txt` & `coguard-cli-0.2.7/src/coguard_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

