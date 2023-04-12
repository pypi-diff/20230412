# Comparing `tmp/developergpt-0.1.4.tar.gz` & `tmp/developergpt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.1.4.tar", last modified: Thu Apr  6 01:53:05 2023, max compression
+gzip compressed data, was "developergpt-0.1.5.tar", last modified: Wed Apr 12 15:33:31 2023, max compression
```

## Comparing `developergpt-0.1.4.tar` & `developergpt-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:53:05.013609 developergpt-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-06 01:52:55.000000 developergpt-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-06 01:52:55.000000 developergpt-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-06 01:53:05.013609 developergpt-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-06 01:52:55.000000 developergpt-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:53:05.013609 developergpt-0.1.4/developergpt/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-06 01:52:55.000000 developergpt-0.1.4/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 01:52:55.000000 developergpt-0.1.4/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-06 01:52:55.000000 developergpt-0.1.4/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-06 01:52:55.000000 developergpt-0.1.4/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-06 01:52:55.000000 developergpt-0.1.4/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-06 01:52:55.000000 developergpt-0.1.4/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-06 01:52:55.000000 developergpt-0.1.4/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-04-06 01:52:55.000000 developergpt-0.1.4/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:53:05.013609 developergpt-0.1.4/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-06 01:53:04.000000 developergpt-0.1.4/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-06 01:53:04.000000 developergpt-0.1.4/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 01:53:04.000000 developergpt-0.1.4/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-06 01:53:04.000000 developergpt-0.1.4/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-06 01:53:04.000000 developergpt-0.1.4/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-06 01:53:04.000000 developergpt-0.1.4/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 01:53:05.013609 developergpt-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-06 01:52:55.000000 developergpt-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:53:05.013609 developergpt-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 01:52:55.000000 developergpt-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-06 01:52:55.000000 developergpt-0.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-06 01:52:55.000000 developergpt-0.1.4/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:33:31.058933 developergpt-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 15:33:19.000000 developergpt-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 15:33:19.000000 developergpt-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-12 15:33:31.058933 developergpt-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-12 15:33:19.000000 developergpt-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:33:31.054933 developergpt-0.1.5/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:33:31.058933 developergpt-0.1.5/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-12 15:33:30.000000 developergpt-0.1.5/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 15:33:31.000000 developergpt-0.1.5/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:33:30.000000 developergpt-0.1.5/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 15:33:30.000000 developergpt-0.1.5/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 15:33:30.000000 developergpt-0.1.5/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 15:33:30.000000 developergpt-0.1.5/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:33:31.058933 developergpt-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-12 15:33:19.000000 developergpt-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:33:31.058933 developergpt-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:33:19.000000 developergpt-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 15:33:19.000000 developergpt-0.1.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 15:33:19.000000 developergpt-0.1.5/tests/test_cli.py
```

### Comparing `developergpt-0.1.4/LICENSE` & `developergpt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.4/PKG-INFO` & `developergpt-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.1.4
+Version: 0.1.5
 Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with GPT-3.5 models
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `developergpt-0.1.4/README.md` & `developergpt-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.4/developergpt/cli.py` & `developergpt-0.1.5/developergpt/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,15 +138,20 @@
             commands = huggingface_adapter.model_command(user_input, console)
 
         if not commands:
             continue
 
         # TODO: make this look nicer
         # Give user options to revise query, execute command(s), or quit
-        options = ["Revise Query", "Execute Command(s)", "Quit"]
+        options = [
+            "Revise Query",
+            "Execute Command(s)",
+            "Copy Command(s) to Clipboard",
+            "Quit",
+        ]
         questions = [
             inquirer.List("Next", message="What would you like to do?", choices=options)
         ]
 
         selected_option = inquirer.prompt(questions)["Next"]
 
         if selected_option == "Revise Query":
@@ -158,14 +163,21 @@
             for idx, cmd in enumerate(commands):
                 if cmd:
                     console.print(
                         f"""[bold blue]Executing Command [{idx+1}]: {cmd}[/bold blue]"""
                     )
                     subprocess.run(cmd, shell=True)
 
+            console.print(
+                "[bold blue]Copied executed command(s) to clipboard[/bold blue]"
+            )
+            utils.copy_comands_to_cliboard(commands)
+        elif selected_option == "Copy Command(s) to Clipboard":
+            utils.copy_comands_to_cliboard(commands)
+            console.print("[bold blue]Copied command(s) to clipboard[/bold blue]")
         else:
             console.print("[bold blue]Exiting...\n[/bold blue]")
 
         sys.exit(0)
 
 
 @click.command()
@@ -178,14 +190,22 @@
 
 @click.command()
 @click.pass_context
 def test(ctx):
     pass
 
 
+@click.command(help="Give feedback")
+def feedback():
+    console.print(
+        "Thanks for using DeveloperGPT! You can [bold blue][link=https://forms.gle/J36KbztsRAPHXnrKA]give feedback here[/link][/bold blue]!"
+    )
+
+
 main.add_command(cmd)
 main.add_command(chat)
+main.add_command(feedback)
 # main.add_command(api)
 # main.add_command(test)
 
 if __name__ == "__main__":
     main()
```

### Comparing `developergpt-0.1.4/developergpt/config.py` & `developergpt-0.1.5/developergpt/config.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.4/developergpt/huggingface_adapter.py` & `developergpt-0.1.5/developergpt/huggingface_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.4/developergpt/openai_adapter.py` & `developergpt-0.1.5/developergpt/openai_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.4/developergpt/utils.py` & `developergpt-0.1.5/developergpt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 DeveloperGPT by luo-anthony
 """
 
 
 import os
 import sys
 
+import pyperclip
 import tiktoken
 from prompt_toolkit.completion import Completer, Completion
 from rich.console import Console
 from rich.markdown import Markdown
 from rich.panel import Panel
 
 from developergpt import config
@@ -30,14 +31,18 @@
             title="[bold blue]Command(s)[/bold blue]",
             title_align="left",
             width=panel_width,
         )
     )
 
 
+def copy_comands_to_cliboard(commands: list):
+    pyperclip.copy("\n".join(commands))
+
+
 def prompt_user_input(
     input_request,
     session,
     console,
     completer=None,
     complete_style=None,
     auto_suggest=None,
```

### Comparing `developergpt-0.1.4/developergpt.egg-info/PKG-INFO` & `developergpt-0.1.5/developergpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.1.4
+Version: 0.1.5
 Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with GPT-3.5 models
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `developergpt-0.1.4/developergpt.egg-info/SOURCES.txt` & `developergpt-0.1.5/developergpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.4/setup.py` & `developergpt-0.1.5/setup.py`

 * *Files identical despite different names*

