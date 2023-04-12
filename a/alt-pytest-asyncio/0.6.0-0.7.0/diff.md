# Comparing `tmp/alt_pytest_asyncio-0.6.0.tar.gz` & `tmp/alt_pytest_asyncio-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alt_pytest_asyncio-0.6.0.tar", last modified: Sat Oct 23 00:42:04 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `alt_pytest_asyncio-0.6.0.tar` & `alt_pytest_asyncio-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-23 00:42:04.249440 alt_pytest_asyncio-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2021-10-23 00:42:03.000000 alt_pytest_asyncio-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6751 2021-10-23 00:42:04.249440 alt_pytest_asyncio-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6335 2021-10-23 00:42:03.000000 alt_pytest_asyncio-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-23 00:42:04.249440 alt_pytest_asyncio-0.6.0/alt_pytest_asyncio/
--rw-r--r--   0 runner    (1001) docker     (121)      994 2021-10-23 00:42:03.000000 alt_pytest_asyncio-0.6.0/alt_pytest_asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6892 2021-10-23 00:42:03.000000 alt_pytest_asyncio-0.6.0/alt_pytest_asyncio/async_converters.py
--rw-r--r--   0 runner    (1001) docker     (121)     8723 2021-10-23 00:42:03.000000 alt_pytest_asyncio-0.6.0/alt_pytest_asyncio/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-10-23 00:42:03.000000 alt_pytest_asyncio-0.6.0/alt_pytest_asyncio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-23 00:42:04.249440 alt_pytest_asyncio-0.6.0/alt_pytest_asyncio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6751 2021-10-23 00:42:04.000000 alt_pytest_asyncio-0.6.0/alt_pytest_asyncio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      425 2021-10-23 00:42:04.000000 alt_pytest_asyncio-0.6.0/alt_pytest_asyncio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-23 00:42:04.000000 alt_pytest_asyncio-0.6.0/alt_pytest_asyncio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-10-23 00:42:04.000000 alt_pytest_asyncio-0.6.0/alt_pytest_asyncio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-10-23 00:42:04.000000 alt_pytest_asyncio-0.6.0/alt_pytest_asyncio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-10-23 00:42:04.000000 alt_pytest_asyncio-0.6.0/alt_pytest_asyncio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-10-23 00:42:03.000000 alt_pytest_asyncio-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-23 00:42:04.249440 alt_pytest_asyncio-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2021-10-23 00:42:03.000000 alt_pytest_asyncio-0.6.0/setup.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/__init__.py
+-rw-r--r--   0        0        0     6859 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/async_converters.py
+-rw-r--r--   0        0        0     8724 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/plugin.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/version.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/README.rst
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/PKG-INFO
```

### Comparing `alt_pytest_asyncio-0.6.0/LICENSE` & `alt_pytest_asyncio-0.7.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2019 Stephen Moore
+Copyright (c) 2023 Stephen Moore
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `alt_pytest_asyncio-0.6.0/PKG-INFO` & `alt_pytest_asyncio-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
-Name: alt_pytest_asyncio
-Version: 0.6.0
+Name: alt-pytest-asyncio
+Version: 0.7.0
 Summary: Alternative pytest plugin to pytest-asyncio
-Home-page: https://github.com/delfick/alt-pytest-asyncio
-Author: Stephen Moore
-Author-email: delfick755@gmail.com
-License: MIT
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/delfick/alt-pytest-asyncio
+Author-email: Stephen Moore <delfick755@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Framework :: Pytest
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >= 3.7
+Requires-Python: >=3.7
+Requires-Dist: pytest>=7.0.0
 Provides-Extra: tests
-License-File: LICENSE
+Requires-Dist: nest-asyncio==1.0.0; extra == 'tests'
+Requires-Dist: noseofyeti[black]==2.4.1; extra == 'tests'
+Requires-Dist: pytest==7.3.0; extra == 'tests'
+Description-Content-Type: text/x-rst
 
 Alternative Pytest Asyncio
 ==========================
 
 This plugin allows you to have async pytest fixtures and tests.
 
 This plugin only supports python 3.6 and above.
@@ -32,14 +35,20 @@
 
 Like pytest-asyncio it supports async tests, coroutine fixtures and async
 generator fixtures.
 
 Changelog
 ---------
 
+0.7.0 - 12 April 2023
+    * Changed the pytest dependency to be greater than pytest version 7
+    * Using isort now
+    * Went from setuptools to hatch
+    * CI now runs against python 3.11
+
 0.6.0 - 23 October 2021
     * Fix bug where it was possible for an async generator fixture to
       be cleaned up even if it was never started.
     * This library is now 3.7+ only
     * Added an equivalent ``shutdown_asyncgen`` to the OverrideLoop helper
 
 0.5.4 - 26 January 2021
@@ -200,9 +209,7 @@
 The ``run_until_complete`` on the ``custom_loop`` in the above example will
 do a ``run_until_complete`` on the new loop, but in a way that means you
 won't get ``unhandled exception during shutdown`` errors when the context
 manager closes the new loop.
 
 When the context manager exits and closes the new loop, it will first cancel
 all tasks to ensure finally blocks are run.
-
-
```

