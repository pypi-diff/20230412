# Comparing `tmp/compilecls-1.0.0.tar.gz` & `tmp/compilecls-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compilecls-1.0.0.tar", last modified: Mon Apr 10 16:08:58 2023, max compression
+gzip compressed data, was "compilecls-1.0.2.tar", last modified: Wed Apr 12 13:23:32 2023, max compression
```

## Comparing `compilecls-1.0.0.tar` & `compilecls-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 16:08:58.077661 compilecls-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      325 2023-04-10 16:08:58.077661 compilecls-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 16:08:58.077661 compilecls-1.0.0/compilecls/
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-10 16:08:57.000000 compilecls-1.0.0/compilecls/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 16:08:58.077661 compilecls-1.0.0/compilecls.egg-info/
--rw-r--r--   0 root         (0) root         (0)      325 2023-04-10 16:08:58.000000 compilecls-1.0.0/compilecls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-10 16:08:58.000000 compilecls-1.0.0/compilecls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 16:08:58.000000 compilecls-1.0.0/compilecls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-10 16:08:58.000000 compilecls-1.0.0/compilecls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 16:08:58.077661 compilecls-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      538 2023-04-10 16:08:57.000000 compilecls-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 13:23:32.362784 compilecls-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      321 2023-04-12 13:23:32.362784 compilecls-1.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 13:23:32.362784 compilecls-1.0.2/compilecls/
+-rw-r--r--   0 root         (0) root         (0)    81719 2023-04-12 13:23:31.000000 compilecls-1.0.2/compilecls/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 13:23:32.362784 compilecls-1.0.2/compilecls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      321 2023-04-12 13:23:32.000000 compilecls-1.0.2/compilecls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-12 13:23:32.000000 compilecls-1.0.2/compilecls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 13:23:32.000000 compilecls-1.0.2/compilecls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-12 13:23:32.000000 compilecls-1.0.2/compilecls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 13:23:32.362784 compilecls-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      534 2023-04-12 13:23:31.000000 compilecls-1.0.2/setup.py
```

