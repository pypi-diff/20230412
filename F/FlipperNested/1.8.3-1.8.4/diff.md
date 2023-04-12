# Comparing `tmp/FlipperNested-1.8.3.tar.gz` & `tmp/FlipperNested-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-1.8.3.tar", last modified: Tue Apr 11 21:23:59 2023, max compression
+gzip compressed data, was "FlipperNested-1.8.4.tar", last modified: Wed Apr 12 00:25:44 2023, max compression
```

## Comparing `FlipperNested-1.8.3.tar` & `FlipperNested-1.8.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:59.364143 FlipperNested-1.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:59.360143 FlipperNested-1.8.3/FlipperNested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:59.360143 FlipperNested-1.8.3/FlipperNested/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/proto/flipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/FlipperNested/proto/storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:59.360143 FlipperNested-1.8.3/FlipperNested.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-11 21:23:59.000000 FlipperNested-1.8.3/FlipperNested.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-11 21:23:59.000000 FlipperNested-1.8.3/FlipperNested.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:23:59.000000 FlipperNested-1.8.3/FlipperNested.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 21:23:59.000000 FlipperNested-1.8.3/FlipperNested.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 21:23:59.000000 FlipperNested-1.8.3/FlipperNested.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 21:23:59.000000 FlipperNested-1.8.3/FlipperNested.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:59.364143 FlipperNested-1.8.3/NestedSolver/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/bucketsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/bucketsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/crapto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/crapto1.h
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/crypto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/library.c
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/library.h
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/parity.h
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/progress.c
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/progress.h
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/NestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-11 21:23:59.364143 FlipperNested-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 21:23:59.364143 FlipperNested-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:23:59.364143 FlipperNested-1.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 21:23:48.000000 FlipperNested-1.8.3/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:25:44.087673 FlipperNested-1.8.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:25:44.083673 FlipperNested-1.8.4/FlipperNested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/FlipperNested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/FlipperNested/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/FlipperNested/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/FlipperNested/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/FlipperNested/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:25:44.083673 FlipperNested-1.8.4/FlipperNested/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/FlipperNested/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/FlipperNested/proto/flipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/FlipperNested/proto/storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:25:44.083673 FlipperNested-1.8.4/FlipperNested.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-12 00:25:44.000000 FlipperNested-1.8.4/FlipperNested.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-12 00:25:44.000000 FlipperNested-1.8.4/FlipperNested.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 00:25:44.000000 FlipperNested-1.8.4/FlipperNested.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 00:25:44.000000 FlipperNested-1.8.4/FlipperNested.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 00:25:44.000000 FlipperNested-1.8.4/FlipperNested.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 00:25:44.000000 FlipperNested-1.8.4/FlipperNested.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:25:44.083673 FlipperNested-1.8.4/NestedSolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/NestedSolver/bucketsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/NestedSolver/bucketsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/NestedSolver/crapto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/NestedSolver/crapto1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/NestedSolver/crypto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/NestedSolver/library.c
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/NestedSolver/library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/NestedSolver/parity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/NestedSolver/progress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/NestedSolver/progress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/NestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-12 00:25:44.083673 FlipperNested-1.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 00:25:44.087673 FlipperNested-1.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:25:44.083673 FlipperNested-1.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 00:25:34.000000 FlipperNested-1.8.4/tests/test_parse.py
```

### Comparing `FlipperNested-1.8.3/FlipperNested/bridge.py` & `FlipperNested-1.8.4/FlipperNested/bridge.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/FlipperNested/cli.py` & `FlipperNested-1.8.4/FlipperNested/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 
 from FlipperNested.main import FlipperNested
 
 
 def main():
-    parser = argparse.ArgumentParser(description='Calculate keys after Nested attack')
+    parser = argparse.ArgumentParser(description='Recover keys after Nested attack')
     parser.add_argument('--uid', type=str, help='Recover only for this UID', default='')
     parser.add_argument('--progress', action='store_true', help='Show key recovery progress bar')
     parser.add_argument('--save', action='store_true', help='Debug: Save nonces/keys from Flipper')
     parser.add_argument('--file', type=argparse.FileType('r'), help='Debug: Recover keys from local .nonces file')
     parser.set_defaults(debug=False)
     args = parser.parse_args()
     flipper = FlipperNested()
