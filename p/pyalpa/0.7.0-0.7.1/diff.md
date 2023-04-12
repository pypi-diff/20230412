# Comparing `tmp/pyalpa-0.7.0.tar.gz` & `tmp/pyalpa-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalpa-0.7.0.tar", max compression
+gzip compressed data, was "pyalpa-0.7.1.tar", max compression
```

## Comparing `pyalpa-0.7.0.tar` & `pyalpa-0.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2023-04-12 16:44:15.732104 pyalpa-0.7.0/LICENSE
--rw-r--r--   0        0        0     1631 2023-04-12 16:44:15.732104 pyalpa-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/cli/__init__.py
--rw-r--r--   0        0        0      732 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/cli/alpa_repo.py
--rw-r--r--   0        0        0     1249 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/cli/base.py
--rw-r--r--   0        0        0     6410 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/cli/local_repo.py
--rw-r--r--   0        0        0      227 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/config/__init__.py
--rw-r--r--   0        0        0     1079 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/config/alpa_local.py
--rw-r--r--   0        0        0     2184 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/config/alpa_repo.py
--rw-r--r--   0        0        0     1157 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/config/base.py
--rw-r--r--   0        0        0     2759 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/config/metadata.py
--rw-r--r--   0        0        0     2790 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/config/packit.py
--rw-r--r--   0        0        0     1233 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/constants.py
--rw-r--r--   0        0        0      158 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/exceptions.py
--rw-r--r--   0        0        0     3900 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/gh.py
--rw-r--r--   0        0        0     1804 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/git.py
--rw-r--r--   0        0        0     1447 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/messages.py
--rw-r--r--   0        0        0        0 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/repository/__init__.py
--rw-r--r--   0        0        0    10335 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/repository/base.py
--rw-r--r--   0        0        0     4331 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/repository/branch.py
--rw-r--r--   0        0        0     1661 2023-04-12 16:44:15.732104 pyalpa-0.7.0/alpa/repository/subdirectory.py
--rw-r--r--   0        0        0     3879 2023-04-12 16:44:15.736104 pyalpa-0.7.0/alpa/upstream_integration.py
--rw-r--r--   0        0        0      846 2023-04-12 16:44:15.736104 pyalpa-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 pyalpa-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 17:44:18.651486 pyalpa-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1631 2023-04-12 17:44:18.651486 pyalpa-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 17:44:18.651486 pyalpa-0.7.1/alpa/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 17:44:18.651486 pyalpa-0.7.1/alpa/cli/__init__.py
+-rw-r--r--   0        0        0      732 2023-04-12 17:44:18.651486 pyalpa-0.7.1/alpa/cli/alpa_repo.py
+-rw-r--r--   0        0        0     1249 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/cli/base.py
+-rw-r--r--   0        0        0     6408 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/cli/local_repo.py
+-rw-r--r--   0        0        0      227 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/config/__init__.py
+-rw-r--r--   0        0        0     1264 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/config/alpa_local.py
+-rw-r--r--   0        0        0     2184 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/config/alpa_repo.py
+-rw-r--r--   0        0        0     1157 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/config/base.py
+-rw-r--r--   0        0        0     2759 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/config/metadata.py
+-rw-r--r--   0        0        0     2790 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/config/packit.py
+-rw-r--r--   0        0        0     1233 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/constants.py
+-rw-r--r--   0        0        0      158 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/exceptions.py
+-rw-r--r--   0        0        0     4021 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/gh.py
+-rw-r--r--   0        0        0     2092 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/git.py
+-rw-r--r--   0        0        0     1447 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/messages.py
+-rw-r--r--   0        0        0        0 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/repository/__init__.py
+-rw-r--r--   0        0        0    11039 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/repository/base.py
+-rw-r--r--   0        0        0     4331 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/repository/branch.py
+-rw-r--r--   0        0        0     1661 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/repository/subdirectory.py
+-rw-r--r--   0        0        0     3879 2023-04-12 17:44:18.655486 pyalpa-0.7.1/alpa/upstream_integration.py
+-rw-r--r--   0        0        0      846 2023-04-12 17:44:18.655486 pyalpa-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 pyalpa-0.7.1/PKG-INFO
```

### Comparing `pyalpa-0.7.0/LICENSE` & `pyalpa-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.0/README.md` & `pyalpa-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.0/alpa/cli/alpa_repo.py` & `pyalpa-0.7.1/alpa/cli/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.0/alpa/cli/base.py` & `pyalpa-0.7.1/alpa/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.0/alpa/cli/local_repo.py` & `pyalpa-0.7.1/alpa/cli/local_repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """
 These commands need to create LocalRepo -> no GH token required
 """
-
-
 from os import getcwd
 from pathlib import Path
 
 import click
 from click import ClickException, Choice
 from specfile import Specfile
```

### Comparing `pyalpa-0.7.0/alpa/config/alpa_local.py` & `pyalpa-0.7.1/alpa/config/alpa_local.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 """
 Class for local cli config
 """
