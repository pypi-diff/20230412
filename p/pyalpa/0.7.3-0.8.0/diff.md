# Comparing `tmp/pyalpa-0.7.3.tar.gz` & `tmp/pyalpa-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalpa-0.7.3.tar", max compression
+gzip compressed data, was "pyalpa-0.8.0.tar", max compression
```

## Comparing `pyalpa-0.7.3.tar` & `pyalpa-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2023-04-12 18:21:09.052332 pyalpa-0.7.3/LICENSE
--rw-r--r--   0        0        0     1631 2023-04-12 18:21:09.052332 pyalpa-0.7.3/README.md
--rw-r--r--   0        0        0        0 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/cli/__init__.py
--rw-r--r--   0        0        0      732 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/cli/alpa_repo.py
--rw-r--r--   0        0        0     1249 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/cli/base.py
--rw-r--r--   0        0        0     6408 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/cli/local_repo.py
--rw-r--r--   0        0        0      227 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/config/__init__.py
--rw-r--r--   0        0        0     1264 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/config/alpa_local.py
--rw-r--r--   0        0        0     2184 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/config/alpa_repo.py
--rw-r--r--   0        0        0     1157 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/config/base.py
--rw-r--r--   0        0        0     2759 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/config/metadata.py
--rw-r--r--   0        0        0     2790 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/config/packit.py
--rw-r--r--   0        0        0     1233 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/constants.py
--rw-r--r--   0        0        0      158 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/exceptions.py
--rw-r--r--   0        0        0     4021 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/gh.py
--rw-r--r--   0        0        0     2463 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/git.py
--rw-r--r--   0        0        0     1447 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/messages.py
--rw-r--r--   0        0        0        0 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/repository/__init__.py
--rw-r--r--   0        0        0    11490 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/repository/base.py
--rw-r--r--   0        0        0     4331 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/repository/branch.py
--rw-r--r--   0        0        0     1661 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/repository/subdirectory.py
--rw-r--r--   0        0        0     3879 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/upstream_integration.py
--rw-r--r--   0        0        0      846 2023-04-12 18:21:09.056331 pyalpa-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 pyalpa-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 21:05:18.616059 pyalpa-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1631 2023-04-12 21:05:18.616059 pyalpa-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/cli/__init__.py
+-rw-r--r--   0        0        0      732 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/cli/alpa_repo.py
+-rw-r--r--   0        0        0     1249 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/cli/base.py
+-rw-r--r--   0        0        0     6243 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/cli/local_repo.py
+-rw-r--r--   0        0        0      227 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/config/__init__.py
+-rw-r--r--   0        0        0     1264 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/config/alpa_local.py
+-rw-r--r--   0        0        0     2184 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/config/alpa_repo.py
+-rw-r--r--   0        0        0     1157 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/config/base.py
+-rw-r--r--   0        0        0     2759 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/config/metadata.py
+-rw-r--r--   0        0        0     2790 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/config/packit.py
+-rw-r--r--   0        0        0     1233 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/constants.py
+-rw-r--r--   0        0        0      158 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/exceptions.py
+-rw-r--r--   0        0        0     4021 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/gh.py
+-rw-r--r--   0        0        0     2463 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/git.py
+-rw-r--r--   0        0        0     1447 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/messages.py
+-rw-r--r--   0        0        0        0 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/repository/__init__.py
+-rw-r--r--   0        0        0    11699 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/repository/base.py
+-rw-r--r--   0        0        0     4536 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/repository/branch.py
+-rw-r--r--   0        0        0     1661 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/repository/subdirectory.py
+-rw-r--r--   0        0        0     3879 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/upstream_integration.py
+-rw-r--r--   0        0        0      846 2023-04-12 21:05:18.616059 pyalpa-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 pyalpa-0.8.0/PKG-INFO
```

### Comparing `pyalpa-0.7.3/LICENSE` & `pyalpa-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/README.md` & `pyalpa-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/alpa/cli/alpa_repo.py` & `pyalpa-0.8.0/alpa/cli/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/alpa/cli/base.py` & `pyalpa-0.8.0/alpa/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/alpa/cli/local_repo.py` & `pyalpa-0.8.0/alpa/cli/local_repo.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,18 +104,14 @@
             f"user {alpa.gh_api.gh_user}"
         ),
         source_branch=f"{local_repo.feat_branch}",
         target_branch=local_repo.package,
     )
     click.echo(f"PR#{pr.number} created. URL: {pr.html_url}")
 
-    # go from feat branch to package branch
-    local_repo.git_cmd(["switch", local_repo.package])
-    local_repo.git_cmd(["branch", "-D", local_repo.feat_branch])
-
 
 @click.command("pull")
 def pull() -> None:
     """Pull last recent changes of package you are on from Alpa repo"""
     local_repo = LocalRepoBranch(Path(getcwd()))
     local_repo.pull(local_repo.branch)
