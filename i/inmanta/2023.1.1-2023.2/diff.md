# Comparing `tmp/inmanta-2023.1.1.tar.gz` & `tmp/inmanta-2023.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmanta-2023.1.1.tar", last modified: Fri Feb 17 16:50:24 2023, max compression
+gzip compressed data, was "inmanta-2023.2.tar", last modified: Wed Apr 12 08:14:20 2023, max compression
```

## Comparing `inmanta-2023.1.1.tar` & `inmanta-2023.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-17 16:50:24.865526 inmanta-2023.1.1/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11357 2023-02-17 16:48:59.000000 inmanta-2023.1.1/LICENSE
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       17 2023-02-17 16:48:59.000000 inmanta-2023.1.1/MANIFEST.in
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      819 2023-02-17 16:50:24.865526 inmanta-2023.1.1/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      245 2023-02-17 16:48:59.000000 inmanta-2023.1.1/README.md
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-17 16:50:24.865526 inmanta-2023.1.1/inmanta.egg-info/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      819 2023-02-17 16:50:24.000000 inmanta-2023.1.1/inmanta.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      217 2023-02-17 16:50:24.000000 inmanta-2023.1.1/inmanta.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-02-17 16:50:24.000000 inmanta-2023.1.1/inmanta.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       38 2023-02-17 16:50:24.000000 inmanta-2023.1.1/inmanta.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-02-17 16:50:24.000000 inmanta-2023.1.1/inmanta.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1880 2023-02-17 16:48:59.000000 inmanta-2023.1.1/pyproject.toml
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       59 2023-02-17 16:50:24.865526 inmanta-2023.1.1/setup.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1141 2023-02-17 16:48:59.000000 inmanta-2023.1.1/setup.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 08:14:20.505241 inmanta-2023.2/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11357 2023-04-12 08:12:46.000000 inmanta-2023.2/LICENSE
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       17 2023-04-12 08:12:46.000000 inmanta-2023.2/MANIFEST.in
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      817 2023-04-12 08:14:20.505241 inmanta-2023.2/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      245 2023-04-12 08:12:46.000000 inmanta-2023.2/README.md
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 08:14:20.505241 inmanta-2023.2/inmanta.egg-info/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      817 2023-04-12 08:14:20.000000 inmanta-2023.2/inmanta.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      217 2023-04-12 08:14:20.000000 inmanta-2023.2/inmanta.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-04-12 08:14:20.000000 inmanta-2023.2/inmanta.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       38 2023-04-12 08:14:20.000000 inmanta-2023.2/inmanta.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-04-12 08:14:20.000000 inmanta-2023.2/inmanta.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1880 2023-04-12 08:12:46.000000 inmanta-2023.2/pyproject.toml
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       59 2023-04-12 08:14:20.506241 inmanta-2023.2/setup.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1139 2023-04-12 08:12:46.000000 inmanta-2023.2/setup.py
```

### Comparing `inmanta-2023.1.1/LICENSE` & `inmanta-2023.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inmanta-2023.1.1/PKG-INFO` & `inmanta-2023.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta
-Version: 2023.1.1
+Version: 2023.2
 Summary: Inmanta deployment tool
 Home-page: https://github.com/inmanta/inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Project-URL: Documentation, https://docs.inmanta.com/community/latest/
```

### Comparing `inmanta-2023.1.1/inmanta.egg-info/PKG-INFO` & `inmanta-2023.2/inmanta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta
-Version: 2023.1.1
+Version: 2023.2
 Summary: Inmanta deployment tool
 Home-page: https://github.com/inmanta/inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Project-URL: Documentation, https://docs.inmanta.com/community/latest/
```

### Comparing `inmanta-2023.1.1/pyproject.toml` & `inmanta-2023.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,8 @@
 image_name = "orchestrator"
 image_tags = [ "latest", "{version}",]
 registry_username_env = "GITHUB_REGISTRY_USERNAME"
 registry_password_env = "GITHUB_REGISTRY_PASSWORD"
 
 [tool.irt.dependencies.npm.web-console]
 repo = "https://github.com/inmanta/web-console"
-version = "==1.12.2"
+version = "==1.12.3"
```

### Comparing `inmanta-2023.1.1/setup.py` & `inmanta-2023.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(
-    version="2023.1.1",
+    version="2023.2",
     python_requires=">=3.9",  # also update classifiers
     # Meta data
     name="inmanta",
     description="Inmanta deployment tool",
     author="Inmanta",
     author_email="code@inmanta.com",
     url="https://github.com/inmanta/inmanta",
@@ -22,13 +22,13 @@
     ],
     keywords="orchestrator orchestration configurationmanagement",
     project_urls={
         "Bug Tracker": "https://github.com/inmanta/inmanta-core/issues",
         "Documentation": "https://docs.inmanta.com/community/latest/",
     },
     install_requires=[
-        "inmanta-core==8.1.0",
-        "inmanta-ui==4.0.1",
+        "inmanta-core==8.3.0",
+        "inmanta-ui==4.0.2",
     ],
     # explicitly declare packages so setuptools does not attempt auto discovery
     packages=[],
 )
```

