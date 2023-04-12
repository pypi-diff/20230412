# Comparing `tmp/packaging-23.0.tar.gz` & `tmp/packaging-23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaging-23.0.tar", last modified: Sun Jan  8 18:18:30 2023, max compression
+gzip compressed data, was "packaging-23.1.tar", last modified: Wed Apr 12 16:10:29 2023, max compression
```

## Comparing `packaging-23.0.tar` & `packaging-23.1.tar`

### file list

```diff
@@ -1,70 +1,74 @@
--rw-r--r--   0        0        0      197 2021-07-23 07:28:26.383309 packaging-23.0/LICENSE
--rw-r--r--   0        0        0    10174 2021-07-23 07:28:26.383397 packaging-23.0/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2021-07-23 07:28:26.383450 packaging-23.0/LICENSE.BSD
--rw-r--r--   0        0        0     1985 2021-07-23 07:28:26.383510 packaging-23.0/README.rst
--rw-r--r--   0        0        0     5576 2021-07-23 07:28:26.383594 packaging-23.0/docs/Makefile
--rw-r--r--   0        0        0       30 2021-07-23 07:28:26.383694 packaging-23.0/docs/changelog.rst
--rw-r--r--   0        0        0     2465 2022-12-08 23:11:51.458772 packaging-23.0/docs/conf.py
--rw-r--r--   0        0        0     2234 2022-04-02 13:23:31.358311 packaging-23.0/docs/development/getting-started.rst
--rw-r--r--   0        0        0      542 2021-07-23 07:28:26.383909 packaging-23.0/docs/development/index.rst
--rw-r--r--   0        0        0      674 2022-04-02 13:23:31.358473 packaging-23.0/docs/development/release-process.rst
--rw-r--r--   0        0        0     1014 2021-07-23 07:28:26.384014 packaging-23.0/docs/development/reviewing-patches.rst
--rw-r--r--   0        0        0     2504 2022-04-02 13:23:31.358636 packaging-23.0/docs/development/submitting-patches.rst
--rw-r--r--   0        0        0      517 2022-11-25 19:59:55.164905 packaging-23.0/docs/index.rst
--rw-r--r--   0        0        0     3285 2022-07-08 12:30:32.570928 packaging-23.0/docs/markers.rst
--rw-r--r--   0        0        0     2751 2022-04-02 13:23:31.358980 packaging-23.0/docs/requirements.rst
--rw-r--r--   0        0        0        5 2021-07-23 07:28:26.384317 packaging-23.0/docs/requirements.txt
--rw-r--r--   0        0        0      685 2021-07-23 07:28:26.384382 packaging-23.0/docs/security.rst
--rw-r--r--   0        0        0     1851 2022-07-19 08:25:45.864361 packaging-23.0/docs/specifiers.rst
--rw-r--r--   0        0        0     8446 2022-10-19 02:08:27.175917 packaging-23.0/docs/tags.rst
--rw-r--r--   0        0        0     3777 2022-09-30 09:55:33.603357 packaging-23.0/docs/utils.rst
--rw-r--r--   0        0        0     1148 2022-07-19 08:25:45.864537 packaging-23.0/docs/version.rst
--rw-r--r--   0        0        0     1763 2022-12-08 23:11:51.459903 packaging-23.0/pyproject.toml
--rw-r--r--   0        0        0      501 2023-01-08 18:18:23.340532 packaging-23.0/src/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2023-01-08 18:00:19.700658 packaging-23.0/src/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2022-12-08 23:11:51.460600 packaging-23.0/src/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2022-12-08 23:11:51.460754 packaging-23.0/src/packaging/_musllinux.py
--rw-r--r--   0        0        0     9399 2023-01-08 18:00:19.700918 packaging-23.0/src/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2022-12-08 23:11:51.461317 packaging-23.0/src/packaging/_structures.py
--rw-r--r--   0        0        0     5148 2022-12-13 07:03:34.352187 packaging-23.0/src/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8161 2022-12-27 15:22:45.000761 packaging-23.0/src/packaging/markers.py
--rw-r--r--   0        0        0        0 2022-12-08 23:11:51.461810 packaging-23.0/src/packaging/py.typed
--rw-r--r--   0        0        0     3264 2022-12-08 23:11:51.462091 packaging-23.0/src/packaging/requirements.py
--rw-r--r--   0        0        0    39046 2023-01-08 18:00:19.701309 packaging-23.0/src/packaging/specifiers.py
--rw-r--r--   0        0        0    18065 2022-12-26 19:52:02.396540 packaging-23.0/src/packaging/tags.py
--rw-r--r--   0        0        0     4355 2022-12-08 23:11:51.462984 packaging-23.0/src/packaging/utils.py
--rw-r--r--   0        0        0    16295 2022-12-08 23:11:51.463324 packaging-23.0/src/packaging/version.py
--rw-r--r--   0        0        0       37 2022-12-05 22:26:39.314466 packaging-23.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-12-05 22:26:39.314566 packaging-23.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2022-12-05 22:26:39.314287 packaging-23.0/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0   930440 2022-12-05 22:35:43.360335 packaging-23.0/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0  1041734 2022-12-05 22:35:43.350332 packaging-23.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-12-05 22:35:43.360882 packaging-23.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      180 2021-07-23 07:28:49.881132 packaging-23.0/tests/__init__.py
--rwxr-xr-x   0        0        0     1794 2022-04-02 13:23:31.362626 packaging-23.0/tests/manylinux/build.sh
--rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.362691 packaging-23.0/tests/manylinux/hello-world-armv7l-armel
--rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.362750 packaging-23.0/tests/manylinux/hello-world-armv7l-armhf
--rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.362813 packaging-23.0/tests/manylinux/hello-world-invalid-class
--rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.362872 packaging-23.0/tests/manylinux/hello-world-invalid-data
--rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.362938 packaging-23.0/tests/manylinux/hello-world-invalid-magic
--rw-r--r--   0        0        0       64 2022-04-02 13:23:31.363000 packaging-23.0/tests/manylinux/hello-world-s390x-s390x
--rw-r--r--   0        0        0       40 2022-04-02 13:23:31.363059 packaging-23.0/tests/manylinux/hello-world-too-short
--rw-r--r--   0        0        0       64 2022-04-02 13:23:31.363115 packaging-23.0/tests/manylinux/hello-world-x86_64-amd64
--rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.363175 packaging-23.0/tests/manylinux/hello-world-x86_64-i386
--rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.363241 packaging-23.0/tests/manylinux/hello-world-x86_64-x32
--rwxr-xr-x   0        0        0     1024 2022-04-02 13:23:31.363438 packaging-23.0/tests/musllinux/glibc-x86_64
--rwxr-xr-x   0        0        0     1024 2022-04-02 13:23:31.363588 packaging-23.0/tests/musllinux/musl-aarch64
--rwxr-xr-x   0        0        0     1024 2022-04-02 13:23:31.363691 packaging-23.0/tests/musllinux/musl-i386
--rwxr-xr-x   0        0        0     1024 2022-04-02 13:23:31.363767 packaging-23.0/tests/musllinux/musl-x86_64
--rw-r--r--   0        0        0       55 2022-12-02 10:53:09.960909 packaging-23.0/tests/requirements.txt
--rw-r--r--   0        0        0     3162 2022-09-30 09:55:33.606015 packaging-23.0/tests/test_elffile.py
--rw-r--r--   0        0        0     5623 2022-09-30 09:55:33.606207 packaging-23.0/tests/test_manylinux.py
--rw-r--r--   0        0        0    13613 2022-12-27 15:22:45.001005 packaging-23.0/tests/test_markers.py
--rw-r--r--   0        0        0     2534 2022-09-30 09:55:33.606582 packaging-23.0/tests/test_musllinux.py
--rw-r--r--   0        0        0    17998 2023-01-08 18:18:04.410140 packaging-23.0/tests/test_requirements.py
--rw-r--r--   0        0        0    29838 2022-09-30 09:55:33.607073 packaging-23.0/tests/test_specifiers.py
--rw-r--r--   0        0        0     1495 2022-04-02 13:23:31.364833 packaging-23.0/tests/test_structures.py
--rw-r--r--   0        0        0    52084 2022-12-26 19:52:02.397271 packaging-23.0/tests/test_tags.py
--rw-r--r--   0        0        0     3796 2022-07-08 21:36:48.260461 packaging-23.0/tests/test_utils.py
--rw-r--r--   0        0        0    26322 2022-07-08 21:36:48.260927 packaging-23.0/tests/test_version.py
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 packaging-23.0/PKG-INFO
+-rw-r--r--   0        0        0      197 2021-07-23 07:28:26.383309 packaging-23.1/LICENSE
+-rw-r--r--   0        0        0    10174 2021-07-23 07:28:26.383397 packaging-23.1/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2021-07-23 07:28:26.383450 packaging-23.1/LICENSE.BSD
+-rw-r--r--   0        0        0     1985 2021-07-23 07:28:26.383510 packaging-23.1/README.rst
+-rw-r--r--   0        0        0     5576 2021-07-23 07:28:26.383594 packaging-23.1/docs/Makefile
+-rw-r--r--   0        0        0       30 2021-07-23 07:28:26.383694 packaging-23.1/docs/changelog.rst
+-rw-r--r--   0        0        0     2465 2023-01-30 15:29:49.447726 packaging-23.1/docs/conf.py
+-rw-r--r--   0        0        0     2234 2023-01-30 15:24:13.025143 packaging-23.1/docs/development/getting-started.rst
+-rw-r--r--   0        0        0      542 2021-07-23 07:28:26.383909 packaging-23.1/docs/development/index.rst
+-rw-r--r--   0        0        0      674 2022-04-02 13:23:31.358473 packaging-23.1/docs/development/release-process.rst
+-rw-r--r--   0        0        0     1014 2021-07-23 07:28:26.384014 packaging-23.1/docs/development/reviewing-patches.rst
+-rw-r--r--   0        0        0     2504 2022-04-02 13:23:31.358636 packaging-23.1/docs/development/submitting-patches.rst
+-rw-r--r--   0        0        0      530 2023-04-12 16:05:06.672022 packaging-23.1/docs/index.rst
+-rw-r--r--   0        0        0     3285 2023-01-30 15:24:13.025342 packaging-23.1/docs/markers.rst
+-rw-r--r--   0        0        0     1069 2023-04-12 16:05:06.672171 packaging-23.1/docs/metadata.rst
+-rw-r--r--   0        0        0     2751 2023-01-30 15:24:13.025904 packaging-23.1/docs/requirements.rst
+-rw-r--r--   0        0        0        5 2021-07-23 07:28:26.384317 packaging-23.1/docs/requirements.txt
+-rw-r--r--   0        0        0      685 2021-07-23 07:28:26.384382 packaging-23.1/docs/security.rst
+-rw-r--r--   0        0        0     1851 2023-01-30 15:24:13.026548 packaging-23.1/docs/specifiers.rst
+-rw-r--r--   0        0        0     8446 2023-01-30 15:29:49.448389 packaging-23.1/docs/tags.rst
+-rw-r--r--   0        0        0     3777 2023-01-30 15:24:46.662988 packaging-23.1/docs/utils.rst
+-rw-r--r--   0        0        0     1148 2023-01-30 15:24:13.028470 packaging-23.1/docs/version.rst
+-rw-r--r--   0        0        0     1784 2023-01-30 15:29:49.449063 packaging-23.1/pyproject.toml
+-rw-r--r--   0        0        0      501 2023-04-12 16:10:22.111652 packaging-23.1/src/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2023-01-30 15:29:49.449590 packaging-23.1/src/packaging/_elffile.py
+-rw-r--r--   0        0        0     8926 2023-04-12 16:05:06.672746 packaging-23.1/src/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2023-01-30 15:29:49.452191 packaging-23.1/src/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10194 2023-04-12 16:05:06.673098 packaging-23.1/src/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2023-01-30 15:29:49.452970 packaging-23.1/src/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2023-04-12 16:05:06.673353 packaging-23.1/src/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2023-04-12 16:05:29.534912 packaging-23.1/src/packaging/markers.py
+-rw-r--r--   0        0        0    16397 2023-04-12 16:05:06.674206 packaging-23.1/src/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2023-01-30 15:29:49.453567 packaging-23.1/src/packaging/py.typed
+-rw-r--r--   0        0        0     3287 2023-04-12 16:05:06.674517 packaging-23.1/src/packaging/requirements.py
+-rw-r--r--   0        0        0    39206 2023-04-12 16:05:06.674899 packaging-23.1/src/packaging/specifiers.py
+-rw-r--r--   0        0        0    18106 2023-04-12 16:05:06.675215 packaging-23.1/src/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2023-01-30 15:29:49.455153 packaging-23.1/src/packaging/utils.py
+-rw-r--r--   0        0        0    16326 2023-04-12 16:05:06.675496 packaging-23.1/src/packaging/version.py
+-rw-r--r--   0        0        0       37 2022-12-05 22:26:39.314466 packaging-23.1/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-12-05 22:26:39.314566 packaging-23.1/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2022-12-05 22:26:39.314287 packaging-23.1/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0   930440 2022-12-05 22:35:43.360335 packaging-23.1/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0  1041734 2022-12-05 22:35:43.350332 packaging-23.1/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-12-05 22:35:43.360882 packaging-23.1/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      180 2021-07-23 07:28:49.881132 packaging-23.1/tests/__init__.py
+-rwxr-xr-x   0        0        0     1794 2022-04-02 13:23:31.362626 packaging-23.1/tests/manylinux/build.sh
+-rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.362691 packaging-23.1/tests/manylinux/hello-world-armv7l-armel
+-rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.362750 packaging-23.1/tests/manylinux/hello-world-armv7l-armhf
+-rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.362813 packaging-23.1/tests/manylinux/hello-world-invalid-class
+-rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.362872 packaging-23.1/tests/manylinux/hello-world-invalid-data
+-rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.362938 packaging-23.1/tests/manylinux/hello-world-invalid-magic
+-rw-r--r--   0        0        0       64 2022-04-02 13:23:31.363000 packaging-23.1/tests/manylinux/hello-world-s390x-s390x
+-rw-r--r--   0        0        0       40 2022-04-02 13:23:31.363059 packaging-23.1/tests/manylinux/hello-world-too-short
+-rw-r--r--   0        0        0       64 2022-04-02 13:23:31.363115 packaging-23.1/tests/manylinux/hello-world-x86_64-amd64
+-rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.363175 packaging-23.1/tests/manylinux/hello-world-x86_64-i386
+-rwxr-xr-x   0        0        0       52 2022-04-02 13:23:31.363241 packaging-23.1/tests/manylinux/hello-world-x86_64-x32
+-rw-r--r--   0        0        0     1630 2023-04-12 16:05:06.675785 packaging-23.1/tests/metadata/everything.metadata
+-rwxr-xr-x   0        0        0     1024 2022-04-02 13:23:31.363438 packaging-23.1/tests/musllinux/glibc-x86_64
+-rwxr-xr-x   0        0        0     1024 2022-04-02 13:23:31.363588 packaging-23.1/tests/musllinux/musl-aarch64
+-rwxr-xr-x   0        0        0     1024 2022-04-02 13:23:31.363691 packaging-23.1/tests/musllinux/musl-i386
+-rwxr-xr-x   0        0        0     1024 2022-04-02 13:23:31.363767 packaging-23.1/tests/musllinux/musl-x86_64
+-rw-r--r--   0        0        0       55 2023-01-30 15:29:49.455821 packaging-23.1/tests/requirements.txt
+-rw-r--r--   0        0        0     3162 2023-01-30 15:24:46.671083 packaging-23.1/tests/test_elffile.py
+-rw-r--r--   0        0        0     5616 2023-04-12 16:05:06.676032 packaging-23.1/tests/test_manylinux.py
+-rw-r--r--   0        0        0    13613 2023-01-30 15:29:49.456242 packaging-23.1/tests/test_markers.py
+-rw-r--r--   0        0        0     9237 2023-04-12 16:05:06.676202 packaging-23.1/tests/test_metadata.py
+-rw-r--r--   0        0        0     2534 2023-01-30 15:24:46.671568 packaging-23.1/tests/test_musllinux.py
+-rw-r--r--   0        0        0    19931 2023-04-12 16:05:06.676444 packaging-23.1/tests/test_requirements.py
+-rw-r--r--   0        0        0    29920 2023-04-12 16:05:06.676737 packaging-23.1/tests/test_specifiers.py
+-rw-r--r--   0        0        0     1495 2022-04-02 13:23:31.364833 packaging-23.1/tests/test_structures.py
+-rw-r--r--   0        0        0    52875 2023-04-12 16:05:06.677162 packaging-23.1/tests/test_tags.py
+-rw-r--r--   0        0        0     3796 2023-01-30 15:24:13.039983 packaging-23.1/tests/test_utils.py
+-rw-r--r--   0        0        0    26322 2023-01-30 15:24:13.040571 packaging-23.1/tests/test_version.py
+-rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 packaging-23.1/PKG-INFO
```

### Comparing `packaging-23.0/LICENSE.APACHE` & `packaging-23.1/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `packaging-23.0/LICENSE.BSD` & `packaging-23.1/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `packaging-23.0/README.rst` & `packaging-23.1/README.rst`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/Makefile` & `packaging-23.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/conf.py` & `packaging-23.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/development/getting-started.rst` & `packaging-23.1/docs/development/getting-started.rst`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/development/index.rst` & `packaging-23.1/docs/development/index.rst`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/development/release-process.rst` & `packaging-23.1/docs/development/release-process.rst`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/development/reviewing-patches.rst` & `packaging-23.1/docs/development/reviewing-patches.rst`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/development/submitting-patches.rst` & `packaging-23.1/docs/development/submitting-patches.rst`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/index.rst` & `packaging-23.1/docs/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     :caption: API Documentation
     :hidden:
 
     version
     specifiers
     markers
     requirements
