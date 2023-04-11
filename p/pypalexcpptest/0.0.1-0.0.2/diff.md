# Comparing `tmp/pypalexcpptest-0.0.1.tar.gz` & `tmp/pypalexcpptest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypalexcpptest-0.0.1.tar", last modified: Tue Apr 11 22:00:24 2023, max compression
+gzip compressed data, was "dist/pypalexcpptest-0.0.2.tar", last modified: Tue Apr 11 22:05:09 2023, max compression
```

## Comparing `pypalexcpptest-0.0.1.tar` & `pypalexcpptest-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 altimofeyev   (501) staff       (20)        0 2023-04-11 22:00:24.104554 pypalexcpptest-0.0.1/
--rw-r--r--   0 altimofeyev   (501) staff       (20)     1001 2023-04-11 22:00:24.104286 pypalexcpptest-0.0.1/PKG-INFO
--rw-r--r--   0 altimofeyev   (501) staff       (20)       61 2023-04-11 21:02:26.000000 pypalexcpptest-0.0.1/README.md
-drwxr-xr-x   0 altimofeyev   (501) staff       (20)        0 2023-04-11 22:00:24.101487 pypalexcpptest-0.0.1/pypalexcpptest/
--rw-r--r--   0 altimofeyev   (501) staff       (20)      419 2023-04-11 21:55:37.000000 pypalexcpptest-0.0.1/pypalexcpptest/__init__.py
--rw-r--r--   0 altimofeyev   (501) staff       (20)     7459 2023-04-11 21:56:22.000000 pypalexcpptest-0.0.1/pypalexcpptest/__main__.py
--rw-r--r--   0 altimofeyev   (501) staff       (20)     2385 2023-03-07 02:13:31.000000 pypalexcpptest-0.0.1/pypalexcpptest/arg_messages.py
--rw-r--r--   0 altimofeyev   (501) staff       (20)     1524 2023-04-11 21:57:06.000000 pypalexcpptest-0.0.1/pypalexcpptest/conversion_tests.py
--rw-r--r--   0 altimofeyev   (501) staff       (20)     4342 2023-04-08 02:04:19.000000 pypalexcpptest-0.0.1/pypalexcpptest/conversion_utils.py
--rw-r--r--   0 altimofeyev   (501) staff       (20)     2211 2023-04-11 21:57:06.000000 pypalexcpptest-0.0.1/pypalexcpptest/image_utils.py
--rw-r--r--   0 altimofeyev   (501) staff       (20)      640 2023-04-11 21:11:43.000000 pypalexcpptest-0.0.1/pypalexcpptest/settings.py
-drwxr-xr-x   0 altimofeyev   (501) staff       (20)        0 2023-04-11 22:00:24.103808 pypalexcpptest-0.0.1/pypalexcpptest.egg-info/
--rw-r--r--   0 altimofeyev   (501) staff       (20)     1001 2023-04-11 22:00:23.000000 pypalexcpptest-0.0.1/pypalexcpptest.egg-info/PKG-INFO
--rw-r--r--   0 altimofeyev   (501) staff       (20)      497 2023-04-11 22:00:23.000000 pypalexcpptest-0.0.1/pypalexcpptest.egg-info/SOURCES.txt
--rw-r--r--   0 altimofeyev   (501) staff       (20)        1 2023-04-11 22:00:23.000000 pypalexcpptest-0.0.1/pypalexcpptest.egg-info/dependency_links.txt
--rw-r--r--   0 altimofeyev   (501) staff       (20)       63 2023-04-11 22:00:23.000000 pypalexcpptest-0.0.1/pypalexcpptest.egg-info/entry_points.txt
--rw-r--r--   0 altimofeyev   (501) staff       (20)        1 2023-04-11 22:00:23.000000 pypalexcpptest-0.0.1/pypalexcpptest.egg-info/not-zip-safe
--rw-r--r--   0 altimofeyev   (501) staff       (20)       22 2023-04-11 22:00:23.000000 pypalexcpptest-0.0.1/pypalexcpptest.egg-info/requires.txt
--rw-r--r--   0 altimofeyev   (501) staff       (20)       15 2023-04-11 22:00:23.000000 pypalexcpptest-0.0.1/pypalexcpptest.egg-info/top_level.txt
--rw-r--r--   0 altimofeyev   (501) staff       (20)       38 2023-04-11 22:00:24.104659 pypalexcpptest-0.0.1/setup.cfg
--rw-r--r--   0 altimofeyev   (501) staff       (20)     1705 2023-04-11 21:40:12.000000 pypalexcpptest-0.0.1/setup.py
+drwxr-xr-x   0 altimofeyev   (501) staff       (20)        0 2023-04-11 22:05:09.070834 pypalexcpptest-0.0.2/
+-rw-r--r--   0 altimofeyev   (501) staff       (20)     1001 2023-04-11 22:05:09.070620 pypalexcpptest-0.0.2/PKG-INFO
+-rw-r--r--   0 altimofeyev   (501) staff       (20)       61 2023-04-11 21:02:26.000000 pypalexcpptest-0.0.2/README.md
+drwxr-xr-x   0 altimofeyev   (501) staff       (20)        0 2023-04-11 22:05:09.068389 pypalexcpptest-0.0.2/pypalexcpptest/
+-rw-r--r--   0 altimofeyev   (501) staff       (20)      419 2023-04-11 21:55:37.000000 pypalexcpptest-0.0.2/pypalexcpptest/__init__.py
+-rw-r--r--   0 altimofeyev   (501) staff       (20)     7466 2023-04-11 22:04:20.000000 pypalexcpptest-0.0.2/pypalexcpptest/__main__.py
+-rw-r--r--   0 altimofeyev   (501) staff       (20)     2385 2023-03-07 02:13:31.000000 pypalexcpptest-0.0.2/pypalexcpptest/arg_messages.py
+-rw-r--r--   0 altimofeyev   (501) staff       (20)     1524 2023-04-11 21:57:06.000000 pypalexcpptest-0.0.2/pypalexcpptest/conversion_tests.py
+-rw-r--r--   0 altimofeyev   (501) staff       (20)     4342 2023-04-08 02:04:19.000000 pypalexcpptest-0.0.2/pypalexcpptest/conversion_utils.py
+-rw-r--r--   0 altimofeyev   (501) staff       (20)     2211 2023-04-11 21:57:06.000000 pypalexcpptest-0.0.2/pypalexcpptest/image_utils.py
+-rw-r--r--   0 altimofeyev   (501) staff       (20)      640 2023-04-11 22:04:32.000000 pypalexcpptest-0.0.2/pypalexcpptest/settings.py
+drwxr-xr-x   0 altimofeyev   (501) staff       (20)        0 2023-04-11 22:05:09.070279 pypalexcpptest-0.0.2/pypalexcpptest.egg-info/
+-rw-r--r--   0 altimofeyev   (501) staff       (20)     1001 2023-04-11 22:05:08.000000 pypalexcpptest-0.0.2/pypalexcpptest.egg-info/PKG-INFO
+-rw-r--r--   0 altimofeyev   (501) staff       (20)      497 2023-04-11 22:05:08.000000 pypalexcpptest-0.0.2/pypalexcpptest.egg-info/SOURCES.txt
+-rw-r--r--   0 altimofeyev   (501) staff       (20)        1 2023-04-11 22:05:08.000000 pypalexcpptest-0.0.2/pypalexcpptest.egg-info/dependency_links.txt
+-rw-r--r--   0 altimofeyev   (501) staff       (20)       63 2023-04-11 22:05:08.000000 pypalexcpptest-0.0.2/pypalexcpptest.egg-info/entry_points.txt
+-rw-r--r--   0 altimofeyev   (501) staff       (20)        1 2023-04-11 22:00:23.000000 pypalexcpptest-0.0.2/pypalexcpptest.egg-info/not-zip-safe
+-rw-r--r--   0 altimofeyev   (501) staff       (20)       22 2023-04-11 22:05:08.000000 pypalexcpptest-0.0.2/pypalexcpptest.egg-info/requires.txt
+-rw-r--r--   0 altimofeyev   (501) staff       (20)       15 2023-04-11 22:05:08.000000 pypalexcpptest-0.0.2/pypalexcpptest.egg-info/top_level.txt
+-rw-r--r--   0 altimofeyev   (501) staff       (20)       38 2023-04-11 22:05:09.070916 pypalexcpptest-0.0.2/setup.cfg
+-rw-r--r--   0 altimofeyev   (501) staff       (20)     1705 2023-04-11 21:40:12.000000 pypalexcpptest-0.0.2/setup.py
```

### Comparing `pypalexcpptest-0.0.1/PKG-INFO` & `pypalexcpptest-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pypalexcpptest
-Version: 0.0.1
+Version: 0.0.2
 Summary: Testing out pypalex with cpp code.
 Home-page: https://github.com/AlTimofeyev/pypalex_cpp_test
 Author: Al Timofeyev
 Author-email: al.timofeyev@outlook.com
 License: MIT
