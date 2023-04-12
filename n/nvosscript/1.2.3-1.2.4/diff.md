# Comparing `tmp/nvosscript-1.2.3.tar.gz` & `tmp/nvosscript-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.2.3.tar", last modified: Wed Apr 12 03:17:52 2023, max compression
+gzip compressed data, was "nvosscript-1.2.4.tar", last modified: Wed Apr 12 03:36:03 2023, max compression
```

## Comparing `nvosscript-1.2.3.tar` & `nvosscript-1.2.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 03:17:52.855477 nvosscript-1.2.3/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.2.3/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-12 03:17:52.855306 nvosscript-1.2.3/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.2.3/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 03:17:52.853289 nvosscript-1.2.3/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.2.3/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    12912 2023-04-12 01:26:56.000000 nvosscript-1.2.3/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-06 06:54:07.000000 nvosscript-1.2.3/nvos/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     7691 2023-04-12 02:03:46.000000 nvosscript-1.2.3/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4612 2023-04-12 02:02:57.000000 nvosscript-1.2.3/nvos/run.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      903 2023-04-12 01:53:07.000000 nvosscript-1.2.3/nvos/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 03:17:52.854195 nvosscript-1.2.3/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-12 03:17:52.000000 nvosscript-1.2.3/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      339 2023-04-12 03:17:52.000000 nvosscript-1.2.3/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-12 03:17:52.000000 nvosscript-1.2.3/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-12 03:17:52.000000 nvosscript-1.2.3/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       21 2023-04-12 03:17:52.000000 nvosscript-1.2.3/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-12 03:17:52.855536 nvosscript-1.2.3/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      655 2023-04-12 03:17:19.000000 nvosscript-1.2.3/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 03:17:52.854420 nvosscript-1.2.3/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.2.3/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     3529 2023-04-12 03:17:25.000000 nvosscript-1.2.3/start/main.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 03:17:52.854657 nvosscript-1.2.3/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1283 2023-04-11 01:53:27.000000 nvosscript-1.2.3/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 03:36:03.497819 nvosscript-1.2.4/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.2.4/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-12 03:36:03.497695 nvosscript-1.2.4/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.2.4/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 03:36:03.495954 nvosscript-1.2.4/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.2.4/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    12912 2023-04-12 01:26:56.000000 nvosscript-1.2.4/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-06 06:54:07.000000 nvosscript-1.2.4/nvos/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     7691 2023-04-12 02:03:46.000000 nvosscript-1.2.4/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4612 2023-04-12 02:02:57.000000 nvosscript-1.2.4/nvos/run.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      903 2023-04-12 01:53:07.000000 nvosscript-1.2.4/nvos/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 03:36:03.496914 nvosscript-1.2.4/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-12 03:36:03.000000 nvosscript-1.2.4/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      372 2023-04-12 03:36:03.000000 nvosscript-1.2.4/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-12 03:36:03.000000 nvosscript-1.2.4/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-12 03:36:03.000000 nvosscript-1.2.4/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-04-12 03:36:03.000000 nvosscript-1.2.4/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       21 2023-04-12 03:36:03.000000 nvosscript-1.2.4/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-12 03:36:03.497859 nvosscript-1.2.4/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-04-12 03:25:41.000000 nvosscript-1.2.4/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 03:36:03.497144 nvosscript-1.2.4/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.2.4/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     3529 2023-04-12 03:25:46.000000 nvosscript-1.2.4/start/main.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-12 03:36:03.497371 nvosscript-1.2.4/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1283 2023-04-11 01:53:27.000000 nvosscript-1.2.4/win/win_auto_script.py
```

### Comparing `nvosscript-1.2.3/LICENSE` & `nvosscript-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.3/nvos/file.py` & `nvosscript-1.2.4/nvos/file.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.3/nvos/login.py` & `nvosscript-1.2.4/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.3/nvos/remote.py` & `nvosscript-1.2.4/nvos/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.3/nvos/run.py` & `nvosscript-1.2.4/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.3/nvos/utils.py` & `nvosscript-1.2.4/nvos/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.2.3/setup.py` & `nvosscript-1.2.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.2.3',
+    version='1.2.4',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
-    install_requires=[],
+    install_requires=[
+        'requests',
+        'python-daemon',
+        'boto3',
+        'ldap3',
+        'daemon',
+        "tqdm"
+        # Any other dependencies
+    ],
     license="MIT",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     entry_points={
```

### Comparing `nvosscript-1.2.3/start/main.py` & `nvosscript-1.2.4/start/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     elif args.subcommand == "async":
         run.command_async()
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.2.3")
+        print("1.2.4")
     elif args.subcommand == 'env':
         run.command_env(args.switch)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
         current_file_dir = os.path.dirname(current_file_dir)
         win_path = os.path.join(current_file_dir, 'win', 'win_auto_script.py')
```

### Comparing `nvosscript-1.2.3/win/win_auto_script.py` & `nvosscript-1.2.4/win/win_auto_script.py`

 * *Files identical despite different names*

