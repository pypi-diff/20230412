# Comparing `tmp/hopsworks-3.1.1rc2.tar.gz` & `tmp/hopsworks-3.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hopsworks-3.1.1rc2.tar", last modified: Thu Mar 30 07:03:49 2023, max compression
+gzip compressed data, was "hopsworks-3.2.0rc0.tar", last modified: Wed Apr 12 12:52:06 2023, max compression
```

## Comparing `hopsworks-3.1.1rc2.tar` & `hopsworks-3.2.0rc0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0     1006     1006        0 2023-03-30 07:03:49.122461 hopsworks-3.1.1rc2/
--rw-r--r--   0     1006     1006       40 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/MANIFEST.in
--rw-r--r--   0     1006     1006     3473 2023-03-30 07:03:49.122461 hopsworks-3.1.1rc2/PKG-INFO
--rw-r--r--   0     1006     1006     2061 2023-03-30 07:03:47.000000 hopsworks-3.1.1rc2/README.md
-drwxr-xr-x   0     1006     1006        0 2023-03-30 07:03:49.110461 hopsworks-3.1.1rc2/hopsworks/
--rw-r--r--   0     1006     1006    11010 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-03-30 07:03:49.114461 hopsworks-3.1.1rc2/hopsworks/client/
--rw-r--r--   0     1006     1006     1552 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/client/__init__.py
--rw-r--r--   0     1006     1006     1132 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/client/auth.py
--rw-r--r--   0     1006     1006     6523 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/client/base.py
--rw-r--r--   0     1006     1006     2308 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/client/exceptions.py
--rw-r--r--   0     1006     1006     5553 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/client/external.py
--rw-r--r--   0     1006     1006     8091 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/client/hopsworks.py
--rw-r--r--   0     1006     1006     1493 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/command.py
--rw-r--r--   0     1006     1006    12072 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/connection.py
--rw-r--r--   0     1006     1006     4461 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/constants.py
-drwxr-xr-x   0     1006     1006        0 2023-03-30 07:03:49.118461 hopsworks-3.1.1rc2/hopsworks/core/
--rw-r--r--   0     1006     1006      605 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/__init__.py
--rw-r--r--   0     1006     1006     9121 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/dataset_api.py
--rw-r--r--   0     1006     1006     3639 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/environment_api.py
--rw-r--r--   0     1006     1006     2502 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/execution_api.py
--rw-r--r--   0     1006     1006    15858 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/git_api.py
--rw-r--r--   0     1006     1006     1419 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/git_op_execution_api.py
--rw-r--r--   0     1006     1006     3289 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/git_provider_api.py
--rw-r--r--   0     1006     1006     3673 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/git_remote_api.py
--rw-r--r--   0     1006     1006     5644 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/job_api.py
--rw-r--r--   0     1006     1006    11477 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/kafka_api.py
--rw-r--r--   0     1006     1006     1602 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/library_api.py
--rw-r--r--   0     1006     1006     2984 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/opensearch_api.py
--rw-r--r--   0     1006     1006     3441 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/project_api.py
--rw-r--r--   0     1006     1006     3890 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/secret_api.py
--rw-r--r--   0     1006     1006     1051 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/core/variable_api.py
--rw-r--r--   0     1006     1006     1651 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/decorators.py
-drwxr-xr-x   0     1006     1006        0 2023-03-30 07:03:49.122461 hopsworks-3.1.1rc2/hopsworks/engine/
--rw-r--r--   0     1006     1006      605 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/engine/__init__.py
--rw-r--r--   0     1006     1006     3504 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/engine/environment_engine.py
--rw-r--r--   0     1006     1006     4835 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/engine/execution_engine.py
--rw-r--r--   0     1006     1006     2025 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/engine/git_engine.py
--rw-r--r--   0     1006     1006     4758 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/environment.py
--rw-r--r--   0     1006     1006     6897 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/execution.py
--rw-r--r--   0     1006     1006     2350 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/git_commit.py
--rw-r--r--   0     1006     1006     2163 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/git_file_status.py
--rw-r--r--   0     1006     1006     3469 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/git_op_execution.py
--rw-r--r--   0     1006     1006     2364 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/git_provider.py
--rw-r--r--   0     1006     1006     2267 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/git_remote.py
--rw-r--r--   0     1006     1006     8756 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/git_repo.py
--rw-r--r--   0     1006     1006     5909 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/job.py
--rw-r--r--   0     1006     1006     2748 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/kafka_schema.py
--rw-r--r--   0     1006     1006     3310 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/kafka_topic.py
--rw-r--r--   0     1006     1006     1649 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/library.py
--rw-r--r--   0     1006     1006     6546 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/project.py
--rw-r--r--   0     1006     1006     2919 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/secret.py
--rw-r--r--   0     1006     1006     2545 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/hopsworks/user.py
--rw-r--r--   0     1006     1006     2830 2023-03-30 07:03:42.000000 hopsworks-3.1.1rc2/hopsworks/util.py
--rw-r--r--   0     1006     1006      631 2023-03-30 07:03:42.000000 hopsworks-3.1.1rc2/hopsworks/version.py
-drwxr-xr-x   0     1006     1006        0 2023-03-30 07:03:49.110461 hopsworks-3.1.1rc2/hopsworks.egg-info/
--rw-r--r--   0     1006     1006     3473 2023-03-30 07:03:48.000000 hopsworks-3.1.1rc2/hopsworks.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     1566 2023-03-30 07:03:49.000000 hopsworks-3.1.1rc2/hopsworks.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2023-03-30 07:03:48.000000 hopsworks-3.1.1rc2/hopsworks.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      331 2023-03-30 07:03:48.000000 hopsworks-3.1.1rc2/hopsworks.egg-info/requires.txt
--rw-r--r--   0     1006     1006       16 2023-03-30 07:03:48.000000 hopsworks-3.1.1rc2/hopsworks.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2023-03-30 07:03:49.122461 hopsworks-3.1.1rc2/setup.cfg
--rw-r--r--   0     1006     1006     1805 2023-03-21 15:14:03.000000 hopsworks-3.1.1rc2/setup.py
-drwxr-xr-x   0     1006     1006        0 2023-03-30 07:03:49.122461 hopsworks-3.1.1rc2/tests/
--rw-r--r--   0     1006     1006      605 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/tests/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-03-30 07:03:49.122461 hopsworks-3.1.1rc2/tests/hopsworks/
--rw-r--r--   0     1006     1006      605 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/tests/hopsworks/__init__.py
--rw-r--r--   0     1006     1006     7564 2023-03-10 13:56:20.000000 hopsworks-3.1.1rc2/tests/hopsworks/test_login.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.399673 hopsworks-3.2.0rc0/
+-rw-r--r--   0     1006     1006       40 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/MANIFEST.in
+-rw-r--r--   0     1006     1006     3473 2023-04-12 12:52:06.399673 hopsworks-3.2.0rc0/PKG-INFO
+-rw-r--r--   0     1006     1006     2061 2023-04-12 12:52:05.000000 hopsworks-3.2.0rc0/README.md
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.391673 hopsworks-3.2.0rc0/hopsworks/
+-rw-r--r--   0     1006     1006    10699 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.395673 hopsworks-3.2.0rc0/hopsworks/client/
+-rw-r--r--   0     1006     1006     1552 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/client/__init__.py
+-rw-r--r--   0     1006     1006     1132 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/client/auth.py
+-rw-r--r--   0     1006     1006     6523 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/client/base.py
+-rw-r--r--   0     1006     1006     2308 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/client/exceptions.py
+-rw-r--r--   0     1006     1006     5553 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/client/external.py
+-rw-r--r--   0     1006     1006     8091 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/client/hopsworks.py
+-rw-r--r--   0     1006     1006     1493 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/command.py
+-rw-r--r--   0     1006     1006    12491 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/connection.py
+-rw-r--r--   0     1006     1006     4461 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/constants.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.395673 hopsworks-3.2.0rc0/hopsworks/core/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/__init__.py
+-rw-r--r--   0     1006     1006    10113 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/dataset_api.py
+-rw-r--r--   0     1006     1006     3639 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/environment_api.py
+-rw-r--r--   0     1006     1006     2502 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/execution_api.py
+-rw-r--r--   0     1006     1006    15858 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/git_api.py
+-rw-r--r--   0     1006     1006     1419 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/git_op_execution_api.py
+-rw-r--r--   0     1006     1006     3289 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/git_provider_api.py
+-rw-r--r--   0     1006     1006     3673 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/git_remote_api.py
+-rw-r--r--   0     1006     1006     5644 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/job_api.py
+-rw-r--r--   0     1006     1006    11477 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/kafka_api.py
+-rw-r--r--   0     1006     1006     1602 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/library_api.py
+-rw-r--r--   0     1006     1006     2984 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/opensearch_api.py
+-rw-r--r--   0     1006     1006     3441 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/project_api.py
+-rw-r--r--   0     1006     1006     3890 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/secret_api.py
+-rw-r--r--   0     1006     1006     1051 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/variable_api.py
+-rw-r--r--   0     1006     1006     1651 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/decorators.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.399673 hopsworks-3.2.0rc0/hopsworks/engine/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/engine/__init__.py
+-rw-r--r--   0     1006     1006     3504 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/engine/environment_engine.py
+-rw-r--r--   0     1006     1006     4835 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/engine/execution_engine.py
+-rw-r--r--   0     1006     1006     2025 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/engine/git_engine.py
+-rw-r--r--   0     1006     1006     4990 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/environment.py
+-rw-r--r--   0     1006     1006     6897 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/execution.py
+-rw-r--r--   0     1006     1006     2350 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/git_commit.py
+-rw-r--r--   0     1006     1006     2163 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/git_file_status.py
+-rw-r--r--   0     1006     1006     3469 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/git_op_execution.py
+-rw-r--r--   0     1006     1006     2364 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/git_provider.py
+-rw-r--r--   0     1006     1006     2267 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/git_remote.py
+-rw-r--r--   0     1006     1006     8756 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/git_repo.py
+-rw-r--r--   0     1006     1006     5909 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/job.py
+-rw-r--r--   0     1006     1006     2748 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/kafka_schema.py
+-rw-r--r--   0     1006     1006     3310 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/kafka_topic.py
+-rw-r--r--   0     1006     1006     1649 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/library.py
+-rw-r--r--   0     1006     1006     6451 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/project.py
+-rw-r--r--   0     1006     1006     2919 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/secret.py
+-rw-r--r--   0     1006     1006     2545 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/user.py
+-rw-r--r--   0     1006     1006     2830 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/util.py
+-rw-r--r--   0     1006     1006      631 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/version.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.395673 hopsworks-3.2.0rc0/hopsworks.egg-info/
+-rw-r--r--   0     1006     1006     3473 2023-04-12 12:52:06.000000 hopsworks-3.2.0rc0/hopsworks.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     1566 2023-04-12 12:52:06.000000 hopsworks-3.2.0rc0/hopsworks.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2023-04-12 12:52:06.000000 hopsworks-3.2.0rc0/hopsworks.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      331 2023-04-12 12:52:06.000000 hopsworks-3.2.0rc0/hopsworks.egg-info/requires.txt
+-rw-r--r--   0     1006     1006       16 2023-04-12 12:52:06.000000 hopsworks-3.2.0rc0/hopsworks.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2023-04-12 12:52:06.399673 hopsworks-3.2.0rc0/setup.cfg
+-rw-r--r--   0     1006     1006     1805 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/setup.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.399673 hopsworks-3.2.0rc0/tests/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/tests/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.399673 hopsworks-3.2.0rc0/tests/hopsworks/
+-rw-r--r--   0     1006     1006      605 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/tests/hopsworks/__init__.py
+-rw-r--r--   0     1006     1006     7564 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/tests/hopsworks/test_login.py
```

### Comparing `hopsworks-3.1.1rc2/PKG-INFO` & `hopsworks-3.2.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hopsworks
-Version: 3.1.1rc2
+Version: 3.2.0rc0
 Summary: HOPSWORKS: An environment independent client to interact with the Hopsworks API
 Home-page: https://github.com/logicalclocks/hopsworks-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/hopsworks-api/releases/tag/3.1.1rc2
