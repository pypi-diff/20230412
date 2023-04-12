# Comparing `tmp/naruno_remote_app-0.56.1.tar.gz` & `tmp/naruno_remote_app-0.56.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_remote_app-0.56.1.tar", last modified: Tue Apr 11 06:16:18 2023, max compression
+gzip compressed data, was "naruno_remote_app-0.56.2.tar", last modified: Wed Apr 12 15:52:47 2023, max compression
```

## Comparing `naruno_remote_app-0.56.1.tar` & `naruno_remote_app-0.56.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:18.855778 naruno_remote_app-0.56.1/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-11 06:16:18.855778 naruno_remote_app-0.56.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:18.855778 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-11 06:16:18.000000 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-11 06:16:18.000000 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:16:18.000000 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:16:18.000000 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 06:16:18.000000 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:16:18.000000 naruno_remote_app-0.56.1/naruno_remote_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:16:18.855778 naruno_remote_app-0.56.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-11 06:16:02.000000 naruno_remote_app-0.56.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:52:47.424366 naruno_remote_app-0.56.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-12 15:52:47.420365 naruno_remote_app-0.56.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:52:47.420365 naruno_remote_app-0.56.2/naruno_remote_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-12 15:52:47.000000 naruno_remote_app-0.56.2/naruno_remote_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-12 15:52:47.000000 naruno_remote_app-0.56.2/naruno_remote_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:52:47.000000 naruno_remote_app-0.56.2/naruno_remote_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:52:47.000000 naruno_remote_app-0.56.2/naruno_remote_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 15:52:47.000000 naruno_remote_app-0.56.2/naruno_remote_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:52:47.000000 naruno_remote_app-0.56.2/naruno_remote_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:52:47.424366 naruno_remote_app-0.56.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-12 15:52:24.000000 naruno_remote_app-0.56.2/setup.py
```

### Comparing `naruno_remote_app-0.56.1/setup.py` & `naruno_remote_app-0.56.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from setuptools import setup
 
 setup(
     name="naruno_remote_app",
-    version="0.56.1",
+    version="0.56.2",
     description="""This is a tool for apps on Naruno""",
     url="https://docs.naruno.org/",
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     license="MPL-2.0",
     install_requires="""
 requests==2.28.2
-naruno_api==0.56.1
+naruno_api==0.56.2
 """,
     python_requires=">=3.8",
     zip_safe=False,
 )
```

