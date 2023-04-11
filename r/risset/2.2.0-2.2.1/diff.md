# Comparing `tmp/risset-2.2.0.tar.gz` & `tmp/risset-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risset-2.2.0.tar", last modified: Mon Apr 10 12:31:18 2023, max compression
+gzip compressed data, was "risset-2.2.1.tar", last modified: Tue Apr 11 23:39:45 2023, max compression
```

## Comparing `risset-2.2.0.tar` & `risset-2.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-10 12:31:18.323536 risset-2.2.0/
--rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-10 12:31:18.323536 risset-2.2.0/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     8076 2022-02-17 11:13:13.000000 risset-2.2.0/README.md
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-10 12:31:18.323536 risset-2.2.0/risset.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-10 12:31:18.000000 risset-2.2.0/risset.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-10 12:31:18.000000 risset-2.2.0/risset.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-10 12:31:18.000000 risset-2.2.0/risset.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       40 2023-04-10 12:31:18.000000 risset-2.2.0/risset.egg-info/entry_points.txt
--rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-10 12:31:18.000000 risset-2.2.0/risset.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-10 12:31:18.000000 risset-2.2.0/risset.egg-info/top_level.txt
--rwxrwxr-x   0 em        (1000) em        (1000)   107324 2023-04-10 12:31:10.000000 risset-2.2.0/risset.py
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-10 12:31:18.323536 risset-2.2.0/setup.cfg
--rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-10 12:28:18.000000 risset-2.2.0/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-11 23:39:45.492111 risset-2.2.1/
+-rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-11 23:39:45.492111 risset-2.2.1/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     8076 2022-02-17 11:13:13.000000 risset-2.2.1/README.md
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-11 23:39:45.492111 risset-2.2.1/risset.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-11 23:39:45.000000 risset-2.2.1/risset.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-11 23:39:45.000000 risset-2.2.1/risset.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-11 23:39:45.000000 risset-2.2.1/risset.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       40 2023-04-11 23:39:45.000000 risset-2.2.1/risset.egg-info/entry_points.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-11 23:39:45.000000 risset-2.2.1/risset.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-11 23:39:45.000000 risset-2.2.1/risset.egg-info/top_level.txt
+-rwxrwxr-x   0 em        (1000) em        (1000)   107475 2023-04-11 23:39:39.000000 risset-2.2.1/risset.py
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-11 23:39:45.492111 risset-2.2.1/setup.cfg
+-rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-10 12:28:18.000000 risset-2.2.1/setup.py
```

### Comparing `risset-2.2.0/PKG-INFO` & `risset-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risset
-Version: 2.2.0
+Version: 2.2.1
 Summary: A package manager for csound
 Home-page: https://github.com/csound-plugins/risset
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `risset-2.2.0/README.md` & `risset-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `risset-2.2.0/risset.egg-info/PKG-INFO` & `risset-2.2.1/risset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risset
-Version: 2.2.0
+Version: 2.2.1
 Summary: A package manager for csound
 Home-page: https://github.com/csound-plugins/risset
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `risset-2.2.0/risset.py` & `risset-2.2.1/risset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 
 import sys
 
 if (sys.version_info.major, sys.version_info.minor) < (3, 8):
     print("Python 3.8 or higher is needed", file=sys.stderr)
     sys.exit(-1)
 
@@ -1995,24 +1995,27 @@
             plugdict['url'] = plugin.url
             plugdict['short_description'] = plugin.short_description
             plugdict['long_description'] = plugin.long_description
             plugdict['author'] = plugin.author
             d[plugin.name] = plugdict
         return d
 
-    def list_plugins(self, installed=False, nameonly=False, leftcolwidth=20, oneline=False, upgradeable=False):
+    def list_plugins(self, installed=False, nameonly=False, leftcolwidth=20, oneline=False, upgradeable=False, header=True):
         width, height = _termsize()
         descr_max_width = width - 36
 
         if upgradeable:
             installed = True
 
         platform = _get_platform()
         csoundversion = _session.csound_version
 
+        print(f"Csound Version: {csoundversion}")
+        print()
+
         for plugin in self.plugins.values():
             data = []
             info = self.installed_plugin_info(plugin)
             plugininstalled = info is not None
 
             if not plugininstalled and installed:
                 continue
@@ -2041,15 +2044,15 @@
             else:
                 status = ""
             leftcol = f"{plugin.name} /{plugin.version}"
             descr = plugin.short_description
             bindef = plugin.find_binary()
             if not bindef:
                 available = ', '.join(plugin.available_binaries())
-                extra_lines.append(f"-- No binaries for {platform}/{_session.csound_version}")
+                extra_lines.append(f"-- No binaries for {platform}/{csoundversion}")
                 extra_lines.append(f"   Available binaries: {available}")
             if oneline and len(descr) > descr_max_width:
                 descr = descr[:descr_max_width] + "…"
             symbol = "*" if plugininstalled else "-"
             print(f"{symbol} {leftcol.ljust(leftcolwidth)} | {descr} {status}")
             if extra_lines:
                 for line in extra_lines:
@@ -2894,23 +2897,26 @@
         _debug(f"Creating main index - csound major version: {csoundversion}")
         if not update:
             mainindex = _mainindex_retrieve() or MainIndex(update=False, majorversion=csoundversion)
         else:
             # this will serialize the mainindex
             mainindex = MainIndex(update=True, majorversion=csoundversion)
     except Exception as e:
-        _debug("Failed to create main index")
+        _errormsg("Failed to create main index")
         if _session.debug:
             raise e
         else:
             _errormsg(str(e))
             sys.exit(-1)
 
     if args.command == 'update':
         sys.exit(0)
     else:
         ok = args.func(mainindex, args)
-        sys.exit(0 if ok else -1)
-    
+        if not ok:
+            _errormsg("Command {args.func} failed")
+            sys.exit(-1)
+        sys.exit(0)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `risset-2.2.0/setup.py` & `risset-2.2.1/setup.py`

 * *Files identical despite different names*

