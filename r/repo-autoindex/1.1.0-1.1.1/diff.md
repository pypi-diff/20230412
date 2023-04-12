# Comparing `tmp/repo_autoindex-1.1.0.tar.gz` & `tmp/repo_autoindex-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo_autoindex-1.1.0.tar", max compression
+gzip compressed data, was "repo_autoindex-1.1.1.tar", max compression
```

## Comparing `repo_autoindex-1.1.0.tar` & `repo_autoindex-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35149 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/LICENSE
--rw-r--r--   0        0        0     1612 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/README.md
--rw-r--r--   0        0        0      967 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      210 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/repo_autoindex/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/repo_autoindex/_impl/__init__.py
--rw-r--r--   0        0        0     5372 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/repo_autoindex/_impl/api.py
--rw-r--r--   0        0        0     2085 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/repo_autoindex/_impl/base.py
--rw-r--r--   0        0        0     1526 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/repo_autoindex/_impl/cmd.py
--rw-r--r--   0        0        0     8532 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/repo_autoindex/_impl/kickstart.py
--rw-r--r--   0        0        0     2511 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/repo_autoindex/_impl/pulp.py
--rw-r--r--   0        0        0     1551 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/repo_autoindex/_impl/template.py
--rw-r--r--   0        0        0      580 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/repo_autoindex/_impl/templates/index.html.j2
--rw-r--r--   0        0        0     2203 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/repo_autoindex/_impl/tree.py
--rw-r--r--   0        0        0     8364 2023-04-03 23:58:47.613748 repo_autoindex-1.1.0/repo_autoindex/_impl/yum.py
--rw-r--r--   0        0        0     2418 1970-01-01 00:00:00.000000 repo_autoindex-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 04:09:01.773423 repo_autoindex-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1710 2023-04-12 04:09:01.773423 repo_autoindex-1.1.1/README.md
+-rw-r--r--   0        0        0      967 2023-04-12 04:09:01.773423 repo_autoindex-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-04-12 04:09:01.773423 repo_autoindex-1.1.1/repo_autoindex/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 04:09:01.773423 repo_autoindex-1.1.1/repo_autoindex/_impl/__init__.py
+-rw-r--r--   0        0        0     5372 2023-04-12 04:09:01.773423 repo_autoindex-1.1.1/repo_autoindex/_impl/api.py
+-rw-r--r--   0        0        0     2085 2023-04-12 04:09:01.773423 repo_autoindex-1.1.1/repo_autoindex/_impl/base.py
+-rw-r--r--   0        0        0     1526 2023-04-12 04:09:01.773423 repo_autoindex-1.1.1/repo_autoindex/_impl/cmd.py
+-rw-r--r--   0        0        0     8599 2023-04-12 04:09:01.777423 repo_autoindex-1.1.1/repo_autoindex/_impl/kickstart.py
+-rw-r--r--   0        0        0     2511 2023-04-12 04:09:01.777423 repo_autoindex-1.1.1/repo_autoindex/_impl/pulp.py
+-rw-r--r--   0        0        0     1551 2023-04-12 04:09:01.777423 repo_autoindex-1.1.1/repo_autoindex/_impl/template.py
+-rw-r--r--   0        0        0      580 2023-04-12 04:09:01.777423 repo_autoindex-1.1.1/repo_autoindex/_impl/templates/index.html.j2
+-rw-r--r--   0        0        0     2203 2023-04-12 04:09:01.777423 repo_autoindex-1.1.1/repo_autoindex/_impl/tree.py
+-rw-r--r--   0        0        0     8364 2023-04-12 04:09:01.777423 repo_autoindex-1.1.1/repo_autoindex/_impl/yum.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 repo_autoindex-1.1.1/PKG-INFO
```

### Comparing `repo_autoindex-1.1.0/LICENSE` & `repo_autoindex-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_autoindex-1.1.0/README.md` & `repo_autoindex-1.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 ```
 
 See [the manual](https://release-engineering.github.io/repo-autoindex/) for more
 information about the usage of `repo-autoindex`.
 
 ## Changelog
 
+### v1.1.1 - 2023-04-12
+
+- Fix handling of kickstart repositories with no checksums in treeinfo.
+
 ### v1.1.0 - 2023-04-04
 
 - Added limited support for kickstart repositories.
 
 ### v1.0.2 - 2022-10-21
 
 - Reduced memory usage when handling large yum repositories.
```

