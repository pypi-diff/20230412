# Comparing `tmp/testit-adapter-nose-2.1.5.tar.gz` & `tmp/testit-adapter-nose-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-nose-2.1.5.tar", last modified: Tue Apr  4 07:02:27 2023, max compression
+gzip compressed data, was "testit-adapter-nose-2.1.6.tar", last modified: Wed Apr 12 09:36:15 2023, max compression
```

## Comparing `testit-adapter-nose-2.1.5.tar` & `testit-adapter-nose-2.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:27.670971 testit-adapter-nose-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-04 07:02:27.670971 testit-adapter-nose-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-04 07:02:08.000000 testit-adapter-nose-2.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 07:02:27.670971 testit-adapter-nose-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-04 07:02:08.000000 testit-adapter-nose-2.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:27.670971 testit-adapter-nose-2.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:27.670971 testit-adapter-nose-2.1.5/src/testit_adapter_nose/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:08.000000 testit-adapter-nose-2.1.5/src/testit_adapter_nose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-04 07:02:08.000000 testit-adapter-nose-2.1.5/src/testit_adapter_nose/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-04 07:02:08.000000 testit-adapter-nose-2.1.5/src/testit_adapter_nose/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-04 07:02:08.000000 testit-adapter-nose-2.1.5/src/testit_adapter_nose/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:27.670971 testit-adapter-nose-2.1.5/src/testit_adapter_nose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-04 07:02:27.000000 testit-adapter-nose-2.1.5/src/testit_adapter_nose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-04 07:02:27.000000 testit-adapter-nose-2.1.5/src/testit_adapter_nose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 07:02:27.000000 testit-adapter-nose-2.1.5/src/testit_adapter_nose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-04 07:02:27.000000 testit-adapter-nose-2.1.5/src/testit_adapter_nose.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-04 07:02:27.000000 testit-adapter-nose-2.1.5/src/testit_adapter_nose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-04 07:02:27.000000 testit-adapter-nose-2.1.5/src/testit_adapter_nose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:15.097477 testit-adapter-nose-2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-12 09:36:15.097477 testit-adapter-nose-2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-12 09:35:58.000000 testit-adapter-nose-2.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:36:15.097477 testit-adapter-nose-2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-12 09:35:58.000000 testit-adapter-nose-2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:15.097477 testit-adapter-nose-2.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:15.097477 testit-adapter-nose-2.1.6/src/testit_adapter_nose/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:35:58.000000 testit-adapter-nose-2.1.6/src/testit_adapter_nose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-12 09:35:58.000000 testit-adapter-nose-2.1.6/src/testit_adapter_nose/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-12 09:35:58.000000 testit-adapter-nose-2.1.6/src/testit_adapter_nose/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-12 09:35:58.000000 testit-adapter-nose-2.1.6/src/testit_adapter_nose/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:15.097477 testit-adapter-nose-2.1.6/src/testit_adapter_nose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-12 09:36:15.000000 testit-adapter-nose-2.1.6/src/testit_adapter_nose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-12 09:36:15.000000 testit-adapter-nose-2.1.6/src/testit_adapter_nose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:36:15.000000 testit-adapter-nose-2.1.6/src/testit_adapter_nose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 09:36:15.000000 testit-adapter-nose-2.1.6/src/testit_adapter_nose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 09:36:15.000000 testit-adapter-nose-2.1.6/src/testit_adapter_nose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 09:36:15.000000 testit-adapter-nose-2.1.6/src/testit_adapter_nose.egg-info/top_level.txt
```

### Comparing `testit-adapter-nose-2.1.5/PKG-INFO` & `testit-adapter-nose-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-nose
-Version: 2.1.5
+Version: 2.1.6
 Summary: Nose adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-nose-2.1.5/README.md` & `testit-adapter-nose-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `testit-adapter-nose-2.1.5/setup.py` & `testit-adapter-nose-2.1.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='testit-adapter-nose',
-    version='2.1.5',
+    version='2.1.6',
     description='Nose adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,14 +16,14 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_nose'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'nose2', 'testit-python-commons==2.1.5'],
+    install_requires=['attrs', 'nose2', 'testit-python-commons==2.1.6'],
     entry_points={
             'nose.plugins.0.10': [
                 'testit_adapter_nose = testit_adapter_nose.plugin:TmsPlugin',
             ]
     }
 )
```

### Comparing `testit-adapter-nose-2.1.5/src/testit_adapter_nose/listener.py` & `testit-adapter-nose-2.1.6/src/testit_adapter_nose/listener.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-nose-2.1.5/src/testit_adapter_nose/plugin.py` & `testit-adapter-nose-2.1.6/src/testit_adapter_nose/plugin.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-nose-2.1.5/src/testit_adapter_nose/utils.py` & `testit-adapter-nose-2.1.6/src/testit_adapter_nose/utils.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-nose-2.1.5/src/testit_adapter_nose.egg-info/PKG-INFO` & `testit-adapter-nose-2.1.6/src/testit_adapter_nose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-nose
-Version: 2.1.5
+Version: 2.1.6
 Summary: Nose adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

