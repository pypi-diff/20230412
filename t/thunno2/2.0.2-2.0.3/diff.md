# Comparing `tmp/thunno2-2.0.2.tar.gz` & `tmp/thunno2-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.0.2.tar", last modified: Wed Apr 12 09:59:53 2023, max compression
+gzip compressed data, was "thunno2-2.0.3.tar", last modified: Wed Apr 12 10:07:26 2023, max compression
```

## Comparing `thunno2-2.0.2.tar` & `thunno2-2.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 09:59:53.677110 thunno2-2.0.2/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 09:59:53.676987 thunno2-2.0.2/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-12 09:59:53.677151 thunno2-2.0.2/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.0.2/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 09:59:53.676061 thunno2-2.0.2/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.0.2/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.0.2/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    39327 2023-04-11 16:50:16.000000 thunno2-2.0.2/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2891 2023-04-03 16:27:37.000000 thunno2-2.0.2/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   244557 2023-04-08 16:04:36.000000 thunno2-2.0.2/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     2896 2023-04-12 09:58:27.000000 thunno2-2.0.2/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    40904 2023-04-11 19:11:59.000000 thunno2-2.0.2/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    18356 2023-04-11 14:03:07.000000 thunno2-2.0.2/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    14374 2023-04-11 14:03:07.000000 thunno2-2.0.2/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1215 2023-04-12 09:58:27.000000 thunno2-2.0.2/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    55521 2023-04-11 17:00:38.000000 thunno2-2.0.2/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     1004 2023-04-06 20:08:08.000000 thunno2-2.0.2/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-12 09:59:17.000000 thunno2-2.0.2/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 09:59:53.676787 thunno2-2.0.2/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 09:59:53.000000 thunno2-2.0.2/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-12 09:59:53.000000 thunno2-2.0.2/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-12 09:59:53.000000 thunno2-2.0.2/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-12 09:59:53.000000 thunno2-2.0.2/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-12 09:59:53.000000 thunno2-2.0.2/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 10:07:26.799659 thunno2-2.0.3/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 10:07:26.799519 thunno2-2.0.3/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-12 10:07:26.799701 thunno2-2.0.3/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.0.3/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 10:07:26.798676 thunno2-2.0.3/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.0.3/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.0.3/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    39327 2023-04-11 16:50:16.000000 thunno2-2.0.3/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2891 2023-04-03 16:27:37.000000 thunno2-2.0.3/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   244557 2023-04-08 16:04:36.000000 thunno2-2.0.3/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2896 2023-04-12 09:58:27.000000 thunno2-2.0.3/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    40904 2023-04-11 19:11:59.000000 thunno2-2.0.3/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    18356 2023-04-11 14:03:07.000000 thunno2-2.0.3/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    14374 2023-04-11 14:03:07.000000 thunno2-2.0.3/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1215 2023-04-12 10:05:20.000000 thunno2-2.0.3/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    55521 2023-04-11 17:00:38.000000 thunno2-2.0.3/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1004 2023-04-06 20:08:08.000000 thunno2-2.0.3/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-12 10:06:44.000000 thunno2-2.0.3/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 10:07:26.799255 thunno2-2.0.3/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 10:07:26.000000 thunno2-2.0.3/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-12 10:07:26.000000 thunno2-2.0.3/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-12 10:07:26.000000 thunno2-2.0.3/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-12 10:07:26.000000 thunno2-2.0.3/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-12 10:07:26.000000 thunno2-2.0.3/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.0.2/PKG-INFO` & `thunno2-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.2
+Version: 2.0.3
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.2.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.3.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.0.2/setup.py` & `thunno2-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.2/thunno2/codepage.py` & `thunno2-2.0.3/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.2/thunno2/commands.py` & `thunno2-2.0.3/thunno2/commands.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.2/thunno2/constants.py` & `thunno2-2.0.3/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.2/thunno2/dictionary.py` & `thunno2-2.0.3/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.2/thunno2/flags.py` & `thunno2-2.0.3/thunno2/flags.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.2/thunno2/helpers.py` & `thunno2-2.0.3/thunno2/helpers.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.2/thunno2/interpreter.py` & `thunno2-2.0.3/thunno2/interpreter.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.2/thunno2/lexer.py` & `thunno2-2.0.3/thunno2/lexer.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.2/thunno2/run.py` & `thunno2-2.0.3/thunno2/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from thunno2 import lexer, version
-import flags, sys
+from thunno2 import lexer, version, flags
+import sys
 
 
 def from_terminal():
     print('Thunno', version.THUNNO_VERSION, 'interpreter\n')
     print('\nFlags:')
     flags_list = input()
     code = ''
```

### Comparing `thunno2-2.0.2/thunno2/tests.py` & `thunno2-2.0.3/thunno2/tests.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.2/thunno2/tokens.py` & `thunno2-2.0.3/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.2/thunno2.egg-info/PKG-INFO` & `thunno2-2.0.3/thunno2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.2
+Version: 2.0.3
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.2.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.3.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

