# Comparing `tmp/mlx.jira_juggler-3.2.3.tar.gz` & `tmp/mlx.jira_juggler-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mlx.jira_juggler-3.2.3.tar", last modified: Mon Feb 13 17:34:54 2023, max compression
+gzip compressed data, was "dist/mlx.jira_juggler-3.2.4.tar", last modified: Wed Apr 12 21:02:42 2023, max compression
```

## Comparing `mlx.jira_juggler-3.2.3.tar` & `mlx.jira_juggler-3.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-02-13 17:34:43.000000 mlx.jira_juggler-3.2.3/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-02-13 17:34:43.000000 mlx.jira_juggler-3.2.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-02-13 17:34:43.000000 mlx.jira_juggler-3.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-02-13 17:34:43.000000 mlx.jira_juggler-3.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-13 17:34:43.000000 mlx.jira_juggler-3.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-13 17:34:43.000000 mlx.jira_juggler-3.2.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-02-13 17:34:43.000000 mlx.jira_juggler-3.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-13 17:34:43.000000 mlx.jira_juggler-3.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/src/mlx/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-13 17:34:43.000000 mlx.jira_juggler-3.2.3/src/mlx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32406 2023-02-13 17:34:43.000000 mlx.jira_juggler-3.2.3/src/mlx/jira_juggler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/src/mlx.jira_juggler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/src/mlx.jira_juggler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/src/mlx.jira_juggler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/src/mlx.jira_juggler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/src/mlx.jira_juggler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/src/mlx.jira_juggler.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/src/mlx.jira_juggler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/src/mlx.jira_juggler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/src/mlx.jira_juggler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 17:34:54.000000 mlx.jira_juggler-3.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    32290 2023-02-13 17:34:43.000000 mlx.jira_juggler-3.2.3/tests/test_jira_juggler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-02-13 17:34:43.000000 mlx.jira_juggler-3.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-12 21:02:30.000000 mlx.jira_juggler-3.2.4/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-12 21:02:30.000000 mlx.jira_juggler-3.2.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-12 21:02:30.000000 mlx.jira_juggler-3.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-04-12 21:02:30.000000 mlx.jira_juggler-3.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-12 21:02:30.000000 mlx.jira_juggler-3.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 21:02:30.000000 mlx.jira_juggler-3.2.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-12 21:02:30.000000 mlx.jira_juggler-3.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-12 21:02:30.000000 mlx.jira_juggler-3.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/src/mlx/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 21:02:30.000000 mlx.jira_juggler-3.2.4/src/mlx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-04-12 21:02:30.000000 mlx.jira_juggler-3.2.4/src/mlx/jira_juggler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/src/mlx.jira_juggler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/src/mlx.jira_juggler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/src/mlx.jira_juggler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/src/mlx.jira_juggler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/src/mlx.jira_juggler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/src/mlx.jira_juggler.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/src/mlx.jira_juggler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/src/mlx.jira_juggler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/src/mlx.jira_juggler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:02:42.000000 mlx.jira_juggler-3.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    32290 2023-04-12 21:02:30.000000 mlx.jira_juggler-3.2.4/tests/test_jira_juggler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-12 21:02:30.000000 mlx.jira_juggler-3.2.4/tox.ini
```

### Comparing `mlx.jira_juggler-3.2.3/.github/workflows/python-package.yml` & `mlx.jira_juggler-3.2.4/.github/workflows/python-package.yml`

 * *Files 19% similar despite different names*

```diff
@@ -7,41 +7,47 @@
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox tox-gh-actions
     - name: Run test
       run: tox -e py
-    - name: Codecov
+    - name: Upload coverage to Codecov
       if: matrix.python-version == 3.9
-      run: tox -e codecov
+      uses: codecov/codecov-action@v3
+      with:
+        token: ${{ secrets.CODECOV_TOKEN }}
+        files: ./coverage.xml
+        fail_ci_if_error: true
+        flags: unittests
+        verbose: true
     - name: Static checks
       if: matrix.python-version == 3.9
       run: tox -e check
 
   deploy:
 
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     needs: test
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.7'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
     - name: Build and publish
