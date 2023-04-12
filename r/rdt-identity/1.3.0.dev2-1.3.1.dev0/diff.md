# Comparing `tmp/rdt_identity-1.3.0.dev2.tar.gz` & `tmp/rdt_identity-1.3.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt_identity-1.3.0.dev2.tar", last modified: Tue Jan 17 21:07:02 2023, max compression
+gzip compressed data, was "rdt_identity-1.3.1.dev0.tar", last modified: Wed Apr 12 20:29:55 2023, max compression
```

## Comparing `rdt_identity-1.3.0.dev2.tar` & `rdt_identity-1.3.1.dev0.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.190242 rdt_identity-1.3.0.dev2/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-06 20:41:33.000000 rdt_identity-1.3.0.dev2/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    25996 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    36568 2022-09-12 17:40:42.000000 rdt_identity-1.3.0.dev2/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-06 20:41:33.000000 rdt_identity-1.3.0.dev2/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8014 2023-01-17 21:07:02.190355 rdt_identity-1.3.0.dev2/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-06 20:41:33.000000 rdt_identity-1.3.0.dev2/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.180146 rdt_identity-1.3.0.dev2/rdt/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.180198 rdt_identity-1.3.0.dev2/rdt/transformers/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.180253 rdt_identity-1.3.0.dev2/rdt/transformers/addons/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.183230 rdt_identity-1.3.0.dev2/rdt/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/rdt/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/rdt/transformers/addons/identity/identity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-01-17 21:07:02.190869 rdt_identity-1.3.0.dev2/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4191 2023-01-06 21:06:17.000000 rdt_identity-1.3.0.dev2/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.183587 rdt_identity-1.3.0.dev2/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21679 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.180452 rdt_identity-1.3.0.dev2/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.184208 rdt_identity-1.3.0.dev2/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.184589 rdt_identity-1.3.0.dev2/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    38895 2023-01-06 20:41:33.000000 rdt_identity-1.3.0.dev2/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9333 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.185441 rdt_identity-1.3.0.dev2/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.185677 rdt_identity-1.3.0.dev2/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-06 20:41:33.000000 rdt_identity-1.3.0.dev2/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2512 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13321 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2312 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8679 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7220 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.186039 rdt_identity-1.3.0.dev2/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5070 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.186278 rdt_identity-1.3.0.dev2/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.3.0.dev2/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.186772 rdt_identity-1.3.0.dev2/tests/quality/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/quality/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    30119 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/quality/dataset_info.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9990 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/quality/test_quality.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1531 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/quality/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.187139 rdt_identity-1.3.0.dev2/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1191 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103818 2023-01-06 20:41:33.000000 rdt_identity-1.3.0.dev2/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.188930 rdt_identity-1.3.0.dev2/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.189073 rdt_identity-1.3.0.dev2/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.189455 rdt_identity-1.3.0.dev2/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-01-17 21:07:02.190065 rdt_identity-1.3.0.dev2/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27556 2023-01-06 20:41:33.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    38551 2023-01-12 19:40:17.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8522 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    59895 2023-01-17 21:05:02.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18913 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20962 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    61010 2022-12-14 19:23:29.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12684 2023-01-06 20:41:33.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1075 2022-08-17 01:38:30.000000 rdt_identity-1.3.0.dev2/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.498223 rdt_identity-1.3.1.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    25996 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    41255 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8014 2023-04-12 20:29:55.498329 rdt_identity-1.3.1.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.487164 rdt_identity-1.3.1.dev0/rdt/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.487230 rdt_identity-1.3.1.dev0/rdt/transformers/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.487295 rdt_identity-1.3.1.dev0/rdt/transformers/addons/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.490584 rdt_identity-1.3.1.dev0/rdt/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/rdt/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/rdt/transformers/addons/identity/identity.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-04-12 20:29:55.498857 rdt_identity-1.3.1.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4191 2023-01-18 20:53:13.000000 rdt_identity-1.3.1.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.491064 rdt_identity-1.3.1.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/code_style.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21679 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/contributing.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.487556 rdt_identity-1.3.1.dev0/tests/datasets/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.491823 rdt_identity-1.3.1.dev0/tests/datasets/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/datasets/tests/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/datasets/tests/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/datasets/tests/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/datasets/tests/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/datasets/tests/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.492289 rdt_identity-1.3.1.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    43118 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/integration/test_hyper_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9356 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/integration/test_transformers.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.493310 rdt_identity-1.3.1.dev0/tests/integration/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.493618 rdt_identity-1.3.1.dev0/tests/integration/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2512 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2312 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8679 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/integration/transformers/test_text.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.494043 rdt_identity-1.3.1.dev0/tests/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/performance/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/performance/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/performance/test_performance.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.494336 rdt_identity-1.3.1.dev0/tests/performance/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/performance/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.3.1.dev0/tests/performance/tests/test_profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.494942 rdt_identity-1.3.1.dev0/tests/quality/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/quality/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    30119 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/quality/dataset_info.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10032 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/quality/test_quality.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1531 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/quality/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.495533 rdt_identity-1.3.1.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1192 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1359 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/unit/test__addons.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   103818 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/test_hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.497182 rdt_identity-1.3.1.dev0/tests/unit/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.497329 rdt_identity-1.3.1.dev0/tests/unit/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/addons/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.497624 rdt_identity-1.3.1.dev0/tests/unit/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/addons/identity/test_identity.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-04-12 20:29:55.498089 rdt_identity-1.3.1.dev0/tests/unit/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/pii/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    38553 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8522 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18913 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    20962 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    61010 2023-01-18 20:52:41.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-12 20:25:40.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1075 2022-08-17 01:38:30.000000 rdt_identity-1.3.1.dev0/tests/unit/transformers/test_utils.py
```

### Comparing `rdt_identity-1.3.0.dev2/CONTRIBUTING.rst` & `rdt_identity-1.3.1.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/HISTORY.md` & `rdt_identity-1.3.1.dev0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,54 @@
 # History
 