### Comparing `repo_autoindex-1.1.0/pyproject.toml` & `repo_autoindex-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "repo-autoindex"
-version = "1.1.0"
+version = "1.1.1"
 description = "Generic static HTML indexes of various repository types"
 authors = ["Rohan McGovern <rmcgover@redhat.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/release-engineering/repo-autoindex"
 repository = "https://github.com/release-engineering/repo-autoindex"
```

### Comparing `repo_autoindex-1.1.0/repo_autoindex/_impl/api.py` & `repo_autoindex-1.1.1/repo_autoindex/_impl/api.py`

 * *Files identical despite different names*

### Comparing `repo_autoindex-1.1.0/repo_autoindex/_impl/base.py` & `repo_autoindex-1.1.1/repo_autoindex/_impl/base.py`

 * *Files identical despite different names*

### Comparing `repo_autoindex-1.1.0/repo_autoindex/_impl/cmd.py` & `repo_autoindex-1.1.1/repo_autoindex/_impl/cmd.py`

 * *Files identical despite different names*

### Comparing `repo_autoindex-1.1.0/repo_autoindex/_impl/kickstart.py` & `repo_autoindex-1.1.1/repo_autoindex/_impl/kickstart.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,23 +128,23 @@
                 text="treeinfo",
                 size=str(len(self.treeinfo_content)),
             ),
         ]
 
         treeinfo = configparser.ConfigParser()
         treeinfo.read_string(self.treeinfo_content)
-
-        for image in treeinfo["checksums"]:
-            entry = IndexEntry(
-                href=image,
-                text=os.path.basename(image),
-            )
-            if entry.href.endswith(".iso") or entry.href.endswith(".img"):
-                entry.icon = ICON_OPTICAL
-            out.append(entry)
+        if "checksums" in treeinfo:
+            for image in treeinfo["checksums"]:
+                entry = IndexEntry(
+                    href=image,
+                    text=os.path.basename(image),
+                )
+                if entry.href.endswith(".iso") or entry.href.endswith(".img"):
+                    entry.icon = ICON_OPTICAL
+                out.append(entry)
         return out
 
     async def _extra_files_entries(self) -> list[IndexEntry]:
         """
         An extra_files.json file might look like this:
 
         {
```

### Comparing `repo_autoindex-1.1.0/repo_autoindex/_impl/pulp.py` & `repo_autoindex-1.1.1/repo_autoindex/_impl/pulp.py`

 * *Files identical despite different names*

### Comparing `repo_autoindex-1.1.0/repo_autoindex/_impl/template.py` & `repo_autoindex-1.1.1/repo_autoindex/_impl/template.py`

 * *Files identical despite different names*

### Comparing `repo_autoindex-1.1.0/repo_autoindex/_impl/templates/index.html.j2` & `repo_autoindex-1.1.1/repo_autoindex/_impl/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `repo_autoindex-1.1.0/repo_autoindex/_impl/tree.py` & `repo_autoindex-1.1.1/repo_autoindex/_impl/tree.py`

 * *Files identical despite different names*

### Comparing `repo_autoindex-1.1.0/repo_autoindex/_impl/yum.py` & `repo_autoindex-1.1.1/repo_autoindex/_impl/yum.py`

 * *Files identical despite different names*

### Comparing `repo_autoindex-1.1.0/PKG-INFO` & `repo_autoindex-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-autoindex
-Version: 1.1.0
+Version: 1.1.1
 Summary: Generic static HTML indexes of various repository types
 Home-page: https://github.com/release-engineering/repo-autoindex
 License: GPL-3.0-or-later
 Author: Rohan McGovern
 Author-email: rmcgover@redhat.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -40,14 +40,18 @@
 ```
 
 See [the manual](https://release-engineering.github.io/repo-autoindex/) for more
 information about the usage of `repo-autoindex`.
 
 ## Changelog
 
+### v1.1.1 - 2023-04-12
+
+- Fix handling of kickstart repositories with no checksums in treeinfo.
+
 ### v1.1.0 - 2023-04-04
 
 - Added limited support for kickstart repositories.
 
 ### v1.0.2 - 2022-10-21
 
 - Reduced memory usage when handling large yum repositories.
```

