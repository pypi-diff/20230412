# Comparing `tmp/dttimeframe-3.6.2.tar.gz` & `tmp/dttimeframe-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dttimeframe-3.6.2.tar", last modified: Thu Mar 30 04:24:44 2023, max compression
+gzip compressed data, was "dttimeframe-3.6.3.tar", last modified: Wed Apr 12 07:21:03 2023, max compression
```

## Comparing `dttimeframe-3.6.2.tar` & `dttimeframe-3.6.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-03-30 04:24:44.726755 dttimeframe-3.6.2/
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)    35147 2023-01-11 07:08:21.000000 dttimeframe-3.6.2/LICENSE
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     2833 2023-03-30 04:24:44.722753 dttimeframe-3.6.2/PKG-INFO
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     1853 2023-03-30 04:22:56.000000 dttimeframe-3.6.2/README.md
-drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-03-30 04:24:44.664684 dttimeframe-3.6.2/dttimeframe/
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-03-29 08:33:59.000000 dttimeframe-3.6.2/dttimeframe/__init__.py
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)    10515 2023-03-29 08:33:59.000000 dttimeframe-3.6.2/dttimeframe/timeFrame.py
-drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-03-30 04:24:44.709946 dttimeframe-3.6.2/dttimeframe.egg-info/
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     2833 2023-03-30 04:24:44.000000 dttimeframe-3.6.2/dttimeframe.egg-info/PKG-INFO
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)      215 2023-03-30 04:24:44.000000 dttimeframe-3.6.2/dttimeframe.egg-info/SOURCES.txt
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        1 2023-03-30 04:24:44.000000 dttimeframe-3.6.2/dttimeframe.egg-info/dependency_links.txt
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)       12 2023-03-30 04:24:44.000000 dttimeframe-3.6.2/dttimeframe.egg-info/top_level.txt
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)       38 2023-03-30 04:24:44.726755 dttimeframe-3.6.2/setup.cfg
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     1148 2023-03-30 04:24:25.000000 dttimeframe-3.6.2/setup.py
+drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-04-12 07:21:03.012568 dttimeframe-3.6.3/
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)    35147 2023-01-11 07:08:21.000000 dttimeframe-3.6.3/LICENSE
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     2833 2023-04-12 07:21:03.009134 dttimeframe-3.6.3/PKG-INFO
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     1853 2023-04-12 07:11:15.000000 dttimeframe-3.6.3/README.md
+drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-04-12 07:21:02.949689 dttimeframe-3.6.3/dttimeframe/
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-03-29 08:33:59.000000 dttimeframe-3.6.3/dttimeframe/__init__.py
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)    10515 2023-03-29 08:33:59.000000 dttimeframe-3.6.3/dttimeframe/timeFrame.py
+drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-04-12 07:21:02.997727 dttimeframe-3.6.3/dttimeframe.egg-info/
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     2833 2023-04-12 07:21:02.000000 dttimeframe-3.6.3/dttimeframe.egg-info/PKG-INFO
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)      215 2023-04-12 07:21:02.000000 dttimeframe-3.6.3/dttimeframe.egg-info/SOURCES.txt
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        1 2023-04-12 07:21:02.000000 dttimeframe-3.6.3/dttimeframe.egg-info/dependency_links.txt
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)       12 2023-04-12 07:21:02.000000 dttimeframe-3.6.3/dttimeframe.egg-info/top_level.txt
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)       38 2023-04-12 07:21:03.013885 dttimeframe-3.6.3/setup.cfg
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     1148 2023-04-12 07:13:41.000000 dttimeframe-3.6.3/setup.py
```

### Comparing `dttimeframe-3.6.2/LICENSE` & `dttimeframe-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dttimeframe-3.6.2/PKG-INFO` & `dttimeframe-3.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dttimeframe
-Version: 3.6.2
+Version: 3.6.3
 Summary: dtTimeFrame is a module that pack time track functions and subprocess call functions into one single class.
 Home-page: https://github.com/SotongDJ/dtTimeFrame
 Author: David Soh
 Author-email: ln@trth.nl
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dttimeframe-3.6.2/README.md` & `dttimeframe-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `dttimeframe-3.6.2/dttimeframe/timeFrame.py` & `dttimeframe-3.6.3/dttimeframe/timeFrame.py`

 * *Files identical despite different names*

### Comparing `dttimeframe-3.6.2/dttimeframe.egg-info/PKG-INFO` & `dttimeframe-3.6.3/dttimeframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dttimeframe
-Version: 3.6.2
+Version: 3.6.3
 Summary: dtTimeFrame is a module that pack time track functions and subprocess call functions into one single class.
 Home-page: https://github.com/SotongDJ/dtTimeFrame
 Author: David Soh
 Author-email: ln@trth.nl
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dttimeframe-3.6.2/setup.py` & `dttimeframe-3.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name = "dttimeframe",
-    version = "3.6.2",
+    version = "3.6.3",
     author = "David Soh",
     author_email = "ln@trth.nl",
     description = "dtTimeFrame is a module that pack time track functions and subprocess call functions into one single class.",
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     url = "https://github.com/SotongDJ/dtTimeFrame",
     packages = ["dttimeframe"],
```

