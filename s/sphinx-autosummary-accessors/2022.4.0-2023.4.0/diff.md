# Comparing `tmp/sphinx-autosummary-accessors-2022.4.0.tar.gz` & `tmp/sphinx-autosummary-accessors-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-autosummary-accessors-2022.4.0.tar", last modified: Mon Apr  4 18:12:45 2022, max compression
+gzip compressed data, was "sphinx-autosummary-accessors-2023.4.0.tar", last modified: Wed Apr 12 10:22:33 2023, max compression
```

## Comparing `sphinx-autosummary-accessors-2022.4.0.tar` & `sphinx-autosummary-accessors-2023.4.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:12:45.677558 sphinx-autosummary-accessors-2022.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:12:45.669557 sphinx-autosummary-accessors-2022.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-04-04 18:12:26.000000 sphinx-autosummary-accessors-2022.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:12:45.673557 sphinx-autosummary-accessors-2022.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-04-04 18:12:26.000000 sphinx-autosummary-accessors-2022.4.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-04-04 18:12:26.000000 sphinx-autosummary-accessors-2022.4.0/.github/workflows/format-logs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5284 2022-04-04 18:12:26.000000 sphinx-autosummary-accessors-2022.4.0/.github/workflows/nightly.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-04-04 18:12:26.000000 sphinx-autosummary-accessors-2022.4.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-04-04 18:12:26.000000 sphinx-autosummary-accessors-2022.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-04-04 18:12:26.000000 sphinx-autosummary-accessors-2022.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-04-04 18:12:26.000000 sphinx-autosummary-accessors-2022.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2499 2022-04-04 18:12:45.677558 sphinx-autosummary-accessors-2022.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:12:45.673557 sphinx-autosummary-accessors-2022.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:12:45.673557 sphinx-autosummary-accessors-2022.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/docs/_templates/custom-template.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3374 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/docs/example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/docs/templates.rst
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/docs/whats-new.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:12:45.673557 sphinx-autosummary-accessors-2022.4.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/licenses/PANDAS_LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-04-04 18:12:45.677558 sphinx-autosummary-accessors-2022.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:12:45.673557 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/autosummary.py
--rw-r--r--   0 runner    (1001) docker     (121)     3792 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/documenters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:12:45.669557 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:12:45.677558 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/templates/autosummary/accessor.rst
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/templates/autosummary/accessor_attribute.rst
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/templates/autosummary/accessor_callable.rst
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/templates/autosummary/accessor_method.rst
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-04-04 18:12:27.000000 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:12:45.673557 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2499 2022-04-04 18:12:44.000000 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-04-04 18:12:45.000000 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-04 18:12:45.000000 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-04-04 18:12:45.000000 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-04-04 18:12:45.000000 sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:22:33.209442 sphinx-autosummary-accessors-2023.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:22:33.205442 sphinx-autosummary-accessors-2023.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:22:33.205442 sphinx-autosummary-accessors-2023.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/.github/workflows/format-logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/.github/workflows/nightly.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-12 10:22:33.205442 sphinx-autosummary-accessors-2023.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:22:33.205442 sphinx-autosummary-accessors-2023.4.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:22:33.205442 sphinx-autosummary-accessors-2023.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:22:33.205442 sphinx-autosummary-accessors-2023.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/docs/_templates/custom-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/docs/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/docs/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/docs/whats-new.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:22:33.205442 sphinx-autosummary-accessors-2023.4.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/licenses/PANDAS_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:22:33.209442 sphinx-autosummary-accessors-2023.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:22:33.205442 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/autosummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/documenters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:22:33.201442 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:22:33.205442 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/templates/autosummary/accessor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/templates/autosummary/accessor_callable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/templates/autosummary/accessor_method.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-12 10:22:19.000000 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:22:33.205442 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-12 10:22:33.000000 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-12 10:22:33.000000 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:22:33.000000 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 10:22:33.000000 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-12 10:22:33.000000 sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors.egg-info/top_level.txt
```

### Comparing `sphinx-autosummary-accessors-2022.4.0/.github/workflows/ci.yaml` & `sphinx-autosummary-accessors-2023.4.0/.github/workflows/ci.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -10,31 +10,29 @@
   linux:
     name: 'sphinx v${{matrix.sphinx-version}} py${{matrix.python-version}}'
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
-        sphinx-version: ['3.3', '3.4', '3.5', '4.0', '4.1', '4.2', '4.3', '4.4', '4.5']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
+        sphinx-version: ['3.5', '4.5', '5.0', '5.1', '5.2', '5.3', '6.0', '6.1']
         exclude:
           # sphinx versions incompatible with python 3.10
           - python-version: "3.10"
             sphinx-version: "3.5"
