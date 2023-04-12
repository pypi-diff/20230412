# Comparing `tmp/dxsp-0.0.9.tar.gz` & `tmp/dxsp-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-0.0.9.tar", last modified: Sun Apr  9 13:03:24 2023, max compression
+gzip compressed data, was "dxsp-1.0.0b2.tar", last modified: Wed Apr 12 14:11:23 2023, max compression
```

## Comparing `dxsp-0.0.9.tar` & `dxsp-1.0.0b2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:03:24.916595 dxsp-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 13:03:12.000000 dxsp-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 13:03:24.916595 dxsp-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-09 13:03:12.000000 dxsp-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:03:24.916595 dxsp-0.0.9/dxsp/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 13:03:12.000000 dxsp-0.0.9/dxsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-04-09 13:03:12.000000 dxsp-0.0.9/dxsp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-09 13:03:12.000000 dxsp-0.0.9/dxsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:03:24.916595 dxsp-0.0.9/dxsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 13:03:24.000000 dxsp-0.0.9/dxsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-09 13:03:24.000000 dxsp-0.0.9/dxsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:03:24.000000 dxsp-0.0.9/dxsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 13:03:24.000000 dxsp-0.0.9/dxsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-09 13:03:12.000000 dxsp-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 13:03:24.916595 dxsp-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:11:23.622600 dxsp-1.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-12 14:11:11.000000 dxsp-1.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-12 14:11:23.622600 dxsp-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-12 14:11:11.000000 dxsp-1.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:11:23.622600 dxsp-1.0.0b2/dxsp/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 14:11:11.000000 dxsp-1.0.0b2/dxsp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:11:23.622600 dxsp-1.0.0b2/dxsp/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:11:11.000000 dxsp-1.0.0b2/dxsp/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-04-12 14:11:11.000000 dxsp-1.0.0b2/dxsp/assets/blockchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-04-12 14:11:11.000000 dxsp-1.0.0b2/dxsp/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:11:23.622600 dxsp-1.0.0b2/dxsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-12 14:11:23.000000 dxsp-1.0.0b2/dxsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-12 14:11:23.000000 dxsp-1.0.0b2/dxsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:11:23.000000 dxsp-1.0.0b2/dxsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 14:11:23.000000 dxsp-1.0.0b2/dxsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 14:11:23.000000 dxsp-1.0.0b2/dxsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 14:11:11.000000 dxsp-1.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-12 14:11:23.622600 dxsp-1.0.0b2/setup.cfg
```

### Comparing `dxsp-0.0.9/LICENSE` & `dxsp-1.0.0b2/LICENSE`

 * *Files identical despite different names*

