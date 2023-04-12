# Comparing `tmp/hardbrake-0.0.5.tar.gz` & `tmp/hardbrake-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardbrake-0.0.5.tar", last modified: Fri Apr  7 19:59:10 2023, max compression
+gzip compressed data, was "hardbrake-0.0.7.tar", last modified: Wed Apr 12 13:22:11 2023, max compression
```

## Comparing `hardbrake-0.0.5.tar` & `hardbrake-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:59:10.147484 hardbrake-0.0.5/
--rw-r--r--   0 tahsin     (501) staff       (20)     1063 2023-04-05 19:04:02.000000 hardbrake-0.0.5/LICENSE
--rw-r--r--   0 tahsin     (501) staff       (20)      199 2023-04-07 19:59:10.147341 hardbrake-0.0.5/PKG-INFO
--rw-r--r--   0 tahsin     (501) staff       (20)      892 2023-04-05 19:04:02.000000 hardbrake-0.0.5/README.md
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:59:10.145304 hardbrake-0.0.5/hardbrake.egg-info/
--rw-r--r--   0 tahsin     (501) staff       (20)      199 2023-04-07 19:59:09.000000 hardbrake-0.0.5/hardbrake.egg-info/PKG-INFO
--rw-r--r--   0 tahsin     (501) staff       (20)      351 2023-04-07 19:59:10.000000 hardbrake-0.0.5/hardbrake.egg-info/SOURCES.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        1 2023-04-07 19:59:09.000000 hardbrake-0.0.5/hardbrake.egg-info/dependency_links.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       43 2023-04-07 19:59:10.000000 hardbrake-0.0.5/hardbrake.egg-info/entry_points.txt
--rw-r--r--   0 tahsin     (501) staff       (20)      206 2023-04-07 19:59:10.000000 hardbrake-0.0.5/hardbrake.egg-info/requires.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        4 2023-04-07 19:59:10.000000 hardbrake-0.0.5/hardbrake.egg-info/top_level.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       38 2023-04-07 19:59:10.147528 hardbrake-0.0.5/setup.cfg
--rw-r--r--   0 tahsin     (501) staff       (20)      744 2023-04-07 19:58:59.000000 hardbrake-0.0.5/setup.py
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:59:10.147033 hardbrake-0.0.5/src/
--rw-r--r--   0 tahsin     (501) staff       (20)        0 2023-04-07 18:33:53.000000 hardbrake-0.0.5/src/__init__.py
--rw-r--r--   0 tahsin     (501) staff       (20)       29 2023-04-07 18:26:58.000000 hardbrake-0.0.5/src/__main__.py
--rw-r--r--   0 tahsin     (501) staff       (20)      812 2023-04-07 19:56:15.000000 hardbrake-0.0.5/src/app.py
--rw-r--r--   0 tahsin     (501) staff       (20)     1370 2023-04-05 19:04:02.000000 hardbrake-0.0.5/src/event.py
--rw-r--r--   0 tahsin     (501) staff       (20)      755 2023-04-05 19:04:02.000000 hardbrake-0.0.5/src/file.py
--rw-r--r--   0 tahsin     (501) staff       (20)      931 2023-04-05 19:04:02.000000 hardbrake-0.0.5/src/loader.py
--rw-r--r--   0 tahsin     (501) staff       (20)     1017 2023-04-07 19:56:42.000000 hardbrake-0.0.5/src/manager.py
--rw-r--r--   0 tahsin     (501) staff       (20)      364 2023-04-05 19:04:02.000000 hardbrake-0.0.5/src/prompts.py
--rw-r--r--   0 tahsin     (501) staff       (20)     1483 2023-04-05 19:04:02.000000 hardbrake-0.0.5/src/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 13:22:11.350115 hardbrake-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-04-12 13:21:44.000000 hardbrake-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-12 13:22:11.350115 hardbrake-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      940 2023-04-12 13:21:44.000000 hardbrake-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 13:22:11.346115 hardbrake-0.0.7/hardbrake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-12 13:22:11.000000 hardbrake-0.0.7/hardbrake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      366 2023-04-12 13:22:11.000000 hardbrake-0.0.7/hardbrake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 13:22:11.000000 hardbrake-0.0.7/hardbrake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-12 13:22:11.000000 hardbrake-0.0.7/hardbrake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2023-04-12 13:22:11.000000 hardbrake-0.0.7/hardbrake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-12 13:22:11.000000 hardbrake-0.0.7/hardbrake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-04-12 13:21:44.000000 hardbrake-0.0.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 13:22:11.350115 hardbrake-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-12 13:21:44.000000 hardbrake-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 13:22:11.350115 hardbrake-0.0.7/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 13:21:44.000000 hardbrake-0.0.7/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-04-12 13:21:44.000000 hardbrake-0.0.7/src/app.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-04-12 13:21:44.000000 hardbrake-0.0.7/src/event.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-04-12 13:21:44.000000 hardbrake-0.0.7/src/file.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-12 13:21:44.000000 hardbrake-0.0.7/src/loader.py
+-rw-r--r--   0 root         (0) root         (0)      169 2023-04-12 13:21:44.000000 hardbrake-0.0.7/src/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-04-12 13:21:44.000000 hardbrake-0.0.7/src/manager.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-04-12 13:21:44.000000 hardbrake-0.0.7/src/prompts.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-04-12 13:21:44.000000 hardbrake-0.0.7/src/utils.py
```

### Comparing `hardbrake-0.0.5/LICENSE` & `hardbrake-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.5/README.md` & `hardbrake-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -12,16 +12,22 @@
 
 <summary>With HardBrake</summary>
 <img style="width: 100%" src="demo/hardbrake.gif" />
 </details>
 
 ## Installation
 
