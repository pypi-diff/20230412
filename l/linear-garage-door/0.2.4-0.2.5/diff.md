# Comparing `tmp/linear_garage_door-0.2.4.tar.gz` & `tmp/linear_garage_door-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linear_garage_door-0.2.4.tar", max compression
+gzip compressed data, was "linear_garage_door-0.2.5.tar", max compression
```

## Comparing `linear_garage_door-0.2.4.tar` & `linear_garage_door-0.2.5.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1098 2023-02-05 15:11:42.260122 linear_garage_door-0.2.4/LICENSE
--rw-r--r--   0        0        0     3005 2023-02-05 15:11:42.260122 linear_garage_door-0.2.4/README.md
--rw-r--r--   0        0        0     2327 2023-02-05 15:11:42.260122 linear_garage_door-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    18997 2023-02-05 15:11:42.260122 linear_garage_door-0.2.4/src/linear_garage_door/__init__.py
--rw-r--r--   0        0        0      861 2023-02-05 15:11:42.260122 linear_garage_door-0.2.4/src/linear_garage_door/_util.py
--rw-r--r--   0        0        0      938 2023-02-05 15:11:42.260122 linear_garage_door-0.2.4/src/linear_garage_door/const.py
--rw-r--r--   0        0        0      390 2023-02-05 15:11:42.260122 linear_garage_door-0.2.4/src/linear_garage_door/errors.py
--rw-r--r--   0        0        0        0 2023-02-05 15:11:42.260122 linear_garage_door-0.2.4/src/linear_garage_door/py.typed
--rw-r--r--   0        0        0     3433 2023-02-05 15:11:42.260122 linear_garage_door-0.2.4/src/linear_garage_door/ws.py
--rw-r--r--   0        0        0     3906 1970-01-01 00:00:00.000000 linear_garage_door-0.2.4/setup.py
--rw-r--r--   0        0        0     4360 1970-01-01 00:00:00.000000 linear_garage_door-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/LICENSE
+-rw-r--r--   0        0        0     3005 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/README.md
+-rw-r--r--   0        0        0     2327 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    18672 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/src/linear_garage_door/__init__.py
+-rw-r--r--   0        0        0      861 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/src/linear_garage_door/_util.py
+-rw-r--r--   0        0        0      938 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/src/linear_garage_door/const.py
+-rw-r--r--   0        0        0      703 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/src/linear_garage_door/errors.py
+-rw-r--r--   0        0        0        0 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/src/linear_garage_door/py.typed
+-rw-r--r--   0        0        0     3433 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/src/linear_garage_door/ws.py
+-rw-r--r--   0        0        0     4360 1970-01-01 00:00:00.000000 linear_garage_door-0.2.5/PKG-INFO
```

### Comparing `linear_garage_door-0.2.4/LICENSE` & `linear_garage_door-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linear_garage_door-0.2.4/README.md` & `linear_garage_door-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `linear_garage_door-0.2.4/pyproject.toml` & `linear_garage_door-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linear-garage-door"
-version = "0.2.4"
+version = "0.2.5"
 description = "Control Linear Garage Doors with Python"
 authors = [
     "IceBotYT <icebotyt@outlook.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `linear_garage_door-0.2.4/src/linear_garage_door/__init__.py` & `linear_garage_door-0.2.5/src/linear_garage_door/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,15 @@
 import uuid
 from typing import Any, Awaitable, Callable
 
 import aiohttp
 
 from ._util import create_request
 from .const import MessageTypes