-          - python-version: "3.10"
-            sphinx-version: "4.0"
-          - python-version: "3.10"
-            sphinx-version: "4.1"
+          - python-version: "3.11"
+            sphinx-version: "3.5"
 
     steps:
       - name: checkout the repository
         uses: actions/checkout@v3
 
       - name: setup python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: cache pip
         uses: actions/cache@v3
         with:
           path: ~/.cache/pip
@@ -45,19 +43,19 @@
       - name: upgrade pip
         run: python -m pip install --upgrade pip
 
       - name: install sphinx
         run: |
           python -m pip install "sphinx==${{matrix.sphinx-version}}"
           if [[ "${{matrix.sphinx-version}}" < "4.0" ]]; then
-              python -m pip install "jinja2<3.1"
+              python -m pip install "jinja2<3.1" "docutils<0.18"
           fi
 
       - name: install other dependencies
-        run: python -m pip install -r docs/requirements.txt
+        run: python -m pip install -r ci/requirements.txt
 
       - name: install the extension
         run: python -m pip install .
 
       - name: show versions
         run: python -m pip list
```

### Comparing `sphinx-autosummary-accessors-2022.4.0/.github/workflows/nightly.yaml` & `sphinx-autosummary-accessors-2023.4.0/.github/workflows/nightly.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       && (github.event_name == 'push' || github.event_name == 'pull_request')
     outputs:
       triggered: ${{ steps.detect-trigger.outputs.trigger-found }}
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 2
-      - uses: xarray-contrib/ci-trigger@v1.1
+      - uses: xarray-contrib/ci-trigger@v1.2
         id: detect-trigger
         with:
           keyword: "[test-upstream]"
 
   upstream-dev:
     name: upstream-dev
     runs-on: ubuntu-latest
@@ -37,40 +37,40 @@
         github.event_name == 'schedule'
         || needs.detect-ci-trigger.outputs.triggered == 'true'
       )
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.9]
+        python-version: ["3.11"]
 
     outputs:
       artifacts_availability: ${{ steps.status.outputs.ARTIFACTS_AVAILABLE }}
 
     steps:
       - name: checkout the repository
         uses: actions/checkout@v3
         with:
           # need to fetch all tags to get a correct version
           fetch-depth: 0  # fetch all branches and tags
 
       - name: setup python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: upgrade pip
         run: python -m pip install --upgrade pip
 
       - name: install sphinx
         run: |
           python -m pip install "git+https://github.com/sphinx-doc/sphinx"
 
       - name: install other dependencies
-        run: python -m pip install -r docs/requirements.txt
+        run: python -m pip install -r ci/requirements.txt
 
       - name: install the extension
         run: python -m pip install .
 
       - name: show versions
         run: python -m pip list
 
@@ -96,18 +96,18 @@
       && github.event_name == 'schedule'
       && github.repository == 'xarray-contrib/sphinx-autosummary-accessors'
       && needs.upstream-dev.outputs.artifacts_availability == 'true'
     steps:
     - name: checkout the repository
       uses: actions/checkout@v3
     - name: setup python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: "3.x"
-    - uses: actions/download-artifact@v2
+    - uses: actions/download-artifact@v3
       with:
         path: /tmp/workspace/logs
     - name: Move all log files into a single directory
       run: |
         rsync -a /tmp/workspace/logs/output-*/ ./logs
         ls -R ./logs
     - name: Parse logs
