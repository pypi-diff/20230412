# Comparing `tmp/rime_sdk-2.0.0rc5.tar.gz` & `tmp/rime_sdk-2.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.0.0rc5.tar", last modified: Sat Apr  8 17:42:50 2023, max compression
+gzip compressed data, was "rime_sdk-2.0.0rc6.tar", last modified: Wed Apr 12 04:35:30 2023, max compression
```

## Comparing `rime_sdk-2.0.0rc5.tar` & `rime_sdk-2.0.0rc6.tar`

### file list

```diff
@@ -1,477 +1,477 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:42:50.736407 rime_sdk-2.0.0rc5/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-04-08 17:42:50.736407 rime_sdk-2.0.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27071 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:42:50.628401 rime_sdk-2.0.0rc5/rime_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57754 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:42:50.632402 rime_sdk-2.0.0rc5/rime_sdk/data_format_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/data_format_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/data_format_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/data_format_check/data_format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/data_format_check/nlp_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/data_format_check/tabular_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:42:50.632402 rime_sdk-2.0.0rc5/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28283 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/internal/security_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    55004 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    23861 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:42:50.632402 rime_sdk-2.0.0rc5/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:42:50.632402 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    45243 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:42:50.640402 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26953 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29422 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55786 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57282 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    50274 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41732 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:42:50.732407 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    43392 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_data_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_location_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_location_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/model_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/model_model_path_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_archived_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20224 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-04-08 17:42:46.000000 rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:42:50.628401 rime_sdk-2.0.0rc5/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-04-08 17:42:50.000000 rime_sdk-2.0.0rc5/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31351 2023-04-08 17:42:50.000000 rime_sdk-2.0.0rc5/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 17:42:50.000000 rime_sdk-2.0.0rc5/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-08 17:42:50.000000 rime_sdk-2.0.0rc5/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-08 17:42:50.000000 rime_sdk-2.0.0rc5/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-08 17:42:50.000000 rime_sdk-2.0.0rc5/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 17:42:50.736407 rime_sdk-2.0.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-08 17:41:48.000000 rime_sdk-2.0.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.543780 rime_sdk-2.0.0rc6/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-04-12 04:35:30.543780 rime_sdk-2.0.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27071 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.459778 rime_sdk-2.0.0rc6/rime_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57754 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.463778 rime_sdk-2.0.0rc6/rime_sdk/data_format_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/data_format_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/data_format_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/data_format_check/data_format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/data_format_check/nlp_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/data_format_check/tabular_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22486 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.467779 rime_sdk-2.0.0rc6/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28424 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/security_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55004 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23861 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.467779 rime_sdk-2.0.0rc6/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.467779 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    45243 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.471778 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26951 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29422 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55776 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57282 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50274 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41732 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.543780 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    43392 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_data_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_location_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_location_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_model_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.459778 rime_sdk-2.0.0rc6/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-04-12 04:35:30.000000 rime_sdk-2.0.0rc6/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31351 2023-04-12 04:35:30.000000 rime_sdk-2.0.0rc6/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:35:30.000000 rime_sdk-2.0.0rc6/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-12 04:35:30.000000 rime_sdk-2.0.0rc6/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 04:35:30.000000 rime_sdk-2.0.0rc6/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 04:35:30.000000 rime_sdk-2.0.0rc6/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 04:35:30.547780 rime_sdk-2.0.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/setup.py
```

### Comparing `rime_sdk-2.0.0rc5/LICENSE` & `rime_sdk-2.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/PKG-INFO` & `rime_sdk-2.0.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.0.0rc5
+Version: 2.0.0rc6
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.0.0rc5/README.md` & `rime_sdk-2.0.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/__init__.py` & `rime_sdk-2.0.0rc6/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/client.py` & `rime_sdk-2.0.0rc6/rime_sdk/client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/data_collector.py` & `rime_sdk-2.0.0rc6/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/data_format_check/cli.py` & `rime_sdk-2.0.0rc6/rime_sdk/data_format_check/cli.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/data_format_check/data_format_checker.py` & `rime_sdk-2.0.0rc6/rime_sdk/data_format_check/data_format_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/data_format_check/nlp_checker.py` & `rime_sdk-2.0.0rc6/rime_sdk/data_format_check/nlp_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/data_format_check/tabular_checker.py` & `rime_sdk-2.0.0rc6/rime_sdk/data_format_check/tabular_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/detection_event.py` & `rime_sdk-2.0.0rc6/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/firewall.py` & `rime_sdk-2.0.0rc6/rime_sdk/firewall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Library defining the interface to firewall."""
 from datetime import timedelta
 from typing import Any, Dict, Iterator, List, Optional
 
+import pandas as pd
+
 from rime_sdk.internal.constants import (
     MONITOR_TYPE_TO_SWAGGER,
     RISK_CATEGORY_TO_SWAGGER,
 )
 from rime_sdk.internal.decorators import prompt_confirmation
 from rime_sdk.internal.rest_error_handler import RESTErrorHandler
+from rime_sdk.internal.swagger_parser import parse_events_to_df
 from rime_sdk.internal.swagger_utils import (
     get_data_location_swagger,
     rest_to_timedelta,
     timedelta_to_rest,
 )
 from rime_sdk.internal.throttle_queue import ThrottleQueue
 from rime_sdk.internal.utils import convert_dict_to_html, make_link
@@ -29,15 +32,19 @@
     RuntimeinfoCustomImage,
     RuntimeinfoCustomImageType,
     RuntimeinfoResourceRequest,
     RuntimeinfoRunTimeInfo,
     TestrunTestRunIncrementalConfig,
     V1firewallfirewallFirewallIdUuidFirewall,
 )
+from rime_sdk.swagger.swagger_client.api.detection_api import DetectionApi
 from rime_sdk.swagger.swagger_client.models import RimeJobMetadata
+from rime_sdk.swagger.swagger_client.models.detection_event_type import (
+    DetectionEventType,
+)
 
 # 30 days in seconds
 # 1 day = 86400 seconds
 LIST_TEST_RUNS_INTERVAL_LENGTH_SECONDS = 30 * 86400
 
 
 class Firewall:
@@ -292,14 +299,46 @@
 
     def _get_firewall(self) -> FirewallFirewall:
         api = swagger_client.FirewallServiceApi(self._api_client)
         with RESTErrorHandler():
             res = api.firewall_service_get_firewall(firewall_id_uuid=self._firewall_id)
         return res.firewall
 
+    def get_events_df(self,) -> pd.DataFrame:
+        """Get a dataframe of Detected Events for the given Firewall.
+
+        Monitors detect Events when degradations occur.
+        For example, a Monitor for the metric "Accuracy" will detect an Event
+        when the value of the model performance metric drops below a threshold.
+        """
+        # TODO [Wombat]: allow user to specify a time interval to query over.
+        detection_api = DetectionApi(self._api_client)
+        next_page_token = ""
+        has_more = True
+        all_events = []
+        while has_more:
+            kwargs: Dict[str, Any] = {}
+            if len(next_page_token) > 0:
+                kwargs["page_token"] = next_page_token
+            else:
+                # Restrict to events for CT.
+                kwargs["first_page_req_event_types"] = [
+                    DetectionEventType.METRIC_DEGRADATION,
+                    DetectionEventType.SECURITY,
+                ]
+            with RESTErrorHandler():
+                res = detection_api.detection_list_detection_events(
+                    self.project_id, **kwargs
+                )
+                next_page_token = res.next_page_token
+                has_more = res.has_more
+                all_events += res.events
+        df = parse_events_to_df(all_events)
+        return df
+
     def list_monitors(
         self,
         monitor_types: Optional[List[str]] = None,
         risk_category_types: Optional[List[str]] = None,
     ) -> Iterator[Monitor]:
         """List Monitors for the given Firewall.
