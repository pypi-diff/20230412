# Comparing `tmp/ipydrawio-widgets-1.2.2.tar.gz` & `tmp/ipydrawio-widgets-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipydrawio-widgets-1.2.2.tar", last modified: Tue Nov  8 14:38:41 2022, max compression
+gzip compressed data, was "ipydrawio-widgets-1.3.0.tar", last modified: Tue Apr 11 21:50:00 2023, max compression
```

## Comparing `ipydrawio-widgets-1.2.2.tar` & `ipydrawio-widgets-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:38:41.108272 ipydrawio-widgets-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4383 2022-11-08 14:38:41.108272 ipydrawio-widgets-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3061 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1784 2022-11-08 14:38:41.108272 ipydrawio-widgets-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:38:41.104272 ipydrawio-widgets-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:38:41.104272 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:38:41.104272 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/js/
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/js/package.json
--rw-r--r--   0 runner    (1001) docker     (121)    35533 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/js/plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     3413 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/widget_diagram.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:38:41.104272 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4383 2022-11-08 14:38:41.000000 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-11-08 14:38:41.000000 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 14:38:41.000000 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 14:38:41.000000 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-11-08 14:38:41.000000 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-08 14:38:41.000000 ipydrawio-widgets-1.2.2/src/ipydrawio_widgets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:38:41.104272 ipydrawio-widgets-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-11-08 14:37:20.000000 ipydrawio-widgets-1.2.2/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:50:00.592162 ipydrawio-widgets-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-11 21:50:00.592162 ipydrawio-widgets-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-11 21:50:00.592162 ipydrawio-widgets-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:50:00.576162 ipydrawio-widgets-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:50:00.584162 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:50:00.588162 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/js/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35047 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/js/plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/widget_diagram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:50:00.588162 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-11 21:50:00.000000 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-11 21:50:00.000000 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:50:00.000000 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:50:00.000000 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-11 21:50:00.000000 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 21:50:00.000000 ipydrawio-widgets-1.3.0/src/ipydrawio_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:50:00.592162 ipydrawio-widgets-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-11 21:49:16.000000 ipydrawio-widgets-1.3.0/tests/test_widgets.py
```

### Comparing `ipydrawio-widgets-1.2.2/LICENSE.txt` & `ipydrawio-widgets-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipydrawio-widgets-1.2.2/PKG-INFO` & `ipydrawio-widgets-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: ipydrawio-widgets
-Version: 1.2.2
+Version: 1.3.0
 Summary: Draw.io Diagrams as Jupyter Widgets (Kernel-only)
 Home-page: https://ipydrawio.rtfd.io
 Author: ipydrawio Contributors
 Author-email: ripxl@example.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/deathbeds/ipydrawio/issues
-Project-URL: Changelog, https://github.com/deathbeds/ipydrawio/blob/master/CHANGELOG.md
+Project-URL: Changelog, https://github.com/deathbeds/ipydrawio/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://app.codecov.io/gh/deathbeds/ipydrawio
 Project-URL: Documentation, https://ipydrawio.rtfd.io
 Project-URL: Source Code, https://github.com/deathbeds/ipydrawio
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # IPyDrawio Widgets
 
 [![docs][docs-badge]][docs] [![binder-badge][]][binder]
@@ -79,15 +78,15 @@
 For more, see the documentation
 
 ## Open Source
 
 This work is licensed under the [Apache-2.0] License.
 
 ```
-Copyright 2022 ipydrawio contributors
+Copyright 2023 ipydrawio contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
   http://www.apache.org/licenses/LICENSE-2.0
 
@@ -95,27 +94,27 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 
 [apache-2.0]:
-  https://github.com/deathbeds/ipydrawio/blob/master/py_packages/ipydrawio-widgets/LICENSE.txt
+  https://github.com/deathbeds/ipydrawio/blob/main/py_packages/ipydrawio-widgets/LICENSE.txt
 [binder]:
-  http://mybinder.org/v2/gh/deathbeds/ipydrawio/master?urlpath=lab/tree/docs/Poster.dio.svg
+  http://mybinder.org/v2/gh/deathbeds/ipydrawio/main?urlpath=lab/tree/docs/Poster.dio.svg
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [cov-badge]:
-  https://codecov.io/gh/deathbeds/ipydrawio/branch/master/graph/badge.svg?token=9B74VKHQDK
+  https://codecov.io/gh/deathbeds/ipydrawio/branch/main/graph/badge.svg?token=9B74VKHQDK
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [pypi-badge]: https://img.shields.io/pypi/v/ipydrawio-widgets
 [pypi]: https://pypi.org/project/ipydrawio-widgets
 [conda-badge]: https://img.shields.io/conda/vn/conda-forge/ipydrawio-widgets
 [conda]: https://anaconda.org/conda-forge/ipydrawio-widgets
 [workflow-badge]:
   https://github.com/deathbeds/ipydrawio/workflows/.github/workflows/ci.yml/badge.svg
 [workflow]:
-  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amaster+workflow%3A.github%2Fworkflows%2Fci.yml
+  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amain+workflow%3A.github%2Fworkflows%2Fci.yml
 [cov-badge]:
-  https://codecov.io/gh/deathbeds/ipydrawio/branch/master/graph/badge.svg?token=9B74VKHQDK
+  https://codecov.io/gh/deathbeds/ipydrawio/branch/main/graph/badge.svg?token=9B74VKHQDK
 [cov]: https://codecov.io/gh/deathbeds/ipydrawio
 [docs-badge]: https://readthedocs.org/projects/ipydrawio/badge/?version=latest
 [docs]: https://ipydrawio.rtfd.io
```

