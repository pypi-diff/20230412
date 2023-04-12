# Comparing `tmp/e2xgradingtools-0.0.1.tar.gz` & `tmp/e2xgradingtools-0.0.2.tar.gz`

## Comparing `e2xgradingtools-0.0.1.tar` & `e2xgradingtools-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    15537 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/E2X_Grading_Tools.ipynb
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/docs/make.bat
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/docs/source/conf.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/docs/source/index.rst
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/docs/source/user_guide/comparators.rst
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/docs/source/user_guide/functions.rst
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/docs/source/user_guide/highlights.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/docs/source/user_guide/installation.rst
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/docs/source/user_guide/misc.rst
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/docs/source/user_guide/variables.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/e2xgradingtools/__init__.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/e2xgradingtools/base.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/e2xgradingtools/classes.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/e2xgradingtools/comparators.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/e2xgradingtools/decorators.py
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/e2xgradingtools/functions.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/e2xgradingtools/utils.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/e2xgradingtools/variables.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/LICENSE
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15537 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/E2X_Grading_Tools.ipynb
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/docs/make.bat
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/docs/source/index.rst
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/docs/source/user_guide/comparators.rst
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/docs/source/user_guide/functions.rst
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/docs/source/user_guide/highlights.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/docs/source/user_guide/installation.rst
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/docs/source/user_guide/misc.rst
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/docs/source/user_guide/variables.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/e2xgradingtools/__init__.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/e2xgradingtools/base.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/e2xgradingtools/classes.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/e2xgradingtools/comparators.py
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/e2xgradingtools/decorators.py
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/e2xgradingtools/functions.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/e2xgradingtools/utils.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/e2xgradingtools/variables.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/LICENSE
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 e2xgradingtools-0.0.2/PKG-INFO
```

### Comparing `e2xgradingtools-0.0.1/E2X_Grading_Tools.ipynb` & `e2xgradingtools-0.0.2/E2X_Grading_Tools.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/docs/Makefile` & `e2xgradingtools-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/docs/make.bat` & `e2xgradingtools-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/docs/source/conf.py` & `e2xgradingtools-0.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/docs/source/user_guide/comparators.rst` & `e2xgradingtools-0.0.2/docs/source/user_guide/comparators.rst`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/docs/source/user_guide/functions.rst` & `e2xgradingtools-0.0.2/docs/source/user_guide/functions.rst`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/docs/source/user_guide/highlights.rst` & `e2xgradingtools-0.0.2/docs/source/user_guide/highlights.rst`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/docs/source/user_guide/misc.rst` & `e2xgradingtools-0.0.2/docs/source/user_guide/misc.rst`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/docs/source/user_guide/variables.rst` & `e2xgradingtools-0.0.2/docs/source/user_guide/variables.rst`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/e2xgradingtools/classes.py` & `e2xgradingtools-0.0.2/e2xgradingtools/classes.py`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/e2xgradingtools/decorators.py` & `e2xgradingtools-0.0.2/e2xgradingtools/decorators.py`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/e2xgradingtools/functions.py` & `e2xgradingtools-0.0.2/e2xgradingtools/functions.py`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/e2xgradingtools/variables.py` & `e2xgradingtools-0.0.2/e2xgradingtools/variables.py`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/.gitignore` & `e2xgradingtools-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/LICENSE` & `e2xgradingtools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `e2xgradingtools-0.0.1/pyproject.toml` & `e2xgradingtools-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "e2xgradingtools"
-version = "0.0.1"
+version = "0.0.2"
 description = "A package for creating autograder tests in Jupyter notebooks"
 readme = "README.md"
 requires-python = ">3.7"
 license = "MIT"
 authors = [
     { name = "Tim Metzler", email = "tim.metzler@h-brs.de"}
 ]
@@ -28,10 +28,10 @@
     "hatchling",
     "pre-commit",
     "sphinx",
     "sphinx-rtd-theme"
 ]
 
 [project.urls]
-Documentation = "https://e2xgradingtools.readthedocs.io"
+Documentation = "https://e2x-grading-tools.readthedocs.io"
 Issues = "https://github.com/Digiklausur/e2xgradingtools/issues"
 Source = "https://github.com/Digiklausur/e2xgradingtools"
```

### Comparing `e2xgradingtools-0.0.1/PKG-INFO` & `e2xgradingtools-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: e2xgradingtools
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for creating autograder tests in Jupyter notebooks
-Project-URL: Documentation, https://e2xgradingtools.readthedocs.io
+Project-URL: Documentation, https://e2x-grading-tools.readthedocs.io
 Project-URL: Issues, https://github.com/Digiklausur/e2xgradingtools/issues
 Project-URL: Source, https://github.com/Digiklausur/e2xgradingtools
 Author-email: Tim Metzler <tim.metzler@h-brs.de>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,8 +21,8 @@
 Requires-Dist: sphinx; extra == 'dev'
 Requires-Dist: sphinx-rtd-theme; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # e2xgradingtools
 Python package to write test cases for Jupyter Notebook assignments
 
-Please consult the [docs](https://e2xgradingtools.readthedocs.io/en/latest) and look at the example notebook in this repository.
+Please consult the [docs](https://e2x-grading-tools.readthedocs.io/en/latest) and look at the example notebook in this repository.
```

