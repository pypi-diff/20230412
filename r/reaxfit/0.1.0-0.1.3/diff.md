# Comparing `tmp/reaxfit-0.1.0.tar.gz` & `tmp/reaxfit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaxfit-0.1.0.tar", last modified: Fri Mar  3 07:37:25 2023, max compression
+gzip compressed data, was "reaxfit-0.1.3.tar", last modified: Wed Apr 12 05:04:43 2023, max compression
```

## Comparing `reaxfit-0.1.0.tar` & `reaxfit-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-03-03 07:37:25.060122 reaxfit-0.1.0/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-03-03 07:37:25.056123 reaxfit-0.1.0/.github/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       48 2023-03-03 06:38:54.000000 reaxfit-0.1.0/.github/release.yml
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-03-03 07:37:25.056123 reaxfit-0.1.0/.github/workflows/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      251 2023-03-03 06:38:54.000000 reaxfit-0.1.0/.github/workflows/tagpr.yml
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      111 2023-03-03 07:37:02.000000 reaxfit-0.1.0/.gitignore
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     1794 2023-03-03 06:38:54.000000 reaxfit-0.1.0/.tagpr
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     1067 2023-03-01 01:38:22.000000 reaxfit-0.1.0/LICENSE
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      953 2023-03-03 07:37:25.060122 reaxfit-0.1.0/PKG-INFO
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      720 2023-03-03 03:25:12.000000 reaxfit-0.1.0/README.md
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-03-03 07:37:25.056123 reaxfit-0.1.0/example/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-03-03 07:37:25.056123 reaxfit-0.1.0/example/CoCO/
--rw-r--r--   0 ykane     (1000) ykane     (1000)     1892 2023-02-22 04:48:36.000000 reaxfit-0.1.0/example/CoCO/0.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2151 2023-02-22 04:48:36.000000 reaxfit-0.1.0/example/CoCO/1.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.0/example/CoCO/2.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.0/example/CoCO/3.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.1.0/example/CoCO/4.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.0/example/CoCO/5.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.1.0/example/CoCO/6.xyz
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      189 2023-02-28 13:43:09.000000 reaxfit-0.1.0/example/CoCO/batch.sh
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      374 2023-02-28 13:52:46.000000 reaxfit-0.1.0/example/CoCO/chk.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      260 2023-03-03 02:56:27.000000 reaxfit-0.1.0/example/CoCO/config.json
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2310 2023-02-22 04:48:36.000000 reaxfit-0.1.0/example/CoCO/data0
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    22677 2023-03-02 14:08:20.000000 reaxfit-0.1.0/example/CoCO/ffield.temp
--rw-r--r--   0 ykane     (1000) ykane     (1000)       58 2023-02-22 04:48:36.000000 reaxfit-0.1.0/example/CoCO/refE
--rw-r--r--   0 ykane     (1000) ykane     (1000)       56 2023-02-22 04:48:36.000000 reaxfit-0.1.0/example/CoCO/refF
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      127 2023-02-28 13:40:22.000000 reaxfit-0.1.0/example/CoCO/run.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      235 2023-03-01 02:14:34.000000 reaxfit-0.1.0/example/README.md
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    56339 2023-03-03 03:15:10.000000 reaxfit-0.1.0/reaxfit_sample.ipynb
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       38 2023-03-03 07:37:25.060122 reaxfit-0.1.0/setup.cfg
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      722 2023-03-03 07:37:02.000000 reaxfit-0.1.0/setup.py
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-03-03 07:37:25.056123 reaxfit-0.1.0/src/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-03-03 07:37:25.060122 reaxfit-0.1.0/src/reaxfit/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       30 2023-02-22 05:23:36.000000 reaxfit-0.1.0/src/reaxfit/__init__.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      160 2023-03-03 07:37:02.000000 reaxfit-0.1.0/src/reaxfit/_version.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     5952 2023-03-03 02:20:33.000000 reaxfit-0.1.0/src/reaxfit/reaxfit.py
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-03-03 07:37:25.060122 reaxfit-0.1.0/src/reaxfit.egg-info/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      953 2023-03-03 07:37:24.000000 reaxfit-0.1.0/src/reaxfit.egg-info/PKG-INFO
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      676 2023-03-03 07:37:25.000000 reaxfit-0.1.0/src/reaxfit.egg-info/SOURCES.txt
--rw-rw-r--   0 ykane     (1000) ykane     (1000)        1 2023-03-03 07:37:24.000000 reaxfit-0.1.0/src/reaxfit.egg-info/dependency_links.txt
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       19 2023-03-03 07:37:24.000000 reaxfit-0.1.0/src/reaxfit.egg-info/requires.txt
--rw-rw-r--   0 ykane     (1000) ykane     (1000)        8 2023-03-03 07:37:24.000000 reaxfit-0.1.0/src/reaxfit.egg-info/top_level.txt
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.049054 reaxfit-0.1.3/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.045054 reaxfit-0.1.3/.github/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       48 2023-03-03 06:38:54.000000 reaxfit-0.1.3/.github/release.yml
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.045054 reaxfit-0.1.3/.github/workflows/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      251 2023-03-03 06:38:54.000000 reaxfit-0.1.3/.github/workflows/tagpr.yml
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      111 2023-04-12 04:40:21.000000 reaxfit-0.1.3/.gitignore
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     1794 2023-03-03 06:38:54.000000 reaxfit-0.1.3/.tagpr
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     1067 2023-03-01 01:38:22.000000 reaxfit-0.1.3/LICENSE
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      796 2023-04-12 05:04:43.049054 reaxfit-0.1.3/PKG-INFO
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      543 2023-04-12 04:40:21.000000 reaxfit-0.1.3/README.md
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.045054 reaxfit-0.1.3/example/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.049054 reaxfit-0.1.3/example/CoCO/
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     1892 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/0.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2151 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/1.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/2.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/3.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/4.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/5.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/6.xyz
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      189 2023-02-28 13:43:09.000000 reaxfit-0.1.3/example/CoCO/batch.sh
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      374 2023-02-28 13:52:46.000000 reaxfit-0.1.3/example/CoCO/chk.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      260 2023-03-03 02:56:27.000000 reaxfit-0.1.3/example/CoCO/config.json
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2310 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/data0
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    22606 2023-04-12 04:40:21.000000 reaxfit-0.1.3/example/CoCO/ffield.reax
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    22677 2023-03-02 14:08:20.000000 reaxfit-0.1.3/example/CoCO/ffield.temp
+-rw-r--r--   0 ykane     (1000) ykane     (1000)       58 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/refE
+-rw-r--r--   0 ykane     (1000) ykane     (1000)       56 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/refF
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      127 2023-02-28 13:40:22.000000 reaxfit-0.1.3/example/CoCO/run.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      235 2023-03-01 02:14:34.000000 reaxfit-0.1.3/example/README.md
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    61858 2023-04-12 04:40:21.000000 reaxfit-0.1.3/reaxfit_sample.ipynb
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       38 2023-04-12 05:04:43.049054 reaxfit-0.1.3/setup.cfg
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      723 2023-04-12 04:40:21.000000 reaxfit-0.1.3/setup.py
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.045054 reaxfit-0.1.3/src/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.049054 reaxfit-0.1.3/src/reaxfit/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       30 2023-02-22 05:23:36.000000 reaxfit-0.1.3/src/reaxfit/__init__.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      160 2023-03-03 07:37:02.000000 reaxfit-0.1.3/src/reaxfit/_version.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     5952 2023-03-03 02:20:33.000000 reaxfit-0.1.3/src/reaxfit/reaxfit.py
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.049054 reaxfit-0.1.3/src/reaxfit.egg-info/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      796 2023-04-12 05:04:42.000000 reaxfit-0.1.3/src/reaxfit.egg-info/PKG-INFO
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      667 2023-04-12 05:04:42.000000 reaxfit-0.1.3/src/reaxfit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)        1 2023-04-12 05:04:42.000000 reaxfit-0.1.3/src/reaxfit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)        8 2023-04-12 05:04:42.000000 reaxfit-0.1.3/src/reaxfit.egg-info/top_level.txt
```

### Comparing `reaxfit-0.1.0/.tagpr` & `reaxfit-0.1.3/.tagpr`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.0/LICENSE` & `reaxfit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.0/PKG-INFO` & `reaxfit-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: reaxfit
-Version: 0.1.0
+Version: 0.1.3
 Summary: parameter fitting for ReaxFF
 Home-page: https://github.com/ykanematsu/reaxfit
 Author: ykanematsu
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ReaxFit
 Parameter-fitting module for lammps-reaxff with differential_evolution of scipy.
 ## Requirements
 - lammps (library)
 - numpy
 - scipy
 ## Install
 - use anaconda
 ```sh
 conda install -c conda-forge lammps
 conda install scipy numpy
