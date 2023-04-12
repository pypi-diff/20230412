# Comparing `tmp/volkanic-0.5.0.tar.gz` & `tmp/volkanic-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volkanic-0.5.0.tar", last modified: Fri Apr  7 02:23:13 2023, max compression
+gzip compressed data, was "volkanic-0.5.1.tar", last modified: Wed Apr 12 09:14:23 2023, max compression
```

## Comparing `volkanic-0.5.0.tar` & `volkanic-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-07 02:23:13.080869 volkanic-0.5.0/
--rw-r--r--   0 Hailong    (502) staff       (20)    35149 2019-04-25 10:44:00.000000 volkanic-0.5.0/LICENSE
--rw-r--r--   0 Hailong    (502) staff       (20)       25 2019-01-21 17:03:54.000000 volkanic-0.5.0/MANIFEST.in
--rw-r--r--   0 Hailong    (502) staff       (20)     4714 2023-04-07 02:23:13.080538 volkanic-0.5.0/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)     3987 2021-09-05 13:58:09.000000 volkanic-0.5.0/README.md
--rw-r--r--   0 Hailong    (502) staff       (20)       12 2022-02-03 05:01:45.000000 volkanic-0.5.0/requirements.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       38 2023-04-07 02:23:13.080978 volkanic-0.5.0/setup.cfg
--rw-r--r--   0 Hailong    (502) staff       (20)     2093 2022-05-12 11:43:32.000000 volkanic-0.5.0/setup.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-07 02:23:13.077693 volkanic-0.5.0/volkanic/
--rw-r--r--   0 Hailong    (502) staff       (20)      203 2023-04-07 02:22:23.000000 volkanic-0.5.0/volkanic/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)      896 2022-01-21 13:22:00.000000 volkanic-0.5.0/volkanic/__main__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     4278 2022-04-18 13:34:09.000000 volkanic-0.5.0/volkanic/cmdline.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1085 2022-04-18 13:34:57.000000 volkanic-0.5.0/volkanic/compat.py
--rw-r--r--   0 Hailong    (502) staff       (20)     8403 2023-04-07 02:22:23.000000 volkanic-0.5.0/volkanic/environ.py
--rw-r--r--   0 Hailong    (502) staff       (20)      474 2023-04-07 02:22:23.000000 volkanic-0.5.0/volkanic/errors.py
--rw-r--r--   0 Hailong    (502) staff       (20)     8787 2023-04-07 02:22:23.000000 volkanic-0.5.0/volkanic/introspect.py
--rw-r--r--   0 Hailong    (502) staff       (20)     6229 2023-04-07 02:22:23.000000 volkanic-0.5.0/volkanic/utils.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-07 02:23:13.080064 volkanic-0.5.0/volkanic.egg-info/
--rw-r--r--   0 Hailong    (502) staff       (20)     4714 2023-04-07 02:23:13.000000 volkanic-0.5.0/volkanic.egg-info/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      441 2023-04-07 02:23:13.000000 volkanic-0.5.0/volkanic.egg-info/SOURCES.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2023-04-07 02:23:13.000000 volkanic-0.5.0/volkanic.egg-info/dependency_links.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       52 2023-04-07 02:23:13.000000 volkanic-0.5.0/volkanic.egg-info/entry_points.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2021-08-14 03:53:40.000000 volkanic-0.5.0/volkanic.egg-info/not-zip-safe
--rw-r--r--   0 Hailong    (502) staff       (20)       13 2023-04-07 02:23:13.000000 volkanic-0.5.0/volkanic.egg-info/requires.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        9 2023-04-07 02:23:13.000000 volkanic-0.5.0/volkanic.egg-info/top_level.txt
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-12 09:14:23.243231 volkanic-0.5.1/
+-rw-r--r--   0 Hailong    (502) staff       (20)    35149 2019-04-25 10:44:00.000000 volkanic-0.5.1/LICENSE
+-rw-r--r--   0 Hailong    (502) staff       (20)       25 2019-01-21 17:03:54.000000 volkanic-0.5.1/MANIFEST.in
+-rw-r--r--   0 Hailong    (502) staff       (20)     4714 2023-04-12 09:14:23.242869 volkanic-0.5.1/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)     3987 2021-09-05 13:58:09.000000 volkanic-0.5.1/README.md
+-rw-r--r--   0 Hailong    (502) staff       (20)       12 2022-02-03 05:01:45.000000 volkanic-0.5.1/requirements.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       38 2023-04-12 09:14:23.243389 volkanic-0.5.1/setup.cfg
+-rw-r--r--   0 Hailong    (502) staff       (20)     2093 2022-05-12 11:43:32.000000 volkanic-0.5.1/setup.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-12 09:14:23.238583 volkanic-0.5.1/volkanic/
+-rw-r--r--   0 Hailong    (502) staff       (20)      203 2023-04-12 09:14:04.000000 volkanic-0.5.1/volkanic/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      896 2022-01-21 13:22:00.000000 volkanic-0.5.1/volkanic/__main__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     4278 2022-04-18 13:34:09.000000 volkanic-0.5.1/volkanic/cmdline.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1085 2022-04-18 13:34:57.000000 volkanic-0.5.1/volkanic/compat.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     8403 2023-04-07 02:22:23.000000 volkanic-0.5.1/volkanic/environ.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      614 2023-04-12 09:14:04.000000 volkanic-0.5.1/volkanic/errors.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     8787 2023-04-07 02:22:23.000000 volkanic-0.5.1/volkanic/introspect.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     6229 2023-04-07 02:22:23.000000 volkanic-0.5.1/volkanic/utils.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-12 09:14:23.242338 volkanic-0.5.1/volkanic.egg-info/
+-rw-r--r--   0 Hailong    (502) staff       (20)     4714 2023-04-12 09:14:23.000000 volkanic-0.5.1/volkanic.egg-info/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      441 2023-04-12 09:14:23.000000 volkanic-0.5.1/volkanic.egg-info/SOURCES.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2023-04-12 09:14:23.000000 volkanic-0.5.1/volkanic.egg-info/dependency_links.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       52 2023-04-12 09:14:23.000000 volkanic-0.5.1/volkanic.egg-info/entry_points.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2021-08-14 03:53:40.000000 volkanic-0.5.1/volkanic.egg-info/not-zip-safe
+-rw-r--r--   0 Hailong    (502) staff       (20)       13 2023-04-12 09:14:23.000000 volkanic-0.5.1/volkanic.egg-info/requires.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        9 2023-04-12 09:14:23.000000 volkanic-0.5.1/volkanic.egg-info/top_level.txt
```

### Comparing `volkanic-0.5.0/LICENSE` & `volkanic-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.0/PKG-INFO` & `volkanic-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volkanic
-Version: 0.5.0
+Version: 0.5.1
 Summary: access config and CLI easily and elegantly
 Home-page: https://github.com/frozflame/volkanic
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `volkanic-0.5.0/README.md` & `volkanic-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.0/setup.py` & `volkanic-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.0/volkanic/__main__.py` & `volkanic-0.5.1/volkanic/__main__.py`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.0/volkanic/cmdline.py` & `volkanic-0.5.1/volkanic/cmdline.py`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.0/volkanic/compat.py` & `volkanic-0.5.1/volkanic/compat.py`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.0/volkanic/environ.py` & `volkanic-0.5.1/volkanic/environ.py`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.0/volkanic/introspect.py` & `volkanic-0.5.1/volkanic/introspect.py`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.0/volkanic/utils.py` & `volkanic-0.5.1/volkanic/utils.py`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.0/volkanic.egg-info/PKG-INFO` & `volkanic-0.5.1/volkanic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volkanic
-Version: 0.5.0
+Version: 0.5.1
 Summary: access config and CLI easily and elegantly
 Home-page: https://github.com/frozflame/volkanic
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

