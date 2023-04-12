# Comparing `tmp/robotframework-debug-4.3.1.tar.gz` & `tmp/robotframework-debug-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robotframework-debug-4.3.1.tar", last modified: Mon Apr  3 06:58:50 2023, max compression
+gzip compressed data, was "robotframework-debug-4.3.2.tar", last modified: Wed Apr 12 20:00:15 2023, max compression
```

## Comparing `robotframework-debug-4.3.1.tar` & `robotframework-debug-4.3.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 snooz      (501) staff       (20)        0 2023-04-03 06:58:50.000000 robotframework-debug-4.3.1/
--rw-r--r--   0 snooz      (501) staff       (20)      545 2023-03-15 17:47:16.000000 robotframework-debug-4.3.1/.coveragerc
--rw-r--r--   0 snooz      (501) staff       (20)      272 2023-03-15 17:47:16.000000 robotframework-debug-4.3.1/.gitpod.yml
--rw-r--r--   0 snooz      (501) staff       (20)     5811 2023-03-15 17:47:16.000000 robotframework-debug-4.3.1/ChangeLog
--rw-r--r--   0 snooz      (501) staff       (20)      139 2023-03-20 22:34:10.000000 robotframework-debug-4.3.1/CreateWheel.sh
--rw-r--r--   0 snooz      (501) staff       (20)     1471 2023-03-15 17:47:16.000000 robotframework-debug-4.3.1/LICENSE
--rw-r--r--   0 snooz      (501) staff       (20)      215 2023-03-15 21:54:14.000000 robotframework-debug-4.3.1/MANIFEST.in
--rw-r--r--   0 snooz      (501) staff       (20)     6027 2023-04-03 06:58:50.000000 robotframework-debug-4.3.1/PKG-INFO
--rw-r--r--   0 snooz      (501) staff       (20)     5047 2023-03-19 19:57:13.000000 robotframework-debug-4.3.1/README.rst
-drwxr-xr-x   0 snooz      (501) staff       (20)        0 2023-04-03 06:58:50.000000 robotframework-debug-4.3.1/RobotDebug/
--rw-r--r--   0 snooz      (501) staff       (20)     5878 2023-03-31 20:37:02.000000 robotframework-debug-4.3.1/RobotDebug/RobotDebug.py
--rw-r--r--   0 snooz      (501) staff       (20)      154 2023-03-31 08:22:53.000000 robotframework-debug-4.3.1/RobotDebug/__init__.py
--rw-r--r--   0 snooz      (501) staff       (20)    12567 2023-04-03 06:49:02.000000 robotframework-debug-4.3.1/RobotDebug/cmdcompleter.py
--rw-r--r--   0 snooz      (501) staff       (20)     9931 2023-04-02 21:41:20.000000 robotframework-debug-4.3.1/RobotDebug/debugcmd.py
--rw-r--r--   0 snooz      (501) staff       (20)      396 2023-03-31 20:37:02.000000 robotframework-debug-4.3.1/RobotDebug/globals.py
--rw-r--r--   0 snooz      (501) staff       (20)     4159 2023-04-02 21:51:57.000000 robotframework-debug-4.3.1/RobotDebug/history_app.py
--rw-r--r--   0 snooz      (501) staff       (20)     9120 2023-04-02 19:12:09.000000 robotframework-debug-4.3.1/RobotDebug/lexer.py
--rw-r--r--   0 snooz      (501) staff       (20)    13309 2023-04-02 21:53:42.000000 robotframework-debug-4.3.1/RobotDebug/prompttoolkitcmd.py
--rw-r--r--   0 snooz      (501) staff       (20)     3330 2023-03-31 08:23:06.000000 robotframework-debug-4.3.1/RobotDebug/robotkeyword.py
--rw-r--r--   0 snooz      (501) staff       (20)     1892 2023-04-01 18:18:08.000000 robotframework-debug-4.3.1/RobotDebug/robotlib.py
--rw-r--r--   0 snooz      (501) staff       (20)     1286 2023-03-31 08:23:06.000000 robotframework-debug-4.3.1/RobotDebug/shell.py
--rw-r--r--   0 snooz      (501) staff       (20)     4279 2023-03-31 08:23:06.000000 robotframework-debug-4.3.1/RobotDebug/sourcelines.py
--rw-r--r--   0 snooz      (501) staff       (20)     2587 2023-03-31 08:23:06.000000 robotframework-debug-4.3.1/RobotDebug/styles.py
--rw-r--r--   0 snooz      (501) staff       (20)       18 2023-04-03 06:57:38.000000 robotframework-debug-4.3.1/RobotDebug/version.py
--rw-r--r--   0 snooz      (501) staff       (20)       26 2023-03-15 17:47:16.000000 robotframework-debug-4.3.1/_config.yml
--rw-r--r--   0 snooz      (501) staff       (20)      738 2023-03-31 08:27:09.000000 robotframework-debug-4.3.1/pyproject.toml
-drwxr-xr-x   0 snooz      (501) staff       (20)        0 2023-04-03 06:58:50.000000 robotframework-debug-4.3.1/robotframework_debug.egg-info/
--rw-r--r--   0 snooz      (501) staff       (20)     6027 2023-04-03 06:58:50.000000 robotframework-debug-4.3.1/robotframework_debug.egg-info/PKG-INFO
--rw-r--r--   0 snooz      (501) staff       (20)      890 2023-04-03 06:58:50.000000 robotframework-debug-4.3.1/robotframework_debug.egg-info/SOURCES.txt
--rw-r--r--   0 snooz      (501) staff       (20)        1 2023-04-03 06:58:50.000000 robotframework-debug-4.3.1/robotframework_debug.egg-info/dependency_links.txt
--rw-r--r--   0 snooz      (501) staff       (20)       86 2023-04-03 06:58:50.000000 robotframework-debug-4.3.1/robotframework_debug.egg-info/entry_points.txt
--rw-r--r--   0 snooz      (501) staff       (20)        1 2023-03-15 17:54:44.000000 robotframework-debug-4.3.1/robotframework_debug.egg-info/not-zip-safe
--rw-r--r--   0 snooz      (501) staff       (20)       77 2023-04-03 06:58:50.000000 robotframework-debug-4.3.1/robotframework_debug.egg-info/requires.txt
--rw-r--r--   0 snooz      (501) staff       (20)       11 2023-04-03 06:58:50.000000 robotframework-debug-4.3.1/robotframework_debug.egg-info/top_level.txt
--rw-r--r--   0 snooz      (501) staff       (20)      159 2023-04-03 06:58:50.000000 robotframework-debug-4.3.1/setup.cfg
--rwxr-xr-x   0 snooz      (501) staff       (20)     2112 2023-04-01 10:10:07.000000 robotframework-debug-4.3.1/setup.py
-drwxr-xr-x   0 snooz      (501) staff       (20)        0 2023-04-03 06:58:50.000000 robotframework-debug-4.3.1/tests/
--rw-r--r--   0 snooz      (501) staff       (20)        0 2023-03-15 17:47:16.000000 robotframework-debug-4.3.1/tests/__init__.py
--rw-r--r--   0 snooz      (501) staff       (20)     1426 2023-04-02 18:53:31.000000 robotframework-debug-4.3.1/tests/demo.py
--rw-r--r--   0 snooz      (501) staff       (20)      609 2023-03-31 08:22:53.000000 robotframework-debug-4.3.1/tests/step.robot
--rw-r--r--   0 snooz      (501) staff       (20)      844 2023-03-31 20:34:46.000000 robotframework-debug-4.3.1/tests/step_listener.robot
--rw-r--r--   0 snooz      (501) staff       (20)     6067 2023-04-01 10:10:07.000000 robotframework-debug-4.3.1/tests/test_debuglibrary.py
--rw-r--r--   0 snooz      (501) staff       (20)     4624 2023-04-01 10:10:07.000000 robotframework-debug-4.3.1/tests/test_lib.py
+drwxr-xr-x   0 snooz      (501) staff       (20)        0 2023-04-12 20:00:15.017619 robotframework-debug-4.3.2/
+-rw-r--r--   0 snooz      (501) staff       (20)      545 2023-03-15 17:47:16.000000 robotframework-debug-4.3.2/.coveragerc
+-rw-r--r--   0 snooz      (501) staff       (20)      272 2023-03-15 17:47:16.000000 robotframework-debug-4.3.2/.gitpod.yml
+-rw-r--r--   0 snooz      (501) staff       (20)     5811 2023-03-15 17:47:16.000000 robotframework-debug-4.3.2/ChangeLog
+-rw-r--r--   0 snooz      (501) staff       (20)      139 2023-03-20 22:34:10.000000 robotframework-debug-4.3.2/CreateWheel.sh
+-rw-r--r--   0 snooz      (501) staff       (20)     1471 2023-03-15 17:47:16.000000 robotframework-debug-4.3.2/LICENSE
+-rw-r--r--   0 snooz      (501) staff       (20)      215 2023-03-15 21:54:14.000000 robotframework-debug-4.3.2/MANIFEST.in
+-rw-r--r--   0 snooz      (501) staff       (20)     6027 2023-04-12 20:00:15.017718 robotframework-debug-4.3.2/PKG-INFO
+-rw-r--r--   0 snooz      (501) staff       (20)     5047 2023-03-19 19:57:13.000000 robotframework-debug-4.3.2/README.rst
+drwxr-xr-x   0 snooz      (501) staff       (20)        0 2023-04-12 20:00:15.014631 robotframework-debug-4.3.2/RobotDebug/
+-rw-r--r--   0 snooz      (501) staff       (20)     5878 2023-03-31 20:37:02.000000 robotframework-debug-4.3.2/RobotDebug/RobotDebug.py
+-rw-r--r--   0 snooz      (501) staff       (20)      154 2023-03-31 08:22:53.000000 robotframework-debug-4.3.2/RobotDebug/__init__.py
+-rw-r--r--   0 snooz      (501) staff       (20)    12567 2023-04-03 06:49:02.000000 robotframework-debug-4.3.2/RobotDebug/cmdcompleter.py
+-rw-r--r--   0 snooz      (501) staff       (20)     9931 2023-04-02 21:41:20.000000 robotframework-debug-4.3.2/RobotDebug/debugcmd.py
+-rw-r--r--   0 snooz      (501) staff       (20)      396 2023-03-31 20:37:02.000000 robotframework-debug-4.3.2/RobotDebug/globals.py
+-rw-r--r--   0 snooz      (501) staff       (20)     4195 2023-04-07 20:09:22.000000 robotframework-debug-4.3.2/RobotDebug/history_app.py
+-rw-r--r--   0 snooz      (501) staff       (20)     9129 2023-04-07 20:09:22.000000 robotframework-debug-4.3.2/RobotDebug/lexer.py
+-rw-r--r--   0 snooz      (501) staff       (20)    13309 2023-04-02 21:53:42.000000 robotframework-debug-4.3.2/RobotDebug/prompttoolkitcmd.py
+-rw-r--r--   0 snooz      (501) staff       (20)     3330 2023-03-31 08:23:06.000000 robotframework-debug-4.3.2/RobotDebug/robotkeyword.py
+-rw-r--r--   0 snooz      (501) staff       (20)     1892 2023-04-01 18:18:08.000000 robotframework-debug-4.3.2/RobotDebug/robotlib.py
+-rw-r--r--   0 snooz      (501) staff       (20)     1286 2023-03-31 08:23:06.000000 robotframework-debug-4.3.2/RobotDebug/shell.py
+-rw-r--r--   0 snooz      (501) staff       (20)     4279 2023-03-31 08:23:06.000000 robotframework-debug-4.3.2/RobotDebug/sourcelines.py
+-rw-r--r--   0 snooz      (501) staff       (20)     2587 2023-03-31 08:23:06.000000 robotframework-debug-4.3.2/RobotDebug/styles.py
+-rw-r--r--   0 snooz      (501) staff       (20)       18 2023-04-12 19:58:55.000000 robotframework-debug-4.3.2/RobotDebug/version.py
+-rw-r--r--   0 snooz      (501) staff       (20)       26 2023-03-15 17:47:16.000000 robotframework-debug-4.3.2/_config.yml
+-rw-r--r--   0 snooz      (501) staff       (20)      738 2023-03-31 08:27:09.000000 robotframework-debug-4.3.2/pyproject.toml
+drwxr-xr-x   0 snooz      (501) staff       (20)        0 2023-04-12 20:00:15.016021 robotframework-debug-4.3.2/robotframework_debug.egg-info/
+-rw-r--r--   0 snooz      (501) staff       (20)     6027 2023-04-12 20:00:14.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/PKG-INFO
+-rw-r--r--   0 snooz      (501) staff       (20)      890 2023-04-12 20:00:14.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/SOURCES.txt
+-rw-r--r--   0 snooz      (501) staff       (20)        1 2023-04-12 20:00:14.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/dependency_links.txt
+-rw-r--r--   0 snooz      (501) staff       (20)       86 2023-04-12 20:00:14.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/entry_points.txt
+-rw-r--r--   0 snooz      (501) staff       (20)        1 2023-03-15 17:54:44.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/not-zip-safe
+-rw-r--r--   0 snooz      (501) staff       (20)       77 2023-04-12 20:00:14.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/requires.txt
+-rw-r--r--   0 snooz      (501) staff       (20)       11 2023-04-12 20:00:14.000000 robotframework-debug-4.3.2/robotframework_debug.egg-info/top_level.txt
+-rw-r--r--   0 snooz      (501) staff       (20)      159 2023-04-12 20:00:15.018064 robotframework-debug-4.3.2/setup.cfg
+-rwxr-xr-x   0 snooz      (501) staff       (20)     2112 2023-04-07 19:54:01.000000 robotframework-debug-4.3.2/setup.py
+drwxr-xr-x   0 snooz      (501) staff       (20)        0 2023-04-12 20:00:15.017444 robotframework-debug-4.3.2/tests/
+-rw-r--r--   0 snooz      (501) staff       (20)        0 2023-03-15 17:47:16.000000 robotframework-debug-4.3.2/tests/__init__.py
+-rw-r--r--   0 snooz      (501) staff       (20)     1426 2023-04-02 18:53:31.000000 robotframework-debug-4.3.2/tests/demo.py
+-rw-r--r--   0 snooz      (501) staff       (20)      609 2023-03-31 08:22:53.000000 robotframework-debug-4.3.2/tests/step.robot
+-rw-r--r--   0 snooz      (501) staff       (20)      844 2023-03-31 20:34:46.000000 robotframework-debug-4.3.2/tests/step_listener.robot
+-rw-r--r--   0 snooz      (501) staff       (20)     6067 2023-04-01 10:10:07.000000 robotframework-debug-4.3.2/tests/test_debuglibrary.py
+-rw-r--r--   0 snooz      (501) staff       (20)     4624 2023-04-01 10:10:07.000000 robotframework-debug-4.3.2/tests/test_lib.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `robotframework-debug-4.3.1/.coveragerc` & `robotframework-debug-4.3.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/ChangeLog` & `robotframework-debug-4.3.2/ChangeLog`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/LICENSE` & `robotframework-debug-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/PKG-INFO` & `robotframework-debug-4.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-debug
-Version: 4.3.1
+Version: 4.3.2
 Summary: RobotFramework debug shell
 Home-page: https://github.com/imbus/robotframework-debug/
 Author: René Rohner
 Author-email: snooz@postoe.de
 License: New BSD
 Keywords: robotframework,debug,shell,repl
 Platform: Linux
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Debug Library for Robot Framework
 =================================
 
 .. contents::