### Comparing `ipydrawio-widgets-1.2.2/README.md` & `ipydrawio-widgets-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 For more, see the documentation
 
 ## Open Source
 
 This work is licensed under the [Apache-2.0] License.
 
 ```
-Copyright 2022 ipydrawio contributors
+Copyright 2023 ipydrawio contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
   http://www.apache.org/licenses/LICENSE-2.0
 
@@ -64,27 +64,27 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 
 [apache-2.0]:
-  https://github.com/deathbeds/ipydrawio/blob/master/py_packages/ipydrawio-widgets/LICENSE.txt
+  https://github.com/deathbeds/ipydrawio/blob/main/py_packages/ipydrawio-widgets/LICENSE.txt
 [binder]:
-  http://mybinder.org/v2/gh/deathbeds/ipydrawio/master?urlpath=lab/tree/docs/Poster.dio.svg
+  http://mybinder.org/v2/gh/deathbeds/ipydrawio/main?urlpath=lab/tree/docs/Poster.dio.svg
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [cov-badge]:
-  https://codecov.io/gh/deathbeds/ipydrawio/branch/master/graph/badge.svg?token=9B74VKHQDK
+  https://codecov.io/gh/deathbeds/ipydrawio/branch/main/graph/badge.svg?token=9B74VKHQDK
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [pypi-badge]: https://img.shields.io/pypi/v/ipydrawio-widgets
 [pypi]: https://pypi.org/project/ipydrawio-widgets
 [conda-badge]: https://img.shields.io/conda/vn/conda-forge/ipydrawio-widgets
 [conda]: https://anaconda.org/conda-forge/ipydrawio-widgets
 [workflow-badge]:
   https://github.com/deathbeds/ipydrawio/workflows/.github/workflows/ci.yml/badge.svg
 [workflow]:
-  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amaster+workflow%3A.github%2Fworkflows%2Fci.yml
+  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amain+workflow%3A.github%2Fworkflows%2Fci.yml
 [cov-badge]:
-  https://codecov.io/gh/deathbeds/ipydrawio/branch/master/graph/badge.svg?token=9B74VKHQDK
+  https://codecov.io/gh/deathbeds/ipydrawio/branch/main/graph/badge.svg?token=9B74VKHQDK
 [cov]: https://codecov.io/gh/deathbeds/ipydrawio
 [docs-badge]: https://readthedocs.org/projects/ipydrawio/badge/?version=latest
 [docs]: https://ipydrawio.rtfd.io
```

### Comparing `ipydrawio-widgets-1.2.2/setup.cfg` & `ipydrawio-widgets-1.3.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -6,35 +6,34 @@
 url = https://ipydrawio.rtfd.io
 author = ipydrawio Contributors
 author_email = ripxl@example.com
 license = Apache-2.0
 license_files = LICENSE.txt
 project_urls = 
 	Bug Tracker = https://github.com/deathbeds/ipydrawio/issues
-	Changelog = https://github.com/deathbeds/ipydrawio/blob/master/CHANGELOG.md
+	Changelog = https://github.com/deathbeds/ipydrawio/blob/main/CHANGELOG.md
 	Coverage = https://app.codecov.io/gh/deathbeds/ipydrawio
 	Documentation = https://ipydrawio.rtfd.io
 	Source Code = https://github.com/deathbeds/ipydrawio
 classifiers = 
 	Development Status :: 4 - Beta
 	Framework :: IPython
 	Framework :: Jupyter
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 package_dir = 
 	= src
 packages = find:
 include_package_data = True
 zip_safe = False
 install_requires = 
 	ipywidgets >=7.6,<9
@@ -46,29 +45,21 @@
 	pytest
 	pytest-console-scripts
 
 [options.packages.find]
 where = 
 	src
 