```

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/image_builder.py` & `rime_sdk-2.0.0rc6/rime_sdk/image_builder.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/internal/config_parser.py` & `rime_sdk-2.0.0rc6/rime_sdk/internal/config_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -573,14 +573,16 @@
         kwargs["custom_tests"] = _get_custom_tests_swagger(
             test_suite_config["custom_tests"]
         )
     if "global_test_sensitivity" in test_suite_config:
         kwargs["global_test_sensitivity"] = _get_test_sensitivities_swagger(
             test_suite_config["global_test_sensitivity"]
         )
+    if "global_exclude_columns" in test_suite_config:
+        kwargs["global_exclude_columns"] = test_suite_config["global_exclude_columns"]
     return TestrunTestSuiteConfig(**kwargs)
 
 
 @validate_types
 def _get_custom_image_swagger(custom_image: dict) -> RuntimeinfoCustomImage:
     kwargs: Dict[str, Any] = {}
     _custom_image = deepcopy(custom_image)
```

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/internal/constants.py` & `rime_sdk-2.0.0rc6/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/internal/decorators.py` & `rime_sdk-2.0.0rc6/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/internal/file_upload.py` & `rime_sdk-2.0.0rc6/rime_sdk/internal/file_upload.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.0.0rc6/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/internal/security_config_parser.py` & `rime_sdk-2.0.0rc6/rime_sdk/internal/security_config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.0.0rc6/rime_sdk/internal/swagger_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Library for converting Swagger objects to Python data types such as dataframes."""
 import re
-from typing import Any, Dict, Union
+from typing import Any, Dict, List, Union
 
 import numpy as np
 import pandas as pd
 
 from rime_sdk.swagger.swagger_client.models import (
     RimeCategoryTestResult,
     TestrunresultTestBatchResult,
     TestrunresultTestCase,
     TestrunresultTestRunDetail,
 )
+from rime_sdk.swagger.swagger_client.models.detection_detection_event import (
+    DetectionDetectionEvent,
+)
 
 MODEL_PERF_REGEX = r"^metrics\.model_perf.*(ref_metric|eval_metric)$"
 
 # Map of flattened field paths to their types in the Dataframe.
 DEFAULT_TEST_RUN_COLUMN_INFO = {
     # Metadata.
     "test_run_id": "str",
@@ -80,14 +83,28 @@
     "int_value",
     "str_value",
     "float_list",
     "int_list",
     "str_list",
 ]
 
+EVENT_COLUMNS_TO_SHOW = [
+    "project_id",
+    "event_type",
+    "severity",
+    "event_object_name",
+    "event_object_id",
+    "risk_category_type",
+    "test_category",
+    "event_time_range.start_time",
+    "event_time_range.end_time",
+    "description",
+    "detail.metric_degradation.rca_result.description",
+]
+
 
 def parse_test_run_metadata(test_run: TestrunresultTestRunDetail) -> pd.DataFrame:
     """Parse test run metadata Swagger message into a Pandas dataframe.
 
     The columns are not guaranteed to be returned in sorted order.
     Some values are optional and will appear as a NaN value in the dataframe.
 