```

### Comparing `robotframework-debug-4.3.1/README.rst` & `robotframework-debug-4.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/RobotDebug/RobotDebug.py` & `robotframework-debug-4.3.2/RobotDebug/RobotDebug.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/RobotDebug/cmdcompleter.py` & `robotframework-debug-4.3.2/RobotDebug/cmdcompleter.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/RobotDebug/debugcmd.py` & `robotframework-debug-4.3.2/RobotDebug/debugcmd.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/RobotDebug/history_app.py` & `robotframework-debug-4.3.2/RobotDebug/history_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,32 +53,16 @@
     return base
 
 
 def run_history(context):
     buffer1 = Buffer()
     buffer2 = Buffer()
     his: FileHistory = context.history
-    history = list(
-        reversed(
-            [
-                re.sub(r" {2,}", "    ", e).strip()
-                for e in dict.fromkeys(reversed(his.get_strings()))
-                if not HEADER_MATCHER.match(e)
-            ]
-        )
-    )
-    kw_history = list(
-        reversed(
-            [
-                re.sub(r" {2,}", "    ", e).strip()
-                for e in dict.fromkeys(reversed(his.get_strings()))
-                if HEADER_MATCHER.match(e)
-            ]
-        )
-    )
+    history = get_history_content(his)
+    kw_history = get_history_content(his, False)
     buffer1.text = "\n".join(history)
     buffer1.cursor_position = len(buffer1.text)
     buffer1.read_only = Always()
     window1 = Window(
         content=BufferControl(buffer=buffer1, lexer=PygmentsLexer(RobotFrameworkLocalLexer))
     )
     vsplits = [
@@ -140,7 +124,22 @@
         include_default_pygments_style=False,
         key_bindings=create_keybindings(context),
         layout=layout,
         mouse_support=True,
         style=context.prompt_style,
     )
     app.run()
