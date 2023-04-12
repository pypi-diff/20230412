# Comparing `tmp/katalytic-files-0.3.2.tar.gz` & `tmp/katalytic-files-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-files-0.3.2.tar", last modified: Sun Apr  9 06:14:04 2023, max compression
+gzip compressed data, was "katalytic-files-0.3.4.tar", last modified: Wed Apr 12 13:31:20 2023, max compression
```

## Comparing `katalytic-files-0.3.2.tar` & `katalytic-files-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/
--rw-rw-r--   0 wip       (1000) wip       (1000)     1066 2023-04-06 18:07:34.000000 katalytic-files-0.3.2/LICENSE.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)     3352 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/PKG-INFO
--rw-rw-r--   0 wip       (1000) wip       (1000)     1224 2023-04-06 18:07:34.000000 katalytic-files-0.3.2/README.md
--rw-rw-r--   0 wip       (1000) wip       (1000)     1081 2023-04-09 04:47:14.000000 katalytic-files-0.3.2/pyproject.toml
--rw-rw-r--   0 wip       (1000) wip       (1000)       38 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/setup.cfg
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/src/
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/src/katalytic/
--rw-rw-r--   0 wip       (1000) wip       (1000)    10912 2023-04-09 04:16:13.000000 katalytic-files-0.3.2/src/katalytic/files.py
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/src/katalytic_files.egg-info/
--rw-rw-r--   0 wip       (1000) wip       (1000)     3352 2023-04-09 06:14:04.000000 katalytic-files-0.3.2/src/katalytic_files.egg-info/PKG-INFO
--rw-rw-r--   0 wip       (1000) wip       (1000)      293 2023-04-09 06:14:04.000000 katalytic-files-0.3.2/src/katalytic_files.egg-info/SOURCES.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)        1 2023-04-09 06:14:04.000000 katalytic-files-0.3.2/src/katalytic_files.egg-info/dependency_links.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)       35 2023-04-09 06:14:04.000000 katalytic-files-0.3.2/src/katalytic_files.egg-info/requires.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)       10 2023-04-09 06:14:04.000000 katalytic-files-0.3.2/src/katalytic_files.egg-info/top_level.txt
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/tests/
--rw-rw-r--   0 wip       (1000) wip       (1000)    39656 2023-04-06 18:07:34.000000 katalytic-files-0.3.2/tests/test_files.py
+-rw-r--r--   0        0        0       87 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0      367 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/.travis.yml
+-rw-r--r--   0        0        0     1066 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/LICENSE.txt
+-rw-r--r--   0        0        0     1905 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/README.md
+-rw-r--r--   0        0        0     1649 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       14 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/requirements.txt
+-rw-r--r--   0        0        0      123 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/build.sh
+-rw-r--r--   0        0        0     3815 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/build_check_release.sh
+-rw-r--r--   0        0        0      234 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1270 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/pytest.sh
+-rw-r--r--   0        0        0     6428 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/release.py
+-rw-r--r--   0        0        0      403 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/setup.sh
+-rw-r--r--   0        0        0     1707 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/scripts/venv.sh
+-rw-r--r--   0        0        0    11060 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/src/katalytic/files.py
+-rw-r--r--   0        0        0    39566 2023-04-12 13:30:33.145918 katalytic-files-0.3.4/tests/test_files.py
+-rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 katalytic-files-0.3.4/PKG-INFO
```

### Comparing `katalytic-files-0.3.2/LICENSE.txt` & `katalytic-files-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.2/pyproject.toml` & `katalytic-files-0.3.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,70 @@
+[build-system]
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
+
 [project]
 name = "katalytic-files"
-version = "0.3.2"
+version = "0.3.4"
 description = "This plugin adds utilities for working with files to the katalytic namespace"
