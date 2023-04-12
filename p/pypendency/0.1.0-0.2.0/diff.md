# Comparing `tmp/pypendency-0.1.0.tar.gz` & `tmp/pypendency-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypendency-0.1.0.tar", last modified: Mon Jan 27 14:31:54 2020, max compression
+gzip compressed data, was "dist/pypendency-0.2.0.tar", last modified: Wed Apr 12 09:34:22 2023, max compression
```

## Comparing `pypendency-0.1.0.tar` & `pypendency-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-27 14:31:54.000000 pypendency-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (115)       38 2020-01-27 14:31:54.000000 pypendency-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     3773 2020-01-27 14:31:54.000000 pypendency-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     2333 2020-01-27 14:31:41.000000 pypendency-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (115)     1127 2020-01-27 14:31:41.000000 pypendency-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-27 14:31:54.000000 pypendency-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-27 14:31:54.000000 pypendency-0.1.0/src/pypendency.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)       48 2020-01-27 14:31:54.000000 pypendency-0.1.0/src/pypendency.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)      632 2020-01-27 14:31:54.000000 pypendency-0.1.0/src/pypendency.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)     3773 2020-01-27 14:31:54.000000 pypendency-0.1.0/src/pypendency.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)       11 2020-01-27 14:31:54.000000 pypendency-0.1.0/src/pypendency.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-27 14:31:54.000000 pypendency-0.1.0/src/pypendency.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-27 14:31:54.000000 pypendency-0.1.0/src/pypendency/
--rw-r--r--   0 runner    (1001) docker     (115)      976 2020-01-27 14:31:41.000000 pypendency-0.1.0/src/pypendency/builder.py
--rw-r--r--   0 runner    (1001) docker     (115)     3060 2020-01-27 14:31:41.000000 pypendency-0.1.0/src/pypendency/container.py
--rw-r--r--   0 runner    (1001) docker     (115)      262 2020-01-27 14:31:41.000000 pypendency-0.1.0/src/pypendency/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-27 14:31:54.000000 pypendency-0.1.0/src/pypendency/loaders/
--rw-r--r--   0 runner    (1001) docker     (115)      403 2020-01-27 14:31:41.000000 pypendency-0.1.0/src/pypendency/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (115)     1771 2020-01-27 14:31:41.000000 pypendency-0.1.0/src/pypendency/loaders/py_loader.py
--rw-r--r--   0 runner    (1001) docker     (115)     1936 2020-01-27 14:31:41.000000 pypendency-0.1.0/src/pypendency/loaders/yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-01-27 14:31:41.000000 pypendency-0.1.0/src/pypendency/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      875 2020-01-27 14:31:41.000000 pypendency-0.1.0/src/pypendency/loaders/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-27 14:31:54.000000 pypendency-0.1.0/src/pypendency/types/
--rw-r--r--   0 runner    (1001) docker     (115)      194 2020-01-27 14:31:41.000000 pypendency-0.1.0/src/pypendency/types/python_loadable_module.py
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-01-27 14:31:41.000000 pypendency-0.1.0/src/pypendency/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      253 2020-01-27 14:31:41.000000 pypendency-0.1.0/src/pypendency/argument.py
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-01-27 14:31:41.000000 pypendency-0.1.0/src/pypendency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1292 2020-01-27 14:31:41.000000 pypendency-0.1.0/src/pypendency/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:22.000000 pypendency-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-12 09:34:22.000000 pypendency-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-12 09:34:09.000000 pypendency-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:34:22.000000 pypendency-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-12 09:34:09.000000 pypendency-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:22.000000 pypendency-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:22.000000 pypendency-0.2.0/src/pypendency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:22.000000 pypendency-0.2.0/src/pypendency/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/loaders/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/loaders/py_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/loaders/yaml_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:22.000000 pypendency-0.2.0/src/pypendency/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/types/python_loadable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:22.000000 pypendency-0.2.0/src/pypendency.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-12 09:34:21.000000 pypendency-0.2.0/src/pypendency.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-12 09:34:22.000000 pypendency-0.2.0/src/pypendency.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:34:21.000000 pypendency-0.2.0/src/pypendency.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 09:34:21.000000 pypendency-0.2.0/src/pypendency.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 09:34:21.000000 pypendency-0.2.0/src/pypendency.egg-info/top_level.txt
```

### Comparing `pypendency-0.1.0/PKG-INFO` & `pypendency-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pypendency
-Version: 0.1.0
+Version: 0.2.0
 Summary: A dependency injection tool for python
 Home-page: https://github.com/Feverup/pypendency
 Author: Marcos Hernandez Juarez
 Author-email: marcos.hernandezjuarez@gmail.com
 License: MIT License
 Description: # Pypendency
