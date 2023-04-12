# Comparing `tmp/rasa_sdk-3.5.0b1.tar.gz` & `tmp/rasa_sdk-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa_sdk-3.5.0b1.tar", max compression
+gzip compressed data, was "rasa_sdk-3.5.1.tar", max compression
```

## Comparing `rasa_sdk-3.5.0b1.tar` & `rasa_sdk-3.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11553 2023-02-21 17:20:47.646015 rasa_sdk-3.5.0b1/LICENSE.txt
--rw-r--r--   0        0        0     5236 2023-02-21 17:20:47.646015 rasa_sdk-3.5.0b1/README.md
--rw-r--r--   0        0        0     2675 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/pyproject.toml
--rw-r--r--   0        0        0      370 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/__init__.py
--rw-r--r--   0        0        0      947 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/__main__.py
--rw-r--r--   0        0        0        0 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/cli/__init__.py
--rw-r--r--   0        0        0     1528 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/cli/arguments.py
--rw-r--r--   0        0        0      399 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/constants.py
--rw-r--r--   0        0        0     5510 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/endpoint.py
--rw-r--r--   0        0        0     6427 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/events.py
--rw-r--r--   0        0        0     1905 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/exceptions.py
--rw-r--r--   0        0        0    15168 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/executor.py
--rw-r--r--   0        0        0    11265 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/forms.py
--rw-r--r--   0        0        0    12929 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/interfaces.py
--rw-r--r--   0        0        0        0 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/knowledge_base/__init__.py
--rw-r--r--   0        0        0     8842 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/knowledge_base/actions.py
--rw-r--r--   0        0        0     7698 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/knowledge_base/storage.py
--rw-r--r--   0        0        0     6226 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/knowledge_base/utils.py
--rw-r--r--   0        0        0     7066 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/slots.py
--rw-r--r--   0        0        0     1683 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/types.py
--rw-r--r--   0        0        0    11303 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/utils.py
--rw-r--r--   0        0        0      118 2023-02-21 17:20:47.650015 rasa_sdk-3.5.0b1/rasa_sdk/version.py
--rw-r--r--   0        0        0     6408 1970-01-01 00:00:00.000000 rasa_sdk-3.5.0b1/setup.py
--rw-r--r--   0        0        0     6720 1970-01-01 00:00:00.000000 rasa_sdk-3.5.0b1/PKG-INFO
+-rw-r--r--   0        0        0    11553 2023-04-12 09:49:45.759693 rasa_sdk-3.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     5236 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/README.md
+-rw-r--r--   0        0        0     2701 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/pyproject.toml
+-rw-r--r--   0        0        0      370 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/__init__.py
+-rw-r--r--   0        0        0      947 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/cli/__init__.py
+-rw-r--r--   0        0        0     1528 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/cli/arguments.py
+-rw-r--r--   0        0        0      399 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/constants.py
+-rw-r--r--   0        0        0     5510 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/endpoint.py
+-rw-r--r--   0        0        0     6427 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/events.py
+-rw-r--r--   0        0        0     1905 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/exceptions.py
+-rw-r--r--   0        0        0    15168 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/executor.py
+-rw-r--r--   0        0        0    11265 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/forms.py
+-rw-r--r--   0        0        0    12929 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/interfaces.py
+-rw-r--r--   0        0        0        0 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/knowledge_base/__init__.py
+-rw-r--r--   0        0        0     8842 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/knowledge_base/actions.py
+-rw-r--r--   0        0        0     7698 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/knowledge_base/storage.py
+-rw-r--r--   0        0        0     6226 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/knowledge_base/utils.py
+-rw-r--r--   0        0        0     7066 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/slots.py
+-rw-r--r--   0        0        0     1683 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/types.py
+-rw-r--r--   0        0        0    11303 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/utils.py
+-rw-r--r--   0        0        0      116 2023-04-12 09:49:45.763694 rasa_sdk-3.5.1/rasa_sdk/version.py
+-rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 rasa_sdk-3.5.1/setup.py
+-rw-r--r--   0        0        0     6759 1970-01-01 00:00:00.000000 rasa_sdk-3.5.1/PKG-INFO
```

### Comparing `rasa_sdk-3.5.0b1/LICENSE.txt` & `rasa_sdk-3.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/README.md` & `rasa_sdk-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/pyproject.toml` & `rasa_sdk-3.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.black]
 line-length = 88
 target-version = [ "py37", "py38", "py39", "py310",]
 exclude = "((.eggs | .git | .mypy_cache | .pytest_cache | build | dist))"
 
 [tool.poetry]
 name = "rasa-sdk"
