# Comparing `tmp/pyclient-2d-0.0.1.tar.gz` & `tmp/pyclient-2d-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclient-2d-0.0.1.tar", last modified: Wed Apr 12 13:57:12 2023, max compression
+gzip compressed data, was "pyclient-2d-0.0.3.tar", last modified: Wed Apr 12 14:00:13 2023, max compression
```

## Comparing `pyclient-2d-0.0.1.tar` & `pyclient-2d-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:57:12.137845 pyclient-2d-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-12 13:57:12.137845 pyclient-2d-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:57:12.133844 pyclient-2d-0.0.1/pyclient-2d/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:57:12.133844 pyclient-2d-0.0.1/pyclient-2d/Client/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/pyclient-2d/Client/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/pyclient-2d/Client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:57:12.137845 pyclient-2d-0.0.1/pyclient-2d/Math/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/pyclient-2d/Math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/pyclient-2d/Math/_time.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/pyclient-2d/Math/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/pyclient-2d/Math/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:57:12.137845 pyclient-2d-0.0.1/pyclient-2d/Server/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/pyclient-2d/Server/Server.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/pyclient-2d/Server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:57:12.137845 pyclient-2d-0.0.1/pyclient-2d/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/pyclient-2d/Shared/Engine.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/pyclient-2d/Shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/pyclient-2d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:57:12.137845 pyclient-2d-0.0.1/pyclient_2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-12 13:57:12.000000 pyclient-2d-0.0.1/pyclient_2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-12 13:57:12.000000 pyclient-2d-0.0.1/pyclient_2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:57:12.000000 pyclient-2d-0.0.1/pyclient_2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 13:57:12.000000 pyclient-2d-0.0.1/pyclient_2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 13:57:12.000000 pyclient-2d-0.0.1/pyclient_2d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 13:57:12.137845 pyclient-2d-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-12 13:57:02.000000 pyclient-2d-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:00:13.936820 pyclient-2d-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-12 14:00:13.936820 pyclient-2d-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:00:13.936820 pyclient-2d-0.0.3/pyclient-2d/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:00:13.936820 pyclient-2d-0.0.3/pyclient-2d/Client/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/pyclient-2d/Client/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/pyclient-2d/Client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:00:13.936820 pyclient-2d-0.0.3/pyclient-2d/Math/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/pyclient-2d/Math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/pyclient-2d/Math/_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/pyclient-2d/Math/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/pyclient-2d/Math/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:00:13.936820 pyclient-2d-0.0.3/pyclient-2d/Server/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/pyclient-2d/Server/Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/pyclient-2d/Server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:00:13.936820 pyclient-2d-0.0.3/pyclient-2d/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/pyclient-2d/Shared/Engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/pyclient-2d/Shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/pyclient-2d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:00:13.936820 pyclient-2d-0.0.3/pyclient_2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-12 14:00:13.000000 pyclient-2d-0.0.3/pyclient_2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-12 14:00:13.000000 pyclient-2d-0.0.3/pyclient_2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:00:13.000000 pyclient-2d-0.0.3/pyclient_2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 14:00:13.000000 pyclient-2d-0.0.3/pyclient_2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 14:00:13.000000 pyclient-2d-0.0.3/pyclient_2d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:00:13.936820 pyclient-2d-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-12 14:00:03.000000 pyclient-2d-0.0.3/setup.py
```

### Comparing `pyclient-2d-0.0.1/LICENSE` & `pyclient-2d-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclient-2d-0.0.1/pyclient-2d/Math/vector.py` & `pyclient-2d-0.0.3/pyclient-2d/Math/vector.py`

 * *Files identical despite different names*

### Comparing `pyclient-2d-0.0.1/pyclient-2d/Shared/Engine.py` & `pyclient-2d-0.0.3/pyclient-2d/Shared/Engine.py`

 * *Files identical despite different names*

### Comparing `pyclient-2d-0.0.1/pyclient_2d.egg-info/SOURCES.txt` & `pyclient-2d-0.0.3/pyclient_2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyclient-2d-0.0.1/setup.py` & `pyclient-2d-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 import codecs
 
 c_dir = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(c_dir, "README.md"), encoding='utf-8') as ld:
     long_description = "\n" + ld.read()
 
-VERNUM = '0.0.1'
+VERNUM = '0.0.3'
 DESC = 'Encapsulating game server and client into one package'
 
 setup(
     name='pyclient-2d',
     version=VERNUM,
     author="Jopat2409",
     author_email="joantpat@gmail.com",
     description=DESC,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['pygame', 'socket'],
+    install_requires=['pygame'],
     keywords=['python', 'game', 'client', 'server', 'engine'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows"
     ]
```