```

### Comparing `mlx.jira_juggler-3.2.3/.gitignore` & `mlx.jira_juggler-3.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mlx.jira_juggler-3.2.3/LICENSE` & `mlx.jira_juggler-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx.jira_juggler-3.2.3/PKG-INFO` & `mlx.jira_juggler-3.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx.jira_juggler
-Version: 3.2.3
+Version: 3.2.4
 Summary: A python script for extracting data from Jira, and converting to task-juggler (tj3) output
 Home-page: https://github.com/melexis/jira-juggler
 Author: Stein Heselmans
 Author-email: teh@melexis.com
 License: Apache License, Version 2.0
 Description: .. image:: https://img.shields.io/hexpm/l/plug.svg
             :target: http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `mlx.jira_juggler-3.2.3/README.rst` & `mlx.jira_juggler-3.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `mlx.jira_juggler-3.2.3/setup.py` & `mlx.jira_juggler-3.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `mlx.jira_juggler-3.2.3/src/mlx/jira_juggler.py` & `mlx.jira_juggler-3.2.4/src/mlx/jira_juggler.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
             jira_issue (jira.resources.Issue): The Jira issue to load from
         """
         self.value = self.DEFAULT_VALUE
         if hasattr(jira_issue.fields, 'issuelinks'):
             for link in jira_issue.fields.issuelinks:
                 if hasattr(link, 'inwardIssue') and link.type.name == 'Blocker':
                     self.append_value(to_identifier(link.inwardIssue.key))
-                if hasattr(link, 'outwardIssue') and link.type.name == 'Dependency':
+                if hasattr(link, 'outwardIssue') and link.type.name in ('Dependency', 'Dependent'):
                     self.append_value(to_identifier(link.outwardIssue.key))
 
     def validate(self, task, tasks):
         """Validates (and corrects) the current task property
 
         Args:
             task (JugglerTask): Task to which the property belongs
```

### Comparing `mlx.jira_juggler-3.2.3/src/mlx.jira_juggler.egg-info/PKG-INFO` & `mlx.jira_juggler-3.2.4/src/mlx.jira_juggler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx.jira-juggler
-Version: 3.2.3
+Version: 3.2.4
 Summary: A python script for extracting data from Jira, and converting to task-juggler (tj3) output
 Home-page: https://github.com/melexis/jira-juggler
 Author: Stein Heselmans
 Author-email: teh@melexis.com
 License: Apache License, Version 2.0
 Description: .. image:: https://img.shields.io/hexpm/l/plug.svg
             :target: http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `mlx.jira_juggler-3.2.3/src/mlx.jira_juggler.egg-info/SOURCES.txt` & `mlx.jira_juggler-3.2.4/src/mlx.jira_juggler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx.jira_juggler-3.2.3/tests/test_jira_juggler.py` & `mlx.jira_juggler-3.2.4/tests/test_jira_juggler.py`

 * *Files identical despite different names*

### Comparing `mlx.jira_juggler-3.2.3/tox.ini` & `mlx.jira_juggler-3.2.4/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -17,29 +17,29 @@
     py: python3
     pypy: {env:TOXPYTHON:pypy}
     py37: {env:TOXPYTHON:python3.7}
     py38: {env:TOXPYTHON:python3.8}
     py39: {env:TOXPYTHON:python3.9}
     py310: {env:TOXPYTHON:python3.10}
     py311: {env:TOXPYTHON:python3.11}
-    {clean,check,report,coveralls,codecov}: python3
+    {clean,check,report,coveralls}: python3
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
 passenv =
     *
 usedevelop = false
 deps =
     pytest
     pytest-cov
     mock
     pip>=20.3.4
     parameterized
 commands =
-    {posargs:py.test --cov --cov-report=term-missing -vv tests}
+    pytest --cov-report=term-missing --cov-report=xml -vv --cov tests
 
 [testenv:check]
 deps =
     docutils
     check-manifest
     flake8
     readme-renderer
@@ -54,23 +54,14 @@
 [testenv:coveralls]
 deps =
     coveralls
 skip_install = true
 commands =
     coveralls []
 
-[testenv:codecov]
-deps =
-    codecov
-skip_install = true
-commands =
-    coverage xml --ignore-errors
-    codecov []
-
-
 [testenv:report]
 deps = coverage
 skip_install = true
 commands =
     coverage combine --append
     coverage report
     coverage html
```

