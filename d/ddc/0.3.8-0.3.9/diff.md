# Comparing `tmp/ddc-0.3.8.tar.gz` & `tmp/ddc-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddc-0.3.8.tar", last modified: Thu Dec 15 15:29:17 2022, max compression
+gzip compressed data, was "dist/ddc-0.3.9.tar", last modified: Wed Apr 12 09:16:54 2023, max compression
```

## Comparing `ddc-0.3.8.tar` & `ddc-0.3.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 am         (502) staff       (20)        0 2022-12-15 15:29:17.041231 ddc-0.3.8/
--rw-r--r--   0 am         (502) staff       (20)    11356 2022-05-18 13:57:23.000000 ddc-0.3.8/LICENSE
--rw-r--r--   0 am         (502) staff       (20)      529 2022-12-15 15:29:17.041092 ddc-0.3.8/PKG-INFO
--rw-r--r--   0 am         (502) staff       (20)      517 2022-12-13 10:57:23.000000 ddc-0.3.8/README.md
-drwxr-xr-x   0 am         (502) staff       (20)        0 2022-12-15 15:29:17.040130 ddc-0.3.8/ddc/
--rw-r--r--   0 am         (502) staff       (20)      127 2022-05-18 13:57:23.000000 ddc-0.3.8/ddc/__init__.py
--rw-r--r--   0 am         (502) staff       (20)     4665 2022-12-13 10:57:23.000000 ddc-0.3.8/ddc/cli.py
--rw-r--r--   0 am         (502) staff       (20)      938 2022-12-15 15:27:38.000000 ddc-0.3.8/ddc/info.py
--rw-r--r--   0 am         (502) staff       (20)     1247 2022-12-13 12:25:37.000000 ddc-0.3.8/ddc/meta_utils.py
--rw-r--r--   0 am         (502) staff       (20)      491 2022-12-13 12:25:37.000000 ddc-0.3.8/ddc/task_black.py
--rw-r--r--   0 am         (502) staff       (20)     1065 2022-05-18 13:57:23.000000 ddc-0.3.8/ddc/task_build_assets.py
--rw-r--r--   0 am         (502) staff       (20)     1061 2022-05-18 13:57:23.000000 ddc-0.3.8/ddc/task_build_docker_image.py
--rw-r--r--   0 am         (502) staff       (20)     7202 2022-05-18 13:57:23.000000 ddc-0.3.8/ddc/task_grpc_docs.py
--rw-r--r--   0 am         (502) staff       (20)     1570 2022-12-13 12:25:37.000000 ddc-0.3.8/ddc/task_lint.py
--rw-r--r--   0 am         (502) staff       (20)     3348 2022-05-18 13:57:23.000000 ddc-0.3.8/ddc/task_meta.py
--rw-r--r--   0 am         (502) staff       (20)     6844 2022-05-18 13:57:23.000000 ddc-0.3.8/ddc/task_test.py
--rw-r--r--   0 am         (502) staff       (20)     7461 2022-12-15 14:27:23.000000 ddc-0.3.8/ddc/utils.py
-drwxr-xr-x   0 am         (502) staff       (20)        0 2022-12-15 15:29:17.040917 ddc-0.3.8/ddc.egg-info/
--rw-r--r--   0 am         (502) staff       (20)      529 2022-12-15 15:29:16.000000 ddc-0.3.8/ddc.egg-info/PKG-INFO
--rw-r--r--   0 am         (502) staff       (20)      433 2022-12-15 15:29:16.000000 ddc-0.3.8/ddc.egg-info/SOURCES.txt
--rw-r--r--   0 am         (502) staff       (20)        1 2022-12-15 15:29:16.000000 ddc-0.3.8/ddc.egg-info/dependency_links.txt
--rw-r--r--   0 am         (502) staff       (20)       38 2022-12-15 15:29:16.000000 ddc-0.3.8/ddc.egg-info/entry_points.txt
--rw-r--r--   0 am         (502) staff       (20)        1 2022-12-15 15:29:16.000000 ddc-0.3.8/ddc.egg-info/not-zip-safe
--rw-r--r--   0 am         (502) staff       (20)       52 2022-12-15 15:29:16.000000 ddc-0.3.8/ddc.egg-info/requires.txt
--rw-r--r--   0 am         (502) staff       (20)        4 2022-12-15 15:29:16.000000 ddc-0.3.8/ddc.egg-info/top_level.txt
--rw-r--r--   0 am         (502) staff       (20)       38 2022-12-15 15:29:17.041268 ddc-0.3.8/setup.cfg
--rw-r--r--   0 am         (502) staff       (20)     1292 2022-05-18 13:57:23.000000 ddc-0.3.8/setup.py
+drwxr-xr-x   0 anton_fedora  (1000) anton_fedora  (1000)        0 2023-04-12 09:16:54.000000 ddc-0.3.9/
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)    11356 2022-11-17 10:57:34.000000 ddc-0.3.9/LICENSE
+drwxr-xr-x   0 anton_fedora  (1000) anton_fedora  (1000)        0 2023-04-12 09:16:54.000000 ddc-0.3.9/ddc/
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     6844 2022-11-17 10:57:34.000000 ddc-0.3.9/ddc/task_test.py
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1065 2022-11-17 10:57:34.000000 ddc-0.3.9/ddc/task_build_assets.py
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1247 2022-12-13 11:01:52.000000 ddc-0.3.9/ddc/meta_utils.py
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      491 2022-12-13 11:01:52.000000 ddc-0.3.9/ddc/task_black.py
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     7459 2023-04-12 09:13:32.000000 ddc-0.3.9/ddc/utils.py
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     3348 2022-11-17 10:57:34.000000 ddc-0.3.9/ddc/task_meta.py
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     4665 2022-11-17 10:57:34.000000 ddc-0.3.9/ddc/cli.py
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      127 2022-11-17 10:57:34.000000 ddc-0.3.9/ddc/__init__.py
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1061 2022-11-17 10:57:34.000000 ddc-0.3.9/ddc/task_build_docker_image.py
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      938 2023-04-12 09:13:32.000000 ddc-0.3.9/ddc/info.py
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     7202 2022-11-17 10:57:34.000000 ddc-0.3.9/ddc/task_grpc_docs.py
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1570 2022-12-13 11:01:52.000000 ddc-0.3.9/ddc/task_lint.py
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1292 2022-11-17 10:57:34.000000 ddc-0.3.9/setup.py
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)       38 2023-04-12 09:16:54.000000 ddc-0.3.9/setup.cfg
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      517 2022-11-17 10:57:34.000000 ddc-0.3.9/README.md
+drwxr-xr-x   0 anton_fedora  (1000) anton_fedora  (1000)        0 2023-04-12 09:16:54.000000 ddc-0.3.9/ddc.egg-info/
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      433 2023-04-12 09:16:54.000000 ddc-0.3.9/ddc.egg-info/SOURCES.txt
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)       38 2023-04-12 09:16:54.000000 ddc-0.3.9/ddc.egg-info/entry_points.txt
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)        1 2023-04-12 09:16:54.000000 ddc-0.3.9/ddc.egg-info/not-zip-safe
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)        1 2023-04-12 09:16:54.000000 ddc-0.3.9/ddc.egg-info/dependency_links.txt
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      529 2023-04-12 09:16:54.000000 ddc-0.3.9/ddc.egg-info/PKG-INFO
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)       52 2023-04-12 09:16:54.000000 ddc-0.3.9/ddc.egg-info/requires.txt
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)        4 2023-04-12 09:16:54.000000 ddc-0.3.9/ddc.egg-info/top_level.txt
+-rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      529 2023-04-12 09:16:54.000000 ddc-0.3.9/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ddc-0.3.8/LICENSE` & `ddc-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ddc-0.3.8/PKG-INFO` & `ddc-0.3.9/ddc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddc
-Version: 0.3.8
+Version: 0.3.9
 Summary: Devision Developers Cli
 Home-page: https://github.com/devision-io/ddc
 Author: Devision
 Author-email: info@devision.io
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Operating System :: OS Independent
```

### Comparing `ddc-0.3.8/README.md` & `ddc-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `ddc-0.3.8/ddc/cli.py` & `ddc-0.3.9/ddc/cli.py`

 * *Files identical despite different names*