@@ -218,7 +235,18 @@
     if unpack_metrics:
         for metric in raw_result.category_metrics:
             raw_dict[metric.name] = metric.value
     severity_count_dict = raw_dict.pop("severity_counts")
     for key in severity_count_dict:
         raw_dict[key] = int(severity_count_dict[key])
     return raw_dict
+
+
+def parse_events_to_df(events: List[DetectionDetectionEvent],) -> pd.DataFrame:
+    """Parse a list of Detection Events to a pandas DateFrame."""
+    event_dicts = [event.to_dict() for event in events]
+    df = pd.json_normalize(event_dicts, sep=DF_FLATTEN_SEPARATOR)
+
+    intersect_df = df[df.columns.intersection(EVENT_COLUMNS_TO_SHOW)]
+    intersect_df = intersect_df.rename({"event_object_id": "monitor_id"}, axis=1)
+
+    return intersect_df
```

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.0.0rc6/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.0.0rc6/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.0.0rc6/rime_sdk/internal/throttle_queue.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/internal/utils.py` & `rime_sdk-2.0.0rc6/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/job.py` & `rime_sdk-2.0.0rc6/rime_sdk/job.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/monitor.py` & `rime_sdk-2.0.0rc6/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/project.py` & `rime_sdk-2.0.0rc6/rime_sdk/project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/registry.py` & `rime_sdk-2.0.0rc6/rime_sdk/registry.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def job_reader_list_jobs_for_project(self, project_id_uuid, **kwargs):  # noqa: E501
         """ListJobsForProject  # noqa: E501
 
-        Returns a paginated list of jobs for a given project. The list can be filtered by job type and status.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this      # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers)     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['jobs'])     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
+        Returns a paginated list of jobs for a given project. The list can be filtered by job type and status.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers)     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['jobs'])     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_reader_list_jobs_for_project(project_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_id_uuid: Unique object ID. (required)
@@ -442,15 +442,15 @@
         else:
             (data) = self.job_reader_list_jobs_for_project_with_http_info(project_id_uuid, **kwargs)  # noqa: E501
             return data
 
     def job_reader_list_jobs_for_project_with_http_info(self, project_id_uuid, **kwargs):  # noqa: E501
         """ListJobsForProject  # noqa: E501
 
-        Returns a paginated list of jobs for a given project. The list can be filtered by job type and status.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this      # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers)     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['jobs'])     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
+        Returns a paginated list of jobs for a given project. The list can be filtered by job type and status.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers)     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['jobs'])     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_reader_list_jobs_for_project_with_http_info(project_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_id_uuid: Unique object ID. (required)
```

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def model_testing_get_latest_logs(self, job_id, **kwargs):  # noqa: E501
         """GetLatestLogs  # noqa: E501
 
-        Returns the logs of the latest pod to run the test job with the  specified job ID.  # noqa: E501
+        Returns the logs of the latest pod to run the test job with the specified job ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.model_testing_get_latest_logs(job_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str job_id: Uniquely specifies a Job. (required)
@@ -53,15 +53,15 @@
         else:
             (data) = self.model_testing_get_latest_logs_with_http_info(job_id, **kwargs)  # noqa: E501
             return data
 
     def model_testing_get_latest_logs_with_http_info(self, job_id, **kwargs):  # noqa: E501
         """GetLatestLogs  # noqa: E501
 
