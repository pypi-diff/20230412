# Comparing `tmp/pop-config-8.0.2.tar.gz` & `tmp/pop-config-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-config-8.0.2.tar", last modified: Tue Nov 30 00:23:12 2021, max compression
+gzip compressed data, was "pop-config-9.0.0.tar", last modified: Fri Mar 11 21:43:10 2022, max compression
```

## Comparing `pop-config-8.0.2.tar` & `pop-config-9.0.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-30 00:23:12.274980 pop-config-8.0.2/
--rw-r--r--   0 root         (0) root         (0)    11343 2021-10-19 21:21:35.000000 pop-config-8.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8080 2021-11-30 00:23:12.274980 pop-config-8.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7198 2021-10-19 21:21:35.000000 pop-config-8.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-30 00:23:12.274980 pop-config-8.0.2/pop_config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-30 00:23:12.274980 pop-config-8.0.2/pop_config/args/
--rw-r--r--   0 root         (0) root         (0)     3228 2021-11-29 23:48:57.000000 pop-config-8.0.2/pop_config/args/cli.py
--rw-r--r--   0 root         (0) root         (0)     1400 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/args/init.py
--rw-r--r--   0 root         (0) root         (0)     2485 2021-11-30 00:22:59.000000 pop-config-8.0.2/pop_config/args/parser.py
--rw-r--r--   0 root         (0) root         (0)     2167 2021-10-30 01:12:29.000000 pop-config-8.0.2/pop_config/args/subcommands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-30 00:23:12.274980 pop-config-8.0.2/pop_config/comps/
--rw-r--r--   0 root         (0) root         (0)     1088 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/comps/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-30 00:23:12.274980 pop-config-8.0.2/pop_config/comps/contracts/
--rw-r--r--   0 root         (0) root         (0)      196 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/comps/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      325 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/comps/ex_group.py
--rw-r--r--   0 root         (0) root         (0)      297 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/comps/group.py
--rw-r--r--   0 root         (0) root         (0)      552 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/comps/init.py
--rw-r--r--   0 root         (0) root         (0)      616 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/comps/options.py
--rw-r--r--   0 root         (0) root         (0)      348 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/comps/subcommands.py
--rw-r--r--   0 root         (0) root         (0)     2298 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-30 00:23:12.274980 pop-config-8.0.2/pop_config/config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-30 00:23:12.274980 pop-config-8.0.2/pop_config/config/contracts/
--rw-r--r--   0 root         (0) root         (0)     2832 2021-10-19 21:21:36.000000 pop-config-8.0.2/pop_config/config/contracts/order.py
--rw-r--r--   0 root         (0) root         (0)     4077 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/config/dirs.py
--rw-r--r--   0 root         (0) root         (0)     3701 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/config/file.py
--rw-r--r--   0 root         (0) root         (0)      314 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/config/init.py
--rw-r--r--   0 root         (0) root         (0)     1049 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/config/integrate.py
--rw-r--r--   0 root         (0) root         (0)     1993 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/config/order.py
--rw-r--r--   0 root         (0) root         (0)      835 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/config/os_vars.py
--rw-r--r--   0 root         (0) root         (0)      279 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/config/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-30 00:23:12.274980 pop-config-8.0.2/pop_config/log/
--rw-r--r--   0 root         (0) root         (0)     5040 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/log/async.py
--rw-r--r--   0 root         (0) root         (0)     3017 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/log/async_timed_rolling.py
--rw-r--r--   0 root         (0) root         (0)      921 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/log/basic.py
--rw-r--r--   0 root         (0) root         (0)     1311 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/log/datagram.py
--rw-r--r--   0 root         (0) root         (0)     1021 2021-10-19 21:21:35.000000 pop-config-8.0.2/pop_config/log/init.py
--rw-r--r--   0 root         (0) root         (0)     1070 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/log/nt_event.py
--rw-r--r--   0 root         (0) root         (0)      587 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/log/null.py
--rw-r--r--   0 root         (0) root         (0)      974 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/log/rotating.py
--rw-r--r--   0 root         (0) root         (0)     1290 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/log/socket.py
--rw-r--r--   0 root         (0) root         (0)      979 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/log/timed_rotating.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-30 00:23:12.274980 pop-config-8.0.2/pop_config/render/
--rw-r--r--   0 root         (0) root         (0)     1271 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/render/cli.py
--rw-r--r--   0 root         (0) root         (0)     1356 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/render/init.py
--rw-r--r--   0 root         (0) root         (0)      447 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/render/json_conf.py
--rw-r--r--   0 root         (0) root         (0)      583 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/render/toml_conf.py
--rw-r--r--   0 root         (0) root         (0)      594 2021-10-25 14:39:22.000000 pop-config-8.0.2/pop_config/render/yaml_conf.py
--rw-r--r--   0 root         (0) root         (0)       18 2021-11-30 00:23:11.000000 pop-config-8.0.2/pop_config/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-30 00:23:12.274980 pop-config-8.0.2/pop_config.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8080 2021-11-30 00:23:12.000000 pop-config-8.0.2/pop_config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1214 2021-11-30 00:23:12.000000 pop-config-8.0.2/pop_config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-30 00:23:12.000000 pop-config-8.0.2/pop_config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       74 2021-11-30 00:23:12.000000 pop-config-8.0.2/pop_config.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2021-11-30 00:23:12.000000 pop-config-8.0.2/pop_config.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      255 2020-11-23 10:06:12.000000 pop-config-8.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       73 2021-11-30 00:23:12.274980 pop-config-8.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2719 2021-10-25 14:39:22.000000 pop-config-8.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 21:43:10.604493 pop-config-9.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11343 2022-03-11 21:42:55.000000 pop-config-9.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8080 2022-03-11 21:43:10.604493 pop-config-9.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7198 2022-03-11 21:42:55.000000 pop-config-9.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 21:43:10.601493 pop-config-9.0.0/pop_config/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 21:43:10.602493 pop-config-9.0.0/pop_config/args/
+-rw-r--r--   0 root         (0) root         (0)     3228 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/args/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/args/init.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/args/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2167 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/args/subcommands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 21:43:10.602493 pop-config-9.0.0/pop_config/comps/
+-rw-r--r--   0 root         (0) root         (0)     1088 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/comps/action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 21:43:10.602493 pop-config-9.0.0/pop_config/comps/contracts/
+-rw-r--r--   0 root         (0) root         (0)      196 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/comps/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      325 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/comps/ex_group.py
+-rw-r--r--   0 root         (0) root         (0)      297 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/comps/group.py
+-rw-r--r--   0 root         (0) root         (0)      552 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/comps/init.py
+-rw-r--r--   0 root         (0) root         (0)      616 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/comps/options.py
+-rw-r--r--   0 root         (0) root         (0)      348 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/comps/subcommands.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 21:43:10.603494 pop-config-9.0.0/pop_config/config/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 21:43:10.603494 pop-config-9.0.0/pop_config/config/contracts/
+-rw-r--r--   0 root         (0) root         (0)     2832 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/config/contracts/order.py
+-rw-r--r--   0 root         (0) root         (0)     4077 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/config/dirs.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/config/file.py
+-rw-r--r--   0 root         (0) root         (0)      314 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/config/init.py
+-rw-r--r--   0 root         (0) root         (0)     1231 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/config/integrate.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/config/order.py
+-rw-r--r--   0 root         (0) root         (0)      835 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/config/os_vars.py
+-rw-r--r--   0 root         (0) root         (0)      809 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/config/template.py
+-rw-r--r--   0 root         (0) root         (0)      279 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/config/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 21:43:10.604493 pop-config-9.0.0/pop_config/log/
+-rw-r--r--   0 root         (0) root         (0)     5040 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/log/async.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/log/async_timed_rolling.py
+-rw-r--r--   0 root         (0) root         (0)      921 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/log/basic.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/log/datagram.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/log/init.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/log/nt_event.py
+-rw-r--r--   0 root         (0) root         (0)      587 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/log/null.py
+-rw-r--r--   0 root         (0) root         (0)      974 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/log/rotating.py
+-rw-r--r--   0 root         (0) root         (0)     1290 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/log/socket.py
+-rw-r--r--   0 root         (0) root         (0)      979 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/log/timed_rotating.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 21:43:10.604493 pop-config-9.0.0/pop_config/render/
+-rw-r--r--   0 root         (0) root         (0)     1271 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/render/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/render/init.py
+-rw-r--r--   0 root         (0) root         (0)      447 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/render/json_conf.py
+-rw-r--r--   0 root         (0) root         (0)      583 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/render/toml_conf.py
+-rw-r--r--   0 root         (0) root         (0)      594 2022-03-11 21:42:55.000000 pop-config-9.0.0/pop_config/render/yaml_conf.py
+-rw-r--r--   0 root         (0) root         (0)       18 2022-03-11 21:43:10.000000 pop-config-9.0.0/pop_config/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 21:43:10.601493 pop-config-9.0.0/pop_config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8080 2022-03-11 21:43:10.000000 pop-config-9.0.0/pop_config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-03-11 21:43:10.000000 pop-config-9.0.0/pop_config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-11 21:43:10.000000 pop-config-9.0.0/pop_config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2022-03-11 21:43:10.000000 pop-config-9.0.0/pop_config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-03-11 21:43:10.000000 pop-config-9.0.0/pop_config.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      255 2022-03-11 21:42:55.000000 pop-config-9.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       73 2022-03-11 21:43:10.605494 pop-config-9.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2719 2022-03-11 21:42:55.000000 pop-config-9.0.0/setup.py
```

### Comparing `pop-config-8.0.2/LICENSE` & `pop-config-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/PKG-INFO` & `pop-config-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-config
-Version: 8.0.2
+Version: 9.0.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-config
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-config-8.0.2/README.rst` & `pop-config-9.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/args/cli.py` & `pop-config-9.0.0/pop_config/args/cli.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/args/init.py` & `pop-config-9.0.0/pop_config/args/init.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/args/parser.py` & `pop-config-9.0.0/pop_config/args/parser.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/args/subcommands.py` & `pop-config-9.0.0/pop_config/args/subcommands.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/comps/action.py` & `pop-config-9.0.0/pop_config/comps/action.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/comps/init.py` & `pop-config-9.0.0/pop_config/comps/init.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/comps/options.py` & `pop-config-9.0.0/pop_config/comps/options.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/conf.py` & `pop-config-9.0.0/pop_config/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,34 @@
     },
     "version": {
         "dyne": "__cli__",
         "default": False,
         "action": "store_true",
         "help": "Display version information",
     },
