# Comparing `tmp/dep_checker-0.7.0.tar.gz` & `tmp/dep_checker-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dep_checker-0.7.0.tar", last modified: Thu Jun  9 14:52:08 2022, max compression
+gzip compressed data, was "dep_checker-0.7.1.tar", last modified: Wed Apr 12 21:10:14 2023, max compression
```

## Comparing `dep_checker-0.7.0.tar` & `dep_checker-0.7.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0 runner    (1001) docker     (121)     4674 2022-06-09 14:52:08.350407 dep_checker-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     4655 2022-06-09 14:52:08.350407 dep_checker-0.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-06-09 14:52:08.342406 dep_checker-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6306 2022-06-09 14:52:08.350407 dep_checker-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-06-09 14:52:08.350407 dep_checker-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 14:51:22.939290 dep_checker-0.7.0/dep_checker/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-06-09 14:51:22.939290 dep_checker-0.7.0/dep_checker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11522 2022-06-09 14:51:22.939290 dep_checker-0.7.0/dep_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6812 2022-06-09 14:51:22.939290 dep_checker-0.7.0/dep_checker/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5312 2022-06-09 14:51:22.939290 dep_checker-0.7.0/dep_checker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6274 2023-04-12 21:10:14.740577 dep_checker-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-04-12 21:10:14.736577 dep_checker-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-12 21:10:14.732577 dep_checker-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4657 2023-04-12 21:10:14.740577 dep_checker-0.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-04-12 21:10:14.736577 dep_checker-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5017 2023-04-12 21:09:43.820131 dep_checker-0.7.1/dep_checker/_stdlib_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11522 2023-04-12 21:09:43.820131 dep_checker-0.7.1/dep_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 21:09:43.820131 dep_checker-0.7.1/dep_checker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-04-12 21:09:43.820131 dep_checker-0.7.1/dep_checker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6812 2023-04-12 21:09:43.820131 dep_checker-0.7.1/dep_checker/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5129 2023-04-12 21:09:43.820131 dep_checker-0.7.1/dep_checker/utils.py
```

### Comparing `dep_checker-0.7.0/pyproject.toml` & `dep_checker-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "dep_checker"
-version = "0.7.0"
+version = "0.7.1"
 description = "Tool to check all requirements are actually required."
 readme = "README.rst"
 keywords = [ "dependencies", "linter", "pre-commit",]
 dynamic = []
 dependencies = [
     "astatine>=0.3.0",
     "click>=7.1.2",
     "configconfig>=0.4.0",
     "consolekit>=0.4.0",
     "dom-toml>=0.2.0",
     "domdf-python-tools>=3.2.0",
     "shippinglabel>=0.1.0",
-    "stdlib-list>=0.7.0",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -147,15 +146,15 @@
     "__new__",
     "__getnewargs__",
     "__abstractmethods__",
     "__hash__",
 ]
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 incremental = false
```

### Comparing `dep_checker-0.7.0/README.rst` & `dep_checker-0.7.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 	:target: https://github.com/python-coincidence/dep_checker/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/python-coincidence/dep_checker/workflows/mypy/badge.svg
 	:target: https://github.com/python-coincidence/dep_checker/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/python-coincidence/dep_checker/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/python-coincidence/dep_checker/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/python-coincidence/dep_checker/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/python-coincidence/dep_checker/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/python-coincidence/dep_checker/master?logo=coveralls
 	:target: https://coveralls.io/github/python-coincidence/dep_checker?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/python-coincidence/dep_checker?logo=codefactor
@@ -87,23 +87,23 @@
 .. |license| image:: https://img.shields.io/github/license/python-coincidence/dep_checker
 	:target: https://github.com/python-coincidence/dep_checker/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/python-coincidence/dep_checker
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/python-coincidence/dep_checker/v0.7.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/python-coincidence/dep_checker/v0.7.1
 	:target: https://github.com/python-coincidence/dep_checker/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/python-coincidence/dep_checker
 	:target: https://github.com/python-coincidence/dep_checker/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/dep_checker
 	:target: https://pypi.org/project/dep_checker/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `dep_checker-0.7.0/LICENSE` & `dep_checker-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dep_checker-0.7.0/PKG-INFO` & `dep_checker-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dep-checker
