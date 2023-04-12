# Comparing `tmp/clean_graph-0.1.0.tar.gz` & `tmp/clean_graph-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_graph-0.1.0.tar", last modified: Tue Feb 21 07:58:32 2023, max compression
+gzip compressed data, was "clean_graph-0.1.1.tar", last modified: Wed Apr 12 07:37:24 2023, max compression
```

## Comparing `clean_graph-0.1.0.tar` & `clean_graph-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 07:58:32.079998 clean_graph-0.1.0/
--rw-rw-rw-   0        0        0      165 2022-12-29 15:26:00.000000 clean_graph-0.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3565 2022-12-29 15:26:00.000000 clean_graph-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      118 2023-02-20 21:50:02.000000 clean_graph-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1077 2022-12-29 15:26:00.000000 clean_graph-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      262 2022-12-29 15:26:00.000000 clean_graph-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1958 2023-02-21 07:58:32.079998 clean_graph-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      996 2023-02-15 21:50:49.000000 clean_graph-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-21 07:58:31.964094 clean_graph-0.1.0/clean_graph/
--rw-rw-rw-   0        0        0      499 2023-02-13 18:38:20.000000 clean_graph-0.1.0/clean_graph/__init__.py
--rw-rw-rw-   0        0        0    25408 2023-02-17 15:51:06.000000 clean_graph-0.1.0/clean_graph/clean_graph.py
--rw-rw-rw-   0        0        0    59833 2023-02-20 19:10:52.000000 clean_graph-0.1.0/clean_graph/columnchartwithwaterfall.py
--rw-rw-rw-   0        0        0    15280 2023-02-19 19:02:27.000000 clean_graph-0.1.0/clean_graph/general_functions.py
--rw-rw-rw-   0        0        0    11293 2023-02-18 10:46:07.000000 clean_graph-0.1.0/clean_graph/multiplier.py
-drwxrwxrwx   0        0        0        0 2023-02-21 07:58:31.984078 clean_graph-0.1.0/clean_graph.egg-info/
--rw-rw-rw-   0        0        0     1958 2023-02-21 07:58:31.000000 clean_graph-0.1.0/clean_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-02-21 07:58:31.000000 clean_graph-0.1.0/clean_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 07:58:31.000000 clean_graph-0.1.0/clean_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-01 19:34:47.000000 clean_graph-0.1.0/clean_graph.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-02-21 07:58:31.000000 clean_graph-0.1.0/clean_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-21 07:58:31.000000 clean_graph-0.1.0/clean_graph.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-21 07:58:32.052022 clean_graph-0.1.0/docs/
--rw-rw-rw-   0        0        0      612 2022-12-29 15:26:00.000000 clean_graph-0.1.0/docs/Makefile
--rw-rw-rw-   0        0        0       28 2022-12-29 15:26:00.000000 clean_graph-0.1.0/docs/authors.rst
--rw-rw-rw-   0        0        0     4848 2022-12-29 15:26:00.000000 clean_graph-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0       33 2022-12-29 15:26:00.000000 clean_graph-0.1.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       28 2022-12-29 15:26:00.000000 clean_graph-0.1.0/docs/history.rst
--rw-rw-rw-   0        0        0      308 2022-12-29 15:26:00.000000 clean_graph-0.1.0/docs/index.rst
--rw-rw-rw-   0        0        0     1158 2022-12-29 15:26:00.000000 clean_graph-0.1.0/docs/installation.rst
--rwxrwxrwx   0        0        0      773 2022-12-29 15:26:00.000000 clean_graph-0.1.0/docs/make.bat
--rw-rw-rw-   0        0        0       27 2022-12-29 15:26:00.000000 clean_graph-0.1.0/docs/readme.rst
--rw-rw-rw-   0        0        0       77 2022-12-29 15:26:00.000000 clean_graph-0.1.0/docs/usage.rst
--rw-rw-rw-   0        0        0      454 2023-02-21 07:58:32.079998 clean_graph-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-02-20 21:45:03.000000 clean_graph-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-21 07:58:32.064019 clean_graph-0.1.0/tests/
--rw-rw-rw-   0        0        0       41 2022-12-29 15:26:00.000000 clean_graph-0.1.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-21 07:58:32.076001 clean_graph-0.1.0/tests/clean_graph/
--rw-rw-rw-   0        0        0     1230 2023-02-19 18:58:59.000000 clean_graph-0.1.0/tests/clean_graph/test_general_functions.py
--rw-rw-rw-   0        0        0     3658 2023-02-18 10:52:29.000000 clean_graph-0.1.0/tests/clean_graph/test_multiplier.py
--rw-rw-rw-   0        0        0      573 2023-02-18 11:59:10.000000 clean_graph-0.1.0/tests/test_clean_graph.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:37:24.011825 clean_graph-0.1.1/
+-rw-rw-rw-   0        0        0      165 2022-12-29 15:26:00.000000 clean_graph-0.1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3565 2022-12-29 15:26:00.000000 clean_graph-0.1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      371 2023-04-12 07:05:39.000000 clean_graph-0.1.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1077 2022-12-29 15:26:00.000000 clean_graph-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      262 2022-12-29 15:26:00.000000 clean_graph-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2477 2023-04-12 07:37:24.011825 clean_graph-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1164 2023-04-12 07:32:05.000000 clean_graph-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-12 07:37:23.880324 clean_graph-0.1.1/clean_graph/
+-rw-rw-rw-   0        0        0      499 2023-04-12 07:27:50.000000 clean_graph-0.1.1/clean_graph/__init__.py
+-rw-rw-rw-   0        0        0    25408 2023-02-17 15:51:06.000000 clean_graph-0.1.1/clean_graph/clean_graph.py
+-rw-rw-rw-   0        0        0    60113 2023-04-12 07:37:00.000000 clean_graph-0.1.1/clean_graph/columnchartwithwaterfall.py
+-rw-rw-rw-   0        0        0    15280 2023-02-19 19:02:27.000000 clean_graph-0.1.1/clean_graph/general_functions.py
+-rw-rw-rw-   0        0        0    11293 2023-02-18 10:46:07.000000 clean_graph-0.1.1/clean_graph/multiplier.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:37:23.895947 clean_graph-0.1.1/clean_graph.egg-info/
+-rw-rw-rw-   0        0        0     2477 2023-04-12 07:37:23.000000 clean_graph-0.1.1/clean_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-04-12 07:37:23.000000 clean_graph-0.1.1/clean_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 07:37:23.000000 clean_graph-0.1.1/clean_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-01 19:34:47.000000 clean_graph-0.1.1/clean_graph.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-04-12 07:37:23.000000 clean_graph-0.1.1/clean_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-12 07:37:23.000000 clean_graph-0.1.1/clean_graph.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 07:37:23.980579 clean_graph-0.1.1/docs/
+-rw-rw-rw-   0        0        0      612 2022-12-29 15:26:00.000000 clean_graph-0.1.1/docs/Makefile
+-rw-rw-rw-   0        0        0       28 2022-12-29 15:26:00.000000 clean_graph-0.1.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     4848 2022-12-29 15:26:00.000000 clean_graph-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0       33 2022-12-29 15:26:00.000000 clean_graph-0.1.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       28 2022-12-29 15:26:00.000000 clean_graph-0.1.1/docs/history.rst
+-rw-rw-rw-   0        0        0      308 2022-12-29 15:26:00.000000 clean_graph-0.1.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1158 2022-12-29 15:26:00.000000 clean_graph-0.1.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      773 2022-12-29 15:26:00.000000 clean_graph-0.1.1/docs/make.bat
+-rw-rw-rw-   0        0        0       27 2022-12-29 15:26:00.000000 clean_graph-0.1.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       77 2022-12-29 15:26:00.000000 clean_graph-0.1.1/docs/usage.rst
+-rw-rw-rw-   0        0        0      454 2023-04-12 07:37:24.027449 clean_graph-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1454 2023-04-12 07:25:51.000000 clean_graph-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:37:23.996202 clean_graph-0.1.1/tests/
+-rw-rw-rw-   0        0        0       41 2022-12-29 15:26:00.000000 clean_graph-0.1.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:37:24.011825 clean_graph-0.1.1/tests/clean_graph/
+-rw-rw-rw-   0        0        0     1230 2023-02-19 18:58:59.000000 clean_graph-0.1.1/tests/clean_graph/test_general_functions.py
+-rw-rw-rw-   0        0        0     3658 2023-02-18 10:52:29.000000 clean_graph-0.1.1/tests/clean_graph/test_multiplier.py
+-rw-rw-rw-   0        0        0      573 2023-02-18 11:59:10.000000 clean_graph-0.1.1/tests/test_clean_graph.py
```

### Comparing `clean_graph-0.1.0/CONTRIBUTING.rst` & `clean_graph-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `clean_graph-0.1.0/LICENSE` & `clean_graph-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_graph-0.1.0/README.rst` & `clean_graph-0.1.1/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 .. image:: https://readthedocs.org/projects/clean-graph/badge/?version=latest
         :target: https://clean-graph.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 
 
-Clean Graph is a Python package for IBCS-like graphs based on matplotlib.
+Clean Graph was a Python package for IBCS-like graphs based on matplotlib. This package will no longer be maintained and has been replaced by 'Clean Business Chart', with pandas support.
+
+* See: https://pypi.org/project/Clean-Business-Chart/
 
 
 * Free software: MIT license
 * Documentation: https://clean-graph.readthedocs.io.
 
 
 Features
```

