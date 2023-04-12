# Comparing `tmp/developergpt-0.1.5.tar.gz` & `tmp/developergpt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.1.5.tar", last modified: Wed Apr 12 15:33:31 2023, max compression
+gzip compressed data, was "developergpt-0.1.6.tar", last modified: Wed Apr 12 19:21:34 2023, max compression
```

## Comparing `developergpt-0.1.5.tar` & `developergpt-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:33:31.058933 developergpt-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 15:33:19.000000 developergpt-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 15:33:19.000000 developergpt-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-12 15:33:31.058933 developergpt-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-12 15:33:19.000000 developergpt-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:33:31.054933 developergpt-0.1.5/developergpt/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-12 15:33:19.000000 developergpt-0.1.5/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:33:31.058933 developergpt-0.1.5/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-12 15:33:30.000000 developergpt-0.1.5/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 15:33:31.000000 developergpt-0.1.5/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:33:30.000000 developergpt-0.1.5/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 15:33:30.000000 developergpt-0.1.5/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 15:33:30.000000 developergpt-0.1.5/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 15:33:30.000000 developergpt-0.1.5/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:33:31.058933 developergpt-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-12 15:33:19.000000 developergpt-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:33:31.058933 developergpt-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:33:19.000000 developergpt-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 15:33:19.000000 developergpt-0.1.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 15:33:19.000000 developergpt-0.1.5/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:21:34.556047 developergpt-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 19:21:25.000000 developergpt-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 19:21:25.000000 developergpt-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-12 19:21:34.556047 developergpt-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-12 19:21:25.000000 developergpt-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:21:34.556047 developergpt-0.1.6/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-12 19:21:25.000000 developergpt-0.1.6/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:21:34.556047 developergpt-0.1.6/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-12 19:21:34.000000 developergpt-0.1.6/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 19:21:34.000000 developergpt-0.1.6/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:21:34.000000 developergpt-0.1.6/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 19:21:34.000000 developergpt-0.1.6/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 19:21:34.000000 developergpt-0.1.6/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 19:21:34.000000 developergpt-0.1.6/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 19:21:34.556047 developergpt-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-12 19:21:25.000000 developergpt-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:21:34.556047 developergpt-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:21:25.000000 developergpt-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 19:21:25.000000 developergpt-0.1.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 19:21:25.000000 developergpt-0.1.6/tests/test_cli.py
```

### Comparing `developergpt-0.1.5/LICENSE` & `developergpt-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.5/PKG-INFO` & `developergpt-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.1.5
+Version: 0.1.6
 Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with GPT-3.5 models
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `developergpt-0.1.5/README.md` & `developergpt-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.5/developergpt/cli.py` & `developergpt-0.1.6/developergpt/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from functools import wraps
 
 import click
 import inquirer
 import openai
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
+from prompt_toolkit.key_binding import KeyBindings
+from prompt_toolkit.key_binding.key_processor import KeyPressEvent
+from prompt_toolkit.keys import Keys
 from prompt_toolkit.shortcuts import CompleteStyle
 from rich.console import Console
 
 from developergpt import config, huggingface_adapter, openai_adapter, utils
 
 console = Console()
 session: "PromptSession" = PromptSession()
@@ -107,31 +110,47 @@
         n_output_tokens = max(RESERVED_OUTPUT_TOKENS, MAX_TOKENS - n_input_tokens)
         full_response = openai_adapter.get_model_chat_response(
             MODEL, console, input_messages, n_output_tokens, ctx.obj["temperature"]
         )
         input_messages.append({"role": "assistant", "content": full_response})
 
 
+kb = KeyBindings()
+
+
+@kb.add(Keys.Enter, eager=True)
+def _(event: KeyPressEvent):
+    buff = event.app.current_buffer
+    if buff.complete_state:
+        # during completion, enter will select the current completion instead of submitting input
+        if buff.complete_state.current_completion:
+            buff.apply_completion(buff.complete_state.current_completion)
+            return  # don't submit input
+    buff.validate_and_handle()
+
+
 @click.command(help="Execute commands using natural language")
 @click.pass_context
 @handle_api_error
 def cmd(ctx):
     input_request = "\nDesired Command Request: "
 
     model = ctx.obj["model"]
     input_messages = copy.deepcopy(openai_adapter.BASE_INPUT_CMD_MSGS)
 
     console.print("[gray]Type 'quit' to exit[/gray]")
+
     while True:
         user_input = utils.prompt_user_input(
             input_request,
             session,
             console,
             completer=utils.PathCompleter(),
             complete_style=CompleteStyle.MULTI_COLUMN,
+            key_bindings=kb,
         )
         if len(user_input) == 0:
             continue
 
         if model == config.GPT35:
             commands = openai_adapter.model_command(user_input, console, input_messages)
         elif model == config.BLOOM:
@@ -178,34 +197,25 @@
             console.print("[bold blue]Exiting...\n[/bold blue]")
 
         sys.exit(0)
 
 
 @click.command()
 @click.pass_context
-def api(ctx):
-    # TODO: API command that exposes api to developer in terminal
-    # NOTE: OpenAI has a command line tool already, this may not be nescessary
-    pass
-
-
-@click.command()
-@click.pass_context
 def test(ctx):
     pass
 
 
 @click.command(help="Give feedback")
 def feedback():
     console.print(
         "Thanks for using DeveloperGPT! You can [bold blue][link=https://forms.gle/J36KbztsRAPHXnrKA]give feedback here[/link][/bold blue]!"
     )
 
 
 main.add_command(cmd)
 main.add_command(chat)
 main.add_command(feedback)
-# main.add_command(api)
 # main.add_command(test)
 
 if __name__ == "__main__":
     main()
```

