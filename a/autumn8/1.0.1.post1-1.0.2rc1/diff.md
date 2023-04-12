# Comparing `tmp/autumn8-1.0.1.post1.tar.gz` & `tmp/autumn8-1.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.1.post1.tar", last modified: Tue Apr 11 14:32:35 2023, max compression
+gzip compressed data, was "autumn8-1.0.2rc1.tar", last modified: Wed Apr 12 20:08:59 2023, max compression
```

## Comparing `autumn8-1.0.1.post1.tar` & `autumn8-1.0.2rc1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.354785 autumn8-1.0.1.post1/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2384 2023-04-11 14:32:35.354785 autumn8-1.0.1.post1/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2161 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.304785 autumn8-1.0.1.post1/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.314785 autumn8-1.0.1.post1/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7850 2023-04-11 13:47:09.000000 autumn8-1.0.1.post1/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.324785 autumn8-1.0.1.post1/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3190 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    15401 2023-04-11 13:56:38.000000 autumn8-1.0.1.post1/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1453 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3227 2023-04-11 14:28:57.000000 autumn8-1.0.1.post1/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4953 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3126 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/cli/pending_uploads.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.324785 autumn8-1.0.1.post1/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      109 2023-04-11 14:31:49.000000 autumn8-1.0.1.post1/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.324785 autumn8-1.0.1.post1/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6503 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3200 2023-04-11 12:40:47.000000 autumn8-1.0.1.post1/autumn8/common/config/s3.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    63841 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      366 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.334785 autumn8-1.0.1.post1/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.344785 autumn8-1.0.1.post1/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.354785 autumn8-1.0.1.post1/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2657 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    10255 2023-04-11 14:30:25.000000 autumn8-1.0.1.post1/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.1.post1/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1149 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-11 12:01:33.000000 autumn8-1.0.1.post1/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.1.post1/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4578 2023-04-11 14:30:05.000000 autumn8-1.0.1.post1/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.304785 autumn8-1.0.1.post1/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2384 2023-04-11 14:32:35.000000 autumn8-1.0.1.post1/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1262 2023-04-11 14:32:35.000000 autumn8-1.0.1.post1/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-04-11 14:32:35.000000 autumn8-1.0.1.post1/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-04-11 14:32:35.000000 autumn8-1.0.1.post1/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      126 2023-04-11 14:32:35.000000 autumn8-1.0.1.post1/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-04-11 14:32:35.000000 autumn8-1.0.1.post1/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1933 2023-03-31 14:44:39.000000 autumn8-1.0.1.post1/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-04-11 14:32:35.354785 autumn8-1.0.1.post1/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-11 14:32:35.354785 autumn8-1.0.1.post1/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.1.post1/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:08:59.012694 autumn8-1.0.2rc1/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-04-12 20:08:59.012694 autumn8-1.0.2rc1/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:08:58.932690 autumn8-1.0.2rc1/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.2rc1/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:08:58.952691 autumn8-1.0.2rc1/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.2rc1/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.2rc1/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7850 2023-04-12 20:01:39.000000 autumn8-1.0.2rc1/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-11 12:01:33.000000 autumn8-1.0.2rc1/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:08:58.952691 autumn8-1.0.2rc1/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4109 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    15368 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.2rc1/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1795 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3304 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5148 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3126 2023-04-11 12:01:33.000000 autumn8-1.0.2rc1/autumn8/cli/pending_uploads.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:08:58.952691 autumn8-1.0.2rc1/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:08:58.952691 autumn8-1.0.2rc1/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3200 2023-04-12 19:59:12.000000 autumn8-1.0.2rc1/autumn8/common/config/s3.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.2rc1/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65037 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:08:58.982693 autumn8-1.0.2rc1/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.2rc1/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.2rc1/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.2rc1/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.2rc1/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.2rc1/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.2rc1/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:08:58.992693 autumn8-1.0.2rc1/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-11 12:01:33.000000 autumn8-1.0.2rc1/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:08:59.012694 autumn8-1.0.2rc1/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.2rc1/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3637 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    10396 2023-04-12 20:08:36.000000 autumn8-1.0.2rc1/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.2rc1/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1149 2023-04-11 12:01:33.000000 autumn8-1.0.2rc1/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-11 12:01:33.000000 autumn8-1.0.2rc1/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.2rc1/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4578 2023-04-12 20:01:39.000000 autumn8-1.0.2rc1/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:08:58.942691 autumn8-1.0.2rc1/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-04-12 20:08:58.000000 autumn8-1.0.2rc1/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1262 2023-04-12 20:08:58.000000 autumn8-1.0.2rc1/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-04-12 20:08:58.000000 autumn8-1.0.2rc1/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-04-12 20:08:58.000000 autumn8-1.0.2rc1/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      126 2023-04-12 20:08:58.000000 autumn8-1.0.2rc1/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-04-12 20:08:58.000000 autumn8-1.0.2rc1/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1933 2023-03-31 14:44:39.000000 autumn8-1.0.2rc1/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-04-12 20:08:59.012694 autumn8-1.0.2rc1/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.2rc1/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-12 20:08:59.012694 autumn8-1.0.2rc1/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.2rc1/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.2rc1/tests/test_settings.py
```

### Comparing `autumn8-1.0.1.post1/autumn8/cli/analyze.py` & `autumn8-1.0.2rc1/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/cli/cli_environment.py` & `autumn8-1.0.2rc1/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/cli/commands/models.py` & `autumn8-1.0.2rc1/autumn8/cli/commands/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,44 +13,45 @@
 import questionary
 from jsonschema import validate
 
 from autumn8.cli import options
 from autumn8.cli.analyze import analyze_model_file, suggest_model_name
 from autumn8.cli.cli_environment import CliEnvironment
 from autumn8.cli.examples import example_model_names
