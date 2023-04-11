# Comparing `tmp/decisionlab-0.0.1b0.tar.gz` & `tmp/decisionlab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decisionlab-0.0.1b0.tar", last modified: Tue Apr 11 23:16:37 2023, max compression
+gzip compressed data, was "decisionlab-0.0.2.tar", last modified: Tue Apr 11 23:27:50 2023, max compression
```

## Comparing `decisionlab-0.0.1b0.tar` & `decisionlab-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:37.337388 decisionlab-0.0.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-11 23:16:37.337388 decisionlab-0.0.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-11 23:16:32.000000 decisionlab-0.0.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:37.337388 decisionlab-0.0.1b0/decisionlab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:32.000000 decisionlab-0.0.1b0/decisionlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-11 23:16:32.000000 decisionlab-0.0.1b0/decisionlab/decision_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:37.337388 decisionlab-0.0.1b0/decisionlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-11 23:16:37.000000 decisionlab-0.0.1b0/decisionlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 23:16:37.000000 decisionlab-0.0.1b0/decisionlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:16:37.000000 decisionlab-0.0.1b0/decisionlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 23:16:37.000000 decisionlab-0.0.1b0/decisionlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 23:16:37.337388 decisionlab-0.0.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-11 23:16:32.000000 decisionlab-0.0.1b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:37.337388 decisionlab-0.0.1b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-11 23:16:32.000000 decisionlab-0.0.1b0/tests/test_decision_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:27:50.798698 decisionlab-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-11 23:27:50.798698 decisionlab-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-11 23:27:47.000000 decisionlab-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:27:50.794697 decisionlab-0.0.2/decisionlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 23:27:47.000000 decisionlab-0.0.2/decisionlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-11 23:27:47.000000 decisionlab-0.0.2/decisionlab/decision_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:27:50.794697 decisionlab-0.0.2/decisionlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-11 23:27:50.000000 decisionlab-0.0.2/decisionlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 23:27:50.000000 decisionlab-0.0.2/decisionlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:27:50.000000 decisionlab-0.0.2/decisionlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 23:27:50.000000 decisionlab-0.0.2/decisionlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 23:27:50.798698 decisionlab-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-11 23:27:47.000000 decisionlab-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:27:50.794697 decisionlab-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-11 23:27:47.000000 decisionlab-0.0.2/tests/test_decision_lab.py
```

### Comparing `decisionlab-0.0.1b0/PKG-INFO` & `decisionlab-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decisionlab
-Version: 0.0.1b0
+Version: 0.0.2
 Summary: A Python package for accessing decision data from JustDecision.com
 Home-page: https://github.com/TuDecides/decisionlab
 Author: decisionLab
 Author-email: jsanchezcastillejos@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -33,17 +33,17 @@
 - Modify the user list in a backend Python code by calling `decision.user_list`, without making changes to the codebase.
 
 ## Getting Started
 
 To get started with `decision_lab`, you need to provide the UUID for accessing decisions. The UUID can be set as an environment variable `DECISION_LAB_UUID` or passed as an argument when creating an instance of the `DecisionLab` class.
 
 ```python
-from decision_lab import DecisionLab
+from decisionlab import DecisionLab
 
 # Create an instance of DecisionLab with UUID
-decision_lab = DecisionLab(uuid='your-uuid')
+decisionlab = DecisionLab(uuid='your-uuid')
 
 # Get the list of decisions
 decisions_list = decision_lab.get_decisions_list()
 
 # Get a specific decision by name
 decision = decision_lab.get_decision('decision_name')
```

### Comparing `decisionlab-0.0.1b0/README.md` & `decisionlab-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 - Modify the user list in a backend Python code by calling `decision.user_list`, without making changes to the codebase.
 
 ## Getting Started
 
 To get started with `decision_lab`, you need to provide the UUID for accessing decisions. The UUID can be set as an environment variable `DECISION_LAB_UUID` or passed as an argument when creating an instance of the `DecisionLab` class.
 
 ```python
-from decision_lab import DecisionLab
+from decisionlab import DecisionLab
 
 # Create an instance of DecisionLab with UUID
-decision_lab = DecisionLab(uuid='your-uuid')
+decisionlab = DecisionLab(uuid='your-uuid')
 
 # Get the list of decisions
 decisions_list = decision_lab.get_decisions_list()
 
 # Get a specific decision by name
 decision = decision_lab.get_decision('decision_name')
```

### Comparing `decisionlab-0.0.1b0/decisionlab/decision_lab.py` & `decisionlab-0.0.2/decisionlab/decision_lab.py`

 * *Files identical despite different names*

### Comparing `decisionlab-0.0.1b0/decisionlab.egg-info/PKG-INFO` & `decisionlab-0.0.2/decisionlab.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decisionlab
-Version: 0.0.1b0
+Version: 0.0.2
 Summary: A Python package for accessing decision data from JustDecision.com
 Home-page: https://github.com/TuDecides/decisionlab
 Author: decisionLab
 Author-email: jsanchezcastillejos@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -33,17 +33,17 @@
 - Modify the user list in a backend Python code by calling `decision.user_list`, without making changes to the codebase.
 
 ## Getting Started
 
 To get started with `decision_lab`, you need to provide the UUID for accessing decisions. The UUID can be set as an environment variable `DECISION_LAB_UUID` or passed as an argument when creating an instance of the `DecisionLab` class.
 
 ```python
-from decision_lab import DecisionLab
+from decisionlab import DecisionLab
 
 # Create an instance of DecisionLab with UUID
-decision_lab = DecisionLab(uuid='your-uuid')
+decisionlab = DecisionLab(uuid='your-uuid')
 
 # Get the list of decisions
 decisions_list = decision_lab.get_decisions_list()
 
 # Get a specific decision by name
 decision = decision_lab.get_decision('decision_name')
```

### Comparing `decisionlab-0.0.1b0/setup.py` & `decisionlab-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="decisionlab",
-    version="0.0.1b",
+    version="0.0.2",
     packages=find_packages(),
     author="decisionLab",
     author_email="jsanchezcastillejos@gmail.com",
     description="A Python package for accessing decision data from JustDecision.com",
     long_description=long_description,  # Add the long_description field
     long_description_content_type="text/markdown",  # Specify the format of the long_description content
     url="https://github.com/TuDecides/decisionlab",
```

### Comparing `decisionlab-0.0.1b0/tests/test_decision_lab.py` & `decisionlab-0.0.2/tests/test_decision_lab.py`

 * *Files identical despite different names*

