# Comparing `tmp/pure_safetensors-0.3.0.tar.gz` & `tmp/pure_safetensors-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_safetensors-0.3.0.tar", last modified: Wed Apr 12 08:38:33 2023, max compression
+gzip compressed data, was "pure_safetensors-0.3.1.tar", last modified: Wed Apr 12 08:48:52 2023, max compression
```

## Comparing `pure_safetensors-0.3.0.tar` & `pure_safetensors-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:38:33.558594 pure_safetensors-0.3.0/
--rw-r--r--   0 user      (1000) user      (1000)     4165 2023-04-12 08:38:33.558594 pure_safetensors-0.3.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     3174 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/README.md
--rw-r--r--   0 user      (1000) user      (1000)       50 2023-04-10 08:57:54.000000 pure_safetensors-0.3.0/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)      110 2023-04-12 08:38:33.558594 pure_safetensors-0.3.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      756 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:38:33.548594 pure_safetensors-0.3.0/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:38:33.548594 pure_safetensors-0.3.0/src/pure_safetensors/
--rw-r--r--   0 user      (1000) user      (1000)       35 2023-04-10 08:57:54.000000 pure_safetensors-0.3.0/src/pure_safetensors/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2270 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/__main__.py
--rw-r--r--   0 user      (1000) user      (1000)     2329 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/adapter.py
--rw-r--r--   0 user      (1000) user      (1000)      163 2023-04-10 08:57:54.000000 pure_safetensors-0.3.0/src/pure_safetensors/exc.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:38:33.558594 pure_safetensors-0.3.0/src/pure_safetensors/ext/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/ext/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     3305 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/ext/torch.py
--rw-r--r--   0 user      (1000) user      (1000)     4194 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/mmap.py
--rw-r--r--   0 user      (1000) user      (1000)     1472 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/numpy.py
--rw-r--r--   0 user      (1000) user      (1000)    26018 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/safetensors.py
--rw-r--r--   0 user      (1000) user      (1000)     1159 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:38:33.558594 pure_safetensors-0.3.0/src/pure_safetensors.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     4165 2023-04-12 08:38:33.000000 pure_safetensors-0.3.0/src/pure_safetensors.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      583 2023-04-12 08:38:33.000000 pure_safetensors-0.3.0/src/pure_safetensors.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-12 08:38:33.000000 pure_safetensors-0.3.0/src/pure_safetensors.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       36 2023-04-12 08:38:33.000000 pure_safetensors-0.3.0/src/pure_safetensors.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-12 08:38:33.000000 pure_safetensors-0.3.0/src/pure_safetensors.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/
+-rw-r--r--   0 user      (1000) user      (1000)      595 2023-04-12 08:48:07.000000 pure_safetensors-0.3.1/CHANGELOG.md
+-rw-r--r--   0 user      (1000) user      (1000)       58 2023-04-12 08:46:43.000000 pure_safetensors-0.3.1/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     4165 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     3174 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/README.md
+-rw-r--r--   0 user      (1000) user      (1000)       50 2023-04-10 08:57:54.000000 pure_safetensors-0.3.1/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)      110 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      756 2023-04-12 08:48:24.000000 pure_safetensors-0.3.1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:48:52.297149 pure_safetensors-0.3.1/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/src/pure_safetensors/
+-rw-r--r--   0 user      (1000) user      (1000)       35 2023-04-10 08:57:54.000000 pure_safetensors-0.3.1/src/pure_safetensors/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2270 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/__main__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2329 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/adapter.py
+-rw-r--r--   0 user      (1000) user      (1000)      163 2023-04-10 08:57:54.000000 pure_safetensors-0.3.1/src/pure_safetensors/exc.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/src/pure_safetensors/ext/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/ext/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3305 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/ext/torch.py
+-rw-r--r--   0 user      (1000) user      (1000)     4194 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/mmap.py
+-rw-r--r--   0 user      (1000) user      (1000)     1472 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/numpy.py
+-rw-r--r--   0 user      (1000) user      (1000)    26018 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/safetensors.py
+-rw-r--r--   0 user      (1000) user      (1000)     1159 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/src/pure_safetensors/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/src/pure_safetensors.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     4165 2023-04-12 08:48:51.000000 pure_safetensors-0.3.1/src/pure_safetensors.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      714 2023-04-12 08:48:52.000000 pure_safetensors-0.3.1/src/pure_safetensors.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-12 08:48:51.000000 pure_safetensors-0.3.1/src/pure_safetensors.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       36 2023-04-12 08:48:51.000000 pure_safetensors-0.3.1/src/pure_safetensors.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-12 08:48:51.000000 pure_safetensors-0.3.1/src/pure_safetensors.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:48:52.307149 pure_safetensors-0.3.1/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-04-10 08:57:54.000000 pure_safetensors-0.3.1/tests/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      442 2023-04-10 08:57:54.000000 pure_safetensors-0.3.1/tests/conftest.py
+-rw-r--r--   0 user      (1000) user      (1000)       56 2023-04-10 08:57:54.000000 pure_safetensors-0.3.1/tests/test_errors.py
+-rw-r--r--   0 user      (1000) user      (1000)     2113 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/tests/test_hypothesis.py
+-rw-r--r--   0 user      (1000) user      (1000)     2127 2023-04-12 08:38:25.000000 pure_safetensors-0.3.1/tests/test_roundtrip.py
```

### Comparing `pure_safetensors-0.3.0/PKG-INFO` & `pure_safetensors-0.3.1/src/pure_safetensors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pure_safetensors
-Version: 0.3.0
+Name: pure-safetensors
+Version: 0.3.1
 Summary: Pure-Python safetensors
 Home-page: UNKNOWN
 Author: Eduard Christian Dumitrescu
 Author-email: eduard.c.dumitrescu@gmail.com
 License: MIT
 Description: # pure_safetensors
