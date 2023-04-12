# Comparing `tmp/pyrefinebio-0.4.8.tar.gz` & `tmp/pyrefinebio-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrefinebio-0.4.8.tar", last modified: Tue Oct 26 18:15:05 2021, max compression
+gzip compressed data, was "pyrefinebio-0.4.9.tar", last modified: Tue Jan 18 20:31:51 2022, max compression
```

## Comparing `pyrefinebio-0.4.8.tar` & `pyrefinebio-0.4.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 18:15:05.868046 pyrefinebio-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2021-10-26 18:15:05.868046 pyrefinebio-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2136 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 18:15:05.864046 pyrefinebio-0.4.8/pyrefinebio/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/annotation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3800 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/api_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4335 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/compendia.py
--rw-r--r--   0 runner    (1001) docker     (121)     2843 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/computational_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     5895 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/computed_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2444 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     9491 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5889 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)     9346 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/high_level_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/institution.py
--rw-r--r--   0 runner    (1001) docker     (121)    11674 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/job.py
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/organism.py
--rw-r--r--   0 runner    (1001) docker     (121)     4520 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/original_file.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/platform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2084 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/qn_target.py
--rw-r--r--   0 runner    (1001) docker     (121)     7659 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/sample.py
--rw-r--r--   0 runner    (1001) docker     (121)     6314 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/script.py
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/token.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/transcriptome_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     3061 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/pyrefinebio/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 18:15:05.864046 pyrefinebio-0.4.8/pyrefinebio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2021-10-26 18:15:05.000000 pyrefinebio-0.4.8/pyrefinebio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2021-10-26 18:15:05.000000 pyrefinebio-0.4.8/pyrefinebio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-26 18:15:05.000000 pyrefinebio-0.4.8/pyrefinebio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-10-26 18:15:05.000000 pyrefinebio-0.4.8/pyrefinebio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-10-26 18:15:05.000000 pyrefinebio-0.4.8/pyrefinebio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-10-26 18:15:05.000000 pyrefinebio-0.4.8/pyrefinebio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      504 2021-10-26 18:15:05.868046 pyrefinebio-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      964 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 18:15:05.868046 pyrefinebio-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/custom_assertions.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_api_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     5084 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_compendia.py
--rw-r--r--   0 runner    (1001) docker     (121)     5623 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_computational_result.py
--rw-r--r--   0 runner    (1001) docker     (121)    12342 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_computed_file.py
--rw-r--r--   0 runner    (1001) docker     (121)    11716 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     4491 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_downloader_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     5407 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)     8175 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_high_level_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)      950 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_institution.py
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_organism.py
--rw-r--r--   0 runner    (1001) docker     (121)     7034 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_original_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     7425 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_platform.py
--rw-r--r--   0 runner    (1001) docker     (121)     2918 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4306 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_processor_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     4348 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_qn_target.py
--rw-r--r--   0 runner    (1001) docker     (121)    17962 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (121)     5427 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (121)     3041 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_survey_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     3520 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2021-10-26 18:14:50.000000 pyrefinebio-0.4.8/tests/test_transcriptome_index.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 20:31:51.983289 pyrefinebio-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2637 2022-01-18 20:31:51.983289 pyrefinebio-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 20:31:51.979289 pyrefinebio-0.4.9/pyrefinebio/
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3800 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/api_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4335 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/compendia.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2843 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/computational_result.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5895 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/computed_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2444 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9491 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5889 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9346 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/high_level_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/institution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11674 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/organism.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4520 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/original_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/platform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/qn_target.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8464 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/sample.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6314 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/script.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3439 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/token.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/transcriptome_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3061 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/pyrefinebio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 20:31:51.979289 pyrefinebio-0.4.9/pyrefinebio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2637 2022-01-18 20:31:51.000000 pyrefinebio-0.4.9/pyrefinebio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-01-18 20:31:51.000000 pyrefinebio-0.4.9/pyrefinebio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-18 20:31:51.000000 pyrefinebio-0.4.9/pyrefinebio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-01-18 20:31:51.000000 pyrefinebio-0.4.9/pyrefinebio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-01-18 20:31:51.000000 pyrefinebio-0.4.9/pyrefinebio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-18 20:31:51.000000 pyrefinebio-0.4.9/pyrefinebio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2022-01-18 20:31:51.983289 pyrefinebio-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-18 20:31:51.983289 pyrefinebio-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/custom_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_api_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5084 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_compendia.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5623 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_computational_result.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12342 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_computed_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11716 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4491 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_downloader_job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5407 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8175 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_high_level_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_institution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_organism.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7034 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_original_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7425 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2918 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4306 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_processor_job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4348 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_qn_target.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17962 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5427 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3041 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_survey_job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3520 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-01-18 20:31:43.000000 pyrefinebio-0.4.9/tests/test_transcriptome_index.py
```

### Comparing `pyrefinebio-0.4.8/LICENSE` & `pyrefinebio-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/PKG-INFO` & `pyrefinebio-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrefinebio
-Version: 0.4.8
+Version: 0.4.9
 Summary: A python client for the refine.bio API.
 Home-page: https://github.com/AlexsLemonade/refinebio-py
 Author: Childhood Cancer Data Lab
 Author-email: ccdl@alexslemonade.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrefinebio-0.4.8/README.md` & `pyrefinebio-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/__init__.py` & `pyrefinebio-0.4.9/pyrefinebio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/api_interface.py` & `pyrefinebio-0.4.9/pyrefinebio/api_interface.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/base.py` & `pyrefinebio-0.4.9/pyrefinebio/base.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/compendia.py` & `pyrefinebio-0.4.9/pyrefinebio/compendia.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/computational_result.py` & `pyrefinebio-0.4.9/pyrefinebio/computational_result.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/computed_file.py` & `pyrefinebio-0.4.9/pyrefinebio/computed_file.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/config.py` & `pyrefinebio-0.4.9/pyrefinebio/config.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/dataset.py` & `pyrefinebio-0.4.9/pyrefinebio/dataset.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/exceptions.py` & `pyrefinebio-0.4.9/pyrefinebio/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/experiment.py` & `pyrefinebio-0.4.9/pyrefinebio/experiment.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/high_level_functions.py` & `pyrefinebio-0.4.9/pyrefinebio/high_level_functions.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/institution.py` & `pyrefinebio-0.4.9/pyrefinebio/institution.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/job.py` & `pyrefinebio-0.4.9/pyrefinebio/job.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/organism.py` & `pyrefinebio-0.4.9/pyrefinebio/organism.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/original_file.py` & `pyrefinebio-0.4.9/pyrefinebio/original_file.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/platform.py` & `pyrefinebio-0.4.9/pyrefinebio/platform.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/processor.py` & `pyrefinebio-0.4.9/pyrefinebio/processor.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/qn_target.py` & `pyrefinebio-0.4.9/pyrefinebio/qn_target.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/sample.py` & `pyrefinebio-0.4.9/pyrefinebio/sample.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pyrefinebio import (
     annotation as prb_annotation,
     computational_result as prb_computational_result,
     computed_file as prb_computed_file,
     experiment as prb_experiment,
     organism as prb_organism,
     original_file as prb_original_file,
+    job as prb_job,
 )
 from pyrefinebio.api_interface import get_by_endpoint
 from pyrefinebio.base import Base
 from pyrefinebio.util import create_paginated_list, parse_date
 
 
 class Sample(Base):
