# Comparing `tmp/pdfreactor.plone-1.0.2.tar.gz` & `tmp/pdfreactor.plone-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pdfreactor.plone-1.0.2.tar", last modified: Fri Jan 20 19:47:13 2023, max compression
+gzip compressed data, was "dist/pdfreactor.plone-1.0.3.tar", last modified: Wed Apr  5 15:57:07 2023, max compression
```

## Comparing `pdfreactor.plone-1.0.2.tar` & `pdfreactor.plone-1.0.3.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/docs/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/docs/resources/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     6930 2022-05-27 12:15:00.000000 pdfreactor.plone-1.0.2/docs/resources/contentPython.html
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      339 2022-05-27 12:15:00.000000 pdfreactor.plone-1.0.2/docs/index.rst
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/pdfreactor/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/profiles/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/profiles/default/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      595 2022-07-11 16:46:11.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/profiles/default/controlpanel.xml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       68 2022-07-11 16:46:11.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/profiles/default/metadata.xml
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/resource/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      543 2022-08-24 08:01:25.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/resource/export.css
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      928 2022-12-13 22:20:33.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/resource/mathjax2-run.js
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       27 2022-06-08 10:16:07.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1079 2022-08-24 08:01:25.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/_mixin.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3624 2022-07-11 10:33:36.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/async.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     7663 2023-01-20 19:45:52.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/base.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2122 2022-12-20 09:35:40.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/config.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2618 2022-12-20 09:35:40.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      575 2022-07-11 16:46:11.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/controlpanel.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2697 2022-12-20 09:35:40.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/interfaces.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3014 2022-07-11 10:33:36.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/monitor.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1301 2022-07-11 16:46:11.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/profiles.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2876 2022-07-12 09:03:52.000000 pdfreactor.plone-1.0.2/src/pdfreactor/plone/setuphandlers.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      627 2022-07-11 10:32:53.000000 pdfreactor.plone-1.0.2/src/pdfreactor/__init__.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/pdfreactor.plone.egg-info/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8129 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/pdfreactor.plone.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1091 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/pdfreactor.plone.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/pdfreactor.plone.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/pdfreactor.plone.egg-info/entry_points.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       11 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/pdfreactor.plone.egg-info/namespace_packages.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2022-06-01 10:22:48.000000 pdfreactor.plone-1.0.2/src/pdfreactor.plone.egg-info/not-zip-safe
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       26 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/pdfreactor.plone.egg-info/requires.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       11 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/src/pdfreactor.plone.egg-info/top_level.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1016 2023-01-20 19:47:10.000000 pdfreactor.plone-1.0.2/CHANGES.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       55 2022-06-17 12:51:45.000000 pdfreactor.plone-1.0.2/CONTRIBUTORS.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      204 2022-06-07 17:09:20.000000 pdfreactor.plone-1.0.2/MANIFEST.in
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4388 2022-12-13 22:14:54.000000 pdfreactor.plone-1.0.2/README.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2022-12-13 22:20:33.000000 pdfreactor.plone-1.0.2/VERSION
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       88 2022-05-27 11:39:37.000000 pdfreactor.plone-1.0.2/pyproject.toml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1539 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/setup.cfg
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     6370 2022-12-13 22:20:40.000000 pdfreactor.plone-1.0.2/setup.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8129 2023-01-20 19:47:13.000000 pdfreactor.plone-1.0.2/PKG-INFO
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 15:57:07.000000 pdfreactor.plone-1.0.3/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 15:57:07.000000 pdfreactor.plone-1.0.3/docs/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 15:57:07.000000 pdfreactor.plone-1.0.3/docs/resources/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     6930 2022-05-27 12:15:00.000000 pdfreactor.plone-1.0.3/docs/resources/contentPython.html
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      339 2022-05-27 12:15:00.000000 pdfreactor.plone-1.0.3/docs/index.rst
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 15:57:07.000000 pdfreactor.plone-1.0.3/src/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 15:57:07.000000 pdfreactor.plone-1.0.3/src/pdfreactor/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 15:57:07.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 15:57:07.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/profiles/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 15:57:07.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/profiles/default/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      595 2022-07-11 16:46:11.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/profiles/default/controlpanel.xml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       68 2022-07-11 16:46:11.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/profiles/default/metadata.xml
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 15:57:07.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/resource/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      543 2022-08-24 08:01:25.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/resource/export.css
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      928 2023-03-12 00:09:29.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/resource/mathjax2-run.js
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       27 2022-06-08 10:16:07.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1079 2022-08-24 08:01:25.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/_mixin.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3624 2022-07-11 10:33:36.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/async.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    11724 2023-04-03 12:25:12.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/base.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2122 2023-03-12 00:09:29.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/config.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2618 2023-03-12 00:09:29.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      575 2022-07-11 16:46:11.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/controlpanel.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2697 2023-03-12 00:09:29.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/interfaces.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3014 2022-07-11 10:33:36.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/monitor.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1301 2022-07-11 16:46:11.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/profiles.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    50383 2023-03-30 13:44:54.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/raw_api.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2876 2022-07-12 09:03:52.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/setuphandlers.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3230 2023-03-30 13:44:54.000000 pdfreactor.plone-1.0.3/src/pdfreactor/plone/utils.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      627 2022-07-11 10:32:53.000000 pdfreactor.plone-1.0.3/src/pdfreactor/__init__.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 15:57:07.000000 pdfreactor.plone-1.0.3/src/pdfreactor.plone.egg-info/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    10088 2023-04-05 15:57:06.000000 pdfreactor.plone-1.0.3/src/pdfreactor.plone.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1153 2023-04-05 15:57:07.000000 pdfreactor.plone-1.0.3/src/pdfreactor.plone.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2023-04-05 15:57:06.000000 pdfreactor.plone-1.0.3/src/pdfreactor.plone.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2023-04-05 15:57:06.000000 pdfreactor.plone-1.0.3/src/pdfreactor.plone.egg-info/entry_points.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       11 2023-04-05 15:57:06.000000 pdfreactor.plone-1.0.3/src/pdfreactor.plone.egg-info/namespace_packages.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2022-06-01 10:22:48.000000 pdfreactor.plone-1.0.3/src/pdfreactor.plone.egg-info/not-zip-safe
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       26 2023-04-05 15:57:06.000000 pdfreactor.plone-1.0.3/src/pdfreactor.plone.egg-info/requires.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       11 2023-04-05 15:57:06.000000 pdfreactor.plone-1.0.3/src/pdfreactor.plone.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2599 2023-04-05 15:57:03.000000 pdfreactor.plone-1.0.3/CHANGES.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       55 2022-06-17 12:51:45.000000 pdfreactor.plone-1.0.3/CONTRIBUTORS.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      204 2022-06-07 17:09:20.000000 pdfreactor.plone-1.0.3/MANIFEST.in
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4388 2022-12-13 22:14:54.000000 pdfreactor.plone-1.0.3/README.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2023-03-30 13:44:54.000000 pdfreactor.plone-1.0.3/VERSION
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       88 2022-05-27 11:39:37.000000 pdfreactor.plone-1.0.3/pyproject.toml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1539 2023-04-05 15:57:07.000000 pdfreactor.plone-1.0.3/setup.cfg
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     6370 2022-12-13 22:20:40.000000 pdfreactor.plone-1.0.3/setup.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    10088 2023-04-05 15:57:07.000000 pdfreactor.plone-1.0.3/PKG-INFO
```

### Comparing `pdfreactor.plone-1.0.2/docs/resources/contentPython.html` & `pdfreactor.plone-1.0.3/docs/resources/contentPython.html`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor/plone/profiles/default/controlpanel.xml` & `pdfreactor.plone-1.0.3/src/pdfreactor/plone/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor/plone/resource/export.css` & `pdfreactor.plone-1.0.3/src/pdfreactor/plone/resource/export.css`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor/plone/resource/mathjax2-run.js` & `pdfreactor.plone-1.0.3/src/pdfreactor/plone/resource/mathjax2-run.js`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor/plone/_mixin.py` & `pdfreactor.plone-1.0.3/src/pdfreactor/plone/_mixin.py`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor/plone/async.py` & `pdfreactor.plone-1.0.3/src/pdfreactor/plone/async.py`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor/plone/config.py` & `pdfreactor.plone-1.0.3/src/pdfreactor/plone/config.py`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor/plone/configure.zcml` & `pdfreactor.plone-1.0.3/src/pdfreactor/plone/configure.zcml`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor/plone/controlpanel.py` & `pdfreactor.plone-1.0.3/src/pdfreactor/plone/controlpanel.py`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor/plone/interfaces.py` & `pdfreactor.plone-1.0.3/src/pdfreactor/plone/interfaces.py`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor/plone/monitor.py` & `pdfreactor.plone-1.0.3/src/pdfreactor/plone/monitor.py`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor/plone/profiles.zcml` & `pdfreactor.plone-1.0.3/src/pdfreactor/plone/profiles.zcml`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor/plone/setuphandlers.py` & `pdfreactor.plone-1.0.3/src/pdfreactor/plone/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor/__init__.py` & `pdfreactor.plone-1.0.3/src/pdfreactor/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor.plone.egg-info/PKG-INFO` & `pdfreactor.plone-1.0.3/src/pdfreactor.plone.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfreactor.plone
-Version: 1.0.2
+Version: 1.0.3
 Summary: PDFreactor integration for Plone
 Home-page: UNKNOWN
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: MIT License
 Project-URL: Source, https://github.com/visaplan/pdfreactor.plone
 Project-URL: Documentation, https://pypi.org/project/pdfreactor.plone
@@ -164,30 +164,75 @@
         - Tobias Herp, tobias.herp@visaplan.com
         
         
         Changelog
         =========
         
         
+        1.0.3 (2023-04-05)
+        ------------------
+        
+        New Features:
+        
+        - The .base.Exporter class now provides an own `.convert` method
+          which accepts `binary`, `async` and `stream` arguments
+          and calls the appropriate conversion method internally.
+        
+          Currently, it will return
+        
+          - `None`, if a `stream` was given,
+          - binary data, if `binary` was given (and not `stream`), and
+          - the document_id, if `async` was given, and
+          - a `dict` with all meta information contained otherwise.
+        
+        Improvements:
+        
+        - The .base.Exporter class now provides (and uses) a `conversionSource`
+          method which in turn uses the existing `converted_url` method.
+        
+          **Note:** if providing text instead of a URL as the ``document`` config key,
+          you likely need to specify a ``baseUrl`` as well; otherwise the reactor
+          might fail to load stylesheets or images during conversion.
+        
+        Development hints:
+        
+        - When developing and testing your PDFreactor_ conversions,
+          be sure you have more than one Zope worker thread ready;
+          otherwise you might wonder about HTTP errors
+          when the reactor sends requests to your instance!
+        
+        - We provide the original API (from the PDFreactor_ distribution) as `.raw_api`
+          module (for development and testing;
+          helps to check whether a certain problem
+          is related to our pythonization measures).
+        
+          Just in case.
+        
+        [tobiasherp]
+        
+        
         1.0.2 (2023-01-20)
         ------------------
         
         New Features:
         
         - For `MathML` support:
          
           - added a `@@pdfreactor-mathjax-vars.js` view (for configuration),
             and 
           - a ``++resource++pdfreactor.plone/mathjax2-run.js``
-            script to ease MathJax integration.
+            script to ease MathJax_ integration.
         
           This is not configurable yet, but will likely be, soon.
         
+          **Note:** `PDFreactor v11.6.3`_ (2023-03-07) contains a fix
+          to a bug which caused `MathML` exports as "continuous media" to fail.
+        
         - The @@as.pdf method supports a `method` option; e.g., call
-          ``.../my/page/@@as.pdf?method=@@from-screeshot`` to create a PDF file from
+          ``.../my/page/@@as.pdf?method=@@from-screenshot`` to create a PDF file from
           ``.../my/page/@@from-screenshot``.
         
         [tobiasherp]
         
         
         1.0.1 (2022-09-20)
         ------------------
@@ -206,14 +251,16 @@
         1.0.0 (2022-07-12)
         ------------------
         
         - Initial release.
           [tobiasherp]
         
         .. _MathJax: https://www.mathjax.org
+        .. _PDFreactor: https://www.pdfreactor.com
+        .. _`PDFreactor v11.6.3`: https://www.pdfreactor.com/product/changelog.htm#v11.6.3
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.3
 Classifier: Framework :: Zope2
 Classifier: Programming Language :: Python
```

