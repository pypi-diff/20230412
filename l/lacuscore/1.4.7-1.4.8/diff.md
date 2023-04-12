# Comparing `tmp/lacuscore-1.4.7.tar.gz` & `tmp/lacuscore-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.4.7.tar", max compression
+gzip compressed data, was "lacuscore-1.4.8.tar", max compression
```

## Comparing `lacuscore-1.4.7.tar` & `lacuscore-1.4.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.4.7/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.4.7/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.4.7/lacuscore/__init__.py
--rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.4.7/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    28070 2023-04-11 13:29:09.084489 lacuscore-1.4.7/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.4.7/lacuscore/py.typed
--rw-r--r--   0        0        0     1516 2023-04-11 17:06:31.918554 lacuscore-1.4.7/pyproject.toml
--rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 lacuscore-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.4.8/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.4.8/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.4.8/lacuscore/__init__.py
+-rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.4.8/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    28070 2023-04-11 13:29:09.084489 lacuscore-1.4.8/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.4.8/lacuscore/py.typed
+-rw-r--r--   0        0        0     1516 2023-04-12 11:36:31.465532 lacuscore-1.4.8/pyproject.toml
+-rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 lacuscore-1.4.8/PKG-INFO
```

### Comparing `lacuscore-1.4.7/LICENSE` & `lacuscore-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.7/README.md` & `lacuscore-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.7/lacuscore/lacus_monitoring.py` & `lacuscore-1.4.8/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.7/lacuscore/lacuscore.py` & `lacuscore-1.4.8/lacuscore/lacuscore.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.7/pyproject.toml` & `lacuscore-1.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.4.7"
+version = "1.4.8"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -28,15 +28,15 @@
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.2"
 Sphinx = { version = "^6.1.3", optional = true }
-playwrightcapture = {extras = ["recaptcha"], version = "^1.19.8"}
+playwrightcapture = {extras = ["recaptcha"], version = "^1.19.9"}
 defang = "^0.5.3"
 ua-parser = "^0.16.1"
 redis = {version = "^4.5.4", extras = ["hiredis"]}
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
```

### Comparing `lacuscore-1.4.7/PKG-INFO` & `lacuscore-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.4.7
+Version: 1.4.8
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
 Requires-Dist: defang (>=0.5.3,<0.6.0)
-Requires-Dist: playwrightcapture[recaptcha] (>=1.19.8,<2.0.0)
+Requires-Dist: playwrightcapture[recaptcha] (>=1.19.9,<2.0.0)
 Requires-Dist: redis[hiredis] (>=4.5.4,<5.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: ua-parser (>=0.16.1,<0.17.0)
 Project-URL: Documentation, https://lacuscore.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ail-project/LacusCore
 Description-Content-Type: text/markdown
```

