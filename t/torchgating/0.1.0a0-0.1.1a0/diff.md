# Comparing `tmp/torchgating-0.1.0a0.tar.gz` & `tmp/torchgating-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchgating-0.1.0a0.tar", last modified: Wed Apr 12 20:24:00 2023, max compression
+gzip compressed data, was "torchgating-0.1.1a0.tar", last modified: Wed Apr 12 20:38:24 2023, max compression
```

## Comparing `torchgating-0.1.0a0.tar` & `torchgating-0.1.1a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:24:00.147278 torchgating-0.1.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 20:23:44.000000 torchgating-0.1.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-12 20:24:00.147278 torchgating-0.1.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-12 20:23:44.000000 torchgating-0.1.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:24:00.147278 torchgating-0.1.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 20:23:44.000000 torchgating-0.1.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:24:00.147278 torchgating-0.1.0a0/torchgating/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-12 20:23:44.000000 torchgating-0.1.0a0/torchgating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-04-12 20:23:44.000000 torchgating-0.1.0a0/torchgating/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-04-12 20:23:44.000000 torchgating-0.1.0a0/torchgating/torchgating.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-12 20:23:44.000000 torchgating-0.1.0a0/torchgating/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 20:23:44.000000 torchgating-0.1.0a0/torchgating/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:24:00.147278 torchgating-0.1.0a0/torchgating.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-12 20:24:00.000000 torchgating-0.1.0a0/torchgating.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 20:24:00.000000 torchgating-0.1.0a0/torchgating.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:24:00.000000 torchgating-0.1.0a0/torchgating.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 20:24:00.000000 torchgating-0.1.0a0/torchgating.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 20:24:00.000000 torchgating-0.1.0a0/torchgating.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 20:24:00.000000 torchgating-0.1.0a0/torchgating.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:38:24.986551 torchgating-0.1.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-12 20:38:24.986551 torchgating-0.1.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:38:24.986551 torchgating-0.1.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:38:24.982551 torchgating-0.1.1a0/torchgating/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/torchgating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/torchgating/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/torchgating/torchgating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/torchgating/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/torchgating/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:38:24.986551 torchgating-0.1.1a0/torchgating.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-12 20:38:24.000000 torchgating-0.1.1a0/torchgating.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 20:38:24.000000 torchgating-0.1.1a0/torchgating.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:38:24.000000 torchgating-0.1.1a0/torchgating.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 20:38:24.000000 torchgating-0.1.1a0/torchgating.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 20:38:24.000000 torchgating-0.1.1a0/torchgating.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 20:38:24.000000 torchgating-0.1.1a0/torchgating.egg-info/top_level.txt
```

### Comparing `torchgating-0.1.0a0/LICENSE` & `torchgating-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchgating-0.1.0a0/PKG-INFO` & `torchgating-0.1.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchgating
-Version: 0.1.0a0
+Version: 0.1.1a0
 Summary: A PyTorch-based implementation of Spectral Gating, an algorithm for denoising audio signals
 Home-page: https://github.com/nuniz/TorchSpectralGating
 Author: Asaf Zorea
 Author-email: zoreasaf@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torchgating-0.1.0a0/README.md` & `torchgating-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `torchgating-0.1.0a0/setup.py` & `torchgating-0.1.1a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="torchgating",
-    version="0.1.0-alpha",
+    version="0.1.1-alpha",
     author="Asaf Zorea",
     author_email="zoreasaf@gmail.com",
     description="A PyTorch-based implementation of Spectral Gating, an algorithm for denoising audio signals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     url="https://github.com/nuniz/TorchSpectralGating",
@@ -20,12 +20,12 @@
         'License :: OSI Approved :: MIT License',
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     entry_points={"console_scripts": ["torchgating = torchgating.run:main"]},
     install_requires=[
         "matplotlib >= 3.7.1",
-        "numpy >= 1.24.2",
+        "numpy >= 1.23.5",
         "soundfile >= 0.11.0",
         "torch >= 2.0.0",
     ],
 )
```

### Comparing `torchgating-0.1.0a0/torchgating/__init__.py` & `torchgating-0.1.1a0/torchgating/__init__.py`

 * *Files identical despite different names*

### Comparing `torchgating-0.1.0a0/torchgating/run.py` & `torchgating-0.1.1a0/torchgating/run.py`

 * *Files identical despite different names*

### Comparing `torchgating-0.1.0a0/torchgating/torchgating.py` & `torchgating-0.1.1a0/torchgating/torchgating.py`

 * *Files identical despite different names*

### Comparing `torchgating-0.1.0a0/torchgating/utils.py` & `torchgating-0.1.1a0/torchgating/utils.py`

 * *Files identical despite different names*

### Comparing `torchgating-0.1.0a0/torchgating.egg-info/PKG-INFO` & `torchgating-0.1.1a0/torchgating.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchgating
-Version: 0.1.0a0
+Version: 0.1.1a0
 Summary: A PyTorch-based implementation of Spectral Gating, an algorithm for denoising audio signals
 Home-page: https://github.com/nuniz/TorchSpectralGating
 Author: Asaf Zorea
 Author-email: zoreasaf@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

