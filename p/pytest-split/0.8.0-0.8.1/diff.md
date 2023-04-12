# Comparing `tmp/pytest-split-0.8.0.tar.gz` & `tmp/pytest_split-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-split-0.8.0.tar", max compression
+gzip compressed data, was "pytest_split-0.8.1.tar", max compression
```

## Comparing `pytest-split-0.8.0.tar` & `pytest_split-0.8.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1058 2022-04-22 13:46:51.067825 pytest-split-0.8.0/LICENCE
--rw-r--r--   0        0        0     8242 2022-04-22 13:46:51.067825 pytest-split-0.8.0/README.md
--rw-r--r--   0        0        0     2546 2022-04-22 13:46:51.067825 pytest-split-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-04-22 13:46:51.067825 pytest-split-0.8.0/src/pytest_split/__init__.py
--rw-r--r--   0        0        0     6126 2022-04-22 13:46:51.067825 pytest-split-0.8.0/src/pytest_split/algorithms.py
--rw-r--r--   0        0        0     1011 2022-04-22 13:46:51.067825 pytest-split-0.8.0/src/pytest_split/cli.py
--rw-r--r--   0        0        0     2078 2022-04-22 13:46:51.067825 pytest-split-0.8.0/src/pytest_split/ipynb_compatibility.py
--rw-r--r--   0        0        0     7923 2022-04-22 13:46:51.067825 pytest-split-0.8.0/src/pytest_split/plugin.py
--rw-r--r--   0        0        0        0 2022-04-22 13:46:51.067825 pytest-split-0.8.0/src/pytest_split/py.typed
--rw-r--r--   0        0        0     9381 2022-04-22 13:47:49.067678 pytest-split-0.8.0/setup.py
--rw-r--r--   0        0        0     9387 2022-04-22 13:47:49.068397 pytest-split-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-04-12 06:38:11.348325 pytest_split-0.8.1/LICENCE
+-rw-r--r--   0        0        0     8231 2023-04-12 06:38:11.348325 pytest_split-0.8.1/README.md
+-rw-r--r--   0        0        0     3280 2023-04-12 06:38:11.352325 pytest_split-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 06:38:11.352325 pytest_split-0.8.1/src/pytest_split/__init__.py
+-rw-r--r--   0        0        0     6126 2023-04-12 06:38:11.352325 pytest_split-0.8.1/src/pytest_split/algorithms.py
+-rw-r--r--   0        0        0     1011 2023-04-12 06:38:11.352325 pytest_split-0.8.1/src/pytest_split/cli.py
+-rw-r--r--   0        0        0     2078 2023-04-12 06:38:11.352325 pytest_split-0.8.1/src/pytest_split/ipynb_compatibility.py
+-rw-r--r--   0        0        0     7839 2023-04-12 06:38:11.352325 pytest_split-0.8.1/src/pytest_split/plugin.py
+-rw-r--r--   0        0        0        0 2023-04-12 06:38:11.352325 pytest_split-0.8.1/src/pytest_split/py.typed
+-rw-r--r--   0        0        0     9677 1970-01-01 00:00:00.000000 pytest_split-0.8.1/PKG-INFO
```

### Comparing `pytest-split-0.8.0/LICENCE` & `pytest_split-0.8.1/LICENCE`

 * *Files identical despite different names*

### Comparing `pytest-split-0.8.0/README.md` & `pytest_split-0.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 Find the draft release from the
 [GitHub releases](https://github.com/jerry-git/pytest-split/releases) and publish it. When
  a release is published, it'll trigger [release](https://github.com/jerry-git/pytest-split/blob/master/.github/workflows/release.yml) workflow which creates PyPI
  release and deploys updated documentation.
 
 ### Pre-commit
 
-Pre-commit hooks run all the auto-formatters (e.g. `black`, `isort`), linters (e.g. `mypy`, `flake8`), and other quality
+Pre-commit hooks run all the auto-formatters (e.g. `black`), linters (e.g. `mypy`, `ruff`), and other quality
  checks to make sure the changeset is in good shape before a commit/push happens.
 
 You can install the hooks with (runs for each commit):
 
 ```sh
 pre-commit install
 ```
```

### Comparing `pytest-split-0.8.0/src/pytest_split/algorithms.py` & `pytest_split-0.8.1/src/pytest_split/algorithms.py`

 * *Files identical despite different names*

### Comparing `pytest-split-0.8.0/src/pytest_split/cli.py` & `pytest_split-0.8.1/src/pytest_split/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 
 
 def _list_slowest_tests(durations: "Dict[str, float]", count: int) -> None:
     slowest_tests = tuple(
         sorted(durations.items(), key=lambda item: item[1], reverse=True)
     )[:count]
     for test, duration in slowest_tests:
-        print(f"{duration:.2f} {test}")  # noqa: T001
+        print(f"{duration:.2f} {test}")  # noqa: T201
```

### Comparing `pytest-split-0.8.0/src/pytest_split/ipynb_compatibility.py` & `pytest_split-0.8.1/src/pytest_split/ipynb_compatibility.py`

 * *Files identical despite different names*

### Comparing `pytest-split-0.8.0/src/pytest_split/plugin.py` & `pytest_split-0.8.1/src/pytest_split/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         help=(
             "Removes the test duration info for tests which are not present "
             "while running the suite with '--store-durations'."
         ),
     )
 
 