+    metadata
     tags
     utils
 
 .. toctree::
     :maxdepth: 2
     :caption: Project
     :hidden:
```

### Comparing `packaging-23.0/docs/markers.rst` & `packaging-23.1/docs/markers.rst`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/requirements.rst` & `packaging-23.1/docs/requirements.rst`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/security.rst` & `packaging-23.1/docs/security.rst`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/specifiers.rst` & `packaging-23.1/docs/specifiers.rst`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/tags.rst` & `packaging-23.1/docs/tags.rst`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/utils.rst` & `packaging-23.1/docs/utils.rst`

 * *Files identical despite different names*

### Comparing `packaging-23.0/docs/version.rst` & `packaging-23.1/docs/version.rst`

 * *Files identical despite different names*

### Comparing `packaging-23.0/pyproject.toml` & `packaging-23.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
+  "Typing :: Typed",
 ]
 dependencies = []
 
 [project.urls]
 Documentation = "https://packaging.pypa.io/"
 Source = "https://github.com/pypa/packaging"
```

### Comparing `packaging-23.0/src/packaging/_elffile.py` & `packaging-23.1/src/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `packaging-23.0/src/packaging/_manylinux.py` & `packaging-23.1/src/packaging/_manylinux.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from ._elffile import EIClass, EIData, ELFFile, EMachine
 
 EF_ARM_ABIMASK = 0xFF000000
 EF_ARM_ABI_VER5 = 0x05000000
 EF_ARM_ABI_FLOAT_HARD = 0x00000400
 
 
+# `os.PathLike` not a generic type until Python 3.9, so sticking with `str`
+# as the type for `path` until then.
 @contextlib.contextmanager
 def _parse_elf(path: str) -> Generator[Optional[ELFFile], None, None]:
     try:
         with open(path, "rb") as f:
             yield ELFFile(f)
     except (OSError, TypeError, ValueError):
         yield None
```

