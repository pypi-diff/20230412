# Comparing `tmp/tables_io-0.7.9.tar.gz` & `tmp/tables_io-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tables_io-0.7.9.tar", last modified: Fri Aug 12 21:50:26 2022, max compression
+gzip compressed data, was "tables_io-0.8.0.tar", last modified: Wed Apr 12 16:42:25 2023, max compression
```

## Comparing `tables_io-0.7.9.tar` & `tables_io-0.8.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 21:50:26.615584 tables_io-0.7.9/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-12 21:50:13.000000 tables_io-0.7.9/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 21:50:26.607584 tables_io-0.7.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 21:50:26.611585 tables_io-0.7.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-08-12 21:50:13.000000 tables_io-0.7.9/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-08-12 21:50:13.000000 tables_io-0.7.9/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-08-12 21:50:13.000000 tables_io-0.7.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    12773 2022-08-12 21:50:13.000000 tables_io-0.7.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-08-12 21:50:13.000000 tables_io-0.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-08-12 21:50:26.615584 tables_io-0.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-08-12 21:50:13.000000 tables_io-0.7.9/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)       59 2022-08-12 21:50:13.000000 tables_io-0.7.9/do_cover.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 21:50:26.611585 tables_io-0.7.9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-08-12 21:50:13.000000 tables_io-0.7.9/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-08-12 21:50:13.000000 tables_io-0.7.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2569 2022-08-12 21:50:13.000000 tables_io-0.7.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4898 2022-08-12 21:50:13.000000 tables_io-0.7.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-08-12 21:50:13.000000 tables_io-0.7.9/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-08-12 21:50:13.000000 tables_io-0.7.9/docs/tables_io.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 21:50:26.611585 tables_io-0.7.9/nb/
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-08-12 21:50:13.000000 tables_io-0.7.9/nb/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3213 2022-08-12 21:50:13.000000 tables_io-0.7.9/nb/hdf5_iter_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     4793 2022-08-12 21:50:13.000000 tables_io-0.7.9/nb/multipleWriteHdf5_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     5885 2022-08-12 21:50:13.000000 tables_io-0.7.9/nb/singleTable_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     8213 2022-08-12 21:50:13.000000 tables_io-0.7.9/nb/tableDict_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-08-12 21:50:13.000000 tables_io-0.7.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-12 21:50:26.615584 tables_io-0.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-08-12 21:50:13.000000 tables_io-0.7.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 21:50:26.611585 tables_io-0.7.9/tables_io/
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-08-12 21:50:13.000000 tables_io-0.7.9/tables_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-08-12 21:50:26.000000 tables_io-0.7.9/tables_io/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4934 2022-08-12 21:50:13.000000 tables_io-0.7.9/tables_io/arrayUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9925 2022-08-12 21:50:13.000000 tables_io-0.7.9/tables_io/convUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)    30855 2022-08-12 21:50:13.000000 tables_io-0.7.9/tables_io/ioUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-08-12 21:50:13.000000 tables_io-0.7.9/tables_io/lazy_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-08-12 21:50:13.000000 tables_io-0.7.9/tables_io/tableDict.py
--rw-r--r--   0 runner    (1001) docker     (121)     2349 2022-08-12 21:50:13.000000 tables_io-0.7.9/tables_io/testUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5226 2022-08-12 21:50:13.000000 tables_io-0.7.9/tables_io/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 21:50:26.615584 tables_io-0.7.9/tables_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-08-12 21:50:26.000000 tables_io-0.7.9/tables_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-08-12 21:50:26.000000 tables_io-0.7.9/tables_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 21:50:26.000000 tables_io-0.7.9/tables_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-08-12 21:50:26.000000 tables_io-0.7.9/tables_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-12 21:50:26.000000 tables_io-0.7.9/tables_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 21:50:26.615584 tables_io-0.7.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 21:50:26.615584 tables_io-0.7.9/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)     8272 2022-08-12 21:50:13.000000 tables_io-0.7.9/tests/data/no_groupname_test.hdf5
--rw-r--r--   0 runner    (1001) docker     (121)     9104 2022-08-12 21:50:13.000000 tables_io-0.7.9/tests/data/pandas_test_hdf5.h5
--rw-r--r--   0 runner    (1001) docker     (121)    10172 2022-08-12 21:50:13.000000 tables_io-0.7.9/tests/data/parquet_test.parquet
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-08-12 21:50:13.000000 tables_io-0.7.9/tests/test_conv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3497 2022-08-12 21:50:13.000000 tables_io-0.7.9/tests/test_fileIO.py
--rw-r--r--   0 runner    (1001) docker     (121)     6190 2022-08-12 21:50:13.000000 tables_io-0.7.9/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-08-12 21:50:13.000000 tables_io-0.7.9/tests/test_table_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     5557 2022-08-12 21:50:13.000000 tables_io-0.7.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.368535 tables_io-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-12 16:42:07.000000 tables_io-0.8.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.364535 tables_io-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.364535 tables_io-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-04-12 16:42:07.000000 tables_io-0.8.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1945 2023-04-12 16:42:07.000000 tables_io-0.8.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-12 16:42:07.000000 tables_io-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-04-12 16:42:07.000000 tables_io-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-04-12 16:42:25.368535 tables_io-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-12 16:42:07.000000 tables_io-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.364535 tables_io-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-04-12 16:42:07.000000 tables_io-0.8.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-04-12 16:42:07.000000 tables_io-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     2569 2023-04-12 16:42:07.000000 tables_io-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4944 2023-04-12 16:42:07.000000 tables_io-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      477 2023-04-12 16:42:07.000000 tables_io-0.8.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      961 2023-04-12 16:42:07.000000 tables_io-0.8.0/docs/tables_io.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-12 16:42:07.000000 tables_io-0.8.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.368535 tables_io-0.8.0/nb/
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-12 16:42:07.000000 tables_io-0.8.0/nb/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-04-12 16:42:07.000000 tables_io-0.8.0/nb/hdf5_iter_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     4793 2023-04-12 16:42:07.000000 tables_io-0.8.0/nb/multipleWriteHdf5_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     5885 2023-04-12 16:42:07.000000 tables_io-0.8.0/nb/singleTable_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     8213 2023-04-12 16:42:07.000000 tables_io-0.8.0/nb/tableDict_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3109 2023-04-12 16:42:07.000000 tables_io-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 16:42:25.368535 tables_io-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-12 16:42:07.000000 tables_io-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.364535 tables_io-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.368535 tables_io-0.8.0/src/tables_io/
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-12 16:42:24.000000 tables_io-0.8.0/src/tables_io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4998 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/arrayUtils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9925 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/convUtils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31624 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/ioUtils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/lazy_modules.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/tableDict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2781 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/testUtils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5328 2023-04-12 16:42:07.000000 tables_io-0.8.0/src/tables_io/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.368535 tables_io-0.8.0/src/tables_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-04-12 16:42:25.000000 tables_io-0.8.0/src/tables_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-04-12 16:42:25.000000 tables_io-0.8.0/src/tables_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 16:42:25.000000 tables_io-0.8.0/src/tables_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-04-12 16:42:25.000000 tables_io-0.8.0/src/tables_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-12 16:42:25.000000 tables_io-0.8.0/src/tables_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.368535 tables_io-0.8.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:42:25.368535 tables_io-0.8.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     8272 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/data/no_groupname_test.hdf5
+-rw-r--r--   0 runner    (1001) docker     (122)     9104 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/data/pandas_test_hdf5.h5
+-rw-r--r--   0 runner    (1001) docker     (122)    10172 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/data/parquet_test.parquet
+-rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/test_conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5176 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/test_fileIO.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7212 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/test_table_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5711 2023-04-12 16:42:07.000000 tables_io-0.8.0/tests/test_utils.py
```

### Comparing `tables_io-0.7.9/.github/workflows/pypi.yaml` & `tables_io-0.8.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/.github/workflows/python-package.yml` & `tables_io-0.8.0/.github/workflows/python-package.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Python package
 
 on:
   push:
