# Comparing `tmp/ChessAnalysisPipeline-0.0.4.tar.gz` & `tmp/ChessAnalysisPipeline-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChessAnalysisPipeline-0.0.4.tar", last modified: Tue Apr 11 18:25:25 2023, max compression
+gzip compressed data, was "ChessAnalysisPipeline-0.0.5.tar", last modified: Wed Apr 12 18:11:58 2023, max compression
```

## Comparing `ChessAnalysisPipeline-0.0.4.tar` & `ChessAnalysisPipeline-0.0.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.092753 ChessAnalysisPipeline-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.084753 ChessAnalysisPipeline-0.0.4/CHAP/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/common/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/common/models/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25169 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/models/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/models/map.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24425 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3547 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   127303 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/utils/fit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48178 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/utils/general.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10472 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/utils/material.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34386 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/utils/scanparsers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2910 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/common/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/edd/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/edd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/edd/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13557 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/edd/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/edd/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/edd/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/inference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/inference/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/inference/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/inference/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4247 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3577 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2412 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/saxswaxs/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/saxswaxs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/saxswaxs/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/saxswaxs/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/saxswaxs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.088753 ChessAnalysisPipeline-0.0.4/CHAP/sin2psi/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/sin2psi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/sin2psi/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/sin2psi/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/sin2psi/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.092753 ChessAnalysisPipeline-0.0.4/CHAP/tomo/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/tomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/tomo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    97527 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/tomo/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/tomo/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/tomo/writer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2759 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/CHAP/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.092753 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-11 18:25:25.000000 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-11 18:25:25.000000 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:25:25.000000 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 18:25:25.000000 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 18:25:25.000000 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 18:25:25.000000 ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:25.092753 ChessAnalysisPipeline-0.0.4/MLaaS/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/MLaaS/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7467 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/MLaaS/ktrain.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/MLaaS/mnist_img.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14889 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/MLaaS/tfaas_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-11 18:25:25.092753 ChessAnalysisPipeline-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-11 18:25:15.000000 ChessAnalysisPipeline-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:25:25.092753 ChessAnalysisPipeline-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-11 18:25:18.000000 ChessAnalysisPipeline-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.005454 ChessAnalysisPipeline-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:57.993453 ChessAnalysisPipeline-0.0.5/CHAP/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:57.997453 ChessAnalysisPipeline-0.0.5/CHAP/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:57.997453 ChessAnalysisPipeline-0.0.5/CHAP/common/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25169 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/models/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/models/map.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24441 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3547 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:57.997453 ChessAnalysisPipeline-0.0.5/CHAP/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   127303 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/utils/fit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48178 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/utils/general.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10472 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/utils/material.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34386 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/utils/scanparsers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2910 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:57.997453 ChessAnalysisPipeline-0.0.5/CHAP/edd/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/edd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/edd/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13629 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/edd/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/edd/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/edd/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.001453 ChessAnalysisPipeline-0.0.5/CHAP/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/inference/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/inference/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/inference/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/inference/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4247 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3577 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2412 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.001453 ChessAnalysisPipeline-0.0.5/CHAP/saxswaxs/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/saxswaxs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/saxswaxs/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/saxswaxs/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/saxswaxs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.001453 ChessAnalysisPipeline-0.0.5/CHAP/sin2psi/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/sin2psi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/sin2psi/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/sin2psi/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/sin2psi/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.001453 ChessAnalysisPipeline-0.0.5/CHAP/tomo/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/tomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/tomo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97469 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/tomo/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/tomo/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/tomo/writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2759 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.005454 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-12 18:11:57.000000 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-12 18:11:57.000000 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:11:57.000000 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 18:11:57.000000 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 18:11:57.000000 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 18:11:57.000000 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.005454 ChessAnalysisPipeline-0.0.5/MLaaS/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/MLaaS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7467 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/MLaaS/ktrain.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/MLaaS/mnist_img.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14889 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/MLaaS/tfaas_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-12 18:11:58.005454 ChessAnalysisPipeline-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:11:58.005454 ChessAnalysisPipeline-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-12 18:11:49.000000 ChessAnalysisPipeline-0.0.5/setup.py
```

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/common/__init__.py` & `ChessAnalysisPipeline-0.0.5/CHAP/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/common/models/integration.py` & `ChessAnalysisPipeline-0.0.5/CHAP/common/models/integration.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/common/models/map.py` & `ChessAnalysisPipeline-0.0.5/CHAP/common/models/map.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/common/processor.py` & `ChessAnalysisPipeline-0.0.5/CHAP/common/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,16 +123,16 @@
         :return: valid map and integration configuration objects.
         :rtype: tuple[MapConfig, IntegrationConfig]
         '''
 
         self.logger.debug('Getting configuration objects')
         t0 = time()
 
-        from CHAP.common.models import MapConfig
-        from CHAP.common.models import IntegrationConfig
+        from CHAP.common.models.map import MapConfig
+        from CHAP.common.models.integration import IntegrationConfig
 
         map_config = False
         integration_config = False
         if isinstance(data, list):
             for item in data:
                 if isinstance(item, dict):
                     schema = item.get('schema')
```

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/common/reader.py` & `ChessAnalysisPipeline-0.0.5/CHAP/common/reader.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/common/utils/fit.py` & `ChessAnalysisPipeline-0.0.5/CHAP/common/utils/fit.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/common/utils/general.py` & `ChessAnalysisPipeline-0.0.5/CHAP/common/utils/general.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/common/utils/material.py` & `ChessAnalysisPipeline-0.0.5/CHAP/common/utils/material.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/common/utils/scanparsers.py` & `ChessAnalysisPipeline-0.0.5/CHAP/common/utils/scanparsers.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/common/writer.py` & `ChessAnalysisPipeline-0.0.5/CHAP/common/writer.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/edd/models.py` & `ChessAnalysisPipeline-0.0.5/CHAP/edd/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,21 +150,21 @@
         flux = np.loadtxt(self.flux_file)
         energies = flux[:,0]/1.e3
         relative_intensities = flux[:,1]/np.max(flux[:,1])
         interpolation_function = interp1d(energies, relative_intensities)
         return(interpolation_function)
 
     def material(self):