```

### Comparing `sphinx-autosummary-accessors-2022.4.0/.github/workflows/publish.yaml` & `sphinx-autosummary-accessors-2023.4.0/.github/workflows/publish.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 jobs:
   publish:
     name: Publish to PyPI
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: '3.x'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip build twine
       - name: Build
         run: |
           python -m build --sdist --wheel --outdir dist/ .
       - name: Check the built archives
         run: |
           twine check dist/*
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@717ba43cfbb0387f6ce311b169a825772f54d295
+        uses: pypa/gh-action-pypi-publish@0bf742be3ebe032c25dd15117957dc15d0cfc38d
         with:
           user: __token__
           password: ${{ secrets.pypi_token }}
           repository_url: https://upload.pypi.org/legacy/
           verify_metadata: true
```

### Comparing `sphinx-autosummary-accessors-2022.4.0/.gitignore` & `sphinx-autosummary-accessors-2023.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx-autosummary-accessors-2022.4.0/.pre-commit-config.yaml` & `sphinx-autosummary-accessors-2023.4.0/.pre-commit-config.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ci:
   autoupdate_schedule: "weekly"
 
 # https://pre-commit.com/
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
       - id: end-of-file-fixer
       - id: trailing-whitespace
       - id: requirements-txt-fixer
       - id: check-merge-conflict
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+  - repo: https://github.com/PyCQA/flake8
+    rev: 6.0.0
     hooks:
       - id: flake8
```

### Comparing `sphinx-autosummary-accessors-2022.4.0/LICENSE` & `sphinx-autosummary-accessors-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-autosummary-accessors-2022.4.0/PKG-INFO` & `sphinx-autosummary-accessors-2023.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: sphinx-autosummary-accessors
-Version: 2022.4.0
+Version: 2023.4.0
 Summary: sphinx autosummary extension to properly format pandas or xarray accessors
-Home-page: https://github.com/xarray-contrib/sphinx-autosummary-accessors
-Author: Justus Magin
-Author-email: keewis@posteo.de
+Author-email: Justus Magin <keewis@posteo.de>
 License: MIT
+Project-URL: Home, https://github.com/xarray-contrib/sphinx-autosummary-accessors
 Project-URL: Documentation, https://sphinx-autosummary-accessors.readthedocs.io/en/stable
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 sphinx-autosummary-accessors
 ============================
 
 .. image:: https://github.com/xarray-contrib/sphinx-autosummary-accessors/workflows/CI/badge.svg?branch=master
@@ -64,9 +62,7 @@
 =============
 For more information and examples, see the `documentation`_.
 
 .. _pandas: https://github.com/pandas-dev/pandas
 .. _xarray: https://github.com/pydata/xarray
 .. _sphinx: https://github.com/sphinx-doc/sphinx
 .. _documentation: https://sphinx-autosummary-accessors.readthedocs.io
-
-
```

### Comparing `sphinx-autosummary-accessors-2022.4.0/README.rst` & `sphinx-autosummary-accessors-2023.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx-autosummary-accessors-2022.4.0/docs/_templates/custom-template.rst` & `sphinx-autosummary-accessors-2023.4.0/docs/_templates/custom-template.rst`

 * *Files identical despite different names*

### Comparing `sphinx-autosummary-accessors-2022.4.0/docs/conf.py` & `sphinx-autosummary-accessors-2023.4.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,16 +89,16 @@
 
 # autosummary
 autosummary_generate = True
 
 # extlinks
 base_url = "https://github.com/xarray-contrib/sphinx-autosummary-accessors"
 extlinks = {
-    "issue": (f"{base_url}/issues/%s", "GH"),
-    "pull": (f"{base_url}/pull/%s", "PR"),
+    "issue": (f"{base_url}/issues/%s", "GH %s"),
+    "pull": (f"{base_url}/pull/%s", "PR %s"),
 }
 
 # napoleon
 napoleon_use_param = False
 napoleon_use_rtype = True
```

### Comparing `sphinx-autosummary-accessors-2022.4.0/docs/example.py` & `sphinx-autosummary-accessors-2023.4.0/docs/example.py`

 * *Files identical despite different names*

### Comparing `sphinx-autosummary-accessors-2022.4.0/docs/examples.rst` & `sphinx-autosummary-accessors-2023.4.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `sphinx-autosummary-accessors-2022.4.0/docs/index.rst` & `sphinx-autosummary-accessors-2023.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-autosummary-accessors-2022.4.0/docs/templates.rst` & `sphinx-autosummary-accessors-2023.4.0/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `sphinx-autosummary-accessors-2022.4.0/docs/usage.rst` & `sphinx-autosummary-accessors-2023.4.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `sphinx-autosummary-accessors-2022.4.0/docs/whats-new.rst` & `sphinx-autosummary-accessors-2023.4.0/docs/whats-new.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 What's new
 ==========
 
+2023.04.0 (2022-04-12)
+----------------------
+- add official support for python 3.11 and `sphinx>=5.0` (:pull:`87`)
+- change the policy to only actively support the last minor release of older major
+  versions of `sphinx`.  Currently supported versions are now: `3.5`, `4.5`, and all minor
+  versions of `5`, and `6` (:pull:`87`, :pull:`100`).
+- switch to a `pyproject.toml`-based build (:pull:`99`)
+- drop support for `python=3.7` (:pull:`93`)
+
 2022.04.0 (2022-04-04)
 ----------------------
 - skip unknown templates (:issue:`66`, :pull:`67`)
 
 v0.2.1 (2021-06-06)
 -------------------
 - don't fail on options which are not parameters to the render function (:pull:`38`)
```

### Comparing `sphinx-autosummary-accessors-2022.4.0/licenses/PANDAS_LICENSE` & `sphinx-autosummary-accessors-2023.4.0/licenses/PANDAS_LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/__init__.py` & `sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/autosummary.py` & `sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/autosummary.py`

 * *Files identical despite different names*

### Comparing `sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors/documenters.py` & `sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors/documenters.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,24 +76,22 @@
             if not modname:
                 modname = self.env.ref_context.get("py:module")
             # ... else, it stays None, which means invalid
         return modname, parents + [base]
 
 
 class AccessorAttributeDocumenter(AccessorLevelDocumenter, AttributeDocumenter):
-
     objtype = "accessorattribute"
     directivetype = "attribute"
 
     # lower than AttributeDocumenter so this is not chosen for normal attributes
     priority = 0.6
 
 
 class AccessorMethodDocumenter(AccessorLevelDocumenter, MethodDocumenter):
-
     objtype = "accessormethod"
     directivetype = "method"
 
     # lower than MethodDocumenter so this is not chosen for normal methods
     priority = 0.6
```

### Comparing `sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors.egg-info/PKG-INFO` & `sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: sphinx-autosummary-accessors
-Version: 2022.4.0
+Version: 2023.4.0
 Summary: sphinx autosummary extension to properly format pandas or xarray accessors
-Home-page: https://github.com/xarray-contrib/sphinx-autosummary-accessors
-Author: Justus Magin
-Author-email: keewis@posteo.de
+Author-email: Justus Magin <keewis@posteo.de>
 License: MIT
+Project-URL: Home, https://github.com/xarray-contrib/sphinx-autosummary-accessors
 Project-URL: Documentation, https://sphinx-autosummary-accessors.readthedocs.io/en/stable
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 sphinx-autosummary-accessors
 ============================
 
 .. image:: https://github.com/xarray-contrib/sphinx-autosummary-accessors/workflows/CI/badge.svg?branch=master
@@ -64,9 +62,7 @@
 =============
 For more information and examples, see the `documentation`_.
 
 .. _pandas: https://github.com/pandas-dev/pandas
 .. _xarray: https://github.com/pydata/xarray
 .. _sphinx: https://github.com/sphinx-doc/sphinx
 .. _documentation: https://sphinx-autosummary-accessors.readthedocs.io
-
-
```

### Comparing `sphinx-autosummary-accessors-2022.4.0/sphinx_autosummary_accessors.egg-info/SOURCES.txt` & `sphinx-autosummary-accessors-2023.4.0/sphinx_autosummary_accessors.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+.flake8
 .gitignore
 .pre-commit-config.yaml
+.readthedocs.yaml
 LICENSE
 README.rst
 pyproject.toml
-readthedocs.yml
 requirements.txt
-setup.cfg
-setup.py
 .github/dependabot.yml
 .github/workflows/ci.yaml
 .github/workflows/format-logs.py
 .github/workflows/nightly.yaml
 .github/workflows/publish.yaml
+ci/requirements.txt
 docs/conf.py
 docs/environment.yml
 docs/example.py
 docs/examples.rst
 docs/index.rst
 docs/installing.rst
 docs/requirements.txt
```

