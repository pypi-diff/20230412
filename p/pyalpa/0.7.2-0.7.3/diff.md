# Comparing `tmp/pyalpa-0.7.2.tar.gz` & `tmp/pyalpa-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalpa-0.7.2.tar", max compression
+gzip compressed data, was "pyalpa-0.7.3.tar", max compression
```

## Comparing `pyalpa-0.7.2.tar` & `pyalpa-0.7.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2023-04-12 18:03:51.773228 pyalpa-0.7.2/LICENSE
--rw-r--r--   0        0        0     1631 2023-04-12 18:03:51.773228 pyalpa-0.7.2/README.md
--rw-r--r--   0        0        0        0 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/cli/__init__.py
--rw-r--r--   0        0        0      732 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/cli/alpa_repo.py
--rw-r--r--   0        0        0     1249 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/cli/base.py
--rw-r--r--   0        0        0     6408 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/cli/local_repo.py
--rw-r--r--   0        0        0      227 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/config/__init__.py
--rw-r--r--   0        0        0     1264 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/config/alpa_local.py
--rw-r--r--   0        0        0     2184 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/config/alpa_repo.py
--rw-r--r--   0        0        0     1157 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/config/base.py
--rw-r--r--   0        0        0     2759 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/config/metadata.py
--rw-r--r--   0        0        0     2790 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/config/packit.py
--rw-r--r--   0        0        0     1233 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/constants.py
--rw-r--r--   0        0        0      158 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/exceptions.py
--rw-r--r--   0        0        0     4021 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/gh.py
--rw-r--r--   0        0        0     2092 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/git.py
--rw-r--r--   0        0        0     1447 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/messages.py
--rw-r--r--   0        0        0        0 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/repository/__init__.py
--rw-r--r--   0        0        0    11490 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/repository/base.py
--rw-r--r--   0        0        0     4331 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/repository/branch.py
--rw-r--r--   0        0        0     1661 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/repository/subdirectory.py
--rw-r--r--   0        0        0     3879 2023-04-12 18:03:51.773228 pyalpa-0.7.2/alpa/upstream_integration.py
--rw-r--r--   0        0        0      846 2023-04-12 18:03:51.773228 pyalpa-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 pyalpa-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 18:21:09.052332 pyalpa-0.7.3/LICENSE
+-rw-r--r--   0        0        0     1631 2023-04-12 18:21:09.052332 pyalpa-0.7.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/cli/__init__.py
+-rw-r--r--   0        0        0      732 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/cli/alpa_repo.py
+-rw-r--r--   0        0        0     1249 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/cli/base.py
+-rw-r--r--   0        0        0     6408 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/cli/local_repo.py
+-rw-r--r--   0        0        0      227 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/config/__init__.py
+-rw-r--r--   0        0        0     1264 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/config/alpa_local.py
+-rw-r--r--   0        0        0     2184 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/config/alpa_repo.py
+-rw-r--r--   0        0        0     1157 2023-04-12 18:21:09.052332 pyalpa-0.7.3/alpa/config/base.py
+-rw-r--r--   0        0        0     2759 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/config/metadata.py
+-rw-r--r--   0        0        0     2790 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/config/packit.py
+-rw-r--r--   0        0        0     1233 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/constants.py
+-rw-r--r--   0        0        0      158 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/exceptions.py
+-rw-r--r--   0        0        0     4021 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/gh.py
+-rw-r--r--   0        0        0     2463 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/git.py
+-rw-r--r--   0        0        0     1447 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/messages.py
+-rw-r--r--   0        0        0        0 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/repository/__init__.py
+-rw-r--r--   0        0        0    11490 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/repository/base.py
+-rw-r--r--   0        0        0     4331 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/repository/branch.py
+-rw-r--r--   0        0        0     1661 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/repository/subdirectory.py
+-rw-r--r--   0        0        0     3879 2023-04-12 18:21:09.056331 pyalpa-0.7.3/alpa/upstream_integration.py
+-rw-r--r--   0        0        0      846 2023-04-12 18:21:09.056331 pyalpa-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 pyalpa-0.7.3/PKG-INFO
```

### Comparing `pyalpa-0.7.2/LICENSE` & `pyalpa-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/README.md` & `pyalpa-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/cli/alpa_repo.py` & `pyalpa-0.7.3/alpa/cli/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/cli/base.py` & `pyalpa-0.7.3/alpa/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/cli/local_repo.py` & `pyalpa-0.7.3/alpa/cli/local_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/config/alpa_local.py` & `pyalpa-0.7.3/alpa/config/alpa_local.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/config/alpa_repo.py` & `pyalpa-0.7.3/alpa/config/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/config/base.py` & `pyalpa-0.7.3/alpa/config/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/config/metadata.py` & `pyalpa-0.7.3/alpa/config/metadata.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/config/packit.py` & `pyalpa-0.7.3/alpa/config/packit.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/constants.py` & `pyalpa-0.7.3/alpa/constants.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/gh.py` & `pyalpa-0.7.3/alpa/gh.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/git.py` & `pyalpa-0.7.3/alpa/git.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,17 +40,23 @@
         )
         process = subprocess.run(
             ["git"] + arguments,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
             cwd=context,
         )
