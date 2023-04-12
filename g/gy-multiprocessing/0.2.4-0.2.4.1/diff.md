# Comparing `tmp/gy_multiprocessing-0.2.4.tar.gz` & `tmp/gy_multiprocessing-0.2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gy_multiprocessing-0.2.4.tar", last modified: Wed Feb 22 11:55:59 2023, max compression
+gzip compressed data, was "gy_multiprocessing-0.2.4.1.tar", last modified: Wed Apr 12 09:25:36 2023, max compression
```

## Comparing `gy_multiprocessing-0.2.4.tar` & `gy_multiprocessing-0.2.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-02-22 11:55:59.378770 gy_multiprocessing-0.2.4/
--rw-r--r--   0 guangyuhe   (501) staff       (20)     6318 2023-02-22 11:55:59.378652 gy_multiprocessing-0.2.4/PKG-INFO
--rw-r--r--   0 guangyuhe   (501) staff       (20)     5900 2023-02-22 11:53:09.000000 gy_multiprocessing-0.2.4/README.md
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-02-22 11:55:59.377266 gy_multiprocessing-0.2.4/gy_multiprocessing/
--rw-r--r--   0 guangyuhe   (501) staff       (20)      138 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4/gy_multiprocessing/__init__.py
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-02-22 11:55:59.378131 gy_multiprocessing-0.2.4/gy_multiprocessing/multiprocessing/
--rw-r--r--   0 guangyuhe   (501) staff       (20)       61 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4/gy_multiprocessing/multiprocessing/__init__.py
--rw-r--r--   0 guangyuhe   (501) staff       (20)     6997 2023-02-22 11:48:10.000000 gy_multiprocessing-0.2.4/gy_multiprocessing/multiprocessing/multi_process.py
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-02-22 11:55:59.378469 gy_multiprocessing-0.2.4/gy_multiprocessing/multithreading/
--rw-r--r--   0 guangyuhe   (501) staff       (20)       59 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4/gy_multiprocessing/multithreading/__init__.py
--rw-r--r--   0 guangyuhe   (501) staff       (20)     2289 2023-02-22 11:22:12.000000 gy_multiprocessing-0.2.4/gy_multiprocessing/multithreading/multi_thread.py
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-02-22 11:55:59.377788 gy_multiprocessing-0.2.4/gy_multiprocessing.egg-info/
--rw-r--r--   0 guangyuhe   (501) staff       (20)     6318 2023-02-22 11:55:59.000000 gy_multiprocessing-0.2.4/gy_multiprocessing.egg-info/PKG-INFO
--rw-r--r--   0 guangyuhe   (501) staff       (20)      412 2023-02-22 11:55:59.000000 gy_multiprocessing-0.2.4/gy_multiprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)        1 2023-02-22 11:55:59.000000 gy_multiprocessing-0.2.4/gy_multiprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)       19 2023-02-22 11:55:59.000000 gy_multiprocessing-0.2.4/gy_multiprocessing.egg-info/top_level.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)       38 2023-02-22 11:55:59.378806 gy_multiprocessing-0.2.4/setup.cfg
--rw-r--r--   0 guangyuhe   (501) staff       (20)      727 2023-02-22 11:13:44.000000 gy_multiprocessing-0.2.4/setup.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 09:25:36.506688 gy_multiprocessing-0.2.4.1/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     6427 2023-04-12 09:25:36.506567 gy_multiprocessing-0.2.4.1/PKG-INFO
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     6007 2023-04-12 09:25:12.000000 gy_multiprocessing-0.2.4.1/README.md
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 09:25:36.505523 gy_multiprocessing-0.2.4.1/gy_multiprocessing/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      138 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing/__init__.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 09:25:36.506183 gy_multiprocessing-0.2.4.1/gy_multiprocessing/multiprocessing/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       61 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing/multiprocessing/__init__.py
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     7090 2023-04-12 09:23:13.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing/multiprocessing/multi_process.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 09:25:36.506401 gy_multiprocessing-0.2.4.1/gy_multiprocessing/multithreading/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       59 2023-02-22 09:46:14.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing/multithreading/__init__.py
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     2289 2023-02-22 11:22:12.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing/multithreading/multi_thread.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 09:25:36.505954 gy_multiprocessing-0.2.4.1/gy_multiprocessing.egg-info/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     6427 2023-04-12 09:25:36.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      412 2023-04-12 09:25:36.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)        1 2023-04-12 09:25:36.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       19 2023-04-12 09:25:36.000000 gy_multiprocessing-0.2.4.1/gy_multiprocessing.egg-info/top_level.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       38 2023-04-12 09:25:36.506723 gy_multiprocessing-0.2.4.1/setup.cfg
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      792 2023-04-12 09:24:19.000000 gy_multiprocessing-0.2.4.1/setup.py
```

### Comparing `gy_multiprocessing-0.2.4/PKG-INFO` & `gy_multiprocessing-0.2.4.1/gy_multiprocessing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gy_multiprocessing
-Version: 0.2.4
+Name: gy-multiprocessing
+Version: 0.2.4.1
 Summary: Run function in multiple processes
 Home-page: https://github.com/guangyu-he/gy-multiprocessing
 Author: Guangyu He
 Author-email: me@heguangyu.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -220,24 +220,32 @@
 
 ### v0.2.3
 
 #### bug fix
 
 - fixed an issue casing not adding new process to pool until all processed are done in current pool
 
