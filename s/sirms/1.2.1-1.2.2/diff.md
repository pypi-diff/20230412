# Comparing `tmp/sirms-1.2.1.tar.gz` & `tmp/sirms-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sirms-1.2.1.tar", last modified: Mon Feb  8 10:06:17 2021, max compression
+gzip compressed data, was "dist/sirms-1.2.2.tar", last modified: Wed Apr 12 07:34:35 2023, max compression
```

## Comparing `sirms-1.2.1.tar` & `sirms-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2021-02-08 10:06:17.000000 sirms-1.2.1/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4409 2021-02-08 10:06:17.000000 sirms-1.2.1/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2021-02-08 10:06:17.000000 sirms-1.2.1/setup.cfg
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2021-02-08 10:06:17.000000 sirms-1.2.1/sirms/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     8191 2021-02-06 20:25:34.000000 sirms-1.2.1/sirms/canon.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10316 2021-02-06 20:25:34.000000 sirms-1.2.1/sirms/mols.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5394 2021-02-06 20:25:34.000000 sirms-1.2.1/sirms/labels.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      861 2021-02-06 19:35:37.000000 sirms-1.2.1/sirms/ppgfunctions.py
--rwxrwxr-x   0 pavel     (1000) pavel     (1000)    33791 2021-02-06 20:25:34.000000 sirms-1.2.1/sirms/sirms.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11502 2021-02-06 20:25:34.000000 sirms-1.2.1/sirms/sdf.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1118 2021-02-06 19:35:37.000000 sirms-1.2.1/sirms/sirms_name.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     8211 2021-02-06 20:25:34.000000 sirms-1.2.1/sirms/files.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       21 2021-02-08 10:00:14.000000 sirms-1.2.1/sirms/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3255 2021-02-08 10:01:15.000000 sirms-1.2.1/README.md
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2021-02-08 10:06:17.000000 sirms-1.2.1/sirms.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4409 2021-02-08 10:06:17.000000 sirms-1.2.1/sirms.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      352 2021-02-08 10:06:17.000000 sirms-1.2.1/sirms.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      131 2021-02-08 10:06:17.000000 sirms-1.2.1/sirms.egg-info/entry_points.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        6 2021-02-08 10:06:17.000000 sirms-1.2.1/sirms.egg-info/top_level.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2021-02-08 10:06:17.000000 sirms-1.2.1/sirms.egg-info/requires.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2021-02-08 10:06:17.000000 sirms-1.2.1/sirms.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1160 2021-02-06 19:29:33.000000 sirms-1.2.1/setup.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-12 07:34:35.000000 sirms-1.2.2/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4487 2023-04-12 07:34:35.000000 sirms-1.2.2/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2023-04-12 07:34:35.000000 sirms-1.2.2/setup.cfg
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8191 2021-02-06 20:25:34.000000 sirms-1.2.2/sirms/canon.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10316 2021-02-06 20:25:34.000000 sirms-1.2.2/sirms/mols.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5394 2021-02-06 20:25:34.000000 sirms-1.2.2/sirms/labels.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      861 2021-02-06 19:35:37.000000 sirms-1.2.2/sirms/ppgfunctions.py
+-rwxrwxr-x   0 pavel     (1000) pavel     (1000)    33791 2021-02-06 20:25:34.000000 sirms-1.2.2/sirms/sirms.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    11502 2021-02-06 20:25:34.000000 sirms-1.2.2/sirms/sdf.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1118 2021-02-06 19:35:37.000000 sirms-1.2.2/sirms/sirms_name.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8211 2021-02-06 20:25:34.000000 sirms-1.2.2/sirms/files.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       21 2023-04-12 07:32:40.000000 sirms-1.2.2/sirms/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3301 2023-04-12 07:32:39.000000 sirms-1.2.2/README.md
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4487 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      352 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      131 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/entry_points.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        6 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/top_level.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/requires.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-04-12 07:34:35.000000 sirms-1.2.2/sirms.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1160 2021-02-06 19:29:33.000000 sirms-1.2.2/setup.py
```

### Comparing `sirms-1.2.1/PKG-INFO` & `sirms-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirms
-Version: 1.2.1
+Version: 1.2.2
 Summary: SiRMS: simplex representation of molecular structure
 Home-page: https://github.com/DrrDom/sirms
 Author: Pavel Polishchuk
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # SiRMS
         
@@ -28,23 +28,23 @@
         
         #### Installation
         
         `pip install sirms`
         
         #### Usage
         Returns 2D simplex descriptors with vertexes labeled by element for single compounds  
