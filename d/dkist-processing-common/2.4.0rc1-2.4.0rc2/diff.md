# Comparing `tmp/dkist-processing-common-2.4.0rc1.tar.gz` & `tmp/dkist-processing-common-2.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-2.4.0rc1.tar", last modified: Fri Mar 10 17:45:44 2023, max compression
+gzip compressed data, was "dkist-processing-common-2.4.0rc2.tar", last modified: Mon Apr 10 20:18:37 2023, max compression
```

## Comparing `dkist-processing-common-2.4.0rc1.tar` & `dkist-processing-common-2.4.0rc2.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.111721 dkist-processing-common-2.4.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    11208 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-03-10 17:45:44.111721 dkist-processing-common-2.4.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.103721 dkist-processing-common-2.4.0rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/changelog/129.misc.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.103721 dkist-processing-common-2.4.0rc1/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.103721 dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.107721 dkist-processing-common-2.4.0rc1/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6987 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.107721 dkist-processing-common-2.4.0rc1/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4959 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3304 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/models/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2156 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     2017 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/models/spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)     7365 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.107721 dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6264 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5598 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.107721 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11470 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     8152 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10675 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.111721 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6718 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13155 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.111721 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8226 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    46378 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     7127 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)    17272 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.111721 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     9758 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_l1_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10499 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    35262 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11128 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    13919 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.103721 dkist-processing-common-2.4.0rc1/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-03-10 17:45:44.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4266 2023-03-10 17:45:44.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-10 17:45:44.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      585 2023-03-10 17:45:44.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-03-10 17:45:44.000000 dkist-processing-common-2.4.0rc1/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.111721 dkist-processing-common-2.4.0rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-10 17:45:44.111721 dkist-processing-common-2.4.0rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1671 2023-03-10 17:45:44.115721 dkist-processing-common-2.4.0rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-03-10 17:45:38.000000 dkist-processing-common-2.4.0rc1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.878137 dkist-processing-common-2.4.0rc2/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11208 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-04-10 20:18:37.878137 dkist-processing-common-2.4.0rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.866137 dkist-processing-common-2.4.0rc2/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/changelog/129.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.866137 dkist-processing-common-2.4.0rc2/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.870137 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.870137 dkist-processing-common-2.4.0rc2/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6987 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.870137 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4959 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3304 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     2017 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/spectral_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     7365 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.874137 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6264 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5598 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.874137 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11470 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     8152 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10675 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.874137 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6718 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13155 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.874137 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8226 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47853 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     7127 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    17272 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.878137 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     9758 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_l1_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10499 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36040 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_spectral_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11128 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    13919 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.870137 dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-04-10 20:18:37.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4266 2023-04-10 20:18:37.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-10 20:18:37.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      585 2023-04-10 20:18:37.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-10 20:18:37.000000 dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.878137 dkist-processing-common-2.4.0rc2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 20:18:37.878137 dkist-processing-common-2.4.0rc2/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-04-10 20:18:37.878137 dkist-processing-common-2.4.0rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-10 20:18:32.000000 dkist-processing-common-2.4.0rc2/setup.py
```

### Comparing `dkist-processing-common-2.4.0rc1/.gitignore` & `dkist-processing-common-2.4.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/.pre-commit-config.yaml` & `dkist-processing-common-2.4.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/CHANGELOG.rst` & `dkist-processing-common-2.4.0rc2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/PKG-INFO` & `dkist-processing-common-2.4.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.4.0rc1
+Version: 2.4.0rc2
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.4.0rc1/README.rst` & `dkist-processing-common-2.4.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/bitbucket-pipelines.yml` & `dkist-processing-common-2.4.0rc2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/check_changelog_updated.sh` & `dkist-processing-common-2.4.0rc2/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/config.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/constants.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/_util/tags.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/manual.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/models/constants.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/models/graphql.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/models/json_encoder.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/models/message.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/models/parameters.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/models/quality.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/quality.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     A Quality Report is made up of a list of metrics with the schema defined by this class.
 
     Additionally, this class can produce a Flowable or List of Flowables to be render the metric in the PDF Report
     """
 
     name: str
     description: str
-    statement: str | None = None
-    plot_data: Plot2D | None = None
-    histogram_data: PlotHistogram | None = None
-    table_data: SimpleTable | None = None
+    statement: str | list[str] | None = None
+    plot_data: Plot2D | list[Plot2D] | None = None
+    histogram_data: PlotHistogram | list[PlotHistogram] | None = None
+    table_data: SimpleTable | list[SimpleTable] | None = None
     modmat_data: ModulationMatrixHistograms | None = None
     efficiency_data: EfficiencyHistograms | None = None
     raincloud_data: PlotRaincloud | None = None
     warnings: list[str] | None = None
```

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/models/spectral_line.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/spectral_line.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/models/tags.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/time.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/base.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -882,75 +882,111 @@
         First, flatten FOV bins dimensions, compute modulation matrices, and record I_sys for all bins.
 
         Then convert to python lists for serialization and write to disk.
         """
         ## Modulation matrices
         fov_shape = polcal_fitter.local_objects.dresser.shape
         num_mod = polcal_fitter.local_objects.dresser.nummod
