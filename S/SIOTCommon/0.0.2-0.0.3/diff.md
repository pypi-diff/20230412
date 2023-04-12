# Comparing `tmp/SIOTCommon-0.0.2.tar.gz` & `tmp/SIOTCommon-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTCommon-0.0.2.tar", last modified: Tue Apr 11 23:30:34 2023, max compression
+gzip compressed data, was "SIOTCommon-0.0.3.tar", last modified: Wed Apr 12 00:29:43 2023, max compression
```

## Comparing `SIOTCommon-0.0.2.tar` & `SIOTCommon-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 23:30:34.971308 SIOTCommon-0.0.2/
--rw-rw-rw-   0        0        0      339 2023-04-11 23:30:34.970308 SIOTCommon-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-11 23:30:34.957307 SIOTCommon-0.0.2/SIOTC/
--rw-rw-rw-   0        0        0     1654 2023-04-11 17:33:40.000000 SIOTCommon-0.0.2/SIOTC/DatabaseLayer.py
--rw-rw-rw-   0        0        0     6794 2023-04-11 17:33:00.000000 SIOTCommon-0.0.2/SIOTC/Operations.py
--rw-rw-rw-   0        0        0      424 2023-04-11 21:34:03.000000 SIOTCommon-0.0.2/SIOTC/__init__.py
--rw-rw-rw-   0        0        0     1335 2023-04-11 17:33:24.000000 SIOTCommon-0.0.2/SIOTC/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-04-11 23:30:34.969311 SIOTCommon-0.0.2/SIOTCommon.egg-info/
--rw-rw-rw-   0        0        0      339 2023-04-11 23:30:34.000000 SIOTCommon-0.0.2/SIOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-11 23:30:34.000000 SIOTCommon-0.0.2/SIOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 23:30:34.000000 SIOTCommon-0.0.2/SIOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-04-11 23:30:34.000000 SIOTCommon-0.0.2/SIOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-11 23:30:34.000000 SIOTCommon-0.0.2/SIOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 23:30:34.971308 SIOTCommon-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-04-11 23:30:30.000000 SIOTCommon-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 00:29:43.451445 SIOTCommon-0.0.3/
+-rw-rw-rw-   0        0        0      339 2023-04-12 00:29:43.451445 SIOTCommon-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 00:29:43.425448 SIOTCommon-0.0.3/SIOTC/
+-rw-rw-rw-   0        0        0     1654 2023-04-11 17:33:40.000000 SIOTCommon-0.0.3/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0     6794 2023-04-11 17:33:00.000000 SIOTCommon-0.0.3/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      427 2023-04-12 00:29:07.000000 SIOTCommon-0.0.3/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     1335 2023-04-11 17:33:24.000000 SIOTCommon-0.0.3/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-04-12 00:29:43.449451 SIOTCommon-0.0.3/SIOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-04-12 00:29:43.000000 SIOTCommon-0.0.3/SIOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-12 00:29:43.000000 SIOTCommon-0.0.3/SIOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 00:29:43.000000 SIOTCommon-0.0.3/SIOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-04-12 00:29:43.000000 SIOTCommon-0.0.3/SIOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-12 00:29:43.000000 SIOTCommon-0.0.3/SIOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 00:29:43.451445 SIOTCommon-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-04-12 00:29:13.000000 SIOTCommon-0.0.3/setup.py
```

### Comparing `SIOTCommon-0.0.2/SIOTC/DatabaseLayer.py` & `SIOTCommon-0.0.3/SIOTC/DatabaseLayer.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.2/SIOTC/Operations.py` & `SIOTCommon-0.0.3/SIOTC/Operations.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.2/SIOTC/helperhttps.py` & `SIOTCommon-0.0.3/SIOTC/helperhttps.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.2/setup.py` & `SIOTCommon-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTCommon',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```

