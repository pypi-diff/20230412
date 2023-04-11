# Comparing `tmp/nbtester-0.6.0.tar.gz` & `tmp/nbtester-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbtester-0.6.0.tar", last modified: Wed Nov 30 23:42:03 2022, max compression
+gzip compressed data, was "nbtester-0.7.0.tar", last modified: Tue Apr 11 23:36:45 2023, max compression
```

## Comparing `nbtester-0.6.0.tar` & `nbtester-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tsutomu    (502) staff       (20)        0 2022-11-30 23:42:03.765911 nbtester-0.6.0/
--rw-r--r--   0 tsutomu    (502) staff       (20)     1109 2020-09-03 00:12:16.000000 nbtester-0.6.0/LICENSE
--rw-r--r--   0 tsutomu    (502) staff       (20)      854 2022-11-30 23:42:03.765657 nbtester-0.6.0/PKG-INFO
--rw-r--r--   0 tsutomu    (502) staff       (20)      672 2020-09-03 00:12:16.000000 nbtester-0.6.0/README.rst
-drwxr-xr-x   0 tsutomu    (502) staff       (20)        0 2022-11-30 23:42:03.763955 nbtester-0.6.0/nbtester/
--rw-r--r--   0 tsutomu    (502) staff       (20)       56 2020-09-03 00:12:16.000000 nbtester-0.6.0/nbtester/__init__.py
--rw-r--r--   0 tsutomu    (502) staff       (20)     6534 2022-11-30 23:40:13.000000 nbtester-0.6.0/nbtester/loader.py
-drwxr-xr-x   0 tsutomu    (502) staff       (20)        0 2022-11-30 23:42:03.765315 nbtester-0.6.0/nbtester.egg-info/
--rw-r--r--   0 tsutomu    (502) staff       (20)      854 2022-11-30 23:42:03.000000 nbtester-0.6.0/nbtester.egg-info/PKG-INFO
--rw-r--r--   0 tsutomu    (502) staff       (20)      226 2022-11-30 23:42:03.000000 nbtester-0.6.0/nbtester.egg-info/SOURCES.txt
--rw-r--r--   0 tsutomu    (502) staff       (20)        1 2022-11-30 23:42:03.000000 nbtester-0.6.0/nbtester.egg-info/dependency_links.txt
--rw-r--r--   0 tsutomu    (502) staff       (20)        9 2022-11-30 23:42:03.000000 nbtester-0.6.0/nbtester.egg-info/requires.txt
--rw-r--r--   0 tsutomu    (502) staff       (20)        9 2022-11-30 23:42:03.000000 nbtester-0.6.0/nbtester.egg-info/top_level.txt
--rw-r--r--   0 tsutomu    (502) staff       (20)       38 2022-11-30 23:42:03.765996 nbtester-0.6.0/setup.cfg
--rw-r--r--   0 tsutomu    (502) staff       (20)      418 2022-11-30 23:40:13.000000 nbtester-0.6.0/setup.py
+drwxr-xr-x   0 tsutomu    (502) staff       (20)        0 2023-04-11 23:36:45.827642 nbtester-0.7.0/
+-rw-r--r--   0 tsutomu    (502) staff       (20)     1109 2020-09-03 00:12:16.000000 nbtester-0.7.0/LICENSE
+-rw-r--r--   0 tsutomu    (502) staff       (20)      854 2023-04-11 23:36:45.827384 nbtester-0.7.0/PKG-INFO
+-rw-r--r--   0 tsutomu    (502) staff       (20)      672 2020-09-03 00:12:16.000000 nbtester-0.7.0/README.rst
+drwxr-xr-x   0 tsutomu    (502) staff       (20)        0 2023-04-11 23:36:45.825508 nbtester-0.7.0/nbtester/
+-rw-r--r--   0 tsutomu    (502) staff       (20)       56 2020-09-03 00:12:16.000000 nbtester-0.7.0/nbtester/__init__.py
+-rw-r--r--   0 tsutomu    (502) staff       (20)     6498 2023-04-08 00:01:52.000000 nbtester-0.7.0/nbtester/loader.py
+drwxr-xr-x   0 tsutomu    (502) staff       (20)        0 2023-04-11 23:36:45.827022 nbtester-0.7.0/nbtester.egg-info/
+-rw-r--r--   0 tsutomu    (502) staff       (20)      854 2023-04-11 23:36:45.000000 nbtester-0.7.0/nbtester.egg-info/PKG-INFO
+-rw-r--r--   0 tsutomu    (502) staff       (20)      226 2023-04-11 23:36:45.000000 nbtester-0.7.0/nbtester.egg-info/SOURCES.txt
+-rw-r--r--   0 tsutomu    (502) staff       (20)        1 2023-04-11 23:36:45.000000 nbtester-0.7.0/nbtester.egg-info/dependency_links.txt
+-rw-r--r--   0 tsutomu    (502) staff       (20)        9 2023-04-11 23:36:45.000000 nbtester-0.7.0/nbtester.egg-info/requires.txt
+-rw-r--r--   0 tsutomu    (502) staff       (20)        9 2023-04-11 23:36:45.000000 nbtester-0.7.0/nbtester.egg-info/top_level.txt
+-rw-r--r--   0 tsutomu    (502) staff       (20)       38 2023-04-11 23:36:45.827723 nbtester-0.7.0/setup.cfg
+-rw-r--r--   0 tsutomu    (502) staff       (20)      418 2023-04-08 00:02:43.000000 nbtester-0.7.0/setup.py
```

### Comparing `nbtester-0.6.0/LICENSE` & `nbtester-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbtester-0.6.0/PKG-INFO` & `nbtester-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbtester
-Version: 0.6.0
+Version: 0.7.0
 Summary: Test utilities for Jupyter Notebook file
 Author: Hiroki KIYOHARA
 Author-email: hirokiky@gmail.com
 License-File: LICENSE
 
 ========
 nbtester
```

### Comparing `nbtester-0.6.0/README.rst` & `nbtester-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `nbtester-0.6.0/nbtester/loader.py` & `nbtester-0.7.0/nbtester/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,17 +174,16 @@
     return re.sub(f"({p})", lambda m: conv_dict[m.group(0)], s)  # noqa
 
 
 def matplotlib_test(ipynb, expected=None, conv_dict=None):
     if MyMagicMock.in_matplotlib_test:
         return False
     MyMagicMock.mocks = []
-    with mock.patch("matplotlib.pyplot", name="plt") as p, mock.patch(
-        "matplotlib.pyplot.subplots", _subplots
-    ):
+    with mock.patch("matplotlib.pyplot", name="plt") as p:
+        p.subplots = _subplots
         MyMagicMock.mocks.append(p)
         try:
             MyMagicMock.in_matplotlib_test = True
             d = {}
             if ipynb.endswith(".ipynb"):
                 load_cells(d, ipynb)
             else:
```

### Comparing `nbtester-0.6.0/nbtester.egg-info/PKG-INFO` & `nbtester-0.7.0/nbtester.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbtester
-Version: 0.6.0
+Version: 0.7.0
 Summary: Test utilities for Jupyter Notebook file
 Author: Hiroki KIYOHARA
 Author-email: hirokiky@gmail.com
 License-File: LICENSE
 
 ========
 nbtester
```

