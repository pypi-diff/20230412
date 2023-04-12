# Comparing `tmp/SIOTCommon-0.0.4.tar.gz` & `tmp/SIOTCommon-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTCommon-0.0.4.tar", last modified: Wed Apr 12 00:35:18 2023, max compression
+gzip compressed data, was "SIOTCommon-0.0.5.tar", last modified: Wed Apr 12 00:43:57 2023, max compression
```

## Comparing `SIOTCommon-0.0.4.tar` & `SIOTCommon-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 00:35:18.014313 SIOTCommon-0.0.4/
--rw-rw-rw-   0        0        0      339 2023-04-12 00:35:18.013315 SIOTCommon-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 00:35:17.980314 SIOTCommon-0.0.4/SIOTC/
--rw-rw-rw-   0        0        0     1654 2023-04-11 17:33:40.000000 SIOTCommon-0.0.4/SIOTC/DatabaseLayer.py
--rw-rw-rw-   0        0        0     6805 2023-04-12 00:34:59.000000 SIOTCommon-0.0.4/SIOTC/Operations.py
--rw-rw-rw-   0        0        0      427 2023-04-12 00:29:07.000000 SIOTCommon-0.0.4/SIOTC/__init__.py
--rw-rw-rw-   0        0        0     1335 2023-04-11 17:33:24.000000 SIOTCommon-0.0.4/SIOTC/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-04-12 00:35:18.012314 SIOTCommon-0.0.4/SIOTCommon.egg-info/
--rw-rw-rw-   0        0        0      339 2023-04-12 00:35:17.000000 SIOTCommon-0.0.4/SIOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-12 00:35:17.000000 SIOTCommon-0.0.4/SIOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 00:35:17.000000 SIOTCommon-0.0.4/SIOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-04-12 00:35:17.000000 SIOTCommon-0.0.4/SIOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-12 00:35:17.000000 SIOTCommon-0.0.4/SIOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 00:35:18.014313 SIOTCommon-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-04-12 00:35:13.000000 SIOTCommon-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 00:43:57.185315 SIOTCommon-0.0.5/
+-rw-rw-rw-   0        0        0      339 2023-04-12 00:43:57.184316 SIOTCommon-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 00:43:57.170315 SIOTCommon-0.0.5/SIOTC/
+-rw-rw-rw-   0        0        0     1654 2023-04-11 17:33:40.000000 SIOTCommon-0.0.5/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0     6805 2023-04-12 00:41:58.000000 SIOTCommon-0.0.5/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      427 2023-04-12 00:42:11.000000 SIOTCommon-0.0.5/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     1335 2023-04-12 00:42:05.000000 SIOTCommon-0.0.5/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-04-12 00:43:57.182315 SIOTCommon-0.0.5/SIOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-04-12 00:43:57.000000 SIOTCommon-0.0.5/SIOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-12 00:43:57.000000 SIOTCommon-0.0.5/SIOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 00:43:57.000000 SIOTCommon-0.0.5/SIOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      597 2023-04-12 00:43:57.000000 SIOTCommon-0.0.5/SIOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-12 00:43:57.000000 SIOTCommon-0.0.5/SIOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 00:43:57.185315 SIOTCommon-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-04-12 00:43:54.000000 SIOTCommon-0.0.5/setup.py
```

### Comparing `SIOTCommon-0.0.4/SIOTC/DatabaseLayer.py` & `SIOTCommon-0.0.5/SIOTC/DatabaseLayer.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.4/SIOTC/Operations.py` & `SIOTCommon-0.0.5/SIOTC/Operations.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.4/SIOTC/helperhttps.py` & `SIOTCommon-0.0.5/SIOTC/helperhttps.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.4/setup.py` & `SIOTCommon-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTCommon',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```