+        num_steps = polcal_fitter.local_objects.dresser.numsteps
         flattened_demod = np.reshape(
             polcal_fitter.demodulation_matrices, (np.prod(fov_shape), 4, num_mod)
         )
         flattened_mod = np.zeros((np.prod(fov_shape), num_mod, 4))
         for i in range(flattened_demod.shape[0]):
             flattened_mod[i] = np.linalg.pinv(flattened_demod[i])
 
         # Move axis so numpoints is the last dimension, which will be easier to understand when
         # plotting
         flattened_mod = np.moveaxis(flattened_mod, 0, -1)
 
         # Because ndarrays can't be Json'd
         mod_list = flattened_mod.tolist()
 
-        ## I_sys
-        I_sys_list = []
-        for point_params in polcal_fitter.local_objects.fit_parameters._all_parameters:
-            for s in range(polcal_fitter.local_objects.dresser.numsteps):
-                I_sys_list.append(point_params[f"I_sys_CS00_step{s:02n}"].value)
-
-        # Get the starting value of I_sys, which is just I_clear
-        # Take the first element because this is a Polcal (not Groupcal) and so there is only
-        # a single Drawer
-        I_sys_init = polcal_fitter.local_objects.dresser.I_clear[0]
+        # Now get the rest of the free variables
+        fit_params = polcal_fitter.local_objects.fit_parameters
+        init_param = polcal_fitter.local_objects.init_parameters
+        param_metadata = fit_params.first_parameters
+
+        free_param_data = dict()
+        for param in param_metadata.keys():
+            # Don't grab modulation matrix values because we got those above.
+            # Also don't grab any parameters that were fixed.
+            if "modmat" in param or not param_metadata[param].vary:
+                continue
+
+            fit_value_list = []
+            for point_param in fit_params._all_parameters:
+                fit_value_list.append(point_param[param].value)
+
+            init_value = init_param.first_parameters[param].value
+
+            free_param_data[param] = {"fit_values": fit_value_list, "init_value": init_value}
 
         data = {
             "task_type": label,
             "bin_1_str": f"{bins_1} {bin_1_type}",
             "bin_2_str": f"{bins_2} {bin_2_type}",
             "total_bins": bins_1 * bins_2,
+            "num_steps": num_steps,
             "modmat_list": mod_list,
-            "I_sys_list": I_sys_list,
-            "I_sys_init": I_sys_init,
+            "free_param_dict": free_param_data,
         }
         self._record_values(
             values=data, tags=[Tag.quality("POLCAL_LOCAL_PAR_VALS"), Tag.quality_task(label)]
         )
 
     def quality_build_polcal_local_parameter_values(self, label: str) -> dict:
         """Build a modulation matrix and I_sys histograms schema from stored data."""
         data_file = next(
             self.read(tags=[Tag.quality("POLCAL_LOCAL_PAR_VALS"), Tag.quality_task(label)])
         )
         with data_file.open() as f:
             data = json.load(f)
 
         modmat_hist = ModulationMatrixHistograms(modmat_list=data["modmat_list"])
+        free_param_dict = data["free_param_dict"]
+        I_sys_series_data = dict()
+        I_sys_vertical_lines = dict()
+        for step in range(data["num_steps"]):
+            I_sys_series_data[f"CS step {step}"] = free_param_dict[f"I_sys_CS00_step{step:02n}"][
+                "fit_values"
+            ]
+            if step == 0:
+                I_sys_vertical_lines["init value"] = free_param_dict[f"I_sys_CS00_step{step:02n}"][
+                    "init_value"
+                ]
+
         I_sys_hist = PlotHistogram(
-            xlabel="I_sys",
-            series_data={"I_sys": data["I_sys_list"]},
-            vertical_lines={"I_clear": data["I_sys_init"]},
+            xlabel="I_sys", series_data=I_sys_series_data, vertical_lines=I_sys_vertical_lines
         )
