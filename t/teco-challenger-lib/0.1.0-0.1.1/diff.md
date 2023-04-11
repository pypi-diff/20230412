# Comparing `tmp/teco_challenger_lib-0.1.0.tar.gz` & `tmp/teco_challenger_lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teco_challenger_lib-0.1.0.tar", max compression
+gzip compressed data, was "teco_challenger_lib-0.1.1.tar", max compression
```

## Comparing `teco_challenger_lib-0.1.0.tar` & `teco_challenger_lib-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-04-11 16:38:45.069344 teco_challenger_lib-0.1.0/README.md
--rw-r--r--   0        0        0      368 2023-04-11 23:18:37.294152 teco_challenger_lib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 16:38:45.069344 teco_challenger_lib-0.1.0/teco_challenger_lib/__init__.py
--rw-r--r--   0        0        0    81981 2023-04-11 23:20:52.270225 teco_challenger_lib-0.1.0/teco_challenger_lib/teco-challenger-lib.py
--rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 teco_challenger_lib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-11 16:38:45.069344 teco_challenger_lib-0.1.1/README.md
+-rw-r--r--   0        0        0      367 2023-04-11 23:30:47.074875 teco_challenger_lib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-11 16:38:45.069344 teco_challenger_lib-0.1.1/teco_challenger_lib/__init__.py
+-rw-r--r--   0        0        0    81981 2023-04-11 23:20:52.270225 teco_challenger_lib-0.1.1/teco_challenger_lib/teco-challenger-lib.py
+-rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 teco_challenger_lib-0.1.1/PKG-INFO
```

### Comparing `teco_challenger_lib-0.1.0/teco_challenger_lib/teco-challenger-lib.py` & `teco_challenger_lib-0.1.1/teco_challenger_lib/teco-challenger-lib.py`

 * *Files identical despite different names*