-[flake8]
-exclude = .git,__pycache__,envs,.ipynb_checkpoints,.mypy_cache
-max-line-length = 88
-ignore = E203
-
-[isort]
-combine_as_imports = True
-include_trailing_comma = True
-line_length = 88
-multi_line_output = 3
-
 [coverage:run]
 branch = True
 source_pkgs = 
 	ipydrawio_widgets
 concurrency = multiprocessing
 parallel = True
 
+[coverage:html]
+show_contexts = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ipydrawio-widgets-1.2.2/setup.py` & `ipydrawio-widgets-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""dynamic setup information for setuptools, also see package.json and setup.cfg"""
+"""dynamic setup information for setuptools, also see package.json and setup.cfg."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/__init__.py` & `ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-""""main importable for ipydrawio-widgets"""
+""""main importable for ipydrawio-widgets."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/_version.py` & `ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/_version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""source of truth for ipydrawio-widgets version"""
+"""source of truth for ipydrawio-widgets version."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 # Copyright 2020 jupyterlab-drawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/constants.py` & `ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/js/package.json` & `ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/js/package.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8541666666666666%*

 * *Differences: {"'dependencies'": "{'@deathbeds/ipydrawio-webpack': '^21.1.600'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^3.6.1'}",*

 * * "'scripts_doit'": "OrderedDict([('build:pre', OrderedDict([('file_dep', ['scripts/schema.py', "*

 * *                   "'schema/*.json']), ('targets', ['src/_schema.d.ts'])]))])",*

 * * "'version'": "'1.3.0'",*

 * * 'delete': "['peerDependencies']"}*

```diff
@@ -1,24 +1,24 @@
 {
     "author": "IPyDrawio Contributors",
     "bugs": {
         "url": "https://github.com/deathbeds/ipydrawio/issues"
     },
     "dependencies": {
-        "@deathbeds/ipydrawio-webpack": "^20.5.300",
+        "@deathbeds/ipydrawio-webpack": "^21.1.600",
         "@jupyterlab/application": "^3.1.0",
         "@jupyterlab/launcher": "^3.1.0",
         "@jupyterlab/mainmenu": "^3.1.0"
     },
     "description": "A JupyterLab extension for embedding interactive drawio / mxgraph diagrams.",
     "devDependencies": {
         "@jupyter-widgets/base": "^4.0.0 || ^6.0.0",
         "@jupyter-widgets/controls": "^3.0.0 || ^5.0.0",
         "@jupyter-widgets/jupyterlab-manager": "^3.0.0 || ^5.0.0",
-        "@jupyterlab/builder": "^3.4.0"
+        "@jupyterlab/builder": "^3.6.1"
     },
     "files": [
         "{lib,schema,style,src}/**/*.{ts,tsx,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,css}"
     ],
     "homepage": "https://ipydrawio.rtfd.io",
     "jupyterlab": {
         "discovery": {
@@ -55,22 +55,28 @@
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "Apache-2.0",
     "main": "lib/index.js",
     "name": "@deathbeds/ipydrawio",
-    "peerDependencies": {
-        "@jupyter-widgets/base": "^4.0.0 || ^6.0.0",
-        "@jupyter-widgets/controls": "^3.0.0 || ^5.0.0",
-        "@jupyter-widgets/jupyterlab-manager": "^3.0.0 || ^5.0.0"
-    },
     "repository": {
         "type": "git",
         "url": "https://github.com/deathbeds/ipydrawio.git"
     },
     "scripts": {
         "build:pre": "python scripts/schema.py"
     },
+    "scripts_doit": {
+        "build:pre": {
+            "file_dep": [
+                "scripts/schema.py",
+                "schema/*.json"
+            ],
+            "targets": [
+                "src/_schema.d.ts"
+            ]
+        }
+    },
     "types": "lib/index.d.ts",
-    "version": "1.2.2"
+    "version": "1.3.0"
 }
```

### Comparing `ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/js/plugin.json` & `ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/js/plugin.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964062759227794%*

 * *Differences: {"'definitions'": "{'drawio-url-params': {'properties': {'clibs': {'description': "*

 * *                  "'key1;key2;key;...;keyN: Specifies custom libraries (keys are file IDs or URLs "*

 * *                  "with a U-prefix)'}, 'configure': {'description': '1: Sends the `configure` "*

 * *                  'event and waits for the `configure` action. See more about the embed mode. '*

 * *                  "**NEW `14.6.10`**'}, 'create': {'description': 'url/name: Creates a new file "*

 * *                  'from a template URL […]*

```diff
@@ -283,35 +283,35 @@
                 },
                 "chrome": {
                     "$ref": "#/definitions/off-switch",
                     "description": "0: Uses the chromeless read-only viewer."
                 },
                 "clibs": {
                     "$ref": "#/definitions/library-keys-string",
-                    "description": "key1;key2;key;...;keyN: Specifies custom libraries (keys are file IDs or _URLs with a U-prefix_)"
+                    "description": "key1;key2;key;...;keyN: Specifies custom libraries (keys are file IDs or URLs with a U-prefix)"
                 },
                 "client": {
                     "$ref": "#/definitions/on-switch",
                     "description": "1: Runs diagrams.net in client mode. This displays a normal UI and sends a `ready` message to the opener or parent when the page is loaded. After receiving a message containing XML or compressed XML, a local file is created. The file is then set to `modified` so the connection to the window can be closed after sending the initial XML. Whether the XML is loaded again after a page refresh, depends on the caller implementation. Use `proto=json` to use a custom protocol for special cases."
                 },
                 "close": {
                     "$ref": "#/definitions/on-switch",
                     "description": "1: Shows the *Close* button in chromeless mode which closes the window when selected."
                 },
                 "configure": {
                     "$ref": "#/definitions/off-switch",
-                    "description": "1: Sends the `configure` event and waits for the `configure` action. See more about the _embed mode_. **NEW `14.6.10`**"
+                    "description": "1: Sends the `configure` event and waits for the `configure` action. See more about the embed mode. **NEW `14.6.10`**"
                 },
                 "cors": {
                     "description": "regex: Checks whether URLS have CORS enabled using a URL encoded regular expression, e.g.cors=%5Ehttps%3F%3A%5C%2F%5C%2F.*%5C.github%5C.io%5C%2F **TBD `14.6.10`**",
                     "format": "regex",
                     "type": "string"
                 },
                 "create": {
-                    "description": "url/name: Creates a new file from a template URL. If the value is not a URL and is not empty, the script will try to use `window.opener_url]`. In [embed mode_, `window.opener[name]` will be used to get the initial XML. Note that this requires the same origin policy in the opener/parent for reading the variable.",
+                    "description": "url/name: Creates a new file from a template URL. If the value is not a URL and is not empty, the script will try to use `window.opener_url`. In embed mode, `window.opener[name]` will be used to get the initial XML. Note that this requires the same origin policy in the opener/parent for reading the variable.",
                     "type": "string"
                 },
                 "dark": {
                     "$ref": "#/definitions/on-off-switch",
                     "description": "[0|1]: Disables/enables dark mode in Sketch and Minimal editor themes."
                 },
                 "data": {
@@ -323,34 +323,34 @@
                     "description": "0: Disables the Dropbox integration."
                 },
                 "demo": {
                     "$ref": "#/definitions/on-switch",
                     "description": "1: Shortcut for `db=0&gapi=0&math=0&picker=0`, disables the splash screen and creates an empty, local diagram file."
                 },
                 "desc": {
-                    "description": "{compressed-json}: Passes the CSV import descriptor (_example](https://web.archive.org/web/20210425055302/https://www.draw.io/?desc=SnVTtjpswEHwafl50gUP5nZC7F7i+gIMdvI3xIrMkSp++u7bh0tKoVSUE9sx6PPuRFLtDUZZTcPwuqj2/LdEwxuUHP9+7oAa76YDsdNoAMqSDugG+aFDM9aMgX0sMXWtVoE07XkWybPh9xtArWm54pLQitRBFWTl1Mi7uXouy9qo3/Cmq5hSK6p2/wMRId2eK6ljUotCiQyb37OBeVIcESnBZDzgCAfokwe4gicxifPOrDea8aPUKHGG8vjaykZOz4HsEoo6S83XDwlU2I4az9wP0qov+yjot5frDzQKZz0G1Qt24qoxZ6vnAccvLgJPXRufdGZxrUmIiI9ukMlLAi3mgEpDIbAm08QR0T65eMiq1HNP1AnMToB8w0My36L1pKdd+lwt5DtjPFYhErpPnvEImpJGZ4OKtgmMTV5HgrybQYzSFyTxGpHI+uXv8XTE+kkecnCdPPJM6ttJtp3Bd6m+83oeAN96eHLaXbxZ8gj+kFblJ6OkTfkg/t9uv0dsd/6OiPIWrlP5cTtDruH9J6W9unTnTclgAwuGX/Q002YSoKToT1BroLK3gQWkNvssjuC3n0ew8hjyBnEjZ5B9Ikya8ydOcHYG/pFD5f8pTjDpO8aL9NtszunvCOHXH6dFiTPsn)). Works with the [www.draw.io_ domain only. **NEW `14.6.10`**"
+                    "description": "{compressed-json}: Passes the CSV import descriptor example. Works with the www.draw.io domain only. **NEW `14.6.10`**"
                 },
                 "drafts": {
                     "$ref": "#/definitions/off-switch",
                     "description": "0: Disables draft states (does not save unsaved files in *IndexedDB*)."
                 },
                 "drive": {
                     "$ref": "#/definitions/off-switch",
-                    "description": "0: Simulates _app.diagrams.net_ regardless of the domain name (uses the old app ID)."
+                    "description": "0: Simulates app.diagrams.net regardless of the domain name (uses the old app ID)."
                 },
                 "edge": {
                     "description": "move: Disables the handling of connector segments without having previously selected the connector.",
                     "type": "string"
                 },
                 "edit": {
                     "$ref": "#/definitions/url-param-url-or-blank",
                     "description": "`edit=url`: Adds a link for the *Edit* button in chromeless mode (use `edit=_blank` to edit the diagram as a new copy)."
                 },
                 "embed": {
-                    "description": "`embed=1:` Runs diagrams.net in _embed mode](/web/20210425055302/https://www.diagrams.net/doc/faq/embed-mode.html). Use this mode with [embed.diagrams.net_ only. **NEW `14.6.10`**"
+                    "description": "`embed=1:` Runs diagrams.net in embed mode. Use this mode with embed.diagrams.net only. **NEW `14.6.10`**"
                 },
                 "format": {
                     "$ref": "#/definitions/off-switch",
                     "description": "0: Disables the format panel on the right."
                 },
                 "gapi": {
                     "$ref": "#/definitions/off-switch",
@@ -362,15 +362,15 @@
                 },
                 "gitlab": {
                     "description": "url: Sets the URL-encoded path to a custom GitLab installation to use for GitLab file operations.",
                     "format": "uri",
                     "type": "string"
                 },
                 "gitlab-id": {
-                    "description": "ID: Specifies the _client ID of the custom GitLab application_ when using a custom GitLab instance.",
+                    "description": "ID: Specifies the client ID of the custom GitLab application when using a custom GitLab instance.",
                     "type": "string"
                 },
                 "gl": {
                     "$ref": "#/definitions/off-switch",
                     "description": "0: Disables the GitLab integration."
                 },
                 "grid": {
@@ -436,15 +436,15 @@
                 },
                 "libraries": {
                     "$ref": "#/definitions/on-switch",
                     "description": "1: Specifies whether libraries should be enabled in embed mode. The default is disabled (0). **TBD `14.6.10`**"
                 },
                 "libs": {
                     "$ref": "#/definitions/library-keys-string",
-                    "description": "key1;key2;...;keyN: Specifies the current libraries. Possible keys are allied\\_telesis, android, archimate, archimate3, arrows2, atlassian, aws3, aws3d, aws4, azure, basic, bootstrap, bpmn, cabinets, cisco, cisco\\_safe, citrix, clipart, dfd, eip, electrical, er, floorplan, flowchart, gcp2, general, gmdl, ibm, images, infographic, ios, lean\\_mapping, mockups, mscae, network, office, pid, rack, signs, sitemap, sysml, uml, veeam and webicons."
+                    "description": "key1;key2;...;keyN: Specifies the current libraries. Possible keys are allied_telesis, android, archimate, archimate3, arrows2, atlassian, aws3, aws3d, aws4, azure, basic, bootstrap, bpmn, cabinets, cisco, cisco\\_safe, citrix, clipart, dfd, eip, electrical, er, floorplan, flowchart, gcp2, general, gmdl, ibm, images, infographic, ios, lean\\_mapping, mockups, mscae, network, office, pid, rack, signs, sitemap, sysml, uml, veeam and webicons."
                 },
                 "lightbox": {
                     "$ref": "#/definitions/on-switch",
                     "description": "1: Uses the lightbox in chromeless mode (larger zoom, no page visible, chromeless)."
                 },
                 "local": {
                     "$ref": "#/definitions/on-switch",
@@ -493,24 +493,24 @@
                     "description": "0: Disables the OneDrive integration."
                 },
                 "offline": {
                     "$ref": "#/definitions/on-off-switch",
                     "description": "[1|0]: Registers or unregisters the progressive web app (all remote storage locations are disabled)."
                 },
                 "open": {
-                    "description": "prefix+ID: If _location hash properties_ are not available, use this as a replacement. The browser will add the hash property to the URL immediately and not remove the URL parameter. Existing hash property takes precedence.",
+                    "description": "prefix+ID: If location hash properties are not available, use this as a replacement. The browser will add the hash property to the URL immediately and not remove the URL parameter. Existing hash property takes precedence.",
                     "type": "string"
                 },
                 "override-mime": {
                     "$ref": "#/definitions/on-switch",
                     "description": "1: Saves all Google Drive files as `application/vnd.jgraph.mxfile`."
                 },
                 "p": {
                     "$ref": "#/definitions/library-keys-string",
-                    "description": "id1;id2;...;idN: Selects which plugins to load. _See the list of available plugins_."
+                    "description": "id1;id2;...;idN: Selects which plugins to load. See the list of available plugins."
                 },
                 "page": {
                     "description": "index: Starts with the given page (the default is the first page, where the index for the first page is `0`)",
                     "type": "number"
                 },
                 "page-id": {
                     "description": "ID: Starts with the given page ID (has precedence over the `page` URL parameter). To find the ID of the current page, right click on the canvas and select *Edit Data*. The ID is the first entry in this dialog.",
@@ -518,15 +518,15 @@
                 },
                 "picker": {
                     "$ref": "#/definitions/on-off-switch",
                     "description": "0/1: Disables/enables the Google file picker in dialogs."
                 },
                 "plugins": {
                     "$ref": "#/definitions/off-switch",
-                    "description": "0: Does not load _plugins_."
+                    "description": "0: Does not load plugins."
                 },
                 "proto": {
                     "description": "`client=1`: Runs diagrams.net in client mode. This displays a normal UI and sends a `ready` message to the opener or parent when the page is loaded. After receiving a message containing XML or compressed XML, a local file is created. The file is then set to `modified` so the connection to the window can be closed after sending the initial XML. Whether the XML is loaded again after a page refresh, depends on the caller implementation. Use `proto=json` to use a custom protocol for special cases. **NEW `14.6.10`**"
                 },
                 "pv": {
                     "$ref": "#/definitions/off-switch",
                     "description": "0: Sets the default `pageVisible` to `false`."
@@ -577,15 +577,15 @@
                 },
                 "splash": {
                     "$ref": "#/definitions/off-switch",
                     "description": "0: Does not show the splash screen."
                 },
                 "stealth": {
                     "$ref": "#/definitions/on-switch",
-                    "description": "1: Disables all features that require external web services (such as _PDF export_)."
+                    "description": "1: Disables all features that require external web services (such as PDF export)."
                 },
                 "storage": {
                     "$ref": "#/definitions/url-param-storage",
                     "description": "device: Adds a device storage option for touch devices."
                 },
                 "svg-warning": {
                     "$ref": "#/definitions/off-switch",
@@ -596,15 +596,15 @@
                     "description": "[none|manual|auto]: Enables/disables collaborative editing (default is `auto`)."
                 },
                 "target": {
                     "$ref": "#/definitions/url-param-target",
                     "description": "[auto|self|frame|blank]: Opens links in the same window or frame or in a blank window in chromeless mode (`auto` is the default which opens relative links and anchors in the same window in chromeless mode, and all links in a new window in editing mode)."
                 },
                 "template-filename": {
-                    "description": "name: If the \\#U hash property is used but the URL does not contain a filename to determine binary mode. See the list of _supported location hash properties_.",
+                    "description": "name: If the \\#U hash property is used but the URL does not contain a filename to determine binary mode. See the list of supported location hash properties.",
                     "type": "string"
                 },
                 "thumb": {
                     "$ref": "#/definitions/off-switch",
                     "description": "0: Disables the creation of thumbnails in Drive."
                 },
                 "title": {
@@ -629,15 +629,15 @@
                         "sketch"
                     ]
                 },
                 "url": {
                     "description": "url: *Deprecated* - Use U hash property `#U{uri_encoded_url}` to open a diagram from a URI-encoded URL, eg. https://app.diagrams.net/\\#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fmaster%2Fdiagrams%2Fschema.xml **NEW `14.6.10`**"
                 },
                 "vars": {
-                    "description": "`vars=json`: Uses a URI-encoded JSON string for global _placeholders for use in labels and tooltips_ where enabled, e.g. `vars={\"key\":\"value\"}`.",
+                    "description": "`vars=json`: Uses a URI-encoded JSON string for global placeholders for use in labels and tooltips where enabled, e.g. `vars={\"key\":\"value\"}`.",
                     "type": "string"
                 },
                 "viewbox": {
                     "description": "{\"x\": int, \"y\": int, \"width\": int, \"height\": int}: Sets the initial viewport when you specify file IDs. **NEW `14.6.10`**"
                 },
                 "zoom": {
                     "description": "nocss: Disables the CSS zoom preview.",
@@ -767,27 +767,51 @@
                 "title": {
                     "$ref": "#/definitions/library-resource"
                 }
             },
             "type": "object"
         },
         "off-switch": {
-            "maximum": 0,
-            "minimum": 0,
-            "type": "number"
+            "anyOf": [
+                {
+                    "const": "",
+                    "title": "on"
+                },
+                {
+                    "const": "0",
+                    "title": "off"
+                }
+            ],
+            "type": "string"
         },
         "on-off-switch": {
-            "maximum": 1,
-            "minimum": 0,
-            "type": "number"
+            "anyOf": [
+                {
+                    "const": "0",
+                    "title": "off"
+                },
+                {
+                    "const": "",
+                    "title": "on"
+                }
+            ],
+            "type": "string"
         },
         "on-switch": {
-            "maximum": 1,
-            "minimum": 1,
-            "type": "number"
+            "anyOf": [
+                {
+                    "const": "1",
+                    "title": "on"
+                },
+                {
+                    "const": "",
+                    "title": "off"
+                }
+            ],
+            "type": "string"
         },
         "plugin-url-list": {
             "items": {
                 "format": "uri",
                 "type": "string"
             },
             "type": "array"
@@ -892,26 +916,26 @@
         "drawioExportUrl": {
             "$ref": "#/definitions/drawio-export-url",
             "description": "URL parameters for the export URL. "
         },
         "drawioUrlParams": {
             "$ref": "#/definitions/drawio-url-params",
             "default": {
-                "db": 0,
-                "drafts": 0,
-                "gapi": 0,
-                "gh": 0,
-                "gl": 0,
-                "od": 0,
+                "db": "0",
+                "drafts": "0",
+                "gapi": "0",
+                "gh": "0",
+                "gl": "0",
+                "od": "0",
                 "p": "ex;tips;svgdata;sql;anim;trees;replay;anon;flow;webcola;tags",
-                "picker": 0,
-                "stealth": 1,
-                "svg-warning": 0,
-                "thumb": 0,
-                "tr": 0,
+                "picker": "0",
+                "stealth": "1",
+                "svg-warning": "0",
+                "thumb": "0",
+                "tr": "0",
                 "ui": "min"
             },
             "description": "URL parameters for the drawio iframe https://web.archive.org/web/20210425055302/https://www.diagrams.net/doc/faq/supported-url-parameters"
         }
     },
     "title": "Diagram Documents",
     "type": "object"
```

### Comparing `ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/schema.py` & `ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""schema for ipydrawio-widgets"""
+"""schema for ipydrawio-widgets."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ipydrawio-widgets-1.2.2/src/ipydrawio_widgets/widget_diagram.py` & `ipydrawio-widgets-1.3.0/src/ipydrawio_widgets/widget_diagram.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-""" jupyter widgets for drawio"""
+"""Jupyter widgets for drawio."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 # Copyright 2020 jupyterlab-drawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -23,59 +23,64 @@
 from .schema import get_schema
 
 module_name = __js__["name"]
 module_version = "^{version}".format(**__js__)
 
 
 class DiagramBase(W.Widget):