-@pytest.mark.tryfirst
+@pytest.hookimpl(tryfirst=True)
 def pytest_cmdline_main(config: "Config") -> "Optional[Union[int, ExitCode]]":
     """
     Validate options.
     """
     group = config.getoption("group")
     splits = config.getoption("splits")
 
@@ -131,17 +131,15 @@
         except FileNotFoundError:
             self.cached_durations = {}
 
         # This code provides backwards compatibility after we switched
         # from saving durations in a list-of-lists to a dict format
         # Remove this when bumping to v1
         if isinstance(self.cached_durations, list):
-            self.cached_durations = {
-                test_name: duration for test_name, duration in self.cached_durations
-            }
+            self.cached_durations = dict(self.cached_durations)
 
 
 class PytestSplitPlugin(Base):
     def __init__(self, config: "Config"):
         super().__init__(config)
 
         if not self.cached_durations:
@@ -178,15 +176,14 @@
             )
         )
         self.writer.line(
             self.writer.markup(
                 f"[pytest-split] Running group {group_idx}/{splits} (estimated duration: {group.duration:.2f}s)\n"
             )
         )
-        return None
 
 
 class PytestSplitCachePlugin(Base):
     """
     The cache plugin writes durations to our durations file.
     """
 
@@ -197,15 +194,14 @@
         """
         terminal_reporter = self.config.pluginmanager.get_plugin("terminalreporter")
         test_durations: "Dict[str, float]" = {}
 
         for test_reports in terminal_reporter.stats.values():
             for test_report in test_reports:
                 if isinstance(test_report, TestReport):
-
                     # These ifs be removed after this is solved: # https://github.com/spulec/freezegun/issues/286
                     if test_report.duration < 0:
                         continue  # pragma: no cover
                     if (
                         test_report.when in ("teardown", "setup")
                         and test_report.duration
                         > STORE_DURATIONS_SETUP_AND_TEARDOWN_THRESHOLD
```

### Comparing `pytest-split-0.8.0/setup.py` & `pytest_split-0.8.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,193 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pytest-split
+Version: 0.8.1
+Summary: Pytest plugin which splits the test suite to equally sized sub suites based on test execution time.
+Home-page: https://jerry-git.github.io/pytest-split
+License: MIT
+Keywords: pytest,plugin,split,tests
+Author: Jerry Pussinen
+Author-email: jerry.pussinen@gmail.com
+Requires-Python: >=3.7.1,<4.0
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
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: pytest (>=5,<8)
+Project-URL: Documentation, https://jerry-git.github.io/pytest-split
+Project-URL: Repository, https://github.com/jerry-git/pytest-split
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# pytest-split
 
-packages = \
-['pytest_split']
+[![PyPI](https://img.shields.io/pypi/v/pytest-split?style=flat-square)](https://pypi.python.org/pypi/pytest-split/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-split?style=flat-square)](https://pypi.python.org/pypi/pytest-split/)
+[![PyPI - License](https://img.shields.io/pypi/l/pytest-split?style=flat-square)](https://pypi.python.org/pypi/pytest-split/)
+[![Coookiecutter - Wolt](https://img.shields.io/badge/cookiecutter-Wolt-00c2e8?style=flat-square&logo=cookiecutter&logoColor=D4AA00&link=https://github.com/woltapp/wolt-python-package-cookiecutter)](https://github.com/woltapp/wolt-python-package-cookiecutter)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pytest>=5,<8']
-
-entry_points = \
-{'console_scripts': ['slowest-tests = pytest_split.cli:list_slowest_tests'],
- 'pytest11': ['pytest-split = pytest_split.plugin']}
-
-setup_kwargs = {
-    'name': 'pytest-split',
-    'version': '0.8.0',
-    'description': 'Pytest plugin which splits the test suite to equally sized sub suites based on test execution time.',
-    'long_description': '# pytest-split\n\n[![PyPI](https://img.shields.io/pypi/v/pytest-split?style=flat-square)](https://pypi.python.org/pypi/pytest-split/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-split?style=flat-square)](https://pypi.python.org/pypi/pytest-split/)\n[![PyPI - License](https://img.shields.io/pypi/l/pytest-split?style=flat-square)](https://pypi.python.org/pypi/pytest-split/)\n[![Coookiecutter - Wolt](https://img.shields.io/badge/cookiecutter-Wolt-00c2e8?style=flat-square&logo=cookiecutter&logoColor=D4AA00&link=https://github.com/woltapp/wolt-python-package-cookiecutter)](https://github.com/woltapp/wolt-python-package-cookiecutter)\n\n\n---\n\n**Documentation**: [https://jerry-git.github.io/pytest-split](https://jerry-git.github.io/pytest-split)\n\n**Source Code**: [https://github.com/jerry-git/pytest-split](https://github.com/jerry-git/pytest-split)\n\n**PyPI**: [https://pypi.org/project/pytest-split/](https://pypi.org/project/pytest-split/)\n\n---\n\nPytest plugin which splits the test suite to equally sized "sub suites" based on test execution time.\n\n## Motivation\n* Splitting the test suite is a prerequisite for parallelization (who does not want faster CI builds?). It\'s valuable to have sub suites which execution time is around the same.\n* [`pytest-test-groups`](https://pypi.org/project/pytest-test-groups/) is great but it does not take into account the execution time of sub suites which can lead to notably unbalanced execution times between the sub suites.\n* [`pytest-xdist`](https://pypi.org/project/pytest-xdist/) is great but it\'s not suitable for all use cases.\nFor example, some test suites may be fragile considering the order in which the tests are executed.\nThis is of course a fundamental problem in the suite itself but sometimes it\'s not worth the effort to refactor, especially if the suite is huge (and smells a bit like legacy).\nAdditionally, `pytest-split` may be a better fit in some use cases considering distributed execution.\n\n## Installation\n```sh\npip install pytest-split\n```\n\n## Usage\nFirst we have to store test durations from a complete test suite run.\nThis produces .test_durations file which should be stored in the repo in order to have it available during future test runs.\nThe file path is configurable via `--durations-path` CLI option.\n```sh\npytest --store-durations\n```\n\nThen we can have as many splits as we want:\n```sh\npytest --splits 3 --group 1\npytest --splits 3 --group 2\npytest --splits 3 --group 3\n```\n\nTime goes by, new tests are added and old ones are removed/renamed during development. No worries!\n`pytest-split` assumes average test execution time (calculated based on the stored information) for every test which does not have duration information stored.\nThus, there\'s no need to store durations after changing the test suite.\nHowever, when there are major changes in the suite compared to what\'s stored in .test_durations, it\'s recommended to update the duration information with `--store-durations` to ensure that the splitting is in balance.\n\nThe splitting algorithm can be controlled with the `--splitting-algorithm` CLI option and defaults to `duration_based_chunks`. For more information about the different algorithms and their tradeoffs, please see the section below.\n\n### CLI commands\n#### slowest-tests\nLists the slowest tests based on the information stored in the test durations file. See `slowest-tests --help` for more\n information.\n\n## Interactions with other pytest plugins\n* [`pytest-random-order`](https://github.com/jbasko/pytest-random-order) and [`pytest-randomly`](https://github.com/pytest-dev/pytest-randomly):\n   ⚠️ `pytest-split` running with the `duration_based_chunks` algorithm is **incompatible** with test-order-randomization plugins.\n  Test selection in the groups happens after randomization, potentially causing some tests to be selected in several groups and others not at all.\n  Instead, a global random seed needs to be computed before running the tests (for example using `$RANDOM` from the shell) and that single seed then needs to be used for all groups by setting the `--random-order-seed` option.\n\n* [`nbval`](https://github.com/computationalmodelling/nbval): `pytest-split` could, in principle, break up a single IPython Notebook into different test groups. This most likely causes broken up pieces to fail (for the very least, package `import`s are usually done at Cell 1, and so, any broken up piece that doesn\'t contain Cell 1 will certainly fail). To avoid this, after splitting step is done, test groups are reorganized based on a simple algorithm illustrated in the following cartoon:\n\n![image](https://user-images.githubusercontent.com/14086031/145830494-07afcaf0-5a0f-4817-b9ee-f84a459652a8.png)\n\nwhere the letters (A to E) refer to individual IPython Notebooks, and the numbers refer to the corresponding cell number.\n\n## Splitting algorithms\nThe plugin supports multiple algorithms to split tests into groups.\nEach algorithm makes different tradeoffs, but generally `least_duration` should give more balanced groups.\n\n| Algorithm      | Maintains Absolute Order | Maintains Relative Order | Split Quality | Works with random ordering |\n|----------------|--------------------------|--------------------------|---------------|----------------------------|\n| duration_based_chunks | ✅                | ✅                       | Good          | ❌                         |\n| least_duration | ❌                       | ✅                       | Better        | ✅                         |\n\nExplanation of the terms in the table:\n* Absolute Order: whether each group contains all tests between first and last element in the same order as the original list of tests\n* Relative Order: whether each test in each group has the same relative order to its neighbours in the group as in the original list of tests\n* Works with random ordering: whether the algorithm works with test-shuffling tools such as [`pytest-randomly`](https://github.com/pytest-dev/pytest-randomly)\n\nThe `duration_based_chunks` algorithm aims to find optimal boundaries for the list of tests and every test group contains all tests between the start and end boundary.\nThe `least_duration` algorithm walks the list of tests and assigns each test to the group with the smallest current duration.\n\n\n[**Demo with GitHub Actions**](https://github.com/jerry-git/pytest-split-gh-actions-demo)\n\n\n## Development\n\n* Clone this repository\n* Requirements:\n  * [Poetry](https://python-poetry.org/)\n  * Python 3.7+\n* Create a virtual environment and install the dependencies\n\n```sh\npoetry install\n```\n\n* Activate the virtual environment\n\n```sh\npoetry shell\n```\n\n### Testing\n\n```sh\npytest\n```\n\n### Documentation\n\nThe documentation is automatically generated from the content of the [docs directory](./docs) and from the docstrings\n of the public signatures of the source code. The documentation is updated and published as a [Github project page\n ](https://pages.github.com/) automatically as part each release.\n\n### Releasing\n\nTrigger the [Draft release workflow](https://github.com/jerry-git/pytest-split/actions/workflows/draft_release.yml)\n(press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.\n\nFind the draft release from the\n[GitHub releases](https://github.com/jerry-git/pytest-split/releases) and publish it. When\n a release is published, it\'ll trigger [release](https://github.com/jerry-git/pytest-split/blob/master/.github/workflows/release.yml) workflow which creates PyPI\n release and deploys updated documentation.\n\n### Pre-commit\n\nPre-commit hooks run all the auto-formatters (e.g. `black`, `isort`), linters (e.g. `mypy`, `flake8`), and other quality\n checks to make sure the changeset is in good shape before a commit/push happens.\n\nYou can install the hooks with (runs for each commit):\n\n```sh\npre-commit install\n```\n\nOr if you want them to run only for each push:\n\n```sh\npre-commit install -t pre-push\n```\n\nOr if you want e.g. want to run all checks manually for all files:\n\n```sh\npre-commit run --all-files\n```\n\n---\n\nThis project was generated using the [wolt-python-package-cookiecutter](https://github.com/woltapp/wolt-python-package-cookiecutter) template.\n',
-    'author': 'Jerry Pussinen',
-    'author_email': 'jerry.pussinen@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://jerry-git.github.io/pytest-split',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0',
-}
 
+---
+
+**Documentation**: [https://jerry-git.github.io/pytest-split](https://jerry-git.github.io/pytest-split)
+
+**Source Code**: [https://github.com/jerry-git/pytest-split](https://github.com/jerry-git/pytest-split)
+
+**PyPI**: [https://pypi.org/project/pytest-split/](https://pypi.org/project/pytest-split/)
+
+---
+
+Pytest plugin which splits the test suite to equally sized "sub suites" based on test execution time.
+
+## Motivation
+* Splitting the test suite is a prerequisite for parallelization (who does not want faster CI builds?). It's valuable to have sub suites which execution time is around the same.
+* [`pytest-test-groups`](https://pypi.org/project/pytest-test-groups/) is great but it does not take into account the execution time of sub suites which can lead to notably unbalanced execution times between the sub suites.
+* [`pytest-xdist`](https://pypi.org/project/pytest-xdist/) is great but it's not suitable for all use cases.
+For example, some test suites may be fragile considering the order in which the tests are executed.
+This is of course a fundamental problem in the suite itself but sometimes it's not worth the effort to refactor, especially if the suite is huge (and smells a bit like legacy).
+Additionally, `pytest-split` may be a better fit in some use cases considering distributed execution.
+
+## Installation
+```sh
+pip install pytest-split
+```
+
+## Usage
+First we have to store test durations from a complete test suite run.
+This produces .test_durations file which should be stored in the repo in order to have it available during future test runs.
+The file path is configurable via `--durations-path` CLI option.
+```sh
+pytest --store-durations
+```
+
+Then we can have as many splits as we want:
+```sh
+pytest --splits 3 --group 1
+pytest --splits 3 --group 2
+pytest --splits 3 --group 3
+```
+
+Time goes by, new tests are added and old ones are removed/renamed during development. No worries!
+`pytest-split` assumes average test execution time (calculated based on the stored information) for every test which does not have duration information stored.
+Thus, there's no need to store durations after changing the test suite.
+However, when there are major changes in the suite compared to what's stored in .test_durations, it's recommended to update the duration information with `--store-durations` to ensure that the splitting is in balance.
+
+The splitting algorithm can be controlled with the `--splitting-algorithm` CLI option and defaults to `duration_based_chunks`. For more information about the different algorithms and their tradeoffs, please see the section below.
+
+### CLI commands
+#### slowest-tests
+Lists the slowest tests based on the information stored in the test durations file. See `slowest-tests --help` for more
+ information.
+
+## Interactions with other pytest plugins
+* [`pytest-random-order`](https://github.com/jbasko/pytest-random-order) and [`pytest-randomly`](https://github.com/pytest-dev/pytest-randomly):
+   ⚠️ `pytest-split` running with the `duration_based_chunks` algorithm is **incompatible** with test-order-randomization plugins.
+  Test selection in the groups happens after randomization, potentially causing some tests to be selected in several groups and others not at all.
+  Instead, a global random seed needs to be computed before running the tests (for example using `$RANDOM` from the shell) and that single seed then needs to be used for all groups by setting the `--random-order-seed` option.
+
+* [`nbval`](https://github.com/computationalmodelling/nbval): `pytest-split` could, in principle, break up a single IPython Notebook into different test groups. This most likely causes broken up pieces to fail (for the very least, package `import`s are usually done at Cell 1, and so, any broken up piece that doesn't contain Cell 1 will certainly fail). To avoid this, after splitting step is done, test groups are reorganized based on a simple algorithm illustrated in the following cartoon:
+
+![image](https://user-images.githubusercontent.com/14086031/145830494-07afcaf0-5a0f-4817-b9ee-f84a459652a8.png)
+
+where the letters (A to E) refer to individual IPython Notebooks, and the numbers refer to the corresponding cell number.
+
+## Splitting algorithms
+The plugin supports multiple algorithms to split tests into groups.
+Each algorithm makes different tradeoffs, but generally `least_duration` should give more balanced groups.
+
+| Algorithm      | Maintains Absolute Order | Maintains Relative Order | Split Quality | Works with random ordering |
+|----------------|--------------------------|--------------------------|---------------|----------------------------|
+| duration_based_chunks | ✅                | ✅                       | Good          | ❌                         |
+| least_duration | ❌                       | ✅                       | Better        | ✅                         |
+
+Explanation of the terms in the table:
+* Absolute Order: whether each group contains all tests between first and last element in the same order as the original list of tests
+* Relative Order: whether each test in each group has the same relative order to its neighbours in the group as in the original list of tests
+* Works with random ordering: whether the algorithm works with test-shuffling tools such as [`pytest-randomly`](https://github.com/pytest-dev/pytest-randomly)
+
+The `duration_based_chunks` algorithm aims to find optimal boundaries for the list of tests and every test group contains all tests between the start and end boundary.
+The `least_duration` algorithm walks the list of tests and assigns each test to the group with the smallest current duration.
+
+
+[**Demo with GitHub Actions**](https://github.com/jerry-git/pytest-split-gh-actions-demo)
+
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
+Trigger the [Draft release workflow](https://github.com/jerry-git/pytest-split/actions/workflows/draft_release.yml)
+(press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.
+
+Find the draft release from the
+[GitHub releases](https://github.com/jerry-git/pytest-split/releases) and publish it. When
+ a release is published, it'll trigger [release](https://github.com/jerry-git/pytest-split/blob/master/.github/workflows/release.yml) workflow which creates PyPI
+ release and deploys updated documentation.
+
+### Pre-commit
+
+Pre-commit hooks run all the auto-formatters (e.g. `black`), linters (e.g. `mypy`, `ruff`), and other quality
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