-from .errors import (
-    InvalidDeviceIDError,
-    InvalidLoginError,
-    NotOpenError,
-    ResponseError,
-    UnexpectedError,
-)
+from .errors import InvalidDeviceIDError, InvalidLoginError, NotOpenError, ResponseError
 from .ws import WebSocketMonitor
 
 
 class Linear:
     """A Linear account.
 
     Instantiate this class then run [`login()`][linear_garage_door.Linear.login] with your credentials to connect.
@@ -105,15 +99,15 @@
             valid = True
             try:
                 uuid.UUID(str(device_id))
             except ValueError:
                 valid = False
 
             if not valid:
-                raise InvalidDeviceIDError("device_id must be a UUID.")
+                raise InvalidDeviceIDError()
             else:
                 device_id = device_id.upper()
 
         return device_id
 
     async def _await_for_any_msg(self: Linear) -> dict[str, Any]:
         future: asyncio.Future[dict[str, Any]] = asyncio.Future()
@@ -122,16 +116,16 @@
             future.set_result(data)
             self._internal_callback = None
 
         self._internal_callback = _got_resp
 
         try:
             result = await asyncio.wait_for(future, timeout=10.0)
-        except asyncio.TimeoutError as e:
-            raise e
+        except asyncio.TimeoutError:
+            raise
 
         return result
 
     async def _await_for_msg_type(self: Linear, msg_type: str) -> dict[str, Any]:
         future: asyncio.Future[dict[str, Any]] = asyncio.Future()
 
         async def _got_resp(data: dict[str, Any]) -> None:
@@ -139,16 +133,16 @@
                 future.set_result(data)
                 self._internal_callback = None
 
         self._internal_callback = _got_resp
 
         try:
             result = await asyncio.wait_for(future, timeout=10.0)
-        except asyncio.TimeoutError as e:
-            raise e
+        except asyncio.TimeoutError:
+            raise
 
         return result
 
     async def _await_for_dev_state_report(self: Linear) -> dict[str, Any]:
         future: asyncio.Future[dict[str, Any]] = asyncio.Future()
 
         async def _got_resp(response: dict[str, Any]) -> None:
@@ -159,29 +153,29 @@
                 future.set_result(response)
                 self._internal_callback = None
 
         self._internal_callback = _got_resp
 
         try:
             result = await asyncio.wait_for(future, timeout=10.0)
-        except asyncio.TimeoutError as e:
-            raise e
+        except asyncio.TimeoutError:
+            raise
 
         return result
 
     async def _message_callback(self: Linear, data: dict[str, Any]) -> None:
         if self._internal_callback:
             # Override user-provided callback
             await self._internal_callback(data)
         elif self.on_device_state_event:
             await self.on_device_state_event(data)
 
     def _check_if_open(self: Linear) -> None:
         if not self.open:
-            raise NotOpenError("The WebSocket has not been opened. Call login() first.")
+            raise NotOpenError()
 
     async def _keepalive(self: Linear) -> None:
         while True:
             if not self.open:
                 return
 
             request = create_request(
@@ -268,34 +262,31 @@
         if ws_monitor.monitor is None or ws_monitor.monitor.done():
             await ws_monitor.start_monitor()
         ws = ws_monitor.websocket
 
         # Start keepalive task
         self._keepalive_task = asyncio.create_task(self._keepalive())
 
-        if ws is None:
-            raise UnexpectedError("ws is None when it should be.")
+        assert ws is not None
 
         self._monitor = ws_monitor
         self._ws = ws
 
         await ws.send_str(request)
 
         response = await self._await_for_any_msg()
 
         if (
             response["Type"] == MessageTypes.GOODBYE.value
             and response["Headers"]["UserID"] == ""
         ):
             if response["Headers"]["Reason"] == "InvalidLogin":
-                raise InvalidLoginError(
-                    "Login provided is invalid, please check the email and password"
-                )
+                raise InvalidLoginError()
 
-            raise InvalidLoginError("Login error: ", response["Headers"]["Reason"])
+            raise InvalidLoginError(response["Headers"]["Reason"])
 
         self._user_id = response["Headers"]["UserID"]
         self._user_email = response["Headers"]["UserEmail"]
 
         return response
 
     async def get_sites(self: Linear) -> list[dict[str, str]]:
```

### Comparing `linear_garage_door-0.2.4/src/linear_garage_door/_util.py` & `linear_garage_door-0.2.5/src/linear_garage_door/_util.py`

 * *Files identical despite different names*

### Comparing `linear_garage_door-0.2.4/src/linear_garage_door/const.py` & `linear_garage_door-0.2.5/src/linear_garage_door/const.py`

 * *Files identical despite different names*

### Comparing `linear_garage_door-0.2.4/src/linear_garage_door/ws.py` & `linear_garage_door-0.2.5/src/linear_garage_door/ws.py`

 * *Files identical despite different names*

### Comparing `linear_garage_door-0.2.4/setup.py` & `linear_garage_door-0.2.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,125 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: linear-garage-door
+Version: 0.2.5
+Summary: Control Linear Garage Doors with Python
+Home-page: https://IceBotYT.github.io/linear-garage-door
+License: MIT
+Author: IceBotYT
+Author-email: icebotyt@outlook.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
+Requires-Dist: dnspython (>=2.3.0,<3.0.0)
+Project-URL: Documentation, https://IceBotYT.github.io/linear-garage-door
+Project-URL: Repository, https://github.com/IceBotYT/linear-garage-door
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Linear Garage Door
 
-packages = \
-['linear_garage_door']
+[![PyPI](https://img.shields.io/pypi/v/linear-garage-door?style=flat-square)](https://pypi.python.org/pypi/linear-garage-door/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/linear-garage-door?style=flat-square)](https://pypi.python.org/pypi/linear-garage-door/)
+[![PyPI - License](https://img.shields.io/pypi/l/linear-garage-door?style=flat-square)](https://pypi.python.org/pypi/linear-garage-door/)
+[![Coookiecutter - Wolt](https://img.shields.io/badge/cookiecutter-Wolt-00c2e8?style=flat-square&logo=cookiecutter&logoColor=D4AA00&link=https://github.com/woltapp/wolt-python-package-cookiecutter)](https://github.com/woltapp/wolt-python-package-cookiecutter)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp>=3.8.1,<4.0.0',
- 'certifi>=2022.12.7,<2023.0.0',
- 'dnspython>=2.3.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'linear-garage-door',
-    'version': '0.2.4',
-    'description': 'Control Linear Garage Doors with Python',
-    'long_description': "# Linear Garage Door\n\n[![PyPI](https://img.shields.io/pypi/v/linear-garage-door?style=flat-square)](https://pypi.python.org/pypi/linear-garage-door/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/linear-garage-door?style=flat-square)](https://pypi.python.org/pypi/linear-garage-door/)\n[![PyPI - License](https://img.shields.io/pypi/l/linear-garage-door?style=flat-square)](https://pypi.python.org/pypi/linear-garage-door/)\n[![Coookiecutter - Wolt](https://img.shields.io/badge/cookiecutter-Wolt-00c2e8?style=flat-square&logo=cookiecutter&logoColor=D4AA00&link=https://github.com/woltapp/wolt-python-package-cookiecutter)](https://github.com/woltapp/wolt-python-package-cookiecutter)\n\n\n---\n\n**Documentation**: [https://IceBotYT.github.io/linear-garage-door](https://IceBotYT.github.io/linear-garage-door)\n\n**Source Code**: [https://github.com/IceBotYT/linear-garage-door](https://github.com/IceBotYT/linear-garage-door)\n\n**PyPI**: [https://pypi.org/project/linear-garage-door/](https://pypi.org/project/linear-garage-door/)\n\n---\n\nControl Linear Garage Doors with Python\n\n## Installation\n\n```sh\npip install linear-garage-door\n```\n\n## Development\n\n* Clone this repository\n* Requirements:\n  * [Poetry](https://python-poetry.org/)\n  * Python 3.7+\n* Create a virtual environment and install the dependencies\n\n```sh\npoetry install\n```\n\n* Activate the virtual environment\n\n```sh\npoetry shell\n```\n\n### Testing\n\n```sh\npytest\n```\n\n### Documentation\n\nThe documentation is automatically generated from the content of the [docs directory](./docs) and from the docstrings\n of the public signatures of the source code. The documentation is updated and published as a [Github project page\n ](https://pages.github.com/) automatically as part each release.\n\n### Releasing\n\nTrigger the [Draft release workflow](https://github.com/IceBotYT/linear-garage-door/actions/workflows/draft_release.yml)\n(press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.\n\nFind the draft release from the\n[GitHub releases](https://github.com/IceBotYT/linear-garage-door/releases) and publish it. When\n a release is published, it'll trigger [release](https://github.com/IceBotYT/linear-garage-door/blob/master/.github/workflows/release.yml) workflow which creates PyPI\n release and deploys updated documentation.\n\n### Pre-commit\n\nPre-commit hooks run all the auto-formatters (e.g. `black`, `isort`), linters (e.g. `mypy`, `flake8`), and other quality\n checks to make sure the changeset is in good shape before a commit/push happens.\n\nYou can install the hooks with (runs for each commit):\n\n```sh\npre-commit install\n```\n\nOr if you want them to run only for each push:\n\n```sh\npre-commit install -t pre-push\n```\n\nOr if you want e.g. want to run all checks manually for all files:\n\n```sh\npre-commit run --all-files\n```\n\n---\n\nThis project was generated using the [wolt-python-package-cookiecutter](https://github.com/woltapp/wolt-python-package-cookiecutter) template.\n",
-    'author': 'IceBotYT',
-    'author_email': 'icebotyt@outlook.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://IceBotYT.github.io/linear-garage-door',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
 
+---
+
+**Documentation**: [https://IceBotYT.github.io/linear-garage-door](https://IceBotYT.github.io/linear-garage-door)
+
+**Source Code**: [https://github.com/IceBotYT/linear-garage-door](https://github.com/IceBotYT/linear-garage-door)
+
+**PyPI**: [https://pypi.org/project/linear-garage-door/](https://pypi.org/project/linear-garage-door/)
+
+---
+
+Control Linear Garage Doors with Python
+
+## Installation
+
+```sh
+pip install linear-garage-door
+```
+
+## Development
+
+* Clone this repository
+* Requirements:
+  * [Poetry](https://python-poetry.org/)
+  * Python 3.7+
+* Create a virtual environment and install the dependencies
+
+```sh
+poetry install
+```
+
+* Activate the virtual environment
+
+```sh
+poetry shell
+```
+
+### Testing
+
+```sh
+pytest
+```
+
+### Documentation
+
+The documentation is automatically generated from the content of the [docs directory](./docs) and from the docstrings
+ of the public signatures of the source code. The documentation is updated and published as a [Github project page
+ ](https://pages.github.com/) automatically as part each release.
+
+### Releasing
+
+Trigger the [Draft release workflow](https://github.com/IceBotYT/linear-garage-door/actions/workflows/draft_release.yml)
+(press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.
+
+Find the draft release from the
+[GitHub releases](https://github.com/IceBotYT/linear-garage-door/releases) and publish it. When
+ a release is published, it'll trigger [release](https://github.com/IceBotYT/linear-garage-door/blob/master/.github/workflows/release.yml) workflow which creates PyPI
+ release and deploys updated documentation.
+
+### Pre-commit
+
+Pre-commit hooks run all the auto-formatters (e.g. `black`, `isort`), linters (e.g. `mypy`, `flake8`), and other quality
+ checks to make sure the changeset is in good shape before a commit/push happens.
+
+You can install the hooks with (runs for each commit):
+
+```sh
+pre-commit install
+```
+
+Or if you want them to run only for each push:
+
+```sh
+pre-commit install -t pre-push
+```
+
+Or if you want e.g. want to run all checks manually for all files:
+
+```sh
+pre-commit run --all-files
+```
+
+---
+
+This project was generated using the [wolt-python-package-cookiecutter](https://github.com/woltapp/wolt-python-package-cookiecutter) template.
 
-setup(**setup_kwargs)
```

