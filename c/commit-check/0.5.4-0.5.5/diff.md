# Comparing `tmp/commit_check-0.5.4-py3-none-any.whl.zip` & `tmp/commit_check-0.5.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 11162 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1735 b- defN 23-Apr-07 04:57 commit_check/__init__.py
--rw-r--r--  2.0 unx     1117 b- defN 23-Apr-07 04:57 commit_check/author.py
--rw-r--r--  2.0 unx      926 b- defN 23-Apr-07 04:57 commit_check/branch.py
--rw-r--r--  2.0 unx     1407 b- defN 23-Apr-07 04:57 commit_check/commit.py
--rw-r--r--  2.0 unx     2675 b- defN 23-Apr-07 04:57 commit_check/error.py
--rw-r--r--  2.0 unx     2919 b- defN 23-Apr-07 04:57 commit_check/main.py
--rw-r--r--  2.0 unx     4748 b- defN 23-Apr-07 04:57 commit_check/util.py
--rw-r--r--  2.0 unx     1095 b- defN 23-Apr-07 04:57 commit_check-0.5.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     8716 b- defN 23-Apr-07 04:57 commit_check-0.5.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 04:57 commit_check-0.5.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 23-Apr-07 04:57 commit_check-0.5.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Apr-07 04:57 commit_check-0.5.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1060 b- defN 23-Apr-07 04:57 commit_check-0.5.4.dist-info/RECORD
-13 files, 26559 bytes uncompressed, 9392 bytes compressed:  64.6%
+Zip file size: 11183 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1735 b- defN 23-Apr-12 06:50 commit_check/__init__.py
+-rw-r--r--  2.0 unx     1117 b- defN 23-Apr-12 06:50 commit_check/author.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Apr-12 06:50 commit_check/branch.py
+-rw-r--r--  2.0 unx     1508 b- defN 23-Apr-12 06:50 commit_check/commit.py
+-rw-r--r--  2.0 unx     2675 b- defN 23-Apr-12 06:50 commit_check/error.py
+-rw-r--r--  2.0 unx     2919 b- defN 23-Apr-12 06:50 commit_check/main.py
+-rw-r--r--  2.0 unx     4748 b- defN 23-Apr-12 06:50 commit_check/util.py
+-rw-r--r--  2.0 unx     1095 b- defN 23-Apr-12 06:51 commit_check-0.5.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8716 b- defN 23-Apr-12 06:51 commit_check-0.5.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 06:51 commit_check-0.5.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 23-Apr-12 06:51 commit_check-0.5.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-12 06:51 commit_check-0.5.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1060 b- defN 23-Apr-12 06:51 commit_check-0.5.5.dist-info/RECORD
+13 files, 26660 bytes uncompressed, 9413 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: commit_check/main.py
 Comment: 
 
 Filename: commit_check/util.py
 Comment: 
 
-Filename: commit_check-0.5.4.dist-info/LICENSE
+Filename: commit_check-0.5.5.dist-info/LICENSE
 Comment: 
 
-Filename: commit_check-0.5.4.dist-info/METADATA
+Filename: commit_check-0.5.5.dist-info/METADATA
 Comment: 
 
-Filename: commit_check-0.5.4.dist-info/WHEEL
+Filename: commit_check-0.5.5.dist-info/WHEEL
 Comment: 
 
-Filename: commit_check-0.5.4.dist-info/entry_points.txt
+Filename: commit_check-0.5.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: commit_check-0.5.4.dist-info/top_level.txt
+Filename: commit_check-0.5.5.dist-info/top_level.txt
 Comment: 
 
-Filename: commit_check-0.5.4.dist-info/RECORD
+Filename: commit_check-0.5.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## commit_check/commit.py

```diff
@@ -10,22 +10,25 @@
     for check in checks:
         if check['check'] == 'message':
             if check['regex'] == "":
                 print(
                     f"{YELLOW}Not found regex for commit message. skip checking.{RESET_COLOR}",
                 )
                 return PASS
-            # check the message of the current commit
-            if os.environ.get("IS_PRE_COMMIT") == "1":
+            commit_msg = ""
+            if os.environ.get("IS_PRE_COMMIT"):
+                # check the message of the current commit
                 git_dir = cmd_output(['git', 'rev-parse', '--git-dir']).strip()
                 commit_msg_file = PurePath(git_dir, "COMMIT_EDITMSG")
-                with open(commit_msg_file, 'r') as f:
-                    commit_msg = f.read()
-            else:  # check the message of the last commit
-                commit_msg = str(get_commits_info("s"))
+                try:
+                    with open(commit_msg_file, 'r') as f:
+                        commit_msg = f.read()
+                except FileNotFoundError:
+                    # check the message of the last commit
+                    commit_msg = str(get_commits_info("s"))
             result = re.match(check['regex'], commit_msg)
             if result is None:
                 print_error_message(
                     check['check'], check['regex'],
                     check['error'], commit_msg,
                 )
                 if check['suggest']:
```

## Comparing `commit_check-0.5.4.dist-info/LICENSE` & `commit_check-0.5.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `commit_check-0.5.4.dist-info/METADATA` & `commit_check-0.5.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commit-check
-Version: 0.5.4
+Version: 0.5.5
 Summary: Check commit message formatting, branch naming, commit author, email, and more.
 Author-email: Peter Shen <xianpeng.shen@gmail.com>
 License: MIT License
 Project-URL: source, https://github.com/commit-check/commit-check
 Project-URL: tracker, https://github.com/commit-check/commit-check/issues
 Keywords: commit conventions,conventional commits,branch naming,commit-check,message,lint message
 Classifier: Development Status :: 4 - Beta
```

