# Comparing `tmp/nheri_simcenter-0.9.6.tar.gz` & `tmp/nheri_simcenter-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nheri_simcenter-0.9.6.tar", last modified: Sat Apr  8 16:02:33 2023, max compression
+gzip compressed data, was "nheri_simcenter-0.9.7.tar", last modified: Wed Apr 12 17:34:22 2023, max compression
```

## Comparing `nheri_simcenter-0.9.6.tar` & `nheri_simcenter-0.9.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-08 16:02:33.849426 nheri_simcenter-0.9.6/
--rw-r--r--   0 adamzs     (504) staff       (20)     1669 2021-01-11 23:23:41.000000 nheri_simcenter-0.9.6/LICENSE
--rw-r--r--   0 adamzs     (504) staff       (20)     2071 2023-04-08 16:02:33.849305 nheri_simcenter-0.9.6/PKG-INFO
--rw-r--r--   0 adamzs     (504) staff       (20)     1051 2021-01-11 23:36:45.000000 nheri_simcenter-0.9.6/README.md
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-08 16:02:33.848450 nheri_simcenter-0.9.6/nheri_simcenter/
--rw-r--r--   0 adamzs     (504) staff       (20)     2116 2023-04-07 16:38:43.000000 nheri_simcenter-0.9.6/nheri_simcenter/__init__.py
-drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-08 16:02:33.849119 nheri_simcenter-0.9.6/nheri_simcenter.egg-info/
--rw-r--r--   0 adamzs     (504) staff       (20)     2071 2023-04-08 16:02:33.000000 nheri_simcenter-0.9.6/nheri_simcenter.egg-info/PKG-INFO
--rw-r--r--   0 adamzs     (504) staff       (20)      248 2023-04-08 16:02:33.000000 nheri_simcenter-0.9.6/nheri_simcenter.egg-info/SOURCES.txt
--rw-r--r--   0 adamzs     (504) staff       (20)        1 2023-04-08 16:02:33.000000 nheri_simcenter-0.9.6/nheri_simcenter.egg-info/dependency_links.txt
--rw-r--r--   0 adamzs     (504) staff       (20)      132 2023-04-08 16:02:33.000000 nheri_simcenter-0.9.6/nheri_simcenter.egg-info/requires.txt
--rw-r--r--   0 adamzs     (504) staff       (20)       16 2023-04-08 16:02:33.000000 nheri_simcenter-0.9.6/nheri_simcenter.egg-info/top_level.txt
--rw-r--r--   0 adamzs     (504) staff       (20)       38 2023-04-08 16:02:33.849467 nheri_simcenter-0.9.6/setup.cfg
--rw-r--r--   0 adamzs     (504) staff       (20)     2003 2023-04-08 16:00:08.000000 nheri_simcenter-0.9.6/setup.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-12 17:34:22.043329 nheri_simcenter-0.9.7/
+-rw-r--r--   0 adamzs     (504) staff       (20)     1669 2021-01-11 23:23:41.000000 nheri_simcenter-0.9.7/LICENSE
+-rw-r--r--   0 adamzs     (504) staff       (20)     2071 2023-04-12 17:34:22.043160 nheri_simcenter-0.9.7/PKG-INFO
+-rw-r--r--   0 adamzs     (504) staff       (20)     1051 2021-01-11 23:36:45.000000 nheri_simcenter-0.9.7/README.md
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-12 17:34:22.041941 nheri_simcenter-0.9.7/nheri_simcenter/
+-rw-r--r--   0 adamzs     (504) staff       (20)     2116 2023-04-12 17:32:46.000000 nheri_simcenter-0.9.7/nheri_simcenter/__init__.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2023-04-12 17:34:22.042891 nheri_simcenter-0.9.7/nheri_simcenter.egg-info/
+-rw-r--r--   0 adamzs     (504) staff       (20)     2071 2023-04-12 17:34:22.000000 nheri_simcenter-0.9.7/nheri_simcenter.egg-info/PKG-INFO
+-rw-r--r--   0 adamzs     (504) staff       (20)      248 2023-04-12 17:34:22.000000 nheri_simcenter-0.9.7/nheri_simcenter.egg-info/SOURCES.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)        1 2023-04-12 17:34:22.000000 nheri_simcenter-0.9.7/nheri_simcenter.egg-info/dependency_links.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)      145 2023-04-12 17:34:22.000000 nheri_simcenter-0.9.7/nheri_simcenter.egg-info/requires.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       16 2023-04-12 17:34:22.000000 nheri_simcenter-0.9.7/nheri_simcenter.egg-info/top_level.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       38 2023-04-12 17:34:22.043374 nheri_simcenter-0.9.7/setup.cfg
+-rw-r--r--   0 adamzs     (504) staff       (20)     2028 2023-04-12 17:32:32.000000 nheri_simcenter-0.9.7/setup.py
```

### Comparing `nheri_simcenter-0.9.6/LICENSE` & `nheri_simcenter-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nheri_simcenter-0.9.6/PKG-INFO` & `nheri_simcenter-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nheri_simcenter
-Version: 0.9.6
+Version: 0.9.7
 Summary: NHERI SimCenter Python Dependencies
 Home-page: http://nheri-simcenter.github.io/nheri_simcenter/
 Author: Adam Zsarnóczay
 Author-email: adamzs@stanford.edu
 License: BSD License
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `nheri_simcenter-0.9.6/README.md` & `nheri_simcenter-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `nheri_simcenter-0.9.6/nheri_simcenter/__init__.py` & `nheri_simcenter-0.9.7/nheri_simcenter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 # nheri_simcenter. If not, see <http://www.opensource.org/licenses/>.
 #
 # Contributors:
 # Adam Zsarnóczay
 
 name = "nheri_simcenter"
 
-__version__ = '0.9.6'
+__version__ = '0.9.7'
 
 __copyright__ = """Copyright (c) 2018 Leland Stanford Junior University and
 The Regents of the University of California"""
 
 __license__ = "BSD 3-Clause License"
```

### Comparing `nheri_simcenter-0.9.6/nheri_simcenter.egg-info/PKG-INFO` & `nheri_simcenter-0.9.7/nheri_simcenter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nheri-simcenter
-Version: 0.9.6
+Version: 0.9.7
 Summary: NHERI SimCenter Python Dependencies
 Home-page: http://nheri-simcenter.github.io/nheri_simcenter/
 Author: Adam Zsarnóczay
 Author-email: adamzs@stanford.edu
 License: BSD License
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `nheri_simcenter-0.9.6/setup.py` & `nheri_simcenter-0.9.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         'numpy>=1.23.5, <2.0',
         'scipy>=1.9.3, <2.0',
         'pandas>=1.5.2, <2.0',
         'openpyxl',
         'tables',
         'openseespy',
         'sklearn',
+        'scikit-learn',
         'jpype1',
         'tqdm',
         'gpy',
         'emukit'
     ],
     classifiers = [
         'Programming Language :: Python',
```

