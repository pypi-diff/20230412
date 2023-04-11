# Comparing `tmp/SIOTC-0.1.2.tar.gz` & `tmp/SIOTC-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTC-0.1.2.tar", last modified: Tue Apr 11 22:02:23 2023, max compression
+gzip compressed data, was "SIOTC-0.1.3.tar", last modified: Tue Apr 11 22:04:56 2023, max compression
```

## Comparing `SIOTC-0.1.2.tar` & `SIOTC-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 22:02:23.317084 SIOTC-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-04-11 22:02:23.300084 SIOTC-0.1.2/IOTCommon/
--rw-rw-rw-   0        0        0     1654 2023-04-11 17:33:40.000000 SIOTC-0.1.2/IOTCommon/DatabaseLayer.py
--rw-rw-rw-   0        0        0     6794 2023-04-11 17:33:00.000000 SIOTC-0.1.2/IOTCommon/Operations.py
--rw-rw-rw-   0        0        0      424 2023-04-11 21:34:03.000000 SIOTC-0.1.2/IOTCommon/__init__.py
--rw-rw-rw-   0        0        0     1335 2023-04-11 17:33:24.000000 SIOTC-0.1.2/IOTCommon/helperhttps.py
--rw-rw-rw-   0        0        0      331 2023-04-11 22:02:23.317084 SIOTC-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTC-0.1.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-11 22:02:23.315082 SIOTC-0.1.2/SIOTC.egg-info/
--rw-rw-rw-   0        0        0      331 2023-04-11 22:02:23.000000 SIOTC-0.1.2/SIOTC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-11 22:02:23.000000 SIOTC-0.1.2/SIOTC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 22:02:23.000000 SIOTC-0.1.2/SIOTC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-04-11 22:02:23.000000 SIOTC-0.1.2/SIOTC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-11 22:02:23.000000 SIOTC-0.1.2/SIOTC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 22:02:23.317084 SIOTC-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      573 2023-04-11 21:57:29.000000 SIOTC-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:04:56.071727 SIOTC-0.1.3/
+-rw-rw-rw-   0        0        0      334 2023-04-11 22:04:56.070726 SIOTC-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTC-0.1.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 22:04:56.048728 SIOTC-0.1.3/SIOTC/
+-rw-rw-rw-   0        0        0     1654 2023-04-11 17:33:40.000000 SIOTC-0.1.3/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0     6794 2023-04-11 17:33:00.000000 SIOTC-0.1.3/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      424 2023-04-11 21:34:03.000000 SIOTC-0.1.3/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     1335 2023-04-11 17:33:24.000000 SIOTC-0.1.3/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:04:56.069727 SIOTC-0.1.3/SIOTC.egg-info/
+-rw-rw-rw-   0        0        0      334 2023-04-11 22:04:55.000000 SIOTC-0.1.3/SIOTC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-04-11 22:04:55.000000 SIOTC-0.1.3/SIOTC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 22:04:55.000000 SIOTC-0.1.3/SIOTC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-04-11 22:04:55.000000 SIOTC-0.1.3/SIOTC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-11 22:04:55.000000 SIOTC-0.1.3/SIOTC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 22:04:56.071727 SIOTC-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      576 2023-04-11 22:04:45.000000 SIOTC-0.1.3/setup.py
```

### Comparing `SIOTC-0.1.2/IOTCommon/DatabaseLayer.py` & `SIOTC-0.1.3/SIOTC/DatabaseLayer.py`

 * *Files identical despite different names*

### Comparing `SIOTC-0.1.2/IOTCommon/Operations.py` & `SIOTC-0.1.3/SIOTC/Operations.py`

 * *Files identical despite different names*

### Comparing `SIOTC-0.1.2/IOTCommon/helperhttps.py` & `SIOTC-0.1.3/SIOTC/helperhttps.py`

 * *Files identical despite different names*

### Comparing `SIOTC-0.1.2/setup.py` & `SIOTC-0.1.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTC',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
-        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.10',
         'Operating System :: OS Independent',
     ],
 )
```

