# Comparing `tmp/spawn-lia-0.2.2.tar.gz` & `tmp/spawn-lia-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spawn-lia-0.2.2.tar", last modified: Sat Apr  8 10:22:52 2023, max compression
+gzip compressed data, was "spawn-lia-0.2.3.tar", last modified: Wed Apr 12 17:14:13 2023, max compression
```

## Comparing `spawn-lia-0.2.2.tar` & `spawn-lia-0.2.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-08 10:22:52.775508 spawn-lia-0.2.2/
--rw-r--r--   0 developer  (1001) developer  (1001)    34693 2023-04-08 10:22:46.000000 spawn-lia-0.2.2/LICENSE.txt
--rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-08 10:22:52.775508 spawn-lia-0.2.2/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     3835 2023-04-07 19:35:39.000000 spawn-lia-0.2.2/README.md
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-08 10:22:52.775508 spawn-lia-0.2.2/lia/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-03 18:48:44.000000 spawn-lia-0.2.2/lia/__init__.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-08 10:22:52.775508 spawn-lia-0.2.2/lia/check_git/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-03 18:48:44.000000 spawn-lia-0.2.2/lia/check_git/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1486 2023-04-08 10:22:46.000000 spawn-lia-0.2.2/lia/check_git/verify_branch.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-08 10:22:52.775508 spawn-lia-0.2.2/lia/conversation/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 20:03:31.000000 spawn-lia-0.2.2/lia/conversation/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1003 2023-04-08 10:22:46.000000 spawn-lia-0.2.2/lia/conversation/ask_to_proceed.py
--rw-r--r--   0 developer  (1001) developer  (1001)      104 2023-04-08 09:57:30.000000 spawn-lia-0.2.2/lia/conversation/decision.py
--rw-r--r--   0 developer  (1001) developer  (1001)      873 2023-04-08 10:05:19.000000 spawn-lia-0.2.2/lia/conversation/emojis.py
--rw-r--r--   0 developer  (1001) developer  (1001)      394 2023-04-08 10:16:41.000000 spawn-lia-0.2.2/lia/conversation/end_message.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1026 2023-04-08 10:18:13.000000 spawn-lia-0.2.2/lia/conversation/start_message.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2218 2023-04-08 10:20:14.000000 spawn-lia-0.2.2/lia/conversation/virtualenv.py
--rw-r--r--   0 developer  (1001) developer  (1001)     3976 2023-04-08 10:22:46.000000 spawn-lia-0.2.2/lia/main.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-08 10:22:52.775508 spawn-lia-0.2.2/lia/simplify/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 19:56:24.000000 spawn-lia-0.2.2/lia/simplify/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1774 2023-04-08 10:22:46.000000 spawn-lia-0.2.2/lia/simplify/create_venv.py
--rw-r--r--   0 developer  (1001) developer  (1001)      246 2023-04-03 18:48:44.000000 spawn-lia-0.2.2/lia/verify_package.py
--rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-04-08 10:22:52.775508 spawn-lia-0.2.2/setup.cfg
--rw-r--r--   0 developer  (1001) developer  (1001)     1156 2023-04-08 10:22:43.000000 spawn-lia-0.2.2/setup.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-08 10:22:52.775508 spawn-lia-0.2.2/spawn_lia.egg-info/
--rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-08 10:22:52.000000 spawn-lia-0.2.2/spawn_lia.egg-info/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)      690 2023-04-08 10:22:52.000000 spawn-lia-0.2.2/spawn_lia.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-08 10:22:52.000000 spawn-lia-0.2.2/spawn_lia.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       40 2023-04-08 10:22:52.000000 spawn-lia-0.2.2/spawn_lia.egg-info/entry_points.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       96 2023-04-08 10:22:52.000000 spawn-lia-0.2.2/spawn_lia.egg-info/requires.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        4 2023-04-08 10:22:52.000000 spawn-lia-0.2.2/spawn_lia.egg-info/top_level.txt
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-08 10:22:52.775508 spawn-lia-0.2.2/tests/
--rw-r--r--   0 developer  (1001) developer  (1001)      626 2023-04-07 19:00:56.000000 spawn-lia-0.2.2/tests/test_deploy.py
--rw-r--r--   0 developer  (1001) developer  (1001)     3841 2023-04-07 19:00:56.000000 spawn-lia-0.2.2/tests/test_git_check.py
--rw-r--r--   0 developer  (1001) developer  (1001)      668 2023-04-07 19:00:56.000000 spawn-lia-0.2.2/tests/test_heal.py
--rw-r--r--   0 developer  (1001) developer  (1001)      772 2023-04-08 10:13:59.000000 spawn-lia-0.2.2/tests/test_venv.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/
+-rw-r--r--   0 developer  (1001) developer  (1001)    34693 2023-04-12 17:14:07.000000 spawn-lia-0.2.3/LICENSE.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     3835 2023-04-07 19:35:39.000000 spawn-lia-0.2.3/README.md
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/lia/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-03 18:48:44.000000 spawn-lia-0.2.3/lia/__init__.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/lia/check_git/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-03 18:48:44.000000 spawn-lia-0.2.3/lia/check_git/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1486 2023-04-12 17:14:07.000000 spawn-lia-0.2.3/lia/check_git/verify_branch.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/lia/conversation/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 20:03:31.000000 spawn-lia-0.2.3/lia/conversation/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1003 2023-04-12 17:14:07.000000 spawn-lia-0.2.3/lia/conversation/ask_to_proceed.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      104 2023-04-08 09:57:30.000000 spawn-lia-0.2.3/lia/conversation/decision.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      873 2023-04-08 10:05:19.000000 spawn-lia-0.2.3/lia/conversation/emojis.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      394 2023-04-08 10:16:41.000000 spawn-lia-0.2.3/lia/conversation/end_message.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1026 2023-04-08 10:18:13.000000 spawn-lia-0.2.3/lia/conversation/start_message.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2236 2023-04-12 17:13:06.000000 spawn-lia-0.2.3/lia/conversation/virtualenv.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      542 2023-04-12 17:07:04.000000 spawn-lia-0.2.3/lia/main.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/lia/simplify/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 19:56:24.000000 spawn-lia-0.2.3/lia/simplify/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1774 2023-04-12 17:14:07.000000 spawn-lia-0.2.3/lia/simplify/create_venv.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      246 2023-04-03 18:48:44.000000 spawn-lia-0.2.3/lia/simplify/verify_package.py
+-rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/setup.cfg
+-rw-r--r--   0 developer  (1001) developer  (1001)     1156 2023-04-12 17:14:03.000000 spawn-lia-0.2.3/setup.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/spawn_lia.egg-info/
+-rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-12 17:14:13.000000 spawn-lia-0.2.3/spawn_lia.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)      699 2023-04-12 17:14:13.000000 spawn-lia-0.2.3/spawn_lia.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-12 17:14:13.000000 spawn-lia-0.2.3/spawn_lia.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       40 2023-04-12 17:14:13.000000 spawn-lia-0.2.3/spawn_lia.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       96 2023-04-12 17:14:13.000000 spawn-lia-0.2.3/spawn_lia.egg-info/requires.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        4 2023-04-12 17:14:13.000000 spawn-lia-0.2.3/spawn_lia.egg-info/top_level.txt
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-12 17:14:13.783950 spawn-lia-0.2.3/tests/
+-rw-r--r--   0 developer  (1001) developer  (1001)      626 2023-04-07 19:00:56.000000 spawn-lia-0.2.3/tests/test_deploy.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     3841 2023-04-07 19:00:56.000000 spawn-lia-0.2.3/tests/test_git_check.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1140 2023-04-12 17:06:07.000000 spawn-lia-0.2.3/tests/test_heal.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      772 2023-04-08 10:13:59.000000 spawn-lia-0.2.3/tests/test_venv.py
```

### Comparing `spawn-lia-0.2.2/LICENSE.txt` & `spawn-lia-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.2/PKG-INFO` & `spawn-lia-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spawn-lia
-Version: 0.2.2
+Version: 0.2.3
 Summary: The most wanted support
 Home-page: https://codeberg.org/cap_jmk/lia
 Author: Julian M. Kleber
 Author-email: julian.kleber@sail.black
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `spawn-lia-0.2.2/README.md` & `spawn-lia-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.2/lia/check_git/verify_branch.py` & `spawn-lia-0.2.3/lia/check_git/verify_branch.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.2/lia/conversation/ask_to_proceed.py` & `spawn-lia-0.2.3/lia/conversation/ask_to_proceed.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.2/lia/conversation/emojis.py` & `spawn-lia-0.2.3/lia/conversation/emojis.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.2/lia/conversation/start_message.py` & `spawn-lia-0.2.3/lia/conversation/start_message.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.2/lia/conversation/virtualenv.py` & `spawn-lia-0.2.3/lia/conversation/virtualenv.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,12 +68,13 @@
         echo(f"Good decision, darling {magic_wand} {kissing_cat}")
         out = subprocess.run(
             ["source", venv_path, "&&", "deactivate"],
             check=True,
             shell=True,
             capture_output=True,
         )
+        echo(out)
         echo(f"Okay, I am done {dizzy}")
         sys.exit()
     else:
         echo(f"You have to decide y/n, darling...{face_with_rolling_eyes}")
         sys.exit()
```

