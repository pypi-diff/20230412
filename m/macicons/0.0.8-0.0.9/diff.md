# Comparing `tmp/macicons-0.0.8.tar.gz` & `tmp/macicons-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macicons-0.0.8.tar", last modified: Mon Mar 27 18:56:07 2023, max compression
+gzip compressed data, was "macicons-0.0.9.tar", last modified: Wed Apr 12 19:53:38 2023, max compression
```

## Comparing `macicons-0.0.8.tar` & `macicons-0.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-03-27 18:56:07.535782 macicons-0.0.8/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       28 2023-02-28 15:06:00.000000 macicons-0.0.8/MANIFEST.in
--rw-r--r--   0 cangyuanli   (501) staff       (20)      349 2023-03-27 18:56:07.535363 macicons-0.0.8/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1063 2023-03-27 18:50:43.000000 macicons-0.0.8/README.md
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-03-27 18:56:07.502180 macicons-0.0.8/macicons/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     8196 2023-02-27 15:54:37.000000 macicons-0.0.8/macicons/.DS_Store
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-03-27 18:50:44.000000 macicons-0.0.8/macicons/__init__.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-03-27 18:56:07.507769 macicons-0.0.8/macicons/__pycache__/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      159 2022-12-16 20:33:59.000000 macicons-0.0.8/macicons/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3333 2022-12-16 20:44:02.000000 macicons-0.0.8/macicons/__pycache__/change_icons.cpython-310.pyc
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1025 2022-12-16 20:47:16.000000 macicons-0.0.8/macicons/__pycache__/cli.cpython-310.pyc
--rwxr-xr-x   0 cangyuanli   (501) staff       (20)     3892 2023-03-27 18:55:26.000000 macicons-0.0.8/macicons/change_icons.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)      889 2023-03-27 18:50:45.000000 macicons-0.0.8/macicons/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-03-27 18:56:07.509391 macicons-0.0.8/macicons/data_files/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       67 2023-03-27 18:55:26.000000 macicons-0.0.8/macicons/data_files/ignorelist.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)      576 2023-03-27 18:50:45.000000 macicons-0.0.8/macicons/data_files/mapper.json
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-03-27 18:56:07.534002 macicons-0.0.8/macicons/icons/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     6148 2023-03-06 14:22:10.000000 macicons-0.0.8/macicons/icons/.DS_Store
--rw-r--r--   0 cangyuanli   (501) staff       (20)    22833 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/c.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)     4798 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/cpp.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    24761 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/csharp.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    11343 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/csv.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    33738 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/cython.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    12460 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/git.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    10248 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/gitfolder.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    15876 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/ipynb.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)     5972 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/javascript.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    14746 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/json.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    23798 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/julia.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    12492 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/latex.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3320 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/markdown.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    31146 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/php.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    15076 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/python.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    25826 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/r.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)   196597 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/ruby.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1727 2023-02-28 15:06:00.000000 macicons-0.0.8/macicons/icons/toml.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)     5240 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/txt.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)     5128 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/typescript.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    17648 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/vscode.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)    13555 2022-12-16 20:53:26.000000 macicons-0.0.8/macicons/icons/xml.png
--rw-r--r--   0 cangyuanli   (501) staff       (20)      337 2023-02-28 15:06:00.000000 macicons-0.0.8/macicons/icons/zig.png
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-03-27 18:56:07.504905 macicons-0.0.8/macicons.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      349 2023-03-27 18:56:07.000000 macicons-0.0.8/macicons.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1119 2023-03-27 18:56:07.000000 macicons-0.0.8/macicons.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-03-27 18:56:07.000000 macicons-0.0.8/macicons.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       47 2023-03-27 18:56:07.000000 macicons-0.0.8/macicons.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       40 2023-03-27 18:56:07.000000 macicons-0.0.8/macicons.egg-info/requires.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        9 2023-03-27 18:56:07.000000 macicons-0.0.8/macicons.egg-info/top_level.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       38 2023-03-27 18:56:07.535895 macicons-0.0.8/setup.cfg
--rw-r--r--   0 cangyuanli   (501) staff       (20)      628 2023-03-27 18:55:59.000000 macicons-0.0.8/setup.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-03-27 18:56:07.534865 macicons-0.0.8/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     4170 2023-03-27 18:55:26.000000 macicons-0.0.8/tests/test.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-12 19:53:38.699904 macicons-0.0.9/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       28 2023-02-28 15:06:00.000000 macicons-0.0.9/MANIFEST.in
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      349 2023-04-12 19:53:38.699120 macicons-0.0.9/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1063 2023-04-12 19:48:26.000000 macicons-0.0.9/README.md
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-12 19:53:38.651346 macicons-0.0.9/macicons/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     8196 2023-02-27 15:54:37.000000 macicons-0.0.9/macicons/.DS_Store
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-12 19:48:27.000000 macicons-0.0.9/macicons/__init__.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-12 19:53:38.660050 macicons-0.0.9/macicons/__pycache__/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      159 2022-12-16 20:33:59.000000 macicons-0.0.9/macicons/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3333 2022-12-16 20:44:02.000000 macicons-0.0.9/macicons/__pycache__/change_icons.cpython-310.pyc
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1025 2022-12-16 20:47:16.000000 macicons-0.0.9/macicons/__pycache__/cli.cpython-310.pyc
+-rwxr-xr-x   0 cangyuanli   (501) staff       (20)     3905 2023-04-12 19:48:27.000000 macicons-0.0.9/macicons/change_icons.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      889 2023-04-12 19:48:27.000000 macicons-0.0.9/macicons/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-12 19:53:38.661961 macicons-0.0.9/macicons/data_files/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       67 2023-04-12 19:48:27.000000 macicons-0.0.9/macicons/data_files/ignorelist.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      576 2023-04-12 19:48:27.000000 macicons-0.0.9/macicons/data_files/mapper.json
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-12 19:53:38.696019 macicons-0.0.9/macicons/icons/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     6148 2023-03-06 14:22:10.000000 macicons-0.0.9/macicons/icons/.DS_Store
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    22833 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/c.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     4798 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/cpp.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    24761 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/csharp.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    11343 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/csv.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    33738 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/cython.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    12460 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/git.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    10248 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/gitfolder.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    15876 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/ipynb.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     5972 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/javascript.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    14746 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/json.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    23798 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/julia.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    12492 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/latex.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3320 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/markdown.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    31146 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/php.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    15076 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/python.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    25826 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/r.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)   196597 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/ruby.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1727 2023-02-28 15:06:00.000000 macicons-0.0.9/macicons/icons/toml.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     5240 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/txt.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     5128 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/typescript.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    17648 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/vscode.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    13555 2022-12-16 20:53:26.000000 macicons-0.0.9/macicons/icons/xml.png
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      337 2023-02-28 15:06:00.000000 macicons-0.0.9/macicons/icons/zig.png
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-12 19:53:38.656997 macicons-0.0.9/macicons.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      349 2023-04-12 19:53:38.000000 macicons-0.0.9/macicons.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1119 2023-04-12 19:53:38.000000 macicons-0.0.9/macicons.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-12 19:53:38.000000 macicons-0.0.9/macicons.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       47 2023-04-12 19:53:38.000000 macicons-0.0.9/macicons.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       40 2023-04-12 19:53:38.000000 macicons-0.0.9/macicons.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        9 2023-04-12 19:53:38.000000 macicons-0.0.9/macicons.egg-info/top_level.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       38 2023-04-12 19:53:38.700080 macicons-0.0.9/setup.cfg
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      628 2023-04-12 19:53:25.000000 macicons-0.0.9/setup.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-12 19:53:38.697412 macicons-0.0.9/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     4170 2023-04-12 19:48:26.000000 macicons-0.0.9/tests/test.py
```

### Comparing `macicons-0.0.8/README.md` & `macicons-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/.DS_Store` & `macicons-0.0.9/macicons/.DS_Store`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/__pycache__/change_icons.cpython-310.pyc` & `macicons-0.0.9/macicons/__pycache__/change_icons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/__pycache__/cli.cpython-310.pyc` & `macicons-0.0.9/macicons/__pycache__/cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/change_icons.py` & `macicons-0.0.9/macicons/change_icons.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 def replace_all_icons(filelist: list[str], mapper_dict: dict, dumb: bool, nice: bool):
     func = functools.partial(
         replace_icon, mapper_dict=mapper_dict, dumb=dumb, nice=nice
     )
 
     # TODO: Fix multi-threaded version
     # with tqdm.tqdm(total=len(filelist)) as pbar:
-    #     with concurrent.futures.ThreadPoolExecutor() as pool:
+    #     with concurrent.futures.ThreadPoolExecutor(2) as pool:
     #         futures = [pool.submit(func, file) for file in filelist]
 
     #         total_changed = 0
     #         for future in concurrent.futures.as_completed(futures):
     #             total_changed += future.result()
     #             pbar.update(1)
 
@@ -139,9 +139,10 @@
     )
     numfiles, num_changed = replace_all_icons(
         filelist=lst, mapper_dict=mapper_dict, dumb=dumb, nice=nice
     )
 
     end = time.perf_counter()
     print(
-        f"Visited {numfiles} files and made {num_changed} changes in {display_time(end - start)}."
+        f"Visited {numfiles} files and made {num_changed} changes in"
+        f" {display_time(end - start)}."
     )
```