```

### Comparing `pyalpa-0.7.3/alpa/config/alpa_local.py` & `pyalpa-0.8.0/alpa/config/alpa_local.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/alpa/config/alpa_repo.py` & `pyalpa-0.8.0/alpa/config/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/alpa/config/base.py` & `pyalpa-0.8.0/alpa/config/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/alpa/config/metadata.py` & `pyalpa-0.8.0/alpa/config/metadata.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/alpa/config/packit.py` & `pyalpa-0.8.0/alpa/config/packit.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/alpa/constants.py` & `pyalpa-0.8.0/alpa/constants.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/alpa/gh.py` & `pyalpa-0.8.0/alpa/gh.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/alpa/git.py` & `pyalpa-0.8.0/alpa/git.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/alpa/messages.py` & `pyalpa-0.8.0/alpa/messages.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/alpa/repository/base.py` & `pyalpa-0.8.0/alpa/repository/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         if without_git_suffix.startswith("https://") or without_git_suffix.startswith(
             "http://"
         ):
             logger.info(f"Git remote url is in https form {without_git_suffix}")
             split = without_git_suffix.split("/")
             return f"{split[-2]}/{split[-1]}"
 
-        return url.split(":")[-1]
+        return without_git_suffix.split(":")[-1]
 
     def full_reponame(self) -> str:
         logger.debug(f"Trying to find {self.remote_name} in {self.remotes}")
         for remote in self.remotes:
             if remote == self.remote_name:
                 remote_url = self.git_cmd(
                     ["config", "--get", f"remote.{remote}.url"]
@@ -288,14 +288,18 @@
         logger.debug("There are no remotes in this repo")
         return ""
 
     @property
     def git_root(self) -> Path:
         return Path(self.git.git_root)
 
+    def is_branch_merged(self, branch: str) -> bool:
+        ret = self.git_cmd(["fetch", self.remote_name, branch])
+        return ret.retval != 0 and "couldn't find remote ref" in ret.stderr
+
 
 class AlpaRepo(LocalRepo):
     def __init__(self, repo_path: Path, gh_api: Optional[GithubAPI] = None) -> None:
         super().__init__(repo_path)
 
         self.gh_api = gh_api or GithubAPI(self.repo_name)
         self.gh_repo = self.gh_api.get_repo(self.namespace, self.repo_name)
```

### Comparing `pyalpa-0.7.3/alpa/repository/branch.py` & `pyalpa-0.8.0/alpa/repository/branch.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,21 @@
             click.echo(
                 "Repo is dirty, please commit your changes before switching to"
                 f" another package.\n {self.get_status_output()}"
             )
             return None
 
         feat_branch = self.get_feat_branch_of_package(package)
-        branch_to_switch = feat_branch if self.branch_exists(feat_branch) else package
+        if self.branch_exists(feat_branch) and not self.is_branch_merged(feat_branch):
+            branch_to_switch = feat_branch
+        else:
+            branch_to_switch = package
+            if self.branch_exists(feat_branch):
+                self.git_cmd(["branch", "-D", feat_branch])
+
         result = self.git_cmd(["switch", branch_to_switch])
         if result.retval == 0:
             click.echo(result.stdout.replace("branch", "package"))
         else:
             click.echo(f"Switching to the package {package} for the first time")
             click.echo(
                 self.git_cmd(["fetch", self.remote_name, branch_to_switch]).stdout
```

### Comparing `pyalpa-0.7.3/alpa/repository/subdirectory.py` & `pyalpa-0.8.0/alpa/repository/subdirectory.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/alpa/upstream_integration.py` & `pyalpa-0.8.0/alpa/upstream_integration.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.3/pyproject.toml` & `pyalpa-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyalpa"
-version = "0.7.3"
+version = "0.8.0"
 description = "Integration tool with Alpa repository"
 authors = ["Jiri Kyjovsky <j1.kyjovsky@gmail.com>"]
 maintainers = ["Jiří Kyjovský <j1.kyjovsky@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/alpa-team/alpa"
 repository = "https://github.com/alpa-team/alpa"
```

### Comparing `pyalpa-0.7.3/PKG-INFO` & `pyalpa-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalpa
-Version: 0.7.3
+Version: 0.8.0
 Summary: Integration tool with Alpa repository
 Home-page: https://github.com/alpa-team/alpa
 License: GPLv3
 Author: Jiri Kyjovsky
 Author-email: j1.kyjovsky@gmail.com
 Maintainer: Jiří Kyjovský
 Maintainer-email: j1.kyjovsky@gmail.com
```

