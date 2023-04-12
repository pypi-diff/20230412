# Comparing `tmp/wonder-sdk-0.1.0.tar.gz` & `tmp/wonder-sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-sdk-0.1.0.tar", last modified: Sun Apr  9 07:43:09 2023, max compression
+gzip compressed data, was "wonder-sdk-0.1.1.tar", last modified: Wed Apr 12 11:43:34 2023, max compression
```

## Comparing `wonder-sdk-0.1.0.tar` & `wonder-sdk-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-09 07:43:09.948892 wonder-sdk-0.1.0/
--rw-r--r--   0 basri      (501) staff       (20)      166 2023-04-09 07:43:09.948741 wonder-sdk-0.1.0/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-09 07:43:09.948939 wonder-sdk-0.1.0/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      419 2023-04-09 07:37:23.000000 wonder-sdk-0.1.0/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-09 07:43:09.947846 wonder-sdk-0.1.0/wonder_sdk/
--rw-r--r--   0 basri      (501) staff       (20)     3577 2023-04-09 07:36:48.000000 wonder-sdk-0.1.0/wonder_sdk/wonder_sdk.py
--rw-r--r--   0 basri      (501) staff       (20)      461 2023-04-09 07:36:41.000000 wonder-sdk-0.1.0/wonder_sdk/wonder_sdk_config.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-09 07:43:09.948538 wonder-sdk-0.1.0/wonder_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      166 2023-04-09 07:43:09.000000 wonder-sdk-0.1.0/wonder_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)      234 2023-04-09 07:43:09.000000 wonder-sdk-0.1.0/wonder_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-09 07:43:09.000000 wonder-sdk-0.1.0/wonder_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)      108 2023-04-09 07:43:09.000000 wonder-sdk-0.1.0/wonder_sdk.egg-info/requires.txt
--rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-09 07:43:09.000000 wonder-sdk-0.1.0/wonder_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 11:43:34.084409 wonder-sdk-0.1.1/
+-rw-r--r--   0 basri      (501) staff       (20)      146 2023-04-12 11:43:34.084280 wonder-sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 11:43:34.084457 wonder-sdk-0.1.1/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 11:41:04.000000 wonder-sdk-0.1.1/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 11:43:34.083582 wonder-sdk-0.1.1/wonder_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)      742 2023-04-12 11:37:03.000000 wonder-sdk-0.1.1/wonder_sdk/config.py
+-rw-r--r--   0 basri      (501) staff       (20)      520 2023-04-12 09:13:42.000000 wonder-sdk-0.1.1/wonder_sdk/health.py
+-rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.1/wonder_sdk/logger.py
+-rw-r--r--   0 basri      (501) staff       (20)     4231 2023-04-12 11:39:24.000000 wonder-sdk-0.1.1/wonder_sdk/wonder_sdk.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 11:43:34.084125 wonder-sdk-0.1.1/wonder_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      146 2023-04-12 11:43:34.000000 wonder-sdk-0.1.1/wonder_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)      232 2023-04-12 11:43:34.000000 wonder-sdk-0.1.1/wonder_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 11:43:34.000000 wonder-sdk-0.1.1/wonder_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 11:43:34.000000 wonder-sdk-0.1.1/wonder_sdk.egg-info/top_level.txt
```

