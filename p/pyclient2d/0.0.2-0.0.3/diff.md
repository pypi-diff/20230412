# Comparing `tmp/pyclient2d-0.0.2.tar.gz` & `tmp/pyclient2d-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclient2d-0.0.2.tar", last modified: Wed Apr 12 14:24:45 2023, max compression
+gzip compressed data, was "pyclient2d-0.0.3.tar", last modified: Wed Apr 12 17:14:30 2023, max compression
```

## Comparing `pyclient2d-0.0.2.tar` & `pyclient2d-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/pyclient2d/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/pyclient2d/Client/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Client/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/pyclient2d/Math/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Math/_time.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Math/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Math/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/pyclient2d/Server/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Server/Server.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/pyclient2d/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Shared/Engine.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/Shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/pyclient2d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/pyclient2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 14:24:45.000000 pyclient2d-0.0.2/pyclient2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-12 14:24:45.000000 pyclient2d-0.0.2/pyclient2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:24:45.000000 pyclient2d-0.0.2/pyclient2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 14:24:45.000000 pyclient2d-0.0.2/pyclient2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 14:24:45.000000 pyclient2d-0.0.2/pyclient2d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:24:45.605651 pyclient2d-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-12 14:24:33.000000 pyclient2d-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:14:30.231467 pyclient2d-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 17:14:30.231467 pyclient2d-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:14:30.227467 pyclient2d-0.0.3/pyclient2d/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:14:30.231467 pyclient2d-0.0.3/pyclient2d/Client/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/pyclient2d/Client/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/pyclient2d/Client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:14:30.231467 pyclient2d-0.0.3/pyclient2d/Math/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/pyclient2d/Math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/pyclient2d/Math/_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/pyclient2d/Math/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/pyclient2d/Math/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:14:30.231467 pyclient2d-0.0.3/pyclient2d/Server/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/pyclient2d/Server/Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/pyclient2d/Server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:14:30.231467 pyclient2d-0.0.3/pyclient2d/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/pyclient2d/Shared/Engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/pyclient2d/Shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/pyclient2d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:14:30.227467 pyclient2d-0.0.3/pyclient2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 17:14:30.000000 pyclient2d-0.0.3/pyclient2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-12 17:14:30.000000 pyclient2d-0.0.3/pyclient2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:14:30.000000 pyclient2d-0.0.3/pyclient2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 17:14:30.000000 pyclient2d-0.0.3/pyclient2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 17:14:30.000000 pyclient2d-0.0.3/pyclient2d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:14:30.231467 pyclient2d-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-12 17:14:18.000000 pyclient2d-0.0.3/setup.py
```

### Comparing `pyclient2d-0.0.2/LICENSE` & `pyclient2d-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclient2d-0.0.2/PKG-INFO` & `pyclient2d-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclient2d
-Version: 0.0.2
+Version: 0.0.3
 Summary: Encapsulating game server and client into one package
 Home-page: https://github.com/Jopat2409/pyclient2d
 Author: Jopat2409
 Author-email: joantpat@gmail.com
 Keywords: python,game,client,server,engine
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pyclient2d-0.0.2/pyclient2d/Math/vector.py` & `pyclient2d-0.0.3/pyclient2d/Math/vector.py`

 * *Files identical despite different names*

### Comparing `pyclient2d-0.0.2/pyclient2d/Shared/Engine.py` & `pyclient2d-0.0.3/pyclient2d/Shared/Engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,16 +43,17 @@
         """"""
         lag = 0.0
         updates, frames = 0, 0
         prev_time = get_system_time()
         while self.__running:
             current_time = get_system_time()
             lag += time_between(prev_time, current_time)
-            while lag <= self.__ms_per_tick:
+            while lag >= self.__ms_per_tick:
                 self.update()
+                lag -= self.__ms_per_tick
                 updates += 1
                 if self.__tickbase % int(self.__tickrate) == 0:
                     print(f"Frames: {frames}")
                     print(f"Ticks: {updates}")
                     frames, updates = 0, 0
             self.render()
             frames += 1
```

### Comparing `pyclient2d-0.0.2/pyclient2d.egg-info/PKG-INFO` & `pyclient2d-0.0.3/pyclient2d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclient2d
-Version: 0.0.2
+Version: 0.0.3
 Summary: Encapsulating game server and client into one package
 Home-page: https://github.com/Jopat2409/pyclient2d
 Author: Jopat2409
 Author-email: joantpat@gmail.com
 Keywords: python,game,client,server,engine
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pyclient2d-0.0.2/setup.py` & `pyclient2d-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import codecs
 
 c_dir = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(c_dir, "README.md"), encoding='utf-8') as ld:
     long_description = "\n" + ld.read()
 
-VERNUM = '0.0.2'
+VERNUM = '0.0.3'
 DESC = 'Encapsulating game server and client into one package'
 
 setup(
     name='pyclient2d',
     version=VERNUM,
     author="Jopat2409",
     author_email="joantpat@gmail.com",
```