-
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
-requires-python = ">=3.6"
-dependencies = [
-	"katalytic-pkg>=0.2.0",
-]
-
 classifiers = [
-	"Development Status :: 4 - Beta",
-	"Intended Audience :: Developers",
-	"Intended Audience :: System Administrators",
-	"License :: OSI Approved :: MIT License",
-	"Natural Language :: English",
-	"Operating System :: OS Independent",
-	"Programming Language :: Python :: 3",
-	"Topic :: Software Development :: Libraries",
-	"Topic :: System :: Filesystems",
-	"Topic :: System :: Systems Administration",
-	"Topic :: Utilities",
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "Intended Audience :: System Administrators",
+    "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Topic :: Software Development :: Libraries",
+    "Topic :: System :: Filesystems",
+    "Topic :: System :: Systems Administration",
+    "Topic :: Utilities",
 ]
 keywords = [
-	"automation",
+    "automation",
+    "filesystem"
 ]
-authors = [
-	{name="Valentin Neagu", email="vali19th@protonmail.com"}
+authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
+
+requires-python = ">=3.6"
+dependencies = [
+    "katalytic-pkg>=0.2.0",
 ]
 
 [project.optional-dependencies]
-dev = ["pytest"]
+dev = [
+    "pytest",
+    "pytest-cov",
+    "pytest-randomly",
+]
 
 [project.urls]
 homepage = "https://gitlab.com/katalytic/katalytic-files.git"
 repository = "https://gitlab.com/katalytic/katalytic-files.git"
 
 [tool.pytest.ini_options]
-addopts = [
-    "--import-mode=importlib",
-]
+addopts = ["--import-mode=importlib"]
+
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+env_list = py36, py37, py38, py39
+isolated_build = True
+
+[testenv]
+extras = dev
+deps = -e .
+
+commands = pytest --cov-fail-under=100 --cov=katalytic --cov-report term-missing
+"""
+
+[tool.semantic_release]
+version_variable = "pyproject.toml:version"
+
+[testpypi]
+repository = "https://test.pypi.org/legacy/"
 
+[tool.flit.module]
+name = "katalytic.files"
```

### Comparing `katalytic-files-0.3.2/src/katalytic/files.py` & `katalytic-files-0.3.4/src/katalytic/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import itertools
 import re
 import shutil
+import tempfile
 from pathlib import Path
 
 from katalytic.pkg import get_version
 
 __version__, __version_info__ = get_version(__name__)
 
 
@@ -14,16 +15,14 @@
         raise TypeError(f'<create_missing> expects False or True. Got {type(create_missing)}')
 
     path = Path(path)
     delete_dir(path, missing_ok=True, non_empty_dir=True)
     if create_missing:
         make_dir(path)
 
-    assert is_dir_empty(path, missing=True)
-
 
 def copy_dir(src, dest, *, dir_exists='error', file_exists='error', make_dirs=True):
     if dir_exists not in ('error', 'merge', 'replace', 'skip'):
         raise ValueError(f'<dir_exists> expects "error", "merge", "replace", "skip". Got {dir_exists!r}')
     elif file_exists not in ('error', 'replace', 'skip'):
         raise ValueError(f'<file_exists> expects "error", False, or True. Got {file_exists!r}')
     elif not isinstance(make_dirs, bool):
@@ -196,23 +195,30 @@
 
     if iter_:
         return result
     else:
         return sorted(result)
 
 
-def get_unique_path(pattern='/tmp/{}'):
+def get_unique_path(pattern='{}'):
     if not isinstance(pattern, (str, Path)):
         raise TypeError(f'<pattern> expects a str or pathlib.Path. Got {type(pattern)}')
 
     pattern = str(pattern)
     placeholders = re.findall(r'{(:((\d*)?d)?)?}', pattern)
     if len(placeholders) != 1:
         raise ValueError(f'Invalid pattern: {pattern!r}.' + 'You must provide exactly one placeholder, optionally with an integer format. Try using "{}" or "{:03d}"')
 
+    if pattern.startswith('./'):
+        pattern = pattern.partition('./')[2]
+
+    if not pattern.startswith('/'):
+        d = tempfile.mkdtemp()
+        pattern = f'{d}/{pattern}'
+
     n = 0
     while True:
         n += 1
         path = pattern.format(n)
         if not Path(path).exists():
             return path
```

### Comparing `katalytic-files-0.3.2/tests/test_files.py` & `katalytic-files-0.3.4/tests/test_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 from katalytic.files import _get_all, clear_dir, copy_dir, copy_file, delete_dir, delete_file, get_dirs, get_files, get_unique_path, is_dir_empty, get_all, make_dir, move_dir, move_file
 
 
 class TestGroup_copy:
     class Test_copy_dir:
         def test_dest_is_dir(self):
-            src = Path(_setup_tree('/tmp/{}_src'))
+            src = Path(_setup_tree('{}_src'))
 
-            dest = Path(get_unique_path('/tmp/{}_dest'))
+            dest = Path(get_unique_path('{}_dest'))
             copy_dir(src, dest)
             _check_tree(src, dest/src.name)
 
-            dest_2 = Path(get_unique_path('/tmp/{}_dest_2'))
+            dest_2 = Path(get_unique_path('{}_dest_2'))
             copy_dir(src, dest_2/src.name)
             _check_tree(src, dest_2/src.name)
 
         def test_dest_is_file(self):
             with pytest.raises(NotADirectoryError):
                 src = _setup_dir()
                 dest = _setup_file()
@@ -116,15 +116,15 @@
             with pytest.raises(ValueError):
                 src = _setup_dir()
                 copy_dir(src, src)
 
         def test_src_is_file(self):
             with pytest.raises(NotADirectoryError):
                 src = _setup_file()
-                dest = get_unique_path('/tmp/{}_new')
+                dest = get_unique_path('{}_new')
                 copy_dir(src, dest)
 
         def test_src_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 src = get_unique_path()
                 copy_dir(src, f'{src}_copy')
 
@@ -193,15 +193,15 @@
             root = get_unique_path()
             dest = root + '/1/2/3/'
             copy_file(src, dest)
 
         def test_make_dirs_false(self):
             with pytest.raises(FileNotFoundError):
                 src = _setup_file()
-                dest = get_unique_path('/tmp/{}/a/b/c/')
+                dest = get_unique_path('{}/a/b/c/')
                 copy_file(src, dest, make_dirs=False)
 
         def test_make_dirs_true(self):
             src = _setup_file()
             dest = _setup_path()
             copy_file(src, dest, make_dirs=True)
             assert Path(dest).read_text() == src
@@ -697,15 +697,15 @@
                 is_dir_empty(mistake)
 
     class Test_mkdir:
         def test_create(self):
             path = _setup_dir()
             assert Path(path).is_dir()
 
-            path = _setup_dir('/tmp/a/{}/b')
+            path = _setup_dir('a/{}/b')
             assert Path(path).is_dir()
 
         def test_exists_error(self):
             with pytest.raises(FileExistsError):
                 path = _setup_dir()
                 make_dir(path, exists_ok=False)
 
@@ -722,15 +722,15 @@
         def test_is_file(self):
             with pytest.raises(NotADirectoryError):
                 path = _setup_file()
                 make_dir(path)
 
         def test_no_parents(self):
             with pytest.raises(FileNotFoundError):
-                d = get_unique_path('/tmp/parent/{}/child')
+                d = get_unique_path('parent/{}/child')
                 make_dir(d, create_parents=False)
 
         @pytest.mark.parametrize('mistake', [0, None, {}, ''])
         def test_precondition_create_parents(self, mistake):
             with pytest.raises(TypeError):
                 make_dir(get_unique_path(), create_parents=mistake)
 
@@ -744,28 +744,28 @@
             with pytest.raises(TypeError):
                 make_dir(mistake)
 
 
 class TestGroup_move:
     class Test_move_dir:
         def test_dest_is_dir(self):
-            src = Path(_setup_tree('/tmp/{}_src'))
-            src_copy = Path(get_unique_path('/tmp/{}_src_copy'))
+            src = Path(_setup_tree('{}_src'))
+            src_copy = Path(get_unique_path('{}_src_copy'))
             copy_dir(src, src_copy)
 
-            dest = get_unique_path('/tmp/{}_dest')
+            dest = get_unique_path('{}_dest')
             move_dir(src, dest)
             _check_tree(src_copy, dest)
             assert not src.exists()
 
-            src = Path(_setup_tree('/tmp/{}_src'))
-            src_copy = Path(get_unique_path('/tmp/{}_src_copy'))
+            src = Path(_setup_tree('{}_src'))
+            src_copy = Path(get_unique_path('{}_src_copy'))
             copy_dir(src, src_copy)
 
-            dest = Path(get_unique_path('/tmp/{}_dest'))
+            dest = Path(get_unique_path('{}_dest'))
             move_dir(src, dest/src.name)
             _check_tree(src_copy/src.name, dest/src.name)
             assert not src.exists()
 
         def test_dest_is_file(self):
             with pytest.raises(NotADirectoryError):
                 src = _setup_dir()
@@ -848,39 +848,39 @@
                     make_dir(src)
                     move_dir(src, dest, make_dirs=False)
 
         def test_make_dirs_true(self):
             with tempfile.TemporaryDirectory() as d:
                 src = _setup_tree()
                 src_name = Path(src).name
-                src_copy = Path(get_unique_path('/tmp/{}_src_copy'))
+                src_copy = Path(get_unique_path('{}_src_copy'))
                 copy_dir(src, src_copy)
 
                 dest = get_unique_path(d + '/{}_dest')
                 move_dir(src, dest, make_dirs=True)
                 _check_tree(src_copy/src_name, f'{dest}/{src_name}')
 
                 src = _setup_tree()
                 src_name = Path(src).name
-                src_copy = Path(get_unique_path('/tmp/{}_src_copy'))
+                src_copy = Path(get_unique_path('{}_src_copy'))
                 copy_dir(src, src_copy)
 
                 dest_2 = get_unique_path(d + '/{}_dest_2')
                 move_dir(src, f'{dest_2}/{src_name}', make_dirs=True)
                 _check_tree(src_copy/src_name, f'{dest_2}/{src_name}')
 
         def test_same_path(self):
             with pytest.raises(ValueError):
                 src = _setup_dir()
                 move_dir(src, src)
 
         def test_src_is_file(self):
             with pytest.raises(NotADirectoryError):
                 src = _setup_file()
-                dest = get_unique_path('/tmp/{}_new')
+                dest = get_unique_path('{}_new')
                 move_dir(src, dest)
 
         def test_src_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 src = get_unique_path()
                 move_dir(src, f'{src}_copy')
 
@@ -940,15 +940,15 @@
             assert text != Path(src).read_text()
             assert text == dest
             assert Path(src).exists()
 
         def test_make_dirs_false(self):
             with pytest.raises(FileNotFoundError):
                 src = _setup_file()
-                dest = get_unique_path('/tmp/{}/a/b/c/')
+                dest = get_unique_path('{}/a/b/c/')
                 move_file(src, dest, make_dirs=False)
 
         def test_make_dirs_true(self):
             src = _setup_file()
             dest = _setup_path()
             move_file(src, dest, make_dirs=True)
             assert Path(dest).read_text() == src
@@ -998,15 +998,15 @@
 
         @pytest.mark.parametrize('mistake', ['', '{0}', '{a}', '{:f}'])
         def test_invalid_placeholder(self, mistake):
             with pytest.raises(ValueError):
                 get_unique_path(mistake)
 
         def test_keeps_slash_at_the_end(self):
-            assert get_unique_path('/tmp/{}/').endswith('/')
+            assert get_unique_path('{}/').endswith('/')
 
         @pytest.mark.parametrize('mistake', ['hello_{}', '{}', './{}', '/a/{}', '/{}/a', '{:06d}'])
         def test_not_exists(self, mistake):
             path = get_unique_path(mistake)
             assert not Path(path).exists()
```

