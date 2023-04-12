# Comparing `tmp/piplibcrypto-1.0.0.tar.gz` & `tmp/piplibcrypto-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piplibcrypto-1.0.0.tar", last modified: Tue Apr 11 17:09:59 2023, max compression
+gzip compressed data, was "piplibcrypto-1.2.0.tar", last modified: Wed Apr 12 00:30:59 2023, max compression
```

## Comparing `piplibcrypto-1.0.0.tar` & `piplibcrypto-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:09:59.510755 piplibcrypto-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      320 2023-04-11 17:09:59.510755 piplibcrypto-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:09:59.506755 piplibcrypto-1.0.0/piplibcrypto/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 17:09:59.000000 piplibcrypto-1.0.0/piplibcrypto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:09:59.510755 piplibcrypto-1.0.0/piplibcrypto.egg-info/
--rw-r--r--   0 root         (0) root         (0)      320 2023-04-11 17:09:59.000000 piplibcrypto-1.0.0/piplibcrypto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      177 2023-04-11 17:09:59.000000 piplibcrypto-1.0.0/piplibcrypto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 17:09:59.000000 piplibcrypto-1.0.0/piplibcrypto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 17:09:59.000000 piplibcrypto-1.0.0/piplibcrypto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 17:09:59.510755 piplibcrypto-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      533 2023-04-11 17:09:58.000000 piplibcrypto-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:30:59.936063 piplibcrypto-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      378 2023-04-12 00:30:59.936063 piplibcrypto-1.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:30:59.932063 piplibcrypto-1.2.0/piplibcrypto/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-12 00:30:59.000000 piplibcrypto-1.2.0/piplibcrypto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:30:59.936063 piplibcrypto-1.2.0/piplibcrypto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      378 2023-04-12 00:30:59.000000 piplibcrypto-1.2.0/piplibcrypto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      177 2023-04-12 00:30:59.000000 piplibcrypto-1.2.0/piplibcrypto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:30:59.000000 piplibcrypto-1.2.0/piplibcrypto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-12 00:30:59.000000 piplibcrypto-1.2.0/piplibcrypto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 00:30:59.936063 piplibcrypto-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      591 2023-04-12 00:30:58.000000 piplibcrypto-1.2.0/setup.py
```

