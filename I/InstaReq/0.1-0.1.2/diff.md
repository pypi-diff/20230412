# Comparing `tmp/InstaReq-0.1.tar.gz` & `tmp/InstaReq-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InstaReq-0.1.tar", last modified: Wed Apr 12 17:39:50 2023, max compression
+gzip compressed data, was "InstaReq-0.1.2.tar", last modified: Wed Apr 12 18:04:26 2023, max compression
```

## Comparing `InstaReq-0.1.tar` & `InstaReq-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 17:39:50.535560 InstaReq-0.1/
-drwxrwxrwx   0        0        0        0 2023-04-12 17:39:50.531559 InstaReq-0.1/InstaReq/
--rw-rw-rw-   0        0        0       26 2023-04-12 17:38:39.000000 InstaReq-0.1/InstaReq/__init__.py
--rw-rw-rw-   0        0        0       70 2023-04-12 17:38:44.000000 InstaReq-0.1/InstaReq/__main__.py
--rw-rw-rw-   0        0        0     2931 2023-04-12 17:39:09.000000 InstaReq-0.1/InstaReq/instareq.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:39:50.535560 InstaReq-0.1/InstaReq.egg-info/
--rw-rw-rw-   0        0        0       53 2023-04-12 17:39:50.000000 InstaReq-0.1/InstaReq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-12 17:39:50.000000 InstaReq-0.1/InstaReq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 17:39:50.000000 InstaReq-0.1/InstaReq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-12 17:39:50.000000 InstaReq-0.1/InstaReq.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 17:39:50.000000 InstaReq-0.1/InstaReq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 17:39:50.000000 InstaReq-0.1/InstaReq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       53 2023-04-12 17:39:50.535560 InstaReq-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-04-12 17:38:12.000000 InstaReq-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 17:39:50.536560 InstaReq-0.1/setup.cfg
--rw-rw-rw-   0        0        0      293 2023-04-12 17:38:30.000000 InstaReq-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:04:26.112685 InstaReq-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-04-12 18:04:26.108685 InstaReq-0.1.2/InstaReq/
+-rw-rw-rw-   0        0        0       26 2023-04-12 17:38:39.000000 InstaReq-0.1.2/InstaReq/__init__.py
+-rw-rw-rw-   0        0        0       70 2023-04-12 17:38:44.000000 InstaReq-0.1.2/InstaReq/__main__.py
+-rw-rw-rw-   0        0        0     2931 2023-04-12 17:39:09.000000 InstaReq-0.1.2/InstaReq/instareq.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:04:26.111685 InstaReq-0.1.2/InstaReq.egg-info/
+-rw-rw-rw-   0        0        0     1469 2023-04-12 18:04:26.000000 InstaReq-0.1.2/InstaReq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-04-12 18:04:26.000000 InstaReq-0.1.2/InstaReq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 18:04:26.000000 InstaReq-0.1.2/InstaReq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-12 18:04:26.000000 InstaReq-0.1.2/InstaReq.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 18:04:26.000000 InstaReq-0.1.2/InstaReq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 18:04:26.000000 InstaReq-0.1.2/InstaReq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2023-04-12 17:53:47.000000 InstaReq-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1469 2023-04-12 18:04:26.112685 InstaReq-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2023-04-12 17:47:06.000000 InstaReq-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 18:04:26.112685 InstaReq-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2023-04-12 18:03:12.000000 InstaReq-0.1.2/setup.py
```

### Comparing `InstaReq-0.1/InstaReq/instareq.py` & `InstaReq-0.1.2/InstaReq/instareq.py`

 * *Files identical despite different names*

