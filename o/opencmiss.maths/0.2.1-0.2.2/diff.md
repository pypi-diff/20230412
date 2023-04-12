# Comparing `tmp/opencmiss.maths-0.2.1.tar.gz` & `tmp/opencmiss.maths-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencmiss.maths-0.2.1.tar", last modified: Wed Apr 12 03:40:41 2023, max compression
+gzip compressed data, was "opencmiss.maths-0.2.2.tar", last modified: Wed Apr 12 21:01:07 2023, max compression
```

## Comparing `opencmiss.maths-0.2.1.tar` & `opencmiss.maths-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-12 03:40:41.801276 opencmiss.maths-0.2.1/
--rw-r--r--   0 hsor001  (1210695619) 1403514002    11357 2023-04-12 03:30:32.000000 opencmiss.maths-0.2.1/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002    13643 2023-04-12 03:40:41.800976 opencmiss.maths-0.2.1/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      180 2023-04-12 03:39:50.000000 opencmiss.maths-0.2.1/README.rst
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-12 03:40:41.800572 opencmiss.maths-0.2.1/opencmiss.maths.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002    13643 2023-04-12 03:40:41.000000 opencmiss.maths-0.2.1/opencmiss.maths.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      221 2023-04-12 03:40:41.000000 opencmiss.maths-0.2.1/opencmiss.maths.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-12 03:40:41.000000 opencmiss.maths-0.2.1/opencmiss.maths.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       13 2023-04-12 03:40:41.000000 opencmiss.maths-0.2.1/opencmiss.maths.egg-info/requires.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-12 03:40:41.000000 opencmiss.maths-0.2.1/opencmiss.maths.egg-info/top_level.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-12 03:40:41.801365 opencmiss.maths-0.2.1/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1054 2023-04-12 03:37:32.000000 opencmiss.maths-0.2.1/setup.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-12 21:01:07.331387 opencmiss.maths-0.2.2/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    11357 2023-04-12 03:30:32.000000 opencmiss.maths-0.2.2/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      744 2023-04-12 21:01:07.331165 opencmiss.maths-0.2.2/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      300 2023-04-12 21:00:33.000000 opencmiss.maths-0.2.2/README.rst
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-12 21:01:07.330843 opencmiss.maths-0.2.2/opencmiss.maths.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      744 2023-04-12 21:01:07.000000 opencmiss.maths-0.2.2/opencmiss.maths.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      221 2023-04-12 21:01:07.000000 opencmiss.maths-0.2.2/opencmiss.maths.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-12 21:01:07.000000 opencmiss.maths-0.2.2/opencmiss.maths.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       13 2023-04-12 21:01:07.000000 opencmiss.maths-0.2.2/opencmiss.maths.egg-info/requires.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-12 21:01:07.000000 opencmiss.maths-0.2.2/opencmiss.maths.egg-info/top_level.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-12 21:01:07.331465 opencmiss.maths-0.2.2/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      871 2023-04-12 20:58:18.000000 opencmiss.maths-0.2.2/setup.py
```

### Comparing `opencmiss.maths-0.2.1/LICENSE` & `opencmiss.maths-0.2.2/LICENSE`

 * *Files identical despite different names*

