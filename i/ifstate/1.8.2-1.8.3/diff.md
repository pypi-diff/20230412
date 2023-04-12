# Comparing `tmp/ifstate-1.8.2.tar.gz` & `tmp/ifstate-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifstate-1.8.2.tar", last modified: Fri Feb 17 22:11:39 2023, max compression
+gzip compressed data, was "ifstate-1.8.3.tar", last modified: Wed Apr 12 20:37:32 2023, max compression
```

## Comparing `ifstate-1.8.2.tar` & `ifstate-1.8.3.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-17 22:11:25.000000 ifstate-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-02-17 22:11:39.483735 ifstate-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-17 22:11:25.000000 ifstate-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.479735 ifstate-1.8.2/ifstate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:25.000000 ifstate-1.8.2/ifstate/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6364 2023-02-17 22:11:25.000000 ifstate-1.8.2/ifstate/ifstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-02-17 22:11:25.000000 ifstate-1.8.2/ifstate/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.479735 ifstate-1.8.2/ifstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-02-17 22:11:39.000000 ifstate-1.8.2/ifstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-02-17 22:11:39.000000 ifstate-1.8.2/ifstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 22:11:39.000000 ifstate-1.8.2/ifstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-17 22:11:39.000000 ifstate-1.8.2/ifstate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-17 22:11:39.000000 ifstate-1.8.2/ifstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-17 22:11:39.000000 ifstate-1.8.2/ifstate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/libifstate/
--rw-r--r--   0 runner    (1001) docker     (123)    23262 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/libifstate/address/
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/address/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/libifstate/bpf/
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/bpf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/bpf/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/bpf/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/libifstate/brport/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/brport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/libifstate/link/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21912 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/link/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/link/physical.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/link/veth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/libifstate/neighbour/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/neighbour/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/libifstate/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/parser/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/libifstate/routing/
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/routing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/libifstate/sysctl/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/sysctl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/libifstate/tc/
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/libifstate/wireguard/
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/wireguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/libifstate/xdp/
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-02-17 22:11:25.000000 ifstate-1.8.2/libifstate/xdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:11:39.483735 ifstate-1.8.2/schema/
--rw-r--r--   0 runner    (1001) docker     (123)   174283 2023-02-17 22:11:25.000000 ifstate-1.8.2/schema/ifstate.conf.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 22:11:39.483735 ifstate-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-02-17 22:11:25.000000 ifstate-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.707270 ifstate-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 20:37:24.000000 ifstate-1.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-12 20:37:32.707270 ifstate-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-12 20:37:24.000000 ifstate-1.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/ifstate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:24.000000 ifstate-1.8.3/ifstate/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6391 2023-04-12 20:37:24.000000 ifstate-1.8.3/ifstate/ifstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-12 20:37:24.000000 ifstate-1.8.3/ifstate/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/ifstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-12 20:37:32.000000 ifstate-1.8.3/ifstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-12 20:37:32.000000 ifstate-1.8.3/ifstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:37:32.000000 ifstate-1.8.3/ifstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 20:37:32.000000 ifstate-1.8.3/ifstate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 20:37:32.000000 ifstate-1.8.3/ifstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 20:37:32.000000 ifstate-1.8.3/ifstate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/
+-rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/address/
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/address/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/bpf/
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/bpf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/bpf/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/bpf/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/brport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/brport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/link/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/link/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/link/physical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/link/tun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/link/veth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/neighbour/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/neighbour/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/parser/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.707270 ifstate-1.8.3/libifstate/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/routing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.707270 ifstate-1.8.3/libifstate/sysctl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/sysctl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.707270 ifstate-1.8.3/libifstate/tc/
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.707270 ifstate-1.8.3/libifstate/wireguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/wireguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.707270 ifstate-1.8.3/libifstate/xdp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/xdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)   178382 2023-04-12 20:37:24.000000 ifstate-1.8.3/schema/ifstate.conf.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:37:32.707270 ifstate-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-12 20:37:24.000000 ifstate-1.8.3/setup.py
```

### Comparing `ifstate-1.8.2/LICENSE` & `ifstate-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/PKG-INFO` & `ifstate-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifstate
-Version: 1.8.2
+Version: 1.8.3
 Summary: Manage host interface settings in a declarative manner
 Home-page: https://ifstate.net/
 Author: Thomas Liske
 Author-email: thomas@fiasko-nw.net
 License: GPL3+
 Description-Content-Type: text/markdown
 Provides-Extra: shell
