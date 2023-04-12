# Comparing `tmp/pyprojectx-1.0.0b1.tar.gz` & `tmp/pyprojectx-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprojectx-1.0.0b1.tar", max compression
+gzip compressed data, was "pyprojectx-1.0.0b2.tar", last modified: Wed Apr 12 07:07:00 2023, max compression
```

## Comparing `pyprojectx-1.0.0b1.tar` & `pyprojectx-1.0.0b2.tar`

### file list

```diff
@@ -1,23 +1,38 @@
--rw-r--r--   0        0        0     1071 2023-04-09 21:51:00.235975 pyprojectx-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     4600 2023-04-09 21:51:00.235975 pyprojectx-1.0.0b1/README.md
--rw-r--r--   0        0        0     3228 2023-04-09 21:51:19.068231 pyprojectx-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/__init__.py
--rw-r--r--   0        0        0     4218 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/cli.py
--rw-r--r--   0        0        0     6435 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/config.py
--rw-r--r--   0        0        0     5537 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/env.py
--rw-r--r--   0        0        0        0 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/__init__.py
--rw-r--r--   0        0        0      348 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/global-template.toml
--rw-r--r--   0        0        0     7226 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/initializers.py
--rw-r--r--   0        0        0      839 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/pdm-template.toml
--rw-r--r--   0        0        0      858 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/poetry-template.toml
--rw-r--r--   0        0        0       32 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/poetry.toml
--rw-r--r--   0        0        0      863 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/project-template.toml
--rw-r--r--   0        0        0      303 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/log.py
--rw-r--r--   0        0        0        0 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/__init__.py
--rw-r--r--   0        0        0       30 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/pw.bat
--rwxr-xr-x   0        0        0     5804 2023-04-09 21:51:19.168232 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/pw.py
--rwxr-xr-x   0        0        0      253 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/px
--rw-r--r--   0        0        0      373 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/px.bat
--rwxr-xr-x   0        0        0      275 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/pxg
--rw-r--r--   0        0        0      270 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/pxg.bat
--rw-r--r--   0        0        0     5583 1970-01-01 00:00:00.000000 pyprojectx-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-12 07:04:39.710029 pyprojectx-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0     4600 2023-04-12 07:04:39.710029 pyprojectx-1.0.0b2/README.md
+-rw-r--r--   0        0        0     3303 2023-04-12 07:07:00.570073 pyprojectx-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/__init__.py
+-rw-r--r--   0        0        0     4218 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/cli.py
+-rw-r--r--   0        0        0     6435 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/config.py
+-rw-r--r--   0        0        0     5537 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/env.py
+-rw-r--r--   0        0        0        0 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/initializer/__init__.py
+-rw-r--r--   0        0        0      348 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/initializer/global-template.toml
+-rw-r--r--   0        0        0     7226 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/initializer/initializers.py
+-rw-r--r--   0        0        0      839 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/initializer/pdm-template.toml
+-rw-r--r--   0        0        0      858 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/initializer/poetry-template.toml
+-rw-r--r--   0        0        0       32 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/initializer/poetry.toml
+-rw-r--r--   0        0        0      863 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/initializer/project-template.toml
+-rw-r--r--   0        0        0      303 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/log.py
+-rw-r--r--   0        0        0        0 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/wrapper/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/wrapper/pw.bat
+-rwxr-xr-x   0        0        0     5808 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/wrapper/pw.py
+-rwxr-xr-x   0        0        0      253 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/wrapper/px
+-rw-r--r--   0        0        0      373 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/wrapper/px.bat
+-rwxr-xr-x   0        0        0      275 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/wrapper/pxg
+-rw-r--r--   0        0        0      270 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/src/pyprojectx/wrapper/pxg.bat
+-rw-r--r--   0        0        0        0 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/__init__.py
+-rw-r--r--   0        0        0      907 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/conftest.py
+-rw-r--r--   0        0        0      188 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/data/alias-abbreviations.toml
+-rw-r--r--   0        0        0       21 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/data/invalid.toml
+-rw-r--r--   0        0        0      682 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/data/pw-test.toml
+-rw-r--r--   0        0        0       19 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/data/test-no-config.toml
+-rw-r--r--   0        0        0       94 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/data/test-no-tool-config.toml
+-rw-r--r--   0        0        0      644 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/data/test.toml
+-rw-r--r--   0        0        0        0 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/integration/__init__.py
+-rw-r--r--   0        0        0     5380 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/integration/test_pw.py
+-rw-r--r--   0        0        0     4046 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/integration/test_px.py
+-rw-r--r--   0        0        0        0 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/unit/__init__.py
+-rw-r--r--   0        0        0     6940 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/unit/test_cli.py
+-rw-r--r--   0        0        0     4034 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/unit/test_config.py
+-rw-r--r--   0        0        0     3139 2023-04-12 07:04:39.714029 pyprojectx-1.0.0b2/tests/unit/test_env.py
+-rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 pyprojectx-1.0.0b2/PKG-INFO
```

### Comparing `pyprojectx-1.0.0b1/LICENSE` & `pyprojectx-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b1/README.md` & `pyprojectx-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b1/pyproject.toml` & `pyprojectx-1.0.0b2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,110 +1,113 @@
-[tool.poetry]
+[project]
 name = "pyprojectx"
