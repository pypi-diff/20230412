# Comparing `tmp/autoMMM-0.1.0.tar.gz` & `tmp/autoMMM-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoMMM-0.1.0.tar", last modified: Wed Apr 12 09:27:56 2023, max compression
+gzip compressed data, was "autoMMM-0.1.1.tar", last modified: Wed Apr 12 09:35:13 2023, max compression
```

## Comparing `autoMMM-0.1.0.tar` & `autoMMM-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.327288 autoMMM-0.1.0/
--rw-rw-rw-   0        0        0    10900 2023-04-12 09:27:56.327288 autoMMM-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    10134 2023-04-12 09:24:51.000000 autoMMM-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 09:27:56.327288 autoMMM-0.1.0/autoMMM.egg-info/
--rw-rw-rw-   0        0        0    10900 2023-04-12 09:27:56.000000 autoMMM-0.1.0/autoMMM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-04-12 09:27:56.000000 autoMMM-0.1.0/autoMMM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 09:27:56.000000 autoMMM-0.1.0/autoMMM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-12 09:27:56.000000 autoMMM-0.1.0/autoMMM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 09:27:56.000000 autoMMM-0.1.0/autoMMM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 09:27:56.327288 autoMMM-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      975 2023-04-12 09:20:28.000000 autoMMM-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:35:13.883307 autoMMM-0.1.1/
+-rw-rw-rw-   0        0        0    10898 2023-04-12 09:35:13.883307 autoMMM-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10132 2023-04-12 09:34:42.000000 autoMMM-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 09:35:13.879305 autoMMM-0.1.1/autoMMM.egg-info/
+-rw-rw-rw-   0        0        0    10898 2023-04-12 09:35:13.000000 autoMMM-0.1.1/autoMMM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-04-12 09:35:13.000000 autoMMM-0.1.1/autoMMM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 09:35:13.000000 autoMMM-0.1.1/autoMMM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-12 09:35:13.000000 autoMMM-0.1.1/autoMMM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 09:35:13.000000 autoMMM-0.1.1/autoMMM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 09:35:13.883307 autoMMM-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      975 2023-04-12 09:34:51.000000 autoMMM-0.1.1/setup.py
```

### Comparing `autoMMM-0.1.0/PKG-INFO` & `autoMMM-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMMM
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -93,15 +93,15 @@
 - Throughout this process, the automodeller ensures that it does not overfit the model or select variables that do not make sense in the context of a marketing mix model. The goal is to find a model with the best balance of performance (highest R-squared and lowest AIC) and practical relevance, considering the impact of media channels, price, distribution, and other relevant factors.
 
 ## Limitations and Risks
 - As an experimental library, AutoMMM.ai may produce unexpected or suboptimal results.
 - There is a risk of misuse through looping a self-prompt, which may lead to unintended consequences. Users should exercise caution and be aware of the risks involved.
 - The open source software and 1749.io are not responsible for any misuse of the OpenAI API or any consequences resulting from looping a self-prompt.
 
-# Contributing to AutoMedia.ai
+# Contributing to AutoMMM.ai
 
 Thank you for considering contributing to AutoMMM.ai, We appreciate your interest in making this library better for everyone. Before you start working on your contribution, please familiarize yourself with the following guidelines and processes.
 
 ## Table of Contents
 
 1. [Getting Started](#getting-started)
 2. [Reporting Bugs](#reporting-bugs)
```

### Comparing `autoMMM-0.1.0/README.md` & `autoMMM-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 - Throughout this process, the automodeller ensures that it does not overfit the model or select variables that do not make sense in the context of a marketing mix model. The goal is to find a model with the best balance of performance (highest R-squared and lowest AIC) and practical relevance, considering the impact of media channels, price, distribution, and other relevant factors.
 
 ## Limitations and Risks
 - As an experimental library, AutoMMM.ai may produce unexpected or suboptimal results.
 - There is a risk of misuse through looping a self-prompt, which may lead to unintended consequences. Users should exercise caution and be aware of the risks involved.
 - The open source software and 1749.io are not responsible for any misuse of the OpenAI API or any consequences resulting from looping a self-prompt.
 
-# Contributing to AutoMedia.ai
+# Contributing to AutoMMM.ai
 
 Thank you for considering contributing to AutoMMM.ai, We appreciate your interest in making this library better for everyone. Before you start working on your contribution, please familiarize yourself with the following guidelines and processes.
 
 ## Table of Contents
 
 1. [Getting Started](#getting-started)
 2. [Reporting Bugs](#reporting-bugs)
```

### Comparing `autoMMM-0.1.0/autoMMM.egg-info/PKG-INFO` & `autoMMM-0.1.1/autoMMM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMMM
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -93,15 +93,15 @@
 - Throughout this process, the automodeller ensures that it does not overfit the model or select variables that do not make sense in the context of a marketing mix model. The goal is to find a model with the best balance of performance (highest R-squared and lowest AIC) and practical relevance, considering the impact of media channels, price, distribution, and other relevant factors.
 
 ## Limitations and Risks
 - As an experimental library, AutoMMM.ai may produce unexpected or suboptimal results.
 - There is a risk of misuse through looping a self-prompt, which may lead to unintended consequences. Users should exercise caution and be aware of the risks involved.
 - The open source software and 1749.io are not responsible for any misuse of the OpenAI API or any consequences resulting from looping a self-prompt.
 
-# Contributing to AutoMedia.ai
+# Contributing to AutoMMM.ai
 
 Thank you for considering contributing to AutoMMM.ai, We appreciate your interest in making this library better for everyone. Before you start working on your contribution, please familiarize yourself with the following guidelines and processes.
 
 ## Table of Contents
 
 1. [Getting Started](#getting-started)
 2. [Reporting Bugs](#reporting-bugs)
```

### Comparing `autoMMM-0.1.0/setup.py` & `autoMMM-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="autoMMM",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "scikit-learn",
         "statsmodels",
         "matplotlib",
```