-version = "3.5.0b1"
+version = "3.5.1"
 description = "Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants"
 authors = [ "Rasa Technologies GmbH <hi@rasa.com>",]
 maintainers = [ "Tom Bocklisch <tom@rasa.com>",]
 homepage = "https://rasa.com"
 repository = "https://github.com/rasahq/rasa-sdk"
 documentation = "https://rasa.com/docs"
 classifiers = [ "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "License :: OSI Approved :: Apache Software License", "Topic :: Software Development :: Libraries",]
@@ -66,14 +66,15 @@
 python = ">=3.7,<3.11"
 coloredlogs = ">=10,<16"
 sanic = "^21.12.0"
 typing-extensions = ">=4.1.1,<5.0.0"
 Sanic-Cors = "^2.0.0"
 prompt-toolkit = "^3.0,<3.0.29"
 "ruamel.yaml" = ">=0.16.5,<0.18.0"
+websockets = ">=10.0,<11.0"
 
 [tool.poetry.dev-dependencies]
 pytest-cov = "^4.0.0"
 coveralls = "^3.0.1"
 pytest = "^7.2.1"
 black = "22.12.0"
 flake8 = "^5.0.4"
```

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/__main__.py` & `rasa_sdk-3.5.1/rasa_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/cli/arguments.py` & `rasa_sdk-3.5.1/rasa_sdk/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/endpoint.py` & `rasa_sdk-3.5.1/rasa_sdk/endpoint.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/events.py` & `rasa_sdk-3.5.1/rasa_sdk/events.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/exceptions.py` & `rasa_sdk-3.5.1/rasa_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/executor.py` & `rasa_sdk-3.5.1/rasa_sdk/executor.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/forms.py` & `rasa_sdk-3.5.1/rasa_sdk/forms.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/interfaces.py` & `rasa_sdk-3.5.1/rasa_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/knowledge_base/actions.py` & `rasa_sdk-3.5.1/rasa_sdk/knowledge_base/actions.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/knowledge_base/storage.py` & `rasa_sdk-3.5.1/rasa_sdk/knowledge_base/storage.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/knowledge_base/utils.py` & `rasa_sdk-3.5.1/rasa_sdk/knowledge_base/utils.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/slots.py` & `rasa_sdk-3.5.1/rasa_sdk/slots.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/types.py` & `rasa_sdk-3.5.1/rasa_sdk/types.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/rasa_sdk/utils.py` & `rasa_sdk-3.5.1/rasa_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.5.0b1/setup.py` & `rasa_sdk-3.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 
 install_requires = \
 ['Sanic-Cors>=2.0.0,<3.0.0',
  'coloredlogs>=10,<16',
  'prompt-toolkit>=3.0,<3.0.29',
  'ruamel.yaml>=0.16.5,<0.18.0',
  'sanic>=21.12.0,<22.0.0',
- 'typing-extensions>=4.1.1,<5.0.0']
+ 'typing-extensions>=4.1.1,<5.0.0',
+ 'websockets>=10.0,<11.0']
 
 setup_kwargs = {
     'name': 'rasa-sdk',
-    'version': '3.5.0b1',
+    'version': '3.5.1',
     'description': 'Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants',
     'long_description': '# Rasa Python-SDK\n[![Join the chat on Rasa Community Forum](https://img.shields.io/badge/forum-join%20discussions-brightgreen.svg)](https://forum.rasa.com/?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)\n[![Build Status](https://github.com/RasaHQ/rasa-sdk/workflows/Continous%20Integration/badge.svg?event=push)](https://github.com/RasaHQ/rasa-sdk/actions/runs/)\n[![Coverage Status](https://coveralls.io/repos/github/RasaHQ/rasa-sdk/badge.svg?branch=main)](https://coveralls.io/github/RasaHQ/rasa-sdk?branch=main)\n[![PyPI version](https://img.shields.io/pypi/v/rasa-sdk.svg)](https://pypi.python.org/pypi/rasa-sdk)\n\nPython SDK for the development of custom actions for Rasa.\n\n<hr />\n\n💡 **We\'re migrating issues to Jira** 💡\n\nStarting January 2023, issues for Rasa Open Source are located in\n[this Jira board](https://rasa-open-source.atlassian.net/browse/OSS). You can browse issues without being logged in;\nif you want to create issues, you\'ll need to create a Jira account.\n\n<hr />\n\n## Installation\n\nTo install the SDK run\n\n```bash\npip install rasa-sdk\n```\n\n## Compatibility\n\n`rasa-sdk` package:\n\n| SDK version    | compatible Rasa version           |\n|----------------|-----------------------------------|\n| `1.0.x`        | `>=1.0.x`                         |\n\nold `rasa_core_sdk` package:\n\n| SDK version    | compatible Rasa Core version           |\n|----------------|----------------------------------------|\n| `0.12.x`       | `>=0.12.x`                             |\n| `0.11.x`       | `0.11.x`                               |\n| not compatible | `<=0.10.x`                             |\n\n## Usage\n\nDetailed instructions can be found in the Rasa Documentation about\n[Custom Actions](https://rasa.com/docs/rasa/core/actions).\n\n## Docker\n\n### Usage\n\nIn order to start an action server using implemented custom actions,\nyou can use the available Docker image `rasa/rasa-sdk`.\n\nBefore starting the action server ensure that the folder containing\nyour actions is handled as Python module and therefore has to contain\na file called `__init__.py`\n\nThen start the action server using:\n\n```bash\ndocker run -p 5055:5055 --mount type=bind,source=<ABSOLUTE_PATH_TO_YOUR_ACTIONS>,target=/app/actions \\\n\trasa/rasa-sdk:<version>\n```\n\nThe action server is then available at `http://localhost:5055/webhook`.\n\n### Custom Dependencies\n\nTo add custom dependencies you enhance the given Docker image, e.g.:\n\n```\n# Extend the official Rasa SDK image\nFROM rasa/rasa-sdk:<version>\n\n# Change back to root user to install dependencies\nUSER root\n\n# To install system dependencies\nRUN apt-get update -qq && \\\n    apt-get install -y <NAME_OF_REQUIRED_PACKAGE> && \\\n    apt-get clean && \\\n    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*\n\n# To install packages from PyPI\nRUN pip install --no-cache-dir <A_REQUIRED_PACKAGE_ON_PYPI>\n\n# Switch back to non-root to run code\nUSER 1001\n```\n\n\n## Building from source\n\nRasa SDK uses Poetry for packaging and dependency management. If you want to build it from source,\nyou have to install Poetry first. This is how it can be done:\n\n```\ncurl -sSL https://install.python-poetry.org | python3 -\n```\n\nThere are several other ways to install Poetry. Please, follow\n[the official guide](https://python-poetry.org/docs/#installation) to see all possible options.\n\nTo install dependencies and `rasa-sdk` itself in editable mode execute\n```\nmake install\n```\n\n## Code Style\n\nTo ensure a standardized code style we use the formatter [black](https://github.com/ambv/black).\nIf your code is not formatted properly, GitHub CI will fail to build.\n\nIf you want to automatically format your code on every commit, you can use [pre-commit](https://pre-commit.com/).\nJust install it via `pip install pre-commit` and execute `pre-commit install`.\n\nTo check and reformat files execute\n```\nmake lint\n```\n\n## Steps to release a new version\nReleasing a new version is quite simple, as the packages are build and distributed\nby GitHub Actions.\n\n*Release steps*:\n1. Switch to the branch you want to cut the release from (`main` in case of a\n  major / minor, the current release branch for patch releases).\n2. If this is a minor / major release: Make sure all fixes from currently supported minor versions have been merged from their respective release branches (e.g. 3.3.x) back into main.\n3. Run `make release`\n4. Create a PR against main or the release branch (e.g. `1.2.x`)\n5. Once your PR is merged, tag a new release (this SHOULD always happen on\n  `main` or release branches), e.g. using\n    ```bash\n    git tag 1.2.0 -m "next release"\n    git push origin 1.2.0\n    ```\n    GitHub Actions will build this tag and push a package to\n    [pypi](https://pypi.python.org/pypi/rasa-sdk).\n6. **If this is a minor release**, a new release branch should be created\n  pointing to the same commit as the tag to allow for future patch releases,\n  e.g.\n    ```bash\n    git checkout -b 1.2.x\n    git push origin 1.2.x\n    ```\n\n## License\nLicensed under the Apache License, Version 2.0. Copyright 2021 Rasa\nTechnologies GmbH. [Copy of the license](LICENSE.txt).\n\nA list of the Licenses of the dependencies of the project can be found at\nthe bottom of the\n[Libraries Summary](https://libraries.io/github/RasaHQ/rasa-sdk).\n',
     'author': 'Rasa Technologies GmbH',
     'author_email': 'hi@rasa.com',
     'maintainer': 'Tom Bocklisch',
     'maintainer_email': 'tom@rasa.com',
     'url': 'https://rasa.com',
```

### Comparing `rasa_sdk-3.5.0b1/PKG-INFO` & `rasa_sdk-3.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasa-sdk
-Version: 3.5.0b1
+Version: 3.5.1
 Summary: Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants
 Home-page: https://rasa.com
 License: Apache-2.0
 Keywords: nlp,machine-learning,machine-learning-library,bot,bots,botkit,rasa conversational-agents,conversational-ai,chatbot,chatbot-framework,bot-framework
 Author: Rasa Technologies GmbH
 Author-email: hi@rasa.com
 Maintainer: Tom Bocklisch
@@ -21,14 +21,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: Sanic-Cors (>=2.0.0,<3.0.0)
 Requires-Dist: coloredlogs (>=10,<16)
 Requires-Dist: prompt-toolkit (>=3.0,<3.0.29)
 Requires-Dist: ruamel.yaml (>=0.16.5,<0.18.0)
 Requires-Dist: sanic (>=21.12.0,<22.0.0)
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
+Requires-Dist: websockets (>=10.0,<11.0)
 Project-URL: Documentation, https://rasa.com/docs
 Project-URL: Repository, https://github.com/rasahq/rasa-sdk
 Description-Content-Type: text/markdown
 
 # Rasa Python-SDK
 [![Join the chat on Rasa Community Forum](https://img.shields.io/badge/forum-join%20discussions-brightgreen.svg)](https://forum.rasa.com/?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 [![Build Status](https://github.com/RasaHQ/rasa-sdk/workflows/Continous%20Integration/badge.svg?event=push)](https://github.com/RasaHQ/rasa-sdk/actions/runs/)
```