+Download-URL: https://github.com/logicalclocks/hopsworks-api/releases/tag/3.2.0rc0
 Description: # Hopsworks Client
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hopsworks Version: 3.1.1rc2 Summary: HOPSWORKS: An
+Metadata-Version: 2.1 Name: hopsworks Version: 3.2.0rc0 Summary: HOPSWORKS: An
 environment independent client to interact with the Hopsworks API Home-page:
 https://github.com/logicalclocks/hopsworks-api Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/hopsworks-api/releases/tag/3.1.1rc2
+https://github.com/logicalclocks/hopsworks-api/releases/tag/3.2.0rc0
 Description: # Hopsworks Client
    [Hopsworks_Community] [Hopsworks_Documentation] [PyPiStatus] [Downloads]
                              [CodeStyle] [License]
 *hopsworks* is the python API for interacting with a Hopsworks cluster. ##
 Getting Started On Hopsworks Instantiate a connection and get the project
 object ```python import hopsworks connection = hopsworks.connection() project =
 connection.get_project("my_project") ``` Create a new project ```python project
```

### Comparing `hopsworks-3.1.1rc2/README.md` & `hopsworks-3.2.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/__init__.py` & `hopsworks-3.2.0rc0/hopsworks/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import hsml  # noqa: F401, E402
 import hsfs  # noqa: F401, E402
 
 __version__ = version.__version__
 
 connection = Connection.connection
 