### Comparing `spawn-lia-0.2.2/lia/simplify/create_venv.py` & `spawn-lia-0.2.3/lia/simplify/create_venv.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.2/setup.py` & `spawn-lia-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="spawn-lia",
-    version="0.2.2",
+    version="0.2.3",
     packages=find_packages(include=["lia*"]),
     include_package_data=True,
     install_requires=[
         "Click",
         "black",
         "autopep8",
         "mypy",
```

### Comparing `spawn-lia-0.2.2/spawn_lia.egg-info/PKG-INFO` & `spawn-lia-0.2.3/spawn_lia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spawn-lia
-Version: 0.2.2
+Version: 0.2.3
 Summary: The most wanted support
 Home-page: https://codeberg.org/cap_jmk/lia
 Author: Julian M. Kleber
 Author-email: julian.kleber@sail.black
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `spawn-lia-0.2.2/spawn_lia.egg-info/SOURCES.txt` & `spawn-lia-0.2.3/spawn_lia.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 LICENSE.txt
 README.md
 setup.py
 lia/__init__.py
 lia/main.py
-lia/verify_package.py
 lia/check_git/__init__.py
 lia/check_git/verify_branch.py
 lia/conversation/__init__.py
 lia/conversation/ask_to_proceed.py
 lia/conversation/decision.py
 lia/conversation/emojis.py
 lia/conversation/end_message.py
 lia/conversation/start_message.py
 lia/conversation/virtualenv.py
 lia/simplify/__init__.py
 lia/simplify/create_venv.py
+lia/simplify/verify_package.py
 spawn_lia.egg-info/PKG-INFO
 spawn_lia.egg-info/SOURCES.txt
 spawn_lia.egg-info/dependency_links.txt
 spawn_lia.egg-info/entry_points.txt
 spawn_lia.egg-info/requires.txt
 spawn_lia.egg-info/top_level.txt
 tests/test_deploy.py
```

### Comparing `spawn-lia-0.2.2/tests/test_deploy.py` & `spawn-lia-0.2.3/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.2/tests/test_git_check.py` & `spawn-lia-0.2.3/tests/test_git_check.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.2/tests/test_venv.py` & `spawn-lia-0.2.3/tests/test_venv.py`

 * *Files identical despite different names*