-    branches: [ main ]
+    branches: [main]
   pull_request:
-    branches: [ main ]
+    branches: [main]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
+    defaults:
+      run:
+        shell: bash -l {0}
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9]
+        python-version: [3.8, 3.9, "3.10"]
 
     steps:
     - uses: actions/checkout@v2
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+    - uses: conda-incubator/setup-miniconda@v2
       with:
         python-version: ${{ matrix.python-version }}
+        channels: conda-forge,defaults
+        channel-priority: strict
+        show-channel-urls: true
+        miniforge-version: latest
+        miniforge-variant: Mambaforge
+        use-mamba: true
+        environment-file: environment.yml
+        activate-environment: tables_io
     - name: Install dependencies
       run: |
-        sudo apt install -y libopenmpi-dev libhdf5-mpi-dev
-        python -m pip install --upgrade pip
-        python -m pip install pylint pytest pytest-cov
-        python -m pip install jupyter
-        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-        CC="mpicc" HDF5_MPI="ON" pip install --upgrade --force-reinstall --no-binary=h5py h5py
-        python setup.py install
-      env:
-        CC: mpicc
-        HDF5_MPI: ON
+        pip install --no-deps .
     - name: Lint with pylint
       run: |
+        # stop the build if there are Pylint errors
+        pylint --disable=all --extension-pkg-whitelist=numpy --init-hook='import sys; sys.setrecursionlimit(8 * sys.getrecursionlimit())' src/tables_io
+    - name: Lint with flake8
+      run: |
         # stop the build if there are Python syntax errors or undefined names
