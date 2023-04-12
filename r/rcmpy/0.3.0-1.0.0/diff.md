# Comparing `tmp/rcmpy-0.3.0.tar.gz` & `tmp/rcmpy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmpy-0.3.0.tar", last modified: Mon Apr 10 05:45:40 2023, max compression
+gzip compressed data, was "rcmpy-1.0.0.tar", last modified: Wed Apr 12 06:23:36 2023, max compression
```

## Comparing `rcmpy-0.3.0.tar` & `rcmpy-1.0.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 05:44:36.000000 rcmpy-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-10 05:45:40.713079 rcmpy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-10 05:44:36.000000 rcmpy-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-10 05:44:36.000000 rcmpy-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.709079 rcmpy-0.3.0/rcmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/commands/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.709079 rcmpy-0.3.0/rcmpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/data/schemas/ManagedFile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/data/schemas/State.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/environment/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/rcmpy/xdg/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-10 05:44:36.000000 rcmpy-0.3.0/rcmpy/xdg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.709079 rcmpy-0.3.0/rcmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-10 05:45:40.000000 rcmpy-0.3.0/rcmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-10 05:45:40.000000 rcmpy-0.3.0/rcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 05:45:40.000000 rcmpy-0.3.0/rcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 05:45:40.000000 rcmpy-0.3.0/rcmpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-10 05:45:40.000000 rcmpy-0.3.0/rcmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 05:45:40.000000 rcmpy-0.3.0/rcmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 05:45:40.713079 rcmpy-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-10 05:44:36.000000 rcmpy-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 05:45:40.713079 rcmpy-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-10 05:44:36.000000 rcmpy-0.3.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-10 05:44:36.000000 rcmpy-0.3.0/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-10 05:44:36.000000 rcmpy-0.3.0/tests/test_xdg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 06:22:17.000000 rcmpy-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-12 06:23:36.110685 rcmpy-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-12 06:22:17.000000 rcmpy-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-12 06:22:17.000000 rcmpy-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.106685 rcmpy-1.0.0/rcmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/commands/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.106685 rcmpy-1.0.0/rcmpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/data/schemas/ManagedFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/data/schemas/State.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/environment/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy/xdg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-12 06:22:17.000000 rcmpy-1.0.0/rcmpy/xdg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/rcmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-12 06:23:36.000000 rcmpy-1.0.0/rcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-12 06:23:36.000000 rcmpy-1.0.0/rcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 06:23:36.000000 rcmpy-1.0.0/rcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 06:23:36.000000 rcmpy-1.0.0/rcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-12 06:23:36.000000 rcmpy-1.0.0/rcmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 06:23:36.000000 rcmpy-1.0.0/rcmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 06:23:36.114685 rcmpy-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-12 06:22:17.000000 rcmpy-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:36.110685 rcmpy-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-12 06:22:17.000000 rcmpy-1.0.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 06:22:17.000000 rcmpy-1.0.0/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 06:22:17.000000 rcmpy-1.0.0/tests/test_xdg.py
```

### Comparing `rcmpy-0.3.0/LICENSE` & `rcmpy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmpy-0.3.0/PKG-INFO` & `rcmpy-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 0.3.0
+Version: 1.0.0
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=96aa8923f1d36b7eddcfda3f7e4d8171
+    hash=4e253e82b70bf6a2a6479e0620da720b
     =====================================
 -->
 
-# rcmpy ([0.3.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.0.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-0.3.0/README.md` & `rcmpy-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=96aa8923f1d36b7eddcfda3f7e4d8171
+    hash=4e253e82b70bf6a2a6479e0620da720b
     =====================================
 -->
 
-# rcmpy ([0.3.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.0.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-0.3.0/pyproject.toml` & `rcmpy-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "rcmpy"
-version = "0.3.0"
+version = "1.0.0"
 description = "A configuration-file management system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `rcmpy-0.3.0/rcmpy/app.py` & `rcmpy-1.0.0/rcmpy/app.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.3.0/rcmpy/commands/all.py` & `rcmpy-1.0.0/rcmpy/commands/all.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.3.0/rcmpy/commands/apply.py` & `rcmpy-1.0.0/rcmpy/commands/apply.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from argparse import ArgumentParser as _ArgumentParser
 from argparse import Namespace as _Namespace
 from logging import getLogger
 
 # third-party
 from vcorelib.args import CommandFunction as _CommandFunction
 from vcorelib.logging import log_time
+from vcorelib.paths import rel
 
 # internal
 from rcmpy.environment import Environment, load_environment
 
 
 def apply_env(env: Environment) -> int:
     """Apply pending changes from the environment."""
@@ -23,22 +24,32 @@
     for file in env.config.files:
         # Check if a template is found for this file.
         if file.template not in env.templates_by_name:
             result += 1
             env.logger.error("Template '%s' not found!", file.template)
             continue
 