-pip3 install git+https://github.com/ykanematsu/reaxfit.git
+pip3 install reaxfit
 ```
-- [option] install lammps from source code
+- [option] install jupyterlab and ase
+It will be convenient to use reaxff with jupyterlab and ase.
 ```sh
-mkdir build
-cd build
-cmake ../cmake -DLAMMPS_EXCEPTIONS=yes -DBUILD_SHARED_LIBS=yes -DMLIAP_ENABLE_PYTHON=yes -DPKG_PYTHON=yes -DPKG_MANYBODY=yes -DPKG_REAXFF=yes -DPYTHON_EXECUTABLE:FILEPATH=`which python3`
-make -j4
-make install-python
+conda install -c conda-forge jupyterlab ase
 ```
 ## Useage 
-- See [A sample on colab](https://colab.research.google.com/github/ykanematsu/reaxfit/blob/master/reaxfit_sample.ipynb)
+- See [A sample on colab](https://colab.research.google.com/github/ykanematsu/reaxfit/blob/main/reaxfit_sample.ipynb)
+
+
```

### Comparing `reaxfit-0.1.0/example/CoCO/0.xyz` & `reaxfit-0.1.3/example/CoCO/0.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.0/example/CoCO/1.xyz` & `reaxfit-0.1.3/example/CoCO/1.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.0/example/CoCO/2.xyz` & `reaxfit-0.1.3/example/CoCO/2.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.0/example/CoCO/3.xyz` & `reaxfit-0.1.3/example/CoCO/3.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.0/example/CoCO/4.xyz` & `reaxfit-0.1.3/example/CoCO/4.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.0/example/CoCO/5.xyz` & `reaxfit-0.1.3/example/CoCO/5.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.0/example/CoCO/6.xyz` & `reaxfit-0.1.3/example/CoCO/6.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.0/example/CoCO/data0` & `reaxfit-0.1.3/example/CoCO/data0`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.0/example/CoCO/ffield.temp` & `reaxfit-0.1.3/example/CoCO/ffield.temp`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.0/setup.py` & `reaxfit-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,11 +12,11 @@
         use_scm_version=True,
         setup_requires=["setuptools_scm"],
         license='MIT',
         url='https://github.com/ykanematsu/reaxfit',
         description='parameter fitting for ReaxFF',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        install_requires=["scipy","numpy","lammps"],
