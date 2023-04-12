# Comparing `tmp/thunno2-2.0.5.tar.gz` & `tmp/thunno2-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.0.5.tar", last modified: Wed Apr 12 15:36:12 2023, max compression
+gzip compressed data, was "thunno2-2.0.6.tar", last modified: Wed Apr 12 15:38:06 2023, max compression
```

## Comparing `thunno2-2.0.5.tar` & `thunno2-2.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 15:36:12.560567 thunno2-2.0.5/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 15:36:12.560438 thunno2-2.0.5/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-12 15:36:12.560607 thunno2-2.0.5/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.0.5/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 15:36:12.559675 thunno2-2.0.5/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.0.5/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.0.5/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    39327 2023-04-11 16:50:16.000000 thunno2-2.0.5/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2891 2023-04-03 16:27:37.000000 thunno2-2.0.5/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   244557 2023-04-08 16:04:36.000000 thunno2-2.0.5/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     4252 2023-04-12 15:35:27.000000 thunno2-2.0.5/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    40904 2023-04-11 19:11:59.000000 thunno2-2.0.5/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    18356 2023-04-11 14:03:07.000000 thunno2-2.0.5/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    14374 2023-04-11 14:03:07.000000 thunno2-2.0.5/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1215 2023-04-12 10:14:32.000000 thunno2-2.0.5/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    55521 2023-04-11 17:00:38.000000 thunno2-2.0.5/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     1004 2023-04-06 20:08:08.000000 thunno2-2.0.5/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-12 15:36:03.000000 thunno2-2.0.5/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 15:36:12.560267 thunno2-2.0.5/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 15:36:12.000000 thunno2-2.0.5/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-12 15:36:12.000000 thunno2-2.0.5/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-12 15:36:12.000000 thunno2-2.0.5/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-12 15:36:12.000000 thunno2-2.0.5/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-12 15:36:12.000000 thunno2-2.0.5/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 15:38:06.962514 thunno2-2.0.6/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 15:38:06.962402 thunno2-2.0.6/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-12 15:38:06.962550 thunno2-2.0.6/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.0.6/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 15:38:06.961693 thunno2-2.0.6/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.0.6/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.0.6/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    39327 2023-04-11 16:50:16.000000 thunno2-2.0.6/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2891 2023-04-03 16:27:37.000000 thunno2-2.0.6/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   244557 2023-04-08 16:04:36.000000 thunno2-2.0.6/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4260 2023-04-12 15:37:54.000000 thunno2-2.0.6/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    40904 2023-04-11 19:11:59.000000 thunno2-2.0.6/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    18356 2023-04-11 14:03:07.000000 thunno2-2.0.6/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    14374 2023-04-11 14:03:07.000000 thunno2-2.0.6/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1215 2023-04-12 10:14:32.000000 thunno2-2.0.6/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    55521 2023-04-11 17:00:38.000000 thunno2-2.0.6/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1004 2023-04-06 20:08:08.000000 thunno2-2.0.6/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-12 15:37:54.000000 thunno2-2.0.6/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 15:38:06.962249 thunno2-2.0.6/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 15:38:06.000000 thunno2-2.0.6/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-12 15:38:06.000000 thunno2-2.0.6/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-12 15:38:06.000000 thunno2-2.0.6/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-12 15:38:06.000000 thunno2-2.0.6/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-12 15:38:06.000000 thunno2-2.0.6/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.0.5/PKG-INFO` & `thunno2-2.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.5
+Version: 2.0.6
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.5.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.6.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.0.5/setup.py` & `thunno2-2.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.5/thunno2/codepage.py` & `thunno2-2.0.6/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.5/thunno2/commands.py` & `thunno2-2.0.6/thunno2/commands.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.5/thunno2/constants.py` & `thunno2-2.0.6/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.5/thunno2/dictionary.py` & `thunno2-2.0.6/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.5/thunno2/flags.py` & `thunno2-2.0.6/thunno2/flags.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                     new_inputs = process_input_flags(new_flags, '\n'.join(map(repr, x)))
                 else:
                     new_inputs = [x]
             except:
                 new_inputs = [line]
             commands.ctx.og_input_list = new_inputs.copy()
             commands.ctx.other_il = new_inputs.copy()
-            print(line, '--> ')
+            print(line, '--> ', end='')
             interpreter.run(code, n=0, iteration_index=0)
             process_output_flags(new_flags)
         return None
 
     inputs = process_input_flags(flags, inputs)
     commands.ctx.og_input_list = inputs.copy()
     commands.ctx.other_il = inputs.copy()
```

### Comparing `thunno2-2.0.5/thunno2/helpers.py` & `thunno2-2.0.6/thunno2/helpers.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.5/thunno2/interpreter.py` & `thunno2-2.0.6/thunno2/interpreter.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.5/thunno2/lexer.py` & `thunno2-2.0.6/thunno2/lexer.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.5/thunno2/run.py` & `thunno2-2.0.6/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.5/thunno2/tests.py` & `thunno2-2.0.6/thunno2/tests.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.5/thunno2/tokens.py` & `thunno2-2.0.6/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.5/thunno2.egg-info/PKG-INFO` & `thunno2-2.0.6/thunno2.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.5
+Version: 2.0.6
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.5.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.6.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