### Comparing `packaging-23.0/src/packaging/_musllinux.py` & `packaging-23.1/src/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `packaging-23.0/src/packaging/_parser.py` & `packaging-23.1/src/packaging/_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,15 +159,19 @@
 def _parse_extras(tokenizer: Tokenizer) -> List[str]:
     """
     extras = (LEFT_BRACKET wsp* extras_list? wsp* RIGHT_BRACKET)?
     """
     if not tokenizer.check("LEFT_BRACKET", peek=True):
         return []
 
-    with tokenizer.enclosing_tokens("LEFT_BRACKET", "RIGHT_BRACKET"):
+    with tokenizer.enclosing_tokens(
+        "LEFT_BRACKET",
+        "RIGHT_BRACKET",
+        around="extras",
+    ):
         tokenizer.consume("WS")
         extras = _parse_extras_list(tokenizer)
         tokenizer.consume("WS")
 
     return extras
 
 
@@ -199,29 +203,46 @@
 
 
 def _parse_specifier(tokenizer: Tokenizer) -> str:
     """
     specifier = LEFT_PARENTHESIS WS? version_many WS? RIGHT_PARENTHESIS
               | WS? version_many WS?
     """
-    with tokenizer.enclosing_tokens("LEFT_PARENTHESIS", "RIGHT_PARENTHESIS"):
+    with tokenizer.enclosing_tokens(
+        "LEFT_PARENTHESIS",
+        "RIGHT_PARENTHESIS",
+        around="version specifier",
+    ):
         tokenizer.consume("WS")
         parsed_specifiers = _parse_version_many(tokenizer)
         tokenizer.consume("WS")
 
     return parsed_specifiers
 
 
 def _parse_version_many(tokenizer: Tokenizer) -> str:
     """
     version_many = (SPECIFIER (WS? COMMA WS? SPECIFIER)*)?
     """
     parsed_specifiers = ""
     while tokenizer.check("SPECIFIER"):
