# Comparing `tmp/pylookout-0.2.5.tar.gz` & `tmp/pylookout-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylookout-0.2.5.tar", last modified: Tue Apr 11 19:28:57 2023, max compression
+gzip compressed data, was "pylookout-0.2.6.tar", last modified: Wed Apr 12 20:02:46 2023, max compression
```

## Comparing `pylookout-0.2.5.tar` & `pylookout-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:28:57.954370 pylookout-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-11 19:28:46.000000 pylookout-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-11 19:28:57.954370 pylookout-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-11 19:28:46.000000 pylookout-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:28:57.954370 pylookout-0.2.5/pylookout/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 19:28:46.000000 pylookout-0.2.5/pylookout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 19:28:46.000000 pylookout-0.2.5/pylookout/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-11 19:28:46.000000 pylookout-0.2.5/pylookout/info_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-11 19:28:46.000000 pylookout-0.2.5/pylookout/lookout.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-11 19:28:46.000000 pylookout-0.2.5/pylookout/lookout_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-11 19:28:46.000000 pylookout-0.2.5/pylookout/notification_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:28:57.954370 pylookout-0.2.5/pylookout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-11 19:28:57.000000 pylookout-0.2.5/pylookout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-11 19:28:57.000000 pylookout-0.2.5/pylookout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:28:57.000000 pylookout-0.2.5/pylookout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-11 19:28:57.000000 pylookout-0.2.5/pylookout.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 19:28:57.000000 pylookout-0.2.5/pylookout.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 19:28:57.000000 pylookout-0.2.5/pylookout.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-11 19:28:46.000000 pylookout-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-11 19:28:57.958370 pylookout-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:28:46.000000 pylookout-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:02:46.440396 pylookout-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 20:02:34.000000 pylookout-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-12 20:02:46.440396 pylookout-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-12 20:02:34.000000 pylookout-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:02:46.436396 pylookout-0.2.6/pylookout/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 20:02:34.000000 pylookout-0.2.6/pylookout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 20:02:34.000000 pylookout-0.2.6/pylookout/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-12 20:02:34.000000 pylookout-0.2.6/pylookout/info_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-04-12 20:02:34.000000 pylookout-0.2.6/pylookout/lookout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-12 20:02:34.000000 pylookout-0.2.6/pylookout/lookout_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-12 20:02:34.000000 pylookout-0.2.6/pylookout/notification_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:02:46.440396 pylookout-0.2.6/pylookout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-12 20:02:46.000000 pylookout-0.2.6/pylookout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 20:02:46.000000 pylookout-0.2.6/pylookout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:02:46.000000 pylookout-0.2.6/pylookout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 20:02:46.000000 pylookout-0.2.6/pylookout.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 20:02:46.000000 pylookout-0.2.6/pylookout.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 20:02:46.000000 pylookout-0.2.6/pylookout.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-12 20:02:34.000000 pylookout-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-12 20:02:46.440396 pylookout-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:02:34.000000 pylookout-0.2.6/setup.py
```

### Comparing `pylookout-0.2.5/LICENSE` & `pylookout-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pylookout-0.2.5/PKG-INFO` & `pylookout-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylookout
-Version: 0.2.5
+Version: 0.2.6
 Summary: Simple Linux system monitoring tool
 Home-page: https://github.com/Lab-Brat/pyLookout
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pylookout-0.2.5/README.md` & `pylookout-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pylookout-0.2.5/pylookout/info_collector.py` & `pylookout-0.2.6/pylookout/info_collector.py`

 * *Files identical despite different names*

### Comparing `pylookout-0.2.5/pylookout/lookout.py` & `pylookout-0.2.6/pylookout/lookout.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+import os
 import logging
-from pathlib import Path
 from time import sleep
+from pathlib import Path
 from .info_collector import Collector
 from .notification_methods import simple_push, sendgrid
 
 
 class PyLookout:
     def __init__(
         self,
-        threshold=75,
-        method="local",
-        check_containers=False,
+        threshold,
+        method,
+        logins,
+        check_containers,
     ):
         logging.basicConfig(
             format="%(asctime)s %(message)s",
             level=logging.INFO,
             handlers=[
                 logging.FileHandler(f"{str(Path.home())}/.pylookout.log"),
                 logging.StreamHandler(),
@@ -22,14 +24,15 @@
         )
 
         self.logger = logging.getLogger()
         self.info = Collector(check_containers)
         self.logger.info("Information collected successfully!")
         self.critical = threshold
         self.method = method
+        self.logins = logins
         self.containers = check_containers
         self.notification = []
 
     def _messge_percent(self, metric, percent):
         """
         Notification message.
         """
@@ -99,19 +102,21 @@
 
     def _add_login_info(self):
         """
         Add login information to notification message.
         """
         if self.info.logins:
             user_ips = ""
-            for login in self.info.logins:
+            for i, login in enumerate(self.info.logins):
                 user_ips += f"{login['user']}->{login['ip']} "
-            self.notification.append(
-                f"{len(self.info.logins)} active logins: {user_ips}"
-            )
+
+            if i + 1 > self.logins:
+                self.notification.append(
+                    f"{len(self.info.logins)} active logins: {user_ips}"
+                )
 
     def _stressed(self, metric, percent):
         """
         Compare a metric with the critical value.
         """
         stressed = True if percent > self.critical else False
 
@@ -142,7 +147,24 @@
         Run checker in background.
         """
         while True:
             self.logger.info("Running checker...")
             self.checker()
             self.logger.info("Checker finished. Sleeping for 60 seconds...")
             sleep(60)
+
+    def create_config(self, flags=""):
+        """
+        Create a systemd service file.
+        """
+        user = os.getenv("USER")
+        service_file = f"/home/{user}/.config/systemd/user/pylookout.service"
+        with open(service_file, "w+") as file:
+            file.write("[Unit]\n")
+            file.write("Description=Launch pyLookout monitoring app\n\n")
+            file.write("[Service]\n")
+            file.write(
+                f"ExecStart=/home/{user}/.local/bin/pylookout {flags}\n\n"
+            )
+            file.write("[Install]\n")
+            file.write("WantedBy=default.target\n\n")
+        os.system("systemctl --user daemon-reload")
```

### Comparing `pylookout-0.2.5/pylookout/notification_methods.py` & `pylookout-0.2.6/pylookout/notification_methods.py`

 * *Files identical despite different names*

### Comparing `pylookout-0.2.5/pylookout.egg-info/PKG-INFO` & `pylookout-0.2.6/pylookout.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylookout
-Version: 0.2.5
+Version: 0.2.6
 Summary: Simple Linux system monitoring tool
 Home-page: https://github.com/Lab-Brat/pyLookout
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pylookout-0.2.5/setup.cfg` & `pylookout-0.2.6/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylookout
-version = 0.2.5
+version = 0.2.6
 description = Simple Linux system monitoring tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Lab-Brat
 author_email = labbrat_social@pm.me
 url = https://github.com/Lab-Brat/pyLookout
 license = MIT
```