```

### Comparing `FlipperNested-1.8.3/FlipperNested/main.py` & `FlipperNested-1.8.4/FlipperNested/main.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/FlipperNested/proto/flipper_pb2.py` & `FlipperNested-1.8.4/FlipperNested/proto/flipper_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/FlipperNested/proto/storage_pb2.py` & `FlipperNested-1.8.4/FlipperNested/proto/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/FlipperNested.egg-info/PKG-INFO` & `FlipperNested-1.8.4/FlipperNested.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.8.3
+Version: 1.8.4
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -37,25 +37,25 @@
 ```
 
 ## Usage
 
 ```bash
 $ FlipperNested
 Checking 12345678.nonces
-Calculating for key type A, sector 0
+Recovering key type A, sector 0
 Found 1 key(s): ['ffffffffffff']
 ...
 Found potential 32 keys, use "Check found keys" in app
 ```
 
 ```bash
 $ FlipperNested --help
 usage: FlipperNested [-h] [--uid UID] [--progress] [--save] [--file FILE]
 
-Calculate keys after Nested attack
+Recover keys after Nested attack
 
 options:
   -h, --help   show this help message and exit
   --uid UID    Recover only for this UID
   --progress   Show key recovery progress bar
   --save       Debug: Save nonces/keys from Flipper
   --file FILE  Debug: Recover keys from local .nonces file
```

### Comparing `FlipperNested-1.8.3/FlipperNested.egg-info/SOURCES.txt` & `FlipperNested-1.8.4/FlipperNested.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/LICENSE.md` & `FlipperNested-1.8.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/NestedSolver/bucketsort.c` & `FlipperNested-1.8.4/NestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/NestedSolver/bucketsort.h` & `FlipperNested-1.8.4/NestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/NestedSolver/crapto1.c` & `FlipperNested-1.8.4/NestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/NestedSolver/crapto1.h` & `FlipperNested-1.8.4/NestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/NestedSolver/crypto1.c` & `FlipperNested-1.8.4/NestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/NestedSolver/library.c` & `FlipperNested-1.8.4/NestedSolver/library.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/NestedSolver/library.h` & `FlipperNested-1.8.4/NestedSolver/library.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/NestedSolver/parity.h` & `FlipperNested-1.8.4/NestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/NestedSolver/progress.c` & `FlipperNested-1.8.4/NestedSolver/progress.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/NestedSolver/python.c` & `FlipperNested-1.8.4/NestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.8.3/PKG-INFO` & `FlipperNested-1.8.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.8.3
+Version: 1.8.4
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -37,25 +37,25 @@
 ```
 
 ## Usage
 
 ```bash
 $ FlipperNested
 Checking 12345678.nonces
-Calculating for key type A, sector 0
+Recovering key type A, sector 0
 Found 1 key(s): ['ffffffffffff']
 ...
 Found potential 32 keys, use "Check found keys" in app
 ```
 
 ```bash
 $ FlipperNested --help
 usage: FlipperNested [-h] [--uid UID] [--progress] [--save] [--file FILE]
 
-Calculate keys after Nested attack
+Recover keys after Nested attack
 
 options:
   -h, --help   show this help message and exit
   --uid UID    Recover only for this UID
   --progress   Show key recovery progress bar
   --save       Debug: Save nonces/keys from Flipper
   --file FILE  Debug: Recover keys from local .nonces file
```

### Comparing `FlipperNested-1.8.3/README.md` & `FlipperNested-1.8.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 ```
 
 ## Usage
 
 ```bash
 $ FlipperNested
 Checking 12345678.nonces
-Calculating for key type A, sector 0
+Recovering key type A, sector 0
 Found 1 key(s): ['ffffffffffff']
 ...
 Found potential 32 keys, use "Check found keys" in app
 ```
 
 ```bash
 $ FlipperNested --help
 usage: FlipperNested [-h] [--uid UID] [--progress] [--save] [--file FILE]
 
-Calculate keys after Nested attack
+Recover keys after Nested attack
 
 options:
   -h, --help   show this help message and exit
   --uid UID    Recover only for this UID
   --progress   Show key recovery progress bar
   --save       Debug: Save nonces/keys from Flipper
   --file FILE  Debug: Recover keys from local .nonces file
```

### Comparing `FlipperNested-1.8.3/setup.py` & `FlipperNested-1.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                           libraries=libraries)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FlipperNested",
-    version="1.8.3",
+    version="1.8.4",
     author="AloneLiberty",
     description="Recover keys from collected nonces",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AloneLiberty/FlipperNestedRecovery",
     entry_points={'console_scripts': ['FlipperNested = FlipperNested.cli:main']},
     install_requires=['protobuf>4', 'pyserial'],
```

### Comparing `FlipperNested-1.8.3/tests/test_calculate.py` & `FlipperNested-1.8.4/tests/test_calculate.py`

 * *Files identical despite different names*