+        stdout = process.stdout.decode()
+        stderr = process.stderr.decode()
+        logger.debug(
+            f"git cmd results: stdout: {stdout}; stderr: {stderr}; "
+            f"retval: {process.returncode}"
+        )
         return GitCmdResult(
-            stdout=process.stdout.decode().strip(),
-            stderr=process.stderr.decode().strip(),
+            stdout=stdout.strip(),
+            stderr=stderr.strip(),
             retval=process.returncode,
         )
 
     async def async_git_cmd(
         self, arguments: list[str], cwd: Optional[str] = None
     ) -> "GitCmdResult":
         if cwd is None:
@@ -65,12 +71,16 @@
             "git",
             *arguments,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
             cwd=context,
         )
         stdout, stderr = await async_subprocess.communicate()
+        logger.debug(
+            f"async git cmd results: stdout: {stdout.decode()}; "
+            f"stderr: {stderr.decode()}; retval: {async_subprocess.returncode}"
+        )
         return GitCmdResult(
             stdout=stdout.decode().strip(),
             stderr=stderr.decode().strip(),
             retval=async_subprocess.returncode,  # type: ignore
         )
```

### Comparing `pyalpa-0.7.2/alpa/messages.py` & `pyalpa-0.7.3/alpa/messages.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/repository/base.py` & `pyalpa-0.7.3/alpa/repository/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/repository/branch.py` & `pyalpa-0.7.3/alpa/repository/branch.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/repository/subdirectory.py` & `pyalpa-0.7.3/alpa/repository/subdirectory.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/alpa/upstream_integration.py` & `pyalpa-0.7.3/alpa/upstream_integration.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.7.2/pyproject.toml` & `pyalpa-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyalpa"
-version = "0.7.2"
+version = "0.7.3"
 description = "Integration tool with Alpa repository"
 authors = ["Jiri Kyjovsky <j1.kyjovsky@gmail.com>"]
 maintainers = ["Jiří Kyjovský <j1.kyjovsky@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/alpa-team/alpa"
 repository = "https://github.com/alpa-team/alpa"
```

### Comparing `pyalpa-0.7.2/PKG-INFO` & `pyalpa-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalpa
-Version: 0.7.2
+Version: 0.7.3
 Summary: Integration tool with Alpa repository
 Home-page: https://github.com/alpa-team/alpa
 License: GPLv3
 Author: Jiri Kyjovsky
 Author-email: j1.kyjovsky@gmail.com
 Maintainer: Jiří Kyjovský
 Maintainer-email: j1.kyjovsky@gmail.com
```

