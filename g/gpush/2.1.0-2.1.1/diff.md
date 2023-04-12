# Comparing `tmp/gpush-2.1.0.tar.gz` & `tmp/gpush-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpush-2.1.0.tar", last modified: Tue Apr 11 06:40:05 2023, max compression
+gzip compressed data, was "gpush-2.1.1.tar", last modified: Wed Apr 12 19:34:49 2023, max compression
```

## Comparing `gpush-2.1.0.tar` & `gpush-2.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:40:05.609789 gpush-2.1.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-11 06:40:01.000000 gpush-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1300 2023-04-11 06:40:05.609789 gpush-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1188 2023-04-11 06:40:01.000000 gpush-2.1.0/README.md
--rwxr-xr-x   0 root         (0) root         (0)     2549 2023-04-11 06:40:01.000000 gpush-2.1.0/gpush
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:40:05.609789 gpush-2.1.0/gpush.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1300 2023-04-11 06:40:05.000000 gpush-2.1.0/gpush.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      191 2023-04-11 06:40:05.000000 gpush-2.1.0/gpush.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 06:40:05.000000 gpush-2.1.0/gpush.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-11 06:40:05.000000 gpush-2.1.0/gpush.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 06:40:05.000000 gpush-2.1.0/gpush.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-11 06:40:01.000000 gpush-2.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 06:40:05.609789 gpush-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      521 2023-04-11 06:40:02.000000 gpush-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:34:49.469299 gpush-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-12 19:34:46.000000 gpush-2.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-04-12 19:34:49.469299 gpush-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-04-12 19:34:46.000000 gpush-2.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 19:34:47.000000 gpush-2.1.1/_version.py
+-rwxr-xr-x   0 root         (0) root         (0)     3234 2023-04-12 19:34:46.000000 gpush-2.1.1/gpush
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:34:49.469299 gpush-2.1.1/gpush.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-04-12 19:34:49.000000 gpush-2.1.1/gpush.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-04-12 19:34:49.000000 gpush-2.1.1/gpush.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 19:34:49.000000 gpush-2.1.1/gpush.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-04-12 19:34:49.000000 gpush-2.1.1/gpush.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 19:34:49.000000 gpush-2.1.1/gpush.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-12 19:34:46.000000 gpush-2.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 19:34:49.469299 gpush-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      547 2023-04-12 19:34:46.000000 gpush-2.1.1/setup.py
```

### Comparing `gpush-2.1.0/LICENSE` & `gpush-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpush-2.1.0/PKG-INFO` & `gpush-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpush
-Version: 2.1.0
+Version: 2.1.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gpush
 
 `gpush` is a command line utility for standardising commit messages using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
```

### Comparing `gpush-2.1.0/README.md` & `gpush-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gpush-2.1.0/gpush` & `gpush-2.1.1/gpush`

 * *Files 15% similar despite different names*

```diff
@@ -2,59 +2,80 @@
 
 """
 Python script to handle git commit and push to standardise commit messages using conventional commit
 messages.
 
 Usage: gpush
 """
-import sys
 
 import inquirer
 from git import Repo
 import argparse
+from _version import __version__
 
-found_version = False
-with open("setup.py", encoding="UTF-8") as setup_file:
-    for line in setup_file:
-        if line.startswith("__version__"):
-            version = line.split("=")[1].replace("\"","").strip()
-            found_version = True
-
-if not found_version:
-    print("__version__ not detected in setup.py")
-    sys.exit(1)
+version = __version__
 
 parser = argparse.ArgumentParser(
     prog="gpush " + version,
     description="Git commit helper for conventional commit messages",
 )
 parser.add_argument(
-    '--version',
-    action='store_true',
-    help="Option to print the current version only"
+    "--version", action="store_true", help="Option to print the current version only"
 )
+parser.add_argument(
+    "--no-commit",
+    action="store_false",
+    help="[Default: False] Option to enable git commit",
+)
+parser.add_argument(
+    "--no-push",
+    action="store_false",
+    help="[Default: False] Option to enable git push",
+)
+
 args = parser.parse_args()
 
-def git_push(commit_message):
+
+def git_commit(commit_message):
     """
-    Function to push commit up to Git on the current branch for the repository
+    Function to commit changes to Git on the current branch for the repository
     :param commit_message: String containing the conventional commit message formatted commit
     message
     :return: True/False
     """
     try:
         repo = Repo(search_parent_directories=True)
         repo.index.write()
         repo.git.commit("-m" + commit_message)
+        print("committing: " + commit_message)
+        print("Committed successfully")
+    except Exception as error_message:
+        print("Some error occured while committing the code:")
+        print(str(error_message))
+        raise
+
+    return True
+
+
+def git_push():
+    """
+    Function to push commit up to Git on the current branch for the repository
+
+    :return: True/False
+    """
+    try:
+        repo = Repo(search_parent_directories=True)
         repo.git.push("--set-upstream", "origin", repo.active_branch)
-        print("pushing commit: " + commit_message)
         print("Pushed successfully")
     except Exception as error_message:
-        print("Some error occured while pushing the code:")
+        print("Some error occurred while pushing the code:")
         print(str(error_message))
+        raise
+
+    return True
 
 
 def collect_details():
     """
     Function that collects commit message detail from the committer and executes git commit
     and push.
 
@@ -76,18 +97,26 @@
 
     answers = inquirer.prompt(questions)
     if answers["breaking_change"] == "Yes":
         is_breaking_change = "!"
     else:
         is_breaking_change = ""
 
-    commit_message = (
+    commit_message_final = (
         answers["type"] + is_breaking_change + ": " + answers["commit_message"]
     )
-    git_push(commit_message)
+    return commit_message_final
 
 
 if __name__ == "__main__":
     if args.version:
-        print("Current version: " + version)
+        print(version)
     else:
-        collect_details()
+        try:
+            if args.no_commit:
+                commit_message = collect_details()
+                git_commit(commit_message)
+            if args.no_push:
+                git_push()
+        except Exception as error_message:
+            print("Some error occurred while pushing the code:")
+            print(str(error_message))
```

### Comparing `gpush-2.1.0/gpush.egg-info/PKG-INFO` & `gpush-2.1.1/gpush.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpush
-Version: 2.1.0
+Version: 2.1.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gpush
 
 `gpush` is a command line utility for standardising commit messages using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
```

### Comparing `gpush-2.1.0/setup.py` & `gpush-2.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Setup file for python-semantic-versioning
 """
 from setuptools import setup
 
+from _version import __version__
+
 with open("README.md", encoding="UTF-8") as readme_file:
     readme_contents = readme_file.read()
 
 with open("requirements.txt", encoding="UTF-8") as requirements_file:
     required = requirements_file.read().splitlines()
 
-__version__ = "2.1.0"
-
 setup(
     name="gpush",
     version=__version__,
     long_description=readme_contents,
     long_description_content_type="text/markdown",
     install_requires=required,
-    scripts=["gpush"],
+    scripts=["gpush", "_version.py"],
 )
```