-        pylint --reports=no --errors-only tables_io
-        # stp the build if there are a lot of messages
-        pylint --reports=no --fail-under=9.5 tables_io
-        # exit-zero treats all errors as warnings.
-        pylint --exit-zero tables_io
+        flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
+        # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
+        flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
     - name: Test with pytest
       run: |
-        python -m pytest --cov=./tables_io --cov-report=xml tests
+        python -m pytest --cov-report=xml tests
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v1
       with:
         file: ./coverage.xml
         flags: unittests
         env_vars: OS,PYTHON
         name: codecov-umbrella
```

### Comparing `tables_io-0.7.9/.gitignore` & `tables_io-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/LICENSE` & `tables_io-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/docs/.gitignore` & `tables_io-0.8.0/docs/.gitignore`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/docs/Makefile` & `tables_io-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/docs/conf.py` & `tables_io-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/docs/index.rst` & `tables_io-0.8.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 4. 'HDF5', as used to store pandas dataframes, e.g., as produced by: 
 
 .. code-block:: python
 		
     df.to_hdf(filepath, key)
 
     
-5. 'parquet', as used to store pandas datafames, e.g., as produced by:
+5. 'parquet' ('parq' or 'pq' are also valid file suffixes), as used to store pandas datafames, e.g., as produced by:
 
    
 .. code-block:: python
 		
     df.to_parquet(filepath)
```

### Comparing `tables_io-0.7.9/docs/tables_io.rst` & `tables_io-0.8.0/docs/tables_io.rst`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/nb/.gitignore` & `tables_io-0.8.0/nb/.gitignore`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/nb/hdf5_iter_example.ipynb` & `tables_io-0.8.0/nb/hdf5_iter_example.ipynb`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/nb/multipleWriteHdf5_example.ipynb` & `tables_io-0.8.0/nb/multipleWriteHdf5_example.ipynb`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/nb/singleTable_example.ipynb` & `tables_io-0.8.0/nb/singleTable_example.ipynb`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/nb/tableDict_example.ipynb` & `tables_io-0.8.0/nb/tableDict_example.ipynb`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/tables_io/__init__.py` & `tables_io-0.8.0/src/tables_io/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """tables_io is a library of functions for input, output and conversion of tabular data formats"""
 
 try:
     from ._version import version
 except:  #pylint: disable=bare-except   #pragma: no cover
-    version = "unknown"  
+    version = "unknown"
 
 from .lazy_modules import *
 
 from . import types
 
 from . import arrayUtils
```

### Comparing `tables_io-0.7.9/tables_io/arrayUtils.py` & `tables_io-0.8.0/src/tables_io/arrayUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,17 @@
     should be the same length
     """
     firstkey = list(hg.keys())[0]
     nrows = len(hg[firstkey])
     firstname = hg[firstkey].name
     for value in hg.values():
         if len(value) != nrows:
-            raise ValueError(f"Group does not represent a table. Length ({len(value)}) of column {value.name} not not match length ({nrows}) of first column {firstname}")
+            raise ValueError(f"Group does not represent a table. Length ({len(value)})"
+                             f"of column {value.name} not not match length ({nrows}) of"
+                             f"first column {firstname}")
     return nrows
 
 
 def getInitializationForODict(in_dict, nRow_out=None):
     """ shape of arrays and dtypes in a dictionary.
     This is useful for initialize hdf5 files