### Comparing `clean_graph-0.1.0/clean_graph/clean_graph.py` & `clean_graph-0.1.1/clean_graph/clean_graph.py`

 * *Files identical despite different names*

### Comparing `clean_graph-0.1.0/clean_graph/columnchartwithwaterfall.py` & `clean_graph-0.1.1/clean_graph/columnchartwithwaterfall.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,19 @@
                  force_pl_is_zero=False, force_zero_decimals=False, force_max_one_decimals=False):
         """
         This is the first function that will be called automatically. Here you'll find all the possible parameters to customize your experience.
         """
         super().__init__()                            # Get the variables from the parent class
         self._other_columnwithwaterfall_variables()   # Get additional variables for this class
         
+        # Announcement
+        print("'Clean Graph' will no longer be supported. It was a working title for the package 'Clean Business Chart'.")
+        print("More info: https://pypi.org/project/Clean-Business-Chart/")
+        print("Thank you for your support!")
+        
         # Store variables
         self.original_data          = data
         self.original_multiplier    = Multiplier(multiplier)
         self.year                   = None
         self.positive_is_good       = positive_is_good
         self.base_scenario          = preferred_base_scenario
         self.hatch                  = self.hatch_pattern
```

### Comparing `clean_graph-0.1.0/clean_graph/general_functions.py` & `clean_graph-0.1.1/clean_graph/general_functions.py`

 * *Files identical despite different names*

### Comparing `clean_graph-0.1.0/clean_graph/multiplier.py` & `clean_graph-0.1.1/clean_graph/multiplier.py`

 * *Files identical despite different names*

### Comparing `clean_graph-0.1.0/clean_graph.egg-info/SOURCES.txt` & `clean_graph-0.1.1/clean_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clean_graph-0.1.0/docs/Makefile` & `clean_graph-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clean_graph-0.1.0/docs/conf.py` & `clean_graph-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `clean_graph-0.1.0/docs/installation.rst` & `clean_graph-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `clean_graph-0.1.0/docs/make.bat` & `clean_graph-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clean_graph-0.1.0/setup.py` & `clean_graph-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,21 +24,21 @@
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
-    description="Clean Graph is a Python package for IBCS-like graphs based on matplotlib.",
+    description="Clean Graph was a Python package for IBCS-like graphs based on matplotlib. This package will no longer be maintained and has been replaced by 'Clean Business Chart', with pandas support.",
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='clean_graph',
     name='clean_graph',
     packages=find_packages(include=['clean_graph', 'clean_graph.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/marcelw1323/clean_graph',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `clean_graph-0.1.0/tests/clean_graph/test_general_functions.py` & `clean_graph-0.1.1/tests/clean_graph/test_general_functions.py`

 * *Files identical despite different names*

### Comparing `clean_graph-0.1.0/tests/clean_graph/test_multiplier.py` & `clean_graph-0.1.1/tests/clean_graph/test_multiplier.py`

 * *Files identical despite different names*

### Comparing `clean_graph-0.1.0/tests/test_clean_graph.py` & `clean_graph-0.1.1/tests/test_clean_graph.py`

 * *Files identical despite different names*

