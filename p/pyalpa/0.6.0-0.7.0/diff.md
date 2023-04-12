# Comparing `tmp/pyalpa-0.6.0.tar.gz` & `tmp/pyalpa-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalpa-0.6.0.tar", max compression
+gzip compressed data, was "pyalpa-0.7.0.tar", max compression
```

## Comparing `pyalpa-0.6.0.tar` & `pyalpa-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0    35149 2023-04-11 19:41:22.776185 pyalpa-0.6.0/LICENSE
--rw-r--r--   0        0        0     1631 2023-04-11 19:41:22.776185 pyalpa-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/cli/__init__.py
--rw-r--r--   0        0        0      739 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/cli/alpa_repo.py
--rw-r--r--   0        0        0     1249 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/cli/base.py
--rw-r--r--   0        0        0     6351 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/cli/local_repo.py
--rw-r--r--   0        0        0      227 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/config/__init__.py
--rw-r--r--   0        0        0     1079 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/config/alpa_local.py
--rw-r--r--   0        0        0     2184 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/config/alpa_repo.py
--rw-r--r--   0        0        0     1157 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/config/base.py
--rw-r--r--   0        0        0     2759 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/config/metadata.py
--rw-r--r--   0        0        0     2790 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/config/packit.py
--rw-r--r--   0        0        0     1233 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/constants.py
--rw-r--r--   0        0        0      158 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/exceptions.py
--rw-r--r--   0        0        0     3900 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/gh.py
--rw-r--r--   0        0        0     1447 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/messages.py
--rw-r--r--   0        0        0        0 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/repository/__init__.py
--rw-r--r--   0        0        0    10659 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/repository/base.py
--rw-r--r--   0        0        0     4400 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/repository/branch.py
--rw-r--r--   0        0        0     1661 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/repository/subdirectory.py
--rw-r--r--   0        0        0     3879 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/upstream_integration.py
--rw-r--r--   0        0        0      866 2023-04-11 19:41:22.780185 pyalpa-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 pyalpa-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 16:44:15.732104 pyalpa-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1631 2023-04-12 16:44:15.732104 pyalpa-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/cli/__init__.py
+-rw-r--r--   0        0        0      732 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/cli/alpa_repo.py
+-rw-r--r--   0        0        0     1249 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/cli/base.py
+-rw-r--r--   0        0        0     6410 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/cli/local_repo.py
+-rw-r--r--   0        0        0      227 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/config/__init__.py
+-rw-r--r--   0        0        0     1079 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/config/alpa_local.py
+-rw-r--r--   0        0        0     2184 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/config/alpa_repo.py
+-rw-r--r--   0        0        0     1157 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/config/base.py
+-rw-r--r--   0        0        0     2759 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/config/metadata.py
+-rw-r--r--   0        0        0     2790 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/config/packit.py
+-rw-r--r--   0        0        0     1233 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/constants.py
+-rw-r--r--   0        0        0      158 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/exceptions.py
+-rw-r--r--   0        0        0     3900 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/gh.py
+-rw-r--r--   0        0        0     1804 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/git.py
+-rw-r--r--   0        0        0     1447 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/messages.py
+-rw-r--r--   0        0        0        0 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/repository/__init__.py
+-rw-r--r--   0        0        0    10335 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/repository/base.py
+-rw-r--r--   0        0        0     4331 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/repository/branch.py
+-rw-r--r--   0        0        0     1661 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/repository/subdirectory.py
+-rw-r--r--   0        0        0     3879 2023-04-12 16:44:15.736104 pyalpa-0.7.0/alpa/upstream_integration.py
+-rw-r--r--   0        0        0      846 2023-04-12 16:44:15.736104 pyalpa-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 pyalpa-0.7.0/PKG-INFO
```

### Comparing `pyalpa-0.6.0/LICENSE` & `pyalpa-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalpa-0.6.0/README.md` & `pyalpa-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyalpa-0.6.0/alpa/cli/alpa_repo.py` & `pyalpa-0.7.0/alpa/cli/alpa_repo.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     AlpaRepoBranch(Path(getcwd())).request_package_delete(name)
 
 
 @click.command("request-package")
 @pkg_name
 def request_package(name: str) -> None:
     """Request new branch for new package in Alpa repo"""