+## 1.3.0 - 2023-01-18
+
+This release makes changes to the way that individual transformers are stored in the `HyperTransformer`. When accessing the config via `HyperTransformer.get_config()`, the transformers listed in the config are now the actual transformer instances used during fitting and transforming. These instances can now be accessed and used to examine their properties post fitting. For example, you can now view the mapping for a `PseudoAnonymizedFaker` instance using `PseudoAnonymizedFaker.get_mapping()` on the instance retrieved from the config.
+
+Additionally, the output of `reverse_tranform` no longer appends the `.value` suffix to every unnamed output column. Only output columns that are created from context extracted from the input columns will have suffixes (eg. `.normalized` in the `ClusterBasedNormalizer`).
+
+The `AnonymizedFaker` and `RegexGenerator` now have an `enforce_uniqueness` parameter, which controls whether the data returned by `reverse_transform` should be unique. The `HyperTransformer` now has a method called `create_anonymized_columns` that can be used to generate columns that are matched with anonymizing transformers like `AnonymizedFaker` and `RegexGenerator`. The method can be used as follows:
+`HyperTransformer.create_anonymized_columns(num_rows=5, column_names=['email_optin', 'credit_card'])`
+
+Another major change in this release is the ability to control randomization. Every time a `HyperTransformer` is initialized, its randomness will be reset to the same seed, and it will yield the same results for `reverse_transform` if given the same input. Every subsequent call to `reverse_transform` yields a different result. If a user desires to reset the seed, they can call `HyperTransformer.reset_randomization`.
+
+Finally, this release adds support for Python 3.10 and drops support for 3.6.
+
+### Bugs
+
+* The reset_randomization should also apply to fit and transform - Issue [#608](https://github.com/sdv-dev/RDT/issues/608) by @amontanez24
+* Cannot print CustomLabelEncoder: ValueError - Issue [#607](https://github.com/sdv-dev/RDT/issues/607) by @amontanez24
+* Float formatter learn_rounding_scheme doesn't work on all digits - Issue [#556](https://github.com/sdv-dev/RDT/issues/556) by @fealho
+* Warnings not showing on update_transformers_by_sdtype - Issue [#582](https://github.com/sdv-dev/RDT/issues/582) by @amontanez24
+* OneHotEncoder doesn't work with boolean sdtype - Issue [#583](https://github.com/sdv-dev/RDT/issues/583) by @pvk-developer
+* Setting config on HyperTransformer does not read supported_sdtypes - Issue [#560](https://github.com/sdv-dev/RDT/issues/560) by @pvk-developer
+* https://github.com/sdv-dev/RDT/issues/545 - Issue [#545](https://github.com/sdv-dev/RDT/issues/545) by @pvk-developer
+* Add error to NullTransformer when data only contains nans - PR [#567](https://github.com/sdv-dev/RDT/pull/567) by @fealho
+* Update update_transformers validation - PR [#563](https://github.com/sdv-dev/RDT/pull/563) by @fealho
+
+### Maintenance
+
+* Support Python 3.10 - Issue [#593](https://github.com/sdv-dev/RDT/issues/593) by @pvk-developer
+* RDT 1.3 Package Maintenance Updates - Issue [#594](https://github.com/sdv-dev/RDT/issues/594) by @pvk-developer
+
+### New Features
+
+* Update errors - Issue [#599](https://github.com/sdv-dev/RDT/issues/599) by @amontanez24
+* Add ability to control randomness - Issue [#584](https://github.com/sdv-dev/RDT/issues/584) by @amontanez24
+* Printing and error improvements - Issue [#581](https://github.com/sdv-dev/RDT/issues/581) by @amontanez24
+* Make RegexGenerator not to reset itself - Issue [#558](https://github.com/sdv-dev/RDT/issues/558) by @pvk-developer
+* Add a reset_anonymization method - Issue [#559](https://github.com/sdv-dev/RDT/issues/559) by @pvk-developer
+* Don't copy instances of tranformer - Issue [#541](https://github.com/sdv-dev/RDT/issues/541) by @fealho
+* Remove '.value' suffix - Issue [#533](https://github.com/sdv-dev/RDT/issues/533) by @fealho
+* Change the NEXT_TRANSFORMERS logic - Issue [#557](https://github.com/sdv-dev/RDT/issues/557) by @fealho
+* Add utility functions to AnonymizedFaker - Issue [#561](https://github.com/sdv-dev/RDT/issues/561) by @pvk-developer
+* Update API for update_transformers_by_sdtype to be more explicit about instances vs. copies - Issue [#540](https://github.com/sdv-dev/RDT/issues/540) by @fealho
+* Add create_anonymized_columns method to anonymize data from scratch - Issue [#546](https://github.com/sdv-dev/RDT/issues/546) by @pvk-developer
+* Add parameter to AnonymizedFaker() and RegexGenerator() to generate only unique values - Issue [#542](https://github.com/sdv-dev/RDT/issues/542) by @pvk-developer
+
 ## 1.2.1 - 2022-9-12
 
 This release fixes a bug that caused the `UnixTimestampEncoder` to return data with the incorrect datetime format. It also fixes a bug that caused the null column
 not to be reverse transformed when using the `UnixTimestampEncoder` when the `missing_value_replacement` was not set.
 
 ### Bugs
```

### Comparing `rdt_identity-1.3.0.dev2/LICENSE` & `rdt_identity-1.3.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/PKG-INFO` & `rdt_identity-1.3.1.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt_identity
-Version: 1.3.0.dev2
+Version: 1.3.1.dev0
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
-Metadata-Version: 2.1 Name: rdt_identity Version: 1.3.0.dev2 Summary:
+Metadata-Version: 2.1 Name: rdt_identity Version: 1.3.1.dev0 Summary:
 Reversible Data Transforms Home-page: https://github.com/sdv-dev/RDT Author:
 DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1 Keywords:
 rdt,rdt_identity Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: Free for non-commercial
 use Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `rdt_identity-1.3.0.dev2/README.md` & `rdt_identity-1.3.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/RELEASE.md` & `rdt_identity-1.3.1.dev0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/rdt/transformers/addons/identity/identity.py` & `rdt_identity-1.3.1.dev0/rdt/transformers/addons/identity/identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/setup.cfg` & `rdt_identity-1.3.1.dev0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.3.0.dev2
+current_version = 1.3.1.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `rdt_identity-1.3.0.dev2/setup.py` & `rdt_identity-1.3.1.dev0/setup.py`

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
-    version='1.3.0.dev2',
+    version='1.3.1.dev0',
     zip_safe=False,
 )
```

### Comparing `rdt_identity-1.3.0.dev2/tests/__init__.py` & `rdt_identity-1.3.1.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/code_style.py` & `rdt_identity-1.3.1.dev0/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/contributing.py` & `rdt_identity-1.3.1.dev0/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/datasets/tests/test_boolean.py` & `rdt_identity-1.3.1.dev0/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/datasets/tests/test_categorical.py` & `rdt_identity-1.3.1.dev0/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/datasets/tests/test_datetime.py` & `rdt_identity-1.3.1.dev0/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/datasets/tests/test_numerical.py` & `rdt_identity-1.3.1.dev0/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/datasets/tests/test_utils.py` & `rdt_identity-1.3.1.dev0/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/integration/test_hyper_transformer.py` & `rdt_identity-1.3.1.dev0/tests/integration/test_hyper_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from rdt import HyperTransformer, get_demo
 from rdt.errors import ConfigNotSetError, InvalidConfigError, InvalidDataError, NotFittedError
 from rdt.transformers import (
     AnonymizedFaker, BaseTransformer, BinaryEncoder, ClusterBasedNormalizer, FloatFormatter,
     FrequencyEncoder, LabelEncoder, OneHotEncoder, RegexGenerator, UnixTimestampEncoder,
     get_default_transformer, get_default_transformers)
+from rdt.transformers.pii.anonymizer import PseudoAnonymizedFaker
 
 
 class DummyTransformerNumerical(BaseTransformer):
 
     INPUT_SDTYPE = 'categorical'
 
     def _fit(self, data):
@@ -1094,44 +1095,43 @@
     pd.testing.assert_frame_equal(first_transformed1, expected_first_transformed)
     pd.testing.assert_frame_equal(first_transformed2, expected_first_transformed)
     pd.testing.assert_frame_equal(second_transformed1, expected_second_transformed)
 
     # test reverse transforming multiple times with different tranformers
     expected_first_reverse = pd.DataFrame({
         'credit_card': [
-            '180090934066211',
-            '30083012986584',
-            '2290394691481974',
-            '4444812351068428276',
-            '4875851017747494'
+            '3564483245479407',
+            '4863061245886958069',
+            '4039466324278480',
+            '4217004814656859',
+            '4343691397776091'
         ],
         'age': [18, 25, 54, 60, 31],
         'name': ['AAAAA', 'AAAAB', 'AAAAC', 'AAAAD', 'AAAAE'],
         'signup_day': [np.nan, '02/19/2016', '04/01/2019', np.nan, '05/16/2016'],
         'balance': [np.nan, 5400, 150000, np.nan, 91000],
         'card_type': ['Visa', 'Visa', 'Master Card', 'Amex', 'Visa']
     })
     expected_second_reverse = pd.DataFrame({
         'credit_card': [
-            '4228463375694866475',
-            '378224850315805',
-            '3568070297954787',
-            '4681503697026160',
-            '4490550771579'
+            '4208002654643',
+            '3547584322792794',
+            '30187802217181',
+            '4138954513622487900',
+            '346502559595986'
         ],
         'age': [18, 25, 54, 60, 31],
         'name': ['AAAAF', 'AAAAG', 'AAAAH', 'AAAAI', 'AAAAJ'],
         'signup_day': ['01/01/2020', '02/19/2016', np.nan, '12/01/2008', '05/16/2016'],
         'balance': [250, 5400, np.nan, 61662.5, 91000],
         'card_type': ['Visa', 'Visa', 'Master Card', 'Amex', 'Visa']
     })
     first_reverse1 = ht1.reverse_transform(first_transformed1)
     first_reverse2 = ht2.reverse_transform(first_transformed1)
     second_reverse1 = ht1.reverse_transform(first_transformed1)
-
     pd.testing.assert_frame_equal(first_reverse1, expected_first_reverse)
     pd.testing.assert_frame_equal(first_reverse2, expected_first_reverse)
     pd.testing.assert_frame_equal(expected_second_reverse, second_reverse1)
 
     # Test resetting randomization
     ht1.reset_randomization()
 
@@ -1163,7 +1163,145 @@
     ht2.detect_initial_config(data)
     ht2.update_transformers({
         'age': ClusterBasedNormalizer()
     })
     ht2.fit(data)
 
     pd.testing.assert_frame_equal(transformed1, ht2.transform(data))
+
+
+def test_hypertransformer_anonymized_faker():
+    """Test ``AnonymizedFaker`` generates different random values for different columns.
+
+    Issue: https://github.com/sdv-dev/RDT/issues/619.
+    """
+    # Setup
+    data = pd.DataFrame({
+        'id1': ['a', 'b', 'c'],
+        'id2': ['d', 'e', 'f'],
+    })
+    ht = HyperTransformer()
+
+    # Run - simple run
+    ht.detect_initial_config(data)
+    ht.update_sdtypes({
+        'id1': 'pii',
+        'id2': 'pii'
+    })
+    ht.update_transformers({
+        'id1': AnonymizedFaker(),
+        'id2': AnonymizedFaker()
+    })
+    ht.fit(data)
+    transformed = ht.transform(data)
+    reverse_transformed1 = ht.reverse_transform(transformed)
+
+    # Assert
+    assert reverse_transformed1['id1'].tolist() != reverse_transformed1['id2'].tolist()
+
+    # Run - make sure transforming again returns different values than the original transform
+    transformed = ht.transform(data)
+    reverse_transformed2 = ht.reverse_transform(transformed)
+
+    # Assert
+    assert reverse_transformed2['id1'].tolist() != reverse_transformed2['id2'].tolist()
+    assert reverse_transformed1['id1'].tolist() != reverse_transformed2['id1'].tolist()
+    assert reverse_transformed1['id2'].tolist() != reverse_transformed2['id2'].tolist()
+
+    # Run - make sure resetting randomization works
+    ht.reset_randomization()
+    transformed = ht.transform(data)
+    reverse_transformed3 = ht.reverse_transform(transformed)
+
+    # Assert
+    pd.testing.assert_frame_equal(reverse_transformed1, reverse_transformed3)
+
+
+def test_hypertransformer_pseudo_anonymized_faker():
+    """Test ``PseudoAnonymizedFaker`` generates different random values for different columns."""
+    # Setup
+    data = pd.DataFrame({
+        'id1': ['a', 'b', 'c'],
+        'id2': ['a', 'b', 'c'],
+    })
+    ht = HyperTransformer()
+
+    # Run
+    ht.detect_initial_config(data)
+    ht.update_sdtypes({
+        'id1': 'pii',
+        'id2': 'pii'
+    })
+    ht.update_transformers({
+        'id1': PseudoAnonymizedFaker(),
+        'id2': PseudoAnonymizedFaker()
+    })
+    ht.fit(data)
+    transformed = ht.transform(data)
+    reverse_transformed1 = ht.reverse_transform(transformed)
+
+    # Assert
+    assert reverse_transformed1['id1'].tolist() != reverse_transformed1['id2'].tolist()
+
+    # Run - run it again on the exact same data
+    ht = HyperTransformer()
+    ht.detect_initial_config(data)
+    ht.update_sdtypes({
+        'id1': 'pii',
+        'id2': 'pii'
+    })
+    ht.update_transformers({
+        'id1': PseudoAnonymizedFaker(),
+        'id2': PseudoAnonymizedFaker()
+    })
+    ht.fit(data)
+    transformed = ht.transform(data)
+    reverse_transformed2 = ht.reverse_transform(transformed)
+
+    # Assert - different instances of the same transformer should return the same result
+    assert reverse_transformed1['id1'].tolist() == reverse_transformed2['id1'].tolist()
+
+
+def test_hypertransformer_anonymized_faker_multi_table():
+    """Test ``AnonymizedFaker`` generates different values for columns with same name."""
+    # Setup
+    data1 = pd.DataFrame({
+        'id1': ['a', 'b', 'c'],
+        'id2': ['a', 'b', 'c'],
+    })
+    data2 = pd.DataFrame({
+        'id1': ['d', 'e', 'f'],
+        'id2': ['d', 'e', 'f'],
+    })
+    ht = HyperTransformer()
+
+    # Run on data1
+    ht.detect_initial_config(data1)
+    ht.update_sdtypes({
+        'id1': 'pii',
+        'id2': 'pii'
+    })
+    ht.update_transformers({
+        'id1': AnonymizedFaker(),
+        'id2': PseudoAnonymizedFaker()
+    })
+    ht.fit(data1)
+    transformed = ht.transform(data1)
+    reverse_transformed1 = ht.reverse_transform(transformed)
+
+    # Run on data2
+    ht.detect_initial_config(data2)
+    ht.update_sdtypes({
+        'id1': 'pii',
+        'id2': 'pii'
+    })
+    ht.update_transformers({
+        'id1': AnonymizedFaker(),
+        'id2': PseudoAnonymizedFaker()
+    })
+    ht.fit(data2)
+    transformed = ht.transform(data2)
+    reverse_transformed2 = ht.reverse_transform(transformed)
+
+    # Assert
+    assert reverse_transformed1['id1'].tolist() != reverse_transformed2['id1'].tolist()
+    assert reverse_transformed1['id2'].tolist() != reverse_transformed2['id2'].tolist()
```

### Comparing `rdt_identity-1.3.0.dev2/tests/integration/test_transformers.py` & `rdt_identity-1.3.1.dev0/tests/integration/test_transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         steps.append(validator_function.__name__)
 
     validator_function(*args)
 
 
 def _is_valid_transformer(transformer_name):
     """Determine if transformer should be tested or not."""
-    invalid_names = ['IdentityTransformer', 'Dummy', 'CustomLabelEncoder']
+    invalid_names = ['IdentityTransformer', 'Dummy', 'OrderedLabelEncoder', 'CustomLabelEncoder']
     return all(invalid_name not in transformer_name for invalid_name in invalid_names)
 
 
 def _get_all_transformers():
     """Get all transformers to be tested."""
     all_transformers = BaseTransformer.get_subclasses()
     return [t for t in all_transformers if _is_valid_transformer(t.__name__)]
```

### Comparing `rdt_identity-1.3.0.dev2/tests/integration/transformers/pii/test_anonymizer.py` & `rdt_identity-1.3.1.dev0/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/integration/transformers/test_base.py` & `rdt_identity-1.3.1.dev0/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/integration/transformers/test_boolean.py` & `rdt_identity-1.3.1.dev0/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/integration/transformers/test_categorical.py` & `rdt_identity-1.3.1.dev0/tests/integration/transformers/test_categorical.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pickle
 from io import BytesIO
 from unittest.mock import Mock, patch
 
 import numpy as np
 import pandas as pd
 
-from rdt.transformers import CustomLabelEncoder, FrequencyEncoder, LabelEncoder, OneHotEncoder
+from rdt.transformers import FrequencyEncoder, LabelEncoder, OneHotEncoder, OrderedLabelEncoder
 
 
 def test_frequency_encoder_numerical_nans():
     """Ensure FrequencyEncoder works on numerical + nan only columns."""
 
     data = pd.DataFrame([1, 2, float('nan'), np.nan], columns=['column_name'])
     column = 'column_name'
@@ -370,50 +370,50 @@
     reverse = transformer.reverse_transform(transformed)
 
     expected = pd.DataFrame([1, 3, 4, 2, 0], columns=['column_name'])
     pd.testing.assert_frame_equal(transformed, expected)
     pd.testing.assert_frame_equal(reverse, data)
 
 
-def test_custom_label_encoder():
-    """Test the CustomLabelEncoder end to end.
+def test_ordered_label_encoder():
+    """Test the OrderedLabelEncoder end to end.
 
     Input:
         - pandas.DataFrame of different types of data.
 
     Output:
         - Transformed data should have values based on the provided order.
         - Reverse transformed data should match the input
     """
 
     data = pd.DataFrame(['two', 3, 1, np.nan, 'zero'], columns=['column_name'])
-    transformer = CustomLabelEncoder(order=['zero', 1, 'two', 3, np.nan])
+    transformer = OrderedLabelEncoder(order=['zero', 1, 'two', 3, np.nan])
     transformer.fit(data, 'column_name')
 
     transformed = transformer.transform(data)
     reverse = transformer.reverse_transform(transformed)
 
     expected = pd.DataFrame([2, 3, 1, 4, 0], columns=['column_name'])
     pd.testing.assert_frame_equal(transformed, expected)
     pd.testing.assert_frame_equal(reverse, data)
 
 
-def test_custom_label_encoder_nans():
-    """The the CustomLabelEncoder with missing values.
+def test_ordered_label_encoder_nans():
+    """The the OrderedLabelEncoder with missing values.
 
     Input:
         - pandas.DataFrame of different types of data and different types of missing values.
 
     Output:
         - Transformed data should have values based on the provided order.
         - Reverse transformed data should match the input
     """
 
     data = pd.DataFrame(['two', 3, 1, np.nan, 'zero', None], columns=['column_name'])
-    transformer = CustomLabelEncoder(order=['zero', 1, 'two', 3, None])
+    transformer = OrderedLabelEncoder(order=['zero', 1, 'two', 3, None])
     transformer.fit(data, 'column_name')
 
     transformed = transformer.transform(data)
     reverse = transformer.reverse_transform(transformed)
 
     expected = pd.DataFrame([2, 3, 1, 4, 0, 4], columns=['column_name'])
     pd.testing.assert_frame_equal(transformed, expected)
```

### Comparing `rdt_identity-1.3.0.dev2/tests/integration/transformers/test_datetime.py` & `rdt_identity-1.3.1.dev0/tests/integration/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/integration/transformers/test_numerical.py` & `rdt_identity-1.3.1.dev0/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/integration/transformers/test_text.py` & `rdt_identity-1.3.1.dev0/tests/integration/transformers/test_text.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,46 +4,52 @@
 import pandas as pd
 
 from rdt.transformers.text import RegexGenerator
 
 
 def test_regexgenerator():
     """Test ``RegexGenerator`` with the default parameters."""
+    # Setup
     data = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
         'username': ['a', 'b', 'c', 'd', 'e']
     })
 
+    # Run
     instance = RegexGenerator()
     transformed = instance.fit_transform(data, 'id')
     reverse_transform = instance.reverse_transform(transformed)
 
+    # Assert
     expected_transformed = pd.DataFrame({
         'username': ['a', 'b', 'c', 'd', 'e']
     })
     expected_reverse_transformed = pd.DataFrame({
         'username': ['a', 'b', 'c', 'd', 'e'],
         'id': ['AAAAA', 'AAAAB', 'AAAAC', 'AAAAD', 'AAAAE'],
     })
 
     pd.testing.assert_frame_equal(transformed, expected_transformed)
     pd.testing.assert_frame_equal(reverse_transform, expected_reverse_transformed)
 
 
 def test_regexgenerator_with_custom_regex():
     """Test the ``RegexGenerator`` with a custom regex format."""
+    # Setup
     data = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
         'username': ['a', 'b', 'c', 'd', 'e'],
     })
 
+    # Run
     instance = RegexGenerator(regex_format='[1-9]')
     transformed = instance.fit_transform(data, 'id')
     reverse_transform = instance.reverse_transform(transformed)
 
+    # Assert
     expected_transformed = pd.DataFrame({
         'username': ['a', 'b', 'c', 'd', 'e'],
     })
 
     expected_reverse_transformed = pd.DataFrame({
         'username': ['a', 'b', 'c', 'd', 'e'],
         'id': ['1', '2', '3', '4', '5'],
@@ -51,23 +57,26 @@
 
     pd.testing.assert_frame_equal(transformed, expected_transformed)
     pd.testing.assert_frame_equal(reverse_transform, expected_reverse_transformed)
 
 
 def test_regexgenerator_with_nans():
     """Test the ``RegexGenerator`` with a custom regex format and ``nans``."""
+    # Setup
     data = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
         'username': ['a', np.nan, 'c', 'd', 'e']
     })
 
+    # Run
     instance = RegexGenerator('[A-Z]')
     transformed = instance.fit_transform(data, 'username')
     reverse_transform = instance.reverse_transform(transformed)
 
+    # Assert
     expected_transformed = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
     })
 
     expected_reverse_transformed = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
         'username': ['A', 'B', 'C', 'D', 'E'],
@@ -75,23 +84,26 @@
 
     pd.testing.assert_frame_equal(transformed, expected_transformed)
     pd.testing.assert_frame_equal(reverse_transform, expected_reverse_transformed)
 
 
 def test_regexgenerator_data_length_bigger_than_regex():
     """Test the ``RegexGenerator`` with short regex and more data length."""
+    # Setup
     data = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
         'username': ['a', np.nan, 'c', 'd', 'e']
     })
 
+    # Run
     instance = RegexGenerator('[a-b]')
     transformed = instance.fit_transform(data, 'username')
     reverse_transform = instance.reverse_transform(transformed)
 
+    # Assert
     expected_transformed = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
     })
 
     expected_reverse_transformed = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
         'username': ['a', 'b', 'a', 'b', 'a'],
@@ -99,27 +111,30 @@
 
     pd.testing.assert_frame_equal(transformed, expected_transformed)
     pd.testing.assert_frame_equal(reverse_transform, expected_reverse_transformed)
 
 
 def test_regexgenerator_input_data_bigger_than_data_length():
     """Test the ``RegexGenerator`` with input dataframe bigger than the learned data length."""
+    # Setup
     data = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
         'username': ['a', 'b', 'c', 'd', 'e']
     })
 
+    # Run
     instance = RegexGenerator('[a-b]')
     instance.fit(data, 'username')
 
     transformed = pd.DataFrame({
         'id': [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
     })
     reverse_transform = instance.reverse_transform(transformed)
 
+    # Assert
     expected_reverse_transformed = pd.DataFrame({
         'id': [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
         'username': ['a', 'b', 'a', 'b', 'a', 'b', 'a', 'b', 'a', 'b'],
     })
 
     pd.testing.assert_frame_equal(reverse_transform, expected_reverse_transformed)
 
@@ -198,25 +213,54 @@
     })
     pd.testing.assert_frame_equal(first_reverse_transform, expected_first_reverse_transform)
     pd.testing.assert_frame_equal(second_reverse_transform, expected_second_reverse_transform)
 
 
 def test_regexgenerator_pickled(tmpdir):
     """Test that ensures that ``RegexGenerator`` can be pickled."""
+    # Setup
     data = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
         'username': ['a', 'b', 'c', 'd', 'e']
     })
 
+    # Run
     instance = RegexGenerator()
     transformed = instance.fit_transform(data, 'id')
     instance.reverse_transform(transformed)
 
     # Pickle
     with open(tmpdir / 'file.pkl', 'wb') as f:
         pickle.dump(instance, f)
 
     with open(tmpdir / 'file.pkl', 'rb') as f:
         loaded = pickle.load(f)
 
     # Assert
     assert next(instance.generator) == next(loaded.generator)
+
+
+def test_regexgenerator_with_many_possibilities():
+    """Test the ``RegexGenerator`` with regex containing many possibilities."""
+    # Setup
+    data = pd.DataFrame({
+        'id': ['a' * 50, 'a' * 49 + 'b', 'a' * 49 + 'c', 'a' * 49 + 'd', 'a' * 49 + 'e'],
+        'username': ['aa', 'bb', 'cc', 'dd', 'ee'],
+    })
+
+    # Run
+    instance = RegexGenerator(regex_format='[a-z]{50}')
+    transformed = instance.fit_transform(data, 'id')
+    reverse_transform = instance.reverse_transform(transformed)
+
+    # Assert
+    expected_transformed = pd.DataFrame({
+        'username': ['aa', 'bb', 'cc', 'dd', 'ee'],
+    })
+
+    expected_reverse_transformed = pd.DataFrame({
+        'username': ['aa', 'bb', 'cc', 'dd', 'ee'],
+        'id': ['a' * 50, 'a' * 49 + 'b', 'a' * 49 + 'c', 'a' * 49 + 'd', 'a' * 49 + 'e'],
+    })
+
+    pd.testing.assert_frame_equal(transformed, expected_transformed)
+    pd.testing.assert_frame_equal(reverse_transform, expected_reverse_transformed)
```

### Comparing `rdt_identity-1.3.0.dev2/tests/performance/test_performance.py` & `rdt_identity-1.3.1.dev0/tests/performance/test_performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import pandas as pd
 import pytest
 
 from rdt.performance.datasets import get_dataset_generators_by_type
 from rdt.performance.performance import evaluate_transformer_performance
 from rdt.performance.profiling import profile_transformer
 from rdt.transformers import get_transformers_by_type
-from rdt.transformers.categorical import CustomLabelEncoder
+from rdt.transformers.categorical import CustomLabelEncoder, OrderedLabelEncoder
 from rdt.transformers.numerical import ClusterBasedNormalizer
 
-SANDBOX_TRANSFORMERS = [ClusterBasedNormalizer, CustomLabelEncoder]
+SANDBOX_TRANSFORMERS = [ClusterBasedNormalizer, OrderedLabelEncoder, CustomLabelEncoder]
 
 
 def _get_performance_test_cases():
     """Get all the (transformer, dataset_generator) combinations for testing."""
     all_test_cases = []
 
     dataset_generators = get_dataset_generators_by_type()
```

### Comparing `rdt_identity-1.3.0.dev2/tests/performance/tests/test_profiling.py` & `rdt_identity-1.3.1.dev0/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/quality/dataset_info.csv` & `rdt_identity-1.3.1.dev0/tests/quality/dataset_info.csv`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/quality/test_quality.py` & `rdt_identity-1.3.1.dev0/tests/quality/test_quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import numpy as np
 import pandas as pd
 from sklearn.linear_model import LinearRegression
 from sklearn.model_selection import cross_val_score
 
 from rdt import HyperTransformer
-from rdt.transformers import CustomLabelEncoder, FloatFormatter, get_transformers_by_type
+from rdt.transformers import (
+    CustomLabelEncoder, FloatFormatter, OrderedLabelEncoder, get_transformers_by_type)
 from tests.quality.utils import download_single_table
 
 R2_THRESHOLD = 0.2
 TEST_THRESHOLD = 0.3
 MAX_SIZE = 5000000
 SDTYPES_TO_SKIP = {'numerical', 'float', 'integer', 'id', None}
 
@@ -19,15 +20,15 @@
     'numerical': ['number'],
     'float': ['float'],
     'int': ['int'],
     'categorical': ['object', 'category'],
     'datetime': ['datetime'],
     'boolean': ['bool']
 }
-TRANSFORMERS_TO_SKIP = [CustomLabelEncoder]
+TRANSFORMERS_TO_SKIP = [OrderedLabelEncoder, CustomLabelEncoder]
 
 
 def format_array(array):
     if not isinstance(array, np.ndarray):
         array = array.to_numpy()
 
     if len(array.shape) == 1:
@@ -224,19 +225,18 @@
         of the average score for the dataset across all transformers of the same
         sdtype.
         4. For every unique transformer in the results, a test is run to check
         that the transformer's score for each table is either higher than the
         threshold, or the comparitive score is higher than the threshold.
     """
     transformers_by_type = get_transformers_by_type()
-    for transformer_list in transformers_by_type.values():
-        for transformer in transformer_list:
-            if transformer in TRANSFORMERS_TO_SKIP:
-                transformer_list.remove(transformer)
-
+    transformers_by_type = {
+        transformer_type: [t for t in transformer_list if t not in TRANSFORMERS_TO_SKIP]
+        for transformer_type, transformer_list in transformers_by_type.items()
+    }
     sdtypes_to_test = {
         sdtype
         for sdtype in transformers_by_type.keys()
         if sdtype not in SDTYPES_TO_SKIP
     }
     test_cases = get_test_cases(sdtypes_to_test)
     all_regression_scores = get_regression_scores(test_cases, transformers_by_type)
```

### Comparing `rdt_identity-1.3.0.dev2/tests/quality/utils.py` & `rdt_identity-1.3.1.dev0/tests/quality/utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/test___init__.py` & `rdt_identity-1.3.1.dev0/tests/unit/test___init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 import numpy as np
 import pandas as pd
 
 from rdt import get_demo
 
 
 def test_get_demo():
```

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/test_hyper_transformer.py` & `rdt_identity-1.3.1.dev0/tests/unit/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/transformers/addons/identity/test_identity.py` & `rdt_identity-1.3.1.dev0/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/transformers/pii/test_anonymizer.py` & `rdt_identity-1.3.1.dev0/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,50 +15,55 @@
 
 
 class TestAnonymizedFaker:
     """Test class for ``AnonymizedFaker``."""
 
     @patch('rdt.transformers.pii.anonymizer.faker')
     @patch('rdt.transformers.pii.anonymizer.getattr')
-    def test_check_provider_function_baseprovider(self, mock_getattr, mock_faker):
+    @patch('rdt.transformers.pii.anonymizer.attrgetter')
+    def test_check_provider_function_baseprovider(self, mock_attrgetter, mock_getattr, mock_faker):
         """Test that ``getattr`` is being called with ``BaseProvider`` and ``function_name``.
 
         Mock:
             - Mock the ``getattr`` from Python to ensure that is being called with the input.
             - Mock faker and ensure that ``getattr`` is being called with ``faker.providers``.
         """
         # Setup
-        mock_getattr.side_effect = ['module', 'provider', None]
+        mock_attrgetter.return_value = lambda x: 'module'
+        mock_getattr.side_effect = ['provider', None]
 
         # Run
         AnonymizedFaker.check_provider_function('BaseProvider', 'function_name')
 
         # Assert
-        assert mock_getattr.call_args_list[0] == call(mock_faker.providers, 'BaseProvider')
-        assert mock_getattr.call_args_list[1] == call('module', 'function_name')
+        assert mock_attrgetter.call_args_list[0] == call('BaseProvider')
+        assert mock_getattr.call_args_list[0] == call('module', 'function_name')
 
     @patch('rdt.transformers.pii.anonymizer.faker')
     @patch('rdt.transformers.pii.anonymizer.getattr')
-    def test_check_provider_function_other_providers(self, mock_getattr, mock_faker):
+    @patch('rdt.transformers.pii.anonymizer.attrgetter')
+    def test_check_provider_function_other_providers(self, mock_attrgetter, mock_getattr,
+                                                     mock_faker):
         """Test that ``getattr`` is being called with ``provider_name`` and ``function_name``.
 
         Mock:
             - Mock the ``getattr`` from Python to ensure that is being called with the input.
             - Mock faker and ensure that ``getattr`` is being called with ``faker.providers``.
         """
         # Setup
-        mock_getattr.side_effect = ['module', 'provider_class', None]
+        mock_attrgetter.return_value = lambda x: 'module'
+        mock_getattr.side_effect = ['provider_class', None]
 
         # Run
         AnonymizedFaker.check_provider_function('provider_name', 'function_name')
 
         # Assert
-        assert mock_getattr.call_args_list[0] == call(mock_faker.providers, 'provider_name')
-        assert mock_getattr.call_args_list[1] == call('module', 'Provider')
-        assert mock_getattr.call_args_list[2] == call('provider_class', 'function_name')
+        assert mock_attrgetter.call_args_list[0] == call('provider_name')
+        assert mock_getattr.call_args_list[0] == call('module', 'Provider')
+        assert mock_getattr.call_args_list[1] == call('provider_class', 'function_name')
 
     def test_check_provider_function_raise_attribute_error(self):
         """Test that ``check_provider_function`` raises an ``AttributeError``.
 
         Test when the provider class is not in the ``faker.providers`` an ``AttributeError`` is
         being raised or when the ``function`` is not within the ``provider``.
         """
@@ -304,14 +309,15 @@
 
         Side Effects:
             - ``instance.data_length`` equals to the length of the input data.
         """
         # Setup
         transformer = AnonymizedFaker()
         columns_data = pd.Series(['1', '2', '3'])
+        transformer.columns = ['col']
 
         # Run
         transformer._fit(columns_data)
 
         # Assert
         assert transformer.data_length == 3
         assert transformer.output_properties == {None: {'next_transformer': None}}
@@ -608,14 +614,15 @@
             - ``instance._reverse_mapping_dict`` contains the ``_function`` returned values as keys
               and the input data as values.
         """
         # Setup
         instance = PseudoAnonymizedFaker()
         instance._function = Mock()
         instance._function.side_effect = [1, 2, 3]
+        instance.columns = ['col']
         data = pd.Series(['a', 'b', 'c'])
 
         # Run
         instance._fit(data)
 
         # Assert
         assert instance._mapping_dict == {'a': 1, 'b': 2, 'c': 3}
@@ -644,14 +651,15 @@
             - Mock the ``instance._function`` to return only 1 value.
 
         Side Effect:
             - Raises an error.
         """
         # Setup
         instance = PseudoAnonymizedFaker('misc', 'boolean')
+        instance.columns = ['col']
         data = pd.Series(['a', 'b', 'c', 'd'])
 
         # Run / Assert
         error_msg = (
             'The Faker function you specified is not able to generate '
             '4 unique values. Please use a different '
             'Faker function for this column.'
```

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/transformers/pii/test_utils.py` & `rdt_identity-1.3.1.dev0/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/transformers/test___init__.py` & `rdt_identity-1.3.1.dev0/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/transformers/test_base.py` & `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -931,15 +931,15 @@
         """
         # Setup
         data = pd.DataFrame({
             'a': [1, 2, 3],
             'b': [4, 5, 6],
             'c': [7, 8, 9]
         })
-        column = 'a'
+        column = ['a']
 
         class Dummy(BaseTransformer):
             def __init__(self):
                 super().__init__()
                 self.output_properties = {
                     None: {'sdtype': 'categorical'},
                     'is_null': {'sdtype': 'float'}
```

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/transformers/test_boolean.py` & `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/transformers/test_categorical.py` & `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_categorical.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from rdt.errors import TransformerInputError
 from rdt.transformers.categorical import (
-    CustomLabelEncoder, FrequencyEncoder, LabelEncoder, OneHotEncoder)
+    CustomLabelEncoder, FrequencyEncoder, LabelEncoder, OneHotEncoder, OrderedLabelEncoder)
 
 RE_SSN = re.compile(r'\d\d\d-\d\d-\d\d\d\d')
 
 
 class TestFrequencyEncoder:
 
     def test___setstate__(self):
@@ -1790,77 +1790,77 @@
         # Run
         out = transformer._reverse_transform(data)
 
         # Assert
         pd.testing.assert_series_equal(out, pd.Series(['a', 'b', 'c']))
 
 
-class TestCustomLabelEncoder:
+class TestOrderedLabelEncoder:
 
     def test___init__(self):
         """The the ``__init__`` method.
 
         Passed arguments must be stored as attributes.
         """
         # Run
-        transformer = CustomLabelEncoder(order=['b', 'c', 'a', None], add_noise='add_noise_value')
+        transformer = OrderedLabelEncoder(order=['b', 'c', 'a', None], add_noise='add_noise_value')
 
         # Asserts
         assert transformer.add_noise == 'add_noise_value'
         pd.testing.assert_series_equal(transformer.order, pd.Series(['b', 'c', 'a', np.nan]))
 
     def test___repr___default(self):
         """Test that the ``__repr__`` method prints the custom order.
 
         The order should be printed as <CUSTOM> instead of the actual order.
         """
         # Setup
-        transformer = CustomLabelEncoder(order=['VISA', 'AMEX', 'DISCOVER', None])
+        transformer = OrderedLabelEncoder(order=['VISA', 'AMEX', 'DISCOVER', None])
 
         # Run
         stringified_transformer = transformer.__repr__()
 
         # Assert
-        assert stringified_transformer == 'CustomLabelEncoder(order=<CUSTOM>)'
+        assert stringified_transformer == 'OrderedLabelEncoder(order=<CUSTOM>)'
 
     def test___repr___add_noise_true(self):
         """Test that the ``__repr__`` method prints the custom order with ``add_noise``.
 
         The order should be printed as <CUSTOM> instead of the actual order. If ``add_noise``
         is provided, it should be printed too.
         """
         # Setup
-        transformer = CustomLabelEncoder(order=['VISA', 'AMEX', 'DISCOVER', None], add_noise=True)
+        transformer = OrderedLabelEncoder(order=['VISA', 'AMEX', 'DISCOVER', None], add_noise=True)
 
         # Run
         stringified_transformer = transformer.__repr__()
 
         # Assert
-        assert stringified_transformer == 'CustomLabelEncoder(order=<CUSTOM>, add_noise=True)'
+        assert stringified_transformer == 'OrderedLabelEncoder(order=<CUSTOM>, add_noise=True)'
 
     def test__fit(self):
         """Test the ``_fit`` method.
 
         Validate that a unique integer representation for each category of the data is stored
         in the ``categories_to_values`` attribute, and the reverse is stored in the
         ``values_to_categories`` attribute. The order should match the ``self.order`` indices.
 
         Setup:
-            - create an instance of the ``CustomLabelEncoder``.
+            - create an instance of the ``OrderedLabelEncoder``.
 
         Input:
             - a pandas series.
 
         Side effects:
             - set the ``values_to_categories`` dictionary to the appropriate value.
             - set ``categories_to_values`` dictionary to the appropriate value.
         """
         # Setup
         data = pd.Series([1, 2, 3, 2, np.nan, 1])
-        transformer = CustomLabelEncoder(order=[2, 3, np.nan, 1])
+        transformer = OrderedLabelEncoder(order=[2, 3, np.nan, 1])
 
         # Run
         transformer._fit(data)
 
         # Assert
         expected_values_to_categories = {0: 2, 1: 3, 2: np.nan, 3: 1}
         expected_categories_to_values = {2: 0, 3: 1, 1: 3, np.nan: 2}
@@ -1872,27 +1872,40 @@
 
     def test__fit_error(self):
         """Test the ``_fit`` method checks that data is in ``self.order``.
 
         If the data being fit is not in ``self.order`` an error should be raised.
 
         Setup:
-            - create an instance of the ``CustomLabelEncoder``.
+            - create an instance of the ``OrderedLabelEncoder``.
 
         Input:
             - a pandas series.
 
         Side effects:
             - set the ``values_to_categories`` dictionary to the appropriate value.
             - set ``categories_to_values`` dictionary to the appropriate value.
         """
         # Setup
         data = pd.Series([1, 2, 3, 2, 1, 4])
-        transformer = CustomLabelEncoder(order=[2, 1])
+        transformer = OrderedLabelEncoder(order=[2, 1])
 
         # Run / Assert
         message = re.escape(
             "Unknown categories '[3, 4]'. All possible categories must be defined in the "
             "'order' parameter."
         )
         with pytest.raises(TransformerInputError, match=message):
             transformer._fit(data)
+
+
+class TestCustomLabelEncoder:
+
+    def test___init__(self):
+        """Test the warning message for  backwards compatibility of ``CustomLabelEncoder``."""
+        # Setup / Run / Assert
+        warning_msg = re.escape(
+            "The 'CustomLabelEncoder' is renamed to 'OrderedLabelEncoder'. Please update the"
+            'name to ensure compatibility with future versions of RDT.'
+        )
+        with pytest.warns(FutureWarning, match=warning_msg):
+            CustomLabelEncoder(order=[2, 1])
```

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/transformers/test_datetime.py` & `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/transformers/test_null.py` & `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_null.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/transformers/test_numerical.py` & `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/transformers/test_text.py` & `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         assert state == {
             'data_length': None,
             'enforce_uniqueness': False,
             'generated': 0,
             'generator_size': 380204032,
             'output_properties': {None: {'next_transformer': None}},
             'regex_format': '[A-Za-z]{5}',
-            'random_states': mock_random_sates
+            'random_states': mock_random_sates,
         }
 
     @patch('rdt.transformers.text.strings_from_regex')
     def test___setstate__generated_and_generator_size(self, mock_strings_from_regex):
         """Test that ``__setstate__`` will initialize a generator and wind it forward."""
         # Setup
         state = {
```

### Comparing `rdt_identity-1.3.0.dev2/tests/unit/transformers/test_utils.py` & `rdt_identity-1.3.1.dev0/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*