```

### Comparing `ifstate-1.8.2/README.md` & `ifstate-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/ifstate/ifstate.py` & `ifstate-1.8.3/ifstate/ifstate.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     else:
         lvl = logging.INFO
 
     if args.action == Actions.SHELL:
         shell()
         exit(0)
 
-    ifslog = IfStateLogging(lvl)
+    ifslog = IfStateLogging(lvl, action=args.action)
     ifs = IfState()
 
     if args.action in [Actions.SHOW, Actions.SHOWALL]:
         # preserve dict order on python 3.7+
         if sys.version_info >= (3, 7):
             yaml.add_representer(
                 dict, lambda self, data: yaml.representer.SafeRepresenter.represent_dict(self, data.items()))
@@ -133,15 +133,15 @@
         if args.action == Actions.CHECK:
             try:
                 ifs.check()
             except LinkNoConfigFound:
                 pass
         elif args.action == Actions.VRRP_FIFO:
             status_pattern = re.compile(
-                r'(group|instance) "([^"]+)" (unknown|fault|backup|master)$', re.IGNORECASE)
+                r'(group|instance) "([^"]+)" (unknown|fault|backup|master)( \d+)?$', re.IGNORECASE)
 
             with open(args.fifo) as fifo:
                 for line in fifo:
                     m = status_pattern.match(line.strip())
                     if m:
                         signal.signal(signal.SIGHUP, signal.SIG_IGN)
                         signal.signal(signal.SIGPIPE, signal.SIG_IGN)
```

### Comparing `ifstate-1.8.2/ifstate/shell.py` & `ifstate-1.8.3/ifstate/shell.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/ifstate.egg-info/PKG-INFO` & `ifstate-1.8.3/ifstate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifstate
-Version: 1.8.2
+Version: 1.8.3
 Summary: Manage host interface settings in a declarative manner
 Home-page: https://ifstate.net/
 Author: Thomas Liske
 Author-email: thomas@fiasko-nw.net
 License: GPL3+
 Description-Content-Type: text/markdown
 Provides-Extra: shell
```

### Comparing `ifstate-1.8.2/ifstate.egg-info/SOURCES.txt` & `ifstate-1.8.3/ifstate.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 libifstate/bpf/__init__.py
 libifstate/bpf/ctypes.py
 libifstate/bpf/map.py
 libifstate/brport/__init__.py
 libifstate/link/__init__.py
 libifstate/link/base.py
 libifstate/link/physical.py
+libifstate/link/tun.py
 libifstate/link/veth.py
 libifstate/neighbour/__init__.py
 libifstate/parser/__init__.py
 libifstate/parser/base.py
 libifstate/parser/yaml.py
 libifstate/routing/__init__.py
 libifstate/sysctl/__init__.py
```

### Comparing `ifstate-1.8.2/libifstate/__init__.py` & `ifstate-1.8.3/libifstate/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 import os
 import pkgutil
 import re
 import json
 import errno
 import logging
 
-__version__ = "1.8.2"
+__version__ = "1.8.3"
 
 
 class IfState():
     def __init__(self):
         logger.debug('IfState {}'.format(__version__))
         self.links = {}
         self.addresses = {}
