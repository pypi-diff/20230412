# Comparing `tmp/stdlibby_py-0.5.7.tar.gz` & `tmp/stdlibby_py-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdlibby_py-0.5.7.tar", max compression
+gzip compressed data, was "stdlibby_py-0.5.8.tar", max compression
```

## Comparing `stdlibby_py-0.5.7.tar` & `stdlibby_py-0.5.8.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0        0 2023-04-02 19:48:10.235584 stdlibby_py-0.5.7/README.md
--rw-r--r--   0        0        0      323 2023-04-05 22:43:51.365882 stdlibby_py-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      127 2023-04-05 22:43:23.462609 stdlibby_py-0.5.7/stdlibby_py/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 20:12:06.312094 stdlibby_py-0.5.7/stdlibby_py/api.py
--rw-r--r--   0        0        0       13 2023-04-04 18:46:42.219852 stdlibby_py-0.5.7/stdlibby_py/cly.py
--rw-r--r--   0        0        0     1096 2023-04-02 20:11:15.833248 stdlibby_py-0.5.7/stdlibby_py/datetime.py
--rw-r--r--   0        0        0       53 2023-04-04 18:25:30.091683 stdlibby_py-0.5.7/stdlibby_py/main.py
--rw-r--r--   0        0        0     1070 2023-04-05 22:45:36.702915 stdlibby_py-0.5.7/stdlibby_py/ndjson.py
--rw-r--r--   0        0        0     1748 2023-04-02 20:45:47.244740 stdlibby_py-0.5.7/stdlibby_py/sqlite.py
--rw-r--r--   0        0        0      528 2023-04-05 21:12:37.009143 stdlibby_py-0.5.7/stdlibby_py/utils.py
--rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 stdlibby_py-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0      528 2023-04-06 19:06:52.675586 stdlibby_py-0.5.8/README.md
+-rw-r--r--   0        0        0      364 2023-04-12 00:47:41.108207 stdlibby_py-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      127 2023-04-05 22:43:23.462609 stdlibby_py-0.5.8/stdlibby_py/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 20:12:06.312094 stdlibby_py-0.5.8/stdlibby_py/api.py
+-rw-r--r--   0        0        0       13 2023-04-04 18:46:42.219852 stdlibby_py-0.5.8/stdlibby_py/cly.py
+-rw-r--r--   0        0        0     1769 2023-04-08 00:13:21.039591 stdlibby_py-0.5.8/stdlibby_py/date_time.py
+-rw-r--r--   0        0        0      456 2023-04-06 02:15:53.707113 stdlibby_py-0.5.8/stdlibby_py/errors.py
+-rw-r--r--   0        0        0       53 2023-04-04 18:25:30.091683 stdlibby_py-0.5.8/stdlibby_py/main.py
+-rw-r--r--   0        0        0     1070 2023-04-05 22:45:36.702915 stdlibby_py-0.5.8/stdlibby_py/ndjson.py
+-rw-r--r--   0        0        0     3072 2023-04-11 07:40:52.998482 stdlibby_py-0.5.8/stdlibby_py/sqlite.py
+-rw-r--r--   0        0        0     2067 2023-04-12 00:47:28.388952 stdlibby_py-0.5.8/stdlibby_py/utils.py
+-rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 stdlibby_py-0.5.8/PKG-INFO
```

### Comparing `stdlibby_py-0.5.7/stdlibby_py/ndjson.py` & `stdlibby_py-0.5.8/stdlibby_py/ndjson.py`

 * *Files identical despite different names*