-Download-URL: https://github.com/AlTimofeyev/pypalex_cpp_test/archive/0.0.1.tar.gz
+Download-URL: https://github.com/AlTimofeyev/pypalex_cpp_test/archive/0.0.2.tar.gz
 Description: # pypalex_cpp_test
         Testing if cpp code can work with pypalex
         
 Keywords: python,pypalexcpptest
 Platform: UNKNOWN
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pypalexcpptest-0.0.1/pypalexcpptest/__main__.py` & `pypalexcpptest-0.0.2/pypalexcpptest/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 def handle_args():
     # Converts arguments into a dictionary: {'files': None, 'path': None, 'output': None}
     argument_parser = setup_argument_parser()
     args = vars(argument_parser.parse_args())
 
     # Check if pypalex version was requested.
     if args['version']:
-        print("pypalex ", __version__, sep="")
+        print("pypalexcpptest ", __version__, sep="")
         sys.exit()
 
     # Exit if no files/paths were provided.
     if (args['files'] is None or args['files'] == []) and args['path'] is None:
         sys.exit(argmsg.no_args_help_message())
 
     # Check either the file(s) or the file(s) in the path
```

### Comparing `pypalexcpptest-0.0.1/pypalexcpptest/arg_messages.py` & `pypalexcpptest-0.0.2/pypalexcpptest/arg_messages.py`

 * *Files identical despite different names*

### Comparing `pypalexcpptest-0.0.1/pypalexcpptest/conversion_tests.py` & `pypalexcpptest-0.0.2/pypalexcpptest/conversion_tests.py`

 * *Files identical despite different names*

### Comparing `pypalexcpptest-0.0.1/pypalexcpptest/conversion_utils.py` & `pypalexcpptest-0.0.2/pypalexcpptest/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `pypalexcpptest-0.0.1/pypalexcpptest/image_utils.py` & `pypalexcpptest-0.0.2/pypalexcpptest/image_utils.py`

 * *Files identical despite different names*

