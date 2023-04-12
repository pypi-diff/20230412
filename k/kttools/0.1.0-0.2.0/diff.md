# Comparing `tmp/kttools-0.1.0.tar.gz` & `tmp/kttools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kttools-0.1.0.tar", max compression
+gzip compressed data, was "kttools-0.2.0.tar", max compression
```

## Comparing `kttools-0.1.0.tar` & `kttools-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      978 2023-04-11 22:21:48.851619 kttools-0.1.0/README.md
--rw-r--r--   0        0        0      718 2023-04-11 23:11:49.344181 kttools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      457 2023-04-11 12:10:45.033626 kttools-0.1.0/tools/__init__.py
--rw-r--r--   0        0        0      366 2023-04-11 12:10:45.033839 kttools-0.1.0/tools/sc/__init__.py
--rw-r--r--   0        0        0    12358 2023-04-11 12:10:45.034030 kttools-0.1.0/tools/sc/_sc.py
--rw-r--r--   0        0        0      429 2023-04-11 12:10:45.034250 kttools-0.1.0/tools/tools/__init__.py
--rw-r--r--   0        0        0     8879 2023-04-11 12:10:45.034425 kttools-0.1.0/tools/tools/_tools.py
--rw-r--r--   0        0        0     1863 1970-01-01 00:00:00.000000 kttools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-12 06:12:13.687609 kttools-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1538 2023-04-12 06:12:13.687609 kttools-0.2.0/README.rst
+-rw-r--r--   0        0        0     1084 2023-04-12 06:12:13.687609 kttools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-04-12 06:12:13.687609 kttools-0.2.0/tools/__init__.py
+-rw-r--r--   0        0        0      366 2023-04-12 06:12:13.687609 kttools-0.2.0/tools/sc/__init__.py
+-rw-r--r--   0        0        0    12358 2023-04-12 06:12:13.687609 kttools-0.2.0/tools/sc/_sc.py
+-rw-r--r--   0        0        0      429 2023-04-12 06:12:13.687609 kttools-0.2.0/tools/tools/__init__.py
+-rw-r--r--   0        0        0     8879 2023-04-12 06:12:13.687609 kttools-0.2.0/tools/tools/_tools.py
+-rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 kttools-0.2.0/PKG-INFO
```

### Comparing `kttools-0.1.0/tools/sc/_sc.py` & `kttools-0.2.0/tools/sc/_sc.py`

 * *Files identical despite different names*

### Comparing `kttools-0.1.0/tools/tools/_tools.py` & `kttools-0.2.0/tools/tools/_tools.py`

 * *Files identical despite different names*

### Comparing `kttools-0.1.0/PKG-INFO` & `kttools-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,97 @@
 Metadata-Version: 2.1
 Name: kttools
-Version: 0.1.0
+Version: 0.2.0
 Summary: Kelvin's miscellaneous tools for python
 License: MIT
 Author: Zewen Kelvin Tuong
 Author-email: z.tuong@uq.edu.au
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
+Provides-Extra: docs
 Requires-Dist: anndata (>=0.7.6,<0.8.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: numpy (>=1.21.6,<2.0.0)
 Requires-Dist: pandas (>=1.2.4,<2.0.0)
+Requires-Dist: readthedocs-sphinx-ext ; extra == "docs"
+Requires-Dist: recommonmark ; extra == "docs"
 Requires-Dist: scanpy (>=1.7.1,<2.0.0)
-Description-Content-Type: text/markdown
+Requires-Dist: sphinx-autodoc-typehints ; extra == "docs"
+Requires-Dist: sphinx_rtd_theme ; extra == "docs"
+Description-Content-Type: text/x-rst
 
-# tools
-Miscellaneous python tools
+|Docs| |PyPI|
 
+kttools
+=======
 
-### Install
-```bash
-pip install kttools
-
-# or 
-pip install git+https://github.com/zktuong/kttools.git
-
-# or
-git clone https://github.com/zktuong/kttools.git
-cd kttools; pip install -e .
-```
-
-### Usage
-```python
-import tools
-```
-
-
-### jupyterhub issue
-
-On jupyterhub, If you find yourself trying to import from local directory, i.e. `git clone`, and finding that you can't import it, you will need to edit your your `kernel.json` file like so:
-
-```bash
-vi /home/jovyan/.local/share/jupyter/kernels/<condaenvironmentname>/kernel.json 
-```
-
-add in the `$PATH` and `$PYTHONPATH` bits:
-```bash
-{
- "argv": [
-  "/home/jovyan/my-conda-envs/<condaenvironmentname>/bin/python",
-  "-m",
-  "ipykernel_launcher",
-  "-f",
-  "{connection_file}"
- ],
- "env": {
-     "PATH": "/home/jovyan/scripts/kttools:$PATH",
-     "PYTHONPATH": "/home/jovyan/scripts/kttools:$PYTHONPATH"
- },
- "display_name": "Python (<condaenvironmentname>)",
- "language": "python"
-}
-```
+Kelvin’s miscellaneous python tools
+
+Install
+~~~~~~~
+
+.. code:: bash
+
+   pip install kttools
+
+   # or 
+   pip install git+https://github.com/zktuong/kttools.git
+
+   # or
+   git clone https://github.com/zktuong/kttools.git
+   cd kttools; pip install -e .
+
+Usage
+~~~~~
+
+.. code:: python
+
+   import tools 
+
+Please checkout the documentation
+`api <https://kttools.readthedocs.org>`__ for details about the
+functions you can use to make your life easier.
+
+jupyterhub issue
+~~~~~~~~~~~~~~~~
+
+On jupyterhub, If you find yourself trying to import from local
+directory, i.e. ``git clone``, and finding that you can’t import it, you
+will need to edit your your ``kernel.json`` file like so:
+
+.. code:: bash
+
+   vi /home/jovyan/.local/share/jupyter/kernels/<condaenvironmentname>/kernel.json 
+
+add in the ``$PATH`` and ``$PYTHONPATH`` bits:
+
+.. code:: bash
+
+   {
+    "argv": [
+     "/home/jovyan/my-conda-envs/<condaenvironmentname>/bin/python",
+     "-m",
+     "ipykernel_launcher",
+     "-f",
+     "{connection_file}"
+    ],
+    "env": {
+        "PATH": "/home/jovyan/scripts/kttools:$PATH",
+        "PYTHONPATH": "/home/jovyan/scripts/kttools:$PYTHONPATH"
+    },
+    "display_name": "Python (<condaenvironmentname>)",
+    "language": "python"
+   }
+
+.. |Docs| image:: https://readthedocs.org/projects/kttools/badge/?version=latest
+   :target: https://kttools.readthedocs.io/en/latest/?badge=latest
+.. |PyPI| image:: https://img.shields.io/pypi/v/kttools?logo=PyPI
+   :target: https://pypi.org/project/kttools/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

