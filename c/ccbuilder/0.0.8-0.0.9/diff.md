# Comparing `tmp/ccbuilder-0.0.8.tar.gz` & `tmp/ccbuilder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccbuilder-0.0.8.tar", last modified: Mon Jul 11 10:35:09 2022, max compression
+gzip compressed data, was "ccbuilder-0.0.9.tar", last modified: Fri Jul 29 09:18:51 2022, max compression
```

## Comparing `ccbuilder-0.0.8.tar` & `ccbuilder-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-11 10:35:09.914274 ccbuilder-0.0.8/
--rw-r--r--   0 theo      (1000) theo      (1000)    11368 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/LICENSE
--rw-r--r--   0 theo      (1000) theo      (1000)       54 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/MANIFEST.in
--rw-r--r--   0 theo      (1000) theo      (1000)      681 2022-07-11 10:35:09.914274 ccbuilder-0.0.8/PKG-INFO
--rw-r--r--   0 theo      (1000) theo      (1000)      290 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/README.md
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-11 10:35:09.910940 ccbuilder-0.0.8/ccbuilder/
--rw-r--r--   0 theo      (1000) theo      (1000)     9576 2022-07-11 10:34:44.000000 ccbuilder-0.0.8/ccbuilder/__init__.py
--rw-r--r--   0 theo      (1000) theo      (1000)       75 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/ccbuilder/__main__.py
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-11 10:35:09.910940 ccbuilder-0.0.8/ccbuilder/builder/
--rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/ccbuilder/builder/__init__.py
--rw-r--r--   0 theo      (1000) theo      (1000)    14754 2022-07-11 10:34:44.000000 ccbuilder-0.0.8/ccbuilder/builder/builder.py
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-11 10:35:09.910940 ccbuilder-0.0.8/ccbuilder/data/
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-11 10:35:09.910940 ccbuilder-0.0.8/ccbuilder/data/patches/
--rw-r--r--   0 theo      (1000) theo      (1000)     1248 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/ccbuilder/data/patches/gcc-fix-simple-object-decl-and-use-in-gcc-lto.patch
--rw-r--r--   0 theo      (1000) theo      (1000)      632 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/ccbuilder/data/patches/gcc-libsanitizer.sh
--rw-r--r--   0 theo      (1000) theo      (1000)      739 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/ccbuilder/data/patches/gcc-simple-object-declaration.patch
--rw-r--r--   0 theo      (1000) theo      (1000)     2761 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/ccbuilder/data/patches/gcc-ustat.patch
--rw-r--r--   0 theo      (1000) theo      (1000)     2072 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/ccbuilder/data/patches/llvm-GCOpenMPRuntime.cpp-lambda-issues.patch
--rw-r--r--   0 theo      (1000) theo      (1000)      810 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes-missing-includes.patch
--rw-r--r--   0 theo      (1000) theo      (1000)      955 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes.h-fix-includes.patch
--rw-r--r--   0 theo      (1000) theo      (1000)  1011052 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/ccbuilder/data/patches/patchdb.json
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-11 10:35:09.914274 ccbuilder-0.0.8/ccbuilder/patcher/
--rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/ccbuilder/patcher/__init__.py
--rw-r--r--   0 theo      (1000) theo      (1000)     6300 2022-07-11 10:34:44.000000 ccbuilder-0.0.8/ccbuilder/patcher/patchdatabase.py
--rw-r--r--   0 theo      (1000) theo      (1000)    20255 2022-07-11 10:34:44.000000 ccbuilder-0.0.8/ccbuilder/patcher/patcher.py
--rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/ccbuilder/py.typed
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-11 10:35:09.914274 ccbuilder-0.0.8/ccbuilder/utils/
--rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/ccbuilder/utils/__init__.py
--rw-r--r--   0 theo      (1000) theo      (1000)    10483 2022-07-11 10:34:44.000000 ccbuilder-0.0.8/ccbuilder/utils/repository.py
--rw-r--r--   0 theo      (1000) theo      (1000)     5648 2022-07-11 10:34:44.000000 ccbuilder-0.0.8/ccbuilder/utils/utils.py
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-11 10:35:09.910940 ccbuilder-0.0.8/ccbuilder.egg-info/
--rw-r--r--   0 theo      (1000) theo      (1000)      681 2022-07-11 10:35:09.000000 ccbuilder-0.0.8/ccbuilder.egg-info/PKG-INFO
--rw-r--r--   0 theo      (1000) theo      (1000)      987 2022-07-11 10:35:09.000000 ccbuilder-0.0.8/ccbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 theo      (1000) theo      (1000)        1 2022-07-11 10:35:09.000000 ccbuilder-0.0.8/ccbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 theo      (1000) theo      (1000)       54 2022-07-11 10:35:09.000000 ccbuilder-0.0.8/ccbuilder.egg-info/entry_points.txt
--rw-r--r--   0 theo      (1000) theo      (1000)       10 2022-07-11 10:35:09.000000 ccbuilder-0.0.8/ccbuilder.egg-info/top_level.txt
--rw-r--r--   0 theo      (1000) theo      (1000)      126 2022-07-05 11:38:26.000000 ccbuilder-0.0.8/pyproject.toml
--rw-r--r--   0 theo      (1000) theo      (1000)      678 2022-07-11 10:35:09.914274 ccbuilder-0.0.8/setup.cfg
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.992906 ccbuilder-0.0.9/
+-rw-r--r--   0 theo      (1000) theo      (1000)    11368 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/LICENSE
+-rw-r--r--   0 theo      (1000) theo      (1000)       54 2022-05-25 09:41:26.000000 ccbuilder-0.0.9/MANIFEST.in
+-rw-r--r--   0 theo      (1000) theo      (1000)      681 2022-07-29 09:18:51.992906 ccbuilder-0.0.9/PKG-INFO
+-rw-r--r--   0 theo      (1000) theo      (1000)      290 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/README.md
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.982906 ccbuilder-0.0.9/ccbuilder/
+-rw-r--r--   0 theo      (1000) theo      (1000)     9576 2022-07-29 08:14:28.000000 ccbuilder-0.0.9/ccbuilder/__init__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)       75 2022-05-25 09:41:26.000000 ccbuilder-0.0.9/ccbuilder/__main__.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.982906 ccbuilder-0.0.9/ccbuilder/builder/
+-rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/builder/__init__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)    14768 2022-07-29 08:16:54.000000 ccbuilder-0.0.9/ccbuilder/builder/builder.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.979572 ccbuilder-0.0.9/ccbuilder/data/
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.986239 ccbuilder-0.0.9/ccbuilder/data/patches/
+-rw-r--r--   0 theo      (1000) theo      (1000)     1248 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/gcc-fix-simple-object-decl-and-use-in-gcc-lto.patch
+-rw-r--r--   0 theo      (1000) theo      (1000)      632 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/gcc-libsanitizer.sh
+-rw-r--r--   0 theo      (1000) theo      (1000)      739 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/gcc-simple-object-declaration.patch
+-rw-r--r--   0 theo      (1000) theo      (1000)     2761 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/gcc-ustat.patch
+-rw-r--r--   0 theo      (1000) theo      (1000)     2072 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/llvm-GCOpenMPRuntime.cpp-lambda-issues.patch
+-rw-r--r--   0 theo      (1000) theo      (1000)      810 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes-missing-includes.patch
+-rw-r--r--   0 theo      (1000) theo      (1000)      955 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes.h-fix-includes.patch
+-rw-r--r--   0 theo      (1000) theo      (1000)  1011052 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/data/patches/patchdb.json
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.992906 ccbuilder-0.0.9/ccbuilder/patcher/
+-rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/patcher/__init__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     6300 2022-07-29 08:14:28.000000 ccbuilder-0.0.9/ccbuilder/patcher/patchdatabase.py
+-rw-r--r--   0 theo      (1000) theo      (1000)    20255 2022-07-29 08:14:28.000000 ccbuilder-0.0.9/ccbuilder/patcher/patcher.py
+-rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-05-25 09:41:26.000000 ccbuilder-0.0.9/ccbuilder/py.typed
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.992906 ccbuilder-0.0.9/ccbuilder/utils/
+-rw-r--r--   0 theo      (1000) theo      (1000)        0 2022-04-21 11:15:44.000000 ccbuilder-0.0.9/ccbuilder/utils/__init__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)    10483 2022-07-29 08:14:28.000000 ccbuilder-0.0.9/ccbuilder/utils/repository.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     5648 2022-07-29 08:14:28.000000 ccbuilder-0.0.9/ccbuilder/utils/utils.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2022-07-29 09:18:51.982906 ccbuilder-0.0.9/ccbuilder.egg-info/
+-rw-r--r--   0 theo      (1000) theo      (1000)      681 2022-07-29 09:18:51.000000 ccbuilder-0.0.9/ccbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 theo      (1000) theo      (1000)      987 2022-07-29 09:18:51.000000 ccbuilder-0.0.9/ccbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)        1 2022-07-29 09:18:51.000000 ccbuilder-0.0.9/ccbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)       54 2022-07-29 09:18:51.000000 ccbuilder-0.0.9/ccbuilder.egg-info/entry_points.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)       10 2022-07-29 09:18:51.000000 ccbuilder-0.0.9/ccbuilder.egg-info/top_level.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)      126 2022-05-25 09:41:26.000000 ccbuilder-0.0.9/pyproject.toml
+-rw-r--r--   0 theo      (1000) theo      (1000)      678 2022-07-29 09:18:51.996240 ccbuilder-0.0.9/setup.cfg
```

### Comparing `ccbuilder-0.0.8/LICENSE` & `ccbuilder-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/PKG-INFO` & `ccbuilder-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccbuilder
-Version: 0.0.8
+Version: 0.0.9
 Summary: A clang/gcc compiler builder and patcher
 Home-page: https://github.com/DeadCodeProductions/ccbuilder
 Author: Theodoros Theodoridis
 Author-email: theodort@inf.ethz.ch
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `ccbuilder-0.0.8/ccbuilder/__init__.py` & `ccbuilder-0.0.9/ccbuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/ccbuilder/builder/builder.py` & `ccbuilder-0.0.9/ccbuilder/builder/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
     repo = select_repo(project, llvm_repo, gcc_repo)
     commit = repo.rev_to_commit(rev)
     install_prefix = get_install_path(cache_prefix, project, commit)
     success_indicator = install_prefix / "DONE"
 
     if not logdir:
         logdir = cache_prefix / "logs"
-    logdir.mkdir(exist_ok=True)
+    logdir.mkdir(exist_ok=True, parents=True)
     with BuildContext(install_prefix, success_indicator, project, commit, logdir) as (
         tmpdir,
         build_log,
     ):
         run_cmd_to_logfile(
             f"git -C {str(repo.path)} worktree" f" add {tmpdir} {commit} -f",
             log_file=build_log,
```