+        is_new = env.state.is_new()
+
         # Check if this file has any updated templates.
-        if env.is_updated(file):
+        if is_new or env.is_updated(file):
             template = env.templates_by_name[file.template]
 
-            # If a template doesn't require rendering, link or
-            # copy it.
-            if template.template is None:
-                file.update(template.path, env.logger)
+            # If a template doesn't require rendering, use it as-is.
+            source = template.path
+
+            if template.template is not None:
+                # Render the template to the build directory.
+                source = env.build.joinpath(file.template)
+                with source.open("w") as path_fd:
+                    path_fd.write(template.template.render(env.state.configs))
+                    env.logger.info("Rendered '%s'.", rel(source))
+
+                # Update the output file.
+            file.update(source, env.logger)
 
     return result
 
 
 def apply_cmd(_: _Namespace) -> int:
     """Execute the apply command."""
```

### Comparing `rcmpy-0.3.0/rcmpy/commands/use.py` & `rcmpy-1.0.0/rcmpy/commands/use.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.3.0/rcmpy/commands/variant.py` & `rcmpy-1.0.0/rcmpy/commands/variant.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.3.0/rcmpy/commands/watch.py` & `rcmpy-1.0.0/rcmpy/commands/watch.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.3.0/rcmpy/config/__init__.py` & `rcmpy-1.0.0/rcmpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.3.0/rcmpy/entry.py` & `rcmpy-1.0.0/rcmpy/entry.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.3.0/rcmpy/environment/__init__.py` & `rcmpy-1.0.0/rcmpy/environment/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,10 +21,14 @@
 @contextmanager
 def load_environment(
     root: Pathlike = None, name: str = "state.json"
 ) -> Iterator[Environment]:
     """A wrapper for loading an environment with default state data."""
 
     with ExitStack() as stack:
-        yield Environment(
+        env = Environment(
             stack.enter_context(load_state(root=root, name=name)), stack
         )
+        yield env
+
+        # Ensure that the previous variant gets set.
+        env.state.previous["variant"] = env.state.variant
```

### Comparing `rcmpy-0.3.0/rcmpy/environment/base.py` & `rcmpy-1.0.0/rcmpy/environment/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
         super().__init__()
         self.state = state
         self.stack = stack
         self._config: Optional[Config] = None
         self._cache = default_cache_directory()
 
-        self._build = state.directory.joinpath("build")
-        self._build.mkdir(exist_ok=True)
+        self.build = state.directory.joinpath("build")
+        self.build.mkdir(exist_ok=True)
 
         config_base = state.directory.joinpath(PKG_NAME)
 
         config_candidates = list(
             FileExtension.data_candidates(config_base, exists_only=True)
         )
```

### Comparing `rcmpy-0.3.0/rcmpy/environment/template.py` & `rcmpy-1.0.0/rcmpy/environment/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,25 +88,15 @@
 
     def _init_templates(self, template_names: Set[str]) -> bool:
         """
         Initialize the template environment based on a set of template names
         that may be relevant to some task.
         """
 
-        template_root = self.state.directory.joinpath("templates")
-
-        candidates = [template_root.joinpath("common")]
-
-        # Only consider a 'variant' sub-directory if variant is set. Ensure
-        # that the candidate directory comes first.
-        if self.state.variant:
-            candidates.insert(0, template_root.joinpath(self.state.variant))
-
-        # Only consider directories that exist.
-        candidates = [x for x in candidates if x.is_dir()]
+        candidates = self.state.root_directories("templates")
 
         # Prefer variant templates, if the variant template-directory
         # exists.
         self.jinja = environment(
             loader=FileSystemLoader(candidates, followlinks=True)
         )
```

### Comparing `rcmpy-0.3.0/rcmpy/paths/__init__.py` & `rcmpy-1.0.0/rcmpy/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.3.0/rcmpy/schemas.py` & `rcmpy-1.0.0/rcmpy/schemas.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.3.0/rcmpy/xdg/__init__.py` & `rcmpy-1.0.0/rcmpy/xdg/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.3.0/rcmpy.egg-info/PKG-INFO` & `rcmpy-1.0.0/rcmpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 0.3.0
+Version: 1.0.0
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=96aa8923f1d36b7eddcfda3f7e4d8171
+    hash=4e253e82b70bf6a2a6479e0620da720b
     =====================================
 -->
 
-# rcmpy ([0.3.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.0.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-0.3.0/rcmpy.egg-info/SOURCES.txt` & `rcmpy-1.0.0/rcmpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcmpy-0.3.0/setup.py` & `rcmpy-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `rcmpy-0.3.0/tests/test_entry.py` & `rcmpy-1.0.0/tests/test_entry.py`

 * *Files identical despite different names*