```

### Comparing `pure_safetensors-0.3.0/README.md` & `pure_safetensors-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pure_safetensors-0.3.0/setup.py` & `pure_safetensors-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text("utf-8")
 
 setup(
     name="pure_safetensors",
     description="Pure-Python safetensors",
-    version="0.3.0",
+    version="0.3.1",
     author="Eduard Christian Dumitrescu",
     author_email="eduard.c.dumitrescu@gmail.com",
     install_requires=["attrs", "marshmallow", "sortedcollections"],
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     license="MIT",
     classifiers=[
```

### Comparing `pure_safetensors-0.3.0/src/pure_safetensors/__main__.py` & `pure_safetensors-0.3.1/src/pure_safetensors/__main__.py`

 * *Files identical despite different names*

### Comparing `pure_safetensors-0.3.0/src/pure_safetensors/adapter.py` & `pure_safetensors-0.3.1/src/pure_safetensors/adapter.py`

 * *Files identical despite different names*

### Comparing `pure_safetensors-0.3.0/src/pure_safetensors/ext/torch.py` & `pure_safetensors-0.3.1/src/pure_safetensors/ext/torch.py`

 * *Files identical despite different names*

### Comparing `pure_safetensors-0.3.0/src/pure_safetensors/mmap.py` & `pure_safetensors-0.3.1/src/pure_safetensors/mmap.py`

 * *Files identical despite different names*

### Comparing `pure_safetensors-0.3.0/src/pure_safetensors/numpy.py` & `pure_safetensors-0.3.1/src/pure_safetensors/numpy.py`

 * *Files identical despite different names*

### Comparing `pure_safetensors-0.3.0/src/pure_safetensors/safetensors.py` & `pure_safetensors-0.3.1/src/pure_safetensors/safetensors.py`

 * *Files identical despite different names*

### Comparing `pure_safetensors-0.3.0/src/pure_safetensors/util.py` & `pure_safetensors-0.3.1/src/pure_safetensors/util.py`

 * *Files identical despite different names*

### Comparing `pure_safetensors-0.3.0/src/pure_safetensors.egg-info/PKG-INFO` & `pure_safetensors-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pure-safetensors
-Version: 0.3.0
+Name: pure_safetensors
+Version: 0.3.1
 Summary: Pure-Python safetensors
 Home-page: UNKNOWN
 Author: Eduard Christian Dumitrescu
 Author-email: eduard.c.dumitrescu@gmail.com
 License: MIT
 Description: # pure_safetensors
```

