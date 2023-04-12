# Comparing `tmp/python-git-info-0.8.2.tar.gz` & `tmp/python-git-info-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-git-info-0.8.2.tar", last modified: Sat Oct 29 07:08:57 2022, max compression
+gzip compressed data, was "python-git-info-0.8.3.tar", last modified: Wed Apr 12 05:45:34 2023, max compression
```

## Comparing `python-git-info-0.8.2.tar` & `python-git-info-0.8.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 07:08:57.266502 python-git-info-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-10-29 07:08:48.000000 python-git-info-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6820 2022-10-29 07:08:57.266502 python-git-info-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5847 2022-10-29 07:08:48.000000 python-git-info-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 07:08:57.266502 python-git-info-0.8.2/gitinfo/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-29 07:08:48.000000 python-git-info-0.8.2/gitinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-10-29 07:08:48.000000 python-git-info-0.8.2/gitinfo/gitinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-10-29 07:08:48.000000 python-git-info-0.8.2/gitinfo/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5200 2022-10-29 07:08:48.000000 python-git-info-0.8.2/gitinfo/pack_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 07:08:57.266502 python-git-info-0.8.2/python_git_info.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6820 2022-10-29 07:08:57.000000 python-git-info-0.8.2/python_git_info.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-10-29 07:08:57.000000 python-git-info-0.8.2/python_git_info.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 07:08:57.000000 python-git-info-0.8.2/python_git_info.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 07:08:57.000000 python-git-info-0.8.2/python_git_info.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-29 07:08:57.000000 python-git-info-0.8.2/python_git_info.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-29 07:08:57.266502 python-git-info-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-10-29 07:08:48.000000 python-git-info-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:45:34.118345 python-git-info-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-12 05:45:22.000000 python-git-info-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-12 05:45:34.118345 python-git-info-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-12 05:45:22.000000 python-git-info-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:45:34.114345 python-git-info-0.8.3/gitinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 05:45:22.000000 python-git-info-0.8.3/gitinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-04-12 05:45:22.000000 python-git-info-0.8.3/gitinfo/gitinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-12 05:45:22.000000 python-git-info-0.8.3/gitinfo/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-12 05:45:22.000000 python-git-info-0.8.3/gitinfo/pack_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:45:34.118345 python-git-info-0.8.3/python_git_info.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-12 05:45:34.000000 python-git-info-0.8.3/python_git_info.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 05:45:34.000000 python-git-info-0.8.3/python_git_info.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:45:34.000000 python-git-info-0.8.3/python_git_info.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:45:33.000000 python-git-info-0.8.3/python_git_info.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 05:45:34.000000 python-git-info-0.8.3/python_git_info.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 05:45:34.118345 python-git-info-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-12 05:45:22.000000 python-git-info-0.8.3/setup.py
```

### Comparing `python-git-info-0.8.2/LICENSE` & `python-git-info-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-git-info-0.8.2/PKG-INFO` & `python-git-info-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-git-info
-Version: 0.8.2
+Version: 0.8.3
 Summary: Get git information repository, directly from .git
 Home-page: https://github.com/spapas/python-git-info/
 Author: Serafeim Papastefanos
 Author-email: spapas@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python
@@ -118,14 +118,18 @@
 
 Also it is important to add here that this project is pure python and does not have
 any external dependencies (not even `git`); making it very easy to install and 
 use in any project.
 
 ## Changes
 
+0.8.3
+
+* Make it work with empty head refs
+
 0.8.2
 
 * Try the pypi github action
 
 0.8.1
 
 * Fix bug in decode_delta
```

### Comparing `python-git-info-0.8.2/README.md` & `python-git-info-0.8.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,18 @@
 
 Also it is important to add here that this project is pure python and does not have
 any external dependencies (not even `git`); making it very easy to install and 
 use in any project.
 
 ## Changes
 
+0.8.3
+
+* Make it work with empty head refs
+
 0.8.2
 
 * Try the pypi github action
 
 0.8.1
 
 * Fix bug in decode_delta
```

### Comparing `python-git-info-0.8.2/gitinfo/gitinfo.py` & `python-git-info-0.8.3/gitinfo/gitinfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,16 +48,28 @@
             # The head may contain just a commit so let's return it in that case:
             return data, refs
     if not head_parts:
         logger.warning("Git repository is broken (no head parts)")
         return None, None
 
     head_ref_file = os.path.join(directory, *head_parts)
+
     if not os.path.isfile(head_ref_file):
         logger.warning("Git repository is broken (no head ref file)")
+        # Try to find it on the remotes ?
+        bname = head_parts[-1]
+        remotes_dir = os.path.join(directory, "refs", "remotes")
+        remotes = os.listdir(remotes_dir)
+        for r in remotes:
+            remote_branch_file = os.path.join(remotes_dir, r, bname)
+            if os.path.isfile(remote_branch_file):
+                with open(remote_branch_file, "r") as fl:
+                    head_commit = fl.read().strip()
+                    return head_commit, refs
+
         return None, None
     head_commit = None
     with open(head_ref_file, "r") as fl:
         head_commit = fl.read().strip()
         return head_commit, refs
```

### Comparing `python-git-info-0.8.2/gitinfo/helpers.py` & `python-git-info-0.8.3/gitinfo/helpers.py`

 * *Files identical despite different names*

### Comparing `python-git-info-0.8.2/gitinfo/pack_reader.py` & `python-git-info-0.8.3/gitinfo/pack_reader.py`

 * *Files identical despite different names*

### Comparing `python-git-info-0.8.2/python_git_info.egg-info/PKG-INFO` & `python-git-info-0.8.3/python_git_info.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-git-info
-Version: 0.8.2
+Version: 0.8.3
 Summary: Get git information repository, directly from .git
 Home-page: https://github.com/spapas/python-git-info/
 Author: Serafeim Papastefanos
 Author-email: spapas@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python
@@ -118,14 +118,18 @@
 
 Also it is important to add here that this project is pure python and does not have
 any external dependencies (not even `git`); making it very easy to install and 
 use in any project.
 
 ## Changes
 
+0.8.3
+
+* Make it work with empty head refs
+
 0.8.2
 
 * Try the pypi github action
 
 0.8.1
 
 * Fix bug in decode_delta
```

### Comparing `python-git-info-0.8.2/setup.py` & `python-git-info-0.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="python-git-info",
-    version="0.8.2",
+    version="0.8.3",
     description="Get git information repository, directly from .git",
     author="Serafeim Papastefanos",
     author_email="spapas@gmail.com",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/spapas/python-git-info/",
```