-feel free to check source code in <a href="https://github.com/guangyu-he/gy-multiprocessing">GitHub</a>, you are welcome
-to leave any comments.
-
 ### v0.2.4
 
 #### feature
 
 - a silent mode is added to multiprocessing which is possible not showing messages in console
 - solved multiprocessing not going to the end when there are internal error exceptions in input function
 - solved multiprocessing not going to the end when there are missing queue.put() method in input function
 
+### v0.2.4.1
+
+#### bug fix
+
+- fixed an issue from readme long desc causing installation error
+
 #### improvement
 
 - simplified duplicated codes
 
+## Support
+
+feel free to check source code in <a href="https://github.com/guangyu-he/gy-multiprocessing">GitHub</a>, you are welcome
+to leave any comments.
+
 2022&copy;Guangyu He, for further support please contact author. <br>
 Email: <a href="mailto:me@heguangyu.net">me@heguangyu.net</a>
```

### Comparing `gy_multiprocessing-0.2.4/README.md` & `gy_multiprocessing-0.2.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -207,24 +207,32 @@
 
 ### v0.2.3
 
 #### bug fix
 
 - fixed an issue casing not adding new process to pool until all processed are done in current pool
 
-feel free to check source code in <a href="https://github.com/guangyu-he/gy-multiprocessing">GitHub</a>, you are welcome
-to leave any comments.
-
 ### v0.2.4
 
 #### feature
 
 - a silent mode is added to multiprocessing which is possible not showing messages in console
 - solved multiprocessing not going to the end when there are internal error exceptions in input function
 - solved multiprocessing not going to the end when there are missing queue.put() method in input function
 
+### v0.2.4.1
+
+#### bug fix
+
+- fixed an issue from readme long desc causing installation error
+
 #### improvement
 
 - simplified duplicated codes
 
+## Support
+
+feel free to check source code in <a href="https://github.com/guangyu-he/gy-multiprocessing">GitHub</a>, you are welcome
+to leave any comments.
+
 2022&copy;Guangyu He, for further support please contact author. <br>
 Email: <a href="mailto:me@heguangyu.net">me@heguangyu.net</a>
```

### Comparing `gy_multiprocessing-0.2.4/gy_multiprocessing/multiprocessing/multi_process.py` & `gy_multiprocessing-0.2.4.1/gy_multiprocessing/multiprocessing/multi_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+# loading multiprocessing package
 from multiprocessing import Process, cpu_count, get_context
+
+# importing relevant types
 from multiprocessing.context import Process as ProcessType
-import time
 from types import FunctionType, MethodType
+
+# importing necessary modules
+import time
 import warnings
 
 
 class MultiProcess:
 
     def __init__(self, max_process: int = cpu_count(), silent: bool = False):
         """
```

### Comparing `gy_multiprocessing-0.2.4/gy_multiprocessing/multithreading/multi_thread.py` & `gy_multiprocessing-0.2.4.1/gy_multiprocessing/multithreading/multi_thread.py`

 * *Files identical despite different names*

### Comparing `gy_multiprocessing-0.2.4/gy_multiprocessing.egg-info/PKG-INFO` & `gy_multiprocessing-0.2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gy-multiprocessing
-Version: 0.2.4
+Name: gy_multiprocessing
+Version: 0.2.4.1
 Summary: Run function in multiple processes
 Home-page: https://github.com/guangyu-he/gy-multiprocessing
 Author: Guangyu He
 Author-email: me@heguangyu.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -220,24 +220,32 @@
 
 ### v0.2.3
 
 #### bug fix
 
 - fixed an issue casing not adding new process to pool until all processed are done in current pool
 
-feel free to check source code in <a href="https://github.com/guangyu-he/gy-multiprocessing">GitHub</a>, you are welcome
-to leave any comments.
-
 ### v0.2.4
 
 #### feature
 
 - a silent mode is added to multiprocessing which is possible not showing messages in console
 - solved multiprocessing not going to the end when there are internal error exceptions in input function
 - solved multiprocessing not going to the end when there are missing queue.put() method in input function
 
+### v0.2.4.1
+
+#### bug fix
+
+- fixed an issue from readme long desc causing installation error
+
 #### improvement
 
 - simplified duplicated codes
 
+## Support
+
+feel free to check source code in <a href="https://github.com/guangyu-he/gy-multiprocessing">GitHub</a>, you are welcome
+to leave any comments.
+
 2022&copy;Guangyu He, for further support please contact author. <br>
 Email: <a href="mailto:me@heguangyu.net">me@heguangyu.net</a>
```

### Comparing `gy_multiprocessing-0.2.4/setup.py` & `gy_multiprocessing-0.2.4.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
+from pathlib import Path
 
-with open('README.md') as fh:
-    long_description = fh.read()
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="gy_multiprocessing",
-    version="0.2.4",
+    version="0.2.4.1",
     author="Guangyu He",
     author_email="me@heguangyu.net",
     description="Run function in multiple processes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/guangyu-he/gy-multiprocessing",
     install_requires=[],
```