-        '''Get CeO2 as a `CHAP.common.utils.Material` object.
+        '''Get CeO2 as a `CHAP.common.utils.material.Material` object.
 
         :return: CeO2 material
-        :rtype: CHAP.common.utils.Material
+        :rtype: CHAP.common.utils.material.Material
         '''
 
-        from CHAP.common.utils import Material
+        from CHAP.common.utils.material import Material
         material = Material(material_name=self.hexrd_h5_material_name,
                             material_file=self.hexrd_h5_material_file,
                             lattice_parameters_angstroms=self.lattice_parameter_angstrom)
         # The following kwargs will be needed if we allow the material to be
         # built using xrayutilities (for now, we only allow hexrd to make the
         # material):
                             # sgnum=225,
```

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/edd/processor.py` & `ChessAnalysisPipeline-0.0.5/CHAP/edd/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             procedure
         :type calibration_config: MCACeriaCalibrationConfig
         :return: calibrated values of 2&theta and linear correction parameters
             for MCA channel energies : tth, slope, intercept
         :rtype: float, float, float
         '''
 
-        from CHAP.common.utils import Fit, FitMultipeak
+        from CHAP.common.utils.fit import Fit, FitMultipeak
         import numpy as np
         from scipy.constants import physical_constants
 
         hc = (physical_constants['Planck constant in eV/Hz'][0]
               * physical_constants['speed of light in vacuum'][0]
               * 1e7) # We'll work in keV and A, not eV and m.
 
@@ -123,15 +123,16 @@
 
             # Run the uniform fit
             best_fit, residual, best_values, best_errors, redchi, success = \
                 FitMultipeak.fit_multipeak(
                     fit_mca_intensities,
                     fit_E0,
                     x=fit_mca_energies,
-                    fit_type='uniform')
+                    fit_type='uniform',
+                    plot=False)
 
             # Extract values of interest from the best values for the uniform fit
             # parameters
             uniform_fit_centers = [best_values[f'peak{i+1}_center'] for i in range(len(calibration_config.fit_hkls))]
             # uniform_a = best_values['scale_factor']
             # uniform_strain = np.log(
             #     (uniform_a 