+
+
+def get_history_content(his, pure_commands: bool = True):
+    return list(
+        reversed(
+            [
+                e
+                for e in dict.fromkeys(
+                    reversed([re.sub(r" {2,}", " " * 4, v).strip() for v in his.get_strings()])
+                )
+                if (not HEADER_MATCHER.match(e) and pure_commands)
+                or (HEADER_MATCHER.match(e) and not pure_commands)
+            ]
+        )
+    )
```

### Comparing `robotframework-debug-4.3.1/RobotDebug/lexer.py` & `robotframework-debug-4.3.2/RobotDebug/lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from robot.parsing import get_tokens
 
 
 def get_robot_token_from_file(file: Path):
     return list(get_tokens(file))
 
 
-HEADER_MATCHER = re.compile(r"\*+ ?(keywords?|settings?|variables?|comments?) ?\**", re.IGNORECASE)
+HEADER_MATCHER = re.compile(
+    r"\s*\*+ ?(keywords?|settings?|variables?|comments?) ?\**", re.IGNORECASE
+)
 
 
 def get_robot_token(text):
     if HEADER_MATCHER.match(text):
         yield from get_tokens(text)
     else:
         marker_len = 20
```

### Comparing `robotframework-debug-4.3.1/RobotDebug/prompttoolkitcmd.py` & `robotframework-debug-4.3.2/RobotDebug/prompttoolkitcmd.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/RobotDebug/robotkeyword.py` & `robotframework-debug-4.3.2/RobotDebug/robotkeyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/RobotDebug/robotlib.py` & `robotframework-debug-4.3.2/RobotDebug/robotlib.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/RobotDebug/shell.py` & `robotframework-debug-4.3.2/RobotDebug/shell.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/RobotDebug/sourcelines.py` & `robotframework-debug-4.3.2/RobotDebug/sourcelines.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/RobotDebug/styles.py` & `robotframework-debug-4.3.2/RobotDebug/styles.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/pyproject.toml` & `robotframework-debug-4.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/robotframework_debug.egg-info/PKG-INFO` & `robotframework-debug-4.3.2/robotframework_debug.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-debug
-Version: 4.3.1
+Version: 4.3.2
 Summary: RobotFramework debug shell
 Home-page: https://github.com/imbus/robotframework-debug/
 Author: René Rohner
 Author-email: snooz@postoe.de
 License: New BSD
 Keywords: robotframework,debug,shell,repl
 Platform: Linux
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Debug Library for Robot Framework
 =================================
 
 .. contents::