-_saas_connection = Connection.connection
+_hw_connection = Connection.connection
 
 _connected_project = None
 
 
 def hw_formatwarning(message, category, filename, lineno, line=None):
     return "{}: {}\n".format(category.__name__, message)
 
@@ -100,20 +100,20 @@
     """
 
     global _connected_project
 
     # If already logged in, should reset connection and follow login procedure as Connection may no longer be valid
     logout()
 
-    global _saas_connection
+    global _hw_connection
 
     # If inside hopsworks, just return the current project for now
     if "REST_ENDPOINT" in os.environ:
-        _saas_connection = _saas_connection()
-        _connected_project = _saas_connection.get_project()
+        _hw_connection = _hw_connection()
+        _connected_project = _hw_connection.get_project()
         print("\nLogged in to project, explore it here " + _connected_project.get_url())
         return _connected_project
 
     # This is run for an external client
 
     # Function arguments takes precedence over environment variable.
     # Here we check if environment variable exists and function argument is not set, we use the environment variable.
@@ -161,18 +161,18 @@
         else:
             raise IOError(
                 "Could not find api key file on path: {}".format(api_key_file)
             )
     # If user connected to Serverless Hopsworks, and the cached .hw_api_key exists, then use it.
     elif os.path.exists(api_key_path) and host == "c.app.hopsworks.ai":
         try:
-            _saas_connection = _saas_connection(
+            _hw_connection = _hw_connection(
                 host=host, port=port, api_key_file=api_key_path
             )
-            _connected_project = _prompt_project(_saas_connection, project)
+            _connected_project = _prompt_project(_hw_connection, project)
             print(
                 "\nLogged in to project, explore it here "
                 + _connected_project.get_url()
             )
             return _connected_project
         except RestAPIError:
             logout()
@@ -190,16 +190,16 @@
         descriptor = os.open(
             path=api_key_path, flags=(os.O_WRONLY | os.O_CREAT | os.O_TRUNC), mode=0o600
         )
         with open(descriptor, "w") as fh:
             fh.write(api_key.strip())
 
     try:
-        _saas_connection = _saas_connection(host=host, port=port, api_key_value=api_key)
-        _connected_project = _prompt_project(_saas_connection, project)
+        _hw_connection = _hw_connection(host=host, port=port, api_key_value=api_key)
+        _connected_project = _prompt_project(_hw_connection, project)
     except RestAPIError as e:
         logout()
         raise e
 
     print("\nLogged in to project, explore it here " + _connected_project.get_url())
     return _connected_project
 
@@ -278,19 +278,11 @@
         for proj in saas_projects:
             if proj.name == project:
                 return proj
         raise ProjectException("Could not find project {}".format(project))
 
 
 def logout():
-    global _connected_project
-    if _connected_project is not None:
-        if (
-            _connected_project._hsfs_connection is not None
-            and _connected_project._hsfs_connection._connected is True
-        ):
-            _connected_project._hsfs_connection.close()
-
-    global _saas_connection
-    if type(_saas_connection) is Connection:
-        _saas_connection.close()
-    _saas_connection = Connection.connection
+    global _hw_connection
+    if type(_hw_connection) is Connection:
+        _hw_connection.close()
+    _hw_connection = Connection.connection
```

### Comparing `hopsworks-3.1.1rc2/hopsworks/client/__init__.py` & `hopsworks-3.2.0rc0/hopsworks/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/client/auth.py` & `hopsworks-3.2.0rc0/hopsworks/client/auth.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/client/base.py` & `hopsworks-3.2.0rc0/hopsworks/client/base.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/client/exceptions.py` & `hopsworks-3.2.0rc0/hopsworks/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/client/external.py` & `hopsworks-3.2.0rc0/hopsworks/client/external.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/client/hopsworks.py` & `hopsworks-3.2.0rc0/hopsworks/client/hopsworks.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/command.py` & `hopsworks-3.2.0rc0/hopsworks/command.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/connection.py` & `hopsworks-3.2.0rc0/hopsworks/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,16 +265,36 @@
         """Close a connection gracefully.
 
         This will clean up any materialized certificates on the local file system of
         external environments such as AWS SageMaker.
 
         Usage is recommended but optional.
         """
+        from hsfs import client as hsfs_client
+        from hsfs import engine as hsfs_engine
+        from hsml import client as hsml_client
+
+        try:
+            hsfs_client.stop()
+        except:  # noqa: E722
+            pass
+
+        try:
+            hsfs_engine.stop()
+        except:  # noqa: E722
+            pass
+
+        try:
+            hsml_client.stop()
+        except:  # noqa: E722
+            pass
+
         client.stop()
         self._connected = False
+
         print("Connection closed.")
 
     @classmethod
     def connection(
         cls,
         host: str = None,
         port: int = HOPSWORKS_PORT_DEFAULT,
```

### Comparing `hopsworks-3.1.1rc2/hopsworks/constants.py` & `hopsworks-3.2.0rc0/hopsworks/constants.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/__init__.py` & `hopsworks-3.2.0rc0/hopsworks/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/dataset_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/dataset_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -267,7 +267,41 @@
             path: path to remove
         # Raises
             `RestAPIError`: If unable to remove the path
         """
         _client = client.get_instance()
         path_params = ["project", self._project_id, "dataset", path]
         _client._send_request("DELETE", path_params)
