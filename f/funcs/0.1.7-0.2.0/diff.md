# Comparing `tmp/funcs-0.1.7.tar.gz` & `tmp/funcs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs-0.1.7.tar", last modified: Sat Sep 10 15:29:05 2022, max compression
+gzip compressed data, was "funcs-0.2.0.tar", max compression
```

## Comparing `funcs-0.1.7.tar` & `funcs-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 15:29:05.814306 funcs-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-09-10 15:28:55.000000 funcs-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-10 15:28:55.000000 funcs-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-09-10 15:29:05.814306 funcs-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-10 15:28:55.000000 funcs-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 15:29:05.810305 funcs-0.1.7/funcs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-10 15:28:55.000000 funcs-0.1.7/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-10 15:28:55.000000 funcs-0.1.7/funcs/image.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-10 15:28:55.000000 funcs-0.1.7/funcs/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3383 2022-09-10 15:28:55.000000 funcs-0.1.7/funcs/video.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-09-10 15:28:55.000000 funcs-0.1.7/funcs/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 15:29:05.814306 funcs-0.1.7/funcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-09-10 15:29:05.000000 funcs-0.1.7/funcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-09-10 15:29:05.000000 funcs-0.1.7/funcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-10 15:29:05.000000 funcs-0.1.7/funcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-10 15:29:05.000000 funcs-0.1.7/funcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-10 15:29:05.000000 funcs-0.1.7/funcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-10 15:28:55.000000 funcs-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-10 15:29:05.814306 funcs-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-09-10 15:28:55.000000 funcs-0.1.7/setup.py
+-rw-r--r--   0        0        0     1092 2023-04-12 12:11:49.139292 funcs-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2872 2023-04-12 12:11:49.139292 funcs-0.2.0/README.md
+-rw-r--r--   0        0        0     1435 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/__init__.py
+-rw-r--r--   0        0        0      883 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/application.py
+-rw-r--r--   0        0        0      563 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/callers.py
+-rw-r--r--   0        0        0     4121 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/composition.py
+-rw-r--r--   0        0        0      300 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/debug.py
+-rw-r--r--   0        0        0      166 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/decorators.py
+-rw-r--r--   0        0        0     3595 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/flow.py
+-rw-r--r--   0        0        0      899 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/functions.py
+-rw-r--r--   0        0        0      418 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/getters.py
+-rw-r--r--   0        0        0      264 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/primitives.py
+-rw-r--r--   0        0        0        0 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/py.typed
+-rw-r--r--   0        0        0      492 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/reduction.py
+-rw-r--r--   0        0        0      475 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/types.py
+-rw-r--r--   0        0        0     2627 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/typing.py
+-rw-r--r--   0        0        0     1369 2023-04-12 12:11:49.143292 funcs-0.2.0/funcs/unpacking.py
+-rw-r--r--   0        0        0     3022 2023-04-12 12:11:49.143292 funcs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 funcs-0.2.0/PKG-INFO
```

### Comparing `funcs-0.1.7/LICENSE` & `funcs-0.2.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Ayoub Assis
+Copyright (c) 2023-present, Nikita Tikhonov (nekitdev)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

