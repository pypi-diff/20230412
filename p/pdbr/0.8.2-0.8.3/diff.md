# Comparing `tmp/pdbr-0.8.2.tar.gz` & `tmp/pdbr-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbr-0.8.2.tar", max compression
+gzip compressed data, was "pdbr-0.8.3.tar", max compression
```

## Comparing `pdbr-0.8.2.tar` & `pdbr-0.8.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-01-31 09:17:29.107929 pdbr-0.8.2/LICENSE
--rw-r--r--   0        0        0     6273 2023-01-31 09:17:29.107929 pdbr-0.8.2/README.md
--rw-r--r--   0        0        0      286 2023-01-31 09:17:29.119922 pdbr-0.8.2/pdbr/__init__.py
--rw-r--r--   0        0        0     1239 2023-01-31 09:17:29.119922 pdbr-0.8.2/pdbr/__main__.py
--rw-r--r--   0        0        0     1206 2023-01-31 09:17:29.119922 pdbr-0.8.2/pdbr/_cm.py
--rw-r--r--   0        0        0     1485 2023-01-31 09:17:29.119922 pdbr-0.8.2/pdbr/_console_layout.py
--rw-r--r--   0        0        0    15936 2023-01-31 09:17:29.119922 pdbr-0.8.2/pdbr/_pdbr.py
--rw-r--r--   0        0        0     1306 2023-01-31 09:17:29.119922 pdbr-0.8.2/pdbr/cli.py
--rw-r--r--   0        0        0     1421 2023-01-31 09:17:29.119922 pdbr-0.8.2/pdbr/helpers.py
--rw-r--r--   0        0        0        0 2023-01-31 09:17:29.119922 pdbr-0.8.2/pdbr/middlewares/__init__.py
--rw-r--r--   0        0        0      492 2023-01-31 09:17:29.119922 pdbr-0.8.2/pdbr/middlewares/django.py
--rw-r--r--   0        0        0      334 2023-01-31 09:17:29.119922 pdbr-0.8.2/pdbr/middlewares/starlette.py
--rw-r--r--   0        0        0      782 2023-01-31 09:17:29.119922 pdbr-0.8.2/pdbr/runner.py
--rw-r--r--   0        0        0     3242 2023-01-31 09:17:29.119922 pdbr-0.8.2/pdbr/utils.py
--rw-r--r--   0        0        0     1480 2023-01-31 09:17:29.119922 pdbr-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     7518 1970-01-01 00:00:00.000000 pdbr-0.8.2/setup.py
--rw-r--r--   0        0        0     7608 1970-01-01 00:00:00.000000 pdbr-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-12 21:02:07.507291 pdbr-0.8.3/LICENSE
+-rw-r--r--   0        0        0     6273 2023-04-12 21:02:07.507291 pdbr-0.8.3/README.md
+-rw-r--r--   0        0        0      286 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/__init__.py
+-rw-r--r--   0        0        0     1239 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/__main__.py
+-rw-r--r--   0        0        0     1206 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/_cm.py
+-rw-r--r--   0        0        0     1485 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/_console_layout.py
+-rw-r--r--   0        0        0    15955 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/_pdbr.py
+-rw-r--r--   0        0        0     1306 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/cli.py
+-rw-r--r--   0        0        0     1421 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/middlewares/__init__.py
+-rw-r--r--   0        0        0      492 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/middlewares/django.py
+-rw-r--r--   0        0        0      334 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/middlewares/starlette.py
+-rw-r--r--   0        0        0      782 2023-04-12 21:02:07.519291 pdbr-0.8.3/pdbr/runner.py
+-rw-r--r--   0        0        0     3242 2023-04-12 21:02:07.523291 pdbr-0.8.3/pdbr/utils.py
+-rw-r--r--   0        0        0     1762 2023-04-12 21:02:07.523291 pdbr-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     7608 1970-01-01 00:00:00.000000 pdbr-0.8.3/PKG-INFO
```

### Comparing `pdbr-0.8.2/LICENSE` & `pdbr-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.2/README.md` & `pdbr-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.2/pdbr/__main__.py` & `pdbr-0.8.3/pdbr/__main__.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.2/pdbr/_cm.py` & `pdbr-0.8.3/pdbr/_cm.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.2/pdbr/_console_layout.py` & `pdbr-0.8.3/pdbr/_console_layout.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.2/pdbr/_pdbr.py` & `pdbr-0.8.3/pdbr/_pdbr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import inspect
 import io
 import re