### Comparing `macicons-0.0.8/macicons/cli.py` & `macicons-0.0.9/macicons/cli.py`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/data_files/mapper.json` & `macicons-0.0.9/macicons/data_files/mapper.json`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/.DS_Store` & `macicons-0.0.9/macicons/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/c.png` & `macicons-0.0.9/macicons/icons/c.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/cpp.png` & `macicons-0.0.9/macicons/icons/cpp.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/csharp.png` & `macicons-0.0.9/macicons/icons/csharp.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/csv.png` & `macicons-0.0.9/macicons/icons/csv.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/cython.png` & `macicons-0.0.9/macicons/icons/cython.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/git.png` & `macicons-0.0.9/macicons/icons/git.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/gitfolder.png` & `macicons-0.0.9/macicons/icons/gitfolder.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/ipynb.png` & `macicons-0.0.9/macicons/icons/ipynb.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/javascript.png` & `macicons-0.0.9/macicons/icons/javascript.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/json.png` & `macicons-0.0.9/macicons/icons/json.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/julia.png` & `macicons-0.0.9/macicons/icons/julia.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/latex.png` & `macicons-0.0.9/macicons/icons/latex.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/markdown.png` & `macicons-0.0.9/macicons/icons/markdown.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/php.png` & `macicons-0.0.9/macicons/icons/php.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/python.png` & `macicons-0.0.9/macicons/icons/python.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/r.png` & `macicons-0.0.9/macicons/icons/r.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/ruby.png` & `macicons-0.0.9/macicons/icons/ruby.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/toml.png` & `macicons-0.0.9/macicons/icons/toml.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/txt.png` & `macicons-0.0.9/macicons/icons/txt.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/typescript.png` & `macicons-0.0.9/macicons/icons/typescript.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/vscode.png` & `macicons-0.0.9/macicons/icons/vscode.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons/icons/xml.png` & `macicons-0.0.9/macicons/icons/xml.png`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/macicons.egg-info/SOURCES.txt` & `macicons-0.0.9/macicons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macicons-0.0.8/setup.py` & `macicons-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="macicons",
-    version="0.0.8",
+    version="0.0.9",
     author="Cangyuan Li",
     author_email="everest229@gmail.com",
     description="CLI utility to change Mac Icons.",
     url="https://github.com/CangyuanLi/macicons",
     packages=["macicons"],
     include_package_data=True,
     entry_points={"console_scripts": ["macicons=macicons.cli:main"]},
```

### Comparing `macicons-0.0.8/tests/test.py` & `macicons-0.0.9/tests/test.py`

 * *Files identical despite different names*