+
+    def mkdir(self, path: str):
+        """Create a directory in the Hopsworks Filesystem.
+
+        ```python
+
+        import hopsworks
+
+        project = hopsworks.login()
+
+        dataset_api = project.get_dataset_api()
+
+        directory_path = dataset_api.mkdir("Resources/my_dir")
+
+        ```
+        # Arguments
+            path: path to directory
+        # Returns
+            `str`: Path to created directory
+        # Raises
+            `RestAPIError`: If unable to create the directory
+        """
+        _client = client.get_instance()
+        path_params = ["project", self._project_id, "dataset", path]
+        query_params = {
+            "action": "create",
+            "searchable": "true",
+            "generate_readme": "false",
+            "type": "DATASET",
+        }
+        headers = {"content-type": "application/json"}
+        return _client._send_request(
+            "POST", path_params, headers=headers, query_params=query_params
+        )["attributes"]["path"]
```

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/environment_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/environment_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/execution_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/execution_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/git_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/git_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/git_op_execution_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/git_op_execution_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/git_provider_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/git_provider_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/git_remote_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/git_remote_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/job_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/job_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/kafka_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/kafka_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/library_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/library_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/opensearch_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/opensearch_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/project_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/project_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/secret_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/secret_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/core/variable_api.py` & `hopsworks-3.2.0rc0/hopsworks/core/variable_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/decorators.py` & `hopsworks-3.2.0rc0/hopsworks/decorators.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/engine/__init__.py` & `hopsworks-3.2.0rc0/hopsworks/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/engine/environment_engine.py` & `hopsworks-3.2.0rc0/hopsworks/engine/environment_engine.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/engine/execution_engine.py` & `hopsworks-3.2.0rc0/hopsworks/engine/execution_engine.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/engine/git_engine.py` & `hopsworks-3.2.0rc0/hopsworks/engine/git_engine.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/environment.py` & `hopsworks-3.2.0rc0/hopsworks/environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,17 @@
         ```
 
         # Arguments
             path: str. The path on Hopsworks where the wheel file is located
             await_installation: bool. If True the method returns only when the installation finishes. Default True
         """
 
+        # Wait for any ongoing environment operations
+        self._environment_engine.await_environment_command()
+
         library_name = os.path.basename(path)
 
         path = util.convert_to_abs(path, self._project_name)
 
         library_spec = {
             "dependencyUrl": path,
             "channelUrl": "wheel",
@@ -120,14 +123,17 @@
         ```
 
         # Arguments
             path: str. The path on Hopsworks where the requirements.txt file is located
             await_installation: bool. If True the method returns only when the installation is finished. Default True
         """
 
