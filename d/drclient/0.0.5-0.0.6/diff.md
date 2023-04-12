# Comparing `tmp/drclient-0.0.5.tar.gz` & `tmp/drclient-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drclient-0.0.5.tar", last modified: Mon Apr 10 15:01:24 2023, max compression
+gzip compressed data, was "drclient-0.0.6.tar", last modified: Wed Apr 12 20:28:45 2023, max compression
```

## Comparing `drclient-0.0.5.tar` & `drclient-0.0.6.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.542635 drclient-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.530635 drclient-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.538635 drclient-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-10 15:01:16.000000 drclient-0.0.5/.github/workflows/multi-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-10 15:01:16.000000 drclient-0.0.5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-10 15:01:16.000000 drclient-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 15:01:16.000000 drclient-0.0.5/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.538635 drclient-0.0.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-10 15:01:16.000000 drclient-0.0.5/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-10 15:01:16.000000 drclient-0.0.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 15:01:16.000000 drclient-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 15:01:16.000000 drclient-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-10 15:01:24.542635 drclient-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-10 15:01:16.000000 drclient-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.538635 drclient-0.0.5/drclient/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.542635 drclient-0.0.5/drclient/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/cli/cmd_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/cli/cmd_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/cli/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.542635 drclient-0.0.5/drclient/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/registry/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/registry/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/threaded_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.542635 drclient-0.0.5/drclient/view/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/view/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/view/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-10 15:01:16.000000 drclient-0.0.5/drclient/view/info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.538635 drclient-0.0.5/drclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 15:01:24.000000 drclient-0.0.5/drclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-10 15:01:16.000000 drclient-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 15:01:16.000000 drclient-0.0.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 15:01:16.000000 drclient-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-10 15:01:24.542635 drclient-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-10 15:01:16.000000 drclient-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:01:24.542635 drclient-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-10 15:01:16.000000 drclient-0.0.5/tests/test_image_url.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-10 15:01:16.000000 drclient-0.0.5/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-10 15:01:16.000000 drclient-0.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.167979 drclient-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.159979 drclient-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.163979 drclient-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-12 20:28:36.000000 drclient-0.0.6/.github/workflows/multi-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 20:28:36.000000 drclient-0.0.6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-12 20:28:36.000000 drclient-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-12 20:28:36.000000 drclient-0.0.6/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.163979 drclient-0.0.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-12 20:28:36.000000 drclient-0.0.6/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-12 20:28:36.000000 drclient-0.0.6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-12 20:28:36.000000 drclient-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 20:28:36.000000 drclient-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-12 20:28:45.167979 drclient-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-12 20:28:36.000000 drclient-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.163979 drclient-0.0.6/drclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.163979 drclient-0.0.6/drclient/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/cli/cmd_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/cli/cmd_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.163979 drclient-0.0.6/drclient/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/registry/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/registry/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/threaded_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 20:28:44.000000 drclient-0.0.6/drclient/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.167979 drclient-0.0.6/drclient/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/view/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/view/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-12 20:28:36.000000 drclient-0.0.6/drclient/view/info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.163979 drclient-0.0.6/drclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-12 20:28:45.000000 drclient-0.0.6/drclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-12 20:28:45.000000 drclient-0.0.6/drclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:28:45.000000 drclient-0.0.6/drclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 20:28:45.000000 drclient-0.0.6/drclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 20:28:45.000000 drclient-0.0.6/drclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 20:28:45.000000 drclient-0.0.6/drclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-12 20:28:36.000000 drclient-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 20:28:36.000000 drclient-0.0.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 20:28:36.000000 drclient-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-12 20:28:45.167979 drclient-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 20:28:36.000000 drclient-0.0.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-12 20:28:36.000000 drclient-0.0.6/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:28:45.167979 drclient-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-12 20:28:36.000000 drclient-0.0.6/tests/test_image_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 20:28:36.000000 drclient-0.0.6/tests/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 20:28:36.000000 drclient-0.0.6/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-12 20:28:36.000000 drclient-0.0.6/tox.ini
```

### Comparing `drclient-0.0.5/.github/workflows/multi-test.yaml` & `drclient-0.0.6/.github/workflows/multi-test.yaml`

 * *Files identical despite different names*

### Comparing `drclient-0.0.5/.github/workflows/release.yaml` & `drclient-0.0.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `drclient-0.0.5/.gitignore` & `drclient-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `drclient-0.0.5/.pre-commit-config.yaml` & `drclient-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `drclient-0.0.5/LICENSE` & `drclient-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drclient-0.0.5/PKG-INFO` & `drclient-0.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: drclient
-Version: 0.0.5
-Summary: A docker registry client command line utility and Python library
-Home-page: https://github.com/joaompinto/drclient
-Author: João Pinto
-Author-email: lamego.pinto@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # drclient
 A docker registry client command line utility and Python library
 
 [![PyPi](https://img.shields.io/pypi/v/drclient.svg?style=flat-square)](https://pypi.python.org/pypi/drclient)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `drclient-0.0.5/README.md` & `drclient-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: drclient