@@ -52,20 +53,25 @@
         cell_line=None,
         treatment=None,
         race=None,
         subject=None,
         compound=None,
         time=None,
         is_processed=None,
+        is_unable_to_be_processed=None,
         created_at=None,
         last_modified=None,
         contributed_metadata=None,
         contributed_keywords=None,
         original_files=[],
         computed_files=[],
+        last_processor_job=None,
+        last_downloader_job=None,
+        most_recent_smashable_file=None,
+        most_recent_quant_file=None,
         experiment_accession_codes=None,
         experiments=None,
     ):
         super().__init__(identifier=accession_code)
 
         self.id = id
         self.title = title
@@ -99,14 +105,15 @@
         self.cell_line = cell_line
         self.treatment = treatment
         self.race = race
         self.subject = subject
         self.compound = compound
         self.time = time
         self.is_processed = is_processed
+        self.is_unable_to_be_processed = is_unable_to_be_processed
         self.created_at = parse_date(created_at)
         self.last_modified = parse_date(last_modified)
         self.contributed_metadata = contributed_metadata
 
         self.original_files = (
             [prb_original_file.OriginalFile(id=file_id) for file_id in original_files]
             if original_files
@@ -114,14 +121,23 @@
         )
         self.computed_files = (
             [prb_computed_file.ComputedFile(id=file_id) for file_id in computed_files]
             if computed_files
             else []
         )
 
