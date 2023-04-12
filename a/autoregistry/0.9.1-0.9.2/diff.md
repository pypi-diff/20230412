# Comparing `tmp/autoregistry-0.9.1.tar.gz` & `tmp/autoregistry-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoregistry-0.9.1.tar", max compression
+gzip compressed data, was "autoregistry-0.9.2.tar", max compression
```

## Comparing `autoregistry-0.9.1.tar` & `autoregistry-0.9.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-02-22 20:52:15.469758 autoregistry-0.9.1/LICENSE
--rw-r--r--   0        0        0     4730 2023-02-22 20:52:15.469758 autoregistry-0.9.1/README.rst
--rw-r--r--   0        0        0      374 2023-02-22 20:52:35.829794 autoregistry-0.9.1/autoregistry/__init__.py
--rw-r--r--   0        0        0     2537 2023-02-22 20:52:15.469758 autoregistry-0.9.1/autoregistry/config.py
--rw-r--r--   0        0        0      592 2023-02-22 20:52:15.473758 autoregistry-0.9.1/autoregistry/exceptions.py
--rw-r--r--   0        0        0      693 2023-02-22 20:52:15.473758 autoregistry-0.9.1/autoregistry/regex.py
--rw-r--r--   0        0        0    12273 2023-02-22 20:52:15.473758 autoregistry-0.9.1/autoregistry/registry.py
--rw-r--r--   0        0        0     1685 2023-02-22 20:52:35.829794 autoregistry-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 autoregistry-0.9.1/setup.py
--rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 autoregistry-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-25 01:09:51.783225 autoregistry-0.9.2/LICENSE
+-rw-r--r--   0        0        0     4730 2023-02-25 01:09:51.783225 autoregistry-0.9.2/README.rst
+-rw-r--r--   0        0        0      534 2023-02-25 01:10:12.106982 autoregistry-0.9.2/autoregistry/__init__.py
+-rw-r--r--   0        0        0     2537 2023-02-25 01:09:51.783225 autoregistry-0.9.2/autoregistry/config.py
+-rw-r--r--   0        0        0      592 2023-02-25 01:09:51.783225 autoregistry-0.9.2/autoregistry/exceptions.py
+-rw-r--r--   0        0        0        0 2023-02-25 01:09:51.783225 autoregistry-0.9.2/autoregistry/py.typed
+-rw-r--r--   0        0        0      693 2023-02-25 01:09:51.783225 autoregistry-0.9.2/autoregistry/regex.py
+-rw-r--r--   0        0        0    12273 2023-02-25 01:09:51.783225 autoregistry-0.9.2/autoregistry/registry.py
+-rw-r--r--   0        0        0     1685 2023-02-25 01:10:12.102982 autoregistry-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 autoregistry-0.9.2/setup.py
+-rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 autoregistry-0.9.2/PKG-INFO
```

### Comparing `autoregistry-0.9.1/LICENSE` & `autoregistry-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autoregistry-0.9.1/README.rst` & `autoregistry-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `autoregistry-0.9.1/autoregistry/config.py` & `autoregistry-0.9.2/autoregistry/config.py`

 * *Files identical despite different names*

### Comparing `autoregistry-0.9.1/autoregistry/exceptions.py` & `autoregistry-0.9.2/autoregistry/exceptions.py`

 * *Files identical despite different names*

### Comparing `autoregistry-0.9.1/autoregistry/regex.py` & `autoregistry-0.9.2/autoregistry/regex.py`

 * *Files identical despite different names*

### Comparing `autoregistry-0.9.1/autoregistry/registry.py` & `autoregistry-0.9.2/autoregistry/registry.py`

 * *Files identical despite different names*

### Comparing `autoregistry-0.9.1/pyproject.toml` & `autoregistry-0.9.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "autoregistry"
-version = "0.9.1"  # Do not change, let poetry-dynamic-versioning handle it.
+version = "0.9.2"  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/BrianPugh/autoregistry"
 repository = "https://github.com/BrianPugh/autoregistry"
 license = "Apache-2.0"
 description = "Automatic registry design-pattern for mapping names to functionality."
 authors = ["Brian Pugh"]
 readme = "README.rst"
 packages = [{include = "autoregistry"}]