```

### Comparing `tables_io-0.7.9/tables_io/convUtils.py` & `tables_io-0.8.0/src/tables_io/convUtils.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/tables_io/ioUtils.py` & `tables_io-0.8.0/src/tables_io/ioUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     """
     hg, infp = readHdf5Group(filepath, groupname)
     nrow = getGroupInputDataLength(hg)
     infp.close()
     return nrow
 
 
-def initializeHdf5WriteSingle(filepath, groupname=None, **kwds):
+def initializeHdf5WriteSingle(filepath, groupname=None, comm=None, **kwds):
     """ Prepares an hdf5 file for output
 
     Parameters
     ----------
     filepath : `str`
         The output file name
     groupname : `str` or `None`
@@ -109,22 +109,27 @@
     `initializeHdf5WriteSingle('test.hdf5', data = dict(scalar=((100000,), 'f4'), vect=((100000, 3), 'f4'))`
     Would initialize an hdf5 file with two datasets, with shapes and data types as given
 
     """
     outdir = os.path.dirname(os.path.abspath(filepath))
     if not os.path.exists(outdir):  #pragma: no cover
         os.makedirs(outdir, exist_ok=True)
-    outf = h5py.File(filepath, "w")
+    if comm is None:
+        outf = h5py.File(filepath, "w")
+    else:
+        if not h5py.get_config().mpi:
+            raise TypeError("hdf5py module not prepared for parallel writing.") #pragma: no cover
+        outf = h5py.File(filepath, "w",driver='mpio', comm=comm)
     if groupname is None:
         group = outf
     else:
         group = outf.create_group(groupname)
     for key, shape in kwds.items():
         group.create_dataset(key, shape[0], shape[1])
-    return group, outf        
+    return group, outf
 
 
 def initializeHdf5Write(filepath, comm=None, **kwds):
     """ Prepares an hdf5 file for output
 
     Parameters
     ----------
@@ -142,15 +147,15 @@
 
     Notes
     -----
     The keywords should be used to create groups within the hdf5 file.
     Each keyword should provide a dictionary with the data set information of the form:
      group = {'data1' : ( (shape1), (dtype1) ), 'data2' : ( (shape2), (dtype2) )}
 
-    group : `str` 
+    group : `str`
         Name of the Hdf5 group
     data  : `str`
         Name of the column to be written
     shape : `tuple` ( `int` )
         The shape of the data for this dataset
     dtype : `str`
         The data type for this dataset
@@ -159,19 +164,19 @@
     `initializeHdf5Write('test.hdf5', data = dict(scalar=((100000,), 'f4'), vect=((100000, 3), 'f4'))`
 
     Would initialize an hdf5 file with one group and two datasets, with shapes and data types as given
     """
     outdir = os.path.dirname(os.path.abspath(filepath))
     if not os.path.exists(outdir):  #pragma: no cover
         os.makedirs(outdir, exist_ok=True)
-    if comm == None:
+    if comm is None:
         outf = h5py.File(filepath, "w")
     else:
         if not h5py.get_config().mpi:
-            raise TypeError(f"hdf5py module not prepared for parallel writing.") #pragma: no cover
+            raise TypeError("hdf5py module not prepared for parallel writing.") #pragma: no cover
         outf = h5py.File(filepath, "w",driver='mpio', comm=comm)
     groups = {}
     for k, v in kwds.items():
         group = outf.create_group(k)
         groups[k] = group
         for key, shape in v.items():
             group.create_dataset(key, shape[0], shape[1])
@@ -208,15 +213,15 @@
 
     I.e., if `key` is present in kwds in will override the name.
     """
     for key, val in odict.items():
         k_out = kwds.get(key, key)
         fout[k_out][start:end] = val
 
-        
+
 def writeDictToHdf5Chunk(groups, odict, start, end, **kwds):
     """ Writes a data chunk to an hdf5 file
 
     Parameters
     ----------
     fout : `h5py.File`
         The file
@@ -273,15 +278,15 @@
 def split_tasks_by_rank(tasks, parallel_size, rank):
     """Iterate through a list of items, yielding ones this process is responsible for/
 
     Tasks are allocated in a round-robin way.
 
     Parameters
     ----------
-        tasks: Tasks to split up (iterator)  
+        tasks: Tasks to split up (iterator)
         parallel_size: the number of processes under MPI (int)
         rank: the rank of this process under MPI (int)
 
     Returns
         output: number of the first task for this process (iterator)
     """
     for i, task in enumerate(tasks):
@@ -335,15 +340,16 @@
 
     Currently only implemented for hdf5, returns `tuple`
         start: start index (int)
         end: ending index (int)
         data: dictionary of all data from start:end (dict)
     """
     if rank>=parallel_size:
-        raise TypeError(f"MPI rank {rank} larger than the total number of processes {parallel_size}") #pragma: no cover
+        raise TypeError(f"MPI rank {rank} larger than the total "
+                        f"number of processes {parallel_size}") #pragma: no cover
     f, infp = readHdf5Group(filepath, groupname)
     num_rows = getGroupInputDataLength(f)
     ranges = data_ranges_by_rank(num_rows, chunk_size, parallel_size, rank)
     data = OrderedDict()
     for start, end in ranges:
         for key, val in f.items():
             data[key] = readHdf5DatasetToArray(val, start, end)
@@ -583,19 +589,20 @@
     if isinstance(hg, h5py.Dataset):
         return readHdf5DatasetToArray(hg, start, end)
     return OrderedDict([(key, readHdf5DatasetToArray(val, start, end)) for key, val in hg.items()])
 
 
 def writeDictToHdf5(odict, filepath, groupname, **kwargs):
     """
-    Writes a dictionary of `numpy.array` to a single hdf5 file
+    Writes a dictionary of `numpy.array` or `jaxlib.xla_extension.DeviceArray`
+    to a single hdf5 file
 
     Parameters
     ----------
-    odict : `Mapping`, (`str`, `numpy.array`)
+    odict : `Mapping`, (`str`, `numpy.array` or `jaxlib.xla_extension.DeviceArray`)
         The data being written
 
     filepath: `str`
         Path to output file
 
     groupname : `str` or `None`
         The groupname for the data
@@ -604,15 +611,22 @@
     fout = h5py.File(filepath, 'a')
     if groupname is None:  #pragma: no cover
         group = fout
     else:
         group = fout.create_group(groupname)
     for key, val in odict.items():
         try:
-            group.create_dataset(key, dtype=val.dtype, data=val.data)
+            if isinstance(val, np.ndarray):
+                group.create_dataset(key, dtype=val.dtype, data=val.data)
+            else:
+                # In the future, it may be better to specifically case for
+                # jaxlib.xla_extension.DeviceArray here. For now, we're
+                # resorting to duck typing so we don't have to import jax just
+                # to check the type.
+                group.create_dataset(key, dtype=val.dtype, data=val.device_buffer)
         except Exception as msg:  #pragma: no cover
             print(f"Warning.  Failed to convert column {str(msg)}")
     fout.close()
 
 
 def writeDictsToHdf5(odicts, filepath):
     """
@@ -979,15 +993,17 @@
                 PANDAS_HDF5:iterH5ToDataFrame,
                 PANDAS_PARQUET:iterPqToDataFrame}
 
     try:
         theFunc = funcDict[fType]
         return theFunc(filepath, **kwargs)
     except KeyError as msg:
-        raise NotImplementedError(f"Unsupported FileType for iterateNative {fType}") from msg #pragma: no cover
+        raise NotImplementedError(
+            f"Unsupported FileType for iterateNative {fType}"
+        ) from msg #pragma: no cover
 
 
 def iterator(filepath, tType=None, fmt=None, **kwargs):
     """ Read a file to the corresponding table type iterate over the file
 
     Parameters
     ----------
```

### Comparing `tables_io-0.7.9/tables_io/lazy_modules.py` & `tables_io-0.8.0/src/tables_io/lazy_modules.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ Lazy loading modules """
 
-import sys
 import importlib
 
 class LazyModule:
     """
     A partial implementation of a lazily imported module.
 
     This isn't a general solution, since it doesn't actually
@@ -18,16 +17,16 @@
 
     @property
     def module(self):
         if self._module is not None:
             return self._module
         try:
             self._module = importlib.import_module(self.name)
-        except ImportError:
-            raise ImportError("Cannot use selected data format, {self.modulename} not available")
+        except ImportError as err:
+            raise ImportError(f"Cannot use selected data format, {self.name} not available") from err
 
         return self._module
 
 
     def __dir__(self):
         """
         Get the attributes of the module, to support tab-autocomplete.