+        # Wait for any ongoing environment operations
+        self._environment_engine.await_environment_command()
+
         library_name = os.path.basename(path)
 
         path = util.convert_to_abs(path, self._project_name)
 
         library_spec = {
             "dependencyUrl": path,
             "channelUrl": "requirements_txt",
```

### Comparing `hopsworks-3.1.1rc2/hopsworks/execution.py` & `hopsworks-3.2.0rc0/hopsworks/execution.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/git_commit.py` & `hopsworks-3.2.0rc0/hopsworks/git_commit.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/git_file_status.py` & `hopsworks-3.2.0rc0/hopsworks/git_file_status.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/git_op_execution.py` & `hopsworks-3.2.0rc0/hopsworks/git_op_execution.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/git_provider.py` & `hopsworks-3.2.0rc0/hopsworks/git_provider.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/git_remote.py` & `hopsworks-3.2.0rc0/hopsworks/git_remote.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/git_repo.py` & `hopsworks-3.2.0rc0/hopsworks/git_repo.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/job.py` & `hopsworks-3.2.0rc0/hopsworks/job.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/kafka_schema.py` & `hopsworks-3.2.0rc0/hopsworks/kafka_schema.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/kafka_topic.py` & `hopsworks-3.2.0rc0/hopsworks/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/library.py` & `hopsworks-3.2.0rc0/hopsworks/library.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/project.py` & `hopsworks-3.2.0rc0/hopsworks/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 
         self._opensearch_api = opensearch_api.OpenSearchApi(project_id, project_name)
         self._kafka_api = kafka_api.KafkaApi(project_id, project_name)
         self._jobs_api = job_api.JobsApi(project_id, project_name)
         self._git_api = git_api.GitApi(project_id, project_name)
         self._dataset_api = dataset_api.DatasetApi(project_id)
         self._environment_api = environment_api.EnvironmentApi(project_id, project_name)
-        self._hsfs_connection = None
 
     @classmethod
     def from_response_json(cls, json_dict):
         if json_dict:
             json_decamelized = humps.decamelize(json_dict)
             return cls(**json_decamelized)
         else:
@@ -105,22 +104,21 @@
         # Raises
             `RestAPIError`: If unable to connect
         """
         from hsfs import connection
 
         _client = client.get_instance()
         if type(_client) == Client:  # If external client
-            self._hsfs_connection = connection(
+            return connection(
                 host=_client._host,
                 port=_client._port,
                 project=self.name,
                 api_key_value=_client._auth._token,
                 engine="python",
-            )
-            return self._hsfs_connection.get_feature_store()
+            ).get_feature_store()
         else:
             return connection().get_feature_store()  # If internal client
 
     def get_model_registry(self):
         """Connect to Project's Model Registry API.
         # Returns
             `hsml.model_registry.ModelRegistry`: The Model Registry API
```

### Comparing `hopsworks-3.1.1rc2/hopsworks/secret.py` & `hopsworks-3.2.0rc0/hopsworks/secret.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/user.py` & `hopsworks-3.2.0rc0/hopsworks/user.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/util.py` & `hopsworks-3.2.0rc0/hopsworks/util.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/hopsworks/version.py` & `hopsworks-3.2.0rc0/tests/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,9 +9,7 @@
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
-
-__version__ = "3.1.1rc2"
```

### Comparing `hopsworks-3.1.1rc2/hopsworks.egg-info/PKG-INFO` & `hopsworks-3.2.0rc0/hopsworks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hopsworks
-Version: 3.1.1rc2
+Version: 3.2.0rc0
 Summary: HOPSWORKS: An environment independent client to interact with the Hopsworks API
 Home-page: https://github.com/logicalclocks/hopsworks-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/hopsworks-api/releases/tag/3.1.1rc2
+Download-URL: https://github.com/logicalclocks/hopsworks-api/releases/tag/3.2.0rc0
 Description: # Hopsworks Client
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hopsworks Version: 3.1.1rc2 Summary: HOPSWORKS: An
+Metadata-Version: 2.1 Name: hopsworks Version: 3.2.0rc0 Summary: HOPSWORKS: An
 environment independent client to interact with the Hopsworks API Home-page:
 https://github.com/logicalclocks/hopsworks-api Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/hopsworks-api/releases/tag/3.1.1rc2
+https://github.com/logicalclocks/hopsworks-api/releases/tag/3.2.0rc0
 Description: # Hopsworks Client
    [Hopsworks_Community] [Hopsworks_Documentation] [PyPiStatus] [Downloads]
                              [CodeStyle] [License]
 *hopsworks* is the python API for interacting with a Hopsworks cluster. ##
 Getting Started On Hopsworks Instantiate a connection and get the project
 object ```python import hopsworks connection = hopsworks.connection() project =
 connection.get_project("my_project") ``` Create a new project ```python project
```

### Comparing `hopsworks-3.1.1rc2/hopsworks.egg-info/SOURCES.txt` & `hopsworks-3.2.0rc0/hopsworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/setup.py` & `hopsworks-3.2.0rc0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="hopsworks",
     version=__version__,
     install_requires=[
-        "hsfs[python]~=3.1.1rc0",
-        "hsml~=3.1.0rc0",
+        "hsfs[python]~=3.2.0rc0",
+        "hsml~=3.2.0rc0",
         "pyhumps==1.6.1",
         "requests",
         "furl",
         "boto3",
         "pyjks",
         "mock",
         "tqdm",
```

### Comparing `hopsworks-3.1.1rc2/tests/__init__.py` & `hopsworks-3.2.0rc0/tests/hopsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.1.1rc2/tests/hopsworks/__init__.py` & `hopsworks-3.2.0rc0/hopsworks/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,7 +9,9 @@
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
+
+__version__ = "3.2.0rc0"
```

### Comparing `hopsworks-3.1.1rc2/tests/hopsworks/test_login.py` & `hopsworks-3.2.0rc0/tests/hopsworks/test_login.py`

 * *Files identical despite different names*