-Will Add
+Install via pip:
+
+```
+pip install hardbrake
+```
 
 ## Usage
 
-Will Add
+```
+hardbrake
+```
 
 ## License
 
 HardBrake is licensed under the MIT License. See the LICENSE file for more information.
```

### Comparing `hardbrake-0.0.5/setup.py` & `hardbrake-0.0.7/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 from setuptools import setup, find_packages
 
+
+with open("requirements.txt", "r") as f:
+  required_packages = f.read().splitlines()
+
+
 setup(
     name="hardbrake",
-    version="0.0.5",
+    version="0.0.7",
     author="Tahsin",
     author_email="hello@tahsin.us",
     description="A wrapper around HandBrake CLI for encoding multiple files with ease.",
     packages=find_packages(),
-    install_requires=[
-        "autopep8==2.0.1",
-        "markdown-it-py==2.1.0",
-        "mdurl==0.1.2",
-        "prompt-toolkit==3.0.36",
-        "pycodestyle==2.10.0",
-        "pyee==9.0.4",
-        "Pygments==2.14.0",
-        "ranger-fm==1.9.3",
-        "rich==13.3.1",
-        "tomli==2.0.1",
-        "typing_extensions==4.5.0",
-        "wcwidth==0.2.6",
-    ],
+    install_requires=required_packages,
+    data_files=[("", ["requirements.txt"])],
     entry_points={
         'console_scripts': [
-            'hardbrake = src.app:main'
+            'hardbrake = src.app:cli',
+            'hb = src.app:cli'
         ]
     }
 )
```

### Comparing `hardbrake-0.0.5/src/event.py` & `hardbrake-0.0.7/src/event.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.5/src/loader.py` & `hardbrake-0.0.7/src/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     if not self.started:
       raise Exception("Loader not started")
 
   def stop(self):
     self.check_if_started()
     self.progress.stop()
     self.progress.__exit__(None, None, None)
+    self.started = False
 
 
 loader = Loader()
 
 
 def main():
   loader = Loader()
```

### Comparing `hardbrake-0.0.5/src/manager.py` & `hardbrake-0.0.7/src/manager.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.5/src/utils.py` & `hardbrake-0.0.7/src/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import hashlib
 import subprocess
+import src.prompts as prompts
+import src.file as file
 
 
 def hash(cmd: str) -> str:
   return hashlib.sha256(cmd.encode("utf-8")).hexdigest()[0:8]
 
 
 def get_encode_cmd(input_file_path: str, preset: str):
   file_name_without_extension = input_file_path.rsplit(".", 1)[0]
   output_file_path = f"{file_name_without_extension}_HandBraked-{preset}.mp4"
   cmd = f"HandBrakeCLI -i '{input_file_path}' -o '{output_file_path}' -Z '{preset}'"
+  file.manager.add_file(output_file_path)
 
   return cmd
 
 
 def get_presets():
   cmd = "HandBrakeCLI -z"
   result = subprocess.run(cmd, shell=True, capture_output=True)
@@ -35,18 +38,25 @@
 
     if len(category) > 0 and is_preset:
       preset_map[category].append(line.strip().strip("\t"))
 
   return preset_map
 
 
+def select_preset():
+  categories = get_presets()
+  category = prompts.ask_autocomplete(choices=list(categories.keys()), question="Select a category")
+  presets = categories[category]
+  preset = prompts.ask_autocomplete(choices=presets, question="Select a preset")
+
+  return preset
+
+
 def verify_installation(program_name: str):
   cmd = f"which {program_name}"
   result = subprocess.run(cmd, shell=True, capture_output=True)
   output_text = result.stdout.decode("utf-8")
   stderr_text = result.stderr.decode("utf-8")
 
   if len(output_text) == 0 or len(stderr_text) > 0:
     raise Exception("HandBrakeCLI is not installed",
                     stderr_text or output_text or "No output")
-
-  print("HandBrakeCLI is installed")
```