```

### Comparing `autoregistry-0.9.1/setup.py` & `autoregistry-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['autoregistry']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'autoregistry',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'Automatic registry design-pattern for mapping names to functionality.',
     'long_description': '.. image:: https://raw.githubusercontent.com/BrianPugh/autoregistry/main/assets/logo_400w.png\n\n|Python compat| |PyPi| |GHA tests| |Codecov report| |readthedocs|\n\n.. inclusion-marker-do-not-remove\n\nAutoRegistry\n============\n\nInvoking functions and class-constructors from a string is a common design pattern\nthat AutoRegistry aims to solve.\nFor example, a user might specify a backend of type ``"sqlite"`` in a yaml configuration\nfile, for which our program needs to construct the ``SQLite`` subclass of our ``Database`` class.\nClassically, you would need to manually create a lookup, mapping the string ``"sqlite"`` to\nthe ``SQLite`` constructor.\nWith AutoRegistry, the lookup is automatically created for you.\n\n\nAutoRegistry has a single  powerful class ``Registry`` that can do the following:\n\n* Be inherited to automatically register subclasses by their name.\n\n* Be directly invoked ``my_registery = Registry()`` to create a decorator\n  for registering callables like functions.\n\n* Traverse and automatically create registries for other python libraries.\n\n.. inclusion-marker-remove\n\nAutoRegistry is also highly configurable, with features like name-schema-enforcement and name-conversion-rules.\n`Checkout the docs for more information <https://autoregistry.readthedocs.io/en/latest/?badge=latest/>`_.\n\n`Watch AutoRegistry in action! <https://youtu.be/4No_NE7bUOM>`_\n\nInstallation\n============\nAutoRegistry requires Python ``>=3.8``.\n\n.. code-block:: bash\n\n   python -m pip install autoregistry\n\n\nExamples\n========\n\nClass Inheritance\n^^^^^^^^^^^^^^^^^\n\n``Registry`` adds a dictionary-like interface to class constructors\nfor looking up subclasses.\n\n.. code-block:: python\n\n   from abc import abstractmethod\n   from dataclasses import dataclass\n   from autoregistry import Registry\n\n\n   @dataclass\n   class Pokemon(Registry):\n       level: int\n       hp: int\n\n       @abstractmethod\n       def attack(self, target):\n           """Attack another Pokemon."""\n\n\n   class Charmander(Pokemon):\n       def attack(self, target):\n           return 1\n\n\n   class Pikachu(Pokemon):\n       def attack(self, target):\n           return 2\n\n\n   class SurfingPikachu(Pikachu):\n       def attack(self, target):\n           return 3\n\n\n   print(f"{len(Pokemon)} Pokemon types registered:")\n   print(f"    {list(Pokemon)}")\n   # By default, lookup is case-insensitive\n   charmander = Pokemon["cHaRmAnDer"](level=7, hp=31)\n   print(f"Created Pokemon: {charmander}")\n\nThis code block produces the following output:\n\n.. code-block::\n\n   3 Pokemon types registered:\n       [\'charmander\', \'pikachu\', \'surfingpikachu\']\n   Created Pokemon: Charmander(level=7, hp=31)\n\n\nFunction Registry\n^^^^^^^^^^^^^^^^^\n\nDirectly instantiating a ``Registry`` object allows you to\nregister functions by decorating them.\n\n.. code-block:: python\n\n   from autoregistry import Registry\n\n   pokeballs = Registry()\n\n\n   @pokeballs\n   def masterball(target):\n       return 1.0\n\n\n   @pokeballs\n   def pokeball(target):\n       return 0.1\n\n\n   for ball in ["pokeball", "masterball"]:\n       success_rate = pokeballs[ball](None)\n       print(f"Ash used {ball} and had {success_rate=}")\n\nThis code block produces the following output:\n\n.. code-block:: text\n\n   Ash used pokeball and had success_rate=0.1\n   Ash used masterball and had success_rate=1.0\n\n\nModule Registry\n^^^^^^^^^^^^^^^\n\nCreate a registry for another python module.\n\n.. code-block:: python\n\n   import torch\n   from autoregistry import Registry\n\n   optims = Registry(torch.optim)\n\n   # "adamw" and ``lr`` could be coming from a configuration file.\n   optimizer = optims["adamw"](model.parameters(), lr=3e-3)\n\n   assert list(optims) == [\n       "asgd",\n       "adadelta",\n       "adagrad",\n       "adam",\n       "adamw",\n       "adamax",\n       "lbfgs",\n       "nadam",\n       "optimizer",\n       "radam",\n       "rmsprop",\n       "rprop",\n       "sgd",\n       "sparseadam",\n       "lr_scheduler",\n       "swa_utils",\n   ]\n\n\n.. |GHA tests| image:: https://github.com/BrianPugh/autoregistry/workflows/tests/badge.svg\n   :target: https://github.com/BrianPugh/autoregistry/actions?query=workflow%3Atests\n   :alt: GHA Status\n.. |Codecov report| image:: https://codecov.io/github/BrianPugh/autoregistry/coverage.svg?branch=main\n   :target: https://codecov.io/github/BrianPugh/autoregistry?branch=main\n   :alt: Coverage\n.. |readthedocs| image:: https://readthedocs.org/projects/autoregistry/badge/?version=latest\n        :target: https://autoregistry.readthedocs.io/en/latest/?badge=latest\n        :alt: Documentation Status\n.. |Python compat| image:: https://img.shields.io/badge/>=python-3.8-blue.svg\n.. |PyPi| image:: https://img.shields.io/pypi/v/autoregistry.svg\n        :target: https://pypi.python.org/pypi/autoregistry\n',
     'author': 'Brian Pugh',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/BrianPugh/autoregistry',
```

### Comparing `autoregistry-0.9.1/PKG-INFO` & `autoregistry-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoregistry
-Version: 0.9.1
+Version: 0.9.2
 Summary: Automatic registry design-pattern for mapping names to functionality.
 Home-page: https://github.com/BrianPugh/autoregistry
 License: Apache-2.0
 Author: Brian Pugh
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