@@ -258,30 +258,42 @@
         self._apply(True, vrrp_type, vrrp_name, vrrp_state)
 
     def check(self, vrrp_type=None, vrrp_name=None, vrrp_state=None):
         self._apply(False, vrrp_type, vrrp_name, vrrp_state)
 
     def _apply(self, do_apply, vrrp_type, vrrp_name, vrrp_state):
         vrrp_ignore = []
-        vrrp_remove = []
+        vrrp_disable = []
 
         by_vrrp = not None in [
             vrrp_type, vrrp_name, vrrp_state]
 
+        if by_vrrp:
+            logger.info("vrrp state change: {} {} => {}".format(vrrp_type, vrrp_name, vrrp_state))
+
+            # ifstate schema requires lower case keywords
+            vrrp_type = vrrp_type.lower()
+            vrrp_state = vrrp_state.lower()
+
+        # check which links to remove or ignore:
+        #   remove: vrrp type & name matches, but vrrp state not
+        #   ignore: vrrp type & name does not match
         for ifname, link in self.links.items():
             if ifname in self.vrrp['links']:
                 if not by_vrrp:
                     vrrp_ignore.append(ifname)
                 else:
                     if not link.match_vrrp_select(vrrp_type, vrrp_name):
                         vrrp_ignore.append(ifname)
                     elif not vrrp_name in self.vrrp[vrrp_type] or not vrrp_state in self.vrrp[vrrp_type][vrrp_name] or not ifname in self.vrrp[vrrp_type][vrrp_name][vrrp_state]:
-                        vrrp_remove.append(ifname)
+                        vrrp_disable.append(ifname)
             elif by_vrrp:
                 vrrp_ignore.append(ifname)
+        logger.debug("vrrp links to be disabled: {}".format(", ".join(vrrp_disable)))
+        logger.debug("vrrp links to be ignored: {}".format(", ".join(vrrp_ignore)))
 
         self.ipaddr_ignore = set()
         for ip in self.ignore.get('ipaddr', []):
             self.ipaddr_ignore.add(ip_network(ip))
 
         if not any(not x is None for x in self.links.values()):
             logger.error("DANGER: Not a single link config has been found!")
@@ -295,18 +307,18 @@
         if not self.bpf_progs is None:
             self.bpf_progs.apply(do_apply)
 
         for stage in range(2):
             if stage == 0:
                 logger.info("\nconfiguring interface links")
 
-                for ifname in vrrp_remove:
-                    logger.debug('to be removed due to vrrp constraint',
+                for ifname in vrrp_disable:
+                    logger.debug('to be disabled due to vrrp constraint',
                                  extra={'iface': ifname})
-                    del self.links[ifname]
+                    self.links[ifname].settings['state'] = 'down'
             else:
                 logger.info("\nconfiguring interface links (stage 2)")
 
             retry = False
             applied = []
             while len(applied) + len(vrrp_ignore) < len(self.links):
                 last = len(applied)
@@ -321,15 +333,15 @@
 
                     if link is None:
                         logger.debug('skipped due to no link settings',
                                      extra={'iface': name})
                         applied.append(name)
                     else:
                         deps = link.depends()
-                        if all(x in applied for x in deps):
+                        if all(x in applied+vrrp_ignore for x in deps):
                             excpts = link.apply(do_apply, self.sysctl)
                             if excpts.has_errno(errno.EEXIST):
                                 retry = True
                             applied.append(name)
                 if last == len(applied):
                     raise LinkCircularLinked()
```

### Comparing `ifstate-1.8.2/libifstate/address/__init__.py` & `ifstate-1.8.3/libifstate/address/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/bpf/__init__.py` & `ifstate-1.8.3/libifstate/bpf/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/bpf/ctypes.py` & `ifstate-1.8.3/libifstate/bpf/ctypes.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/bpf/map.py` & `ifstate-1.8.3/libifstate/bpf/map.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/brport/__init__.py` & `ifstate-1.8.3/libifstate/brport/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/exception.py` & `ifstate-1.8.3/libifstate/exception.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/link/base.py` & `ifstate-1.8.3/libifstate/link/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,19 @@
             1: 'fast',
         },
         'bond_ad_select': {
             0: "stable",
             1: "bandwidth",
             2: "count",
         },