-Version: 0.7.0
+Version: 0.7.1
 Summary: Tool to check all requirements are actually required.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: dependencies,linter,pre-commit
 Home-page: https://github.com/python-coincidence/dep_checker
 Project-URL: Issue Tracker, https://github.com/python-coincidence/dep_checker/issues
 Project-URL: Source Code, https://github.com/python-coincidence/dep_checker
@@ -31,15 +31,14 @@
 Requires-Dist: astatine>=0.3.0
 Requires-Dist: click>=7.1.2
 Requires-Dist: configconfig>=0.4.0
 Requires-Dist: consolekit>=0.4.0
 Requires-Dist: dom-toml>=0.2.0
 Requires-Dist: domdf-python-tools>=3.2.0
 Requires-Dist: shippinglabel>=0.1.0
-Requires-Dist: stdlib-list>=0.7.0
 Description-Content-Type: text/x-rst
 
 
 ############
 dep_checker
 ############
 
@@ -93,16 +92,16 @@
 	:target: https://github.com/python-coincidence/dep_checker/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/python-coincidence/dep_checker/workflows/mypy/badge.svg
 	:target: https://github.com/python-coincidence/dep_checker/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/python-coincidence/dep_checker/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/python-coincidence/dep_checker/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/python-coincidence/dep_checker/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/python-coincidence/dep_checker/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/python-coincidence/dep_checker/master?logo=coveralls
 	:target: https://coveralls.io/github/python-coincidence/dep_checker?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/python-coincidence/dep_checker?logo=codefactor
@@ -128,23 +127,23 @@
 .. |license| image:: https://img.shields.io/github/license/python-coincidence/dep_checker
 	:target: https://github.com/python-coincidence/dep_checker/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/python-coincidence/dep_checker
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/python-coincidence/dep_checker/v0.7.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/python-coincidence/dep_checker/v0.7.1
 	:target: https://github.com/python-coincidence/dep_checker/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/python-coincidence/dep_checker
 	:target: https://github.com/python-coincidence/dep_checker/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/dep_checker
 	:target: https://pypi.org/project/dep_checker/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `dep_checker-0.7.0/dep_checker/__main__.py` & `dep_checker-0.7.1/dep_checker/__main__.py`

 * *Files identical despite different names*

### Comparing `dep_checker-0.7.0/dep_checker/__init__.py` & `dep_checker-0.7.1/dep_checker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 # this package
 from dep_checker.config import AllowedUnused, ConfigReader, NameMapping, NamespacePackages
 from dep_checker.utils import Visitor
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.7.0"
+__version__: str = "0.7.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = (
 		"template",
 		"check_imports",
 		"DepChecker",
 		"PassingRequirement",
```

### Comparing `dep_checker-0.7.0/dep_checker/config.py` & `dep_checker-0.7.1/dep_checker/config.py`

 * *Files identical despite different names*

### Comparing `dep_checker-0.7.0/dep_checker/utils.py` & `dep_checker-0.7.1/dep_checker/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,29 +25,23 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
 import ast
 import re
-import sys
 from typing import Any, Dict, List, Optional, Tuple
 
 # 3rd party
 from astatine import get_attribute_name, is_type_checking
 
-__all__ = ["Visitor", "is_suppress_importerror"]
+# this package
+from dep_checker import _stdlib_list
 
-if sys.version_info < (3, 10):  # pragma: no cover (py310+)
-	# 3rd party
-	from stdlib_list import stdlib_list  # type: ignore[import]
-
-	libraries = stdlib_list()
-else:  # pragma: no cover (<py310)
-	libraries = sys.stdlib_module_names
+__all__ = ["Visitor", "is_suppress_importerror"]
 
 
 class Visitor(ast.NodeVisitor):
 	"""
 	:class:`ast.NodeVisitor` to identify imports in a module.
 	"""
 
@@ -72,15 +66,15 @@
 				if len(name_elements) > 1 and name_elements[1] in children:
 					name = '.'.join(name_elements[:2])
 					break
 		else:
 			# Not a namespace package
 			name = name.split('.')[0]
 
-		if name not in libraries and name != self.pkg_name:
+		if name not in _stdlib_list.stdlib and name != self.pkg_name:
 			self.import_sources.append((name, lineno))
 
 	def visit_Import(self, node: ast.Import) -> None:  # noqa: D102
 		name: ast.alias
 		for name in node.names:
 			self.record_import(name.name, node.lineno)
```