### Comparing `alt_pytest_asyncio-0.6.0/README.rst` & `alt_pytest_asyncio-0.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 
 Like pytest-asyncio it supports async tests, coroutine fixtures and async
 generator fixtures.
 
 Changelog
 ---------
 
+0.7.0 - 12 April 2023
+    * Changed the pytest dependency to be greater than pytest version 7
+    * Using isort now
+    * Went from setuptools to hatch
+    * CI now runs against python 3.11
+
 0.6.0 - 23 October 2021
     * Fix bug where it was possible for an async generator fixture to
       be cleaned up even if it was never started.
     * This library is now 3.7+ only
     * Added an equivalent ``shutdown_asyncgen`` to the OverrideLoop helper
 
 0.5.4 - 26 January 2021
```

### Comparing `alt_pytest_asyncio-0.6.0/alt_pytest_asyncio/__init__.py` & `alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/__init__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """pytest-cov: avoid already-imported warning: PYTEST_DONT_REWRITE."""
-from alt_pytest_asyncio.version import VERSION
-
 import pytest
 
+from alt_pytest_asyncio.version import VERSION
+
 
 @pytest.hookimpl
 def pytest_addoption(parser):
     """Add an option for default async timeouts"""
     desc = "timeout in seconds before failing a test. This can be overriden with @pytest.mark.async_timeout(<my_timeout>)"
 
     group = parser.getgroup(
```

### Comparing `alt_pytest_asyncio-0.6.0/alt_pytest_asyncio/async_converters.py` & `alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/async_converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 convert_fixtures and converted_async_test are used by the Plugin
 to convert async fixtures and async tests.
 
 We try our best to make sure error reporting is short and useful by doing some
 hacks with capturing errors inside run_until_complete rather than outside so
 that you don't get asyncio internals in the errors.
 """
-from functools import wraps
 import asyncio
 import inspect
 import sys
+from functools import wraps
 
 
 def convert_fixtures(fixturedef, request, node):
     """Used to replace async fixtures"""
     if not hasattr(fixturedef, "func"):
         return
 
@@ -69,15 +69,14 @@
 
     fle = inspect.getfile(func)
     if hasattr(func, "__func__"):
         func = func.__func__
     lineno = func.__code__.co_firstlineno
 
     def raise_error():
-        __tracebackhide__ = True
         if info["cancelled"]:
             assert False, f"Took too long to complete: {fle}:{lineno}"
         raise info["e"]
 
     if info.get("e"):
         # Use a separate function so when --tb=short is not set we don't get
         # this entire function in the output
```

### Comparing `alt_pytest_asyncio-0.6.0/alt_pytest_asyncio/plugin.py` & `alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from alt_pytest_asyncio.async_converters import convert_fixtures, converted_async_test
-
-from _pytest._code.code import ExceptionInfo
-from functools import partial, wraps
-from collections import defaultdict
-import inspect
 import asyncio
-import pytest
+import inspect
 import sys
+from collections import defaultdict
+from functools import partial, wraps
+
+import pytest
+from _pytest._code.code import ExceptionInfo
+
+from alt_pytest_asyncio.async_converters import convert_fixtures, converted_async_test
 
 
 class AltPytestAsyncioPlugin:
     def __init__(self, loop=None):
         self.own_loop = False
         self.test_tasks = defaultdict(list)
```