### Comparing `ddc-0.3.8/ddc/info.py` & `ddc-0.3.9/ddc/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 from ddc.utils import exec_cmd
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 __package_name__ = "ddc"
 
 
 def print_about_version():
     print("Devision Developers Cli")  # noqa
     print("Version: " + __version__)  # noqa
```

### Comparing `ddc-0.3.8/ddc/meta_utils.py` & `ddc-0.3.9/ddc/meta_utils.py`

 * *Files identical despite different names*

### Comparing `ddc-0.3.8/ddc/task_build_assets.py` & `ddc-0.3.9/ddc/task_build_assets.py`

 * *Files identical despite different names*

### Comparing `ddc-0.3.8/ddc/task_build_docker_image.py` & `ddc-0.3.9/ddc/task_build_docker_image.py`

 * *Files identical despite different names*

### Comparing `ddc-0.3.8/ddc/task_grpc_docs.py` & `ddc-0.3.9/ddc/task_grpc_docs.py`

 * *Files identical despite different names*

### Comparing `ddc-0.3.8/ddc/task_lint.py` & `ddc-0.3.9/ddc/task_lint.py`

 * *Files identical despite different names*

### Comparing `ddc-0.3.8/ddc/task_meta.py` & `ddc-0.3.9/ddc/task_meta.py`

 * *Files identical despite different names*

### Comparing `ddc-0.3.8/ddc/task_test.py` & `ddc-0.3.9/ddc/task_test.py`

 * *Files identical despite different names*

### Comparing `ddc-0.3.8/ddc/utils.py` & `ddc-0.3.9/ddc/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 def get_exists_langs(base_path: str):
     """
     Compute which languages use in base_path
     """
     extensions = {
         # "js": False,
         # "ts": False,
-        # "java": False,
+        "java": False,
         "php": False,
         "py": False,
         # "go": False,
     }
     for file in iterate_source_files_with_gitignore(base_path):
         for f_ext, is_found in extensions.items():
             if not is_found:
```

### Comparing `ddc-0.3.8/ddc.egg-info/PKG-INFO` & `ddc-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddc
-Version: 0.3.8
+Version: 0.3.9
 Summary: Devision Developers Cli
 Home-page: https://github.com/devision-io/ddc
 Author: Devision
 Author-email: info@devision.io
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Operating System :: OS Independent
```

### Comparing `ddc-0.3.8/setup.py` & `ddc-0.3.9/setup.py`

 * *Files identical despite different names*

