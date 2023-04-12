# Comparing `tmp/fast_jl-0.1.2.tar.gz` & `tmp/fast_jl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_jl-0.1.2.tar", last modified: Sun Mar 19 04:22:41 2023, max compression
+gzip compressed data, was "fast_jl-0.1.3.tar", last modified: Wed Apr 12 17:53:46 2023, max compression
```

## Comparing `fast_jl-0.1.2.tar` & `fast_jl-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-03-19 04:22:41.344279 fast_jl-0.1.2/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       14 2023-03-19 03:13:04.000000 fast_jl-0.1.2/MANIFEST.in
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      361 2023-03-19 04:22:41.340279 fast_jl-0.1.2/PKG-INFO
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      211 2023-03-19 04:18:54.000000 fast_jl-0.1.2/README.rst
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1752 2023-03-19 02:36:41.000000 fast_jl-0.1.2/data_loading.cuh
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1030 2023-03-19 02:36:41.000000 fast_jl-0.1.2/error_handling.cuh
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4512 2023-03-19 02:36:41.000000 fast_jl-0.1.2/fast_jl.cu
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-03-19 04:22:41.324278 fast_jl-0.1.2/fast_jl.egg-info/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      361 2023-03-19 04:22:41.000000 fast_jl-0.1.2/fast_jl.egg-info/PKG-INFO
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      242 2023-03-19 04:22:41.000000 fast_jl-0.1.2/fast_jl.egg-info/SOURCES.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        1 2023-03-19 04:22:41.000000 fast_jl-0.1.2/fast_jl.egg-info/dependency_links.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        8 2023-03-19 04:22:41.000000 fast_jl-0.1.2/fast_jl.egg-info/top_level.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4958 2023-03-19 02:36:41.000000 fast_jl-0.1.2/fast_jl_kernel.cuh
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1989 2023-03-19 02:36:41.000000 fast_jl-0.1.2/random.cuh
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       38 2023-03-19 04:22:41.348279 fast_jl-0.1.2/setup.cfg
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      633 2023-03-19 04:21:04.000000 fast_jl-0.1.2/setup.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       68 2023-03-19 02:36:41.000000 fast_jl-0.1.2/types.cuh
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-12 17:53:46.406926 fast_jl-0.1.3/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       14 2023-03-27 15:11:23.000000 fast_jl-0.1.3/MANIFEST.in
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      361 2023-04-12 17:53:46.390926 fast_jl-0.1.3/PKG-INFO
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      211 2023-03-27 15:11:23.000000 fast_jl-0.1.3/README.rst
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1752 2023-03-27 15:11:23.000000 fast_jl-0.1.3/data_loading.cuh
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1030 2023-03-27 15:11:23.000000 fast_jl-0.1.3/error_handling.cuh
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4512 2023-03-27 15:11:23.000000 fast_jl-0.1.3/fast_jl.cu
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-12 17:53:46.358926 fast_jl-0.1.3/fast_jl.egg-info/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      361 2023-04-12 17:53:44.000000 fast_jl-0.1.3/fast_jl.egg-info/PKG-INFO
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      272 2023-04-12 17:53:45.000000 fast_jl-0.1.3/fast_jl.egg-info/SOURCES.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        1 2023-04-12 17:53:44.000000 fast_jl-0.1.3/fast_jl.egg-info/dependency_links.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       13 2023-04-12 17:53:44.000000 fast_jl-0.1.3/fast_jl.egg-info/requires.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        8 2023-04-12 17:53:44.000000 fast_jl-0.1.3/fast_jl.egg-info/top_level.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4958 2023-03-27 15:11:24.000000 fast_jl-0.1.3/fast_jl_kernel.cuh
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1989 2023-03-27 15:11:24.000000 fast_jl-0.1.3/random.cuh
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       38 2023-04-12 17:53:46.410926 fast_jl-0.1.3/setup.cfg
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      673 2023-04-12 17:48:19.000000 fast_jl-0.1.3/setup.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       68 2023-03-27 15:11:24.000000 fast_jl-0.1.3/types.cuh
```

### Comparing `fast_jl-0.1.2/data_loading.cuh` & `fast_jl-0.1.3/data_loading.cuh`

 * *Files identical despite different names*

### Comparing `fast_jl-0.1.2/error_handling.cuh` & `fast_jl-0.1.3/error_handling.cuh`

 * *Files identical despite different names*

### Comparing `fast_jl-0.1.2/fast_jl.cu` & `fast_jl-0.1.3/fast_jl.cu`

 * *Files identical despite different names*

### Comparing `fast_jl-0.1.2/fast_jl_kernel.cuh` & `fast_jl-0.1.3/fast_jl_kernel.cuh`

 * *Files identical despite different names*

### Comparing `fast_jl-0.1.2/random.cuh` & `fast_jl-0.1.3/random.cuh`

 * *Files identical despite different names*

### Comparing `fast_jl-0.1.2/setup.py` & `fast_jl-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 from setuptools import setup
 from torch.utils.cpp_extension import BuildExtension, CUDAExtension
 
 long_description = open('README.rst').read()
 
 setup(
     name='fast_jl',
-    version="0.1.2",
+    version="0.1.3",
     description="Fast JL: Compute JL projection fast on a GPU",
     author="MadryLab",
     author_email='trak@mit.edu',
+    install_requires=["torch>=2.0.0"],
     long_description=long_description,
     ext_modules=[
         CUDAExtension('fast_jl', [
             'fast_jl.cu',
         ]),
     ],
     cmdclass={
         'build_ext': BuildExtension
     },
-    setup_requires=["torch>=1.13"])
+    setup_requires=["torch>=2.0.0"])
```

