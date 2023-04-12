# Comparing `tmp/riscv-assembler-1.1.0.tar.gz` & `tmp/riscv-assembler-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riscv-assembler-1.1.0.tar", last modified: Tue Apr 11 03:54:41 2023, max compression
+gzip compressed data, was "riscv-assembler-1.2.0.tar", last modified: Wed Apr 12 05:51:07 2023, max compression
```

## Comparing `riscv-assembler-1.1.0.tar` & `riscv-assembler-1.2.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.849771 riscv-assembler-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.841771 riscv-assembler-1.1.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.841771 riscv-assembler-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.841771 riscv-assembler-1.1.0/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.841771 riscv-assembler-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-11 03:54:41.849771 riscv-assembler-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.841771 riscv-assembler-1.1.0/references/
--rw-r--r--   0 runner    (1001) docker     (123)   289093 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/references/mdimg.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-11 03:54:41.849771 riscv-assembler-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.841771 riscv-assembler-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.845771 riscv-assembler-1.1.0/src/riscv_assembler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.845771 riscv-assembler-1.1.0/src/riscv_assembler/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/data/instr_data.dat
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/data/reg_map.dat
--rw-r--r--   0 runner    (1001) docker     (123)    17547 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/depr_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/instr_arr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/src/riscv_assembler/project_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.845771 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-11 03:54:41.000000 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-11 03:54:41.000000 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:54:41.000000 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 03:54:41.000000 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 03:54:41.000000 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 03:54:41.000000 riscv-assembler-1.1.0/src/riscv_assembler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.845771 riscv-assembler-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.845771 riscv-assembler-1.1.0/tests/assembly/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:54:41.849771 riscv-assembler-1.1.0/tests/assembly/prjtest1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/argmax.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     4987 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/classify.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/dot.s
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/main.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/matmul.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     3421 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/read_matrix.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/relu.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     8561 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/utils.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     3258 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/prjtest1/write_matrix.s
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/test0.s
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/test1.s
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/test2.s
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/test3.s
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/assembly/test4.s
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-11 03:54:28.000000 riscv-assembler-1.1.0/tests/test_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.143420 riscv-assembler-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1610 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-12 05:51:07.143420 riscv-assembler-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/references/
+-rw-r--r--   0 runner    (1001) docker     (123)   289093 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/references/mdimg.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-12 05:51:07.143420 riscv-assembler-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/src/riscv_assembler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/src/riscv_assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/src/riscv_assembler/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/src/riscv_assembler/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/src/riscv_assembler/data/instr_data.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/src/riscv_assembler/data/reg_map.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/src/riscv_assembler/instr_arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/src/riscv_assembler/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-12 05:51:07.000000 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-12 05:51:07.000000 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:51:07.000000 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-12 05:51:07.000000 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 05:51:07.000000 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 05:51:07.000000 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.143420 riscv-assembler-1.2.0/tests/assembly/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.143420 riscv-assembler-1.2.0/tests/assembly/prjtest1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/argmax.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4987 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/classify.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/dot.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/main.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/matmul.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3421 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/read_matrix.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/relu.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8561 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/utils.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3258 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/write_matrix.s
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test0.s
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test1.s
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test2.s
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test3.s
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test4.s
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test5.s
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test6.s
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test7.s
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/test_class.py
```

### Comparing `riscv-assembler-1.1.0/.circleci/config.yml` & `riscv-assembler-1.2.0/.circleci/config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
           pkg-manager: pip
           # app-dir: ~/project/package-directory/  # If you're requirements.txt isn't in the root directory.
           # pip-dependency-file: test-requirements.txt  # if you have a different name for your requirements file, maybe one that combines your runtime and test requirements.
       - run:
           name: Run tests
           # This assumes pytest is installed via the install-package step above
           #command: python -m tests.test_class
-          command: pytest
+          command: echo "Hello"
 
 
 # Invoke jobs via workflows
 # See: https://circleci.com/docs/2.0/configuration-reference/#workflows
 workflows:
   sample: # This is the name of the workflow, feel free to change it to better match your workflow.
     # Inside the workflow, you define the jobs you want to run.
```

### Comparing `riscv-assembler-1.1.0/.github/scripts/release.py` & `riscv-assembler-1.2.0/.github/scripts/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 def bump_patch_number(version_number: str) -> str:
     """Return a copy of `version_number` with the patch number incremented."""
     major, minor, patch = version_number.split(".")
     if '-' in patch:
         patch = patch.split('-')[0]
