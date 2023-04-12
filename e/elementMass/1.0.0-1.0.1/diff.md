# Comparing `tmp/elementMass-1.0.0.tar.gz` & `tmp/elementMass-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elementMass-1.0.0.tar", last modified: Wed Apr 12 14:02:12 2023, max compression
+gzip compressed data, was "elementMass-1.0.1.tar", last modified: Wed Apr 12 14:44:04 2023, max compression
```

## Comparing `elementMass-1.0.0.tar` & `elementMass-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:02:12.189443 elementMass-1.0.0/
--rw-rw-rw-   0        0        0     1094 2023-04-12 10:21:42.000000 elementMass-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       14 2023-04-12 10:21:42.000000 elementMass-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2409 2023-04-12 14:02:12.189443 elementMass-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      756 2023-04-12 12:14:48.000000 elementMass-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-12 14:02:12.148282 elementMass-1.0.0/elementMass/
--rw-rw-rw-   0        0        0      353 2023-04-12 13:56:13.000000 elementMass-1.0.0/elementMass/Periodic_table.py
--rw-rw-rw-   0        0        0       25 2023-04-12 11:39:14.000000 elementMass-1.0.0/elementMass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:02:12.189443 elementMass-1.0.0/elementMass/data/
--rw-rw-rw-   0        0        0        0 2023-04-12 10:21:42.000000 elementMass-1.0.0/elementMass/data/__init__.py
--rw-rw-rw-   0        0        0    30318 2023-04-12 10:21:42.000000 elementMass-1.0.0/elementMass/data/periodic_table.parquet
--rw-rw-rw-   0        0        0     4073 2023-04-12 11:26:03.000000 elementMass-1.0.0/elementMass/elements.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:02:12.182691 elementMass-1.0.0/elementMass.egg-info/
--rw-rw-rw-   0        0        0     2409 2023-04-12 14:02:12.000000 elementMass-1.0.0/elementMass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-04-12 14:02:12.000000 elementMass-1.0.0/elementMass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 14:02:12.000000 elementMass-1.0.0/elementMass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-12 14:02:12.000000 elementMass-1.0.0/elementMass.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-12 14:02:12.000000 elementMass-1.0.0/elementMass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      622 2023-04-12 12:13:49.000000 elementMass-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 14:02:12.189443 elementMass-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 14:44:04.010190 elementMass-1.0.1/
+-rw-rw-rw-   0        0        0     1094 2023-04-12 10:21:42.000000 elementMass-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-04-12 10:21:42.000000 elementMass-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2511 2023-04-12 14:44:04.005412 elementMass-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-04-12 14:41:25.000000 elementMass-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-12 14:44:03.966088 elementMass-1.0.1/elementMass/
+-rw-rw-rw-   0        0        0      353 2023-04-12 13:56:13.000000 elementMass-1.0.1/elementMass/Periodic_table.py
+-rw-rw-rw-   0        0        0       25 2023-04-12 11:39:14.000000 elementMass-1.0.1/elementMass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:44:04.004428 elementMass-1.0.1/elementMass/data/
+-rw-rw-rw-   0        0        0        0 2023-04-12 10:21:42.000000 elementMass-1.0.1/elementMass/data/__init__.py
+-rw-rw-rw-   0        0        0    30318 2023-04-12 10:21:42.000000 elementMass-1.0.1/elementMass/data/periodic_table.parquet
+-rw-rw-rw-   0        0        0     4073 2023-04-12 11:26:03.000000 elementMass-1.0.1/elementMass/elements.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:44:03.998852 elementMass-1.0.1/elementMass.egg-info/
+-rw-rw-rw-   0        0        0     2511 2023-04-12 14:44:03.000000 elementMass-1.0.1/elementMass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-04-12 14:44:03.000000 elementMass-1.0.1/elementMass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:44:03.000000 elementMass-1.0.1/elementMass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-12 14:44:03.000000 elementMass-1.0.1/elementMass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-12 14:44:03.000000 elementMass-1.0.1/elementMass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      714 2023-04-12 14:43:19.000000 elementMass-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:44:04.011220 elementMass-1.0.1/setup.cfg
```

### Comparing `elementMass-1.0.0/LICENSE` & `elementMass-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elementMass-1.0.0/PKG-INFO` & `elementMass-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: elementMass
-Version: 1.0.0
+Version: 1.0.1
+Summary: elementMass is a compact Python library for calculating atomic weights of chemical compounds
 Author: Thomas van Gerve
 License: MIT License
         
         Copyright (c) 2023 Thomas van Gerve
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -37,15 +38,15 @@
 ===========
 elementMass is a compact Python library for calculating atomic weights of chemical compounds as well as cation and oxygen amounts in simple oxides.
 
 
 
 Documentation
 -------------
-Code documentation is available at `elements_tvg.readthedocs.io <https://elements-tvg.readthedocs.io/en/latest/>`_
+Code documentation is available at `elements_tvg.readthedocs.io <https://elementMass.readthedocs.io/en/latest/>`_
 
 Installation
 ------------
 elements can be installed with pip by running:
 
 .. code-block:: bash
```

### Comparing `elementMass-1.0.0/README.rst` & `elementMass-1.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ===========
 elementMass is a compact Python library for calculating atomic weights of chemical compounds as well as cation and oxygen amounts in simple oxides.
 
 
 
 Documentation
 -------------
-Code documentation is available at `elements_tvg.readthedocs.io <https://elements-tvg.readthedocs.io/en/latest/>`_
+Code documentation is available at `elements_tvg.readthedocs.io <https://elementMass.readthedocs.io/en/latest/>`_
 
 Installation
 ------------
 elements can be installed with pip by running:
 
 .. code-block:: bash
```

### Comparing `elementMass-1.0.0/elementMass/data/periodic_table.parquet` & `elementMass-1.0.1/elementMass/data/periodic_table.parquet`

 * *Files identical despite different names*

### Comparing `elementMass-1.0.0/elementMass/elements.py` & `elementMass-1.0.1/elementMass/elements.py`

 * *Files identical despite different names*

### Comparing `elementMass-1.0.0/elementMass.egg-info/PKG-INFO` & `elementMass-1.0.1/elementMass.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: elementMass
-Version: 1.0.0
+Version: 1.0.1
+Summary: elementMass is a compact Python library for calculating atomic weights of chemical compounds
 Author: Thomas van Gerve
 License: MIT License
         
         Copyright (c) 2023 Thomas van Gerve
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -37,15 +38,15 @@
 ===========
 elementMass is a compact Python library for calculating atomic weights of chemical compounds as well as cation and oxygen amounts in simple oxides.
 
 
 
 Documentation
 -------------
-Code documentation is available at `elements_tvg.readthedocs.io <https://elements-tvg.readthedocs.io/en/latest/>`_
+Code documentation is available at `elements_tvg.readthedocs.io <https://elementMass.readthedocs.io/en/latest/>`_
 
 Installation
 ------------
 elements can be installed with pip by running:
 
 .. code-block:: bash
```