### Comparing `pdfreactor.plone-1.0.2/src/pdfreactor.plone.egg-info/SOURCES.txt` & `pdfreactor.plone-1.0.3/src/pdfreactor.plone.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -23,12 +23,14 @@
 src/pdfreactor/plone/base.py
 src/pdfreactor/plone/config.py
 src/pdfreactor/plone/configure.zcml
 src/pdfreactor/plone/controlpanel.py
 src/pdfreactor/plone/interfaces.py
 src/pdfreactor/plone/monitor.py
 src/pdfreactor/plone/profiles.zcml
+src/pdfreactor/plone/raw_api.py
 src/pdfreactor/plone/setuphandlers.py
+src/pdfreactor/plone/utils.py
 src/pdfreactor/plone/profiles/default/controlpanel.xml
 src/pdfreactor/plone/profiles/default/metadata.xml
 src/pdfreactor/plone/resource/export.css
 src/pdfreactor/plone/resource/mathjax2-run.js
```

### Comparing `pdfreactor.plone-1.0.2/README.rst` & `pdfreactor.plone-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/setup.cfg` & `pdfreactor.plone-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/setup.py` & `pdfreactor.plone-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `pdfreactor.plone-1.0.2/PKG-INFO` & `pdfreactor.plone-1.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfreactor.plone
-Version: 1.0.2
+Version: 1.0.3
 Summary: PDFreactor integration for Plone
 Home-page: UNKNOWN
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: MIT License
 Project-URL: Source, https://github.com/visaplan/pdfreactor.plone
 Project-URL: Documentation, https://pypi.org/project/pdfreactor.plone
@@ -164,30 +164,75 @@
         - Tobias Herp, tobias.herp@visaplan.com
         
         
         Changelog
         =========
         
         
+        1.0.3 (2023-04-05)
+        ------------------
+        
+        New Features:
+        
+        - The .base.Exporter class now provides an own `.convert` method
+          which accepts `binary`, `async` and `stream` arguments
+          and calls the appropriate conversion method internally.
+        
+          Currently, it will return
+        
+          - `None`, if a `stream` was given,
+          - binary data, if `binary` was given (and not `stream`), and
+          - the document_id, if `async` was given, and
+          - a `dict` with all meta information contained otherwise.
+        
+        Improvements:
+        
+        - The .base.Exporter class now provides (and uses) a `conversionSource`
+          method which in turn uses the existing `converted_url` method.
+        
+          **Note:** if providing text instead of a URL as the ``document`` config key,
+          you likely need to specify a ``baseUrl`` as well; otherwise the reactor
+          might fail to load stylesheets or images during conversion.
+        
+        Development hints:
+        
+        - When developing and testing your PDFreactor_ conversions,
+          be sure you have more than one Zope worker thread ready;
+          otherwise you might wonder about HTTP errors
+          when the reactor sends requests to your instance!
+        
+        - We provide the original API (from the PDFreactor_ distribution) as `.raw_api`
+          module (for development and testing;
+          helps to check whether a certain problem
+          is related to our pythonization measures).
+        
+          Just in case.
+        
+        [tobiasherp]
+        
+        
         1.0.2 (2023-01-20)
         ------------------
         
         New Features:
         
         - For `MathML` support:
          
           - added a `@@pdfreactor-mathjax-vars.js` view (for configuration),
             and 
           - a ``++resource++pdfreactor.plone/mathjax2-run.js``
-            script to ease MathJax integration.
+            script to ease MathJax_ integration.
         
           This is not configurable yet, but will likely be, soon.
         
+          **Note:** `PDFreactor v11.6.3`_ (2023-03-07) contains a fix
+          to a bug which caused `MathML` exports as "continuous media" to fail.
+        
         - The @@as.pdf method supports a `method` option; e.g., call
-          ``.../my/page/@@as.pdf?method=@@from-screeshot`` to create a PDF file from
+          ``.../my/page/@@as.pdf?method=@@from-screenshot`` to create a PDF file from
           ``.../my/page/@@from-screenshot``.
         
         [tobiasherp]
         
         
         1.0.1 (2022-09-20)
         ------------------
@@ -206,14 +251,16 @@
         1.0.0 (2022-07-12)
         ------------------
         
         - Initial release.
           [tobiasherp]
         
         .. _MathJax: https://www.mathjax.org
+        .. _PDFreactor: https://www.pdfreactor.com
+        .. _`PDFreactor v11.6.3`: https://www.pdfreactor.com/product/changelog.htm#v11.6.3
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.3
 Classifier: Framework :: Zope2
 Classifier: Programming Language :: Python
```

