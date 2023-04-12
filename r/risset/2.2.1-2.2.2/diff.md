# Comparing `tmp/risset-2.2.1.tar.gz` & `tmp/risset-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risset-2.2.1.tar", last modified: Tue Apr 11 23:39:45 2023, max compression
+gzip compressed data, was "risset-2.2.2.tar", last modified: Wed Apr 12 10:24:53 2023, max compression
```

## Comparing `risset-2.2.1.tar` & `risset-2.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-11 23:39:45.492111 risset-2.2.1/
--rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-11 23:39:45.492111 risset-2.2.1/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     8076 2022-02-17 11:13:13.000000 risset-2.2.1/README.md
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-11 23:39:45.492111 risset-2.2.1/risset.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-11 23:39:45.000000 risset-2.2.1/risset.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-11 23:39:45.000000 risset-2.2.1/risset.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-11 23:39:45.000000 risset-2.2.1/risset.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       40 2023-04-11 23:39:45.000000 risset-2.2.1/risset.egg-info/entry_points.txt
--rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-11 23:39:45.000000 risset-2.2.1/risset.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-11 23:39:45.000000 risset-2.2.1/risset.egg-info/top_level.txt
--rwxrwxr-x   0 em        (1000) em        (1000)   107475 2023-04-11 23:39:39.000000 risset-2.2.1/risset.py
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-11 23:39:45.492111 risset-2.2.1/setup.cfg
--rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-10 12:28:18.000000 risset-2.2.1/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-12 10:24:53.687569 risset-2.2.2/
+-rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-12 10:24:53.687569 risset-2.2.2/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     8076 2022-02-17 11:13:13.000000 risset-2.2.2/README.md
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-12 10:24:53.686569 risset-2.2.2/risset.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-12 10:24:53.000000 risset-2.2.2/risset.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-12 10:24:53.000000 risset-2.2.2/risset.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-12 10:24:53.000000 risset-2.2.2/risset.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       40 2023-04-12 10:24:53.000000 risset-2.2.2/risset.egg-info/entry_points.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-12 10:24:53.000000 risset-2.2.2/risset.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-12 10:24:53.000000 risset-2.2.2/risset.egg-info/top_level.txt
+-rwxrwxr-x   0 em        (1000) em        (1000)   107792 2023-04-12 10:24:42.000000 risset-2.2.2/risset.py
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-12 10:24:53.687569 risset-2.2.2/setup.cfg
+-rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-10 12:28:18.000000 risset-2.2.2/setup.py
```

### Comparing `risset-2.2.1/PKG-INFO` & `risset-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risset
-Version: 2.2.1
+Version: 2.2.2
 Summary: A package manager for csound
 Home-page: https://github.com/csound-plugins/risset
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `risset-2.2.1/README.md` & `risset-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `risset-2.2.1/risset.egg-info/PKG-INFO` & `risset-2.2.2/risset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risset
-Version: 2.2.1
+Version: 2.2.2
 Summary: A package manager for csound
 Home-page: https://github.com/csound-plugins/risset
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `risset-2.2.1/risset.py` & `risset-2.2.2/risset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
-__version__ = "2.2.1"
+__version__ = "2.2.2"
 
 import sys
 
 if (sys.version_info.major, sys.version_info.minor) < (3, 8):
     print("Python 3.8 or higher is needed", file=sys.stderr)
     sys.exit(-1)
 
@@ -1850,14 +1850,23 @@
             return out
         out = {opcode.name: opcode
                for opcode in self.defined_opcodes()}
         self._cache['opcodes_by_name'] = out
         return out
 
     def parse_manpage(self, opcode: str) -> Optional[ManPage]:
+        """
+        Parse the manual page for a given opcode
+
+        Args:
+            opcode: opcode name
+
+        Returns:
+            a ManPage, if a manpage was found for the opcode, or None
+        """
         manpage = self.find_manpage(opcode, markdown=True)
         return _manpage_parse(manpage, opcode) if manpage else None
 
     def defined_opcodes(self) -> list[Opcode]:
         """
         Returns a list of opcodes
         """
@@ -1995,15 +2004,17 @@
             plugdict['url'] = plugin.url
             plugdict['short_description'] = plugin.short_description
             plugdict['long_description'] = plugin.long_description
             plugdict['author'] = plugin.author
             d[plugin.name] = plugdict
         return d
 
-    def list_plugins(self, installed=False, nameonly=False, leftcolwidth=20, oneline=False, upgradeable=False, header=True):
+    def list_plugins(self, installed=False, nameonly=False, leftcolwidth=20,
+                     oneline=False, upgradeable=False, header=True
+                     ) -> bool:
         width, height = _termsize()
         descr_max_width = width - 36
 
         if upgradeable:
             installed = True
 
         platform = _get_platform()
@@ -2054,14 +2065,15 @@
                 descr = descr[:descr_max_width] + "…"
             symbol = "*" if plugininstalled else "-"
             print(f"{symbol} {leftcol.ljust(leftcolwidth)} | {descr} {status}")
             if extra_lines:
                 for line in extra_lines:
                     print(" " * leftcolwidth + f"   |   ", line)
         print()
+        return True
 
     def show_plugin(self, pluginname: str) -> bool:
         """
         Show info about a plugin
 
         Returns True on success
         """
@@ -2441,28 +2453,29 @@
 
 
 ###############################################################
 #                        Subcommands                          #
 ###############################################################
 
 
-def cmd_list(mainindex: MainIndex, args) -> None:
+def cmd_list(mainindex: MainIndex, args) -> bool:
     """
     Lists all plugins available for download
     """
     if args.json:
         d = mainindex.list_plugins_as_dict(installed=args.installed)
         if args.outfile:
             with open(args.outfile, "w") as f:
                 json.dump(d, f, indent=2)
         else:
             print(json.dumps(d, indent=2))
+        return True
     else:
-        mainindex.list_plugins(installed=args.installed, nameonly=args.nameonly, oneline=args.oneline,
-                               upgradeable=args.upgradeable)
+        return mainindex.list_plugins(installed=args.installed, nameonly=args.nameonly, oneline=args.oneline,
+                                      upgradeable=args.upgradeable)
 
 
 def cmd_show(index: MainIndex, args) -> bool:
     """
     Returns True on success
     """
     return index.show_plugin(args.plugin)
@@ -2909,14 +2922,14 @@
             sys.exit(-1)
 
     if args.command == 'update':
         sys.exit(0)
     else:
         ok = args.func(mainindex, args)
         if not ok:
-            _errormsg("Command {args.func} failed")
+            _errormsg(f"Command {args.command} failed")
             sys.exit(-1)
         sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `risset-2.2.1/setup.py` & `risset-2.2.2/setup.py`

 * *Files identical despite different names*