-version = "1.0.0b1"
+dynamic = []
 description = "Execute scripts from pyproject.toml, installing tools on-the-fly"
-license = "MIT"
-authors = ["Houbie <ivo@houbrechts-it.be>"]
+authors = [
+    { name = "Houbie", email = "ivo@houbrechts-it.be" },
+]
 readme = "README.md"
-homepage = "https://github.com/pyprojectx/pyprojectx"
-documentation = "https://pyprojectx.github.io"
-keywords = ["build", "dependency", "pyprojectx"]
+keywords = [
+    "build",
+    "dependency",
+    "pyprojectx",
+]
 classifiers = [
     "Topic :: Software Development :: Build Tools",
-    "Topic :: Software Development :: Libraries :: Python Modules"
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+requires-python = ">=3.7"
+dependencies = [
+    "tomli>=2.0.1",
+    "virtualenv>=20.21.0",
+    "userpath>=1.8.0",
 ]
+version = "1.0.0b2"
+
+[project.license]
+text = "MIT"
 
-[tool.poetry.scripts]
+[project.urls]
+homepage = "https://github.com/pyprojectx/pyprojectx"
+documentation = "https://pyprojectx.github.io"
+
+[project.scripts]
 pyprojectx = "pyprojectx.cli:main"
 
-[tool.poetry.dependencies]
-python = ">=3.7"
-tomli = ">=2.0"
-virtualenv = ">=20.21"
-userpath = ">=1.8"
-
-[tool.poetry.dev-dependencies]
-pytest = ">=7.3"
-pytest-mock = ">=3.10"
+[tool.pdm.version]
+source = "scm"
 
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.pdm.dev-dependencies]
+test = [
+    "pytest>=7.3.0",
+    "pytest-mock>=3.10.0",
+]
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.format]
 max-line-length = 120
-variable-rgx = '^[a-z_][a-z0-9_]*$'
+variable-rgx = "^[a-z_][a-z0-9_]*$"
+
 [tool.pylint.similarities]
-ignore-imports= true
+ignore-imports = true
+
 [tool.pylint.master]
-init-hook = """
-import sys
-sys.path.append(f".venv/lib/python{sys.version_info.major}.{sys.version_info.minor}/site-packages")
-sys.path.append(f".venv/Lib/site-packages")
-"""
+init-hook = "import sys\nsys.path.append(f\".venv/lib/python{sys.version_info.major}.{sys.version_info.minor}/site-packages\")\nsys.path.append(f\".venv/Lib/site-packages\")\n"
+
 [tool.pylint.messages_control]
 disable = [
     "missing-docstring",
-    "unspecified-encoding"
+    "unspecified-encoding",
 ]
 
 [tool.pyprojectx]