-        Returns the logs of the latest pod to run the test job with the  specified job ID.  # noqa: E501
+        Returns the logs of the latest pod to run the test job with the specified job ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.model_testing_get_latest_logs_with_http_info(job_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str job_id: Uniquely specifies a Job. (required)
```

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def project_service_add_users_to_project(self, body, project_id_uuid, **kwargs):  # noqa: E501
         """AddUsersToProject  # noqa: E501
 
-        Grants existing Organization users permissions to a Project  for a given Project ID, based on the pairs of role and User ID provided in the request.  # noqa: E501
+        Grants existing Organization users permissions to a Project for a given Project ID, based on the pairs of role and User ID provided in the request.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.project_service_add_users_to_project(body, project_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param RoleUsersBody body: (required)
@@ -54,15 +54,15 @@
         else:
             (data) = self.project_service_add_users_to_project_with_http_info(body, project_id_uuid, **kwargs)  # noqa: E501
             return data
 
     def project_service_add_users_to_project_with_http_info(self, body, project_id_uuid, **kwargs):  # noqa: E501
         """AddUsersToProject  # noqa: E501
 
-        Grants existing Organization users permissions to a Project  for a given Project ID, based on the pairs of role and User ID provided in the request.  # noqa: E501
+        Grants existing Organization users permissions to a Project for a given Project ID, based on the pairs of role and User ID provided in the request.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.project_service_add_users_to_project_with_http_info(body, project_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param RoleUsersBody body: (required)
@@ -138,15 +138,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def project_service_create_project(self, body, **kwargs):  # noqa: E501
         """CreateProject  # noqa: E501
 
-        Creates a Project with required fields. Project is an organizational entity under a Workspace that contains  Test Runs, Continuous Tests, and Stress Tests, along with their  configurations.  # noqa: E501
+        Creates a Project with required fields. Project is an organizational entity under a Workspace that contains Test Runs, Continuous Tests, and Stress Tests, along with their configurations.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.project_service_create_project(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param ProjectCreateProjectRequest body: (required)
@@ -160,15 +160,15 @@
         else:
             (data) = self.project_service_create_project_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
     def project_service_create_project_with_http_info(self, body, **kwargs):  # noqa: E501
         """CreateProject  # noqa: E501
 
-        Creates a Project with required fields. Project is an organizational entity under a Workspace that contains  Test Runs, Continuous Tests, and Stress Tests, along with their  configurations.  # noqa: E501
+        Creates a Project with required fields. Project is an organizational entity under a Workspace that contains Test Runs, Continuous Tests, and Stress Tests, along with their configurations.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.project_service_create_project_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param ProjectCreateProjectRequest body: (required)
@@ -617,15 +617,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def project_service_list_projects(self, **kwargs):  # noqa: E501
         """ListProjects  # noqa: E501
 
-        Returns a paginated list of Projects for a given Workspace ID.  Filters out Projects that the user does not have access to. The list is sorted by the last test run time field of each Project.  # noqa: E501
+        Returns a paginated list of Projects for a given Workspace ID. Filters out Projects that the user does not have access to. The list is sorted by the last test run time field of each Project.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.project_service_list_projects(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str workspace_id_uuid: Unique object ID.
@@ -641,15 +641,15 @@
         else:
             (data) = self.project_service_list_projects_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def project_service_list_projects_with_http_info(self, **kwargs):  # noqa: E501
         """ListProjects  # noqa: E501
 
-        Returns a paginated list of Projects for a given Workspace ID.  Filters out Projects that the user does not have access to. The list is sorted by the last test run time field of each Project.  # noqa: E501
+        Returns a paginated list of Projects for a given Workspace ID. Filters out Projects that the user does not have access to. The list is sorted by the last test run time field of each Project.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.project_service_list_projects_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str workspace_id_uuid: Unique object ID.
@@ -1029,15 +1029,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def project_service_update_user_of_project(self, body, project_id_uuid, user_user_id_uuid, **kwargs):  # noqa: E501
         """UpdateUserOfProject  # noqa: E501
 
-        Updates the existing permission of a user of a Project given  Project ID and User ID.  # noqa: E501
+        Updates the existing permission of a user of a Project given Project ID and User ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.project_service_update_user_of_project(body, project_id_uuid, user_user_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param UsersUserUserIdUuidBody body: (required)
@@ -1053,15 +1053,15 @@
         else:
             (data) = self.project_service_update_user_of_project_with_http_info(body, project_id_uuid, user_user_id_uuid, **kwargs)  # noqa: E501
             return data
 
     def project_service_update_user_of_project_with_http_info(self, body, project_id_uuid, user_user_id_uuid, **kwargs):  # noqa: E501
         """UpdateUserOfProject  # noqa: E501
 
-        Updates the existing permission of a user of a Project given  Project ID and User ID.  # noqa: E501
+        Updates the existing permission of a user of a Project given Project ID and User ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.project_service_update_user_of_project_with_http_info(body, project_id_uuid, user_user_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param UsersUserUserIdUuidBody body: (required)
```

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,26 +126,26 @@
 
         self._nrows_per_query = nrows_per_query
 
     @property
     def drop_query_id(self):
         """Gets the drop_query_id of this DataInfoParamsRankingInfo.  # noqa: E501
 
-        Whether to drop the query ID column from the dataset to avoid  passing as a feature to the model.  # noqa: E501
+        Whether to drop the query ID column from the dataset to avoid passing as a feature to the model.  # noqa: E501
 
         :return: The drop_query_id of this DataInfoParamsRankingInfo.  # noqa: E501
         :rtype: bool
         """
         return self._drop_query_id
 
     @drop_query_id.setter
     def drop_query_id(self, drop_query_id):
         """Sets the drop_query_id of this DataInfoParamsRankingInfo.
 
-        Whether to drop the query ID column from the dataset to avoid  passing as a feature to the model.  # noqa: E501
+        Whether to drop the query ID column from the dataset to avoid passing as a feature to the model.  # noqa: E501
 
         :param drop_query_id: The drop_query_id of this DataInfoParamsRankingInfo.  # noqa: E501
         :type: bool
         """
 
         self._drop_query_id = drop_query_id
```

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_data_location.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_data_location.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_location_args.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_location_args.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_location_params.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_location_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,26 +68,26 @@
 
         self._model_uri = model_uri
 
     @property
     def kwargs(self):
         """Gets the kwargs of this ModelHuggingFaceModelInfo.  # noqa: E501
 
-        We are currently in the process of adding extra  huggingface params and separating use cases into tabular and nlp. Use a serialized json dictionary for other variables right now to ensure maximum flexibility.  # noqa: E501
+        We are currently in the process of adding extra huggingface params and separating use cases into tabular and nlp. Use a serialized json dictionary for other variables right now to ensure maximum flexibility.  # noqa: E501
 
         :return: The kwargs of this ModelHuggingFaceModelInfo.  # noqa: E501
         :rtype: str
         """
         return self._kwargs
 
     @kwargs.setter
     def kwargs(self, kwargs):
         """Sets the kwargs of this ModelHuggingFaceModelInfo.
 
-        We are currently in the process of adding extra  huggingface params and separating use cases into tabular and nlp. Use a serialized json dictionary for other variables right now to ensure maximum flexibility.  # noqa: E501
+        We are currently in the process of adding extra huggingface params and separating use cases into tabular and nlp. Use a serialized json dictionary for other variables right now to ensure maximum flexibility.  # noqa: E501
 
         :param kwargs: The kwargs of this ModelHuggingFaceModelInfo.  # noqa: E501
         :type: str
         """
 
         self._kwargs = kwargs
```

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,26 +191,26 @@
 
         self._creation_time = creation_time
 
     @property
     def external_id(self):
         """Gets the external_id of this ModelModel.  # noqa: E501
 
-        external_id is an optional way for a user to identify the model  with their own Model IDs.  # noqa: E501
+        external_id is an optional way for a user to identify the model with their own Model IDs.  # noqa: E501
 
         :return: The external_id of this ModelModel.  # noqa: E501
         :rtype: str
         """
         return self._external_id
 
     @external_id.setter
     def external_id(self, external_id):
         """Sets the external_id of this ModelModel.
 
-        external_id is an optional way for a user to identify the model  with their own Model IDs.  # noqa: E501
+        external_id is an optional way for a user to identify the model with their own Model IDs.  # noqa: E501
 
         :param external_id: The external_id of this ModelModel.  # noqa: E501
         :type: str
         """
 
         self._external_id = external_id
```

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/model_model_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/model_model_path_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_model_path_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rca_rca_result.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_rca_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rca_rca_role.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_rca_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_archived_job_logs.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_archived_job_logs.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_request.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_tag.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_tag.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,26 +263,26 @@
 
         self._nrows = nrows
 
     @property
     def nrows_per_time_bin(self):
         """Gets the nrows_per_time_bin of this TestrunDataInfoParams.  # noqa: E501
 
-        Number of rows of data per time bin to load and test in CT. If null,  will load all rows.  # noqa: E501
+        Number of rows of data per time bin to load and test in CT. If null, will load all rows.  # noqa: E501
 
         :return: The nrows_per_time_bin of this TestrunDataInfoParams.  # noqa: E501
         :rtype: str
         """
         return self._nrows_per_time_bin
 
     @nrows_per_time_bin.setter
     def nrows_per_time_bin(self, nrows_per_time_bin):
         """Sets the nrows_per_time_bin of this TestrunDataInfoParams.
 
-        Number of rows of data per time bin to load and test in CT. If null,  will load all rows.  # noqa: E501
+        Number of rows of data per time bin to load and test in CT. If null, will load all rows.  # noqa: E501
 
         :param nrows_per_time_bin: The nrows_per_time_bin of this TestrunDataInfoParams.  # noqa: E501
         :type: str
         """
 
         self._nrows_per_time_bin = nrows_per_time_bin
 
@@ -468,26 +468,26 @@
 
         self._loading_kwargs = loading_kwargs
 
     @property
     def feature_type_path(self):
         """Gets the feature_type_path of this TestrunDataInfoParams.  # noqa: E501
 
-        Path to a CSV file that specifies the data type of each feature.  The file should have two columns: FeatureName and FeatureType.  # noqa: E501
+        Path to a CSV file that specifies the data type of each feature. The file should have two columns: FeatureName and FeatureType.  # noqa: E501
 
         :return: The feature_type_path of this TestrunDataInfoParams.  # noqa: E501
         :rtype: str
         """
         return self._feature_type_path
 
     @feature_type_path.setter
     def feature_type_path(self, feature_type_path):
         """Sets the feature_type_path of this TestrunDataInfoParams.
 
-        Path to a CSV file that specifies the data type of each feature.  The file should have two columns: FeatureName and FeatureType.  # noqa: E501
+        Path to a CSV file that specifies the data type of each feature. The file should have two columns: FeatureName and FeatureType.  # noqa: E501
 
         :param feature_type_path: The feature_type_path of this TestrunDataInfoParams.  # noqa: E501
         :type: str
         """
 
         self._feature_type_path = feature_type_path
```

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_category.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/test_batch.py` & `rime_sdk-2.0.0rc6/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk/test_run.py` & `rime_sdk-2.0.0rc6/rime_sdk/test_run.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.0.0rc6/rime_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.0.0rc5
+Version: 2.0.0rc6
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.0.0rc5/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.0.0rc6/rime_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc5/setup.py` & `rime_sdk-2.0.0rc6/setup.py`

 * *Files identical despite different names*

