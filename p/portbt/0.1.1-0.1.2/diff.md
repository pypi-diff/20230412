# Comparing `tmp/portbt-0.1.1.tar.gz` & `tmp/portbt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portbt-0.1.1.tar", max compression
+gzip compressed data, was "portbt-0.1.2.tar", max compression
```

## Comparing `portbt-0.1.1.tar` & `portbt-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      125 2023-04-11 22:16:42.242993 portbt-0.1.1/portbt/__init__.py
--rw-r--r--   0        0        0     3139 2023-04-11 22:35:26.638321 portbt-0.1.1/portbt/backtest_functions.py
--rw-r--r--   0        0        0     1355 2023-04-11 22:19:38.696933 portbt-0.1.1/portbt/portfolio.py
--rw-r--r--   0        0        0      658 2023-04-11 22:15:59.356410 portbt-0.1.1/portbt/utils.py
--rw-r--r--   0        0        0      431 2023-04-11 22:40:32.625612 portbt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 16:54:48.162724 portbt-0.1.1/README.md
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 portbt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 portbt-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      127 2023-04-12 00:16:50.304309 portbt-0.1.2/portbt/__init__.py
+-rw-r--r--   0        0        0     3139 2023-04-11 22:35:26.638321 portbt-0.1.2/portbt/backtest_functions.py
+-rw-r--r--   0        0        0     1643 2023-04-12 02:22:47.006848 portbt-0.1.2/portbt/portfolio.py
+-rw-r--r--   0        0        0      658 2023-04-11 22:15:59.356410 portbt-0.1.2/portbt/utils.py
+-rw-r--r--   0        0        0      575 2023-04-12 02:38:04.522063 portbt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-04-12 02:39:37.960111 portbt-0.1.2/README.md
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 portbt-0.1.2/PKG-INFO
```

### Comparing `portbt-0.1.1/portbt/backtest_functions.py` & `portbt-0.1.2/portbt/backtest_functions.py`

 * *Files identical despite different names*

### Comparing `portbt-0.1.1/portbt/utils.py` & `portbt-0.1.2/portbt/utils.py`

 * *Files identical despite different names*