+        # this isn't populated yet but the api does include these keys in the response
+        # so for now let's just try to apply them
+        if last_processor_job:
+            self.last_processor_job = prb_job.ProcessorJob(**last_processor_job)
+        if last_downloader_job:
+            self.last_downloader_job = prb_job.DownloaderJob(**last_downloader_job)
+
+        self.most_recent_smashable_file = most_recent_smashable_file
+        self.most_recent_quant_file = most_recent_quant_file
         self.experiment_accession_codes = experiment_accession_codes
         self.experiments = experiments
 
         # Avoid initializing every Sample with the sample empty list as a default
         if not contributed_keywords:
             contributed_keywords = []
 
@@ -159,15 +175,17 @@
             list of Sample
 
         Keyword Arguments:
             ordering (str): which field to use when ordering the results
 
             title (str): filter based on the Sample's title
 
-            organism (str): filter based on the Organism that the Sample was taken from
+            organism__name (str): filter based on the Organism that the Sample was taken from
+
+            organism__taxonomy_id (int): filter based on the Organism that the Sample was taken from
 
             source_database (str): filter based on the publically available repository
                                    that the Sample was taken from
 
             source_archive_url (str): filter based on Sample's source url
 
             has_raw (bool): filter based on if the Sample had raw data available in the source database
@@ -200,16 +218,14 @@
 
             compound (str): filter based on the compound information provided by the submitter
 
             time (str): filter based on the time information provided by the submitter
 
             is_processed (bool): filter based on if the Sample has been processed
 
-            is_public (bool): filter based on if the Sample is public
-
             limit (int): number of results to return per page.
 
             offset (int): the initial index from which to return the results.
 
             dataset_id (str): filter based on the Dataset ids that the Sample has been added to
 
             experiment_accession_code (str): filter based on the Experiments that are associated
```

### Comparing `pyrefinebio-0.4.8/pyrefinebio/script.py` & `pyrefinebio-0.4.9/pyrefinebio/script.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/token.py` & `pyrefinebio-0.4.9/pyrefinebio/token.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/transcriptome_index.py` & `pyrefinebio-0.4.9/pyrefinebio/transcriptome_index.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio/util.py` & `pyrefinebio-0.4.9/pyrefinebio/util.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/pyrefinebio.egg-info/PKG-INFO` & `pyrefinebio-0.4.9/pyrefinebio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrefinebio
-Version: 0.4.8
+Version: 0.4.9
 Summary: A python client for the refine.bio API.
 Home-page: https://github.com/AlexsLemonade/refinebio-py
 Author: Childhood Cancer Data Lab
 Author-email: ccdl@alexslemonade.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrefinebio-0.4.8/pyrefinebio.egg-info/SOURCES.txt` & `pyrefinebio-0.4.9/pyrefinebio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/setup.py` & `pyrefinebio-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/custom_assertions.py` & `pyrefinebio-0.4.9/tests/custom_assertions.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_api_interface.py` & `pyrefinebio-0.4.9/tests/test_api_interface.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_compendia.py` & `pyrefinebio-0.4.9/tests/test_compendia.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_computational_result.py` & `pyrefinebio-0.4.9/tests/test_computational_result.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_computed_file.py` & `pyrefinebio-0.4.9/tests/test_computed_file.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_dataset.py` & `pyrefinebio-0.4.9/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_downloader_job.py` & `pyrefinebio-0.4.9/tests/test_downloader_job.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_experiment.py` & `pyrefinebio-0.4.9/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_high_level_functions.py` & `pyrefinebio-0.4.9/tests/test_high_level_functions.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_institution.py` & `pyrefinebio-0.4.9/tests/test_institution.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_organism.py` & `pyrefinebio-0.4.9/tests/test_organism.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_original_file.py` & `pyrefinebio-0.4.9/tests/test_original_file.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_paginated_list.py` & `pyrefinebio-0.4.9/tests/test_paginated_list.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_platform.py` & `pyrefinebio-0.4.9/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_processor.py` & `pyrefinebio-0.4.9/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_processor_job.py` & `pyrefinebio-0.4.9/tests/test_processor_job.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_qn_target.py` & `pyrefinebio-0.4.9/tests/test_qn_target.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_sample.py` & `pyrefinebio-0.4.9/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_script.py` & `pyrefinebio-0.4.9/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_survey_job.py` & `pyrefinebio-0.4.9/tests/test_survey_job.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_token.py` & `pyrefinebio-0.4.9/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `pyrefinebio-0.4.8/tests/test_transcriptome_index.py` & `pyrefinebio-0.4.9/tests/test_transcriptome_index.py`

 * *Files identical despite different names*

