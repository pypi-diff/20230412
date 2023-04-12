# Comparing `tmp/ape-polygon-0.6.0.tar.gz` & `tmp/ape-polygon-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-polygon-0.6.0.tar", last modified: Tue Jan 31 19:22:53 2023, max compression
+gzip compressed data, was "ape-polygon-0.6.1.tar", last modified: Wed Apr 12 21:30:16 2023, max compression
```

## Comparing `ape-polygon-0.6.0.tar` & `ape-polygon-0.6.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:22:53.403837 ape-polygon-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:22:53.403837 ape-polygon-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:22:53.403837 ape-polygon-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:22:53.403837 ape-polygon-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-01-31 19:22:53.403837 ape-polygon-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:22:53.403837 ape-polygon-0.6.0/ape_polygon/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/ape_polygon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/ape_polygon/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/ape_polygon/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-31 19:22:53.000000 ape-polygon-0.6.0/ape_polygon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:22:53.403837 ape-polygon-0.6.0/ape_polygon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-01-31 19:22:53.000000 ape-polygon-0.6.0/ape_polygon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-01-31 19:22:53.000000 ape-polygon-0.6.0/ape_polygon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:22:53.000000 ape-polygon-0.6.0/ape_polygon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:22:53.000000 ape-polygon-0.6.0/ape_polygon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-01-31 19:22:53.000000 ape-polygon-0.6.0/ape_polygon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-31 19:22:53.000000 ape-polygon-0.6.0/ape_polygon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-31 19:22:53.403837 ape-polygon-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:22:53.403837 ape-polygon-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-31 19:21:55.000000 ape-polygon-0.6.0/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/ape_polygon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/ape_polygon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/ape_polygon/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/ape_polygon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/ape_polygon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 21:30:16.000000 ape-polygon-0.6.1/ape_polygon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:30:16.860195 ape-polygon-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 21:29:32.000000 ape-polygon-0.6.1/tests/test_provider.py
```

### Comparing `ape-polygon-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-polygon-0.6.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/.github/release-drafter.yml` & `ape-polygon-0.6.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/.github/workflows/commitlint.yaml` & `ape-polygon-0.6.1/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/.github/workflows/prtitle.yaml` & `ape-polygon-0.6.1/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/.github/workflows/publish.yaml` & `ape-polygon-0.6.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/.github/workflows/test.yaml` & `ape-polygon-0.6.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/.gitignore` & `ape-polygon-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/.pre-commit-config.yaml` & `ape-polygon-0.6.1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -6,26 +6,31 @@
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
     -   id: mypy
         additional_dependencies: [types-setuptools, pydantic]
 
+-   repo: https://github.com/executablebooks/mdformat
+    rev: 0.7.14
+    hooks:
+    -   id: mdformat
+        additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
 
 default_language_version:
     python: python3
```

### Comparing `ape-polygon-0.6.0/CONTRIBUTING.md` & `ape-polygon-0.6.1/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 
 It's a good idea to make pull requests early on.
 A pull request represents the start of a discussion, and doesn't necessarily need to be the final, finished submission.
 
 If you are opening a work-in-progress pull request to verify that it passes CI tests, please consider
 [marking it as a draft](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests#draft-pull-requests).
 
-Join the Ethereum Python [Discord](https://discord.gg/PcEJ54yX) if you have any questions.
+Join the ApeWorX [Discord](https://discord.gg/apeworx) if you have any questions.
```

### Comparing `ape-polygon-0.6.0/LICENSE` & `ape-polygon-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/PKG-INFO` & `ape-polygon-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-polygon
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-polygon: Ape Ecosystem Plugin for Polygon
 Home-page: https://github.com/ApeWorX/ape-polygon
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-polygon-0.6.0/README.md` & `ape-polygon-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/ape_polygon/__init__.py` & `ape-polygon-0.6.1/ape_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/ape_polygon/ecosystem.py` & `ape-polygon-0.6.1/ape_polygon/ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/ape_polygon.egg-info/PKG-INFO` & `ape-polygon-0.6.1/ape_polygon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-polygon
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-polygon: Ape Ecosystem Plugin for Polygon
 Home-page: https://github.com/ApeWorX/ape-polygon
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-polygon-0.6.0/ape_polygon.egg-info/SOURCES.txt` & `ape-polygon-0.6.1/ape_polygon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/pyproject.toml` & `ape-polygon-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.0/setup.py` & `ape-polygon-0.6.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=22.12.0",  # auto-formatter and linter
-        "mypy>=0.991",  # Static type analyzer
+        "black>=23.3.0,<24",  # Auto-formatter and linter
+        "mypy>=0.991,<1",  # Static type analyzer
         "types-setuptools",  # Needed due to mypy typeshed
-        "flake8>=5.0.4",  # Style linter
-        "isort>=5.10.1",  # Import sorting linter
+        "flake8>=6.0.0,<7",  # Style linter
+        "isort>=5.10.1,<6",  # Import sorting linter
         "mdformat>=0.7.16",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
         "wheel",  # Packaging tool
```

### Comparing `ape-polygon-0.6.0/tests/test_integration.py` & `ape-polygon-0.6.1/tests/test_integration.py`

 * *Files identical despite different names*

