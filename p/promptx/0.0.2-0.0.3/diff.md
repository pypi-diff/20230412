# Comparing `tmp/promptx-0.0.2.tar.gz` & `tmp/promptx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptx-0.0.2.tar", last modified: Wed Sep 21 20:49:26 2022, max compression
+gzip compressed data, was "promptx-0.0.3.tar", last modified: Wed Apr 12 06:18:31 2023, max compression
```

## Comparing `promptx-0.0.2.tar` & `promptx-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-09-21 20:49:26.636521 promptx-0.0.2/
--rw-r--r--   0 anon      (1000) wheel      (998)    34880 2022-09-15 20:58:55.000000 promptx-0.0.2/LICENSE.md
--rw-r--r--   0 anon      (1000) wheel      (998)     2839 2022-09-21 20:49:26.636521 promptx-0.0.2/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)     2526 2022-09-21 20:19:44.000000 promptx-0.0.2/README.md
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-09-21 20:49:26.636521 promptx-0.0.2/promptx/
--rw-r--r--   0 anon      (1000) wheel      (998)      145 2022-09-15 21:02:32.000000 promptx-0.0.2/promptx/__init__.py
--rw-r--r--   0 anon      (1000) wheel      (998)     5871 2022-09-21 20:47:04.000000 promptx-0.0.2/promptx/promptx.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-09-21 20:49:26.636521 promptx-0.0.2/promptx.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)     2839 2022-09-21 20:49:26.000000 promptx-0.0.2/promptx.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      198 2022-09-21 20:49:26.000000 promptx-0.0.2/promptx.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2022-09-21 20:49:26.000000 promptx-0.0.2/promptx.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        8 2022-09-21 20:49:26.000000 promptx-0.0.2/promptx.egg-info/top_level.txt
--rw-r--r--   0 anon      (1000) wheel      (998)      463 2022-09-21 20:48:03.000000 promptx-0.0.2/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2022-09-21 20:49:26.636521 promptx-0.0.2/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-12 06:18:31.142002 promptx-0.0.3/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34880 2022-09-15 20:58:55.000000 promptx-0.0.3/LICENSE.md
+-rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-12 06:18:31.142002 promptx-0.0.3/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)     2526 2022-09-21 20:19:44.000000 promptx-0.0.3/README.md
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-12 06:18:31.142002 promptx-0.0.3/promptx/
+-rw-r--r--   0 anon      (1000) wheel      (998)      145 2022-09-15 21:02:32.000000 promptx-0.0.3/promptx/__init__.py
+-rw-r--r--   0 anon      (1000) wheel      (998)     5991 2023-04-12 06:16:21.000000 promptx-0.0.3/promptx/promptx.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-12 06:18:31.142002 promptx-0.0.3/promptx.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-12 06:18:31.000000 promptx-0.0.3/promptx.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      198 2023-04-12 06:18:31.000000 promptx-0.0.3/promptx.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-12 06:18:31.000000 promptx-0.0.3/promptx.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        8 2023-04-12 06:18:31.000000 promptx-0.0.3/promptx.egg-info/top_level.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)      463 2023-04-12 06:17:59.000000 promptx-0.0.3/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-12 06:18:31.142002 promptx-0.0.3/setup.cfg
```

### Comparing `promptx-0.0.2/LICENSE.md` & `promptx-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `promptx-0.0.2/PKG-INFO` & `promptx-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptx
-Version: 0.0.2
+Version: 0.0.3
 Summary: Flexible prompt wrapper for dmenu, fzf, and rofi.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/promptx
 Keywords: dmenu,fzf,rofi
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `promptx-0.0.2/README.md` & `promptx-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `promptx-0.0.2/promptx/promptx.py` & `promptx-0.0.3/promptx/promptx.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,34 +140,37 @@
             prompt.stdin.write(opts_str)
 
         # Wait for selection
         if prompt.wait() == 0:
             # Process user selection
             selection = prompt.stdout.read().rstrip().splitlines()
             # Return the requested selection
-            if select == "first":
+            if select == "first" and len(selection) > 0:
                 return selection[0]
-            elif select == "last":
+            elif select == "last" and len(selection) > 0:
                 return selection[-1]
-            else:
+            elif len(selection) > 0:
                 return selection
+            else:
+                return None
 
         # fzf has no error to read, return None
         if stderr_file == None:
             return None
         # dmenu does print to stderr so we read it and return None
         # unless an actual error was encountered
         stderr = prompt.stderr.read()
         # If no err return None as user hit escape
         if stderr == "":
             return None
         # Otherwise some error occured
         raise PromptXError(cmd, stderr)
 
-    def add_args(self,
+    def add_args(
+        self,
         additional_args: List,
         default_args: bool = False,
     ):
         """
         Add args that are in a list. These are temporary by default but can be
         appended to the base_cmd if desired.
         """
```

### Comparing `promptx-0.0.2/promptx.egg-info/PKG-INFO` & `promptx-0.0.3/promptx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptx
-Version: 0.0.2
+Version: 0.0.3
 Summary: Flexible prompt wrapper for dmenu, fzf, and rofi.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/promptx
 Keywords: dmenu,fzf,rofi
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