-
-
+import logging
 from os.path import isfile
 from pathlib import Path
 from typing import Optional
 
 from yaml import safe_load
 
 from alpa.constants import CONFIG_FILE_LOCATIONS
 
 
+logger = logging.getLogger(__name__)
+
+
 class AlpaLocalConfig:
     def __init__(self, gh_api_token: str) -> None:
         self.gh_api_token = gh_api_token
 
     @staticmethod
     def _get_config_file_path() -> Optional[Path]:
         for location in CONFIG_FILE_LOCATIONS:
             expanded_path = Path(location).expanduser()
             if isfile(str(expanded_path)):
+                logger.info(f"Config file found in {str(expanded_path)}")
                 return expanded_path
 
+        logger.info("No config file found for local alpa")
         return None
 
     @classmethod
     def get_config(cls, repo_name: str) -> Optional["AlpaLocalConfig"]:
         cfg_file_path = cls._get_config_file_path()
         if cfg_file_path is None:
             return None
```

### Comparing `pyalpa-0.7.0/alpa/config/alpa_repo.py` & `pyalpa-0.7.1/alpa/config/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.0/alpa/config/base.py` & `pyalpa-0.7.1/alpa/config/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.0/alpa/config/metadata.py` & `pyalpa-0.7.1/alpa/config/metadata.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.0/alpa/config/packit.py` & `pyalpa-0.7.1/alpa/config/packit.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.0/alpa/constants.py` & `pyalpa-0.7.1/alpa/constants.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.0/alpa/gh.py` & `pyalpa-0.7.1/alpa/gh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Wrapper aroung pygithub API since the documentation is awful..
 """
-
-
+import logging
 from os import getenv
 from typing import Optional
 
 import click
 from click import UsageError
 from github import Github, Issue, PullRequest, UnknownObjectException
 
 from alpa.config.alpa_local import AlpaLocalConfig
 from alpa.constants import GH_API_TOKEN_NAME, GH_WRITE_ACCESS
 from alpa.messages import NO_GH_API_KEY_FOUND, RETURNING_CLONE_URL_MSG
 
 
+logger = logging.getLogger(__name__)
+
+
 class GithubRepo:
     def __init__(self, api: Github, namespace: str, repo_name: str) -> None:
         self.namespace = namespace
         self.repo_name = repo_name
 
         self._api = api
         self._repo = api.get_repo(f"{namespace}/{repo_name}")
@@ -119,8 +121,9 @@
         access_token_config = AlpaLocalConfig.get_config(repo_name)
         if access_token_config is None:
             raise UsageError(NO_GH_API_KEY_FOUND.format(token=GH_API_TOKEN_NAME))
 
         return access_token_config.gh_api_token
 
     def get_repo(self, namespace: str, repo_name: str) -> GithubRepo:
+        logger.info(f"Trying to find repo: {namespace}/{repo_name}")
         return GithubRepo(self._gh_api, namespace, repo_name)
```

### Comparing `pyalpa-0.7.0/alpa/git.py` & `pyalpa-0.7.1/alpa/git.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """
 Wrapper around git cmd using subprocess
 """
 import asyncio
+import logging
 import subprocess
 from dataclasses import dataclass
 from typing import Optional
 
 
+logger = logging.getLogger(__name__)
+
+
 @dataclass
 class GitCmdResult:
     stdout: str
     stderr: str
     retval: int
 
 
@@ -27,14 +31,17 @@
         self, arguments: list[str], cwd: Optional[str] = None
     ) -> "GitCmdResult":
         if cwd is None:
             context = self.git_root
         else:
             context = cwd
 
+        logger.debug(
+            f"Running git cmd: $ git {' '.join(arguments)}; in context {context}"
+        )
         process = subprocess.run(
             ["git"] + arguments,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
             cwd=context,
         )
         return GitCmdResult(
@@ -47,14 +54,17 @@
         self, arguments: list[str], cwd: Optional[str] = None
     ) -> "GitCmdResult":
         if cwd is None:
             context = self.git_root
         else:
             context = cwd
 
+        logger.debug(
+            f"Running async git cmd: $ git {' '.join(arguments)}; in context {context}"
+        )
         async_subprocess = await asyncio.create_subprocess_exec(
             "git",
             *arguments,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
             cwd=context,
         )
```

### Comparing `pyalpa-0.7.0/alpa/messages.py` & `pyalpa-0.7.1/alpa/messages.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.0/alpa/repository/base.py` & `pyalpa-0.7.1/alpa/repository/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Set of commands that helps with integration of Alpa
 repository.
 """
+import logging
 import subprocess
 from abc import ABC, abstractmethod
 from os import getcwd
 from pathlib import Path
 from typing import Optional, Iterable
 from urllib.parse import urlparse
 
@@ -24,26 +25,30 @@
     CLONED_REPO_IS_NOT_FORK,
     NOT_IN_PREDEFINED_STATE,
     CLONED_REPO_IS_FORK,
     NO_PERMISSION_FOR_ALPA_REPO,
 )
 
 