-from autumn8.cli.interactive import announce_model_upload_response
+from autumn8.cli.interactive import (
+    announce_model_upload_response,
+    normalize_args,
+)
 from autumn8.common.config.settings import supported_quants
 from autumn8.lib import api_creds, logging
 from autumn8.lib import service as autodl
 from autumn8.lib.api import lab
 
 USER_ID_LENGTH = len(str(uuid.uuid4()))
 API_KEY_LENGTH = 32
 
 logger = logging.getLogger(__name__)
 
 
-@click.group()
+@click.group(context_settings={"token_normalize_func": normalize_args})
 def model_commands_group():
     pass
 
 
 @model_commands_group.command()
 @options.use_environment
 @options.use_quiet_mode
 @click.option(
     "-u",
     "--user_id",
-    "--user-id",
     help="The ID of the user that the CLI will authenticate as in AutoDL.",
 )
 @click.option(
     "-a",
     "--api_key",
-    "--api-key",
     help="API Key to use when authenticating in AutoDL from now on.",
 )
 def login(user_id, api_key, environment: CliEnvironment, quiet):
     """Store API credentials for the CLI for future use."""
 
     logger.info(
         f"To setup up CLI access, please visit {environment.value.app_host}/profile - once you're signed in, generate a new API Key, then copy and paste the API Key data from the browser here\ngg"
@@ -232,42 +233,39 @@
             "--quantization",
             "--quants",
             type=click.Choice(supported_quants, case_sensitive=False),
             help="Quantization for the model.",
         ),
         click.option(
             "--input_dims",
-            "--input-dims",
             type=str,
             help="The model input dimensions, specified as a JSON array.",
         ),
         click.option(
             "-w",
             "--max_upload_workers",
             type=int,
             help=f"The count of workers to use for multipart uploads; defaults to {DEFAULT_MAX_UPLOAD_WORKERS}.",
             default=DEFAULT_MAX_UPLOAD_WORKERS,
         ),
         click.option(
-            "--input-file",
             "--input_file",
             type=str,
             help="The model input filepath.",
         ),
         click.option(
             "-y",
             "--yes",
             "auto_confirm",
             type=bool,
             is_flag=True,
             help="Skip all confirmation input from the user.",
         ),
         click.option(
             "--skip_inputs",
-            "--skip-inputs",
             "should_skip_inputs",
             type=bool,
             is_flag=True,
             help="Don't ask about inputs, let AutoDL try to infer them.",
         ),
         options.use_organization_id,
         options.use_quiet_mode,
