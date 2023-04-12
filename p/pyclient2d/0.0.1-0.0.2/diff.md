# Comparing `tmp/pyclient2d-0.0.1.tar.gz` & `tmp/pyclient2d-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclient2d-0.0.1.tar", last modified: Wed Apr 12 14:09:15 2023, max compression
+gzip compressed data, was "pyclient2d-0.0.2.tar", last modified: Wed Apr 12 14:24:45 2023, max compression
```

## Comparing `pyclient2d-0.0.1.tar` & `pyclient2d-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:09:15.796245 pyclient2d-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 14:09:15.796245 pyclient2d-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:09:15.796245 pyclient2d-0.0.1/pyclient-2d/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:09:15.796245 pyclient2d-0.0.1/pyclient-2d/Client/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/pyclient-2d/Client/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/pyclient-2d/Client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:09:15.796245 pyclient2d-0.0.1/pyclient-2d/Math/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/pyclient-2d/Math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/pyclient-2d/Math/_time.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/pyclient-2d/Math/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/pyclient-2d/Math/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:09:15.796245 pyclient2d-0.0.1/pyclient-2d/Server/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/pyclient-2d/Server/Server.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/pyclient-2d/Server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:09:15.796245 pyclient2d-0.0.1/pyclient-2d/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/pyclient-2d/Shared/Engine.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/pyclient-2d/Shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/pyclient-2d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:09:15.796245 pyclient2d-0.0.1/pyclient2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 14:09:15.000000 pyclient2d-0.0.1/pyclient2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-12 14:09:15.000000 pyclient2d-0.0.1/pyclient2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:09:15.000000 pyclient2d-0.0.1/pyclient2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 14:09:15.000000 pyclient2d-0.0.1/pyclient2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 14:09:15.000000 pyclient2d-0.0.1/pyclient2d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:09:15.796245 pyclient2d-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-12 14:09:04.000000 pyclient2d-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/pyclient2d/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/pyclient2d/Client/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Client/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/pyclient2d/Math/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Math/_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Math/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Math/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/pyclient2d/Server/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Server/Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/pyclient2d/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Shared/Engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/pyclient2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 14:24:45.000000 pyclient2d-0.0.2/pyclient2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-12 14:24:45.000000 pyclient2d-0.0.2/pyclient2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:24:45.000000 pyclient2d-0.0.2/pyclient2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 14:24:45.000000 pyclient2d-0.0.2/pyclient2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 14:24:45.000000 pyclient2d-0.0.2/pyclient2d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/setup.py
```

### Comparing `pyclient2d-0.0.1/LICENSE` & `pyclient2d-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclient2d-0.0.1/PKG-INFO` & `pyclient2d-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclient2d
-Version: 0.0.1
+Version: 0.0.2
 Summary: Encapsulating game server and client into one package
 Home-page: https://github.com/Jopat2409/pyclient2d
 Author: Jopat2409
 Author-email: joantpat@gmail.com
 Keywords: python,game,client,server,engine
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pyclient2d-0.0.1/pyclient-2d/Math/vector.py` & `pyclient2d-0.0.2/pyclient2d/Math/vector.py`

 * *Files identical despite different names*

### Comparing `pyclient2d-0.0.1/pyclient-2d/Shared/Engine.py` & `pyclient2d-0.0.2/pyclient2d/Shared/Engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def run(self):
         pass
 
     def __init__(self,
                  ms_per_tick: Number = 15,
                  should_render: bool = True):
         """
-        Creates an instance of the main Engine used to power pyclient-2d
+        Creates an instance of the main Engine used to power pyclient2d
         :param ms_per_tick: Number of ms per game-tick
         :param should_render: Should this instance of the engine actually render anything?
         """
 
         self.__ms_per_tick = ms_per_tick
         self.__tickrate = float(1e3) / ms_per_tick
         self.run = self.__mainloop_norender if not should_render else self.__mainloop
```

### Comparing `pyclient2d-0.0.1/pyclient2d.egg-info/PKG-INFO` & `pyclient2d-0.0.2/pyclient2d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclient2d
-Version: 0.0.1
+Version: 0.0.2
 Summary: Encapsulating game server and client into one package
 Home-page: https://github.com/Jopat2409/pyclient2d
 Author: Jopat2409
 Author-email: joantpat@gmail.com
 Keywords: python,game,client,server,engine
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pyclient2d-0.0.1/setup.py` & `pyclient2d-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import codecs
 
 c_dir = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(c_dir, "README.md"), encoding='utf-8') as ld:
     long_description = "\n" + ld.read()
 
-VERNUM = '0.0.1'
+VERNUM = '0.0.2'
 DESC = 'Encapsulating game server and client into one package'
 
 setup(
     name='pyclient2d',
     version=VERNUM,
     author="Jopat2409",
     author_email="joantpat@gmail.com",
```

