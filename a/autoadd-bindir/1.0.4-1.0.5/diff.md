# Comparing `tmp/autoadd_bindir-1.0.4.tar.gz` & `tmp/autoadd_bindir-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoadd_bindir-1.0.4.tar", max compression
+gzip compressed data, was "autoadd_bindir-1.0.5.tar", max compression
```

## Comparing `autoadd_bindir-1.0.4.tar` & `autoadd_bindir-1.0.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3137 2023-03-29 11:51:20.000233 autoadd_bindir-1.0.4/docs/readme.md
--rw-r--r--   0        0        0     7245 2023-03-29 11:53:39.297262 autoadd_bindir-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1705 2023-03-29 11:51:20.000233 autoadd_bindir-1.0.4/src/autoadd_bindir/__init__.py
--rw-r--r--   0        0        0     4889 1970-01-01 00:00:00.000000 autoadd_bindir-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3340 2023-03-30 07:51:28.321733 autoadd_bindir-1.0.5/docs/readme.md
+-rw-r--r--   0        0        0     7299 2023-04-12 15:30:50.381455 autoadd_bindir-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      777 2023-04-12 15:30:50.381455 autoadd_bindir-1.0.5/src/autoadd_bindir/__init__.py
+-rw-r--r--   0        0        0     5092 1970-01-01 00:00:00.000000 autoadd_bindir-1.0.5/PKG-INFO
```

### Comparing `autoadd_bindir-1.0.4/docs/readme.md` & `autoadd_bindir-1.0.5/docs/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [![Testing](https://img.shields.io/github/actions/workflow/status/libranet/autoadd-bindir/testing.yaml?branch=main&longCache=true&style=flat-square&label=tests&logo=GitHub%20Actions&logoColor=fff")](https://github.com/libranet/autoadd-bindir/actions/workflows/testing.yaml)
 [![Linting](https://img.shields.io/github/actions/workflow/status/libranet/autoadd-bindir/linting.yaml?branch=main&longCache=true&style=flat-square&label=linting&logo=GitHub%20Actions&logoColor=fff")](https://github.com/libranet/autoadd-bindir/actions/workflows/linting.yaml)
 [![Read the Docs](https://readthedocs.org/projects/autoadd-bindir/badge/?version=latest)](https://autoadd-bindir.readthedocs.io/en/latest/)
+[![Codecov](https://codecov.io/gh/libranet/autoadd-bindir/branch/main/graph/badge.svg?token=AFP6UMXEN5)](https://codecov.io/gh/libranet/autoadd-bindir)
 [![PyPi Package](https://img.shields.io/pypi/v/autoadd-bindir?color=%2334D058&label=pypi%20package)](https://pypi.org/project/autoadd-bindir/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/libranet/autoadd-bindir/blob/main/docs/license.md)
 
 
+
+https://app.codecov.io/gh/libranet/autoadd-bindir
 # Autoadd-bindir
 
 Automatically add the bin-directory of your virtualenv to the ``PATH``-environment variable
 via ``sitecustomize``-entrypoint. You now no  longer need to manually *activate* your
 virtual environment for the sole purpose of adding thie bin-drectory to your ``$PATH``.
 
 ## How does it work?
```

### Comparing `autoadd_bindir-1.0.4/pyproject.toml` & `autoadd_bindir-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 # [tool.nox.session]
 # python = ["3.10n", "3.11n"]
 
 
 [tool.poetry]
 name = "autoadd_bindir"
-version = "1.0.4" # version managed by poetry-version-plugin
+version = "1.0.5" # version managed by poetry-version-plugin
 license = "MIT"
 description = "Automatically add bin-dir to PATH for every process in your virtualenv."
 readme = "docs/readme.md"
 authors = ["Wouter Vanden Hove <wouter@libranet.eu>"]
 maintainers = ["Wouter Vanden Hove <wouter@libranet.eu>"]
 homepage = "https://github.com/libranet/autoadd_bindir"
 repository = "https://github.com/libranet/autoadd_bindir"
@@ -110,27 +110,28 @@
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 packages = [{ include = "autoadd_bindir", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4.0"
-sitecustomize-entrypoints = ">=0.1.0"
+sitecustomize-entrypoints = ">=1.1.0"
 
 [tool.poetry.group.dev.dependencies]
 bandit = { extras = ["toml"], version = ">=1.7.4" }
 black = { version = ">=22.1.0", allow-prereleases = true }
 flake8 = ">=4.0.1"
 flake8-bugbear = ">=23.2.13"
 flake8-docstrings = ">=1.6.0"
 flake8-pyproject = ">=1.2.2"
 flake8-rst-docstrings = ">=0.2.5"
 isort = ">=5.10.1"
 pre-commit = ">=2.14.1"
 pre-commit-hooks = ">=4.1.0"
+pydocstyle = ">=6.3.0"
 pylint = ">=2.12.2"
 ruff = ">=0.0.254"
 
 [tool.poetry.group.dist.dependencies]
 pyroma = ">=4.2"
 twine = ">=4.0.2"
 
@@ -151,14 +152,15 @@
 tuna = ">=0.5.11"
 
 [tool.poetry.group.testing.dependencies]
 coverage = { extras = ["toml"], version = ">=6.2" }
 nox = ">=2022.11.21"
 nox-poetry = ">=1.0.2"
 pytest = ">=7.0.1"
+pytest-codecov = ">=0.5.1"
 pytest-cov = ">=3.0.0"
 tox = ">=4.4.7"
 
 [tool.poetry.group.typing.dependencies]
 lxml = { version = ">=4.9.2", optional = true, allow-prereleases = false } # mypy coverage-report
 mypy = ">=0.931"
 
@@ -203,16 +205,16 @@
 tag-name = "{version}"
 release-replacements = [
     { file = "docs/changes.md", pattern = "Unreleased \\(YYYY-MM-DD\\)", replace = "{version} ({date})" },
     { file = "src/autoadd_bindir/__init__.py", pattern = '__version__ = "{version}"', replace = '__version__ = "{next_version}"' },
 ]
 
 
-[tool.poetry-version-plugin]
-source = "init"
+# [tool.poetry-version-plugin]
+# source = "init"
 
 [tool.pylint.format]
 max-line-length = 120
 good-names = [
     "i",  # counter in loop
     "ok", # status
     "ts", # timestamp or timeseries object
```

### Comparing `autoadd_bindir-1.0.4/PKG-INFO` & `autoadd_bindir-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoadd-bindir
-Version: 1.0.4
+Version: 1.0.5
 Summary: Automatically add bin-dir to PATH for every process in your virtualenv.
 Home-page: https://github.com/libranet/autoadd_bindir
 License: MIT
 Keywords: entrypoints,sitecustomize
 Author: Wouter Vanden Hove
 Author-email: wouter@libranet.eu
 Maintainer: Wouter Vanden Hove
@@ -26,28 +26,31 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Dist: sitecustomize-entrypoints (>=0.1.0)
+Requires-Dist: sitecustomize-entrypoints (>=1.1.0)
 Project-URL: Changelog, https://github.com/libranet/autoadd_bindir/releases
 Project-URL: Documentation, https://autoadd-bindir.readthedocs.io
 Project-URL: Issues, https://github.com/libranet/autoadd_bindir/issues
 Project-URL: Repository, https://github.com/libranet/autoadd_bindir
 Description-Content-Type: text/markdown
 
 [![Testing](https://img.shields.io/github/actions/workflow/status/libranet/autoadd-bindir/testing.yaml?branch=main&longCache=true&style=flat-square&label=tests&logo=GitHub%20Actions&logoColor=fff")](https://github.com/libranet/autoadd-bindir/actions/workflows/testing.yaml)
 [![Linting](https://img.shields.io/github/actions/workflow/status/libranet/autoadd-bindir/linting.yaml?branch=main&longCache=true&style=flat-square&label=linting&logo=GitHub%20Actions&logoColor=fff")](https://github.com/libranet/autoadd-bindir/actions/workflows/linting.yaml)
 [![Read the Docs](https://readthedocs.org/projects/autoadd-bindir/badge/?version=latest)](https://autoadd-bindir.readthedocs.io/en/latest/)
+[![Codecov](https://codecov.io/gh/libranet/autoadd-bindir/branch/main/graph/badge.svg?token=AFP6UMXEN5)](https://codecov.io/gh/libranet/autoadd-bindir)
 [![PyPi Package](https://img.shields.io/pypi/v/autoadd-bindir?color=%2334D058&label=pypi%20package)](https://pypi.org/project/autoadd-bindir/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/libranet/autoadd-bindir/blob/main/docs/license.md)
 
 
+
+https://app.codecov.io/gh/libranet/autoadd-bindir
 # Autoadd-bindir
 
 Automatically add the bin-directory of your virtualenv to the ``PATH``-environment variable
 via ``sitecustomize``-entrypoint. You now no  longer need to manually *activate* your
 virtual environment for the sole purpose of adding thie bin-drectory to your ``$PATH``.
 
 ## How does it work?
```

