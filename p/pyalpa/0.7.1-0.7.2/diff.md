# Comparing `tmp/pyalpa-0.7.1.tar.gz` & `tmp/pyalpa-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalpa-0.7.1.tar", max compression
+gzip compressed data, was "pyalpa-0.7.2.tar", max compression
```

## Comparing `pyalpa-0.7.1.tar` & `pyalpa-0.7.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2023-04-12 17:44:18.651486 pyalpa-0.7.1/LICENSE
--rw-r--r--   0        0        0     1631 2023-04-12 17:44:18.651486 pyalpa-0.7.1/README.md
--rw-r--r--   0        0        0        0 2023-04-12 17:44:18.651486 pyalpa-0.7.1/alpa/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 17:44:18.651486 pyalpa-0.7.1/alpa/cli/__init__.py
--rw-r--r--   0        0        0      732 2023-04-12 17:44:18.651486 pyalpa-0.7.1/alpa/cli/alpa_repo.py
--rw-r--r--   0        0        0     1249 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/cli/base.py
--rw-r--r--   0        0        0     6408 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/cli/local_repo.py
--rw-r--r--   0        0        0      227 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/config/__init__.py
--rw-r--r--   0        0        0     1264 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/config/alpa_local.py
--rw-r--r--   0        0        0     2184 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/config/alpa_repo.py
--rw-r--r--   0        0        0     1157 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/config/base.py
--rw-r--r--   0        0        0     2759 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/config/metadata.py
--rw-r--r--   0        0        0     2790 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/config/packit.py
--rw-r--r--   0        0        0     1233 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/constants.py
--rw-r--r--   0        0        0      158 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/exceptions.py
--rw-r--r--   0        0        0     4021 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/gh.py
--rw-r--r--   0        0        0     2092 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/git.py
--rw-r--r--   0        0        0     1447 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/messages.py
--rw-r--r--   0        0        0        0 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/repository/__init__.py
--rw-r--r--   0        0        0    11039 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/repository/base.py
--rw-r--r--   0        0        0     4331 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/repository/branch.py
--rw-r--r--   0        0        0     1661 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/repository/subdirectory.py
--rw-r--r--   0        0        0     3879 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/upstream_integration.py
--rw-r--r--   0        0        0      846 2023-04-12 17:44:18.655486 pyalpa-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 pyalpa-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 18:03:51.773228 pyalpa-0.7.2/LICENSE
+-rw-r--r--   0        0        0     1631 2023-04-12 18:03:51.773228 pyalpa-0.7.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/cli/__init__.py
+-rw-r--r--   0        0        0      732 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/cli/alpa_repo.py
+-rw-r--r--   0        0        0     1249 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/cli/base.py
+-rw-r--r--   0        0        0     6408 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/cli/local_repo.py
+-rw-r--r--   0        0        0      227 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/config/__init__.py
+-rw-r--r--   0        0        0     1264 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/config/alpa_local.py
+-rw-r--r--   0        0        0     2184 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/config/alpa_repo.py
+-rw-r--r--   0        0        0     1157 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/config/base.py
+-rw-r--r--   0        0        0     2759 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/config/metadata.py
+-rw-r--r--   0        0        0     2790 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/config/packit.py
+-rw-r--r--   0        0        0     1233 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/constants.py
+-rw-r--r--   0        0        0      158 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/exceptions.py
+-rw-r--r--   0        0        0     4021 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/gh.py
+-rw-r--r--   0        0        0     2092 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/git.py
+-rw-r--r--   0        0        0     1447 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/messages.py
+-rw-r--r--   0        0        0        0 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/repository/__init__.py
+-rw-r--r--   0        0        0    11490 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/repository/base.py
+-rw-r--r--   0        0        0     4331 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/repository/branch.py
+-rw-r--r--   0        0        0     1661 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/repository/subdirectory.py
+-rw-r--r--   0        0        0     3879 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/upstream_integration.py
+-rw-r--r--   0        0        0      846 2023-04-12 18:03:51.773228 pyalpa-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 pyalpa-0.7.2/PKG-INFO
```

### Comparing `pyalpa-0.7.1/LICENSE` & `pyalpa-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/README.md` & `pyalpa-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/cli/alpa_repo.py` & `pyalpa-0.7.2/alpa/cli/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/cli/base.py` & `pyalpa-0.7.2/alpa/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/cli/local_repo.py` & `pyalpa-0.7.2/alpa/cli/local_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/config/alpa_local.py` & `pyalpa-0.7.2/alpa/config/alpa_local.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/config/alpa_repo.py` & `pyalpa-0.7.2/alpa/config/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/config/base.py` & `pyalpa-0.7.2/alpa/config/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/config/metadata.py` & `pyalpa-0.7.2/alpa/config/metadata.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/config/packit.py` & `pyalpa-0.7.2/alpa/config/packit.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/constants.py` & `pyalpa-0.7.2/alpa/constants.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/gh.py` & `pyalpa-0.7.2/alpa/gh.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/git.py` & `pyalpa-0.7.2/alpa/git.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/messages.py` & `pyalpa-0.7.2/alpa/messages.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/repository/base.py` & `pyalpa-0.7.2/alpa/repository/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,25 +257,37 @@
     def pull(self, branch: str) -> None:
         click.echo(self.git_cmd(["pull", self.remote_name, branch]).stdout)
 
     def push(self, branch: str) -> None:
         # you always want to push to origin, even from a fork
         click.echo(self.git_cmd(["push", ORIGIN_NAME, branch]).stdout)
 