### Comparing `pypalexcpptest-0.0.1/pypalexcpptest/settings.py` & `pypalexcpptest-0.0.2/pypalexcpptest/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   @section authors Author(s)
 #   - Created by Al Timofeyev on April 11, 2023
 
 
 import os
 import platform
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __cache_version__ = "1.0.0"
 
 HOME = os.getenv("HOME", os.getenv("USERPROFILE"))
 XDG_CACHE_DIR = os.getenv("XDG_CACHE_HOME", os.path.join(HOME, ".cache"))
 XDG_CONF_DIR = os.getenv("XDG_CONFIG_HOME", os.path.join(HOME, ".config"))
 
 CACHE_DIR = os.getenv("PYPALEXCPPTEST_CACHE_DIR", os.path.join(XDG_CACHE_DIR, "palexcpptest"))
```

### Comparing `pypalexcpptest-0.0.1/pypalexcpptest.egg-info/PKG-INFO` & `pypalexcpptest-0.0.2/pypalexcpptest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pypalexcpptest
-Version: 0.0.1
+Version: 0.0.2
 Summary: Testing out pypalex with cpp code.
 Home-page: https://github.com/AlTimofeyev/pypalex_cpp_test
 Author: Al Timofeyev
 Author-email: al.timofeyev@outlook.com
 License: MIT
-Download-URL: https://github.com/AlTimofeyev/pypalex_cpp_test/archive/0.0.1.tar.gz
+Download-URL: https://github.com/AlTimofeyev/pypalex_cpp_test/archive/0.0.2.tar.gz
 Description: # pypalex_cpp_test
         Testing if cpp code can work with pypalex
         
 Keywords: python,pypalexcpptest
 Platform: UNKNOWN
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pypalexcpptest-0.0.1/setup.py` & `pypalexcpptest-0.0.2/setup.py`

 * *Files identical despite different names*

