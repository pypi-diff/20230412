# Comparing `tmp/ordpy-1.1.1.tar.gz` & `tmp/ordpy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ordpy-1.1.1.tar", last modified: Tue Apr 11 22:51:24 2023, max compression
+gzip compressed data, was "ordpy-1.1.2.tar", last modified: Wed Apr 12 18:15:22 2023, max compression
```

## Comparing `ordpy-1.1.1.tar` & `ordpy-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-04-11 22:51:24.334302 ordpy-1.1.1/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1098 2023-01-09 15:37:59.000000 ordpy-1.1.1/LICENSE
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    11305 2023-04-11 22:51:24.334302 ordpy-1.1.1/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    10760 2023-04-11 22:32:54.000000 ordpy-1.1.1/README.rst
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-04-11 22:51:24.334302 ordpy-1.1.1/ordpy/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       20 2023-01-09 15:37:59.000000 ordpy-1.1.1/ordpy/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    95644 2023-04-11 22:23:00.000000 ordpy-1.1.1/ordpy/ordpy.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-04-11 22:51:24.334302 ordpy-1.1.1/ordpy.egg-info/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    11305 2023-04-11 22:51:24.000000 ordpy-1.1.1/ordpy.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      201 2023-04-11 22:51:24.000000 ordpy-1.1.1/ordpy.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-04-11 22:51:24.000000 ordpy-1.1.1/ordpy.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        6 2023-04-11 22:51:24.000000 ordpy-1.1.1/ordpy.egg-info/top_level.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      123 2023-04-11 22:22:56.000000 ordpy-1.1.1/pyproject.toml
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      588 2023-04-11 22:51:24.334302 ordpy-1.1.1/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1310 2023-04-11 22:37:31.000000 ordpy-1.1.1/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-04-12 18:15:22.258100 ordpy-1.1.2/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1098 2023-01-09 15:37:59.000000 ordpy-1.1.2/LICENSE
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    11305 2023-04-12 18:15:22.258100 ordpy-1.1.2/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    10760 2023-04-11 22:32:54.000000 ordpy-1.1.2/README.rst
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-04-12 18:15:22.254100 ordpy-1.1.2/ordpy/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       20 2023-01-09 15:37:59.000000 ordpy-1.1.2/ordpy/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    95614 2023-04-12 18:11:20.000000 ordpy-1.1.2/ordpy/ordpy.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-04-12 18:15:22.258100 ordpy-1.1.2/ordpy.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    11305 2023-04-12 18:15:22.000000 ordpy-1.1.2/ordpy.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      201 2023-04-12 18:15:22.000000 ordpy-1.1.2/ordpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-04-12 18:15:22.000000 ordpy-1.1.2/ordpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        6 2023-04-12 18:15:22.000000 ordpy-1.1.2/ordpy.egg-info/top_level.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      123 2023-04-11 22:22:56.000000 ordpy-1.1.2/pyproject.toml
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      588 2023-04-12 18:15:22.258100 ordpy-1.1.2/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1310 2023-04-12 18:12:34.000000 ordpy-1.1.2/setup.py
```

### Comparing `ordpy-1.1.1/LICENSE` & `ordpy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ordpy-1.1.1/PKG-INFO` & `ordpy-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ordpy
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python package for data analysis with permutation entropy and ordinal networks methods.
 Home-page: https://github.com/arthurpessa/ordpy
 Author: Arthur A. B. Pessa and Haroldo V. Ribeiro
 Author-email: arthur_pessa@hotmail.com, hvr@dfi.uem.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ordpy-1.1.1/README.rst` & `ordpy-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `ordpy-1.1.1/ordpy/ordpy.py` & `ordpy-1.1.2/ordpy/ordpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,22 +410,24 @@
                     If `True`, it returns ordinal patterns not appearing in the 
                     symbolic sequence obtained from **data**. If `False`, these
                     missing patterns (permutations) are omitted (default: `False`).
     tie_precision : None, int
                     If not `None`, **data** is rounded with `tie_precision`
                     decimal numbers (default: `None`).
     ordered: boolean
-                    If `True`, it returns ordinal patterns not appearing in the 
-                    symbolic sequence obtained from **data**. If `False`, these
-                    missing patterns (permutations) are omitted (default: `False`).
+             If `True`, it also returns ordinal patterns not appearing in the 
+             symbolic sequence obtained from **data** in ascending ordered. 
+             The `return_missing` parameter must also be `True`.
+   
     Returns
     -------
      : tuple
-       Tuple containing two arrays, one with the ordinal patterns occurring in data 
-       and another with their corresponding probabilities.
+       Tuple containing two arrays, one with the ordinal patterns and another 
+       with their corresponding probabilities.
+       
     Examples
     --------
     >>> ordinal_distribution([4,7,9,10,6,11,3], dx=2)
     (array([[0, 1],
             [1, 0]]),
      array([0.66666667, 0.33333333]))
     >>>
```

### Comparing `ordpy-1.1.1/ordpy.egg-info/PKG-INFO` & `ordpy-1.1.2/ordpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ordpy
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python package for data analysis with permutation entropy and ordinal networks methods.
 Home-page: https://github.com/arthurpessa/ordpy
 Author: Arthur A. B. Pessa and Haroldo V. Ribeiro
 Author-email: arthur_pessa@hotmail.com, hvr@dfi.uem.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ordpy-1.1.1/setup.cfg` & `ordpy-1.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ordpy
-version = 1.1.1
+version = 1.1.2
 url = https://github.com/arthurpessa/ordpy
 author = Arthur A. B. Pessa and Haroldo V. Ribeiro
 author_email = arthur_pessa@hotmail.com, hvr@uem.dfi.br
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

### Comparing `ordpy-1.1.1/setup.py` & `ordpy-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import setuptools
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ordpy",
-    version="1.1.1",
+    version="1.1.2",
     author="Arthur A. B. Pessa and Haroldo V. Ribeiro",
     author_email="arthur_pessa@hotmail.com, hvr@dfi.uem.br",
     description="A Python package for data analysis with permutation entropy and ordinal networks methods.",
     long_description=long_description,
     long_description_content_type="text/x-rst; charset=UTF-8",
     url="https://github.com/arthurpessa/ordpy",
     packages=setuptools.find_packages(),
```