+from inspect import getsourcelines
 from pathlib import Path
-from pdb import Pdb, getsourcelines
+from pdb import Pdb
 
 import sqlparse
 from rich import box, markup
 from rich._inspect import Inspect
 from rich.console import Console
 from rich.panel import Panel
 from rich.pretty import pprint
```

### Comparing `pdbr-0.8.2/pdbr/cli.py` & `pdbr-0.8.3/pdbr/cli.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.2/pdbr/helpers.py` & `pdbr-0.8.3/pdbr/helpers.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.2/pdbr/runner.py` & `pdbr-0.8.3/pdbr/runner.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.2/pdbr/utils.py` & `pdbr-0.8.3/pdbr/utils.py`

 * *Files identical despite different names*

### Comparing `pdbr-0.8.2/pyproject.toml` & `pdbr-0.8.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdbr"
-version = "0.8.2"
+version = "0.8.3"
 description = "Pdb with Rich library."
 authors = ["Can Sarigol <ertugrulsarigol@gmail.com>"]
 packages = [
     { include = "pdbr" }
 ]
 readme = "README.md"
 homepage = "https://github.com/cansarigol/pdbr"
@@ -27,35 +27,49 @@
 rich = "*"
 celery = {version = "^5.2.2", optional = true}
 ipython = {version = "*", optional = true}
 pyreadline3 = {version = "^3.4.1", markers = "sys_platform == 'win32'"}
 icecream = "*"
 sqlparse = "*"
 
-[tool.poetry.dev-dependencies]
-nox = "^2020.5.24"
-
 [tool.poetry.extras]
 celery = ["celery"]
 ipython = ["ipython"]
 
 [tool.poetry.scripts]
 pdbr = 'pdbr.cli:shell'
 pdbr_telnet = 'pdbr.cli:telnet'
 
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.0.261"
+nox = "^2022.11.21"
+
 [build-system]
 requires = ["poetry>=1.0.0", "setuptools"]
 build-backend = "poetry.masonry.api"
 
 [tool.vulture]
 make_whitelist = true
 min_confidence = 80
 paths = ["pdbr", "tests"]
 sort_by_size = true
 verbose = false
 
 [project]
 name = "pdbr"
-version = "0.8.2"
+version = "0.8.3"
 
 [tool.setuptools]
 py-modules = []
+
+[tool.ruff]
+select = [
+    "E",  # pycodestyle errors
+    "W",  # pycodestyle warnings
+    "F",  # pyflakes
+    "I",   # isort
+    "B",   # flake8-bugbear
+    "C4",  # flake8-comprehensions
+    "PIE", # flake8-pie
+    "ERA", # eradicate
+]
+line-length = 88
```

### Comparing `pdbr-0.8.2/setup.py` & `pdbr-0.8.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,287 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pdbr
+Version: 0.8.3
+Summary: Pdb with Rich library.
+Home-page: https://github.com/cansarigol/pdbr
+Author: Can Sarigol
+Author-email: ertugrulsarigol@gmail.com
+Requires-Python: >=3.7.9,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: celery
+Provides-Extra: ipython
+Requires-Dist: celery (>=5.2.2,<6.0.0) ; extra == "celery"
+Requires-Dist: icecream
+Requires-Dist: ipython ; extra == "ipython"
+Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0) ; sys_platform == "win32"
+Requires-Dist: rich
+Requires-Dist: sqlparse
+Project-URL: Repository, https://github.com/cansarigol/pdbr
+Description-Content-Type: text/markdown
 