```

### Comparing `robotframework-debug-4.3.1/robotframework_debug.egg-info/SOURCES.txt` & `robotframework-debug-4.3.2/robotframework_debug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/setup.py` & `robotframework-debug-4.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     keywords="robotframework,debug,shell,repl",
     install_requires=[
         "prompt-toolkit >= 3.0.38",
         "robotframework >= 5.0",
         "pygments >= 2.14.0",
         "pyperclip >= 1.8.2",
     ],
-    python_requires=">=3.7.0",
+    python_requires=">=3.8.0",
     tests_require=["pexpect", "coverage", "docutils"],
     test_suite="tests.test_debuglibrary.suite",
     platforms=["Linux", "Unix", "Windows", "MacOS X"],
     classifiers=[
         "Environment :: Console",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: BSD License",
```

### Comparing `robotframework-debug-4.3.1/tests/demo.py` & `robotframework-debug-4.3.2/tests/demo.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/tests/step.robot` & `robotframework-debug-4.3.2/tests/step.robot`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/tests/step_listener.robot` & `robotframework-debug-4.3.2/tests/step_listener.robot`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/tests/test_debuglibrary.py` & `robotframework-debug-4.3.2/tests/test_debuglibrary.py`

 * *Files identical despite different names*

### Comparing `robotframework-debug-4.3.1/tests/test_lib.py` & `robotframework-debug-4.3.2/tests/test_lib.py`

 * *Files identical despite different names*