-    raise NotImplementedError("Not implemented yet (1.0 goal)")
+    AlpaRepoBranch(Path(getcwd())).request_package(name)
```

### Comparing `pyalpa-0.6.0/alpa/cli/base.py` & `pyalpa-0.7.0/alpa/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.6.0/alpa/cli/local_repo.py` & `pyalpa-0.7.0/alpa/cli/local_repo.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,18 +57,18 @@
     if len(message) > 80:
         raise ClickException("Message longer than 80 characters")
 
     LocalRepoBranch(Path(getcwd())).commit(message, not no_verify)
 
 
 @click.command("add")
-@click.argument("files", type=str, nargs=-1, required=True)
-def add(files: list[str]) -> None:
+@click.argument("to_add", type=str, required=True)
+def add(to_add: str) -> None:
     """Add files to git history. Basically calls `git add <input>`"""
-    LocalRepoBranch(Path(getcwd())).add(files)
+    LocalRepoBranch(Path(getcwd())).add(to_add)
 
 
 @click.command("push")
 @click.option(
     "-p",
     "--pull-request",
     is_flag=True,
@@ -80,23 +80,26 @@
     """Pushes your commited changes to the Alpa repo so you can make PR"""
     repo_path = Path(getcwd())
     local_repo = LocalRepoBranch(repo_path)
 
     packit_conf = PackitConfig(local_repo.package)
     if not packit_conf.packit_config_file_exists():
         packit_conf.create_packit_config()
-        local_repo.git_cmd.add(".packit.yaml")
-        local_repo.git_cmd.commit(
-            '-m "alpa: automatically add .packit.yaml config to the package"'
+        local_repo.git_cmd(["add", ".packit.yaml"])
+        local_repo.git_cmd(
+            [
+                "commit",
+                '-m "alpa: automatically add .packit.yaml config to the package"',
+            ]
         )
 
     local_repo.push(local_repo.branch)
 
     if not pull_request:
-        local_repo.git_cmd.branch("-d", local_repo.feat_branch)
+        local_repo.git_cmd(["branch", "-d", local_repo.feat_branch])
         return
 
     alpa = AlpaRepoBranch(repo_path)
     pr = alpa.gh_repo.create_pr(
         title=f"[alpa-cli] Create update of package {local_repo.package}",
         body=(
             "This PR was created automatically via alpa-cli for "
@@ -104,16 +107,16 @@
         ),
         source_branch=f"{local_repo.feat_branch}",
         target_branch=local_repo.package,
     )
     click.echo(f"PR#{pr.number} created. URL: {pr.html_url}")
 
     # go from feat branch to package branch
-    local_repo.git_cmd.switch(local_repo.package)
-    local_repo.git_cmd.branch("-D", local_repo.feat_branch)
+    local_repo.git_cmd(["switch", local_repo.package])
+    local_repo.git_cmd(["branch", "-D", local_repo.feat_branch])
 
 
 @click.command("pull")
 def pull() -> None:
     """Pull last recent changes of package you are on from Alpa repo"""
     local_repo = LocalRepoBranch(Path(getcwd()))
     local_repo.pull(local_repo.branch)
```

### Comparing `pyalpa-0.6.0/alpa/config/alpa_local.py` & `pyalpa-0.7.0/alpa/config/alpa_local.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.6.0/alpa/config/alpa_repo.py` & `pyalpa-0.7.0/alpa/config/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.6.0/alpa/config/base.py` & `pyalpa-0.7.0/alpa/config/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.6.0/alpa/config/metadata.py` & `pyalpa-0.7.0/alpa/config/metadata.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.6.0/alpa/config/packit.py` & `pyalpa-0.7.0/alpa/config/packit.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.6.0/alpa/constants.py` & `pyalpa-0.7.0/alpa/constants.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.6.0/alpa/gh.py` & `pyalpa-0.7.0/alpa/gh.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.6.0/alpa/messages.py` & `pyalpa-0.7.0/alpa/messages.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.6.0/alpa/repository/base.py` & `pyalpa-0.7.0/alpa/repository/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,53 @@
 """
 Set of commands that helps with integration of Alpa
 repository.
 """
 import subprocess
 from abc import ABC, abstractmethod
-from os import getcwd, environ
+from os import getcwd
 from pathlib import Path
-from subprocess import call
-from tempfile import NamedTemporaryFile
 from typing import Optional, Iterable
 from urllib.parse import urlparse
 
 from click import UsageError, ClickException
 import click
-from git import Repo, Remote
 
 from alpa.constants import (
     ALPA_FEAT_BRANCH,
     ALPA_FEAT_BRANCH_PREFIX,
     ORIGIN_NAME,
     UPSTREAM_NAME,
 )
 from alpa.gh import GithubAPI, GithubRepo
+from alpa.git import GitCMD
 from alpa.messages import (
     CLONED_REPO_IS_NOT_FORK,
     NOT_IN_PREDEFINED_STATE,
     CLONED_REPO_IS_FORK,
     NO_PERMISSION_FOR_ALPA_REPO,
 )
 
 
 class LocalRepo(ABC):
     def __init__(self, repo_path: Path) -> None:
         self.repo_path = repo_path
-        # TODO: this will differ in the future with repo_path
-        self.repo_root_path = repo_path
-        self.local_repo = Repo(str(self.repo_path), search_parent_directories=True)
-        self.git_cmd = self.local_repo.git
+        self.git = GitCMD(str(self.repo_path))
+        self.git_cmd = self.git.git_cmd
 
         if not self._is_repo_in_predefined_state():
             raise ClickException(NOT_IN_PREDEFINED_STATE)
 
         # do it after predefined state is checked since this depends on it
         # (see comment in the _should_be_fork)
         self.remote_name = UPSTREAM_NAME if self._should_be_fork() else ORIGIN_NAME
 
         # lazy properties
         self._namespace: Optional[str] = None
         self._repo_name: Optional[str] = None
-        self._git_root: Optional[Path] = None
 
     @abstractmethod
     def get_packages(self, regex: str) -> list[str]:
         pass
 
     @abstractmethod
     def switch_to_package(self, package: str) -> None:
@@ -72,20 +67,16 @@
         pass
 
     @abstractmethod
     def create_packit_config(self, override: bool) -> bool:
         pass
 
     @property
-    def remote_associated_with_current_branch(self) -> str:
-        return self.local_repo.active_branch.tracking_branch().remote_name
-
-    @property
     def branch(self) -> str:
-        return self.local_repo.active_branch.name
+        return self.git_cmd(["rev-parse", "--abbrev-ref", "HEAD"]).stdout
 
     @staticmethod
     def get_feat_branch_of_package(package: str) -> str:
         return ALPA_FEAT_BRANCH.format(pkgname=package)
 
     @property
     def feat_branch(self) -> str:
@@ -100,15 +91,17 @@
                 relevant_refs.append(parsed_ref)
 
         return relevant_refs
 
     def get_remote_branches(self, remote: str) -> list[str]:
         lines = [
             line.strip()
-            for line in self.git_cmd.remote("--verbose", "show", remote).split("\n")
+            for line in self.git_cmd(
+                ["remote", "--verbose", "show", remote]
+            ).stdout.split("\n")
         ]
         # TODO: do a better job
         remote_branch_line = ["Remote branch:", "Remote branches:"]
         start = -1
         for line_to_match in remote_branch_line:
             if line_to_match in lines:
                 start = lines.index(line_to_match)
@@ -132,33 +125,42 @@
 
         if end == -1:
             end = len(lines)
 
         lines_with_remote_branches = lines[start + 1 : end]
         return [line.split()[0] for line in lines_with_remote_branches]
 
+    @property
+    def remotes(self) -> set[str]:
+        return set(self.git_cmd(["remote"]).stdout.split())
+
     def _is_repo_in_predefined_state(self) -> bool:
-        remotes_name_set = {remote.name for remote in self.local_repo.remotes}
-        return remotes_name_set == {ORIGIN_NAME, UPSTREAM_NAME} or remotes_name_set == {
+        return self.remotes == {ORIGIN_NAME, UPSTREAM_NAME} or self.remotes == {
             ORIGIN_NAME
         }
 
     def _should_be_fork(self) -> bool:
-        remotes_name_set = {remote.name for remote in self.local_repo.remotes}
         # if repo is prepared via alpa-cli, fork should have 2 remotes and non-fork 1
-        return len(remotes_name_set) > 1
+        return len(self.remotes) > 1
 
     @property
     def untracked_files(self) -> list[str]:
-        return self.local_repo.untracked_files
+        return self.git_cmd(["ls-files", "-o", "--exclude-standard"]).stdout.split()
 
     def _get_dirty_files(self, staged: bool) -> list[str]:
         result = []
-        status_output = self.git_cmd.status("--porcelain=1").split("\n")
-        for line in status_output:
+        status_output = self.git_cmd(["status", "--porcelain=1"]).stdout
+        if not status_output:
+            return []
+
+        for line in status_output.split("\n"):
+            if line == "":
+                # some empty line in the output
+                continue
+
             file = line.split()[-1]
             if line.startswith("MM"):
                 result.append(file)
                 continue
 
             if not staged and line.startswith(" M"):
                 result.append(file)
@@ -166,14 +168,17 @@
 
             if staged and line.startswith("M "):
                 result.append(file)
                 continue
 
         return result
 
+    def is_dirty(self) -> bool:
+        return self.git_cmd(["status", "--porcelain"]).stdout != ""
+
     @property
     def modified_files(self) -> list[str]:
         return self._get_dirty_files(False)
 
     @property
     def files_to_be_committed(self) -> list[str]:
         return self._get_dirty_files(True)
@@ -208,75 +213,61 @@
             self.files_to_be_committed, "Files to commit:"
         )
         output += self._format_files_to_status(self.modified_files, "Modified files:")
         output += self._format_files_to_status(self.untracked_files, "Untracked files:")
         return output
 
     def branch_exists(self, branch: str) -> bool:
-        for ref in self.local_repo.references:
-            if ref.name == branch:
+        for ref in self.git_cmd(["branch"]).stdout.split():
+            if ref.strip() == branch:
                 return True
 
         return False
 
-    def get_history_of_branch(self, branch: str, *params: list[str]) -> str:
-        return self.git_cmd.log("--decorate", "--graph", *params, branch)
-
-    @staticmethod
-    def _get_message_from_editor() -> str:
-        with NamedTemporaryFile(suffix=".alpa.tmp") as temp_file:
-            call([environ.get("EDITOR", "vim"), temp_file.name])
-            temp_file.seek(0)
-            output = temp_file.read()
-            if isinstance(output, (bytes, bytearray)):
-                return output.decode("utf-8")
-
-            return output
+    def get_history_of_branch(self, branch: str, params: list[str]) -> str:
+        return self.git_cmd(["log", "--decorate", "--graph"] + params + [branch]).stdout
 
     def commit(self, message: str, pre_commit: bool) -> bool:
         if pre_commit:
             ret = subprocess.run(["pre-commit", "run", "--all-files"])
             if ret.returncode != 0:
                 return False
 
         self._ensure_feature_branch()
-        index = self.local_repo.index
         if message:
-            index.commit(message)
+            self.git_cmd(["commit", "-m", message])
         else:
-            index.commit(self._get_message_from_editor())
+            self.git_cmd(["commit"])
 
         return True
 
-    def add(self, files: list[str]) -> None:
+    def add(self, to_add: str) -> None:
         self._ensure_feature_branch()
-        # FIXME: alpa add . acts weird
-        self.git_cmd.add(files)
+        self.git_cmd(["add", to_add])
 
     def pull(self, branch: str) -> None:
-        click.echo(self.git_cmd.pull(self.remote_name, branch))
+        click.echo(self.git_cmd(["pull", self.remote_name, branch]).stdout)
 
     def push(self, branch: str) -> None:
         # you always want to push to origin, even from a fork
-        click.echo(self.git_cmd.push(ORIGIN_NAME, branch))
+        click.echo(self.git_cmd(["push", ORIGIN_NAME, branch]).stdout)
 
     def full_reponame(self) -> str:
-        for remote in self.local_repo.remotes:
-            if remote.name == self.remote_name:
-                return remote.url.split(":")[-1].removesuffix(".git")
+        for remote in self.remotes:
+            if remote == self.remote_name:
+                remote_url = self.git_cmd(
+                    ["config", "--get", f"remote.{remote}.url"]
+                ).stdout
+                return remote_url.split(":")[-1].removesuffix(".git")
 
         return ""
 
     @property
-    def git_root(self) -> Optional[Path]:
-        if self._git_root is not None:
-            return self._git_root
-
-        self._git_root = Path(self.local_repo.working_tree_dir)
-        return self._git_root
+    def git_root(self) -> Path:
+        return Path(self.git.git_root)
 
 
 class AlpaRepo(LocalRepo):
     def __init__(self, repo_path: Path, gh_api: Optional[GithubAPI] = None) -> None:
         super().__init__(repo_path)
 
         self.gh_api = gh_api or GithubAPI(self.repo_name)
@@ -291,19 +282,24 @@
         pass
 
     @abstractmethod
     def request_package_delete(self, package: str) -> None:
         pass
 
     @staticmethod
-    def _prepare_cloned_repo(local_repo: Repo, gh_repo: GithubRepo) -> None:
+    def _prepare_cloned_repo(where_to_clone: str, gh_repo: GithubRepo) -> None:
         if not gh_repo.is_fork:
             return
 
-        Remote.create(local_repo, UPSTREAM_NAME, gh_repo.upstream_clone_url)
+        upstream_clone_url = gh_repo.upstream_clone_url
+        assert upstream_clone_url is not None
+        subprocess.run(
+            ["git", "remote", "add", UPSTREAM_NAME, upstream_clone_url],
+            cwd=where_to_clone,
+        )
 
     @staticmethod
     def _get_repo_name_from_url(repo_url: str) -> str:
         return repo_url.split("/")[-1].removesuffix(".git")
 
     @staticmethod
     def _check_for_permission_and_fork(
@@ -329,11 +325,11 @@
         api = GithubAPI(repo_name)
         gh_repo = api.get_repo(namespace, repo_name)
 
         check_result, stderr = cls._check_for_permission_and_fork(clone_fork, gh_repo)
         if not check_result:
             raise UsageError(stderr)
 
-        cloned_repo = Repo.clone_from(
-            url, f"{getcwd()}/{cls._get_repo_name_from_url(url)}"
-        )
-        cls._prepare_cloned_repo(cloned_repo, gh_repo)
+        cwd = getcwd()
+        where_to_clone = f"{cwd}/{cls._get_repo_name_from_url(url)}"
+        subprocess.run(["git", "clone", url, where_to_clone], cwd=cwd)
+        cls._prepare_cloned_repo(where_to_clone, gh_repo)
```

### Comparing `pyalpa-0.6.0/alpa/repository/branch.py` & `pyalpa-0.7.0/alpa/repository/branch.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from pathlib import Path
 import re
 from typing import Optional, Type
 
 from click import ClickException
 import click
-from git import GitCommandError
 
 from alpa.config import PackitConfig
 from alpa.constants import (
     ALPA_FEAT_BRANCH_PREFIX,
     MAIN_BRANCH,
     PackageRequest,
     DeleteRequest,
@@ -32,54 +31,55 @@
     def package(self) -> str:
         return self.branch.removeprefix(ALPA_FEAT_BRANCH_PREFIX)
 
     def get_history_of_package(self, package: str) -> str:
         raise NotImplementedError("Please implement me!")
 
     def get_packages(self, regex: str) -> list[str]:
-        # self.local_repo.remote(name=self.remote_name).refs don't work on every case
         refs_without_main = filter(
             lambda ref: ref != "main", self.get_remote_branches(self.remote_name)
         )
         relevant_refs = self._get_relevant_remote_refs(refs_without_main)
 
         if regex == "":
             return list(relevant_refs)
 
         pattern = re.compile(regex)
         return [ref for ref in relevant_refs if pattern.match(ref)]
 
     def switch_to_package(self, package: str) -> None:
-        if self.local_repo.is_dirty():
+        if self.is_dirty():
             click.echo(
                 "Repo is dirty, please commit your changes before switching to"
                 f" another package.\n {self.get_status_output()}"
             )
             return None
 
         feat_branch = self.get_feat_branch_of_package(package)
         branch_to_switch = feat_branch if self.branch_exists(feat_branch) else package
-        try:
+        result = self.git_cmd(["switch", branch_to_switch])
+        if result.retval == 0:
+            click.echo(result.stdout.replace("branch", "package"))
+        else:
+            click.echo(f"Switching to the package {package} for the first time")
             click.echo(
-                self.git_cmd.switch(branch_to_switch).replace("branch", "package")
+                self.git_cmd(["fetch", self.remote_name, branch_to_switch]).stdout
             )
-        except GitCommandError:
-            # switching to the package for the first time
-            click.echo(f"Switching to the package {package} for the first time")
-            click.echo(self.git_cmd.fetch(self.remote_name, branch_to_switch))
             click.echo(
-                self.git_cmd.switch(branch_to_switch).replace("branch", "package")
+                self.git_cmd(["switch", branch_to_switch]).stdout.replace(
+                    "branch", "package"
+                )
             )
 
     def _ensure_feature_branch(self) -> None:
         if self.branch != self.package:
             return None
 
         click.echo("Switching to feature branch")
-        self.git_cmd.switch("-c", self.feat_branch)
+        self.git_cmd(["switch", "-c", self.feat_branch])
 
     def create_packit_config(self, override: bool) -> bool:
         packit_conf = PackitConfig(self.package)
         if packit_conf.packit_config_file_exists() and not override:
             return False
 
         packit_conf.create_packit_config()
@@ -94,17 +94,17 @@
         self.gh_repo = self.gh_api.get_repo(self.namespace, self.repo_name)
 
     def create_package(self, package: str) -> None:
         upstream = self.gh_repo.get_upstream()
         if upstream and not upstream.has_write_access(self.gh_api.gh_user):
             raise ClickException(NO_WRITE_ACCESS_ERR)
 
-        self.git_cmd.switch(MAIN_BRANCH)
-        self.git_cmd.switch("-c", package)
-        self.git_cmd.push(self.remote_name, package)
+        self.git_cmd(["switch", MAIN_BRANCH])
+        self.git_cmd(["switch", "-c", package])
+        self.git_cmd(["push", self.remote_name, package])
         click.echo(f"Package {package} created")
 
     def _request_package_action(
         self, action: Type[PackageRequest | DeleteRequest], pkg: str
     ) -> None:
         ensured_upstream = self.gh_repo.get_root_repo()
         upstream_namespace = ensured_upstream.namespace
```

### Comparing `pyalpa-0.6.0/alpa/repository/subdirectory.py` & `pyalpa-0.7.0/alpa/repository/subdirectory.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.6.0/alpa/upstream_integration.py` & `pyalpa-0.7.0/alpa/upstream_integration.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.6.0/pyproject.toml` & `pyalpa-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [tool.poetry]
 name = "pyalpa"
-version = "0.6.0"
+version = "0.7.0"
 description = "Integration tool with Alpa repository"
 authors = ["Jiri Kyjovsky <j1.kyjovsky@gmail.com>"]
 maintainers = ["Jiří Kyjovský <j1.kyjovsky@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/alpa-team/alpa"
 repository = "https://github.com/alpa-team/alpa"
 exclude = ["test/"]
 packages = [{ include = "alpa" }]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = ">=8.0.0"
-gitpython = ">=3.0"
 pygithub = ">=1.4"
 pyyaml = ">=5.0"
 specfile = ">=0.13.0"
 pydantic = ">=1.8"
 email-validator = ">=1.0"
```

### Comparing `pyalpa-0.6.0/PKG-INFO` & `pyalpa-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalpa
-Version: 0.6.0
+Version: 0.7.0
 Summary: Integration tool with Alpa repository
 Home-page: https://github.com/alpa-team/alpa
 License: GPLv3
 Author: Jiri Kyjovsky
 Author-email: j1.kyjovsky@gmail.com
 Maintainer: Jiří Kyjovský
 Maintainer-email: j1.kyjovsky@gmail.com
@@ -12,15 +12,14 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.0)
 Requires-Dist: email-validator (>=1.0)
-Requires-Dist: gitpython (>=3.0)
 Requires-Dist: pydantic (>=1.8)
 Requires-Dist: pygithub (>=1.4)
 Requires-Dist: pyyaml (>=5.0)
 Requires-Dist: specfile (>=0.13.0)
 Project-URL: Repository, https://github.com/alpa-team/alpa
 Description-Content-Type: text/markdown
```