-poetry = { requirements = "poetry==1.4.2", post-install = "pw@pre-commit install" }
 black = "black==23.3.0"
 isort = "isort==5.12.0"
 pylint = "pylint==2.17.2"
 pre-commit = "pre-commit"
-mkdocs = ["mkdocs ~=1.2", "mkdocs-material ~=8.2", "mkdocstrings[python] ~=0.18", "markdown-include ~=0.6", ]
+mkdocs = [
+    "mkdocs ~=1.4",
+    "mkdocs-material ~=9.1",
+    "mkdocstrings[python] ~=0.21",
+    "markdown-include ~=0.8",
+]
+
+[tool.pyprojectx.pdm]
+requirements = "pdm==2.5.2"
+post-install = "pw@pre-commit install"
 
 [tool.pyprojectx.aliases]
-install = "poetry install"
-run = "poetry run pyprojectx -t pyproject.toml "
-outdated = "poetry show --outdated"
+install = "pdm install"
+run = "pdm run pyprojectx -t pyproject.toml "
+outdated = "pdm update --outdated"
 clean = "rm -r .venv .pytest_cache dist"
-clean-all = """\
-pw@clean
-rm -r .pyprojectx"""
+clean-all = "pw@clean\nrm -r .pyprojectx"
 black = "black src tests"
 isort = "isort src tests"
-unit-test = "poetry run pytest tests/unit"
-integration-test = "poetry run pytest tests/integration"
+unit-test = "pdm run pytest tests/unit"
+integration-test = "pdm run pytest tests/integration"
 test = "pw@unit-test && pw@integration-test"
 check-pylint = "pylint src tests"
 check-black = "black src tests --check"
 check = "pw@check-black && pw@check-pylint && pw@test"
-build = "pw@install && pw@check && pw@poetry build"
-
-# used in github actions:
-publish = "poetry publish --username __token__"
-prep-release = """\
-# cleanup
-rm -f wrappers.zip .changelog.md
-# extract version from tag
-RELEASE_VERSION="${GITHUB_REF##*/v}"
-pw@poetry version $RELEASE_VERSION
-# replace __version__ in wrapper
-sed -i -e "s/__version__/${RELEASE_VERSION}/g" src/pyprojectx/wrapper/pw.py
-# cleanup sed backup
-rm -r src/pyprojectx/wrapper/pw.py?*
-mkdir -p dist-zip
-cp src/pyprojectx/wrapper/pw.py dist-zip/pw
-cp src/pyprojectx/wrapper/pw.bat dist-zip/pw.bat
-zip -j wrappers.zip dist-zip/pw*
-awk '/-{3,}/{flag=1;next}/Release/{if (flag==1)exit}flag' CHANGELOG.md > .changelog.md
-"""
-
+build = "pw@install && pw@check && pw@pdm build"
+publish = "pdm publish --username __token__"
+prep-release = "# cleanup\nrm -f wrappers.zip .changelog.md\n# extract version from tag\nRELEASE_VERSION=\"${GITHUB_REF}\"\n# replace __version__ in wrapper\nsed -i -e \"s/__version__/${RELEASE_VERSION}/g\" src/pyprojectx/wrapper/pw.py\n# cleanup sed backup\nrm -r src/pyprojectx/wrapper/pw.py?*\nmkdir -p dist-zip\ncp src/pyprojectx/wrapper/pw.py dist-zip/pw\ncp src/pyprojectx/wrapper/pw.bat dist-zip/pw.bat\nzip -j wrappers.zip dist-zip/pw*\nawk '/-{3,}/{flag=1;next}/Release/{if (flag==1)exit}flag' CHANGELOG.md > .changelog.md\n"
 generate-usage = "pw@ --help > docs/docs/usage.txt"
 serve-docs = "@mkdocs: cd docs && mkdocs serve"
 generate-docs = "@mkdocs: pw@generate-usage && cd docs && mkdocs build"
 deploy-docs = "@mkdocs: cd docs && mkdocs gh-deploy"
 
 [tool.pyprojectx.os.win.aliases]
 clean = "rmdir /s/q .venv .pytest_cache dist"
