# Comparing `tmp/Qpai-0.0.1.tar.gz` & `tmp/Qpai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Qpai-0.0.1.tar", last modified: Tue Apr 11 19:00:59 2023, max compression
+gzip compressed data, was "Qpai-0.0.2.tar", last modified: Tue Apr 11 22:10:20 2023, max compression
```

## Comparing `Qpai-0.0.1.tar` & `Qpai-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 19:00:59.011562 Qpai-0.0.1/
--rw-rw-rw-   0        0        0     1064 2023-04-11 18:59:36.000000 Qpai-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      696 2023-04-11 19:00:59.011562 Qpai-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 19:00:58.980134 Qpai-0.0.1/Qpai/
--rw-rw-rw-   0        0        0        0 2023-04-11 18:39:23.000000 Qpai-0.0.1/Qpai/__init__.py
--rw-rw-rw-   0        0        0       50 2023-04-11 18:37:01.000000 Qpai-0.0.1/Qpai/test_one.py
--rw-rw-rw-   0        0        0       41 2023-04-11 18:36:11.000000 Qpai-0.0.1/Qpai/test_trial.py
-drwxrwxrwx   0        0        0        0 2023-04-11 19:00:59.011562 Qpai-0.0.1/Qpai.egg-info/
--rw-rw-rw-   0        0        0      696 2023-04-11 19:00:58.000000 Qpai-0.0.1/Qpai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2023-04-11 19:00:58.000000 Qpai-0.0.1/Qpai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 19:00:58.000000 Qpai-0.0.1/Qpai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 19:00:58.000000 Qpai-0.0.1/Qpai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 19:00:59.019806 Qpai-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      995 2023-04-11 18:58:00.000000 Qpai-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:10:20.813446 Qpai-0.0.2/
+-rw-rw-rw-   0        0        0     1064 2023-04-11 18:59:36.000000 Qpai-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      744 2023-04-11 22:10:20.812446 Qpai-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 22:10:20.759184 Qpai-0.0.2/Qpai/
+drwxrwxrwx   0        0        0        0 2023-04-11 22:10:20.810445 Qpai-0.0.2/Qpai/ViT/
+-rw-rw-rw-   0        0        0     4573 2023-04-11 22:08:55.000000 Qpai-0.0.2/Qpai/ViT/ViTclassifier.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:17:50.000000 Qpai-0.0.2/Qpai/ViT/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 18:39:23.000000 Qpai-0.0.2/Qpai/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-04-11 18:37:01.000000 Qpai-0.0.2/Qpai/test_one.py
+-rw-rw-rw-   0        0        0       41 2023-04-11 18:36:11.000000 Qpai-0.0.2/Qpai/test_trial.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:10:20.801092 Qpai-0.0.2/Qpai.egg-info/
+-rw-rw-rw-   0        0        0      744 2023-04-11 22:10:20.000000 Qpai-0.0.2/Qpai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-04-11 22:10:20.000000 Qpai-0.0.2/Qpai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 22:10:20.000000 Qpai-0.0.2/Qpai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-11 22:10:20.000000 Qpai-0.0.2/Qpai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-11 22:10:20.000000 Qpai-0.0.2/Qpai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 22:10:20.813446 Qpai-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1094 2023-04-11 22:09:27.000000 Qpai-0.0.2/setup.py
```

### Comparing `Qpai-0.0.1/LICENSE` & `Qpai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Qpai-0.0.1/PKG-INFO` & `Qpai-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: Qpai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Qpai
 Author: Aniket Guchhait
 Author-email: aniket.emailme@gmail.com
 Keywords: quantum,machine learning,quantum computing,qiskit,quantum machine learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Qpai-Quantum Powered A.I. is an open source library which will be used to develop modern edge Quantum Machine Learning projects
+Qpai-Quantum Powered A.I. is an open source library which will be used to develop modern edge Quantum Machine Learning projects.This version includes Vision Transformer model.
```

### Comparing `Qpai-0.0.1/Qpai.egg-info/PKG-INFO` & `Qpai-0.0.2/Qpai.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: Qpai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Qpai
 Author: Aniket Guchhait
 Author-email: aniket.emailme@gmail.com
 Keywords: quantum,machine learning,quantum computing,qiskit,quantum machine learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Qpai-Quantum Powered A.I. is an open source library which will be used to develop modern edge Quantum Machine Learning projects
+Qpai-Quantum Powered A.I. is an open source library which will be used to develop modern edge Quantum Machine Learning projects.This version includes Vision Transformer model.
```

### Comparing `Qpai-0.0.1/setup.py` & `Qpai-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Qpai'
-LONG_DESCRIPTION = 'Qpai-Quantum Powered A.I. is an open source library which will be used to develop modern edge Quantum Machine Learning projects'
+LONG_DESCRIPTION = 'Qpai-Quantum Powered A.I. is an open source library which will be used to develop modern edge Quantum Machine Learning projects.This version includes Vision Transformer model.'
 
 # Setting up
 setup(
     name="Qpai",
     version=VERSION,
     author="Aniket Guchhait",
     author_email="aniket.emailme@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=[],
+    install_requires=['transformer-implementations','numpy','torchvision'],
     keywords=['quantum', 'machine learning', 'quantum computing', 'qiskit', 'quantum machine learning'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

