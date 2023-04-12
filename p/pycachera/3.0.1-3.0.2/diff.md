# Comparing `tmp/pycachera-3.0.1.tar.gz` & `tmp/pycachera-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycachera-3.0.1.tar", last modified: Wed Apr 12 03:30:48 2023, max compression
+gzip compressed data, was "pycachera-3.0.2.tar", last modified: Wed Apr 12 03:37:45 2023, max compression
```

## Comparing `pycachera-3.0.1.tar` & `pycachera-3.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:30:48.423467 pycachera-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-04-12 03:30:36.000000 pycachera-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-04-12 03:30:48.423467 pycachera-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-04-12 03:30:36.000000 pycachera-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:30:48.423467 pycachera-3.0.1/pycachera/
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-12 03:30:36.000000 pycachera-3.0.1/pycachera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-12 03:30:36.000000 pycachera-3.0.1/pycachera/cacher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:30:48.423467 pycachera-3.0.1/pycachera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-04-12 03:30:48.000000 pycachera-3.0.1/pycachera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-04-12 03:30:48.000000 pycachera-3.0.1/pycachera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 03:30:48.000000 pycachera-3.0.1/pycachera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-12 03:30:48.000000 pycachera-3.0.1/pycachera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-12 03:30:48.000000 pycachera-3.0.1/pycachera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 03:30:48.423467 pycachera-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-12 03:30:36.000000 pycachera-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:37:45.947222 pycachera-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-04-12 03:37:36.000000 pycachera-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-04-12 03:37:45.947222 pycachera-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-04-12 03:37:36.000000 pycachera-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:37:45.947222 pycachera-3.0.2/pycachera/
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-12 03:37:36.000000 pycachera-3.0.2/pycachera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-12 03:37:36.000000 pycachera-3.0.2/pycachera/cacher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:37:45.947222 pycachera-3.0.2/pycachera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-04-12 03:37:45.000000 pycachera-3.0.2/pycachera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-04-12 03:37:45.000000 pycachera-3.0.2/pycachera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 03:37:45.000000 pycachera-3.0.2/pycachera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-12 03:37:45.000000 pycachera-3.0.2/pycachera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-12 03:37:45.000000 pycachera-3.0.2/pycachera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 03:37:45.947222 pycachera-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-04-12 03:37:36.000000 pycachera-3.0.2/setup.py
```

### Comparing `pycachera-3.0.1/LICENSE` & `pycachera-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycachera-3.0.1/README.md` & `pycachera-3.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -80,12 +80,25 @@
        self.c = c
    
    @cache(extrarg=['c'])
    def sum(a,b):
       return a + b  
 ```
 
+To cache a class property,
+```
+class math:
+    def __init__(self,a,b):
+        self.a = a
+        self.b = b
+    
+    @property
+    @cache(extrarg=['a','b'],verbose=True)
+    def add(self):
+        return self.a + self.b
+```
+
 
 
 ## API
 
 visit [pycachera.readthedocs.io](https://pycachera.readthedocs.io/en/latest/)
```

### Comparing `pycachera-3.0.1/pycachera/cacher.py` & `pycachera-3.0.2/pycachera/cacher.py`

 * *Files identical despite different names*

### Comparing `pycachera-3.0.1/setup.py` & `pycachera-3.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from distutils.core import setup
 
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 files = ["pycachera/*"]
 setup(
         name = 'pycachera',
         packages = ['pycachera'],
         package_data = {'pycachera' : files },
-        version = '3.0.1',
+        version = '3.0.2',
         install_requires = ['numpy','pandas'],
         description = 'A powerfull python caching tool',
         author = 'Anto Idicherian Lonappan',
         author_email = 'mail@antolonappan.me',
         url = 'https://github.com/antolonappan/pycachera',
+        long_description=long_description,
         long_description_content_type="text/markdown",
         )
```