-        `sirms.py -in input.sdf -o output.txt`  
+        `sirms -in input.sdf -o output.txt`  
         Returns 2D simplex descriptors with vertexes labeled by element for reactions  
-        `sirms.py -in input.rdf -o output.txt`  
+        `sirms -in input.rdf -o output.txt`  
         
         #### Help
         
-        `sirms.py -h`
+        `sirms -h`
         
-        ####Wiki
+        #### Wiki
         
         See wiki pages for more information and examples - https://github.com/DrrDom/sirms/wiki.
         
         #### Notes
         
         Standardize structures before descriptors calculation.
         
@@ -70,14 +70,18 @@
         - per atom fragmentation was added
         
         version 1.2.0 (06.02.2021)
         - reorganized as a Python package
         
         version 1.2.1 (08.02.2021)
         - fix README formatting
+        
+        version 1.2.2 (12.04.2023)
+        - fix examples in README
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.6
```

### Comparing `sirms-1.2.1/sirms/canon.py` & `sirms-1.2.2/sirms/canon.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.1/sirms/mols.py` & `sirms-1.2.2/sirms/mols.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.1/sirms/labels.py` & `sirms-1.2.2/sirms/labels.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.1/sirms/ppgfunctions.py` & `sirms-1.2.2/sirms/ppgfunctions.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.1/sirms/sirms.py` & `sirms-1.2.2/sirms/sirms.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.1/sirms/sdf.py` & `sirms-1.2.2/sirms/sdf.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.1/sirms/sirms_name.py` & `sirms-1.2.2/sirms/sirms_name.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.1/sirms/files.py` & `sirms-1.2.2/sirms/files.py`

 * *Files identical despite different names*

### Comparing `sirms-1.2.1/README.md` & `sirms-1.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 
 #### Installation
 
 `pip install sirms`
 
 #### Usage
 Returns 2D simplex descriptors with vertexes labeled by element for single compounds  
-`sirms.py -in input.sdf -o output.txt`  
+`sirms -in input.sdf -o output.txt`  
 Returns 2D simplex descriptors with vertexes labeled by element for reactions  
-`sirms.py -in input.rdf -o output.txt`  
+`sirms -in input.rdf -o output.txt`  
 
 #### Help
 
-`sirms.py -h`
+`sirms -h`
 
-####Wiki
+#### Wiki
 
 See wiki pages for more information and examples - https://github.com/DrrDom/sirms/wiki.
 
 #### Notes
 
 Standardize structures before descriptors calculation.
 
@@ -61,8 +61,11 @@
 - multiprocessing calculation of descriptors was implemented for single molecules and svm output format only (sparse format)
 - per atom fragmentation was added
 
 version 1.2.0 (06.02.2021)
 - reorganized as a Python package
 
 version 1.2.1 (08.02.2021)
-- fix README formatting
+- fix README formatting
+
+version 1.2.2 (12.04.2023)
+- fix examples in README
```

### Comparing `sirms-1.2.1/sirms.egg-info/PKG-INFO` & `sirms-1.2.2/sirms.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirms
-Version: 1.2.1
+Version: 1.2.2
 Summary: SiRMS: simplex representation of molecular structure
 Home-page: https://github.com/DrrDom/sirms
 Author: Pavel Polishchuk
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # SiRMS
         
@@ -28,23 +28,23 @@
         
         #### Installation
         
         `pip install sirms`
         
         #### Usage
         Returns 2D simplex descriptors with vertexes labeled by element for single compounds  
-        `sirms.py -in input.sdf -o output.txt`  
+        `sirms -in input.sdf -o output.txt`  
         Returns 2D simplex descriptors with vertexes labeled by element for reactions  
-        `sirms.py -in input.rdf -o output.txt`  
+        `sirms -in input.rdf -o output.txt`  
         
         #### Help
         
-        `sirms.py -h`
+        `sirms -h`
         
-        ####Wiki
+        #### Wiki
         
         See wiki pages for more information and examples - https://github.com/DrrDom/sirms/wiki.
         
         #### Notes
         
         Standardize structures before descriptors calculation.
         
@@ -70,14 +70,18 @@
         - per atom fragmentation was added
         
         version 1.2.0 (06.02.2021)
         - reorganized as a Python package
         
         version 1.2.1 (08.02.2021)
         - fix README formatting
+        
+        version 1.2.2 (12.04.2023)
+        - fix examples in README
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.6
```

### Comparing `sirms-1.2.1/setup.py` & `sirms-1.2.2/setup.py`

 * *Files identical despite different names*