### Comparing `developergpt-0.1.5/developergpt/config.py` & `developergpt-0.1.6/developergpt/config.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.5/developergpt/huggingface_adapter.py` & `developergpt-0.1.6/developergpt/huggingface_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.5/developergpt/openai_adapter.py` & `developergpt-0.1.6/developergpt/openai_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.5/developergpt/utils.py` & `developergpt-0.1.6/developergpt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,23 @@
 def prompt_user_input(
     input_request,
     session,
     console,
     completer=None,
     complete_style=None,
     auto_suggest=None,
+    key_bindings=None,
 ):
     user_input = session.prompt(
         input_request,
         style=config.INPUT_STYLE,
         completer=completer,
         complete_style=complete_style,
         auto_suggest=auto_suggest,
+        key_bindings=key_bindings,
     ).strip()
 
     if len(user_input) == 0:
         return ""
 
     if user_input.lower() == "quit":
         console.print("[bold blue]Exiting... [/bold blue]")
@@ -165,18 +167,18 @@
                     for f in os.listdir(curr_dir)
                     if fname in f.lower()
                 ]
 
             # Yield the completions
             for completion in auto_completion:
                 # simplify the completion substitution if possible
-                if cwd in completion:
-                    completion = os.path.relpath(completion, cwd)
-                elif text.startswith("~/"):
+                if text.startswith("~/"):
                     completion = completion.replace(os.path.expanduser("~/"), "~/")
+                elif cwd in completion:
+                    completion = os.path.relpath(completion, cwd)
 
                 # substitute for the full path but only display the basename of the file
                 yield Completion(
                     completion,
                     display=os.path.basename(completion),
                     start_position=-len(text),
                 )
```

### Comparing `developergpt-0.1.5/developergpt.egg-info/PKG-INFO` & `developergpt-0.1.6/developergpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.1.5
+Version: 0.1.6
 Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with GPT-3.5 models
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `developergpt-0.1.5/developergpt.egg-info/SOURCES.txt` & `developergpt-0.1.6/developergpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.5/setup.py` & `developergpt-0.1.6/setup.py`

 * *Files identical despite different names*