### Comparing `ccbuilder-0.0.8/ccbuilder/data/patches/gcc-fix-simple-object-decl-and-use-in-gcc-lto.patch` & `ccbuilder-0.0.9/ccbuilder/data/patches/gcc-fix-simple-object-decl-and-use-in-gcc-lto.patch`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/ccbuilder/data/patches/gcc-libsanitizer.sh` & `ccbuilder-0.0.9/ccbuilder/data/patches/gcc-libsanitizer.sh`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/ccbuilder/data/patches/gcc-simple-object-declaration.patch` & `ccbuilder-0.0.9/ccbuilder/data/patches/gcc-simple-object-declaration.patch`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/ccbuilder/data/patches/gcc-ustat.patch` & `ccbuilder-0.0.9/ccbuilder/data/patches/gcc-ustat.patch`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/ccbuilder/data/patches/llvm-GCOpenMPRuntime.cpp-lambda-issues.patch` & `ccbuilder-0.0.9/ccbuilder/data/patches/llvm-GCOpenMPRuntime.cpp-lambda-issues.patch`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes-missing-includes.patch` & `ccbuilder-0.0.9/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes-missing-includes.patch`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes.h-fix-includes.patch` & `ccbuilder-0.0.9/ccbuilder/data/patches/llvm-MicrosoftDemangleNodes.h-fix-includes.patch`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/ccbuilder/data/patches/patchdb.json` & `ccbuilder-0.0.9/ccbuilder/data/patches/patchdb.json`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/ccbuilder/patcher/patchdatabase.py` & `ccbuilder-0.0.9/ccbuilder/patcher/patchdatabase.py`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/ccbuilder/patcher/patcher.py` & `ccbuilder-0.0.9/ccbuilder/patcher/patcher.py`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/ccbuilder/utils/repository.py` & `ccbuilder-0.0.9/ccbuilder/utils/repository.py`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/ccbuilder/utils/utils.py` & `ccbuilder-0.0.9/ccbuilder/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/ccbuilder.egg-info/PKG-INFO` & `ccbuilder-0.0.9/ccbuilder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccbuilder
-Version: 0.0.8
+Version: 0.0.9
 Summary: A clang/gcc compiler builder and patcher
 Home-page: https://github.com/DeadCodeProductions/ccbuilder
 Author: Theodoros Theodoridis
 Author-email: theodort@inf.ethz.ch
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `ccbuilder-0.0.8/ccbuilder.egg-info/SOURCES.txt` & `ccbuilder-0.0.9/ccbuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccbuilder-0.0.8/setup.cfg` & `ccbuilder-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ccbuilder
-version = 0.0.8
+version = 0.0.9
 author = Theodoros Theodoridis
 author_email = theodort@inf.ethz.ch
 description = A clang/gcc compiler builder and patcher
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0
 url = https://github.com/DeadCodeProductions/ccbuilder
```