+        span_start = tokenizer.position
         parsed_specifiers += tokenizer.read().text
+        if tokenizer.check("VERSION_PREFIX_TRAIL", peek=True):
+            tokenizer.raise_syntax_error(
+                ".* suffix can only be used with `==` or `!=` operators",
+                span_start=span_start,
+                span_end=tokenizer.position + 1,
+            )
+        if tokenizer.check("VERSION_LOCAL_LABEL_TRAIL", peek=True):
+            tokenizer.raise_syntax_error(
+                "Local version label can only be used with `==` or `!=` operators",
+                span_start=span_start,
+                span_end=tokenizer.position,
+            )
         tokenizer.consume("WS")
         if not tokenizer.check("COMMA"):
             break
         parsed_specifiers += tokenizer.read().text
         tokenizer.consume("WS")
 
     return parsed_specifiers
@@ -250,15 +271,19 @@
     """
     marker_atom = WS? LEFT_PARENTHESIS WS? marker WS? RIGHT_PARENTHESIS WS?
                 | WS? marker_item WS?
     """
 
     tokenizer.consume("WS")
     if tokenizer.check("LEFT_PARENTHESIS", peek=True):
-        with tokenizer.enclosing_tokens("LEFT_PARENTHESIS", "RIGHT_PARENTHESIS"):
+        with tokenizer.enclosing_tokens(
+            "LEFT_PARENTHESIS",
+            "RIGHT_PARENTHESIS",
+            around="marker expression",
+        ):
             tokenizer.consume("WS")
             marker: MarkerAtom = _parse_marker(tokenizer)
             tokenizer.consume("WS")
     else:
         marker = _parse_marker_item(tokenizer)
     tokenizer.consume("WS")
     return marker