```

### Comparing `autumn8-1.0.1.post1/autumn8/cli/examples.py` & `autumn8-1.0.2rc1/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/cli/main.py` & `autumn8-1.0.2rc1/autumn8/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from questionary import Choice
 
 from autumn8.cli import options, pending_uploads
 from autumn8.cli.commands import cloud, models
 from autumn8.cli.interactive import (
     announce_model_upload_response,
     fetch_user_data,
+    normalize_args,
 )
 from autumn8.common._version import __version__
 from autumn8.lib.service import resume_upload_model
 
 # from autumn8.cli.cli_environment import CliEnvironment
 # from autumn8.common.config.s3 import init_s3_client
 
@@ -75,15 +76,15 @@
     Test AutoDL connection with the current API key.
     Displays the user's email address upon successful connection.
     """
     user_data = fetch_user_data(environment)
     print(f"Hello! You're authenticated as {user_data['email']}")
 
 
-@click.group()
+@click.group(context_settings={"token_normalize_func": normalize_args})
 @click.version_option(version=__version__)
 def main():
     pass
 
 
 main.command()(test_connection)
```

### Comparing `autumn8-1.0.1.post1/autumn8/cli/options.py` & `autumn8-1.0.2rc1/autumn8/cli/options.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     "--quiet",
     is_flag=True,
     callback=lambda ctx, param, value: logging.set_max_log_verbosity(
         logging.ERROR
     )
     if value
     else None,
-    help="Skip addinional logging, printing only necessary info",
+    help="Skip additional logging, printing only necessary info",
 )
 
 
 def pick_cloud_provider(options: List[CloudServiceProvider]):
     cloud_provider = questionary.select(
         "Choose service provider",
         choices=[
@@ -116,15 +116,15 @@
 ExtendedCloudProviderLabel = Union[
     CloudProviderLabelExtensionsType,
     CloudServiceProvider,
 ]
 
 
 def map_string_value_to_cloud_provider(
-    value: ExtendedCloudProviderLabel,
+    value: str,
 ) -> Optional[CloudServiceProvider]:
     if value is None or value == str(None):
         return None
 
     if value.lower() == "gcp":
         return CloudServiceProvider.GOOGLE
 
@@ -135,52 +135,56 @@
         return CloudServiceProvider.AMAZON
 
     for provider in CloudServiceProvider:
         if provider.value.lower() == value.lower():
             return provider
 
     raise ClickException(
-        f"{value} is not a valid cloud provider. It must be one of "
-        + f"{[p.value for p in CloudServiceProvider]}",
+        f"'{value}' is not a valid cloud provider. It must be one of "
+        + f"{CloudProviderLabelExtensions+ [p.value for p in CloudServiceProvider] }",
     )
 
 
-def get_callback_for_picking_valid_cloud_provider(optional):
-    def callback(ctx: click.Context, param: click.Parameter, value):
+def get_callback_for_picking_valid_cloud_provider(
+    optional: bool = False, default_value: Optional[CloudServiceProvider] = None
+):
+    def callback(ctx: click.Context, param: click.Parameter, value: str):
         provider_from_value = map_string_value_to_cloud_provider(value)
 
         machine_type = ctx.params.get("machine_type")
         valid_cloud_providers = get_valid_cloud_providers_for_machine_type(
             machine_type
         )
 
         if provider_from_value is None:
             if optional:
-                return None
+                return default_value
             return pick_cloud_provider(valid_cloud_providers)
 
         for provider in valid_cloud_providers:
             if provider is provider_from_value:
                 return provider
 
         raise ClickException(
             f"{provider_from_value} is not a valid cloud provider for machine "
             + f"{machine_type}. It must be one of {valid_cloud_providers}",
         )
 
     return callback
 
 
-def use_cloud_provider_picker(optional=False):
+def use_cloud_provider_picker(
+    optional: bool = False, default_value: Optional[CloudServiceProvider] = None
+):
     return click.option(
         "-c",
         "--cloud_provider",
         type=click.Choice(
             CloudProviderLabelExtensions
             + [p.value for p in CloudServiceProvider],
             case_sensitive=False,
         ),
         callback=get_callback_for_picking_valid_cloud_provider(
-            optional=optional
+            optional=optional, default_value=default_value
         ),
         help="Cloud provider to use",
     )
```

### Comparing `autumn8-1.0.1.post1/autumn8/cli/pending_uploads.py` & `autumn8-1.0.2rc1/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/common/config/cloud_info.py` & `autumn8-1.0.2rc1/autumn8/common/config/cloud_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """A client service for CloudInfo, reqires CloudInfo to be running and available under CLOUDINFO_API_PATH"""
 # https://github.com/banzaicloud/cloudinfo
 
 import os
 from dataclasses import dataclass
 from http import HTTPStatus
-from typing import Literal, Optional, TypedDict, Union
+from typing import Dict, Literal, Optional, Union
 
 import requests
 from fastapi import HTTPException
 
 from autumn8.common.config.settings import CloudServiceProvider
 
 CPU_ARCHITECTURE = Literal["x86_64", "arm64"]
@@ -24,14 +24,15 @@
     hyperthreading: bool
     usd_per_hr: Optional[float]
     predictor_target: str
     predictor_num_threads: float
     service_provider: CloudServiceProvider
     ram: Optional[float]
     gpuram: Optional[float]
+    is_supported_by_a8f: bool = False
     cpu_arch: Optional[CPU_ARCHITECTURE] = None
 
     # you can determine if the instance is available in govcloud
     # using https://calculator.aws/#/addService/ec2-enhancement
     # and checking either of the GovCloud regions
     aws_govcloud: Union[bool, str] = False
 
@@ -56,24 +57,27 @@
     return translation_dict[autodl_service_provider]
 
 
 class CloudInfoService:
     _cloud_products_info = None
 
     def __init__(
-        self, provider, region, fetch_data_from_cloud_info=True
+        self, provider, region, fetch_data_from_cloud_info: bool = True
     ) -> None:
         self.cloudinfo_service_enabled = fetch_data_from_cloud_info
         self.provider = provider
         self.region = region
 
     @property
     def cloud_products_info(self):
         """Get cloud products info and cache it for further reuse"""
 
+        if not self.cloudinfo_service_enabled:
+            return None
+
         if self._cloud_products_info is None:
             service_type = "compute"
             cloudinfo_api_path = os.environ["CLOUDINFO_API_PATH"]
             provider = map_autodl_service_provider_to_cloudinfo_provider(
                 self.provider
             )
 
@@ -130,14 +134,15 @@
         cores: int,
         hyperthreading: bool,
         hardcoded_usd_per_hr: Optional[float] = None,
         predictor_target: str,
         predictor_num_threads: float,
         ram: float,
         gpuram: Optional[float] = None,
+        is_supported_by_a8f: bool = False,
         aws_govcloud: Union[bool, str] = False,
         cpu_arch: Optional[CPU_ARCHITECTURE] = None,
     ) -> InstanceDescription:
         usd_per_hr = (
             hardcoded_usd_per_hr
             if hardcoded_usd_per_hr
             else self.get_instance_pricing(label)
@@ -153,14 +158,15 @@
             hyperthreading=hyperthreading,
             usd_per_hr=usd_per_hr,
             predictor_target=predictor_target,
             predictor_num_threads=predictor_num_threads,
             service_provider=self.provider,
             ram=ram,
             gpuram=gpuram,
+            is_supported_by_a8f=is_supported_by_a8f,
             aws_govcloud=aws_govcloud,
             cpu_arch=cpu_arch,
         )
 
     def build_keyed_instance_description(
         self,
         *,
@@ -171,29 +177,31 @@
         cores: int,
         hyperthreading: bool,
         hardcoded_usd_per_hr: Optional[float] = None,
         predictor_target: str,
         predictor_num_threads: int,
         ram: float,
         gpuram: Optional[float] = None,
+        is_supported_by_a8f: bool = False,
         aws_govcloud: Union[bool, str] = False,
         cpu_arch: Optional[CPU_ARCHITECTURE] = None,
-    ):
+    ) -> Dict[str, Dict[int, InstanceDescription]]:
         return {
             predictor_target: {
                 predictor_num_threads: self.build_instance_description(
                     label=label,
                     family=family,
                     instance_description_link=instance_description_link,
                     hw=hw,
                     cores=cores,
                     hyperthreading=hyperthreading,
                     hardcoded_usd_per_hr=hardcoded_usd_per_hr,
                     predictor_target=predictor_target,
                     predictor_num_threads=predictor_num_threads,
                     ram=ram,
                     gpuram=gpuram,
+                    is_supported_by_a8f=is_supported_by_a8f,
                     aws_govcloud=aws_govcloud,
                     cpu_arch=cpu_arch,
                 )
             }
         }
```

### Comparing `autumn8-1.0.1.post1/autumn8/common/config/s3.py` & `autumn8-1.0.2rc1/autumn8/common/config/s3.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/common/config/settings.py` & `autumn8-1.0.2rc1/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/common/config/supported_instances.py` & `autumn8-1.0.2rc1/autumn8/common/config/supported_instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
-from typing import Callable, Dict
+from http import HTTPStatus
+from typing import Callable, Dict, Optional
 
-from autumn8.common.config.cloud_info import CloudInfoService, InstanceDescription
+from fastapi import HTTPException
+
+from autumn8.common.config.cloud_info import (
+    CloudInfoService,
+    InstanceDescription,
+)
 from autumn8.common.config.settings import CloudServiceProvider
 from autumn8.common.types import DEFAULT_CLOUD_ZONES_CONFIG, ZoneConfig
 from autumn8.lib import logging
 
 logger = logging.getLogger(__name__)
 
 
@@ -12,23 +18,26 @@
     return {
         provider: CloudInfoService(provider, zone)
         for provider, zone in DEFAULT_CLOUD_ZONES_CONFIG.items()
     }
 
 
 def find_instance_config(
-    predictor_target, fetch_data_from_cloud_info=True, num_threads=None
+    predictor_target: str,
+    fetch_data_from_cloud_info: bool = True,
+    num_threads: Optional[int] = None,
 ) -> InstanceDescription:
     instances = get_supported_cloud_instances(
         fetch_data_from_cloud_info=fetch_data_from_cloud_info
     )
 
     if predictor_target not in instances:
-        raise ValueError(
-            f'Instance config not found for target="{predictor_target}"'
+        raise HTTPException(
+            HTTPStatus.NOT_FOUND,
+            f'Instance config not found for instance_type="{predictor_target}"',
         )
 
     instances_by_num_threads = instances[predictor_target]
 
     if len(instances_by_num_threads.items()) == 1:
         the_only_key = [*instances_by_num_threads.keys()][0]
         num_threads = the_only_key
@@ -186,110 +195,119 @@
             hyperthreading=True,
             hardcoded_usd_per_hr=0.0000001667
             * 1000
             * 3600,  # TODO cloudinfo doesn't support lambdas pricing, handle that across zones somehow
             predictor_target="lambda_10240MB",
             predictor_num_threads=5,
             ram=10,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5.large",
             family="c5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=2,
             hyperthreading=True,
             predictor_target="c5.large",
             predictor_num_threads=1,
             ram=4,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5.xlarge",
             family="c5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=4,
             hyperthreading=True,
             predictor_target="c5.xlarge",
             predictor_num_threads=2,
             ram=8,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5.2xlarge",
             family="c5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=8,
             hyperthreading=True,
             predictor_target="c5.2xlarge",
             predictor_num_threads=4,
             ram=16,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5.4xlarge",
             family="c5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=16,
             hyperthreading=True,
             predictor_target="c5.4xlarge",
             predictor_num_threads=8,
             ram=32,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5.9xlarge",
             family="c5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=36,
             hyperthreading=True,
             predictor_target="c5.9xlarge",
             predictor_num_threads=18,
             ram=72,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5.12xlarge",
             family="c5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=48,
             hyperthreading=True,
             predictor_target="c5.12xlarge",
             predictor_num_threads=24,
             ram=96,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5.18xlarge",
             family="c5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=72,
             hyperthreading=True,
             predictor_target="c5.18xlarge",
             predictor_num_threads=36,
             ram=144,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5.24xlarge",
             family="c5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=96,
             hyperthreading=True,
             predictor_target="c5.24xlarge",
             predictor_num_threads=48,
             ram=192,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5a.large",
             family="c5a",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="AMD EPYC",
@@ -522,62 +540,67 @@
             instance_description_link="https://aws.amazon.com/ec2/instance-types/t3/",
             hw="Intel Xeon Platinum",
             cores=2,
             hyperthreading=True,
             predictor_target="t3.small",
             predictor_num_threads=2,
             ram=2,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="t3.medium",
             family="t3",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/t3/",
             hw="Intel Xeon Platinum",
             cores=2,
             hyperthreading=True,
             predictor_target="t3.medium",
             predictor_num_threads=2,
             ram=4,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="t3.large",
             family="t3",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/t3/",
             hw="Intel Xeon Platinum",
             cores=2,
             hyperthreading=True,
             predictor_target="t3.large",
             predictor_num_threads=2,
             ram=8,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="t3.xlarge",
             family="t3",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/t3/",
             hw="Intel Xeon Platinum",
             cores=4,
             hyperthreading=True,
             predictor_target="t3.xlarge",
             predictor_num_threads=4,
             ram=16,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="t3.2xlarge",
             family="t3",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/t3/",
             hw="Intel Xeon Platinum",
             cores=8,
             hyperthreading=True,
             predictor_target="t3.2xlarge",
             predictor_num_threads=8,
             ram=32,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         # t4g micro and nano missing
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="t4g.small",
             family="t4",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/t4/",
@@ -918,28 +941,30 @@
             cores=8,
             hyperthreading=False,
             hardcoded_usd_per_hr=0.752,
             predictor_target="g4ad.2xlarge",
             predictor_num_threads=8,
             ram=32,
             gpuram=16,
+            is_supported_by_a8f=True,
             aws_govcloud=False,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="p3.2xlarge",
             family="p3",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/p3/",
             hw="NVIDIA V100 GPUs",
             cores=8,
             hyperthreading=False,
             hardcoded_usd_per_hr=3.06,
             predictor_target="p3.2xlarge",
             predictor_num_threads=8,
             ram=61,
             gpuram=16,
+            is_supported_by_a8f=True,
             aws_govcloud="US West only",
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="p2.xlarge",
             family="p2",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/p2/",
             hw="NVIDIA K80 GPUs",
@@ -958,138 +983,149 @@
             hw="NVIDIA V100 GPUs",
             cores=32,
             hyperthreading=False,
             predictor_target="p3.8xlarge",
             predictor_num_threads=16,
             ram=244,
             gpuram=64,
+            is_supported_by_a8f=True,
             aws_govcloud="US West only",
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="g3s.xlarge",
             family="g3s",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/g3/",
             hw="NVIDIA Tesla M60 GPU",
             cores=2,
             hyperthreading=False,
             predictor_target="g3s.xlarge",
             predictor_num_threads=4,
             ram=30.5,
             gpuram=16,
+            is_supported_by_a8f=True,
             aws_govcloud="US West only",
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="g4dn.xlarge",
             family="g4dn",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/g4/",
             hw="NVIDIA T4 GPU",
             cores=4,
             hyperthreading=False,
             predictor_target="g4dn.xlarge",
             predictor_num_threads=4,
             ram=16,
             gpuram=16,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="g5.xlarge",
             family="g5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/g5/",
             hw="NVIDIA A10G",
             cores=4,
             hyperthreading=False,
             predictor_target="g5.xlarge",
             predictor_num_threads=4,
             ram=16,
             gpuram=24,
+            is_supported_by_a8f=True,
             aws_govcloud=False,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="g5.2xlarge",
             family="g5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/g5/",
             hw="NVIDIA A10G",
             cores=8,
             hyperthreading=False,
             predictor_target="g5.2xlarge",
             predictor_num_threads=4,
             ram=32,
             gpuram=24,
+            is_supported_by_a8f=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="g5.4xlarge",
             family="g5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/g5/",
             hw="NVIDIA A10G",
             cores=16,
             hyperthreading=False,
             predictor_target="g5.4xlarge",
             predictor_num_threads=8,
             ram=64,
             gpuram=24,
+            is_supported_by_a8f=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="g5.8xlarge",
             family="g5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/g5/",
             hw="NVIDIA A10G",
             cores=32,
             hyperthreading=False,
             predictor_target="g5.8xlarge",
             predictor_num_threads=16,
             ram=128,
             gpuram=24,
+            is_supported_by_a8f=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="g5.12xlarge",
             family="g5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/g5/",
             hw="NVIDIA A10G",
             cores=48,
             hyperthreading=False,
             predictor_target="g5.12xlarge",
             predictor_num_threads=24,
             ram=192,
             gpuram=24 * 4,
+            is_supported_by_a8f=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="g5.16xlarge",
             family="g5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/g5/",
             hw="NVIDIA A10G",
             cores=64,
             hyperthreading=False,
             predictor_target="g5.16xlarge",
             predictor_num_threads=32,
             ram=256,
             gpuram=24,
+            is_supported_by_a8f=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="g5.24xlarge",
             family="g5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/g5/",
             hw="NVIDIA A10G",
             cores=96,
             hyperthreading=False,
             predictor_target="g5.24xlarge",
             predictor_num_threads=48,
             ram=384,
             gpuram=24 * 4,
+            is_supported_by_a8f=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="g5.48xlarge",
             family="g5",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/g5/",
             hw="NVIDIA A10G",
             cores=192,
             hyperthreading=False,
             predictor_target="g5.48xlarge",
             predictor_num_threads=96,
             ram=768,
             gpuram=24 * 8,
+            is_supported_by_a8f=True,
         ),
     }
 
 
 def get_supported_oracle_cloud_instances(
     oracle_cloud_info_service: CloudInfoService,
 ):
```

### Comparing `autumn8-1.0.1.post1/autumn8/examples/mnist.py` & `autumn8-1.0.2rc1/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/examples/model.py` & `autumn8-1.0.2rc1/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.2rc1/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.2rc1/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/lib/__init__.py` & `autumn8-1.0.2rc1/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/lib/api/cloud.py` & `autumn8-1.0.2rc1/autumn8/lib/api/cloud.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from typing import Any, Dict, Optional
 
 import requests
 from requests.auth import HTTPBasicAuth
 
 from autumn8.cli.cli_environment import CliEnvironment
 from autumn8.common.config.settings import CloudServiceProvider
+from autumn8.common.types import Sla
 from autumn8.lib.api.lab import require_ok_response, url_with_params
 from autumn8.lib.api_creds import retrieve_api_creds
 
+DEFAULT_API_TIMEOUT = 60
+
 
 def get_running_deployments(
     organization_id: int,
     environment: CliEnvironment,
     model_id: Optional[int] = None,
     service_provider: Optional[CloudServiceProvider] = None,
 ):
@@ -25,20 +28,51 @@
 
     deployments_api_route = f"{autodl_host}/api/cloud/deployments"
     # TODO: wrap the requests library in a custom class to handle common logic like auth and headers for json
     response = requests.get(
         url_with_params(deployments_api_route, params),
         headers={"Content-Type": "application/json"},
         auth=HTTPBasicAuth(*retrieve_api_creds()),
+        timeout=DEFAULT_API_TIMEOUT,
     )
 
     require_ok_response(response)
     return response.json()["deployments"]
 
 
+def deploy_by_best_sla(
+    organization_id: int,
+    environment: CliEnvironment,
+    model_id: int,
+    best_sla: Sla,
+    service_provider: CloudServiceProvider,
+):
+    autodl_host = environment.value.app_host
+
+    params = {
+        "organization_id": organization_id,
+        "model_id": model_id,
+        "best_sla": best_sla.value,
+        "cloud_service_provider": service_provider.value,
+    }
+
+    print("sending", params)
+
+    deployments_api_route = f"{autodl_host}/api/cloud/deployments/by_sla"
+    response = requests.post(
+        url_with_params(deployments_api_route, params),
+        headers={"Content-Type": "application/json"},
+        auth=HTTPBasicAuth(*retrieve_api_creds()),
+        timeout=DEFAULT_API_TIMEOUT,
+    )
+
+    require_ok_response(response)
+    return response.json()
+
+
 def deploy(
     organization_id: int,
     environment: CliEnvironment,
     model_id: int,
     machine_type: str,
     service_provider: CloudServiceProvider,
 ):
@@ -52,14 +86,15 @@
     }
 
     deployments_api_route = f"{autodl_host}/api/cloud/deployments"
     response = requests.post(
         url_with_params(deployments_api_route, params),
         headers={"Content-Type": "application/json"},
         auth=HTTPBasicAuth(*retrieve_api_creds()),
+        timeout=DEFAULT_API_TIMEOUT,
     )
 
     require_ok_response(response)
     return response.json()
 
 
 def terminate_deployment(
@@ -78,11 +113,12 @@
     deployments_api_route = (
         f"{autodl_host}/api/cloud/deployments/{deployment_id}"
     )
     response = requests.delete(
         url_with_params(deployments_api_route, params),
         headers={"Content-Type": "application/json"},
         auth=HTTPBasicAuth(*retrieve_api_creds()),
+        timeout=DEFAULT_API_TIMEOUT,
     )
 
     require_ok_response(response)
     return response.json()
```

### Comparing `autumn8-1.0.1.post1/autumn8/lib/api/lab.py` & `autumn8-1.0.2rc1/autumn8/lib/api/lab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import io
 import json
 import os
 import urllib
 import urllib.parse
 from http import HTTPStatus
 from threading import Lock
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import appdirs
+import httpx
 import requests
 from mypy_boto3_s3 import S3Client
 from mypy_boto3_s3.type_defs import PartTypeDef
 from requests.auth import HTTPBasicAuth
 from tqdm.contrib.concurrent import thread_map
 
 from autumn8.cli import pending_uploads
@@ -27,24 +28,26 @@
 APP_AUTHOR = "autumn8"
 
 logger = logging.getLogger(__name__)
 
 data_dir = appdirs.user_data_dir(APP_NAME, APP_AUTHOR)
 
 
-def url_with_params(url, params):
+def url_with_params(url: str, params: Dict[str, Union[str, int]]):
     url_parse = urllib.parse.urlparse(url)
     url_new_query = urllib.parse.urlencode(params)
     url_parse = url_parse._replace(query=url_new_query)
 
     new_url = urllib.parse.urlunparse(url_parse)
     return new_url
 
 
-def require_ok_response(response):
+def require_ok_response(
+    response: Union[requests.Response, httpx.Response]
+) -> None:
     if response.status_code == HTTPStatus.UNAUTHORIZED:
         raise Exception(
             f"Received response {response.status_code}:\n{response.text}\n\nUser not authenticated; please run `autumn8-cli login` to authorize your CLI"
         )
     if response.status_code != HTTPStatus.OK:
         raise Exception(
             f"Received response {response.status_code}:\n{response.text}"
@@ -87,15 +90,17 @@
         auth=HTTPBasicAuth(*retrieve_api_creds()),
     )
 
     require_ok_response(response)
     return response.json()
 
 
-def delete_model(environment: CliEnvironment, organization_id, model_id):
+def delete_model(
+    environment: CliEnvironment, organization_id: int, model_id: int
+):
     autodl_host = environment.value.app_host
     new_url = url_with_params(
         f"{autodl_host}/api/lab/model",
         {"model_id": model_id, "organization_id": organization_id},
     )
     response = requests.delete(
         new_url,
@@ -322,15 +327,17 @@
                 resume_args,
                 id_key,
                 upload_id,
                 max_upload_workers=max_upload_workers,
             )
 
 
-def async_prediction(environment: CliEnvironment, organization_id, model_id):
+def async_prediction(
+    environment: CliEnvironment, organization_id: int, model_id: int
+):
     autodl_host = environment.value.app_host
     new_url = url_with_params(
         f"{autodl_host}/api/lab/model/async_prediction",
         {
             "model_id": model_id,
             "organization_id": organization_id,
         },
```

### Comparing `autumn8-1.0.1.post1/autumn8/lib/api_creds.py` & `autumn8-1.0.2rc1/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/lib/logging.py` & `autumn8-1.0.2rc1/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/lib/logging.yaml` & `autumn8-1.0.2rc1/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/lib/package_resolver.py` & `autumn8-1.0.2rc1/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8/lib/service.py` & `autumn8-1.0.2rc1/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.2rc1/autumn8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/pyproject.toml` & `autumn8-1.0.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.2rc1/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.1.post1/tests/test_settings.py` & `autumn8-1.0.2rc1/tests/test_settings.py`

 * *Files identical despite different names*