-packages = \
-['pdbr', 'pdbr.middlewares']
+# pdbr
 
-package_data = \
-{'': ['*']}
+[![PyPI version](https://badge.fury.io/py/pdbr.svg)](https://pypi.org/project/pdbr/) [![Python Version](https://img.shields.io/pypi/pyversions/pdbr.svg)](https://pypi.org/project/pdbr/) [![](https://github.com/cansarigol/pdbr/workflows/Test/badge.svg)](https://github.com/cansarigol/pdbr/actions?query=workflow%3ATest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/cansarigol/pdbr/master.svg)](https://results.pre-commit.ci/latest/github/cansarigol/pdbr/master)
 
-install_requires = \
-['icecream', 'rich', 'sqlparse']
-
-extras_require = \
-{':sys_platform == "win32"': ['pyreadline3>=3.4.1,<4.0.0'],
- 'celery': ['celery>=5.2.2,<6.0.0'],
- 'ipython': ['ipython']}
-
-entry_points = \
-{'console_scripts': ['pdbr = pdbr.cli:shell', 'pdbr_telnet = pdbr.cli:telnet']}
-
-setup_kwargs = {
-    'name': 'pdbr',
-    'version': '0.8.2',
-    'description': 'Pdb with Rich library.',
-    'long_description': '# pdbr\n\n[![PyPI version](https://badge.fury.io/py/pdbr.svg)](https://pypi.org/project/pdbr/) [![Python Version](https://img.shields.io/pypi/pyversions/pdbr.svg)](https://pypi.org/project/pdbr/) [![](https://github.com/cansarigol/pdbr/workflows/Test/badge.svg)](https://github.com/cansarigol/pdbr/actions?query=workflow%3ATest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/cansarigol/pdbr/master.svg)](https://results.pre-commit.ci/latest/github/cansarigol/pdbr/master)\n\n\npdbr is intended to make the PDB results more colorful. it uses [Rich](https://github.com/willmcgugan/rich) library to carry out that.\n\n\n## Installing\n\nInstall with `pip` or your favorite PyPi package manager.\n\n```\npip install pdbr\n```\n\n\n## Breakpoint\n\nIn order to use ```breakpoint()```, set **PYTHONBREAKPOINT** with "pdbr.set_trace"\n\n```python\nimport os\n\nos.environ["PYTHONBREAKPOINT"] = "pdbr.set_trace"\n```\n\nor just import pdbr\n\n```python\nimport pdbr\n```\n\n## New commands\n### (ic)ecream\n🍦 [Icecream](https://github.com/gruns/icecream) print.\n### (i)nspect / inspectall | ia\n[rich.inspect](https://rich.readthedocs.io/en/latest/introduction.html?s=03#rich-inspector)\n### search | src\nSearch a phrase in the current frame.\nIn order to repeat the last one, type **/** character as arg.\n### sql\nDisplay value in sql format.\n![](/images/image13.png)\n\nIt can be used for Django model queries as follows.\n```\n>>> sql str(Users.objects.all().query)\n```\n![](/images/image14.png)\n### (syn)tax\n[ val,lexer ] Display [lexer](https://pygments.org/docs/lexers/).\n### (v)ars\nGet the local variables list as table.\n### varstree | vt\nGet the local variables list as tree.\n\n![](/images/image5.png)\n\n## Config\nConfig is specified in **setup.cfg** and can be local or global. Local config (current working directory) has precedence over global (default) one. Global config must be located in `$XDG_CONFIG_HOME/pdbr/` directory.\n\n### Style\nIn order to use Rich\'s traceback, style, and theme:\n\n```\n[pdbr]\nstyle = yellow\nuse_traceback = True\ntheme = friendly\n```\n\n### History\n**store_history** setting is used to keep and reload history, even the prompt is closed and opened again:\n```\n[pdbr]\n...\nstore_history=.pdbr_history\n```\n\n## Celery\nIn order to use **Celery** remote debugger with pdbr, use ```celery_set_trace``` as below sample. For more information see the [Celery user guide](https://docs.celeryproject.org/en/stable/userguide/debugging.html).\n\n```python\nfrom celery import Celery\n\napp = Celery(\'tasks\', broker=\'pyamqp://guest@localhost//\')\n\n@app.task\ndef add(x, y):\n\n    import pdbr; pdbr.celery_set_trace()\n\n    return x + y\n\n```\n#### Telnet\nInstead of using `telnet` or `nc`, in terms of using pdbr style, `pdbr_telnet` command can be used.\n![](/images/image6.png)\n\nAlso in order to activate history and be able to use arrow keys, install and use [rlwrap](https://github.com/hanslub42/rlwrap) package.\n\n```\nrlwrap -H \'~/.pdbr_history\' pdbr_telnet localhost 6899\n```\n\n## IPython\n\n`pdbr` integrates with [IPython](https://ipython.readthedocs.io/).\n\nThis makes [`%magics`](https://ipython.readthedocs.io/en/stable/interactive/magics.html) available, for example:\n\n```python\n(Pdbr) %timeit range(100)\n104 ns ± 2.05 ns per loop (mean ± std. dev. of 7 runs, 10,000,000 loops each)\n```\n\nTo enable `IPython` features, install it separately, or like below:\n\n```\npip install pdbr[ipython]\n```\n\n## pytest\nIn order to use `pdbr` with pytest `--pdb` flag, add `addopts` setting in your pytest.ini.\n\n```\n[pytest]\naddopts: --pdbcls=pdbr:RichPdb\n```\n## Context Decorator\n`pdbr_context` and `apdbr_context` (`asyncio` corresponding) can be used as **with statement** or **decorator**. It calls `post_mortem` if `traceback` is not none.\n\n```python\nfrom pdbr import apdbr_context, pdbr_context\n\n@pdbr_context()\ndef foo():\n    ...\n\ndef bar():\n    with pdbr_context():\n        ...\n\n\n@apdbr_context()\nasync def foo():\n    ...\n\nasync def bar():\n    async with apdbr_context():\n        ...\n```\n\n![](/images/image12.png)\n## Django DiscoverRunner\nTo being activated the pdb in Django test, change `TEST_RUNNER` like below. Unlike Django (since you are not allowed to use for smaller versions than 3), pdbr runner can be used for version 1.8 and subsequent versions.\n\n```\nTEST_RUNNER = "pdbr.runner.PdbrDiscoverRunner"\n```\n![](/images/image10.png)\n## Middlewares\n### Starlette\n```python\nfrom fastapi import FastAPI\nfrom pdbr.middlewares.starlette import PdbrMiddleware\n\napp = FastAPI()\n\napp.add_middleware(PdbrMiddleware, debug=True)\n\n\n@app.get("/")\nasync def main():\n    1 / 0\n    return {"message": "Hello World"}\n```\n### Django\nIn order to catch the problematic codes with post mortem, place the middleware class.\n\n```\nMIDDLEWARE = (\n    ...\n    "pdbr.middlewares.django.PdbrMiddleware",\n)\n```\n![](/images/image11.png)\n## Shell\nRunning `pdbr` command in terminal starts an `IPython` terminal app instance. Unlike default `TerminalInteractiveShell`, the new shell uses pdbr as debugger class instead of `ipdb`.\n#### %debug magic sample\n![](/images/image9.png)\n### As a Script\nIf `pdbr` command is used with an argument, it is invoked as a script and [debugger-commands](https://docs.python.org/3/library/pdb.html#debugger-commands) can be used with it.\n```python\n# equivalent code: `python -m pdbr -c \'b 5\' my_test.py`\npdbr -c \'b 5\' my_test.py\n\n>>> Breakpoint 1 at /my_test.py:5\n> /my_test.py(3)<module>()\n      1\n      2\n----> 3 def test():\n      4         foo = "foo"\n1     5         bar = "bar"\n\n(Pdbr)\n\n```\n### Terminal\n#### Django shell sample\n![](/images/image7.png)\n\n## Vscode user snippet\n\nTo create or edit your own snippets, select **User Snippets** under **File > Preferences** (**Code > Preferences** on macOS), and then select **python.json**.\n\nPlace the below snippet in json file for **pdbr**.\n\n```\n{\n  ...\n  "pdbr": {\n        "prefix": "pdbr",\n        "body": "import pdbr; pdbr.set_trace()",\n        "description": "Code snippet for pdbr debug"\n    },\n}\n```\n\nFor **Celery** debug.\n\n```\n{\n  ...\n  "rdbr": {\n        "prefix": "rdbr",\n        "body": "import pdbr; pdbr.celery_set_trace()",\n        "description": "Code snippet for Celery pdbr debug"\n    },\n}\n```\n\n## Samples\n![](/images/image1.png)\n\n![](/images/image3.png)\n\n![](/images/image4.png)\n\n### Traceback\n![](/images/image2.png)\n',
-    'author': 'Can Sarigol',
-    'author_email': 'ertugrulsarigol@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/cansarigol/pdbr',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.9,<4.0.0',
+
+pdbr is intended to make the PDB results more colorful. it uses [Rich](https://github.com/willmcgugan/rich) library to carry out that.
+
+
+## Installing
+
+Install with `pip` or your favorite PyPi package manager.
+
+```
+pip install pdbr
+```
+
+
+## Breakpoint
+
+In order to use ```breakpoint()```, set **PYTHONBREAKPOINT** with "pdbr.set_trace"
+
+```python
+import os
+
+os.environ["PYTHONBREAKPOINT"] = "pdbr.set_trace"
+```
+
+or just import pdbr
+
+```python
+import pdbr
+```
+
+## New commands
+### (ic)ecream
+🍦 [Icecream](https://github.com/gruns/icecream) print.
+### (i)nspect / inspectall | ia
+[rich.inspect](https://rich.readthedocs.io/en/latest/introduction.html?s=03#rich-inspector)
+### search | src
+Search a phrase in the current frame.
+In order to repeat the last one, type **/** character as arg.
+### sql
+Display value in sql format.
+![](/images/image13.png)
+
+It can be used for Django model queries as follows.
+```
+>>> sql str(Users.objects.all().query)
+```
+![](/images/image14.png)
+### (syn)tax
+[ val,lexer ] Display [lexer](https://pygments.org/docs/lexers/).
+### (v)ars
+Get the local variables list as table.
+### varstree | vt
+Get the local variables list as tree.
+
+![](/images/image5.png)
+
+## Config
+Config is specified in **setup.cfg** and can be local or global. Local config (current working directory) has precedence over global (default) one. Global config must be located in `$XDG_CONFIG_HOME/pdbr/` directory.
+
+### Style
+In order to use Rich's traceback, style, and theme:
+
+```
+[pdbr]
+style = yellow
+use_traceback = True
+theme = friendly
+```
+
+### History
+**store_history** setting is used to keep and reload history, even the prompt is closed and opened again:
+```
+[pdbr]
+...
+store_history=.pdbr_history
+```
+
+## Celery
+In order to use **Celery** remote debugger with pdbr, use ```celery_set_trace``` as below sample. For more information see the [Celery user guide](https://docs.celeryproject.org/en/stable/userguide/debugging.html).
+
+```python
+from celery import Celery
+
+app = Celery('tasks', broker='pyamqp://guest@localhost//')
+
+@app.task
+def add(x, y):
+
+    import pdbr; pdbr.celery_set_trace()
+
+    return x + y
+
+```
+#### Telnet
+Instead of using `telnet` or `nc`, in terms of using pdbr style, `pdbr_telnet` command can be used.
+![](/images/image6.png)
+
+Also in order to activate history and be able to use arrow keys, install and use [rlwrap](https://github.com/hanslub42/rlwrap) package.
+
+```
+rlwrap -H '~/.pdbr_history' pdbr_telnet localhost 6899
+```
+
+## IPython
+
+`pdbr` integrates with [IPython](https://ipython.readthedocs.io/).
+
+This makes [`%magics`](https://ipython.readthedocs.io/en/stable/interactive/magics.html) available, for example:
+
+```python
+(Pdbr) %timeit range(100)
+104 ns ± 2.05 ns per loop (mean ± std. dev. of 7 runs, 10,000,000 loops each)
+```
+
+To enable `IPython` features, install it separately, or like below:
+
+```
+pip install pdbr[ipython]
+```
+
+## pytest
+In order to use `pdbr` with pytest `--pdb` flag, add `addopts` setting in your pytest.ini.
+
+```
+[pytest]
+addopts: --pdbcls=pdbr:RichPdb
+```
+## Context Decorator
+`pdbr_context` and `apdbr_context` (`asyncio` corresponding) can be used as **with statement** or **decorator**. It calls `post_mortem` if `traceback` is not none.
+
+```python
+from pdbr import apdbr_context, pdbr_context
+
+@pdbr_context()
+def foo():
+    ...
+
+def bar():
+    with pdbr_context():
+        ...
+
+
+@apdbr_context()
+async def foo():
+    ...
+
+async def bar():
+    async with apdbr_context():
+        ...
+```
+
+![](/images/image12.png)
+## Django DiscoverRunner
+To being activated the pdb in Django test, change `TEST_RUNNER` like below. Unlike Django (since you are not allowed to use for smaller versions than 3), pdbr runner can be used for version 1.8 and subsequent versions.
+
+```
+TEST_RUNNER = "pdbr.runner.PdbrDiscoverRunner"
+```
+![](/images/image10.png)
+## Middlewares
+### Starlette
+```python
+from fastapi import FastAPI
+from pdbr.middlewares.starlette import PdbrMiddleware
+
+app = FastAPI()
+
+app.add_middleware(PdbrMiddleware, debug=True)
+
+
+@app.get("/")
+async def main():
+    1 / 0
+    return {"message": "Hello World"}
+```
+### Django
+In order to catch the problematic codes with post mortem, place the middleware class.
+
+```
+MIDDLEWARE = (
+    ...
+    "pdbr.middlewares.django.PdbrMiddleware",
+)
+```
+![](/images/image11.png)
+## Shell
+Running `pdbr` command in terminal starts an `IPython` terminal app instance. Unlike default `TerminalInteractiveShell`, the new shell uses pdbr as debugger class instead of `ipdb`.
+#### %debug magic sample
+![](/images/image9.png)
+### As a Script
+If `pdbr` command is used with an argument, it is invoked as a script and [debugger-commands](https://docs.python.org/3/library/pdb.html#debugger-commands) can be used with it.
+```python
+# equivalent code: `python -m pdbr -c 'b 5' my_test.py`
+pdbr -c 'b 5' my_test.py
+
+>>> Breakpoint 1 at /my_test.py:5
+> /my_test.py(3)<module>()
+      1
+      2
+----> 3 def test():
+      4         foo = "foo"
+1     5         bar = "bar"
+
+(Pdbr)
+
+```
+### Terminal
+#### Django shell sample
+![](/images/image7.png)
+
+## Vscode user snippet
+
+To create or edit your own snippets, select **User Snippets** under **File > Preferences** (**Code > Preferences** on macOS), and then select **python.json**.
+
+Place the below snippet in json file for **pdbr**.
+
+```
+{
+  ...
+  "pdbr": {
+        "prefix": "pdbr",
+        "body": "import pdbr; pdbr.set_trace()",
+        "description": "Code snippet for pdbr debug"
+    },
+}
+```
+
+For **Celery** debug.
+
+```
+{
+  ...
+  "rdbr": {
+        "prefix": "rdbr",
+        "body": "import pdbr; pdbr.celery_set_trace()",
+        "description": "Code snippet for Celery pdbr debug"
+    },
 }
+```
+
+## Samples
+![](/images/image1.png)
+
+![](/images/image3.png)
+
+![](/images/image4.png)
 
+### Traceback
+![](/images/image2.png)
 
-setup(**setup_kwargs)
```