-    """Module metadata for SVG"""
+
+    """Module metadata for SVG."""
 
     _model_module = T.Unicode(module_name).tag(sync=True)
     _model_module_version = T.Unicode(module_version).tag(sync=True)
     _view_module = T.Unicode(module_name).tag(sync=True)
     _view_module_version = T.Unicode(module_version).tag(sync=True)
 
 
 @W.register
 class XML(DiagramBase, W.Widget):
-    """A Drawio XML-native Document"""
+
+    """A Drawio XML-native Document."""
 
     value = T.Unicode(A_SHORT_DRAWIO).tag(sync=True)
     _model_name = T.Unicode("XMLModel").tag(sync=True)
     _view_name = T.Unicode("XMLView").tag(sync=True)
 
 
 @W.register
 class Diagram(DiagramBase, W.Box):
-    """A Drawio Diagram"""
+
+    """A Drawio Diagram."""
 
     _model_name = T.Unicode("DiagramModel").tag(sync=True)
     _view_name = T.Unicode("DiagramView").tag(sync=True)
 
     source = T.Instance(XML, help="a drawio xml document").tag(
-        sync=True, **W.widget_serialization
+        sync=True,
+        **W.widget_serialization,
     )
 
     scroll_x = T.Float(help="the current viewport scroll x position").tag(sync=True)
     scroll_y = T.Float(help="the current viewport scroll y position").tag(sync=True)
     zoom = T.Float(help="the current zoom level").tag(sync=True)
     page_ids = W.trait_types.TypedTuple(T.Unicode(), help="known page ids").tag(
-        sync=True
+        sync=True,
     )
     current_page = T.Int(0, min=0, help="the current, 0-based, page index").tag(
-        sync=True
+        sync=True,
     )
     page_format = T.Dict(
         help=(
             "the physical size of the diagram media in milli-inches (or something): "
             "x, y, width, height"
-        )
+        ),
     ).tag(sync=True)
     grid_enabled = T.Bool(
-        True, help="show on-screen grid behind shapes (above background)"
+        True,
+        help="show on-screen grid behind shapes (above background)",
     ).tag(sync=True)
     grid_color = T.Unicode("#66666666").tag(sync=True)
     grid_size = T.Float(10, min=0.01).tag(sync=True)
     selected_cells = W.trait_types.TypedTuple(T.Unicode()).tag(sync=True)
     cell_ids = W.trait_types.TypedTuple(T.Unicode()).tag(sync=True)
     # these are important, but advanced
     url_params = T.Dict(help="drawio URL params").tag(sync=True)
