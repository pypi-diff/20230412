# Comparing `tmp/wonder-sdk-0.1.1.tar.gz` & `tmp/wonder-sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-sdk-0.1.1.tar", last modified: Wed Apr 12 11:43:34 2023, max compression
+gzip compressed data, was "wonder-sdk-0.1.2.tar", last modified: Wed Apr 12 11:55:34 2023, max compression
```

## Comparing `wonder-sdk-0.1.1.tar` & `wonder-sdk-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 11:43:34.084409 wonder-sdk-0.1.1/
--rw-r--r--   0 basri      (501) staff       (20)      146 2023-04-12 11:43:34.084280 wonder-sdk-0.1.1/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 11:43:34.084457 wonder-sdk-0.1.1/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 11:41:04.000000 wonder-sdk-0.1.1/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 11:43:34.083582 wonder-sdk-0.1.1/wonder_sdk/
--rw-r--r--   0 basri      (501) staff       (20)      742 2023-04-12 11:37:03.000000 wonder-sdk-0.1.1/wonder_sdk/config.py
--rw-r--r--   0 basri      (501) staff       (20)      520 2023-04-12 09:13:42.000000 wonder-sdk-0.1.1/wonder_sdk/health.py
--rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.1/wonder_sdk/logger.py
--rw-r--r--   0 basri      (501) staff       (20)     4231 2023-04-12 11:39:24.000000 wonder-sdk-0.1.1/wonder_sdk/wonder_sdk.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 11:43:34.084125 wonder-sdk-0.1.1/wonder_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      146 2023-04-12 11:43:34.000000 wonder-sdk-0.1.1/wonder_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)      232 2023-04-12 11:43:34.000000 wonder-sdk-0.1.1/wonder_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 11:43:34.000000 wonder-sdk-0.1.1/wonder_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 11:43:34.000000 wonder-sdk-0.1.1/wonder_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 11:55:34.195343 wonder-sdk-0.1.2/
+-rw-r--r--   0 basri      (501) staff       (20)     1080 2023-04-12 11:52:01.000000 wonder-sdk-0.1.2/LICENCE
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 11:55:34.195223 wonder-sdk-0.1.2/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 11:55:34.195385 wonder-sdk-0.1.2/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 11:55:31.000000 wonder-sdk-0.1.2/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 11:55:34.194528 wonder-sdk-0.1.2/wonder_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)     4231 2023-04-12 11:55:01.000000 wonder-sdk-0.1.2/wonder_sdk/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      742 2023-04-12 11:37:03.000000 wonder-sdk-0.1.2/wonder_sdk/config.py
+-rw-r--r--   0 basri      (501) staff       (20)      520 2023-04-12 09:13:42.000000 wonder-sdk-0.1.2/wonder_sdk/health.py
+-rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.2/wonder_sdk/logger.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 11:55:34.195074 wonder-sdk-0.1.2/wonder_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 11:55:34.000000 wonder-sdk-0.1.2/wonder_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)      238 2023-04-12 11:55:34.000000 wonder-sdk-0.1.2/wonder_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 11:55:34.000000 wonder-sdk-0.1.2/wonder_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 11:55:34.000000 wonder-sdk-0.1.2/wonder_sdk.egg-info/top_level.txt
```

### Comparing `wonder-sdk-0.1.1/wonder_sdk/config.py` & `wonder-sdk-0.1.2/wonder_sdk/config.py`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.1/wonder_sdk/health.py` & `wonder-sdk-0.1.2/wonder_sdk/health.py`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.1/wonder_sdk/logger.py` & `wonder-sdk-0.1.2/wonder_sdk/logger.py`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.1/wonder_sdk/wonder_sdk.py` & `wonder-sdk-0.1.2/wonder_sdk/__init__.py`

 * *Files identical despite different names*

