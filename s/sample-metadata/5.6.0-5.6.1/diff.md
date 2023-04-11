# Comparing `tmp/sample_metadata-5.6.0.tar.gz` & `tmp/sample_metadata-5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sample_metadata-5.6.0.tar", last modified: Wed Apr  5 05:25:42 2023, max compression
+gzip compressed data, was "sample_metadata-5.6.1.tar", last modified: Tue Apr 11 23:58:43 2023, max compression
```

## Comparing `sample_metadata-5.6.0.tar` & `sample_metadata-5.6.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:25:42.561952 sample_metadata-5.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-04-05 05:25:42.561952 sample_metadata-5.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:25:42.529952 sample_metadata-5.6.0/sample_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:25:42.533952 sample_metadata-5.6.0/sample_metadata/api/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61864 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/api/analysis_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28845 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/api/family_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42202 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/api/participant_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27906 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53539 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/api/sample_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    47013 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/api/seqr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    38773 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/api/sequence_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/api/web_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37587 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:25:42.533952 sample_metadata-5.6.0/sample_metadata/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17054 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:25:42.549952 sample_metadata-5.6.0/sample_metadata/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/analysis_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/analysis_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/analysis_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/analysis_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/analysis_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/body_get_latest_complete_analysis_for_type_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/body_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/body_get_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/body_get_sequences_by_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/export_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/extra_participant_importer_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/family_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/family_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/meta_search_entity_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/nested_family.py
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/nested_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/nested_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/nested_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/new_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/new_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/paging_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/participant_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/participant_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/participant_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/participant_upsert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/project_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/sample_batch_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/sample_batch_upsert_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/sample_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/sample_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/sample_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/search_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/search_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/search_response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/sequence_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/sequence_technology.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/sequence_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/sequence_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/sequence_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model/web_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    82237 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:25:42.549952 sample_metadata-5.6.0/sample_metadata/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:25:42.553952 sample_metadata-5.6.0/sample_metadata/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/sample_metadata/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/sample_metadata/parser/cloudhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)    32263 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/sample_metadata/parser/generic_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    49430 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/sample_metadata/parser/generic_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/sample_metadata/parser/sample_file_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-04-05 05:23:30.000000 sample_metadata-5.6.0/sample_metadata/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:25:42.529952 sample_metadata-5.6.0/sample_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-04-05 05:25:42.000000 sample_metadata-5.6.0/sample_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-05 05:25:42.000000 sample_metadata-5.6.0/sample_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 05:25:42.000000 sample_metadata-5.6.0/sample_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 05:25:42.000000 sample_metadata-5.6.0/sample_metadata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-05 05:25:42.000000 sample_metadata-5.6.0/sample_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-05 05:25:42.000000 sample_metadata-5.6.0/sample_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 05:25:42.561952 sample_metadata-5.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:25:42.561952 sample_metadata-5.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_add_samples_for_joint_calling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_import_individual_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_joint_calling_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_parse_file_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    26731 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_parse_generic_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_parse_ont_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_parse_ont_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16296 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-04-05 05:21:08.000000 sample_metadata-5.6.0/test/testbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.115352 sample_metadata-5.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-04-11 23:58:43.115352 sample_metadata-5.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.099352 sample_metadata-5.6.1/sample_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.099352 sample_metadata-5.6.1/sample_metadata/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61864 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/analysis_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28845 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/family_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42202 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/participant_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27906 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53539 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/sample_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47013 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/seqr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38773 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/sequence_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37587 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.099352 sample_metadata-5.6.1/sample_metadata/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17054 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.103351 sample_metadata-5.6.1/sample_metadata/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/analysis_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/analysis_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/analysis_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/analysis_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/analysis_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/body_get_latest_complete_analysis_for_type_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/body_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/body_get_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/body_get_sequences_by_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/export_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/extra_participant_importer_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/family_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/family_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/meta_search_entity_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/nested_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/nested_participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/nested_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/nested_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/new_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-11 23:56:38.000000 sample_metadata-5.6.1/sample_metadata/model/new_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/paging_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/participant_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/participant_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/participant_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/participant_upsert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/project_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sample_batch_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sample_batch_upsert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sample_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sample_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sample_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/search_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/search_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/search_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sequence_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sequence_technology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sequence_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sequence_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/sequence_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model/web_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82237 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.103351 sample_metadata-5.6.1/sample_metadata/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.107352 sample_metadata-5.6.1/sample_metadata/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/sample_metadata/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/sample_metadata/parser/cloudhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32263 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/sample_metadata/parser/generic_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49430 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/sample_metadata/parser/generic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/sample_metadata/parser/sample_file_map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-04-11 23:56:39.000000 sample_metadata-5.6.1/sample_metadata/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.099352 sample_metadata-5.6.1/sample_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-04-11 23:58:43.000000 sample_metadata-5.6.1/sample_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-11 23:58:43.000000 sample_metadata-5.6.1/sample_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:58:43.000000 sample_metadata-5.6.1/sample_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:58:43.000000 sample_metadata-5.6.1/sample_metadata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 23:58:43.000000 sample_metadata-5.6.1/sample_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 23:58:43.000000 sample_metadata-5.6.1/sample_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 23:58:43.115352 sample_metadata-5.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:58:43.115352 sample_metadata-5.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_add_samples_for_joint_calling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_import_individual_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_joint_calling_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_parse_file_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26731 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_parse_generic_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_parse_ont_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_parse_ont_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16296 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-11 23:54:25.000000 sample_metadata-5.6.1/test/testbase.py
```

### Comparing `sample_metadata-5.6.0/LICENSE` & `sample_metadata-5.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/PKG-INFO` & `sample_metadata-5.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample_metadata
-Version: 5.6.0
+Version: 5.6.1
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sample_metadata-5.6.0/README.md` & `sample_metadata-5.6.1/README.md`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/sample_metadata/__init__.py` & `sample_metadata-5.6.1/sample_metadata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `sample_metadata-5.6.0/sample_metadata/api/analysis_api.py` & `sample_metadata-5.6.1/sample_metadata/api/analysis_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/api/default_api.py` & `sample_metadata-5.6.1/sample_metadata/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/api/family_api.py` & `sample_metadata-5.6.1/sample_metadata/api/family_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/api/import_api.py` & `sample_metadata-5.6.1/sample_metadata/api/import_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/api/participant_api.py` & `sample_metadata-5.6.1/sample_metadata/api/participant_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/api/project_api.py` & `sample_metadata-5.6.1/sample_metadata/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/api/sample_api.py` & `sample_metadata-5.6.1/sample_metadata/api/sample_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/api/seqr_api.py` & `sample_metadata-5.6.1/sample_metadata/api/seqr_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/api/sequence_api.py` & `sample_metadata-5.6.1/sample_metadata/api/sequence_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/api/web_api.py` & `sample_metadata-5.6.1/sample_metadata/api/web_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/api_client.py` & `sample_metadata-5.6.1/sample_metadata/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
```

### Comparing `sample_metadata-5.6.0/sample_metadata/apis/__init__.py` & `sample_metadata-5.6.1/sample_metadata/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/sample_metadata/configuration.py` & `sample_metadata-5.6.1/sample_metadata/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 from os import getenv
 import json
 import copy