+
+        param_histograms = [I_sys_hist]
+        for param, param_data in free_param_dict.items():
+            if "I_sys" in param:
+                # We already dealt with I_sys above
+                continue
+
+            plot_name = param.replace("_CS00", "")
+            hist = PlotHistogram(
+                xlabel=plot_name,
+                series_data={plot_name: param_data["fit_values"]},
+                vertical_lines={"init value": param_data["init_value"]},
+            )
+            param_histograms.append(hist)
+
         metric = ReportMetric(
             name=f"PolCal Local Bin Fits - {label}",
-            description=f"The first panel shows histograms of the individual modulation matrix elements. "
+            description=f"The first plot shows histograms of the individual modulation matrix elements. "
             "Note that the first element is not shown because it is always fixed to 1 in fits. "
-            "The second shows the corresponding fits of I_sys, the overall flux scaling. "
+            "Subsequent plots show the distribution of all other free parameters in the fit, along with their initial "
+            "values. For I_sys there is a separate fit value for each CS step."
             f"There are {data['total_bins']} samples spanning {data['bin_1_str']} "
             f"and {data['bin_2_str']} bins.",
             modmat_data=modmat_hist,
-            histogram_data=I_sys_hist,
+            histogram_data=param_histograms,
         )
         return metric.dict()
 
     def _store_polcal_fit_resdiuals(
         self,
         *,
         polcal_fitter: PolcalFitter,
```

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_l1_output_data_base.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_l1_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -690,23 +690,25 @@
         local_par_dict = json.load(f)
         assert sorted(local_par_dict.keys()) == sorted(
             [
                 "task_type",
                 "bin_1_str",
                 "bin_2_str",
                 "total_bins",
+                "num_steps",
                 "modmat_list",
-                "I_sys_list",
-                "I_sys_init",
+                "free_param_dict",
             ]
         )
         assert local_par_dict["task_type"] == label
         assert type(local_par_dict["total_bins"]) == int
-        assert type(local_par_dict["modmat_list"]) == type(local_par_dict["I_sys_list"]) == list
-        assert type(local_par_dict["I_sys_init"]) == float
+        assert type(local_par_dict["modmat_list"]) == list
+        assert type(local_par_dict["free_param_dict"]) == dict
+        assert type(local_par_dict["free_param_dict"]["I_sys_CS00_step00"]["init_value"]) == float
+        assert type(local_par_dict["free_param_dict"]["I_sys_CS00_step00"]["fit_values"]) == list
 
     # Fit residuals
     fit_res_file = list(
         quality_task.read(tags=[Tag.quality("POLCAL_FIT_RESIDUALS"), Tag.quality_task(label)])
     )
     assert len(fit_res_file) == 1
     with open(fit_res_file[0], "r") as f:
@@ -836,17 +838,21 @@
 def polcal_local_params_json():
     label = "Beam 1"
     data = {
         "task_type": label,
         "bin_1_str": "2 spatial",
         "bin_2_str": "3 radical",
         "total_bins": 6,
+        "num_steps": 2,
         "modmat_list": [[[1, 2.0], [2.0, 3.0]], [[10.0, 20.0], [20.0, 30.0]]],
-        "I_sys_list": [1, 2, 3],
-        "I_sys_init": 6.28,
+        "free_param_dict": {
+            "I_sys_CS00_step00": {"fit_values": [1, 2, 3.0], "init_value": 0.3},
+            "I_sys_CS00_step01": {"fit_values": [10, 20, 30.0], "init_value": 0.33},
+            "param_X": {"fit_values": [5, 6, 7.0], "init_value": 99},
+        },
     }
 
     return json.dumps(data, allow_nan=False, cls=QualityValueEncoder).encode(), label
 
 
 def test_polcal_build_local_parameter_values(quality_task, polcal_local_params_json):
     """
@@ -857,18 +863,25 @@
     data, label = polcal_local_params_json
     quality_task.write(data, tags=[Tag.quality("POLCAL_LOCAL_PAR_VALS"), Tag.quality_task(label)])
     metric = quality_task.quality_build_polcal_local_parameter_values(label=label)
 
     assert metric["name"] == f"PolCal Local Bin Fits - {label}"
     modmat_data = metric["modmat_data"]
     assert modmat_data["modmat_list"] == [[[1, 2.0], [2.0, 3.0]], [[10.0, 20.0], [20.0, 30.0]]]
-    I_sys_data = metric["histogram_data"]
-    assert I_sys_data["xlabel"] == "I_sys"
-    assert I_sys_data["series_data"] == {"I_sys": [1, 2, 3]}
-    assert I_sys_data["vertical_lines"] == {"I_clear": 6.28}
+    hist_list = metric["histogram_data"]
+    assert isinstance(hist_list, list)
+    for hist_data in hist_list:
+        if hist_data["xlabel"] == "I_sys":
+            assert hist_data["xlabel"] == "I_sys"
+            assert hist_data["series_data"] == {"CS step 0": [1, 2, 3], "CS step 1": [10, 20, 30]}
+            assert hist_data["vertical_lines"] == {"init value": 0.3}
+        else:
+            assert hist_data["xlabel"] == "param_X"
+            assert hist_data["series_data"] == {"param_X": [5, 6, 7]}
+            assert hist_data["vertical_lines"] == {"init value": 99}
 
 
 @pytest.fixture
 def polcal_fit_residuals_json():
     label = "Beam 1"
     data = {
         "task_type": label,
```

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_spectral_line.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_spectral_line.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-2.4.0rc2/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.4.0rc1
+Version: 2.4.0rc2
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-2.4.0rc2/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/docs/Makefile` & `dkist-processing-common-2.4.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/docs/conf.py` & `dkist-processing-common-2.4.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/docs/make.bat` & `dkist-processing-common-2.4.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/licenses/LICENSE.rst` & `dkist-processing-common-2.4.0rc2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/pyproject.toml` & `dkist-processing-common-2.4.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.0rc1/setup.cfg` & `dkist-processing-common-2.4.0rc2/setup.cfg`

 * *Files identical despite different names*