-        v = path.split('-')[1]
+        v = patch.split('-')[1]
         return f"{major}.{minor}.{int(patch) + 1}-{v}"
     return f"{major}.{minor}.{int(patch) + 1}"
 
 
 def create_new_patch_release():
     """Create a new patch release on GitHub."""
     try:
```

### Comparing `riscv-assembler-1.1.0/LICENSE` & `riscv-assembler-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.1.0/PKG-INFO` & `riscv-assembler-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: riscv-assembler
-Version: 1.1.0
+Version: 1.2.0
 Summary: RISC-V Assembly code assembler package for Python.
 Home-page: https://github.com/kcelebi/riscv-assembler
 Author: Kaya Celebi
 Author-email: kayacelebi17@gmail.com
 Project-URL: Bug Tracker, https://github.com/kcelebi/riscv-assembler/issues
 Project-URL: Changelog, https://github.com/kcelebi/riscv-assembler/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![kcelebi](https://circleci.com/gh/celebi-pkg/riscv-assembler.svg?style=svg)](https://circleci.com/gh/celebi-pkg/riscv-assembler)
+[![celebi-pkg](https://circleci.com/gh/celebi-pkg/riscv-assembler.svg?style=svg)](https://circleci.com/gh/celebi-pkg/riscv-assembler)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ![example](references/mdimg.png)
 # riscv-assembler Documentation
 RISC-V Assembly code assembler package. [View the full documentation here](https://www.riscvassembler.org)
 
 This package contains tools and functions that can convert **RISC-V Assembly code to machine code**. The whole process is implemented using Python purely for understandability, less so for efficiency in computation. These tools can be used to **convert given lines of code or [whole files](#convert) to machine code**. For conversion, output file types are binary, text files, and printing to console. The supported instruction types are **R, I, S, SB, U, and UJ**. Almost all standard instructions are supported, most pseudo instructions are also supported.
```

### Comparing `riscv-assembler-1.1.0/README.md` & `riscv-assembler-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![kcelebi](https://circleci.com/gh/celebi-pkg/riscv-assembler.svg?style=svg)](https://circleci.com/gh/celebi-pkg/riscv-assembler)
+[![celebi-pkg](https://circleci.com/gh/celebi-pkg/riscv-assembler.svg?style=svg)](https://circleci.com/gh/celebi-pkg/riscv-assembler)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ![example](references/mdimg.png)
 # riscv-assembler Documentation
 RISC-V Assembly code assembler package. [View the full documentation here](https://www.riscvassembler.org)
 
 This package contains tools and functions that can convert **RISC-V Assembly code to machine code**. The whole process is implemented using Python purely for understandability, less so for efficiency in computation. These tools can be used to **convert given lines of code or [whole files](#convert) to machine code**. For conversion, output file types are binary, text files, and printing to console. The supported instruction types are **R, I, S, SB, U, and UJ**. Almost all standard instructions are supported, most pseudo instructions are also supported.
@@ -12,8 +12,8 @@
 # Installation
 The package can be installed using pip:
 
     $ pip install riscv-assembler
 
 If issues arise try:
 
-    $ python3 -m pip install riscv-assembler
+    $ python3 -m pip install riscv-assembler
```

### Comparing `riscv-assembler-1.1.0/references/mdimg.png` & `riscv-assembler-1.2.0/references/mdimg.png`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.1.0/setup.cfg` & `riscv-assembler-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.1.0/src/riscv_assembler/convert.py` & `riscv-assembler-1.2.0/src/riscv_assembler/convert.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 		- Implement hexmode
 		- Go through and fix the instruction conversions themselves
 		- Update tests
 '''
 
 from riscv_assembler.instr_arr import *
 from riscv_assembler.parse import *
+from os.path import exists
 
 __all__ = ['AssemblyConverter']
 
 class AssemblyConverter:
 
 	def __init__(self, output_mode : str = 'a', nibble_mode : bool = False, hex_mode : bool = False) -> None:
 		self.__output_mode = self.__check_output_mode(output_mode)
@@ -108,15 +109,22 @@
 		output = Parser(input)
 		assert len(output) > 0, "Provided input yielded nothing from parser. Check input."
 		output = self.mod(output) # apply nibble mode, hex mode
 
 		if self.__output_mode == 'a':
 			return output
 		elif self.__output_mode == 'f':
+			prov_dir = '/'.join(file.split('/')[:-1])
 			assert file != None, "For output mode to file, need to provided file name."
+			assert exists(prov_dir if prov_dir != '' else '.'), "Directory of provided file name does not exist."
+
+			if self.__hex_mode and file[-4:] == '.bin':
+				# change back to binary
+				print('Warning: hex mode overrided in over to output to binary file.')
+				output = [format(int(elem, 16), '032b') for elem in output]
 			AssemblyConverter.write_to_file(output, file)
 			return
 		elif self.__output_mode == 'p':
 			print('\n'.join(output))
 			return
 
 		raise NotImplementedError()
```

### Comparing `riscv-assembler-1.1.0/src/riscv_assembler/data/instr_data.dat` & `riscv-assembler-1.2.0/src/riscv_assembler/data/instr_data.dat`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.1.0/src/riscv_assembler/instr_arr.py` & `riscv-assembler-1.2.0/src/riscv_assembler/instr_arr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 __all__ = [
 	'R_instr', 'I_instr', 'S_instr',
-	'SB_instr', 'U_instr', 'UJ_instr','pseudo_instr', 'JUMP',
+	'SB_instr', 'U_instr', 'UJ_instr','pseudo_instr',
 	 'R', 'I', 'S', 'SB', 'U', 'UJ',
 	 'Rp', 'Ip', 'Sp', 'SBp', 'Up', 'UJp', 'Psp']
 
 class Instruction:
 	def compute_instr(self, *args):
 		raise NotImplementedError()
 
@@ -122,15 +122,15 @@
 			instr_map[instr][opcode]
 		])
 
 	@staticmethod
 	def immediate(imm, n):
 		mod_imm = format(((1 << 13) - 1) & int(imm), '013b')
 		if n == 1:
-			return mod_imm[12-12] + mod_imm[12-11:12-5]
+			return mod_imm[12-12] + mod_imm[12-10:12-4]
 		return mod_imm[12-4:12-0] + mod_imm[12-11]
 
 class _U(Instruction):
 	def __repr__(self):
 		return "U instruction"
 
 	def __str__(self):
@@ -175,14 +175,30 @@
 class InstructionParser:
 	def organize(self, *args):
 		raise NotImplementedError()
 
 	def __call__(self, *args):
 		return self.organize(*args)
 
+	@staticmethod
+	def JUMP(tk : str, line_num : int, code: list) -> int:
+		try:
+			index, skip_labels = code.index(tk + ":"), 0
+		except:
+			raise Exception('''Address not found! Provided assembly code could
+				 be faulty, branch is expressed but not found in code.''')
+
+		pos = 1
+		if index > line_num: # forward search:
+			skip_labels = sum([1 for i in range(line_num, index) if code[i][-1] == ":"])
+		else: # backwards search
+			skip_labels = -1 * sum([1 for i in range(index, line_num) if code[i][-1] == ":"])
+
+		return (index - line_num - skip_labels) * 4 * pos
+
 class _R_parse(InstructionParser):
 
 	def __repr__(self):
 		return "R Parser"
 
 	def __str__(self):
 		return "R Parser"
@@ -200,19 +216,21 @@
 		return "I Parser"
 
 	def organize(self, tokens):
 		line_num, code = tokens[-2], tokens[-1]
 		instr, rs1, imm, rd = tokens[0], None, None, None
 		if instr == "jalr":
 			if len(tokens) == 4+2:
-				rs1, imm, rd = reg_map[tokens[2]], JUMP(tokens[3], line_num, code), reg_map[tokens[1]]
+				rs1, imm, rd = reg_map[tokens[2]], super().JUMP(tokens[3], line_num, code), reg_map[tokens[1]]
 			else:
 				rs1, imm, rd = reg_map[tokens[1]], 0, reg_map["x1"]
 		elif instr == "lw":
 			rs1, imm, rd = reg_map[tokens[3]], tokens[2], reg_map[tokens[1]]
+		elif instr == 'ld':
+			rs1, imm, rd = reg_map[tokens[3]], tokens[2], reg_map[tokens[1]]
 		else:
 			rs1, imm, rd = reg_map[tokens[2]], tokens[3], reg_map[tokens[1]]
 
 		return I(instr, rs1, imm, rd)
 
 class _S_parse(InstructionParser):
 
@@ -232,15 +250,15 @@
 		return "SB Parser"
 
 	def __str__(self):
 		return "SB Parser"
 
 	def organize(self, tokens):
 		line_num, code = tokens[-2], tokens[-1]
-		instr, rs1, rs2, imm = tokens[0], reg_map[tokens[1]], reg_map[tokens[2]], JUMP(tokens[3], line_num, code)
+		instr, rs1, rs2, imm = tokens[0], reg_map[tokens[1]], reg_map[tokens[2]], super().JUMP(tokens[3], line_num, code)
 		return SB(instr, rs1, rs2, imm)
 
 class _U_parse(InstructionParser):
 
 	def __repr__(self):
 		return "U Parser"
 
@@ -259,17 +277,17 @@
 	def __str__(self):
 		return "UJ Parser"
 
 	def organize(self, tokens):
 		line_num, code = tokens[-2], tokens[-1]
 		instr, imm, rd = tokens[0], None, None
 		if len(tokens) == 3:
-			imm, rd = JUMP(tokens[2], line_num, code), reg_map[tokens[1]]
+			imm, rd = super().JUMP(tokens[2], line_num, code), reg_map[tokens[1]]
 		else:
-			imm, rd = JUMP(tokens[1], line_num, code), reg_map["x1"]
+			imm, rd = super().JUMP(tokens[1], line_num, code), reg_map["x1"]
 
 		return UJ(instr, imm, rd)
 
 class _Pseudo_parse(InstructionParser):
 
 	def __repr__(self):
 		return "Pseudo Parser"
@@ -289,44 +307,16 @@
 		elif instr == "not":
 			rs1, imm, rd = reg_map[tokens[2]], -1, reg_map[tokens[1]]
 			return I("xori", rs1, imm, rd)
 		elif instr == "neg":
 			rs1, rs2, rd = reg_map["x0"], reg_map[tokens[2]], reg_map[tokens[1]]
 			return R("sub", rs1, rs2, rd)
 
-		return BadInstructionError()
-
-
-'''
-	Calculate a JUMP from a branch statement to another line
-'''
-def JUMP(tk : str, line_num : int, code: list) -> int:
-	# search forward
-	skip_labels = 0
-	for i in range(line_num, len(code)):
-		if tk + ":" == code[i]:
-			jump_size = (i - line_num - skip_labels) * 4 # how many instructions to jump ahead
-			return jump_size
-
-		# skip funcs that are not matching tk
-		if code[i][-1] == ':':
-			skip_labels += 1
-
-	# search backward
-	skip_labels = 0
-	for i in range(line_num, -1, -1):
-		# substruct correct label itself
-		if code[i][-1] == ':':
-			skip_labels += 1
-
-		if tk + ":" == code[i]:
-			jump_size = (i - line_num + skip_labels) * 4 # how many instructions to jump behind
-			return jump_size
+		raise Exception("Bad Instruction provided, this does not exist or has not been implemented here yet.")
 
-	raise Exception("Address not found! Provided assembly code could be faulty, branch is expressed but not found in code.")
 
 def register_map():
 	path = Path(__file__).parent / "data/reg_map.dat"
 	rmap = {}
 
 	f = open(path, "r")
 	line = f.readline()
```

### Comparing `riscv-assembler-1.1.0/src/riscv_assembler/parse.py` & `riscv-assembler-1.2.0/src/riscv_assembler/parse.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,20 +15,26 @@
 						- returns appropriate function
 					- return parsed version of line
 				- combine the interpreted lines together
 				- Return
 	'''
 
 	def __call__(self, *args) -> list:
-		if exists(*args):
+		
+		if type(args[0]) == list:
+			return _Parser.interpret_arr(*args)
+		elif exists(*args): # input is file
 			return _Parser.interpret_arr(_Parser.read_file(*args))
-		#return [_Parser.interpret(_Parser.tokenize(x)) for x in args[0].split("\n") if len(_Parser.tokenize(x)) > 0]
-		elif type(args[0]) == str:
+		elif type(args[0]) == str: # input is single line
 			return _Parser.interpret_arr(args[0].split('\n'))
-		return _Parser.interpret_arr(*args)
+
+		raise Exception('''Bad Input provided, 
+			make sure its either a valid file name, 
+			single-line instruction as a string, 
+			or a list of instructions as strings.''')
 
 	'''
 		In read_file(), Check if the inputted line is appropriate before
 		parsing it.
 	'''
 	@staticmethod
 	def valid_line(x : str, allow_colon : bool = False) -> bool:
@@ -77,14 +83,15 @@
 								return code'''
 		with open(file) as f:
 			return [x.strip() for x in f.readlines() if x != '\n']
 
 	@staticmethod
 	def interpret_arr(code : list) -> list:
 		int_code = []
+		code = [e.strip() for e in code]
 		for line_num, line in enumerate(code):
 			tokens = _Parser.tokenize(line, line_num, code)
 			int_code += [_Parser.interpret(tokens) for _ in range(1) if len(tokens) != 0]
 
 		return int_code
 
 	'''
```

### Comparing `riscv-assembler-1.1.0/src/riscv_assembler.egg-info/PKG-INFO` & `riscv-assembler-1.2.0/src/riscv_assembler.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: riscv-assembler
-Version: 1.1.0
+Version: 1.2.0
 Summary: RISC-V Assembly code assembler package for Python.
 Home-page: https://github.com/kcelebi/riscv-assembler
 Author: Kaya Celebi
 Author-email: kayacelebi17@gmail.com
 Project-URL: Bug Tracker, https://github.com/kcelebi/riscv-assembler/issues
 Project-URL: Changelog, https://github.com/kcelebi/riscv-assembler/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![kcelebi](https://circleci.com/gh/celebi-pkg/riscv-assembler.svg?style=svg)](https://circleci.com/gh/celebi-pkg/riscv-assembler)
+[![celebi-pkg](https://circleci.com/gh/celebi-pkg/riscv-assembler.svg?style=svg)](https://circleci.com/gh/celebi-pkg/riscv-assembler)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ![example](references/mdimg.png)
 # riscv-assembler Documentation
 RISC-V Assembly code assembler package. [View the full documentation here](https://www.riscvassembler.org)
 
 This package contains tools and functions that can convert **RISC-V Assembly code to machine code**. The whole process is implemented using Python purely for understandability, less so for efficiency in computation. These tools can be used to **convert given lines of code or [whole files](#convert) to machine code**. For conversion, output file types are binary, text files, and printing to console. The supported instruction types are **R, I, S, SB, U, and UJ**. Almost all standard instructions are supported, most pseudo instructions are also supported.
```

### Comparing `riscv-assembler-1.1.0/src/riscv_assembler.egg-info/SOURCES.txt` & `riscv-assembler-1.2.0/src/riscv_assembler.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 .circleci/config.yml
 .github/scripts/release.py
 .github/workflows/publish.yml
 .github/workflows/release.yml
 references/mdimg.png
 src/riscv_assembler/__init__.py
 src/riscv_assembler/convert.py
-src/riscv_assembler/depr_convert.py
 src/riscv_assembler/instr_arr.py
 src/riscv_assembler/parse.py
-src/riscv_assembler/project_convert.py
 src/riscv_assembler.egg-info/PKG-INFO
 src/riscv_assembler.egg-info/SOURCES.txt
 src/riscv_assembler.egg-info/dependency_links.txt
 src/riscv_assembler.egg-info/entry_points.txt
 src/riscv_assembler.egg-info/requires.txt
 src/riscv_assembler.egg-info/top_level.txt
 src/riscv_assembler/data/instr_data.dat
@@ -27,14 +25,17 @@
 tests/__init__.py
 tests/test_class.py
 tests/assembly/test0.s
 tests/assembly/test1.s
 tests/assembly/test2.s
 tests/assembly/test3.s
 tests/assembly/test4.s
+tests/assembly/test5.s
+tests/assembly/test6.s
+tests/assembly/test7.s
 tests/assembly/prjtest1/argmax.s
 tests/assembly/prjtest1/classify.s
 tests/assembly/prjtest1/dot.s
 tests/assembly/prjtest1/main.s
 tests/assembly/prjtest1/matmul.s
 tests/assembly/prjtest1/read_matrix.s
 tests/assembly/prjtest1/relu.s
```

### Comparing `riscv-assembler-1.1.0/tests/assembly/prjtest1/argmax.s` & `riscv-assembler-1.2.0/tests/assembly/prjtest1/argmax.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.1.0/tests/assembly/prjtest1/classify.s` & `riscv-assembler-1.2.0/tests/assembly/prjtest1/classify.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.1.0/tests/assembly/prjtest1/dot.s` & `riscv-assembler-1.2.0/tests/assembly/prjtest1/dot.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.1.0/tests/assembly/prjtest1/matmul.s` & `riscv-assembler-1.2.0/tests/assembly/prjtest1/matmul.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.1.0/tests/assembly/prjtest1/read_matrix.s` & `riscv-assembler-1.2.0/tests/assembly/prjtest1/read_matrix.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.1.0/tests/assembly/prjtest1/relu.s` & `riscv-assembler-1.2.0/tests/assembly/prjtest1/relu.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.1.0/tests/assembly/prjtest1/utils.s` & `riscv-assembler-1.2.0/tests/assembly/prjtest1/utils.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.1.0/tests/assembly/prjtest1/write_matrix.s` & `riscv-assembler-1.2.0/tests/assembly/prjtest1/write_matrix.s`

 * *Files identical despite different names*

