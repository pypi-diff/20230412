# Comparing `tmp/katalytic-files-0.3.4.tar.gz` & `tmp/katalytic-files-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-files-0.3.4.tar", last modified: Wed Apr 12 13:31:20 2023, max compression
+gzip compressed data, was "katalytic-files-0.3.7.tar", last modified: Wed Apr 12 15:24:17 2023, max compression
```

## Comparing `katalytic-files-0.3.4.tar` & `katalytic-files-0.3.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0       87 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/.gitignore
--rw-r--r--   0        0        0      841 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/.gitlab-ci.yml
--rw-r--r--   0        0        0      367 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/.travis.yml
--rw-r--r--   0        0        0     1066 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/LICENSE.txt
--rw-r--r--   0        0        0     1905 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/README.md
--rw-r--r--   0        0        0     1649 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/pyproject.toml
--rw-r--r--   0        0        0       14 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/requirements.txt
--rw-r--r--   0        0        0      123 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/build.sh
--rw-r--r--   0        0        0     3815 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/build_check_release.sh
--rw-r--r--   0        0        0      234 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/cleanup.sh
--rw-r--r--   0        0        0     1270 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/pytest.sh
--rw-r--r--   0        0        0     6428 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/release.py
--rw-r--r--   0        0        0      403 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/setup.sh
--rw-r--r--   0        0        0     1707 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/venv.sh
--rw-r--r--   0        0        0    11060 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/src/katalytic/files.py
--rw-r--r--   0        0        0    39566 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/tests/test_files.py
--rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 katalytic-files-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/.gitlab-ci.yml
+-rw-r--r--   0        0        0      367 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/.travis.yml
+-rw-r--r--   0        0        0      197 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/LICENSE.txt
+-rw-r--r--   0        0        0     1905 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/README.md
+-rw-r--r--   0        0        0     1608 2023-04-12 15:24:16.396681 katalytic-files-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0       14 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/requirements.txt
+-rw-r--r--   0        0        0      123 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/build.sh
+-rw-r--r--   0        0        0     1460 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/build_check_release.sh
+-rw-r--r--   0        0        0      234 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1270 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/pytest.sh
+-rw-r--r--   0        0        0     6428 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/release.py
+-rw-r--r--   0        0        0      403 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/setup.sh
+-rw-r--r--   0        0        0     1707 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/scripts/venv.sh
+-rw-r--r--   0        0        0    11060 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/src/katalytic/files.py
+-rw-r--r--   0        0        0    39566 2023-04-12 15:23:36.240613 katalytic-files-0.3.7/tests/test_files.py
+-rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 katalytic-files-0.3.7/PKG-INFO
```

### Comparing `katalytic-files-0.3.4/.gitignore` & `katalytic-files-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.4/.gitlab-ci.yml` & `katalytic-files-0.3.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.4/LICENSE.txt` & `katalytic-files-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.4/README.md` & `katalytic-files-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.4/pyproject.toml` & `katalytic-files-0.3.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-files"
-version = "0.3.4"
+version = "0.3.7"
 description = "This plugin adds utilities for working with files to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -58,13 +58,11 @@
 deps = -e .
 
 commands = pytest --cov-fail-under=100 --cov=katalytic --cov-report term-missing
 """
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version"
-
-[testpypi]
-repository = "https://test.pypi.org/legacy/"
+branch = "main"
 
 [tool.flit.module]
 name = "katalytic.files"
```

### Comparing `katalytic-files-0.3.4/scripts/conda.sh` & `katalytic-files-0.3.7/scripts/conda.sh`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.4/scripts/find_requirements.py` & `katalytic-files-0.3.7/scripts/find_requirements.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.4/scripts/release.py` & `katalytic-files-0.3.7/scripts/release.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.4/scripts/venv.sh` & `katalytic-files-0.3.7/scripts/venv.sh`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.4/src/katalytic/files.py` & `katalytic-files-0.3.7/src/katalytic/files.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.4/tests/test_files.py` & `katalytic-files-0.3.7/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.4/PKG-INFO` & `katalytic-files-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-files
-Version: 0.3.4
+Version: 0.3.7
 Summary: This plugin adds utilities for working with files to the katalytic namespace
 Keywords: automation,filesystem
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

