# Comparing `tmp/rdt_identity-1.3.1.dev0.tar.gz` & `tmp/rdt_identity-1.4.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt_identity-1.3.1.dev0.tar", last modified: Wed Apr 12 20:29:55 2023, max compression
+gzip compressed data, was "rdt_identity-1.4.0.dev0.tar", last modified: Wed Apr 12 20:59:46 2023, max compression
```

## Comparing `rdt_identity-1.3.1.dev0.tar` & `rdt_identity-1.4.0.dev0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.498223 rdt_identity-1.3.1.dev0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    25996 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    41255 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8014 2023-04-12 20:29:55.498329 rdt_identity-1.3.1.dev0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.487164 rdt_identity-1.3.1.dev0/rdt/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.487230 rdt_identity-1.3.1.dev0/rdt/transformers/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.487295 rdt_identity-1.3.1.dev0/rdt/transformers/addons/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.490584 rdt_identity-1.3.1.dev0/rdt/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/rdt/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/rdt/transformers/addons/identity/identity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-04-12 20:29:55.498857 rdt_identity-1.3.1.dev0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4191 2023-01-18 20:53:13.000000 rdt_identity-1.3.1.dev0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.491064 rdt_identity-1.3.1.dev0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21679 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.487556 rdt_identity-1.3.1.dev0/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.491823 rdt_identity-1.3.1.dev0/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.492289 rdt_identity-1.3.1.dev0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    43118 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9356 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.493310 rdt_identity-1.3.1.dev0/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.493618 rdt_identity-1.3.1.dev0/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2512 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2312 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8679 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.494043 rdt_identity-1.3.1.dev0/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.494336 rdt_identity-1.3.1.dev0/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.3.1.dev0/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.494942 rdt_identity-1.3.1.dev0/tests/quality/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/quality/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    30119 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/quality/dataset_info.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10032 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/quality/test_quality.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1531 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/quality/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.495533 rdt_identity-1.3.1.dev0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1192 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1359 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/unit/test__addons.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103818 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.497182 rdt_identity-1.3.1.dev0/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.497329 rdt_identity-1.3.1.dev0/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.497624 rdt_identity-1.3.1.dev0/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.498089 rdt_identity-1.3.1.dev0/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    38553 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8522 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18913 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20962 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    61010 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1075 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.861179 rdt_identity-1.4.0.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    25996 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    41255 2023-04-12 20:59:08.000000 rdt_identity-1.4.0.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8014 2023-04-12 20:59:46.861294 rdt_identity-1.4.0.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.849396 rdt_identity-1.4.0.dev0/rdt/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.849463 rdt_identity-1.4.0.dev0/rdt/transformers/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.849531 rdt_identity-1.4.0.dev0/rdt/transformers/addons/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.852671 rdt_identity-1.4.0.dev0/rdt/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/rdt/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/rdt/transformers/addons/identity/identity.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-04-12 20:59:46.861854 rdt_identity-1.4.0.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4191 2023-04-12 20:59:28.000000 rdt_identity-1.4.0.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.853103 rdt_identity-1.4.0.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/code_style.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21679 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/contributing.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.849779 rdt_identity-1.4.0.dev0/tests/datasets/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.854231 rdt_identity-1.4.0.dev0/tests/datasets/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/datasets/tests/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/datasets/tests/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/datasets/tests/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/datasets/tests/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/datasets/tests/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.854722 rdt_identity-1.4.0.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    43118 2023-04-12 20:25:40.000000 rdt_identity-1.4.0.dev0/tests/integration/test_hyper_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9356 2023-04-12 20:25:40.000000 rdt_identity-1.4.0.dev0/tests/integration/test_transformers.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.855750 rdt_identity-1.4.0.dev0/tests/integration/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/integration/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.856041 rdt_identity-1.4.0.dev0/tests/integration/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/integration/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/integration/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/integration/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2512 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/integration/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-12 20:25:40.000000 rdt_identity-1.4.0.dev0/tests/integration/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2312 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/integration/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8679 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/integration/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-12 20:25:40.000000 rdt_identity-1.4.0.dev0/tests/integration/transformers/test_text.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.856539 rdt_identity-1.4.0.dev0/tests/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/performance/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/performance/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-12 20:25:40.000000 rdt_identity-1.4.0.dev0/tests/performance/test_performance.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.856906 rdt_identity-1.4.0.dev0/tests/performance/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/performance/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.4.0.dev0/tests/performance/tests/test_profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.857721 rdt_identity-1.4.0.dev0/tests/quality/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/quality/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    30119 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/quality/dataset_info.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10032 2023-04-12 20:25:40.000000 rdt_identity-1.4.0.dev0/tests/quality/test_quality.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1531 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/quality/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.858326 rdt_identity-1.4.0.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1192 2023-04-12 20:25:40.000000 rdt_identity-1.4.0.dev0/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1359 2023-04-12 20:25:40.000000 rdt_identity-1.4.0.dev0/tests/unit/test__addons.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   103818 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/unit/test_hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.860070 rdt_identity-1.4.0.dev0/tests/unit/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.860234 rdt_identity-1.4.0.dev0/tests/unit/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/addons/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.860556 rdt_identity-1.4.0.dev0/tests/unit/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/addons/identity/test_identity.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:59:46.861041 rdt_identity-1.4.0.dev0/tests/unit/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-12 20:25:40.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/pii/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    38553 2023-04-12 20:25:40.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8522 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-12 20:25:40.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18913 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    20962 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/test_null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    61010 2023-01-18 20:52:41.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-12 20:25:40.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/test_text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1075 2022-08-17 01:38:30.000000 rdt_identity-1.4.0.dev0/tests/unit/transformers/test_utils.py
```

### Comparing `rdt_identity-1.3.1.dev0/CONTRIBUTING.rst` & `rdt_identity-1.4.0.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/HISTORY.md` & `rdt_identity-1.4.0.dev0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/LICENSE` & `rdt_identity-1.4.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/PKG-INFO` & `rdt_identity-1.4.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt_identity
-Version: 1.3.1.dev0
+Version: 1.4.0.dev0
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt,rdt_identity
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rdt_identity Version: 1.3.1.dev0 Summary:
+Metadata-Version: 2.1 Name: rdt_identity Version: 1.4.0.dev0 Summary:
 Reversible Data Transforms Home-page: https://github.com/sdv-dev/RDT Author:
 DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1 Keywords:
 rdt,rdt_identity Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: Free for non-commercial
 use Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `rdt_identity-1.3.1.dev0/README.md` & `rdt_identity-1.4.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/RELEASE.md` & `rdt_identity-1.4.0.dev0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/rdt/transformers/addons/identity/identity.py` & `rdt_identity-1.4.0.dev0/rdt/transformers/addons/identity/identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/setup.cfg` & `rdt_identity-1.4.0.dev0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.3.1.dev0
+current_version = 1.4.0.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `rdt_identity-1.3.1.dev0/setup.py` & `rdt_identity-1.4.0.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,10 +136,10 @@
         exclude=['rdt.transformers.addons.*']
     ),
     python_requires='>=3.7,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/RDT',