-clean-all = """\
-pw@clean
-rmdir /s/q .pyprojectx"""
+clean-all = "pw@clean\nrmdir /s/q .pyprojectx"
+
+[build-system]
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
```

### Comparing `pyprojectx-1.0.0b1/src/pyprojectx/cli.py` & `pyprojectx-1.0.0b2/src/pyprojectx/cli.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b1/src/pyprojectx/config.py` & `pyprojectx-1.0.0b2/src/pyprojectx/config.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b1/src/pyprojectx/env.py` & `pyprojectx-1.0.0b2/src/pyprojectx/env.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b1/src/pyprojectx/initializer/initializers.py` & `pyprojectx-1.0.0b2/src/pyprojectx/initializer/initializers.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b1/src/pyprojectx/initializer/pdm-template.toml` & `pyprojectx-1.0.0b2/src/pyprojectx/initializer/pdm-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b1/src/pyprojectx/initializer/poetry-template.toml` & `pyprojectx-1.0.0b2/src/pyprojectx/initializer/poetry-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b1/src/pyprojectx/initializer/project-template.toml` & `pyprojectx-1.0.0b2/src/pyprojectx/initializer/project-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b1/src/pyprojectx/wrapper/pw.py` & `pyprojectx-1.0.0b2/src/pyprojectx/wrapper/pw.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import argparse
 import os
 import subprocess
 import sys
 from pathlib import Path
 from venv import EnvBuilder
 
-VERSION = "1.0.0b1"
+VERSION = "__version__"
 
 PYPROJECTX_INSTALL_DIR_ENV_VAR = "PYPROJECTX_INSTALL_DIR"
 PYPROJECTX_PACKAGE_ENV_VAR = "PYPROJECTX_PACKAGE"
 PYPROJECT_TOML = "pyproject.toml"
 DEFAULT_INSTALL_DIR = ".pyprojectx"
 
 CYAN = "\033[96m"
```

### Comparing `pyprojectx-1.0.0b1/PKG-INFO` & `pyprojectx-1.0.0b2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 Metadata-Version: 2.1
 Name: pyprojectx
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Execute scripts from pyproject.toml, installing tools on-the-fly
+Keywords: build dependency pyprojectx
 Home-page: https://github.com/pyprojectx/pyprojectx
+Author-Email: Houbie <ivo@houbrechts-it.be>
 License: MIT
-Keywords: build,dependency,pyprojectx
-Author: Houbie
-Author-email: ivo@houbrechts-it.be
-Requires-Python: >=3.7
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: tomli (>=2.0)
-Requires-Dist: userpath (>=1.8)
-Requires-Dist: virtualenv (>=20.21)
+Project-URL: Homepage, https://github.com/pyprojectx/pyprojectx
 Project-URL: Documentation, https://pyprojectx.github.io
+Requires-Python: >=3.7
+Requires-Dist: tomli>=2.0.1
+Requires-Dist: virtualenv>=20.21.0
+Requires-Dist: userpath>=1.8.0
 Description-Content-Type: text/markdown
 
 ![pyprojectx](docs/docs/assets/px.png)
 
 # Pyprojectx: All-inclusive Python Projects
 
 Execute scripts from pyproject.toml, installing tools on-the-fly
@@ -156,8 +149,7 @@
   to use your local pyprojectx copy in another project.
 ```shell
 # Linux, Mac
 export PYPROJECTX_PACKAGE=path/to/pyprojectx
 # windows
 set PYPROJECTX_PACKAGE=path/to/pyprojectx
 ```
-
```

