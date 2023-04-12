# Comparing `tmp/inmanta-ui-4.0.1.tar.gz` & `tmp/inmanta-ui-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmanta-ui-4.0.1.tar", last modified: Mon Feb  6 15:20:44 2023, max compression
+gzip compressed data, was "inmanta-ui-4.0.2.tar", last modified: Wed Apr 12 07:26:08 2023, max compression
```

## Comparing `inmanta-ui-4.0.1.tar` & `inmanta-ui-4.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-06 15:20:44.599880 inmanta-ui-4.0.1/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10173 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/LICENSE
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      264 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/MANIFEST.in
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      321 2023-02-06 15:20:44.599880 inmanta-ui-4.0.1/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       58 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/README.md
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      384 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/pyproject.toml
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      558 2023-02-06 15:20:44.599880 inmanta-ui-4.0.1/setup.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      789 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/setup.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-06 15:20:44.596879 inmanta-ui-4.0.1/src/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-06 15:20:44.596879 inmanta-ui-4.0.1/src/inmanta_ext/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-06 15:20:44.597880 inmanta-ui-4.0.1/src/inmanta_ext/ui/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/src/inmanta_ext/ui/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      815 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/src/inmanta_ext/ui/extension.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-06 15:20:44.598879 inmanta-ui-4.0.1/src/inmanta_ui/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/src/inmanta_ui/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1765 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/src/inmanta_ui/config.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      646 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/src/inmanta_ui/const.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4114 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/src/inmanta_ui/ui.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-06 15:20:44.599880 inmanta-ui-4.0.1/src/inmanta_ui.egg-info/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      321 2023-02-06 15:20:44.000000 inmanta-ui-4.0.1/src/inmanta_ui.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      472 2023-02-06 15:20:44.000000 inmanta-ui-4.0.1/src/inmanta_ui.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-02-06 15:20:44.000000 inmanta-ui-4.0.1/src/inmanta_ui.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       37 2023-02-06 15:20:44.000000 inmanta-ui-4.0.1/src/inmanta_ui.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       23 2023-02-06 15:20:44.000000 inmanta-ui-4.0.1/src/inmanta_ui.egg-info/top_level.txt
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-06 15:20:44.599880 inmanta-ui-4.0.1/tests/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1962 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/tests/conftest.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2392 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/tests/web_console_handler_test.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1174 2023-02-06 15:19:04.000000 inmanta-ui-4.0.1/tox.ini
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.197758 inmanta-ui-4.0.2/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    10173 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/LICENSE
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      264 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/MANIFEST.in
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      321 2023-04-12 07:26:08.197758 inmanta-ui-4.0.2/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       58 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/README.md
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      384 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/pyproject.toml
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      558 2023-04-12 07:26:08.198758 inmanta-ui-4.0.2/setup.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      789 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/setup.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.195758 inmanta-ui-4.0.2/src/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.195758 inmanta-ui-4.0.2/src/inmanta_ext/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.196758 inmanta-ui-4.0.2/src/inmanta_ext/ui/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/src/inmanta_ext/ui/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      815 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/src/inmanta_ext/ui/extension.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.196758 inmanta-ui-4.0.2/src/inmanta_ui/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/src/inmanta_ui/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1765 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/src/inmanta_ui/config.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      646 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/src/inmanta_ui/const.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4114 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/src/inmanta_ui/ui.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.197758 inmanta-ui-4.0.2/src/inmanta_ui.egg-info/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      321 2023-04-12 07:26:08.000000 inmanta-ui-4.0.2/src/inmanta_ui.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      472 2023-04-12 07:26:08.000000 inmanta-ui-4.0.2/src/inmanta_ui.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-04-12 07:26:08.000000 inmanta-ui-4.0.2/src/inmanta_ui.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       37 2023-04-12 07:26:08.000000 inmanta-ui-4.0.2/src/inmanta_ui.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       23 2023-04-12 07:26:08.000000 inmanta-ui-4.0.2/src/inmanta_ui.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:08.197758 inmanta-ui-4.0.2/tests/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1962 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/tests/conftest.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2392 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/tests/web_console_handler_test.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1174 2023-04-12 07:23:18.000000 inmanta-ui-4.0.2/tox.ini
```

### Comparing `inmanta-ui-4.0.1/LICENSE` & `inmanta-ui-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.1/setup.cfg` & `inmanta-ui-4.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.1/setup.py` & `inmanta-ui-4.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "inmanta-core>=6.0.0.dev",
     "tornado~=6.0",
 ]
 
 namespace_packages = ["inmanta_ext.ui"]
 
 setup(
-    version="4.0.1",
+    version="4.0.2",
     python_requires=">=3.9",  # also update classifiers
     # Meta data
     name="inmanta-ui",
     description="Slice serving the inmanta UI",
     author="Inmanta",
     author_email="code@inmanta.com",
     url="https://github.com/inmanta/inmanta-ui",
```

### Comparing `inmanta-ui-4.0.1/src/inmanta_ext/ui/__init__.py` & `inmanta-ui-4.0.2/src/inmanta_ext/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.1/src/inmanta_ext/ui/extension.py` & `inmanta-ui-4.0.2/src/inmanta_ext/ui/extension.py`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.1/src/inmanta_ui/__init__.py` & `inmanta-ui-4.0.2/src/inmanta_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.1/src/inmanta_ui/config.py` & `inmanta-ui-4.0.2/src/inmanta_ui/config.py`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.1/src/inmanta_ui/const.py` & `inmanta-ui-4.0.2/src/inmanta_ui/const.py`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.1/src/inmanta_ui/ui.py` & `inmanta-ui-4.0.2/src/inmanta_ui/ui.py`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.1/tests/conftest.py` & `inmanta-ui-4.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.1/tests/web_console_handler_test.py` & `inmanta-ui-4.0.2/tests/web_console_handler_test.py`

 * *Files identical despite different names*

### Comparing `inmanta-ui-4.0.1/tox.ini` & `inmanta-ui-4.0.2/tox.ini`

 * *Files identical despite different names*