-    version='1.3.1.dev0',
+    version='1.4.0.dev0',
     zip_safe=False,
 )
```

### Comparing `rdt_identity-1.3.1.dev0/tests/__init__.py` & `rdt_identity-1.4.0.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/code_style.py` & `rdt_identity-1.4.0.dev0/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/contributing.py` & `rdt_identity-1.4.0.dev0/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/datasets/tests/test_boolean.py` & `rdt_identity-1.4.0.dev0/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/datasets/tests/test_categorical.py` & `rdt_identity-1.4.0.dev0/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/datasets/tests/test_datetime.py` & `rdt_identity-1.4.0.dev0/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/datasets/tests/test_numerical.py` & `rdt_identity-1.4.0.dev0/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/datasets/tests/test_utils.py` & `rdt_identity-1.4.0.dev0/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/integration/test_hyper_transformer.py` & `rdt_identity-1.4.0.dev0/tests/integration/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/integration/test_transformers.py` & `rdt_identity-1.4.0.dev0/tests/integration/test_transformers.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/integration/transformers/pii/test_anonymizer.py` & `rdt_identity-1.4.0.dev0/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/integration/transformers/test_base.py` & `rdt_identity-1.4.0.dev0/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/integration/transformers/test_boolean.py` & `rdt_identity-1.4.0.dev0/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/integration/transformers/test_categorical.py` & `rdt_identity-1.4.0.dev0/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/integration/transformers/test_datetime.py` & `rdt_identity-1.4.0.dev0/tests/integration/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/integration/transformers/test_numerical.py` & `rdt_identity-1.4.0.dev0/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/integration/transformers/test_text.py` & `rdt_identity-1.4.0.dev0/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/performance/test_performance.py` & `rdt_identity-1.4.0.dev0/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/performance/tests/test_profiling.py` & `rdt_identity-1.4.0.dev0/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/quality/dataset_info.csv` & `rdt_identity-1.4.0.dev0/tests/quality/dataset_info.csv`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/quality/test_quality.py` & `rdt_identity-1.4.0.dev0/tests/quality/test_quality.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/quality/utils.py` & `rdt_identity-1.4.0.dev0/tests/quality/utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/test___init__.py` & `rdt_identity-1.4.0.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/test__addons.py` & `rdt_identity-1.4.0.dev0/tests/unit/test__addons.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/test_hyper_transformer.py` & `rdt_identity-1.4.0.dev0/tests/unit/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/transformers/addons/identity/test_identity.py` & `rdt_identity-1.4.0.dev0/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/transformers/pii/test_anonymizer.py` & `rdt_identity-1.4.0.dev0/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/transformers/pii/test_utils.py` & `rdt_identity-1.4.0.dev0/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/transformers/test___init__.py` & `rdt_identity-1.4.0.dev0/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_base.py` & `rdt_identity-1.4.0.dev0/tests/unit/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_boolean.py` & `rdt_identity-1.4.0.dev0/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_categorical.py` & `rdt_identity-1.4.0.dev0/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_datetime.py` & `rdt_identity-1.4.0.dev0/tests/unit/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_null.py` & `rdt_identity-1.4.0.dev0/tests/unit/transformers/test_null.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_numerical.py` & `rdt_identity-1.4.0.dev0/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_text.py` & `rdt_identity-1.4.0.dev0/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_utils.py` & `rdt_identity-1.4.0.dev0/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*