+        # === tuntap ===
+        'tun_type': {
+            1: 'tun',
+            2: 'tap',
+        },
         # === vlan ===
         'vlan_protocol': {
             0x88a8: '802.1ad',
             0x8100: '802.1q',
         },
     }
     attr_value_lookup = {
@@ -104,15 +109,15 @@
         self.attr_map = {
             'kind': ['IFLA_LINKINFO', 'IFLA_INFO_KIND'],
         }
         self.attr_idx = ['link', 'master', 'gre_link',
                          'ip6gre_link', 'vxlan_link', 'xfrm_link']
         self.idx = None
 
-        if 'address' in self.settings:
+        if 'address' in self.settings and self.settings['kind'] == 'physical':
             self.settings['address'] = self.settings['address'].lower()
             self.idx = next(iter(ipr.link_lookup(
                 address=self.settings['address'])), None)
         if 'permaddr' in self.settings:
             self.settings['permaddr'] = self.settings['permaddr'].lower()
             self.idx = ipr.get_iface_by_permaddr(self.settings['permaddr'])
         if 'businfo' in self.settings:
@@ -365,15 +370,15 @@
             try:
                 ipr.link('del', index=self.idx)
             except Exception as err:
                 if not isinstance(err, netlinkerror_classes):
                     raise
                 excpts.add('del', err)
         self.idx = None
-        self.create(do_apply, ifstate, excpts, "replace")
+        self.create(do_apply, sysctl, excpts, "replace")
 
     def update(self, do_apply, sysctl, excpts):
         logger.debug('checking link', extra={'iface': self.settings['ifname']})
 
         old_state = self.iface['state']
         has_link_changes = False
         has_state_changes = False
@@ -501,21 +506,22 @@
                         self.settings['state'] = 'up'
 
                     has_state_changes = self.settings['state'] == 'up'
 
                 self.brport.apply(do_apply, self.idx, excpts)
 
             if has_state_changes:
-                try:
-                    ipr.link('set', index=self.idx,
-                             state=self.settings["state"])
-                except Exception as err:
-                    if not isinstance(err, netlinkerror_classes):
-                        raise
-                    excpts.add('set', err, state=state)
+                if do_apply:
+                    try:
+                        ipr.link('set', index=self.idx,
+                                 state=self.settings["state"])
+                    except Exception as err:
+                        if not isinstance(err, netlinkerror_classes):
+                            raise
+                        excpts.add('set', err, state=state)
                 logger.info('change', extra={
                             'iface': self.settings['ifname'], 'style': IfStateLogging.STYLE_CHG})
 
             else:
                 logger.info(
                     'ok', extra={'iface': self.settings['ifname'], 'style': IfStateLogging.STYLE_OK})
```

### Comparing `ifstate-1.8.2/libifstate/link/physical.py` & `ifstate-1.8.3/libifstate/link/physical.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/link/veth.py` & `ifstate-1.8.3/libifstate/link/veth.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/neighbour/__init__.py` & `ifstate-1.8.3/libifstate/neighbour/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/parser/base.py` & `ifstate-1.8.3/libifstate/parser/base.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/parser/yaml.py` & `ifstate-1.8.3/libifstate/parser/yaml.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/routing/__init__.py` & `ifstate-1.8.3/libifstate/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/sysctl/__init__.py` & `ifstate-1.8.3/libifstate/sysctl/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/tc/__init__.py` & `ifstate-1.8.3/libifstate/tc/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/util.py` & `ifstate-1.8.3/libifstate/util.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/wireguard/__init__.py` & `ifstate-1.8.3/libifstate/wireguard/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/libifstate/xdp/__init__.py` & `ifstate-1.8.3/libifstate/xdp/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.2/schema/ifstate.conf.schema.json` & `ifstate-1.8.3/schema/ifstate.conf.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999999987199813%*

 * *Differences: {"'properties'": "{'interfaces': {'items': {'properties': {'link': {'oneOf': {7: {'description': "*

 * *                 "'Virtual software device (TUN/TAP)', 'required': {insert: [(1, 'tun_type')]}, "*

 * *                 "'properties': {'kind': {'const': 'tun'}, 'tun_type': "*

 * *                 "OrderedDict([('description', 'device mode (Ethernet headers)'), ('default', "*

 * *                 "'tap'), ('enum', [1, 'tun', 2, 'tap'])]), 'tun_pi': OrderedDict([('description', "*

 * *                 "'provide packet information […]*

```diff
@@ -1863,44 +1863,122 @@
                                     }
                                 },
                                 "required": [
                                     "kind"
                                 ]
                             },
                             {
-                                "description": "Virtual software device",
+                                "additionalProperties": false,
+                                "description": "Virtual software device (TUN/TAP)",
                                 "properties": {
                                     "address": {
                                         "$ref": "#/$defs/iface-link_address"
                                     },
                                     "group": {
                                         "$ref": "#/$defs/iface-link_group"
                                     },
                                     "ifalias": {
                                         "$ref": "#/$defs/iface-link_ifalias"
                                     },
                                     "kind": {
-                                        "const": "tuntap",
+                                        "const": "tun",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
+                                    "tun_group": {
+                                        "description": "device group",
+                                        "type": [
+                                            "integer",
+                                            "string"
+                                        ]
+                                    },
+                                    "tun_multi_queue": {
+                                        "default": false,
+                                        "description": "enable multiqueue tuntap",
+                                        "enum": [
+                                            0,
+                                            false,
+                                            1,
+                                            true
+                                        ],
+                                        "type": [
+                                            "boolean",
+                                            "integer"
+                                        ]
+                                    },
+                                    "tun_owner": {
+                                        "description": "device owner",
+                                        "type": [
+                                            "integer",
+                                            "string"
+                                        ]
+                                    },
+                                    "tun_persist": {
+                                        "default": false,
+                                        "description": "persistent device; non-persistent devices cannot be created",
+                                        "enum": [
+                                            0,
+                                            false,
+                                            1,
+                                            true
+                                        ],
+                                        "type": [
+                                            "boolean",
+                                            "integer"
+                                        ]
+                                    },
+                                    "tun_pi": {
+                                        "default": false,
+                                        "description": "provide packet information",
+                                        "enum": [
+                                            0,
+                                            false,
+                                            1,
+                                            true
+                                        ],
+                                        "type": [
+                                            "boolean",
+                                            "integer"
+                                        ]
+                                    },
+                                    "tun_type": {
+                                        "default": "tap",
+                                        "description": "device mode (Ethernet headers)",
+                                        "enum": [
+                                            1,
+                                            "tun",
+                                            2,
+                                            "tap"
+                                        ]
+                                    },
+                                    "tun_vnet_hdr": {
+                                        "default": false,
+                                        "description": "prepend frames with struct virtio_net_hdr",
+                                        "enum": [
+                                            0,
+                                            false,
+                                            1,
+                                            true
+                                        ]
+                                    },
                                     "txqlen": {
                                         "$ref": "#/$defs/iface-link_txqlen"
                                     }
                                 },
                                 "required": [
-                                    "kind"
+                                    "kind",
+                                    "tun_type"
                                 ]
                             },
                             {
                                 "description": "Virtual Routing and Forwarding device",
                                 "properties": {
                                     "address": {
                                         "$ref": "#/$defs/iface-link_address"
```

### Comparing `ifstate-1.8.2/setup.py` & `ifstate-1.8.3/setup.py`

 * *Files identical despite different names*