+        #install_requires=["scipy","numpy","lammps"],
         package_dir={"": "src"},
         packages=find_packages(where="src"),
 )
```

### Comparing `reaxfit-0.1.0/src/reaxfit/reaxfit.py` & `reaxfit-0.1.3/src/reaxfit/reaxfit.py`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.0/src/reaxfit.egg-info/PKG-INFO` & `reaxfit-0.1.3/src/reaxfit.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: reaxfit
-Version: 0.1.0
+Version: 0.1.3
 Summary: parameter fitting for ReaxFF
 Home-page: https://github.com/ykanematsu/reaxfit
 Author: ykanematsu
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ReaxFit
 Parameter-fitting module for lammps-reaxff with differential_evolution of scipy.
 ## Requirements
 - lammps (library)
 - numpy
 - scipy
 ## Install
 - use anaconda
 ```sh
 conda install -c conda-forge lammps
 conda install scipy numpy
-pip3 install git+https://github.com/ykanematsu/reaxfit.git
+pip3 install reaxfit
 ```
-- [option] install lammps from source code
+- [option] install jupyterlab and ase
+It will be convenient to use reaxff with jupyterlab and ase.
 ```sh
-mkdir build
-cd build
-cmake ../cmake -DLAMMPS_EXCEPTIONS=yes -DBUILD_SHARED_LIBS=yes -DMLIAP_ENABLE_PYTHON=yes -DPKG_PYTHON=yes -DPKG_MANYBODY=yes -DPKG_REAXFF=yes -DPYTHON_EXECUTABLE:FILEPATH=`which python3`
-make -j4
-make install-python
+conda install -c conda-forge jupyterlab ase
 ```
 ## Useage 
-- See [A sample on colab](https://colab.research.google.com/github/ykanematsu/reaxfit/blob/master/reaxfit_sample.ipynb)
+- See [A sample on colab](https://colab.research.google.com/github/ykanematsu/reaxfit/blob/main/reaxfit_sample.ipynb)
+
+
```

### Comparing `reaxfit-0.1.0/src/reaxfit.egg-info/SOURCES.txt` & `reaxfit-0.1.3/src/reaxfit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 example/CoCO/4.xyz
 example/CoCO/5.xyz
 example/CoCO/6.xyz
 example/CoCO/batch.sh
 example/CoCO/chk.py
 example/CoCO/config.json
 example/CoCO/data0
+example/CoCO/ffield.reax
 example/CoCO/ffield.temp
 example/CoCO/refE
 example/CoCO/refF
 example/CoCO/run.py
 src/reaxfit/__init__.py
 src/reaxfit/_version.py
 src/reaxfit/reaxfit.py
 src/reaxfit.egg-info/PKG-INFO
 src/reaxfit.egg-info/SOURCES.txt
 src/reaxfit.egg-info/dependency_links.txt
-src/reaxfit.egg-info/requires.txt
 src/reaxfit.egg-info/top_level.txt
```

