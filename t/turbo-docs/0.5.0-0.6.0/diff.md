# Comparing `tmp/turbo_docs-0.5.0.tar.gz` & `tmp/turbo_docs-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\turbo_docs-0.5.0.tar", last modified: Mon Apr 10 22:55:37 2023, max compression
+gzip compressed data, was "turbo_docs-0.6.0.tar", last modified: Wed Apr 12 02:00:08 2023, max compression
```

## Comparing `turbo_docs-0.5.0.tar` & `turbo_docs-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 22:55:37.484126 turbo_docs-0.5.0/
--rw-rw-rw-   0        0        0      452 2023-04-10 22:55:37.482612 turbo_docs-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1611 2023-04-10 22:45:42.000000 turbo_docs-0.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 22:55:37.484126 turbo_docs-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      784 2023-04-10 22:55:32.000000 turbo_docs-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:55:37.466251 turbo_docs-0.5.0/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.5.0/turbo_docs/__init__.py
--rw-rw-rw-   0        0        0     2021 2023-04-10 22:41:35.000000 turbo_docs-0.5.0/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:55:37.481607 turbo_docs-0.5.0/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.5.0/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      717 2023-04-10 22:20:57.000000 turbo_docs-0.5.0/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     1796 2023-04-10 22:44:30.000000 turbo_docs-0.5.0/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      566 2023-04-10 22:51:04.000000 turbo_docs-0.5.0/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:55:37.475614 turbo_docs-0.5.0/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0      452 2023-04-10 22:55:37.000000 turbo_docs-0.5.0/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-04-10 22:55:37.000000 turbo_docs-0.5.0/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 22:55:37.000000 turbo_docs-0.5.0/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-10 22:55:37.000000 turbo_docs-0.5.0/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-04-10 22:55:37.000000 turbo_docs-0.5.0/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-10 22:55:37.000000 turbo_docs-0.5.0/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 02:00:08.139047 turbo_docs-0.6.0/
+-rw-rw-rw-   0        0        0      520 2023-04-12 02:00:08.138047 turbo_docs-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1213 2023-04-12 01:09:37.000000 turbo_docs-0.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 02:00:08.140047 turbo_docs-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-04-12 02:00:02.000000 turbo_docs-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:00:08.118048 turbo_docs-0.6.0/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.0/turbo_docs/__init__.py
+-rw-rw-rw-   0        0        0     3456 2023-04-12 01:08:34.000000 turbo_docs-0.6.0/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:00:08.136051 turbo_docs-0.6.0/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.0/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      893 2023-04-12 00:51:47.000000 turbo_docs-0.6.0/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1794 2023-04-11 19:29:42.000000 turbo_docs-0.6.0/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      566 2023-04-10 22:51:04.000000 turbo_docs-0.6.0/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:00:08.129049 turbo_docs-0.6.0/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-04-12 02:00:07.000000 turbo_docs-0.6.0/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-12 02:00:08.000000 turbo_docs-0.6.0/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 02:00:07.000000 turbo_docs-0.6.0/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-12 02:00:07.000000 turbo_docs-0.6.0/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-04-12 02:00:07.000000 turbo_docs-0.6.0/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-12 02:00:08.000000 turbo_docs-0.6.0/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.5.0/setup.py` & `turbo_docs-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="turbo_docs",
-    version="0.5.0",
+    version="0.6.0",
     packages=find_packages(),
     install_requires=[
         "requests",
         "openai",
         "click",
         "pyperclip",
     ],
```

### Comparing `turbo_docs-0.5.0/turbo_docs/generate.py` & `turbo_docs-0.6.0/turbo_docs/generate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,72 @@
 import click
 import os
+from pathlib import Path
 import pyperclip
 from turbo_docs.utils import directory, openai_api, cli_options
 
 
 def run_create_readme(text):