@@ -45,11 +44,13 @@
     """
     return LazyModule(modulename)
 
 
 
 tables = lazyImport('tables')
 apTable = lazyImport('astropy.table')
+apDiffUtils = lazyImport('astropy.utils.diff')
 fits = lazyImport('astropy.io.fits')
 h5py = lazyImport('h5py')
 pd = lazyImport('pandas')
 pq = lazyImport('pyarrow.parquet')
+jnp = lazyImport('jax.numpy')
```

### Comparing `tables_io-0.7.9/tables_io/tableDict.py` & `tables_io-0.8.0/src/tables_io/tableDict.py`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/tables_io/testUtils.py` & `tables_io-0.8.0/src/tables_io/testUtils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 """
 Utilities for testing
 """
-
+import sys
 import numpy as np
-from astropy.table import Table as apTable
-from astropy.utils.diff import report_diff_values
+from tables_io.lazy_modules import tables, apTable, apDiffUtils, fits, h5py, pd, pq, jnp
+
+
+def check_deps(deps=None):
+    missing = False
+    if deps is None:  #pragma: no cover
+        deps = [tables, apTable, apDiffUtils, fits, h5py, pd, pq, jnp]
+    for mod in deps:
+        try:
+            _ = mod.__file__
+        except Exception as err:  #pylint: disable=broad-exception-caught
+            sys.stderr.write(f"Missing {err}")
+            missing = True
+    return not missing
 
 
 def compare_tables(t1, t2):
     """ Compare all the tables in two `astropy.table.Table`)
 
     Parameters
     ----------
@@ -54,30 +66,30 @@
     identical = True
     for k, v in d1.items():
         try:
             vv = d2[k]
         except KeyError:  #pragma: no cover
             vv = d2[k.upper()]
         if strict:  #pragma: no cover
-            identical &= report_diff_values(v, vv)
+            identical &= apDiffUtils.report_diff_values(v, vv)
         else:  #pragma: no cover
             identical &= compare_tables(v, vv)
     return identical
 
 
 def make_test_data():
     """ Make and return some test data """
     nrow = 1000
     vect_size = 20
     mat_size = 5
     scalar = np.random.uniform(size=nrow)
     vect = np.random.uniform(size=nrow*vect_size).reshape(nrow, vect_size)
     matrix = np.random.uniform(size=nrow*mat_size*mat_size).reshape(nrow, mat_size, mat_size)
     data = dict(scalar=scalar, vect=vect, matrix=matrix)
-    table = apTable(data)
+    table = apTable.Table(data)
     table.meta['a'] = 1
     table.meta['b'] = None
     table.meta['c'] = [3, 4, 5]
-    small_table = apTable(dict(a=np.ones(21), b=np.zeros(21)))
+    small_table = apTable.Table(dict(a=np.ones(21), b=np.zeros(21)))
     small_table.meta['small'] = True
-    tables = dict(data=table, md=small_table)
-    return tables
+    out_tables = dict(data=table, md=small_table)
+    return out_tables
```

### Comparing `tables_io-0.7.9/tables_io/types.py` & `tables_io-0.8.0/src/tables_io/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,22 +43,26 @@
 # Default suffixes for various file formats
 FILE_FORMAT_SUFFIXS = OrderedDict([
     ('fits', ASTROPY_FITS),
     ('hf5', ASTROPY_HDF5),
     ('hdf5', NUMPY_HDF5),
     ('fit', NUMPY_FITS),
     ('h5', PANDAS_HDF5),
+    ('parquet', PANDAS_PARQUET),
+    ('parq', PANDAS_PARQUET),
     ('pq', PANDAS_PARQUET)])
 
 DEFAULT_TABLE_KEY = OrderedDict([
     ('fits', ''),
     ('hf5', None),
     ('hdf5', None),
     ('fit', ''),
     ('h5', 'data'),
+    ('parquet', ''),
+    ('parq', ''),
     ('pq', '')])
 
 FILE_FORMATS = OrderedDict([(val, key) for key, val in FILE_FORMAT_NAMES.items()])
 
 FILE_FORMAT_SUFFIX_MAP = OrderedDict([(val, key) for key, val in FILE_FORMAT_SUFFIXS.items()])
 
 # Default format to write various table types
```

### Comparing `tables_io-0.7.9/tables_io.egg-info/SOURCES.txt` & `tables_io-0.8.0/src/tables_io.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-.coveragerc
+.flake8
 .gitignore
-.pylintrc
 LICENSE
 README.md
