# Comparing `tmp/autoMMM-0.1.1.tar.gz` & `tmp/autoMMM-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoMMM-0.1.1.tar", last modified: Wed Apr 12 09:35:13 2023, max compression
+gzip compressed data, was "autoMMM-0.1.2.tar", last modified: Wed Apr 12 09:56:32 2023, max compression
```

## Comparing `autoMMM-0.1.1.tar` & `autoMMM-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 09:35:13.883307 autoMMM-0.1.1/
--rw-rw-rw-   0        0        0    10898 2023-04-12 09:35:13.883307 autoMMM-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    10132 2023-04-12 09:34:42.000000 autoMMM-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 09:35:13.879305 autoMMM-0.1.1/autoMMM.egg-info/
--rw-rw-rw-   0        0        0    10898 2023-04-12 09:35:13.000000 autoMMM-0.1.1/autoMMM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-04-12 09:35:13.000000 autoMMM-0.1.1/autoMMM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 09:35:13.000000 autoMMM-0.1.1/autoMMM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-12 09:35:13.000000 autoMMM-0.1.1/autoMMM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 09:35:13.000000 autoMMM-0.1.1/autoMMM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 09:35:13.883307 autoMMM-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      975 2023-04-12 09:34:51.000000 autoMMM-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:56:32.586598 autoMMM-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-04-12 09:56:32.548220 autoMMM-0.1.2/AutoMMM/
+-rw-rw-rw-   0        0        0        0 2023-04-08 15:41:28.000000 autoMMM-0.1.2/AutoMMM/__init__.py
+-rw-rw-rw-   0        0        0    11953 2023-04-12 09:27:13.000000 autoMMM-0.1.2/AutoMMM/automodeller.py
+-rw-rw-rw-   0        0        0    10898 2023-04-12 09:56:32.581001 autoMMM-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10132 2023-04-12 09:34:42.000000 autoMMM-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 09:56:32.581001 autoMMM-0.1.2/autoMMM.egg-info/
+-rw-rw-rw-   0        0        0    10898 2023-04-12 09:56:32.000000 autoMMM-0.1.2/autoMMM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-04-12 09:56:32.000000 autoMMM-0.1.2/autoMMM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 09:56:32.000000 autoMMM-0.1.2/autoMMM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-12 09:56:32.000000 autoMMM-0.1.2/autoMMM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-12 09:56:32.000000 autoMMM-0.1.2/autoMMM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 09:56:32.586598 autoMMM-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      975 2023-04-12 09:55:16.000000 autoMMM-0.1.2/setup.py
```

### Comparing `autoMMM-0.1.1/PKG-INFO` & `autoMMM-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMMM
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `autoMMM-0.1.1/README.md` & `autoMMM-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `autoMMM-0.1.1/autoMMM.egg-info/PKG-INFO` & `autoMMM-0.1.2/autoMMM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMMM
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `autoMMM-0.1.1/setup.py` & `autoMMM-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="autoMMM",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "scikit-learn",
         "statsmodels",
         "matplotlib",
```