```

### Comparing `packaging-23.0/src/packaging/_structures.py` & `packaging-23.1/src/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `packaging-23.0/src/packaging/_tokenizer.py` & `packaging-23.1/src/packaging/_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,16 @@
     "SPECIFIER": re.compile(
         Specifier._operator_regex_str + Specifier._version_regex_str,
         re.VERBOSE | re.IGNORECASE,
     ),
     "AT": r"\@",
     "URL": r"[^ \t]+",
     "IDENTIFIER": r"\b[a-zA-Z0-9][a-zA-Z0-9._-]*\b",
+    "VERSION_PREFIX_TRAIL": r"\.\*",
+    "VERSION_LOCAL_LABEL_TRAIL": r"\+[a-z0-9]+(?:[-_\.][a-z0-9]+)*",
     "WS": r"[ \t]+",
     "END": r"$",
 }
 
 
 class Tokenizer:
     """Context-sensitive token parsing.
@@ -163,26 +165,28 @@
         raise ParserSyntaxError(
             message,
             source=self.source,
             span=span,
         )
 
     @contextlib.contextmanager
-    def enclosing_tokens(self, open_token: str, close_token: str) -> Iterator[bool]:
+    def enclosing_tokens(
+        self, open_token: str, close_token: str, *, around: str
+    ) -> Iterator[None]:
         if self.check(open_token):
             open_position = self.position
             self.read()
         else:
             open_position = None
 
-        yield open_position is not None
+        yield
 
         if open_position is None:
             return
 
         if not self.check(close_token):
             self.raise_syntax_error(
-                f"Expected closing {close_token}",
+                f"Expected matching {close_token} for {open_token}, after {around}",
                 span_start=open_position,
             )
 
         self.read()
```