@@ -145,15 +146,16 @@
             # Use the peak locations found in the uniform fit as the initial
             # guesses for peak locations in the unconstrained fit
             best_fit, residual, best_values, best_errors, redchi, success = \
                 FitMultipeak.fit_multipeak(
                     fit_mca_intensities,
                     uniform_fit_centers,
                     x=fit_mca_energies,
-                    fit_type='unconstrained')
+                    fit_type='unconstrained',
+                    plot=False)
 
             # Extract values of interest from the best values for the
             # unconstrained fit parameters
             unconstrained_fit_centers = np.array(
                 [best_values[f'peak{i+1}_center'] for i in range(len(calibration_config.fit_hkls))])
             unconstrained_a = (0.5 * hc * np.sqrt(c_1)
                                / (unconstrained_fit_centers
@@ -220,15 +222,15 @@
         :raises Exception: If valid config objects cannot be constructed from
             `data`.
         :return: valid instances of the configuration objects with field values
             taken from `data`.
         :rtype: tuple[MapConfig, MCACeriaCalibrationConfig]
         '''
 
-        from CHAP.common.models import MapConfig
+        from CHAP.common.models.map import MapConfig
         from CHAP.edd.models import MCACeriaCalibrationConfig
 
         map_config = False
         calibration_config = False
         if isinstance(data, list):
             for item in data:
                 if isinstance(item, dict):
```

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/inference/processor.py` & `ChessAnalysisPipeline-0.0.5/CHAP/inference/processor.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/pipeline.py` & `ChessAnalysisPipeline-0.0.5/CHAP/pipeline.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/processor.py` & `ChessAnalysisPipeline-0.0.5/CHAP/processor.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/reader.py` & `ChessAnalysisPipeline-0.0.5/CHAP/reader.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/runner.py` & `ChessAnalysisPipeline-0.0.5/CHAP/runner.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/tomo/models.py` & `ChessAnalysisPipeline-0.0.5/CHAP/tomo/models.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/tomo/processor.py` & `ChessAnalysisPipeline-0.0.5/CHAP/tomo/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         :raises Exception: If valid config objects cannot be constructed
             from `data`.
         :return: valid instances of the configuration objects with field
             values taken from `data`.
         :rtype: dict
         '''
         #:rtype: dict{'map': MapConfig, 'reduce': TomoReduceConfig} RV: Is there a way to denote optional items?
-        from CHAP.common.models import MapConfig
+        from CHAP.common.models.map import MapConfig
         from CHAP.tomo.models import TomoSetupConfig, TomoReduceConfig, TomoFindCenterConfig, \
                 TomoReconstructConfig, TomoCombineConfig
         from nexusformat.nexus import NXroot
 
         configs = {}
         if isinstance(data, list):
             for item in data:
@@ -546,16 +546,14 @@
             # Get test mode configuration info
             if self.test_mode:
                 self.test_config = data['sample_maps'][0]['test_mode']
         elif isinstance(data, NXroot):
             nxentry = data[data.attrs['default']]
         else:
             raise ValueError(f'Invalid parameter data ({data})')
-        if 'data' in nxentry:
-            del nxentry['data']
 
         # Create an NXprocess to store data reduction (meta)data
         reduced_data = NXprocess()
 
         # Generate dark field
         if 'dark_field' in nxentry['spec_scans']:
             reduced_data = self._gen_dark(nxentry, reduced_data)
```

### Comparing `ChessAnalysisPipeline-0.0.4/CHAP/writer.py` & `ChessAnalysisPipeline-0.0.5/CHAP/writer.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/PKG-INFO` & `ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChessAnalysisPipeline
-Version: 0.0.4
+Version: 0.0.5
 Summary: CHESS analysis pipeline framework
 Home-page: https://github.com/CHESSComputing/ChessAnalysisPipeline
 Author: Keara Soloway, Rolf Verberg, Valentin Kuznetsov
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ChessAnalysisPipeline-0.0.4/ChessAnalysisPipeline.egg-info/SOURCES.txt` & `ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/LICENSE` & `ChessAnalysisPipeline-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/MLaaS/ktrain.py` & `ChessAnalysisPipeline-0.0.5/MLaaS/ktrain.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/MLaaS/mnist_img.py` & `ChessAnalysisPipeline-0.0.5/MLaaS/mnist_img.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/MLaaS/tfaas_client.py` & `ChessAnalysisPipeline-0.0.5/MLaaS/tfaas_client.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/PKG-INFO` & `ChessAnalysisPipeline-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChessAnalysisPipeline
-Version: 0.0.4
+Version: 0.0.5
 Summary: CHESS analysis pipeline framework
 Home-page: https://github.com/CHESSComputing/ChessAnalysisPipeline
 Author: Keara Soloway, Rolf Verberg, Valentin Kuznetsov
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ChessAnalysisPipeline-0.0.4/README.md` & `ChessAnalysisPipeline-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.4/setup.py` & `ChessAnalysisPipeline-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 to build doc : python setup.py doc
 to run tests : python setup.py test
 """
 
 import os
 import setuptools
 
-version = 'v0.0.4'
+version = 'v0.0.5'
 
 def datafiles(idir, pattern=None):
     """Return list of data files in provided relative dir"""
     files = []
     for dirname, dirnames, filenames in os.walk(idir):
         for subdirname in dirnames:
             files.append(os.path.join(dirname, subdirname))
```