```

### Comparing `ipydrawio-widgets-1.2.2/src/ipydrawio_widgets.egg-info/PKG-INFO` & `ipydrawio-widgets-1.3.0/src/ipydrawio_widgets.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: ipydrawio-widgets
-Version: 1.2.2
+Version: 1.3.0
 Summary: Draw.io Diagrams as Jupyter Widgets (Kernel-only)
 Home-page: https://ipydrawio.rtfd.io
 Author: ipydrawio Contributors
 Author-email: ripxl@example.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/deathbeds/ipydrawio/issues
-Project-URL: Changelog, https://github.com/deathbeds/ipydrawio/blob/master/CHANGELOG.md
+Project-URL: Changelog, https://github.com/deathbeds/ipydrawio/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://app.codecov.io/gh/deathbeds/ipydrawio
 Project-URL: Documentation, https://ipydrawio.rtfd.io
 Project-URL: Source Code, https://github.com/deathbeds/ipydrawio
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # IPyDrawio Widgets
 
 [![docs][docs-badge]][docs] [![binder-badge][]][binder]
@@ -79,15 +78,15 @@
 For more, see the documentation
 
 ## Open Source
 
 This work is licensed under the [Apache-2.0] License.
 
 ```
-Copyright 2022 ipydrawio contributors
+Copyright 2023 ipydrawio contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
   http://www.apache.org/licenses/LICENSE-2.0
 
@@ -95,27 +94,27 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 
 [apache-2.0]:
-  https://github.com/deathbeds/ipydrawio/blob/master/py_packages/ipydrawio-widgets/LICENSE.txt
+  https://github.com/deathbeds/ipydrawio/blob/main/py_packages/ipydrawio-widgets/LICENSE.txt
 [binder]:
-  http://mybinder.org/v2/gh/deathbeds/ipydrawio/master?urlpath=lab/tree/docs/Poster.dio.svg
+  http://mybinder.org/v2/gh/deathbeds/ipydrawio/main?urlpath=lab/tree/docs/Poster.dio.svg
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [cov-badge]:
-  https://codecov.io/gh/deathbeds/ipydrawio/branch/master/graph/badge.svg?token=9B74VKHQDK
+  https://codecov.io/gh/deathbeds/ipydrawio/branch/main/graph/badge.svg?token=9B74VKHQDK
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [pypi-badge]: https://img.shields.io/pypi/v/ipydrawio-widgets
 [pypi]: https://pypi.org/project/ipydrawio-widgets
 [conda-badge]: https://img.shields.io/conda/vn/conda-forge/ipydrawio-widgets
 [conda]: https://anaconda.org/conda-forge/ipydrawio-widgets
 [workflow-badge]:
   https://github.com/deathbeds/ipydrawio/workflows/.github/workflows/ci.yml/badge.svg
 [workflow]:
-  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amaster+workflow%3A.github%2Fworkflows%2Fci.yml
+  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amain+workflow%3A.github%2Fworkflows%2Fci.yml
 [cov-badge]:
-  https://codecov.io/gh/deathbeds/ipydrawio/branch/master/graph/badge.svg?token=9B74VKHQDK
+  https://codecov.io/gh/deathbeds/ipydrawio/branch/main/graph/badge.svg?token=9B74VKHQDK
 [cov]: https://codecov.io/gh/deathbeds/ipydrawio
 [docs-badge]: https://readthedocs.org/projects/ipydrawio/badge/?version=latest
 [docs]: https://ipydrawio.rtfd.io
```

### Comparing `ipydrawio-widgets-1.2.2/src/ipydrawio_widgets.egg-info/SOURCES.txt` & `ipydrawio-widgets-1.3.0/src/ipydrawio_widgets.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+./README.md
 src/ipydrawio_widgets/__init__.py
 src/ipydrawio_widgets/_version.py
 src/ipydrawio_widgets/constants.py
 src/ipydrawio_widgets/schema.py
 src/ipydrawio_widgets/widget_diagram.py
 src/ipydrawio_widgets.egg-info/PKG-INFO
 src/ipydrawio_widgets.egg-info/SOURCES.txt
```

### Comparing `ipydrawio-widgets-1.2.2/tests/__init__.py` & `ipydrawio-widgets-1.3.0/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """tests for ipydrawio-widgets"""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ipydrawio-widgets-1.2.2/tests/test_schema.py` & `ipydrawio-widgets-1.3.0/tests/test_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """minimal tests of schema"""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ipydrawio-widgets-1.2.2/tests/test_widgets.py` & `ipydrawio-widgets-1.3.0/tests/test_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """minimal widget import/invocation test"""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

