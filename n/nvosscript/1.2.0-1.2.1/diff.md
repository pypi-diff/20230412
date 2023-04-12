# Comparing `tmp/nvosscript-1.2.0.tar.gz` & `tmp/nvosscript-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.2.0.tar", last modified: Wed Apr 12 01:43:35 2023, max compression
+gzip compressed data, was "nvosscript-1.2.1.tar", last modified: Wed Apr 12 01:53:46 2023, max compression
```

## Comparing `nvosscript-1.2.0.tar` & `nvosscript-1.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:43:35.589281 nvosscript-1.2.0/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.2.0/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-12 01:43:35.589147 nvosscript-1.2.0/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.2.0/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:43:35.587538 nvosscript-1.2.0/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.2.0/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    12912 2023-04-12 01:26:56.000000 nvosscript-1.2.0/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-06 06:54:07.000000 nvosscript-1.2.0/nvos/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     7481 2023-04-11 11:20:46.000000 nvosscript-1.2.0/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4493 2023-04-12 01:35:00.000000 nvosscript-1.2.0/nvos/run.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      893 2023-04-12 01:33:59.000000 nvosscript-1.2.0/nvos/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:43:35.588431 nvosscript-1.2.0/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-12 01:43:35.000000 nvosscript-1.2.0/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      372 2023-04-12 01:43:35.000000 nvosscript-1.2.0/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-12 01:43:35.000000 nvosscript-1.2.0/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-12 01:43:35.000000 nvosscript-1.2.0/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-04-12 01:43:35.000000 nvosscript-1.2.0/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       21 2023-04-12 01:43:35.000000 nvosscript-1.2.0/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-12 01:43:35.589323 nvosscript-1.2.0/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-04-12 01:40:18.000000 nvosscript-1.2.0/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:43:35.588652 nvosscript-1.2.0/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.2.0/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     3529 2023-04-12 01:40:27.000000 nvosscript-1.2.0/start/main.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:43:35.588869 nvosscript-1.2.0/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1283 2023-04-11 01:53:27.000000 nvosscript-1.2.0/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:53:46.682566 nvosscript-1.2.1/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.2.1/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-12 01:53:46.682425 nvosscript-1.2.1/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.2.1/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:53:46.680900 nvosscript-1.2.1/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.2.1/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    12912 2023-04-12 01:26:56.000000 nvosscript-1.2.1/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-06 06:54:07.000000 nvosscript-1.2.1/nvos/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     7481 2023-04-11 11:20:46.000000 nvosscript-1.2.1/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4493 2023-04-12 01:35:00.000000 nvosscript-1.2.1/nvos/run.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      903 2023-04-12 01:53:07.000000 nvosscript-1.2.1/nvos/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:53:46.681773 nvosscript-1.2.1/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-12 01:53:46.000000 nvosscript-1.2.1/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      372 2023-04-12 01:53:46.000000 nvosscript-1.2.1/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-12 01:53:46.000000 nvosscript-1.2.1/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-12 01:53:46.000000 nvosscript-1.2.1/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-04-12 01:53:46.000000 nvosscript-1.2.1/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       21 2023-04-12 01:53:46.000000 nvosscript-1.2.1/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-12 01:53:46.682609 nvosscript-1.2.1/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-04-12 01:53:38.000000 nvosscript-1.2.1/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:53:46.682001 nvosscript-1.2.1/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.2.1/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     3529 2023-04-12 01:53:41.000000 nvosscript-1.2.1/start/main.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 01:53:46.682118 nvosscript-1.2.1/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1283 2023-04-11 01:53:27.000000 nvosscript-1.2.1/win/win_auto_script.py
```

### Comparing `nvosscript-1.2.0/LICENSE` & `nvosscript-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.0/nvos/file.py` & `nvosscript-1.2.1/nvos/file.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.0/nvos/login.py` & `nvosscript-1.2.1/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.0/nvos/remote.py` & `nvosscript-1.2.1/nvos/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.0/nvos/run.py` & `nvosscript-1.2.1/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.0/nvos/utils.py` & `nvosscript-1.2.1/nvos/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             return current_path, True
     return check_workspace_exist(os.path.dirname(current_path))
 
 
 def check_subdirectory_workspace_exist(current_path, index=0):
     for file_name in os.listdir(current_path):
         if ".ndtc" == file_name and index >= 1:
-            return os.path.join(current_path,file_name) ,True
+            return os.path.join(current_path, file_name), True
     for file_name in os.listdir(current_path):
         if os.path.isdir(os.path.join(current_path, file_name)):
             index = index + 1
-            result = check_subdirectory_workspace_exist(os.path.join(current_path, file_name), index)
+            subdirectory_workspace, result = check_subdirectory_workspace_exist(os.path.join(current_path, file_name), index)
             if result:
-                return os.path.join(current_path, file_name), result
+                return subdirectory_workspace, result
     return "", False
```

### Comparing `nvosscript-1.2.0/setup.py` & `nvosscript-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.2.0',
+    version='1.2.1',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.2.0/start/main.py` & `nvosscript-1.2.1/start/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     elif args.subcommand == "async":
         run.command_async()
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.2.0")
+        print("1.2.1")
     elif args.subcommand == 'env':
         run.command_env(args.switch)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
         current_file_dir = os.path.dirname(current_file_dir)
         win_path = os.path.join(current_file_dir, 'win', 'win_auto_script.py')
```

### Comparing `nvosscript-1.2.0/win/win_auto_script.py` & `nvosscript-1.2.1/win/win_auto_script.py`

 * *Files identical despite different names*

