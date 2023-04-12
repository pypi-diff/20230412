# Comparing `tmp/django_concat_js-0.2.0.tar.gz` & `tmp/django_concat_js-0.2.1.tar.gz`

## Comparing `django_concat_js-0.2.0.tar` & `django_concat_js-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/.coverage
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/tox.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/__about__.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/__init__.py
--rw-r--r--   0        0        0    14048 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/dep_graph.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/settings.py
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/watch_src.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/management/commands/__init__.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/management/commands/watch_js.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/test_app/__init__.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/test_app/concat.json
--rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/test_app/manage.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/test_app/settings.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/test_app/settings_base.py
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/test_app/tests.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/test_app/urls.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/test_app/wsgi.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/test_app/static/src/s1.js
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/test_app/static/src/s2.js
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/test_app/static/src/s3.js
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/concat_js/test_app/static/src/s4.js
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/.gitignore
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/README.md
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 django_concat_js-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/tox.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/__about__.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/__init__.py
+-rw-r--r--   0        0        0    14068 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/dep_graph.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/settings.py
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/watch_src.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/management/commands/__init__.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/management/commands/watch_js.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/concat.json
+-rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/manage.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/settings.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/settings_base.py
+-rw-r--r--   0        0        0     9463 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/tests.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/urls.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/wsgi.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/static/src/s1.js
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/static/src/s2.js
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/static/src/s3.js
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/static/src/s4.js
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/README.md
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/PKG-INFO
```

### Comparing `django_concat_js-0.2.0/tox.ini` & `django_concat_js-0.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.0/concat_js/dep_graph.py` & `django_concat_js-0.2.1/concat_js/dep_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
                     self.printer("Dependancy {} was modified after {}".format(
                         path.relative_to(build.relative_to),
                         bundle.relative_to(build.relative_to)
                     ))
     
     def get_rebuilds(self, changed_file: Union[Path, str]) -> list:
         """
-        changed file is an absolute path in a string
+        changed file is an absolute path
         """
         key = Path(changed_file)
         targets = self._deps.get(key, [])
         return [self._builds[k] for k in targets]
     
     def _write_bundle(self, build : Brick, out: Path) -> None:
         with open(out, "w") as bundle:
@@ -248,15 +248,16 @@
             
     def file_changed(self, path: Path) -> None:
         if path in self.extra_files:
             self.printer("Main concatenation file changed.")
             self.reload()
         else:
             self.printer("{} changed, rebuild if needed".format(path.name))
-            if self.lint_js: # should be a command for linting
+            if self.lint_js and path in self._deps:
+                # don't lint aftre concat.
                 subprocess.run([self.lint_js, str(path)])
             self.bundle(path)
     
     def rebuild_all(self):
         # first pass, check dependancies between build files
         L = self.checker.get_order()
         for dest in L:
```

### Comparing `django_concat_js-0.2.0/concat_js/settings.py` & `django_concat_js-0.2.1/concat_js/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,23 +17,24 @@
     def set_defaults(self):
         # copy all settings
         for k, v in self.conf.items():
             if k == "conf" or k == "set_defaults":
                 raise ImproperlyConfigured("Invalid setting name CONCAT_JS['{}']".format(k))
             setattr(self, k, v)
         # check default values
-        self.CONCAT_ROOT = self.conf.get("CONCAT_ROOT") or settings.BASE_DIR
-        self.JSON_DEPS = self.conf.get("JSON_DEPS")
+        self.CONCAT_ROOT = Path(self.conf.get("CONCAT_ROOT")) or settings.BASE_DIR
+        self.JSON_DEPS = Path(self.conf.get("JSON_DEPS"))
         if self.JSON_DEPS is None:
             raise ImproperlyConfigured("No JSON_DEPS settings defined")
         self.LINT_COMMAND = self.conf.get("LINT_COMMAND", False)
         self.FILTER_EXTS = self.conf.get("FILTER_EXTS", (".js",))
         # copy BASE_DIR
         self.BASE_DIR = settings.BASE_DIR
         self.CREATE_SOURCEMAPS = self.conf.get("CREATE_SOURCEMAPS", False)
+        self.LINT_BASE = self.conf.get("LINT_BASE", False)
     
     def get(self, key, default=None):
         return self.conf.get(key, default)
 
 
 conf = Conf()
```

### Comparing `django_concat_js-0.2.0/concat_js/watch_src.py` & `django_concat_js-0.2.1/concat_js/watch_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     def __call__(self, change: watchfiles.Change, path: str) -> bool:
         path_obj = Path(path)
         if path_obj in self.extras:
             return True
         b = not path_obj.is_dir()
         if self.extensions:
             b = b and (path_obj.suffix in self.extensions)
-        print(b, path)
         return b and super().__call__(change, path)
     
 
 class JsWatcher():
 
     def __init__(self):
         self.exts = conf.FILTER_EXTS
@@ -93,15 +92,14 @@
         # first add extra for each receivers
         for inst in self.notify:
             if hasattr(inst, "extra_files"):
                 for fpath in inst.extra_files:
                     self.extra_files.add(fpath)
         roots = common_roots(self.watched_dirs + tuple(self.extra_files))
         filter = ConcatFilter(self.exts, self.extra_files)
-        print(roots[0].absolute())
         for changes in watchfiles.watch(
             *roots,
             watch_filter=filter,
             raise_interrupt=False,
             stop_event=self._stop_event):
             for change in changes:
                 if change[0] == watchfiles.Change.modified:
```

### Comparing `django_concat_js-0.2.0/concat_js/test_app/manage.py` & `django_concat_js-0.2.1/concat_js/test_app/manage.py`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.0/concat_js/test_app/settings_base.py` & `django_concat_js-0.2.1/concat_js/test_app/settings_base.py`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.0/concat_js/test_app/tests.py` & `django_concat_js-0.2.1/concat_js/test_app/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # from contextlib import contextmanager
 import json
 from pathlib import Path
 # import signal
+import subprocess
 import threading
 import time
 
 
 
 from django.test import TestCase, tag
 
@@ -178,14 +179,15 @@
         # self.clean_build_files()
         L = []
         def printer(msg):
             L.append(msg)
         bd = dg.Bundler(printer=printer)
         bd.check_timestamps()
         self.assertEqual(len(L), 0)
+        
     
     @classmethod
     def tearDownClass(cls) -> None:
         cls.clean_build_files()
         
 
 class TestSourcemaps(TestCase):
@@ -264,8 +266,29 @@
             f.write(orig_content)
         # some sleep to let changes propagate.
         time.sleep(0.2)
         watcher.stop()
         thread.join(timeout=1)
         self.assertFalse(thread.is_alive())
         self.assertEqual(len(receiver.changed), 2)
+    
+    def test_command(self):
+        # the django management command
+        subprocess.run(
+            ["python",
+            "{}".format(Path(".") / "concat_js/test_app/manage.py"),
+            "watch_js",
+            "--rebuild"],
+            timeout=1
+        )
+        with self.assertRaises(subprocess.TimeoutExpired):
+            subprocess.run(
+            ["python",
+            "{}".format(Path(".") / "concat_js/test_app/manage.py"),
+            "watch_js"],
+            timeout=1
+            )
+    
+    @classmethod
+    def tearDownClass(cls) -> None:
+        TestBundler.clean_build_files()
```

### Comparing `django_concat_js-0.2.0/concat_js/test_app/urls.py` & `django_concat_js-0.2.1/concat_js/test_app/urls.py`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.0/LICENSE.txt` & `django_concat_js-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.0/pyproject.toml` & `django_concat_js-0.2.1/pyproject.toml`

 * *Files identical despite different names*

