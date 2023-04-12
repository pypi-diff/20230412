# Comparing `tmp/cythoninstallhelpers-1.2.1.tar.gz` & `tmp/cythoninstallhelpers-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cythoninstallhelpers-1.2.1.tar", last modified: Sun Nov 21 02:33:43 2021, max compression
+gzip compressed data, was "cythoninstallhelpers-1.3.0.tar", last modified: Wed Apr 12 10:31:39 2023, max compression
```

## Comparing `cythoninstallhelpers-1.2.1.tar` & `cythoninstallhelpers-1.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2021-11-21 02:33:43.755437 cythoninstallhelpers-1.2.1/
--rw-rw-rw-   0        0        0      630 2021-11-21 02:33:43.755437 cythoninstallhelpers-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2021-11-21 02:33:43.755437 cythoninstallhelpers-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1531 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-11-21 02:33:43.739767 cythoninstallhelpers-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2021-11-21 02:33:43.739767 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/
--rw-rw-rw-   0        0        0      278 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/__init__.py
--rw-rw-rw-   0        0        0       21 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/_version.py
--rw-rw-rw-   0        0        0     1177 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/build_config.py
--rw-rw-rw-   0        0        0     7514 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/configure_logger.py
--rw-rw-rw-   0        0        0     1171 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/get_version.py
--rw-rw-rw-   0        0        0     2279 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/make_cython_extensions.py
-drwxrwxrwx   0        0        0        0 2021-11-21 02:33:43.755437 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/
--rw-rw-rw-   0        0        0      244 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/__init__.py
--rw-rw-rw-   0        0        0       22 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/_version.py
--rw-rw-rw-   0        0        0       20 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/_version2.py
--rw-rw-rw-   0        0        0       17 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/_version_broken.py
-drwxrwxrwx   0        0        0        0 2021-11-21 02:33:43.755437 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/examplepackage/
--rw-rw-rw-   0        0        0        0 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/examplepackage/__init__.py
--rw-rw-rw-   0        0        0      357 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/examplepackage/example_cython.pxd
--rw-rw-rw-   0        0        0     1592 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/examplepackage/example_cython.pyx
--rw-rw-rw-   0        0        0      189 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/examplepackage/example_cython.pyxbld
--rw-rw-rw-   0        0        0      208 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/module_with_logging.py
--rw-rw-rw-   0        0        0     2009 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/test_logger.py
--rw-rw-rw-   0        0        0     2508 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/test_makeext.py
--rw-rw-rw-   0        0        0     2368 2021-11-21 02:20:22.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/test_version.py
-drwxrwxrwx   0        0        0        0 2021-11-21 02:33:43.755437 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers.egg-info/
--rw-rw-rw-   0        0        0      630 2021-11-21 02:33:43.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1175 2021-11-21 02:33:43.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-21 02:33:43.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-11-21 02:33:43.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2021-11-21 02:33:43.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2021-11-21 02:33:43.000000 cythoninstallhelpers-1.2.1/src/cythoninstallhelpers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 10:31:39.189489 cythoninstallhelpers-1.3.0/
+-rw-rw-rw-   0        0        0      580 2023-04-12 10:31:39.189489 cythoninstallhelpers-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-12 10:31:39.189489 cythoninstallhelpers-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1551 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:31:39.173865 cythoninstallhelpers-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 10:31:39.173865 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/
+-rw-rw-rw-   0        0        0       33 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/_version.py
+-rw-rw-rw-   0        0        0     1168 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/build_config.py
+-rw-rw-rw-   0        0        0     7724 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/configure_logger.py
+-rw-rw-rw-   0        0        0     1171 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/get_version.py
+-rw-rw-rw-   0        0        0     2148 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/make_cython_extensions.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:31:39.189489 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/_version.py
+-rw-rw-rw-   0        0        0       20 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/_version2.py
+-rw-rw-rw-   0        0        0       17 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/_version_broken.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:31:39.189489 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/examplepackage/
+-rw-rw-rw-   0        0        0        0 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/examplepackage/__init__.py
+-rw-rw-rw-   0        0        0      357 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/examplepackage/example_cython.pxd
+-rw-rw-rw-   0        0        0     1592 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/examplepackage/example_cython.pyx
+-rw-rw-rw-   0        0        0      189 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/examplepackage/example_cython.pyxbld
+-rw-rw-rw-   0        0        0      208 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/module_with_logging.py
+-rw-rw-rw-   0        0        0     2312 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/test_logger.py
+-rw-rw-rw-   0        0        0     2508 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/test_makeext.py
+-rw-rw-rw-   0        0        0     2368 2023-04-12 09:48:16.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/test_version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:31:39.173865 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers.egg-info/
+-rw-rw-rw-   0        0        0      580 2023-04-12 10:31:39.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1175 2023-04-12 10:31:39.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 10:31:39.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-12 10:31:39.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-04-12 10:31:39.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-12 10:31:39.000000 cythoninstallhelpers-1.3.0/src/cythoninstallhelpers.egg-info/top_level.txt
```

### Comparing `cythoninstallhelpers-1.2.1/setup.py` & `cythoninstallhelpers-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
 import os
 
 version_dict = dict()
 exec(open(os.path.join(os.path.dirname(__file__),
                        'src',
                        "cythoninstallhelpers",
                        '_version.py')).read(),
@@ -32,15 +32,15 @@
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python',
         'Programming Language :: Cython',
 
     ],
     keywords='cython setuptools',
 