@@ -399,15 +399,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 5.6.0\n"\
+               "Version of the API: 5.6.1\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `sample_metadata-5.6.0/sample_metadata/exceptions.py` & `sample_metadata-5.6.1/sample_metadata/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/analysis_model.py` & `sample_metadata-5.6.1/sample_metadata/model/analysis_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/analysis_query_model.py` & `sample_metadata-5.6.1/sample_metadata/model/analysis_query_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/analysis_status.py` & `sample_metadata-5.6.1/sample_metadata/model/analysis_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/analysis_type.py` & `sample_metadata-5.6.1/sample_metadata/model/analysis_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/analysis_update_model.py` & `sample_metadata-5.6.1/sample_metadata/model/analysis_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/body_get_latest_complete_analysis_for_type_post.py` & `sample_metadata-5.6.1/sample_metadata/model/body_get_latest_complete_analysis_for_type_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/body_get_participants.py` & `sample_metadata-5.6.1/sample_metadata/model/body_get_participants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/body_get_samples.py` & `sample_metadata-5.6.1/sample_metadata/model/body_get_samples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/body_get_sequences_by_criteria.py` & `sample_metadata-5.6.1/sample_metadata/model/body_get_sequences_by_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/error_response.py` & `sample_metadata-5.6.1/sample_metadata/model/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/export_type.py` & `sample_metadata-5.6.1/sample_metadata/model/export_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/extra_participant_importer_handler.py` & `sample_metadata-5.6.1/sample_metadata/model/extra_participant_importer_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/family_search_response_data.py` & `sample_metadata-5.6.1/sample_metadata/model/family_search_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/family_update_model.py` & `sample_metadata-5.6.1/sample_metadata/model/family_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/http_validation_error.py` & `sample_metadata-5.6.1/sample_metadata/model/http_validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/meta_search_entity_prefix.py` & `sample_metadata-5.6.1/sample_metadata/model/meta_search_entity_prefix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/nested_family.py` & `sample_metadata-5.6.1/sample_metadata/model/nested_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/nested_participant.py` & `sample_metadata-5.6.1/sample_metadata/model/nested_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/nested_sample.py` & `sample_metadata-5.6.1/sample_metadata/model/nested_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/nested_sequence.py` & `sample_metadata-5.6.1/sample_metadata/model/nested_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/new_sample.py` & `sample_metadata-5.6.1/sample_metadata/model/new_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/new_sequence.py` & `sample_metadata-5.6.1/sample_metadata/model/new_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/paging_links.py` & `sample_metadata-5.6.1/sample_metadata/model/paging_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/participant_search_response_data.py` & `sample_metadata-5.6.1/sample_metadata/model/participant_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/participant_update_model.py` & `sample_metadata-5.6.1/sample_metadata/model/participant_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/participant_upsert.py` & `sample_metadata-5.6.1/sample_metadata/model/participant_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/participant_upsert_body.py` & `sample_metadata-5.6.1/sample_metadata/model/participant_upsert_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/project.py` & `sample_metadata-5.6.1/sample_metadata/model/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/project_summary_response.py` & `sample_metadata-5.6.1/sample_metadata/model/project_summary_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/sample_batch_upsert.py` & `sample_metadata-5.6.1/sample_metadata/model/sample_batch_upsert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/sample_batch_upsert_body.py` & `sample_metadata-5.6.1/sample_metadata/model/sample_batch_upsert_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/sample_search_response_data.py` & `sample_metadata-5.6.1/sample_metadata/model/sample_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/sample_type.py` & `sample_metadata-5.6.1/sample_metadata/model/sample_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/sample_update_model.py` & `sample_metadata-5.6.1/sample_metadata/model/sample_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/search_item.py` & `sample_metadata-5.6.1/sample_metadata/model/search_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/search_response.py` & `sample_metadata-5.6.1/sample_metadata/model/search_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/search_response_model.py` & `sample_metadata-5.6.1/sample_metadata/model/search_response_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/search_response_type.py` & `sample_metadata-5.6.1/sample_metadata/model/search_response_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/sequence_status.py` & `sample_metadata-5.6.1/sample_metadata/model/sequence_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/sequence_technology.py` & `sample_metadata-5.6.1/sample_metadata/model/sequence_technology.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/sequence_type.py` & `sample_metadata-5.6.1/sample_metadata/model/sequence_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/sequence_update_model.py` & `sample_metadata-5.6.1/sample_metadata/model/sequence_update_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/sequence_upsert.py` & `sample_metadata-5.6.1/sample_metadata/model/sequence_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/validation_error.py` & `sample_metadata-5.6.1/sample_metadata/model/validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model/web_project.py` & `sample_metadata-5.6.1/sample_metadata/model/web_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `sample_metadata-5.6.0/sample_metadata/model_utils.py` & `sample_metadata-5.6.1/sample_metadata/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `sample_metadata-5.6.0/sample_metadata/models/__init__.py` & `sample_metadata-5.6.1/sample_metadata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/sample_metadata/parser/cloudhelper.py` & `sample_metadata-5.6.1/sample_metadata/parser/cloudhelper.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/sample_metadata/parser/generic_metadata_parser.py` & `sample_metadata-5.6.1/sample_metadata/parser/generic_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/sample_metadata/parser/generic_parser.py` & `sample_metadata-5.6.1/sample_metadata/parser/generic_parser.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/sample_metadata/parser/sample_file_map_parser.py` & `sample_metadata-5.6.1/sample_metadata/parser/sample_file_map_parser.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/sample_metadata/rest.py` & `sample_metadata-5.6.1/sample_metadata/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 5.6.0
+    The version of the OpenAPI document: 5.6.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `sample_metadata-5.6.0/sample_metadata.egg-info/PKG-INFO` & `sample_metadata-5.6.1/sample_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample-metadata
-Version: 5.6.0
+Version: 5.6.1
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sample_metadata-5.6.0/sample_metadata.egg-info/SOURCES.txt` & `sample_metadata-5.6.1/sample_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/setup.py` & `sample_metadata-5.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='5.6.0',
+    version='5.6.1',
     description='Python API for interacting with the Sample API system',
     long_description=readme,
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/sample-metadata',
     license='MIT',
     packages=all_packages,
     install_requires=[
```

### Comparing `sample_metadata-5.6.0/test/test_add_samples_for_joint_calling.py` & `sample_metadata-5.6.1/test/test_add_samples_for_joint_calling.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/test_analysis.py` & `sample_metadata-5.6.1/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/test_get_participants.py` & `sample_metadata-5.6.1/test/test_get_participants.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/test_import_individual_metadata.py` & `sample_metadata-5.6.1/test/test_import_individual_metadata.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/test_joint_calling_workflow.py` & `sample_metadata-5.6.1/test/test_joint_calling_workflow.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/test_parse_file_map.py` & `sample_metadata-5.6.1/test/test_parse_file_map.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/test_parse_generic_metadata.py` & `sample_metadata-5.6.1/test/test_parse_generic_metadata.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/test_parse_ont_processor.py` & `sample_metadata-5.6.1/test/test_parse_ont_processor.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/test_parse_ont_sheet.py` & `sample_metadata-5.6.1/test/test_parse_ont_sheet.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/test_pedigree.py` & `sample_metadata-5.6.1/test/test_pedigree.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/test_sample.py` & `sample_metadata-5.6.1/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/test_search.py` & `sample_metadata-5.6.1/test/test_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from db.python.layers.participant import ParticipantLayer
 from db.python.layers.sample import SampleLayer
 from db.python.layers.search import SearchLayer
 from db.python.layers.family import FamilyLayer
 from db.python.tables.family_participant import FamilyParticipantTable
 
 from models.enums import SampleType, SearchResponseType
+from models.models.family import PedRowInternal
 from models.models.sample import sample_id_format
 
 
 class TestSample(DbIsolatedTest):
     """Test sample class"""
 
     # tests run in 'sorted by ascii' order
@@ -120,22 +121,22 @@
         """Create a number of resources, and search for all of them"""
         fptable = FamilyParticipantTable(self.connection)
 
         p_id = await self.player.create_participant(external_id='X:PART01')
         f_id = await self.flayer.create_family(external_id='X:FAM01')
         await fptable.create_rows(
             [
-                {
-                    'family_id': f_id,
-                    'participant_id': p_id,
-                    'paternal_participant_id': None,
-                    'maternal_participant_id': None,
-                    'affected': 0,
-                    'notes': None,
-                }
+                PedRowInternal(
+                    family_id=f_id,
+                    participant_id=p_id,
+                    paternal_id=None,
+                    maternal_id=None,
+                    affected=0,
+                    notes=None,
+                )
             ]
         )
 
         s_id = await self.slayer.insert_sample(
             'X:SAM001', SampleType.BLOOD, participant_id=p_id
         )
```

### Comparing `sample_metadata-5.6.0/test/test_sequence.py` & `sample_metadata-5.6.1/test/test_sequence.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/test_upsert.py` & `sample_metadata-5.6.1/test/test_upsert.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/test_web.py` & `sample_metadata-5.6.1/test/test_web.py`

 * *Files identical despite different names*

### Comparing `sample_metadata-5.6.0/test/testbase.py` & `sample_metadata-5.6.1/test/testbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,17 +130,18 @@
                     author='testuser',
                 )
                 cls.connections[cls.__name__] = connection
 
                 ppt = ProjectPermissionsTable(
                     connection.connection, allow_full_access=True
                 )
-                await ppt.create_project(
-                    project_name='test',
-                    dataset_name='test',
+                cls.project_name = 'test'
+                cls.project_id = await ppt.create_project(
+                    project_name=cls.project_name,
+                    dataset_name=cls.project_name,
                     create_test_project=False,
                     author='testuser',
                     read_group_name='None',
                     write_group_name='None',
                     check_permissions=False,
                 )
 
@@ -166,14 +167,15 @@
         db = cls.dbs.get(cls.__name__)
         if db:
             db.exec(f'DROP DATABASE {db.MYSQL_DATABASE};')
             db.stop()
 
     def setUp(self) -> None:
         self.project_id = 1
+        self.project_name = 'test'
         self.connection = self.connections[self.__class__.__name__]
 
 
 class DbIsolatedTest(DbTest):
     """
     Database integration tests that performs clean-up at the start of each test
     """
```