+    @staticmethod
+    def _parse_reponame_from_url(url: str) -> str:
+        without_git_suffix = url.removesuffix(".git")
+        if without_git_suffix.startswith("https://") or without_git_suffix.startswith(
+            "http://"
+        ):
+            logger.info(f"Git remote url is in https form {without_git_suffix}")
+            split = without_git_suffix.split("/")
+            return f"{split[-2]}/{split[-1]}"
+
+        return url.split(":")[-1]
+
     def full_reponame(self) -> str:
         logger.debug(f"Trying to find {self.remote_name} in {self.remotes}")
         for remote in self.remotes:
             if remote == self.remote_name:
                 remote_url = self.git_cmd(
                     ["config", "--get", f"remote.{remote}.url"]
                 ).stdout
                 logger.debug(
                     f"Remote {remote} found. Parsing its remote url {remote_url}"
                 )
-                return remote_url.split(":")[-1].removesuffix(".git")
+                return self._parse_reponame_from_url(remote_url)
 
         logger.debug("There are no remotes in this repo")
         return ""
 
     @property
     def git_root(self) -> Path:
         return Path(self.git.git_root)
```

### Comparing `pyalpa-0.7.1/alpa/repository/branch.py` & `pyalpa-0.7.2/alpa/repository/branch.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/repository/subdirectory.py` & `pyalpa-0.7.2/alpa/repository/subdirectory.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/alpa/upstream_integration.py` & `pyalpa-0.7.2/alpa/upstream_integration.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.1/pyproject.toml` & `pyalpa-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyalpa"
-version = "0.7.1"
+version = "0.7.2"
 description = "Integration tool with Alpa repository"
 authors = ["Jiri Kyjovsky <j1.kyjovsky@gmail.com>"]
 maintainers = ["Jiří Kyjovský <j1.kyjovsky@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/alpa-team/alpa"
 repository = "https://github.com/alpa-team/alpa"
```

### Comparing `pyalpa-0.7.1/PKG-INFO` & `pyalpa-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalpa
-Version: 0.7.1
+Version: 0.7.2
 Summary: Integration tool with Alpa repository
 Home-page: https://github.com/alpa-team/alpa
 License: GPLv3
 Author: Jiri Kyjovsky
 Author-email: j1.kyjovsky@gmail.com
 Maintainer: Jiří Kyjovský
 Maintainer-email: j1.kyjovsky@gmail.com
```

