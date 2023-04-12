# Comparing `tmp/zoinks-0.0.6.tar.gz` & `tmp/zoinks-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoinks-0.0.6.tar", last modified: Sun Apr  9 18:03:05 2023, max compression
+gzip compressed data, was "zoinks-0.0.7.tar", last modified: Wed Apr 12 19:19:44 2023, max compression
```

## Comparing `zoinks-0.0.6.tar` & `zoinks-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-09 18:03:05.841721 zoinks-0.0.6/
--rw-r--r--   0 mhucka     (503) staff       (20)     1622 2023-04-09 17:58:40.000000 zoinks-0.0.6/LICENSE
--rw-r--r--   0 mhucka     (503) staff       (20)     4241 2023-04-09 18:03:05.841784 zoinks-0.0.6/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)     3429 2023-04-09 17:59:09.000000 zoinks-0.0.6/README.md
--rw-r--r--   0 mhucka     (503) staff       (20)      957 2023-04-09 18:03:05.842151 zoinks-0.0.6/setup.cfg
--rw-r--r--   0 mhucka     (503) staff       (20)      885 2022-01-03 15:12:35.000000 zoinks-0.0.6/setup.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-09 18:03:05.840563 zoinks-0.0.6/zoinks/
--rw-r--r--   0 mhucka     (503) staff       (20)     1493 2023-04-09 18:01:32.000000 zoinks-0.0.6/zoinks/__init__.py
--rw-r--r--   0 mhucka     (503) staff       (20)    15045 2022-11-13 17:22:14.000000 zoinks-0.0.6/zoinks/__main__.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1013 2022-01-03 16:10:18.000000 zoinks-0.0.6/zoinks/exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1394 2022-01-03 15:22:00.000000 zoinks-0.0.6/zoinks/exit_codes.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-09 18:03:05.841610 zoinks-0.0.6/zoinks.egg-info/
--rw-r--r--   0 mhucka     (503) staff       (20)     4241 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)      327 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (503) staff       (20)       64 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (503) staff       (20)      129 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/requires.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        7 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/top_level.txt
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-12 19:19:44.635333 zoinks-0.0.7/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1622 2023-04-09 17:58:40.000000 zoinks-0.0.7/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)     4241 2023-04-12 19:19:44.635404 zoinks-0.0.7/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)     3429 2023-04-09 17:59:09.000000 zoinks-0.0.7/README.md
+-rw-r--r--   0 mhucka     (503) staff       (20)      957 2023-04-12 19:19:44.635639 zoinks-0.0.7/setup.cfg
+-rw-r--r--   0 mhucka     (503) staff       (20)      885 2022-01-03 15:12:35.000000 zoinks-0.0.7/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-12 19:19:44.634254 zoinks-0.0.7/zoinks/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1493 2023-04-12 19:18:13.000000 zoinks-0.0.7/zoinks/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15045 2022-11-13 17:22:14.000000 zoinks-0.0.7/zoinks/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1013 2022-01-03 16:10:18.000000 zoinks-0.0.7/zoinks/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1394 2022-01-03 15:22:00.000000 zoinks-0.0.7/zoinks/exit_codes.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-12 19:19:44.635202 zoinks-0.0.7/zoinks.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)     4241 2023-04-12 19:19:44.000000 zoinks-0.0.7/zoinks.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      327 2023-04-12 19:19:44.000000 zoinks-0.0.7/zoinks.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-12 19:19:44.000000 zoinks-0.0.7/zoinks.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       64 2023-04-12 19:19:44.000000 zoinks-0.0.7/zoinks.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-12 19:19:44.000000 zoinks-0.0.7/zoinks.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      129 2023-04-12 19:19:44.000000 zoinks-0.0.7/zoinks.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        7 2023-04-12 19:19:44.000000 zoinks-0.0.7/zoinks.egg-info/top_level.txt
```

### Comparing `zoinks-0.0.6/LICENSE` & `zoinks-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zoinks-0.0.6/PKG-INFO` & `zoinks-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoinks
-Version: 0.0.6
+Version: 0.0.7
 Summary: Zoinks: a command-line utility to retrieve Zotero record values
 Home-page: https://github.com/mhucka/zoinks
 Author: Mike Hucka
 Author-email: mhucka@caltech.edu
 License: BSD 3-clause license
 Project-URL: Source Code, https://github.com/mhucka/zoinks
 Project-URL: Bug Tracker, https://github.com/mhucka/zoinks/issues
```

### Comparing `zoinks-0.0.6/README.md` & `zoinks-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `zoinks-0.0.6/setup.cfg` & `zoinks-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = zoinks
-version = 0.0.6
+version = 0.0.7
 description = Zoinks: a command-line utility to retrieve Zotero record values
 author = Mike Hucka
 author_email = mhucka@caltech.edu
 license = BSD 3-clause license
 license_files = LICENSE
 url = https://github.com/mhucka/zoinks
 project_urls =
```

### Comparing `zoinks-0.0.6/setup.py` & `zoinks-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `zoinks-0.0.6/zoinks/__init__.py` & `zoinks-0.0.7/zoinks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Package metadata ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '0.0.6'
+__version__     = '0.0.7'
 __description__ = 'Zoinks: a command-line utility to retrieve Zotero record values'
 __url__         = 'https://github.com/mhucka/zoinks'
 __author__      = 'Mike Hucka'
 __email__       = 'mhucka@caltech.edu'
 __license__     = 'BSD 3-clause license'
```

### Comparing `zoinks-0.0.6/zoinks/__main__.py` & `zoinks-0.0.7/zoinks/__main__.py`

 * *Files identical despite different names*

### Comparing `zoinks-0.0.6/zoinks/exceptions.py` & `zoinks-0.0.7/zoinks/exceptions.py`

 * *Files identical despite different names*

### Comparing `zoinks-0.0.6/zoinks/exit_codes.py` & `zoinks-0.0.7/zoinks/exit_codes.py`

 * *Files identical despite different names*

### Comparing `zoinks-0.0.6/zoinks.egg-info/PKG-INFO` & `zoinks-0.0.7/zoinks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoinks
-Version: 0.0.6
+Version: 0.0.7
 Summary: Zoinks: a command-line utility to retrieve Zotero record values
 Home-page: https://github.com/mhucka/zoinks
 Author: Mike Hucka
 Author-email: mhucka@caltech.edu
 License: BSD 3-clause license
 Project-URL: Source Code, https://github.com/mhucka/zoinks
 Project-URL: Bug Tracker, https://github.com/mhucka/zoinks/issues
```