-    packages=find_packages('src', exclude=['ez_setup']),
+    packages=find_namespace_packages('src', exclude=['ez_setup']),
 
     package_dir={'': 'src'},
     package_data={'': ['*.pxd', '*.pyx', '*.pyxbld'],},
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'numpy',
```

### Comparing `cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/build_config.py` & `cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/build_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from typing import List
 import numpy as np
-from distutils.extension import Extension
+from setuptools import Extension
 
 
 if sys.platform == 'win32':
     extra_compile_args = ['/openmp']
     extra_link_args = None
 else:
     # linux
```

### Comparing `cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/configure_logger.py` & `cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/configure_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,20 @@
             instead of from {package} import xyz)'''.format(package=package))
 
         logger = logging.getLogger(caller_name)
         if not logger.handlers:
             logger.addHandler(logging.NullHandler())
         return logger
 
+    def truncate_packages(self):
+        """Delete all loggers for packages"""
+        while self.packages:
+            package_to_remove = self.packages.pop()
+            print(f'remove {package_to_remove}')
+
 
 def get_module_logger(module_name: str) -> logging.Logger:
     """
     create Module logger named after the module
 
     Parameters
     ----------
```

### Comparing `cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/get_version.py` & `cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/get_version.py`

 * *Files identical despite different names*

### Comparing `cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/make_cython_extensions.py` & `cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/make_cython_extensions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import os
-import sys
 from typing import List, Dict
-import numpy as np
-from distutils.extension import Extension
+from setuptools import Extension
 from Cython.Build import cythonize
 
-from .build_config import (extra_compile_args,
-                          extra_link_args,
-                          make_ext,)
+from .build_config import make_ext
 
 
 def make_extensions(ext_modnames: List[str],
                     further_args: Dict[str, str]={},
                     source_dir: str='src',
                     annotate: bool=True,
                     linetrace: bool=True,
```

### Comparing `cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/examplepackage/example_cython.pyx` & `cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/examplepackage/example_cython.pyx`

 * *Files identical despite different names*

### Comparing `cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/test_logger.py` & `cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/test_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,34 @@
 
 from cythoninstallhelpers.configure_logger import (SimLogger,
                                                    get_module_logger,
                                                    get_logger)
 import os
 import glob
 from .module_with_logging import function_with_logging
-from ..get_version import get_version
+from cythoninstallhelpers.get_version import get_version
 
 class Test01_Logger:
     """Test the the SimLogger"""
     def test_01_log_something(self, tmpdir: str):
         """log something to the logger"""
         print(tmpdir)
         scenario = 'TestScenario_without_Packages'
         sim_logger = SimLogger()
+
         sim_logger.configure(LOG_FOLDER=tmpdir, scenario=scenario)
 
+        # create a logger for the 'cythoninstallhelpers'-package
+        logger = get_logger(self)
+        # assert that cythonarrays is registred now
+        assert __package__.split('.')[0] in sim_logger.packages
+
+        # truncate loggers
+        sim_logger.truncate_packages()
+
         # assert that there are no packages registred with the logger
         assert not sim_logger.packages
 
         function_with_logging('Log something in function_with_logging without package')
 
         # assert that cythonarrays is registred now
         assert __package__.split('.')[0] in sim_logger.packages
```

### Comparing `cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/test_makeext.py` & `cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/test_makeext.py`

 * *Files identical despite different names*

### Comparing `cythoninstallhelpers-1.2.1/src/cythoninstallhelpers/tests/test_version.py` & `cythoninstallhelpers-1.3.0/src/cythoninstallhelpers/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `cythoninstallhelpers-1.2.1/src/cythoninstallhelpers.egg-info/SOURCES.txt` & `cythoninstallhelpers-1.3.0/src/cythoninstallhelpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