### Comparing `packaging-23.0/src/packaging/markers.py` & `packaging-23.1/src/packaging/markers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 
 import operator
 import os
 import platform
 import sys
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-from ._parser import MarkerAtom, MarkerList, Op, Value, Variable, parse_marker
+from ._parser import (
+    MarkerAtom,
+    MarkerList,
+    Op,
+    Value,
+    Variable,
+    parse_marker as _parse_marker,
+)
 from ._tokenizer import ParserSyntaxError
 from .specifiers import InvalidSpecifier, Specifier
 from .utils import canonicalize_name
 
 __all__ = [
     "InvalidMarker",
     "UndefinedComparison",
@@ -185,15 +192,15 @@
 
 class Marker:
     def __init__(self, marker: str) -> None:
         # Note: We create a Marker object without calling this constructor in
         #       packaging.requirements.Requirement. If any additional logic is
         #       added here, make sure to mirror/adapt Requirement.
         try:
-            self._markers = _normalize_extra_values(parse_marker(marker))
+            self._markers = _normalize_extra_values(_parse_marker(marker))
             # The attribute `_markers` can be described in terms of a recursive type:
             # MarkerList = List[Union[Tuple[Node, ...], str, MarkerList]]
             #
             # For example, the following expression:
             # python_version > "3.6" or (python_version == "3.6" and os_name == "unix")
             #
             # is parsed into:
```

### Comparing `packaging-23.0/src/packaging/requirements.py` & `packaging-23.1/src/packaging/requirements.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
 import urllib.parse
 from typing import Any, List, Optional, Set
 
-from ._parser import parse_requirement
+from ._parser import parse_requirement as _parse_requirement
 from ._tokenizer import ParserSyntaxError
 from .markers import Marker, _normalize_extra_values
 from .specifiers import SpecifierSet
 
 
 class InvalidRequirement(ValueError):
     """
@@ -28,15 +28,15 @@
     # TODO: Can we test whether something is contained within a requirement?
     #       If so how do we do that? Do we need to test against the _name_ of
     #       the thing as well as the version? What about the markers?
     # TODO: Can we normalize the name and extra name?
 
     def __init__(self, requirement_string: str) -> None:
         try:
-            parsed = parse_requirement(requirement_string)
+            parsed = _parse_requirement(requirement_string)
         except ParserSyntaxError as e:
             raise InvalidRequirement(str(e)) from e
 
         self.name: str = parsed.name
         if parsed.url:
             parsed_url = urllib.parse.urlparse(parsed.url)
             if parsed_url.scheme == "file":
```

### Comparing `packaging-23.0/src/packaging/specifiers.py` & `packaging-23.1/src/packaging/specifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,16 @@
             match.group("operator").strip(),
             match.group("version").strip(),
         )
 
         # Store whether or not this Specifier should accept prereleases
         self._prereleases = prereleases
 
-    @property
+    # https://github.com/python/mypy/pull/13475#pullrequestreview-1079784515
+    @property  # type: ignore[override]
     def prereleases(self) -> bool:
         # If there is an explicit prereleases set for this, then we'll just
         # blindly use that.
         if self._prereleases is not None:
             return self._prereleases
 
         # Look at all of our specifiers and determine if they are inclusive
@@ -394,15 +395,17 @@
         )
 
     def _compare_equal(self, prospective: Version, spec: str) -> bool:
 
         # We need special logic to handle prefix matching
         if spec.endswith(".*"):
             # In the case of prefix matching we want to ignore local segment.
-            normalized_prospective = canonicalize_version(prospective.public)
+            normalized_prospective = canonicalize_version(
+                prospective.public, strip_trailing_zero=False
+            )
             # Get the normalized version string ignoring the trailing .*
             normalized_spec = canonicalize_version(spec[:-2], strip_trailing_zero=False)
             # Split the spec out by dots, and pretend that there is an implicit
             # dot in between a release segment and a pre-release segment.
             split_spec = _version_split(normalized_spec)
 
             # Split the prospective version out by dots, and pretend that there
```

### Comparing `packaging-23.0/src/packaging/tags.py` & `packaging-23.1/src/packaging/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,24 +107,24 @@
         for abi in abis.split("."):
             for platform_ in platforms.split("."):
                 tags.add(Tag(interpreter, abi, platform_))
     return frozenset(tags)
 
 
 def _get_config_var(name: str, warn: bool = False) -> Union[int, str, None]:
-    value = sysconfig.get_config_var(name)
+    value: Union[int, str, None] = sysconfig.get_config_var(name)
     if value is None and warn:
         logger.debug(
             "Config variable '%s' is unset, Python ABI tag may be incorrect", name
         )
     return value
 
 
 def _normalize_string(string: str) -> str:
-    return string.replace(".", "_").replace("-", "_")
+    return string.replace(".", "_").replace("-", "_").replace(" ", "_")
 
 
 def _abi3_applies(python_version: PythonVersion) -> bool:
     """
     Determine if the Python version supports abi3.
 
     PEP 384 was first implemented in Python 3.2.
```

### Comparing `packaging-23.0/src/packaging/utils.py` & `packaging-23.1/src/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `packaging-23.0/src/packaging/version.py` & `packaging-23.1/src/packaging/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
     from packaging.version import parse, Version
 """
 
 import collections
 import itertools
 import re
-from typing import Callable, Optional, SupportsInt, Tuple, Union
+from typing import Any, Callable, Optional, SupportsInt, Tuple, Union
 
 from ._structures import Infinity, InfinityType, NegativeInfinity, NegativeInfinityType
 
 __all__ = ["VERSION_PATTERN", "parse", "Version", "InvalidVersion"]
 
 InfiniteTypes = Union[InfinityType, NegativeInfinityType]
 PrePostDevType = Union[InfiniteTypes, Tuple[str, int]]
@@ -59,15 +59,15 @@
     Traceback (most recent call last):
         ...
     packaging.version.InvalidVersion: Invalid version: 'invalid'
     """
 
 
 class _BaseVersion:
-    _key: CmpKey
+    _key: Tuple[Any, ...]
 
     def __hash__(self) -> int:
         return hash(self._key)
 
     # Please keep the duplicated `isinstance` check
     # in the six comparisons hereunder
     # unless you find a way to avoid adding overhead function calls.
@@ -175,14 +175,15 @@
     >>> v1 >= v2
     False
     >>> v1 <= v2
     True
     """
 
     _regex = re.compile(r"^\s*" + VERSION_PATTERN + r"\s*$", re.VERBOSE | re.IGNORECASE)
+    _key: CmpKey
 
     def __init__(self, version: str) -> None:
         """Initialize a Version object.
 
         :param version:
             The string representation of a version which will be parsed and normalized
             before use.
```

### Comparing `packaging-23.0/tests/.pytest_cache/v/cache/lastfailed` & `packaging-23.1/tests/.pytest_cache/v/cache/lastfailed`

 * *Files identical despite different names*

### Comparing `packaging-23.0/tests/.pytest_cache/v/cache/nodeids` & `packaging-23.1/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `packaging-23.0/tests/manylinux/build.sh` & `packaging-23.1/tests/manylinux/build.sh`

 * *Files identical despite different names*

### Comparing `packaging-23.0/tests/musllinux/glibc-x86_64` & `packaging-23.1/tests/musllinux/glibc-x86_64`

 * *Files identical despite different names*

### Comparing `packaging-23.0/tests/musllinux/musl-aarch64` & `packaging-23.1/tests/musllinux/musl-aarch64`

 * *Files identical despite different names*

### Comparing `packaging-23.0/tests/musllinux/musl-i386` & `packaging-23.1/tests/musllinux/musl-i386`

 * *Files identical despite different names*

### Comparing `packaging-23.0/tests/musllinux/musl-x86_64` & `packaging-23.1/tests/musllinux/musl-x86_64`

 * *Files identical despite different names*

### Comparing `packaging-23.0/tests/test_elffile.py` & `packaging-23.1/tests/test_elffile.py`

 * *Files identical despite different names*

### Comparing `packaging-23.0/tests/test_manylinux.py` & `packaging-23.1/tests/test_manylinux.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 try:
     import ctypes
 except ImportError:
     ctypes = None
 import os
+import pathlib
 import platform
 import sys
 import types
 import warnings
 
 import pretend
 import pytest
@@ -165,16 +166,13 @@
 
 
 @pytest.mark.parametrize(
     "content", [None, "invalid-magic", "invalid-class", "invalid-data", "too-short"]
 )
 def test_parse_elf_bad_executable(monkeypatch, content):
     if content:
-        path = os.path.join(
-            os.path.dirname(__file__),
-            "manylinux",
-            f"hello-world-{content}",
-        )
+        path = pathlib.Path(__file__).parent / "manylinux" / f"hello-world-{content}"
+        path = os.fsdecode(path)
     else:
         path = None
     with _parse_elf(path) as ef:
         assert ef is None
```

### Comparing `packaging-23.0/tests/test_markers.py` & `packaging-23.1/tests/test_markers.py`

 * *Files identical despite different names*

### Comparing `packaging-23.0/tests/test_musllinux.py` & `packaging-23.1/tests/test_musllinux.py`

 * *Files identical despite different names*

### Comparing `packaging-23.0/tests/test_requirements.py` & `packaging-23.1/tests/test_requirements.py`

 * *Files 6% similar despite different names*

```diff
@@ -275,31 +275,69 @@
         # WHEN
         with pytest.raises(InvalidRequirement) as ctx:
             Requirement(to_parse)
 
         # THEN
         assert ctx.exconly() == (
             "packaging.requirements.InvalidRequirement: "
-            "Expected closing RIGHT_PARENTHESIS\n"
+            "Expected matching RIGHT_PARENTHESIS for LEFT_PARENTHESIS, "
+            "after version specifier\n"
             "    name (>= 1.0\n"
             "         ~~~~~~~^"
         )
 
+    def test_error_when_prefix_match_is_used_incorrectly(self) -> None:
+        # GIVEN
+        to_parse = "black (>=20.*) ; extra == 'format'"
+
+        # WHEN
+        with pytest.raises(InvalidRequirement) as ctx:
+            Requirement(to_parse)
+
+        # THEN
+        assert ctx.exconly() == (
+            "packaging.requirements.InvalidRequirement: "
+            ".* suffix can only be used with `==` or `!=` operators\n"
+            "    black (>=20.*) ; extra == 'format'\n"
+            "           ~~~~~^"
+        )
+
+    @pytest.mark.parametrize("operator", [">=", "<=", ">", "<", "~="])
+    def test_error_when_local_version_label_is_used_incorrectly(
+        self, operator: str
+    ) -> None:
+        # GIVEN
+        to_parse = f"name {operator} 1.0+local.version.label"
+        op_tilde = len(operator) * "~"
+
+        # WHEN
+        with pytest.raises(InvalidRequirement) as ctx:
+            Requirement(to_parse)
+
+        # THEN
+        assert ctx.exconly() == (
+            "packaging.requirements.InvalidRequirement: "
+            "Local version label can only be used with `==` or `!=` operators\n"
+            f"    name {operator} 1.0+local.version.label\n"
+            f"         {op_tilde}~~~~^"
+        )
+
     def test_error_when_bracket_not_closed_correctly(self) -> None:
         # GIVEN
         to_parse = "name[bar, baz >= 1.0"
 
         # WHEN
         with pytest.raises(InvalidRequirement) as ctx:
             Requirement(to_parse)
 
         # THEN
         assert ctx.exconly() == (
             "packaging.requirements.InvalidRequirement: "
-            "Expected closing RIGHT_BRACKET\n"
+            "Expected matching RIGHT_BRACKET for LEFT_BRACKET, "
+            "after extras\n"
             "    name[bar, baz >= 1.0\n"
             "        ~~~~~~~~~~^"
         )
 
     def test_error_when_extras_bracket_left_unclosed(self) -> None:
         # GIVEN
         to_parse = "name[bar, baz"
@@ -307,15 +345,16 @@
         # WHEN
         with pytest.raises(InvalidRequirement) as ctx:
             Requirement(to_parse)
 
         # THEN
         assert ctx.exconly() == (
             "packaging.requirements.InvalidRequirement: "
-            "Expected closing RIGHT_BRACKET\n"
+            "Expected matching RIGHT_BRACKET for LEFT_BRACKET, "
+            "after extras\n"
             "    name[bar, baz\n"
             "        ~~~~~~~~~^"
         )
 
     def test_error_no_space_after_url(self) -> None:
         # GIVEN
         to_parse = "name @ https://example.com/; extra == 'example'"
@@ -328,14 +367,31 @@
         assert ctx.exconly() == (
             "packaging.requirements.InvalidRequirement: "
             "Expected end or semicolon (after URL and whitespace)\n"
             "    name @ https://example.com/; extra == 'example'\n"
             "           ~~~~~~~~~~~~~~~~~~~~~~^"
         )
 
+    def test_error_marker_bracket_unclosed(self) -> None:
+        # GIVEN
+        to_parse = "name; (extra == 'example'"
+
+        # WHEN
+        with pytest.raises(InvalidRequirement) as ctx:
+            Requirement(to_parse)
+
+        # THEN
+        assert ctx.exconly() == (
+            "packaging.requirements.InvalidRequirement: "
+            "Expected matching RIGHT_PARENTHESIS for LEFT_PARENTHESIS, "
+            "after marker expression\n"
+            "    name; (extra == 'example'\n"
+            "          ~~~~~~~~~~~~~~~~~~~^"
+        )
+
     def test_error_no_url_after_at(self) -> None:
         # GIVEN
         to_parse = "name @ "
 
         # WHEN
         with pytest.raises(InvalidRequirement) as ctx:
             Requirement(to_parse)
```

### Comparing `packaging-23.0/tests/test_specifiers.py` & `packaging-23.1/tests/test_specifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,14 +365,16 @@
                 ("1.1", "~=1.0a1"),
                 ("2022.01.01", "~=2022.01.01"),
                 # Test that epochs are handled sanely
                 ("2!1.0", "~=2!1.0"),
                 ("2!1.0", "==2!1.*"),
                 ("2!1.0", "==2!1.0"),
                 ("2!1.0", "!=1.0"),
+                ("2!1.0.0", "==2!1.0.*"),
+                ("2!1.0.0", "==2!1.*"),
                 ("1.0", "!=2!1.0"),
                 ("1.0", "<=2!0.1"),
                 ("2!1.0", ">=2.0"),
                 ("1.0", "<2!0.1"),
                 ("2!1.0", ">2.0"),
                 # Test some normalization rules
                 ("2.0.5", ">2.0dev"),
```

### Comparing `packaging-23.0/tests/test_structures.py` & `packaging-23.1/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `packaging-23.0/tests/test_tags.py` & `packaging-23.1/tests/test_tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -230,33 +230,30 @@
             )
         version = platform.mac_ver()[0].split(".")
         major = version[0]
         minor = version[1] if major == "10" else "0"
 
         platforms = list(tags.mac_platforms(arch="x86_64"))
         if (major, minor) == ("10", "16"):
-            print(platforms, "macosx_11+")
             # For 10.16, the real version is at least 11.0.
             prefix, major, minor, _ = platforms[0].split("_", maxsplit=3)
             assert prefix == "macosx"
             assert int(major) >= 11
             assert minor == "0"
         else:
             expected = f"macosx_{major}_{minor}_"
-            print(platforms, expected)
             assert platforms[0].startswith(expected)
 
     def test_version_detection_10_15(self, monkeypatch):
         monkeypatch.setattr(
             platform, "mac_ver", lambda: ("10.15", ("", "", ""), "x86_64")
         )
         expected = "macosx_10_15_"
 
         platforms = list(tags.mac_platforms(arch="x86_64"))
-        print(platforms, expected)
         assert platforms[0].startswith(expected)
 
     def test_version_detection_compatibility(self, monkeypatch):
         if platform.system() != "Darwin":
             monkeypatch.setattr(
                 subprocess,
                 "run",
@@ -266,15 +263,14 @@
             )
         monkeypatch.setattr(
             platform, "mac_ver", lambda: ("10.16", ("", "", ""), "x86_64")
         )
         unexpected = "macosx_10_16_"
 
         platforms = list(tags.mac_platforms(arch="x86_64"))
-        print(platforms, unexpected)
         assert not platforms[0].startswith(unexpected)
 
     @pytest.mark.parametrize("arch", ["x86_64", "i386"])
     def test_arch_detection(self, arch, monkeypatch):
         if platform.system() != "Darwin" or platform.mac_ver()[2] != arch:
             monkeypatch.setattr(
                 platform, "mac_ver", lambda: ("10.14", ("", "", ""), arch)
@@ -599,14 +595,21 @@
 def test_platform_tags(platform_name, dispatch_func, monkeypatch):
     expected = ["sillywalk"]
     monkeypatch.setattr(platform, "system", lambda: platform_name)
     monkeypatch.setattr(tags, dispatch_func, lambda: expected)
     assert tags.platform_tags() == expected
 
 
+def test_platform_tags_space(monkeypatch):
+    """Ensure spaces in platform tags are normalized to underscores."""
+    monkeypatch.setattr(platform, "system", lambda: "Isilon OneFS")
+    monkeypatch.setattr(sysconfig, "get_platform", lambda: "isilon onefs")
+    assert list(tags.platform_tags()) == ["isilon_onefs"]
+
+
 class TestCPythonABI:
     @pytest.mark.parametrize(
         "py_debug,gettotalrefcount,result",
         [(1, False, True), (0, False, False), (None, True, True)],
     )
     def test_debug(self, py_debug, gettotalrefcount, result, monkeypatch):
         config = {"Py_DEBUG": py_debug, "WITH_PYMALLOC": 0, "Py_UNICODE_SIZE": 2}
@@ -770,14 +773,20 @@
         assert tags.Tag("cp38", "whatever", "plat1") in result
 
     def test_platforms_defaults_needs_underscore(self, monkeypatch):
         monkeypatch.setattr(tags, "platform_tags", lambda: ["plat1"])
         result = list(tags.cpython_tags((3, 11), abis=["whatever"]))
         assert tags.Tag("cp311", "whatever", "plat1") in result
 
+    def test_platform_name_space_normalization(self, monkeypatch):
+        """Ensure that spaces are translated to underscores in platform names."""
+        monkeypatch.setattr(sysconfig, "get_platform", lambda: "isilon onefs")
+        for tag in tags.cpython_tags():
+            assert " " not in tag.platform
+
     def test_major_only_python_version(self):
         result = list(tags.cpython_tags((3,), ["abi"], ["plat"]))
         assert result == [
             tags.Tag("cp3", "abi", "plat"),
             tags.Tag("cp3", "none", "plat"),
         ]
 
@@ -839,17 +848,17 @@
         monkeypatch.setattr(sysconfig, "get_config_var", config.__getitem__)
         monkeypatch.setattr(tags, "interpreter_name", lambda: "cp")
         # They are identical
         assert tags._cpython_abis((3, 7)) == ["cp37m"]
         assert tags._generic_abi() == ["cp37m"]
 
     def test__generic_abi_jp(self, monkeypatch):
-        config = {"EXT_SUFFIX": ".return exactly this.so"}
+        config = {"EXT_SUFFIX": ".return_exactly_this.so"}
         monkeypatch.setattr(sysconfig, "get_config_var", config.__getitem__)
-        assert tags._generic_abi() == ["return exactly this"]
+        assert tags._generic_abi() == ["return_exactly_this"]
 
     def test__generic_abi_graal(self, monkeypatch):
         config = {"EXT_SUFFIX": ".graalpy-38-native-x86_64-darwin.so"}
         monkeypatch.setattr(sysconfig, "get_config_var", config.__getitem__)
         assert tags._generic_abi() == ["graalpy_38_native"]
 
     def test__generic_abi_none(self, monkeypatch):
@@ -897,14 +906,20 @@
         assert tags._generic_abi() == tags._cpython_abis(sys.version_info[:2])
 
     def test_generic_platforms(self):
         platform = sysconfig.get_platform().replace("-", "_")
         platform = platform.replace(".", "_")
         assert list(tags._generic_platforms()) == [platform]
 
+    def test_generic_platforms_space(self, monkeypatch):
+        """Ensure platform tags normalize spaces to underscores."""
+        platform_ = "isilon onefs"
+        monkeypatch.setattr(sysconfig, "get_platform", lambda: platform_)
+        assert list(tags._generic_platforms()) == [platform_.replace(" ", "_")]
+
     def test_iterator_returned(self):
         result_iterator = tags.generic_tags("sillywalk33", ["abi"], ["plat1", "plat2"])
         assert isinstance(result_iterator, collections.abc.Iterator)
 
     def test_all_args(self):
         result_iterator = tags.generic_tags("sillywalk33", ["abi"], ["plat1", "plat2"])
         result = list(result_iterator)
```

### Comparing `packaging-23.0/tests/test_utils.py` & `packaging-23.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `packaging-23.0/tests/test_version.py` & `packaging-23.1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `packaging-23.0/PKG-INFO` & `packaging-23.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging
-Version: 23.0
+Version: 23.1
 Summary: Core utilities for Python packages
 Author-email: Donald Stufft <donald@stufft.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Typing :: Typed
 Project-URL: Documentation, https://packaging.pypa.io/
 Project-URL: Source, https://github.com/pypa/packaging
 
 packaging
 =========
 
 .. start-intro
```