+Version: 0.0.6
+Summary: A docker registry client command line utility and Python library
+Home-page: https://github.com/joaompinto/drclient
+Author: João Pinto
+Author-email: lamego.pinto@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # drclient
 A docker registry client command line utility and Python library
 
 [![PyPi](https://img.shields.io/pypi/v/drclient.svg?style=flat-square)](https://pypi.python.org/pypi/drclient)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `drclient-0.0.5/drclient/cli/cmd_info.py` & `drclient-0.0.6/drclient/cli/cmd_info.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.5/drclient/cli/cmd_pull.py` & `drclient-0.0.6/drclient/cli/cmd_pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
     if output_directory is None:
         output_directory = mkdtemp()
         if tar_file or squafshfs_file:
             is_tmp_output_directory = True
             atexit.register(shutil.rmtree, output_directory)
     else:
+        print(output_directory)
         if not output_directory.exists():
             output_directory.mkdir(parents=True)
         else:
             if not output_directory.is_dir():
                 raise typer.BadParameter(
                     f"Output directory {output_directory} is not a directory"
                 )
@@ -71,14 +72,15 @@
         cwd = os.getcwd()
         os.chdir(output_directory)
         with tarfile.open(tar_file, "w:gz") as tar:
             tar.add(".", arcname="", recursive=True)
         os.chdir(cwd)
 
     if squafshfs_file:
+        squafshfs_file = Path(squafshfs_file)
         if squafshfs_file.exists():
             squafshfs_file.unlink()
         print("Creating squashfs file...", end="", flush=True)
         exit_code, output = getstatusoutput(
             f"mksquashfs {output_directory} {squafshfs_file}"
         )
         if exit_code != 0:
```

### Comparing `drclient-0.0.5/drclient/extract.py` & `drclient-0.0.6/drclient/extract.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.5/drclient/registry/registry.py` & `drclient-0.0.6/drclient/registry/registry.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.5/drclient/threaded_pull.py` & `drclient-0.0.6/drclient/threaded_pull.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.5/drclient/view/history.py` & `drclient-0.0.6/drclient/view/history.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.5/drclient/view/info.py` & `drclient-0.0.6/drclient/view/info.py`

 * *Files identical despite different names*

### Comparing `drclient-0.0.5/drclient.egg-info/PKG-INFO` & `drclient-0.0.6/drclient.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drclient
-Version: 0.0.5
+Version: 0.0.6
 Summary: A docker registry client command line utility and Python library
 Home-page: https://github.com/joaompinto/drclient
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `drclient-0.0.5/drclient.egg-info/SOURCES.txt` & `drclient-0.0.6/drclient.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
+test.py
 tox.ini
 .github/workflows/multi-test.yaml
 .github/workflows/release.yaml
 .vscode/launch.json
 .vscode/settings.json
 drclient/__main__.py
 drclient/extract.py
@@ -21,17 +22,18 @@
 drclient.egg-info/SOURCES.txt
 drclient.egg-info/dependency_links.txt
 drclient.egg-info/entry_points.txt
 drclient.egg-info/requires.txt
 drclient.egg-info/top_level.txt
 drclient/cli/cmd_info.py
 drclient/cli/cmd_pull.py
-drclient/cli/verbose.py
+drclient/cli/main.py
 drclient/registry/__init__.py
 drclient/registry/manifest.py
 drclient/registry/registry.py
 drclient/registry/specs.py
 drclient/view/console.py
 drclient/view/history.py
 drclient/view/info.py
 tests/test_image_url.py
+tests/test_pull.py
 tests/test_version.py
```

### Comparing `drclient-0.0.5/setup.py` & `drclient-0.0.6/setup.py`

 * *Files identical despite different names*