-        Pypendency is a dependency injection library for python 3.6+.
+        Pypendency is a dependency injection library for python >=3.7.
         
         ## Installation
         ```bash
         pip install pypendency
         ```
         
         ## Usage
@@ -91,15 +91,14 @@
         docker run -v $(pwd)/.:/usr/src/app pypendency-dev bash -c "pipenv run make run-tests"
         ```
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pypendency-0.1.0/README.md` & `pypendency-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Pypendency
-Pypendency is a dependency injection library for python 3.6+.
+Pypendency is a dependency injection library for python >=3.7.
 
 ## Installation
 ```bash
 pip install pypendency
 ```
 
 ## Usage
```

### Comparing `pypendency-0.1.0/setup.py` & `pypendency-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 
 with open('README.md', 'r') as readme:
     README = readme.read()
 
 
 setup(
     name='pypendency',
-    version='0.1.0',
+    version='0.2.0',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     author='Marcos Hernandez Juarez',
     author_email='marcos.hernandezjuarez@gmail.com',
     description='A dependency injection tool for python',
     long_description=README,
     long_description_content_type='text/markdown',
     license='MIT License',
     url='https://github.com/Feverup/pypendency',
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Libraries',
         'Typing :: Typed',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     install_requires=[
         'pyyaml',
-        'dataclasses;python_version<"3.7.0"',
     ],
     include_package_data=True,
 )
```

### Comparing `pypendency-0.1.0/src/pypendency.egg-info/SOURCES.txt` & `pypendency-0.2.0/src/pypendency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypendency-0.1.0/src/pypendency.egg-info/PKG-INFO` & `pypendency-0.2.0/src/pypendency.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pypendency
-Version: 0.1.0
+Version: 0.2.0
 Summary: A dependency injection tool for python
 Home-page: https://github.com/Feverup/pypendency
 Author: Marcos Hernandez Juarez
 Author-email: marcos.hernandezjuarez@gmail.com
 License: MIT License
 Description: # Pypendency
-        Pypendency is a dependency injection library for python 3.6+.
+        Pypendency is a dependency injection library for python >=3.7.
         
         ## Installation
         ```bash
         pip install pypendency
         ```
         
         ## Usage
@@ -91,15 +91,14 @@
         docker run -v $(pwd)/.:/usr/src/app pypendency-dev bash -c "pipenv run make run-tests"
         ```
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pypendency-0.1.0/src/pypendency/builder.py` & `pypendency-0.2.0/src/pypendency/builder.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.1.0/src/pypendency/container.py` & `pypendency-0.2.0/src/pypendency/container.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.1.0/src/pypendency/loaders/py_loader.py` & `pypendency-0.2.0/src/pypendency/loaders/py_loader.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.1.0/src/pypendency/loaders/yaml_loader.py` & `pypendency-0.2.0/src/pypendency/loaders/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.1.0/src/pypendency/loaders/exceptions.py` & `pypendency-0.2.0/src/pypendency/loaders/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.1.0/src/pypendency/exceptions.py` & `pypendency-0.2.0/src/pypendency/exceptions.py`

 * *Files identical despite different names*

