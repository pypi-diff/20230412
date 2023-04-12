# Comparing `tmp/rawfinder-0.1.3.tar.gz` & `tmp/rawfinder-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rawfinder-0.1.3.tar", max compression
+gzip compressed data, was "rawfinder-0.1.4.tar", max compression
```

## Comparing `rawfinder-0.1.3.tar` & `rawfinder-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      886 2023-01-23 14:52:45.821580 rawfinder-0.1.3/README.md
--rw-r--r--   0        0        0      581 2023-01-23 15:01:48.611772 rawfinder-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-23 14:12:24.382959 rawfinder-0.1.3/rawfinder/__init__.py
--rw-r--r--   0        0        0     2545 2023-01-23 15:01:58.809027 rawfinder-0.1.3/rawfinder/core.py
--rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 rawfinder-0.1.3/setup.py
--rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 rawfinder-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      886 2023-01-23 14:52:45.821580 rawfinder-0.1.4/README.md
+-rw-r--r--   0        0        0      581 2023-04-12 20:25:06.921138 rawfinder-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-23 14:12:24.382959 rawfinder-0.1.4/rawfinder/__init__.py
+-rw-r--r--   0        0        0     3066 2023-04-12 20:22:30.958978 rawfinder-0.1.4/rawfinder/core.py
+-rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 rawfinder-0.1.4/PKG-INFO
```

### Comparing `rawfinder-0.1.3/README.md` & `rawfinder-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rawfinder-0.1.3/pyproject.toml` & `rawfinder-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rawfinder"
-version = "0.1.3"
+version = "0.1.4"
 description = "Raw Finder"
 authors = ["Vitalii Shishorin <moskrc@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/moskrc/rawfinder"
 keywords = ["raw", "finder", "raw_finder", "jpeg_raw"]
 
 [tool.poetry.dependencies]
```

### Comparing `rawfinder-0.1.3/PKG-INFO` & `rawfinder-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rawfinder
-Version: 0.1.3
+Version: 0.1.4
 Summary: Raw Finder
 Home-page: https://github.com/moskrc/rawfinder
 Keywords: raw,finder,raw_finder,jpeg_raw
 Author: Vitalii Shishorin
 Author-email: moskrc@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