-    """ Generates a README.md
+    """ Generate a formatted and user-friendly README.md file using the provided text.
     """
     prompt = f"Create a formatted & user-friendly readme.md from the following:\n\n{text}"
     response = openai_api.gpt_completion_wrapper(prompt)
     with open("README.md", "w") as readme_file:
         readme_file.write(response)
     print(f"(--create_readme) Generated README.md")
 
 
 def run_create_readme_plus(files):
-    """ Extends the run_create_readme function to handle larger repos
+    """ Generate a README.md file with summarized code content from the provided files.
     """
     responses = {}
     for file_path, file_content in files.items():
         if os.stat(file_path).st_size and file_path.split(".")[1]:
-            print(f"(--create_readme_plus) Summarizing from {file_path}")
+            print(f"(--create_readme_plus) Summarizing {file_path}")
             prompt = f"Summarize the following code, especially maintaining key logic:\n{file_content}"
             responses[file_path] = openai_api.gpt_completion_wrapper(prompt)
+
     psuedocode = "\n\n\n".join([f"{file_path}:\n{summary}" for file_path, summary in responses.items()])
     run_create_readme(psuedocode)
     print(f"(--create_readme_plus) Generated README.md")
 
 
+def run_create_tests(test_file_path, file_content):
+    """ Generate unit tests for the provided code file content and save them in a test file.
+    """
+    print(f"(--create_tests) Generating unit tests for {test_file_path}")
+    prompt = f"Generate unit tests for the following code:\n{file_content}"
+    test_content = openai_api.gpt_completion_wrapper(prompt)
+    with open(test_file_path, "w") as test_file:
+        test_file.write(test_content)
+
+
+def run_create_tests_helper(files):
+    """ Create unit tests for the provided code files and save them in a 'tests' directory.
+    """
+    tests_dir = "tests"
+    Path(tests_dir).mkdir(exist_ok=True)
+
+    for file_path, file_content in files.items():
+        if os.stat(file_path).st_size and file_path.split(".")[1]:
+            test_file_name = f"test_{os.path.basename(file_path)}"
+            test_file_path = os.path.join(tests_dir, test_file_name)
+    
+            resp = input(f"Would you like to create unit tests for {test_file_name} (Y/n):")
+            if resp != "n" and resp != "N":
+                run_create_tests(test_file_path, file_content)
+
+
 @click.command()
 @cli_options.copy
 @cli_options.create_readme
 @cli_options.create_readme_plus
-def driver(copy: bool, create_readme: bool, create_readme_plus: bool) -> None:
-    """ Main driver function that generates a README.md file for the current repository.
+@cli_options.create_tests
+def driver(copy: bool, create_readme: bool, create_readme_plus: bool, create_tests: bool) -> None:
+    """ The main driver function that handles various command-line options for generating documentation and tests.
     """
     files = directory.get_files()
     dir_text = "\n\n".join([f"{name}:\n\n{content}" for name, content in files.items()])
 
     # Copy directory text to clipboard if specified
     if copy:
         pyperclip.copy(dir_text)
@@ -47,10 +76,14 @@
     if create_readme:
         run_create_readme(dir_text)
 
     # Generate docs.md file if specified
     if create_readme_plus:
         run_create_readme_plus(files)
 
+    # Generate unit tests for each code file if specified
+    if create_tests:
+        run_create_tests_helper(files)
+
 
 if __name__ == '__main__':
     driver()
```

### Comparing `turbo_docs-0.5.0/turbo_docs/utils/directory.py` & `turbo_docs-0.6.0/turbo_docs/utils/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from pathlib import Path
 from typing import List, Dict
 
 def ignored_files_init() -> List[str]:
     """ Initialize a list of ignored files and including README.md, docs.md, etc.
     """
-    ignored_files = ["README.md", "docs.md"]
+    ignored_files = ["README.md", "tests"]
     for file in os.listdir():
         if file[0] == ".":
             ignored_files.append(file)
     return ignored_files
 
 def read_gitignore() -> List[str]:
     """ Read .gitignore file and return the list of ignored files.
```

### Comparing `turbo_docs-0.5.0/turbo_docs/utils/openai_api.py` & `turbo_docs-0.6.0/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