+    "config_template": {
+        "dyne": "__cli__",
+        "subcommands": ["_global_"],
+        "default": False,
+        "action": "store_true",
+        "help": "Output a config template for this command",
+    },
 }
 
 CONFIG = {
     "log_file": {
         "dyne": "__cli__",
         "default": f"{os.path.splitext(os.path.split(sys.argv[0])[1])[0]}.log",
         "help": "The location of the log file",
         "group": "Logging Options",
     },
     "log_level": {
         "dyne": "__cli__",
         "default": "warning",
-        "help": "Set the log level, either quiet, info, warning, or error",
+        "help": "Set the log level, either quiet, info, warning, debug or error",
         "group": "Logging Options",
     },
     "log_fmt_logfile": {
         "dyne": "__cli__",
         "default": "%(asctime)s,%(msecs)03d [%(name)-17s][%(levelname)-8s] %(message)s",
         "help": "The format to be given to log file messages",
         "group": "Logging Options",
```

### Comparing `pop-config-8.0.2/pop_config/config/contracts/order.py` & `pop-config-9.0.0/pop_config/config/contracts/order.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/config/dirs.py` & `pop-config-9.0.0/pop_config/config/dirs.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/config/file.py` & `pop-config-9.0.0/pop_config/config/file.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/config/integrate.py` & `pop-config-9.0.0/pop_config/config/integrate.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,12 +23,19 @@
     cli_args, raw_cli = hub.args.cli.gather(raw, cli, parse_cli)
     if cli_args.get("version"):
         hub.config.version.run(cli)
     configs = hub.config.file.parse(raw, cli, os_vars, cli_args, loader)
 
     opt = hub.config.order.apply(raw, raw_cli, cli, cli_args, os_vars, configs)
     # Sync pop-config with the log-level
-    opt["pop_config"] = {k: opt[sources[0]][k] for k in opt["pop_config"]}
+    opt["pop_config"] = {
+        k: opt[sources[0]][k] for k in opt["pop_config"] if k in opt[sources[0]]
+    }
+
+    # Output a config based on the current os and cli parameters
+    if cli_args.get("config_template"):
+        hub.config.template.run(opt)
+
     hub.OPT = hub.pop.data.imap(opt)
 
     if logs:
         hub.log[hub.OPT.pop_config.log_plugin].setup(hub.OPT.pop_config)
```

### Comparing `pop-config-8.0.2/pop_config/config/order.py` & `pop-config-9.0.0/pop_config/config/order.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/config/os_vars.py` & `pop-config-9.0.0/pop_config/config/os_vars.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/log/async.py` & `pop-config-9.0.0/pop_config/log/async.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/log/async_timed_rolling.py` & `pop-config-9.0.0/pop_config/log/async_timed_rolling.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/log/basic.py` & `pop-config-9.0.0/pop_config/log/basic.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/log/datagram.py` & `pop-config-9.0.0/pop_config/log/datagram.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/log/init.py` & `pop-config-9.0.0/pop_config/log/init.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/log/nt_event.py` & `pop-config-9.0.0/pop_config/log/nt_event.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/log/null.py` & `pop-config-9.0.0/pop_config/log/null.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/log/rotating.py` & `pop-config-9.0.0/pop_config/log/rotating.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/log/socket.py` & `pop-config-9.0.0/pop_config/log/socket.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/log/timed_rotating.py` & `pop-config-9.0.0/pop_config/log/timed_rotating.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/render/cli.py` & `pop-config-9.0.0/pop_config/render/cli.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/render/init.py` & `pop-config-9.0.0/pop_config/render/init.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/render/toml_conf.py` & `pop-config-9.0.0/pop_config/render/toml_conf.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config/render/yaml_conf.py` & `pop-config-9.0.0/pop_config/render/yaml_conf.py`

 * *Files identical despite different names*

### Comparing `pop-config-8.0.2/pop_config.egg-info/PKG-INFO` & `pop-config-9.0.0/pop_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-config
-Version: 8.0.2
+Version: 9.0.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-config
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-config-8.0.2/pop_config.egg-info/SOURCES.txt` & `pop-config-9.0.0/pop_config.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 pop_config/comps/contracts/init.py
 pop_config/config/dirs.py
 pop_config/config/file.py
 pop_config/config/init.py
 pop_config/config/integrate.py
 pop_config/config/order.py
 pop_config/config/os_vars.py
+pop_config/config/template.py
 pop_config/config/version.py
 pop_config/config/contracts/order.py
 pop_config/log/async.py
 pop_config/log/async_timed_rolling.py
 pop_config/log/basic.py
 pop_config/log/datagram.py
 pop_config/log/init.py
```

### Comparing `pop-config-8.0.2/setup.py` & `pop-config-9.0.0/setup.py`

 * *Files identical despite different names*

