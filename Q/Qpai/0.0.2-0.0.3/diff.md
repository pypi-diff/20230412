# Comparing `tmp/Qpai-0.0.2.tar.gz` & `tmp/Qpai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Qpai-0.0.2.tar", last modified: Tue Apr 11 22:10:20 2023, max compression
+gzip compressed data, was "Qpai-0.0.3.tar", last modified: Tue Apr 11 22:39:22 2023, max compression
```

## Comparing `Qpai-0.0.2.tar` & `Qpai-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 22:10:20.813446 Qpai-0.0.2/
--rw-rw-rw-   0        0        0     1064 2023-04-11 18:59:36.000000 Qpai-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      744 2023-04-11 22:10:20.812446 Qpai-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 22:10:20.759184 Qpai-0.0.2/Qpai/
-drwxrwxrwx   0        0        0        0 2023-04-11 22:10:20.810445 Qpai-0.0.2/Qpai/ViT/
--rw-rw-rw-   0        0        0     4573 2023-04-11 22:08:55.000000 Qpai-0.0.2/Qpai/ViT/ViTclassifier.py
--rw-rw-rw-   0        0        0        0 2023-04-11 20:17:50.000000 Qpai-0.0.2/Qpai/ViT/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 18:39:23.000000 Qpai-0.0.2/Qpai/__init__.py
--rw-rw-rw-   0        0        0       50 2023-04-11 18:37:01.000000 Qpai-0.0.2/Qpai/test_one.py
--rw-rw-rw-   0        0        0       41 2023-04-11 18:36:11.000000 Qpai-0.0.2/Qpai/test_trial.py
-drwxrwxrwx   0        0        0        0 2023-04-11 22:10:20.801092 Qpai-0.0.2/Qpai.egg-info/
--rw-rw-rw-   0        0        0      744 2023-04-11 22:10:20.000000 Qpai-0.0.2/Qpai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-04-11 22:10:20.000000 Qpai-0.0.2/Qpai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 22:10:20.000000 Qpai-0.0.2/Qpai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-11 22:10:20.000000 Qpai-0.0.2/Qpai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 22:10:20.000000 Qpai-0.0.2/Qpai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 22:10:20.813446 Qpai-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1094 2023-04-11 22:09:27.000000 Qpai-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:39:22.512360 Qpai-0.0.3/
+-rw-rw-rw-   0        0        0     1064 2023-04-11 18:59:36.000000 Qpai-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      744 2023-04-11 22:39:22.511352 Qpai-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 22:39:22.482068 Qpai-0.0.3/Qpai/
+drwxrwxrwx   0        0        0        0 2023-04-11 22:39:22.510073 Qpai-0.0.3/Qpai/ViT/
+-rw-rw-rw-   0        0        0     4573 2023-04-11 22:36:20.000000 Qpai-0.0.3/Qpai/ViT/ViTclassifier.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:17:50.000000 Qpai-0.0.3/Qpai/ViT/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 18:39:23.000000 Qpai-0.0.3/Qpai/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-04-11 18:37:01.000000 Qpai-0.0.3/Qpai/test_one.py
+-rw-rw-rw-   0        0        0       41 2023-04-11 18:36:11.000000 Qpai-0.0.3/Qpai/test_trial.py
+drwxrwxrwx   0        0        0        0 2023-04-11 22:39:22.508067 Qpai-0.0.3/Qpai.egg-info/
+-rw-rw-rw-   0        0        0      744 2023-04-11 22:39:22.000000 Qpai-0.0.3/Qpai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-04-11 22:39:22.000000 Qpai-0.0.3/Qpai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 22:39:22.000000 Qpai-0.0.3/Qpai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-11 22:39:22.000000 Qpai-0.0.3/Qpai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-11 22:39:22.000000 Qpai-0.0.3/Qpai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 22:39:22.512360 Qpai-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1094 2023-04-11 22:39:04.000000 Qpai-0.0.3/setup.py
```

### Comparing `Qpai-0.0.2/LICENSE` & `Qpai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Qpai-0.0.2/PKG-INFO` & `Qpai-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qpai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Qpai
 Author: Aniket Guchhait
 Author-email: aniket.emailme@gmail.com
 Keywords: quantum,machine learning,quantum computing,qiskit,quantum machine learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Qpai-0.0.2/Qpai/ViT/ViTclassifier.py` & `Qpai-0.0.3/Qpai/ViT/ViTclassifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,16 @@
             
             epoch_train_loss = 0
                 
             y_true_train = []
             y_pred_train = []
 
             loss_hist = {}
-            loss_hist["train accuracy"] = []
-            loss_hist["train loss"] = []
+            loss_hist["train_accuracy"] = []
+            loss_hist["train_loss"] = []
                 
             for batch_idx, (img, labels) in enumerate(self.trainloader):
                 img = img.to(self.device)
                 labels = labels.to(self.device)
                 
                 preds = self.model(img)
```

### Comparing `Qpai-0.0.2/Qpai.egg-info/PKG-INFO` & `Qpai-0.0.3/Qpai.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qpai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Qpai
 Author: Aniket Guchhait
 Author-email: aniket.emailme@gmail.com
 Keywords: quantum,machine learning,quantum computing,qiskit,quantum machine learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Qpai-0.0.2/setup.py` & `Qpai-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Qpai'
 LONG_DESCRIPTION = 'Qpai-Quantum Powered A.I. is an open source library which will be used to develop modern edge Quantum Machine Learning projects.This version includes Vision Transformer model.'
 
 # Setting up
 setup(
     name="Qpai",
     version=VERSION,
```

