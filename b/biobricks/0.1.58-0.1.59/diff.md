# Comparing `tmp/biobricks-0.1.58.tar.gz` & `tmp/biobricks-0.1.59.tar.gz`

## Comparing `biobricks-0.1.58.tar` & `biobricks-0.1.59.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks.svg
--rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 biobricks-0.1.58/coverage.xml
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 biobricks-0.1.58/requirements.txt
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 biobricks-0.1.58/.github/workflows/biobricks.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.58/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.58/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.58/.pytest_cache/README.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.58/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 biobricks-0.1.58/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.58/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 biobricks-0.1.58/.vscode/tasks.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/api.py
--rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/brick.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/checks.py
--rwxr-xr-x   0        0        0     4049 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/cli.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/config.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/local_bb.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/.pytest_cache/README.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/test_init.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 biobricks-0.1.58/docker/Dockerfile
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.58/docker/test.sh
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 biobricks-0.1.58/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.1.58/LICENSE
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 biobricks-0.1.58/README.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 biobricks-0.1.58/pyproject.toml
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 biobricks-0.1.58/PKG-INFO
+-rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks.svg
+-rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 biobricks-0.1.59/coverage.xml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 biobricks-0.1.59/requirements.txt
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 biobricks-0.1.59/.github/workflows/biobricks.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.59/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.59/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.59/.pytest_cache/README.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.59/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 biobricks-0.1.59/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.59/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 biobricks-0.1.59/.vscode/tasks.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/api.py
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/brick.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/checks.py
+-rwxr-xr-x   0        0        0     3986 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/cli.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/config.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/local_bb.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/.pytest_cache/README.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/test_init.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.59/biobricks/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 biobricks-0.1.59/docker/Dockerfile
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.59/docker/test.sh
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 biobricks-0.1.59/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.1.59/LICENSE
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 biobricks-0.1.59/README.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 biobricks-0.1.59/pyproject.toml
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 biobricks-0.1.59/PKG-INFO
```

### Comparing `biobricks-0.1.58/biobricks.svg` & `biobricks-0.1.59/biobricks.svg`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.58/coverage.xml` & `biobricks-0.1.59/coverage.xml`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.58/.github/workflows/biobricks.yml` & `biobricks-0.1.59/.github/workflows/biobricks.yml`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.58/biobricks/api.py` & `biobricks-0.1.59/biobricks/api.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.58/biobricks/brick.py` & `biobricks-0.1.59/biobricks/brick.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,15 @@
 
     @staticmethod
     def Resolve(ref:str, force_remote=False):
         """find all bricks matching ref. `ref` can be:
             - existing  name ie. 'tox21'
             - git-url syntax ie. 'https://github.com/biobricks-ai/tox21#commit'
         if `force_remote` is True then retrieve brick from remote repository"""
-        # TODO this should resolve from the .bb directory when in a biobrick repo
-
+        
         # if name matches remote#commit then resolve from url        
         if re.match("^http.*[0-9a-f]{40}$",ref):
             return Brick.FromURL(ref)
         
         # if name matches remote then resolve from remote
         if re.match("^http.*$",ref):
             return Brick.FromRemote(ref)
@@ -107,21 +106,22 @@
     def _relpath(self):
         "get the path to this brick relative to bblib"
         return self.urlpath() / self.commit
 
     def install(self):
         "install this brick"
         logger.info(f"running checks on brick")
-        check_url_available(self.remote)
-        check_token(token())
-        check_symlink_permission()
-
+        
         if bblib(self.commit).exists():
             logger.info(f"\033[91m{self.url}\033[0m already exists in BioBricks library.")
             return True
+        
+        check_url_available(self.remote)
+        check_token(token())
+        check_symlink_permission()
 
         cmd = functools.partial(run,shell=True,stdout=DEVNULL,stderr=DEVNULL)
         
         # old way - cmd(f"git submodule add {self.remote} {self.repo}",cwd=bblib())
         logger.info(f"git clone {self.remote} {self._relpath()} in {bblib()}")
         cmd(f"git clone {self.remote} {self._relpath()}", cwd = bblib())
         cmd(f"git checkout {self.commit}", cwd = self.path())
```

### Comparing `biobricks-0.1.58/biobricks/checks.py` & `biobricks-0.1.59/biobricks/checks.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.58/biobricks/cli.py` & `biobricks-0.1.59/biobricks/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,18 +92,17 @@
     check_has_local_bblib()
     localbb = LocalBB.FromPath(os.getcwd())
     localbb.add_dependency(ref)
     
 @cli.command(name="pull", help="install local dependencies", section=Sect.BRICK)
 def pull():
     check_has_local_bblib()
-    with open(local_bblib() / "dependencies.txt", "r") as f:
-        for line in f.readlines():
-            Brick.FromURL(line).install()
-
+    lbb = LocalBB.FromPath(os.getcwd())
+    lbb.install_dependencies()
+    
 @cli.command(help="Show the status of the local brick",
     section=Sect.BRICK)
 def status():
     print("BBLIB: " + str(bb.bblib()))
     # print the dependencies file
     with open(local_bblib() / "dependencies.txt", "r") as f:
         print(f.read())
```

### Comparing `biobricks-0.1.58/biobricks/config.py` & `biobricks-0.1.59/biobricks/config.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.58/biobricks/tests/test_init.py` & `biobricks-0.1.59/biobricks/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.58/docker/Dockerfile` & `biobricks-0.1.59/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.58/LICENSE` & `biobricks-0.1.59/LICENSE`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.58/README.md` & `biobricks-0.1.59/README.md`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.58/pyproject.toml` & `biobricks-0.1.59/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "biobricks"
-version = "0.1.58"
+version = "0.1.59"
 authors = [
   { name="Jose A. Jaramillo", email="jjv@utp.edu.co" },
   { name="Thomas Luechtefeld", email="tom@insilica.co" }
 ]
 description = "Biobricks automates bioinformatics data."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `biobricks-0.1.58/PKG-INFO` & `biobricks-0.1.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobricks
-Version: 0.1.58
+Version: 0.1.59
 Summary: Biobricks automates bioinformatics data.
 Project-URL: Homepage, https://github.com/biobricks-ai/biobricks
 Project-URL: Bug Tracker, https://github.com/biobricks-ai/biobricks/issues
 Author-email: "Jose A. Jaramillo" <jjv@utp.edu.co>, Thomas Luechtefeld <tom@insilica.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

