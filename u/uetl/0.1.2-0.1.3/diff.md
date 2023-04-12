# Comparing `tmp/uetl-0.1.2.tar.gz` & `tmp/uetl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uetl-0.1.2.tar", last modified: Tue Apr 11 13:52:56 2023, max compression
+gzip compressed data, was "uetl-0.1.3.tar", last modified: Wed Apr 12 14:44:59 2023, max compression
```

## Comparing `uetl-0.1.2.tar` & `uetl-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-11 13:52:56.692147 uetl-0.1.2/
--rw-r--r--   0 andre     (1000) andre     (1000)     1070 2020-04-28 23:16:31.000000 uetl-0.1.2/LICENSE
--rw-r--r--   0 andre     (1000) andre     (1000)       29 2020-04-29 20:31:51.000000 uetl-0.1.2/MANIFEST.in
--rw-rw-r--   0 andre     (1000) andre     (1000)     3179 2023-04-11 13:52:56.692147 uetl-0.1.2/PKG-INFO
--rw-rw-r--   0 andre     (1000) andre     (1000)     2763 2022-12-24 18:51:51.000000 uetl-0.1.2/README.md
--rw-rw-r--   0 andre     (1000) andre     (1000)       38 2023-04-11 13:52:56.692147 uetl-0.1.2/setup.cfg
--rw-rw-r--   0 andre     (1000) andre     (1000)     1008 2023-04-11 12:46:31.000000 uetl-0.1.2/setup.py
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-11 13:52:56.692147 uetl-0.1.2/src/
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-11 13:52:56.692147 uetl-0.1.2/src/uetl.egg-info/
--rw-rw-r--   0 andre     (1000) andre     (1000)     3179 2023-04-11 13:52:56.000000 uetl-0.1.2/src/uetl.egg-info/PKG-INFO
--rw-rw-r--   0 andre     (1000) andre     (1000)      209 2023-04-11 13:52:56.000000 uetl-0.1.2/src/uetl.egg-info/SOURCES.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)        1 2023-04-11 13:52:56.000000 uetl-0.1.2/src/uetl.egg-info/dependency_links.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)       98 2023-04-11 13:52:56.000000 uetl-0.1.2/src/uetl.egg-info/requires.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)        5 2023-04-11 13:52:56.000000 uetl-0.1.2/src/uetl.egg-info/top_level.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)    14560 2023-04-11 12:44:35.000000 uetl-0.1.2/src/uetl.py
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-12 14:44:59.488400 uetl-0.1.3/
+-rw-rw-r--   0 andre     (1000) andre     (1000)     1070 2023-04-12 14:37:49.000000 uetl-0.1.3/LICENSE
+-rw-rw-r--   0 andre     (1000) andre     (1000)       29 2023-04-12 14:37:49.000000 uetl-0.1.3/MANIFEST.in
+-rw-rw-r--   0 andre     (1000) andre     (1000)     3179 2023-04-12 14:44:59.488400 uetl-0.1.3/PKG-INFO
+-rw-rw-r--   0 andre     (1000) andre     (1000)     2763 2023-04-12 14:37:49.000000 uetl-0.1.3/README.md
+-rw-rw-r--   0 andre     (1000) andre     (1000)       38 2023-04-12 14:44:59.488400 uetl-0.1.3/setup.cfg
+-rw-rw-r--   0 andre     (1000) andre     (1000)     1055 2023-04-12 14:42:36.000000 uetl-0.1.3/setup.py
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-12 14:44:59.488400 uetl-0.1.3/src/
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-12 14:44:59.488400 uetl-0.1.3/src/uetl.egg-info/
+-rw-rw-r--   0 andre     (1000) andre     (1000)     3179 2023-04-12 14:44:59.000000 uetl-0.1.3/src/uetl.egg-info/PKG-INFO
+-rw-rw-r--   0 andre     (1000) andre     (1000)      209 2023-04-12 14:44:59.000000 uetl-0.1.3/src/uetl.egg-info/SOURCES.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)        1 2023-04-12 14:44:59.000000 uetl-0.1.3/src/uetl.egg-info/dependency_links.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)      116 2023-04-12 14:44:59.000000 uetl-0.1.3/src/uetl.egg-info/requires.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)        5 2023-04-12 14:44:59.000000 uetl-0.1.3/src/uetl.egg-info/top_level.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)    14560 2023-04-12 14:37:49.000000 uetl-0.1.3/src/uetl.py
```

### Comparing `uetl-0.1.2/LICENSE` & `uetl-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uetl-0.1.2/PKG-INFO` & `uetl-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uetl
-Version: 0.1.2
+Version: 0.1.3
 Summary: Minimalist python ETL library.
 Home-page: https://github.com/andrespp/uetl
 Author: Andre Pereira
 Author-email: andrespp@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uetl-0.1.2/README.md` & `uetl-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `uetl-0.1.2/setup.py` & `uetl-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='uetl',
-    version='0.1.2',
+    version='0.1.3',
     description='Minimalist python ETL library.',
     py_modules=["uetl"],
     package_dir={'':'src'},
     classifiers=["Programming Language :: Python :: 3",
                  "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent",
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires = ["pandas >= 0.2",
                         "pyodbc >= 4.0",
                         "SQLAlchemy >= 1.3",
-                        "psycopg2 >= 2.8",
+                        "psycopg2-binary >= 2.8",
+                        "fdb >= 2.0.2",
                        ],
     extras_require = {
         "dev": ["check-manifest",
                 "pytest>=3.7",
                 "twine",
                 "tox",
                ],
```

### Comparing `uetl-0.1.2/src/uetl.egg-info/PKG-INFO` & `uetl-0.1.3/src/uetl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uetl
-Version: 0.1.2
+Version: 0.1.3
 Summary: Minimalist python ETL library.
 Home-page: https://github.com/andrespp/uetl
 Author: Andre Pereira
 Author-email: andrespp@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uetl-0.1.2/src/uetl.py` & `uetl-0.1.3/src/uetl.py`

 * *Files identical despite different names*