+logger = logging.getLogger(__name__)
+
+
 class LocalRepo(ABC):
     def __init__(self, repo_path: Path) -> None:
         self.repo_path = repo_path
         self.git = GitCMD(str(self.repo_path))
         self.git_cmd = self.git.git_cmd
 
         if not self._is_repo_in_predefined_state():
             raise ClickException(NOT_IN_PREDEFINED_STATE)
 
         # do it after predefined state is checked since this depends on it
         # (see comment in the _should_be_fork)
         self.remote_name = UPSTREAM_NAME if self._should_be_fork() else ORIGIN_NAME
+        logger.debug(f"Remote name for this repository is set to {self.remote_name}")
 
         # lazy properties
         self._namespace: Optional[str] = None
         self._repo_name: Optional[str] = None
 
     @abstractmethod
     def get_packages(self, regex: str) -> list[str]:
@@ -84,14 +89,15 @@
 
     @staticmethod
     def _get_relevant_remote_refs(remote_refs: Iterable[str]) -> list[str]:
         relevant_refs = []
         for ref in remote_refs:
             parsed_ref = ref.split("/")[-1]
             if not parsed_ref.startswith(ALPA_FEAT_BRANCH_PREFIX):
+                logger.debug(f"Relevant remote ref found: {parsed_ref}")
                 relevant_refs.append(parsed_ref)
 
         return relevant_refs
 
     def get_remote_branches(self, remote: str) -> list[str]:
         lines = [
             line.strip()
@@ -185,22 +191,24 @@
 
     @property
     def namespace(self) -> str:
         if self._namespace is not None:
             return self._namespace
 
         self._namespace = self.full_reponame().split("/")[0]
+        logger.debug(f"Setting namespace to {self._namespace}")
         return self._namespace
 
     @property
     def repo_name(self) -> str:
         if self._repo_name is not None:
             return self._repo_name
 
         self._repo_name = self.full_reponame().split("/")[1]
+        logger.debug(f"Setting repo name to {self._repo_name}")
         return self._repo_name
 
     @staticmethod
     def _format_files_to_status(files: list[str], msg: str) -> str:
         if not files:
             return ""
 
@@ -213,18 +221,20 @@
             self.files_to_be_committed, "Files to commit:"
         )
         output += self._format_files_to_status(self.modified_files, "Modified files:")
         output += self._format_files_to_status(self.untracked_files, "Untracked files:")
         return output
 
     def branch_exists(self, branch: str) -> bool:
-        for ref in self.git_cmd(["branch"]).stdout.split():
+        branches = self.git_cmd(["branch"]).stdout.split()
+        for ref in branches:
             if ref.strip() == branch:
                 return True
 
+        logger.debug(f"Branch {branch} does not exist in {branches}")
         return False
 
     def get_history_of_branch(self, branch: str, params: list[str]) -> str:
         return self.git_cmd(["log", "--decorate", "--graph"] + params + [branch]).stdout
 
     def commit(self, message: str, pre_commit: bool) -> bool:
         if pre_commit:
@@ -248,21 +258,26 @@
         click.echo(self.git_cmd(["pull", self.remote_name, branch]).stdout)
 
     def push(self, branch: str) -> None:
         # you always want to push to origin, even from a fork
         click.echo(self.git_cmd(["push", ORIGIN_NAME, branch]).stdout)
 
     def full_reponame(self) -> str:
+        logger.debug(f"Trying to find {self.remote_name} in {self.remotes}")
         for remote in self.remotes:
             if remote == self.remote_name:
                 remote_url = self.git_cmd(
                     ["config", "--get", f"remote.{remote}.url"]
                 ).stdout
+                logger.debug(
+                    f"Remote {remote} found. Parsing its remote url {remote_url}"
+                )
                 return remote_url.split(":")[-1].removesuffix(".git")
 
+        logger.debug("There are no remotes in this repo")
         return ""
 
     @property
     def git_root(self) -> Path:
         return Path(self.git.git_root)
```

### Comparing `pyalpa-0.7.0/alpa/repository/branch.py` & `pyalpa-0.7.1/alpa/repository/branch.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.0/alpa/repository/subdirectory.py` & `pyalpa-0.7.1/alpa/repository/subdirectory.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.0/alpa/upstream_integration.py` & `pyalpa-0.7.1/alpa/upstream_integration.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.0/pyproject.toml` & `pyalpa-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyalpa"
-version = "0.7.0"
+version = "0.7.1"
 description = "Integration tool with Alpa repository"
 authors = ["Jiri Kyjovsky <j1.kyjovsky@gmail.com>"]
 maintainers = ["Jiří Kyjovský <j1.kyjovsky@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/alpa-team/alpa"
 repository = "https://github.com/alpa-team/alpa"
```

### Comparing `pyalpa-0.7.0/PKG-INFO` & `pyalpa-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalpa
-Version: 0.7.0
+Version: 0.7.1
 Summary: Integration tool with Alpa repository
 Home-page: https://github.com/alpa-team/alpa
 License: GPLv3
 Author: Jiri Kyjovsky
 Author-email: j1.kyjovsky@gmail.com
 Maintainer: Jiří Kyjovský
 Maintainer-email: j1.kyjovsky@gmail.com
```