-do_cover.sh
-requirements.txt
+environment.yml
+pyproject.toml
 setup.py
 .github/workflows/pypi.yaml
 .github/workflows/python-package.yml
 docs/.gitignore
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/install.rst
 docs/tables_io.rst
 nb/.gitignore
 nb/hdf5_iter_example.ipynb
 nb/multipleWriteHdf5_example.ipynb
 nb/singleTable_example.ipynb
 nb/tableDict_example.ipynb
-tables_io/__init__.py
-tables_io/_version.py
-tables_io/arrayUtils.py
-tables_io/convUtils.py
-tables_io/ioUtils.py
-tables_io/lazy_modules.py
-tables_io/tableDict.py
-tables_io/testUtils.py
-tables_io/types.py
-tables_io.egg-info/PKG-INFO
-tables_io.egg-info/SOURCES.txt
-tables_io.egg-info/dependency_links.txt
-tables_io.egg-info/requires.txt
-tables_io.egg-info/top_level.txt
+src/tables_io/__init__.py
+src/tables_io/_version.py
+src/tables_io/arrayUtils.py
+src/tables_io/convUtils.py
+src/tables_io/ioUtils.py
+src/tables_io/lazy_modules.py
+src/tables_io/tableDict.py
+src/tables_io/testUtils.py
+src/tables_io/types.py
+src/tables_io.egg-info/PKG-INFO
+src/tables_io.egg-info/SOURCES.txt
+src/tables_io.egg-info/dependency_links.txt
+src/tables_io.egg-info/requires.txt
+src/tables_io.egg-info/top_level.txt
 tests/test_conv.py
 tests/test_fileIO.py
 tests/test_io.py
 tests/test_table_dict.py
 tests/test_utils.py
 tests/data/no_groupname_test.hdf5
 tests/data/pandas_test_hdf5.h5
```

### Comparing `tables_io-0.7.9/tests/data/no_groupname_test.hdf5` & `tables_io-0.8.0/tests/data/no_groupname_test.hdf5`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/tests/data/pandas_test_hdf5.h5` & `tables_io-0.8.0/tests/data/pandas_test_hdf5.h5`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/tests/data/parquet_test.parquet` & `tables_io-0.8.0/tests/data/parquet_test.parquet`

 * *Files identical despite different names*

### Comparing `tables_io-0.7.9/tests/test_conv.py` & `tables_io-0.8.0/tests/test_conv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 """
 Unit tests for io_layer module
 """
 
 import unittest
+import pytest
 from tables_io import types, convert, convertObj
-from tables_io.testUtils import compare_table_dicts, make_test_data
+from tables_io.testUtils import compare_table_dicts, make_test_data, check_deps
+from tables_io.lazy_modules import tables, apTable, apDiffUtils, fits, h5py, pd, pq, jnp
 
 
+def test_deps():
+    assert check_deps([tables, apTable, apDiffUtils, fits, h5py, pd, pq, jnp])    
+    dummy = 0
+    assert not check_deps([dummy])
+
+
+@pytest.mark.skipif(not check_deps([apTable, pd]), reason="Missing panda or astropy.table")
 class ConvTestCase(unittest.TestCase):  #pylint: disable=too-many-instance-attributes
     """ Test the utility functions """
 
     def setUp(self):
         """
         Make any objects that are used in multiple tests.
         """
```

### Comparing `tables_io-0.7.9/tests/test_io.py` & `tables_io-0.8.0/tests/test_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 Unit tests for io_layer module
 """
 
 import os
+import pytest
 
 import unittest
 from tables_io import types, convert, io_open, read, write, iterator
-from tables_io.testUtils import compare_table_dicts, compare_tables, make_test_data
-from tables_io.lazy_modules import apTable
+from tables_io.testUtils import compare_table_dicts, compare_tables, make_test_data, check_deps
+from tables_io.lazy_modules import apTable, jnp, h5py, pq
 
 
+@pytest.mark.skipif(not check_deps([apTable, h5py, pq, jnp]), reason="Missing an IO package")
 class IoTestCase(unittest.TestCase):  #pylint: disable=too-many-instance-attributes
     """ Test the utility functions """
 
     def setUp(self):
         """
         Make any objects that are used in multiple tests.
         """
@@ -36,14 +38,29 @@
         else:
             for key in keys:
                 self._files.append("%s%s.%s" % (basepath, key, fmt))
         odict_r = read(filepath, tType=tType, fmt=fmt, keys=keys)
         tables_r = convert(odict_r, types.AP_TABLE)
         assert compare_table_dicts(self._tables, tables_r)
 
+    def _do_loopback_jax(self, basepath, fmt, keys=None):
+        """ Utility function to do loopback tests writing data as a jax array """
+        odict_c = convert(self._tables, types.NUMPY_DICT)
+        for key, val in odict_c["data"].items():
+            odict_c["data"][key] = jnp.array(val)
+        filepath = write(odict_c, basepath, fmt)
+        if keys is None:
+            self._files.append(filepath)
+        else:
+            for key in keys:
+                self._files.append("%s%s.%s" % (basepath, key, fmt))
+        odict_r = read(filepath, tType=types.NUMPY_DICT, fmt=fmt, keys=keys)
+        tables_r = convert(odict_r, types.AP_TABLE)
+        assert compare_table_dicts(self._tables, tables_r)
+
     def _do_loopback_single(self, tType, basepath, fmt, keys=None):
         """ Utility function to do loopback tests """
         obj_c = convert(self._table, tType)
         filepath = write(obj_c, basepath, fmt)
         try:
             os.unlink(filepath)
         except FileNotFoundError:
@@ -122,14 +139,18 @@
     def testHdf5Loopback(self):
         """ Test writing / reading numpy arrays to HDF5 """
         self._do_loopback(types.NUMPY_DICT, 'test_out', 'hdf5')
         self._do_loopback_single(types.NUMPY_DICT, 'test_out_single', 'hdf5')
         self._do_iterator('test_out_single.hdf5', types.NUMPY_DICT, False, chunk_size=50)
         self._do_open('test_out_single.hdf5')
         self._do_open('test_out.hdf5')
+
+    def testHdf5LoopbackWithJaxArray(self):
+        """ Test writing / reading astropy tables to HDF5 with a jax array """
+        self._do_loopback_jax('test_out', 'hdf5')
         
     def testH5Loopback(self):
         """ Test writing / reading pandas dataframes to HDF5 """
         self._do_loopback(types.PD_DATAFRAME, 'test_out', 'h5')
         self._do_loopback_single(types.PD_DATAFRAME, 'test_out_single', 'h5')
         self._do_iterator('test_out_single.h5', types.PD_DATAFRAME, True, chunk_size=50)
         self._do_open('test_out_single.h5')
```

### Comparing `tables_io-0.7.9/tests/test_table_dict.py` & `tables_io-0.8.0/tests/test_table_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Unit tests for io_layer module
 """
 
 import os
+import pytest
 
 import unittest
 
 from tables_io import types, convert, TableDict
-from tables_io.testUtils import compare_table_dicts, make_test_data
+from tables_io.testUtils import compare_table_dicts, make_test_data, check_deps
+from tables_io.lazy_modules import apTable, jnp, h5py, pq
 
 
+@pytest.mark.skipif(not check_deps([apTable, h5py, pq, jnp]), reason="Missing an IO package")
 class TableDictTestCase(unittest.TestCase):  #pylint: disable=too-many-instance-attributes
     """ Test the utility functions """
 
     def setUp(self):
         """
         Make any objects that are used in multiple tests.
         """
```

### Comparing `tables_io-0.7.9/tests/test_utils.py` & `tables_io-0.8.0/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """ Unit tests for the fileIO module """
 
 import numpy as np
 import sys
+import pytest
 import unittest
 from tables_io import arrayUtils, types
-from tables_io.lazy_modules import lazyImport
+from tables_io.testUtils import check_deps
+from tables_io.lazy_modules import lazyImport, apTable, pd
 
 
 def test_array_length():
     """ Test the pandas reading """
     assert arrayUtils.arrayLength(4) == 0
     assert arrayUtils.arrayLength(np.ones(5)) == 5
     assert arrayUtils.arrayLength(np.ones((5, 5, 5))) == 5
@@ -102,14 +104,16 @@
     try:
         types.fileType('xx.out')
     except KeyError:
         pass
     else:
         raise KeyError("Failed to catch unknown fileType")
 
+
+@pytest.mark.skipif(not check_deps([apTable, pd]), reason="Missing an IO package")
 def test_type_finders():
     """ Test the utils that identify apTables and data frames """
     import pandas as pd
     from astropy.table import Table
 
     class DataFrameSub(pd.DataFrame):
         pass
```

