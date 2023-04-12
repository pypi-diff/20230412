# Comparing `tmp/LocalResolver-1.0.0.tar.gz` & `tmp/LocalResolver-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LocalResolver-1.0.0.tar", last modified: Tue Apr 11 17:28:14 2023, max compression
+gzip compressed data, was "LocalResolver-1.0.1.tar", last modified: Wed Apr 12 11:39:06 2023, max compression
```

## Comparing `LocalResolver-1.0.0.tar` & `LocalResolver-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-11 17:28:14.629609 LocalResolver-1.0.0/
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-04-07 01:27:34.000000 LocalResolver-1.0.0/LICENSE.txt
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-11 17:28:14.629609 LocalResolver-1.0.0/LocalResolver.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2791 2023-04-11 17:28:14.000000 LocalResolver-1.0.0/LocalResolver.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      283 2023-04-11 17:28:14.000000 LocalResolver-1.0.0/LocalResolver.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-11 17:28:14.000000 LocalResolver-1.0.0/LocalResolver.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       53 2023-04-11 17:28:14.000000 LocalResolver-1.0.0/LocalResolver.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       21 2023-04-11 17:28:14.000000 LocalResolver-1.0.0/LocalResolver.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       14 2023-04-11 17:28:14.000000 LocalResolver-1.0.0/LocalResolver.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    41489 2023-04-11 23:26:24.000000 LocalResolver-1.0.0/LocalResolver.py
--rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-04-07 01:27:34.000000 LocalResolver-1.0.0/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     2791 2023-04-11 17:28:14.629609 LocalResolver-1.0.0/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1626 2023-04-11 23:24:00.000000 LocalResolver-1.0.0/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-11 17:28:14.629609 LocalResolver-1.0.0/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1556 2023-04-11 23:23:52.000000 LocalResolver-1.0.0/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-12 11:39:06.892926 LocalResolver-1.0.1/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-04-11 23:57:46.000000 LocalResolver-1.0.1/LICENSE.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-12 11:39:06.892926 LocalResolver-1.0.1/LocalResolver.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3108 2023-04-12 11:39:06.000000 LocalResolver-1.0.1/LocalResolver.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      293 2023-04-12 11:39:06.000000 LocalResolver-1.0.1/LocalResolver.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-12 11:39:06.000000 LocalResolver-1.0.1/LocalResolver.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       53 2023-04-12 11:39:06.000000 LocalResolver-1.0.1/LocalResolver.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2023-04-12 11:39:06.000000 LocalResolver-1.0.1/LocalResolver.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       14 2023-04-12 11:39:06.000000 LocalResolver-1.0.1/LocalResolver.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    40871 2023-04-12 17:35:36.000000 LocalResolver-1.0.1/LocalResolver.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-04-11 23:57:46.000000 LocalResolver-1.0.1/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     3108 2023-04-12 11:39:06.892926 LocalResolver-1.0.1/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1943 2023-04-11 23:57:46.000000 LocalResolver-1.0.1/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-12 11:39:06.892926 LocalResolver-1.0.1/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1556 2023-04-12 17:34:48.000000 LocalResolver-1.0.1/setup.py
```

### Comparing `LocalResolver-1.0.0/LICENSE.txt` & `LocalResolver-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LocalResolver-1.0.0/LocalResolver.egg-info/PKG-INFO` & `LocalResolver-1.0.1/LocalResolver.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LocalResolver
-Version: 1.0.0
+Version: 1.0.1
 Summary: This package implements local hostname resolver tool with scapy.
 Home-page: https://github.com/mauricelambert/LocalResolver
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
@@ -31,14 +31,22 @@
 
 # LocalResolver
 
 ## Description
 
 This package implements local hostname resolver tool with scapy (using netbios and LLMNR query).
 
+This tool is useful to:
+ - reverse lookup local IP addresses
+ - resolve manually hostnames/IP from Linux or hardened Windows
+ - resolve hostname with old machines (Windows 2000-2012)
+ - identify:
+     - Machines with old protocols like Netbios or LLMNR,
+     - Hostname spoofer (or two machines with the same name),
+
 ## Requirements
 
 This package require: 
 
  - python3
  - python3 Standard Library
  - Scapy
```

### Comparing `LocalResolver-1.0.0/LocalResolver.py` & `LocalResolver-1.0.1/LocalResolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 ~# sudo systemctl restart systemd-resolved
 ~# sudo systemctl start nmbd
 ~# sudo systemctl start avahi-daemon
 ~# sudo responder -I eth0
 ~# 
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = (
     "This package implements local hostname resolver tool with scapy."
 )
@@ -114,16 +114,14 @@
 from collections.abc import Callable
 from logging import getLogger, ERROR
 from collections import defaultdict
 from dataclasses import dataclass
 from argparse import Namespace
 from os import name
 
-is_windows: bool = name == "nt"
-
 
 def netbios_encode(name: str) -> str:
     """
     This function encodes name in Netbios encoding.
 
     >>> netbios_encode('FRED')
     'EGFCEFEECACACACACACACACACACACACA'
@@ -248,48 +246,28 @@
         self._handle_response: Callable = None
         self.threads: List[Thread] = []
         self.counter: int = 0
         self.ids: Dict[str, Dict[int, Callable]] = defaultdict(
             lambda: defaultdict(lambda: lambda *x, **y: None)
         )
 
-    if is_windows:
-
-        def sniff(self) -> None:
-            """
-            This function starts sniffer.
-            """
-
-            for iface, _ in self.my_ips.values():
-                sniffer = AsyncSniffer(
-                    filter=(
-                        "proto UDP and (port 137 or port 5355"
-                        " or port 5353 or port 53)"
-                    ),
-                    timeout=self.timeout,
-                    prn=self.redirect,
-                    iface=iface,  # all interfaces
-                )
-                sniffer.start()
-
-    else:
-
-        def sniff(self) -> None:
-            """
-            This function starts sniffer.
-            """
+    def sniff(self) -> None:
+        """
+        This function starts sniffer.
+        """
 
-            sniffer = self.sniffer = AsyncSniffer(
+        for iface, _ in self.my_ips.values():
+            sniffer = AsyncSniffer(
                 filter=(
                     "proto UDP and (port 137 or port 5355"
                     " or port 5353 or port 53)"
                 ),
                 timeout=self.timeout,
                 prn=self.redirect,
-                iface=None,  # all interfaces
+                iface=iface,  # all interfaces
             )
             sniffer.start()
 
     def redirect(self, packet: Packet) -> None:
         """
         This function calls callbacks for sniffed packets.
         """
```

### Comparing `LocalResolver-1.0.0/PKG-INFO` & `LocalResolver-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LocalResolver
-Version: 1.0.0
+Version: 1.0.1
 Summary: This package implements local hostname resolver tool with scapy.
 Home-page: https://github.com/mauricelambert/LocalResolver
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
@@ -31,14 +31,22 @@
 
 # LocalResolver
 
 ## Description
 
 This package implements local hostname resolver tool with scapy (using netbios and LLMNR query).
 
+This tool is useful to:
+ - reverse lookup local IP addresses
+ - resolve manually hostnames/IP from Linux or hardened Windows
+ - resolve hostname with old machines (Windows 2000-2012)
+ - identify:
+     - Machines with old protocols like Netbios or LLMNR,
+     - Hostname spoofer (or two machines with the same name),
+
 ## Requirements
 
 This package require: 
 
  - python3
  - python3 Standard Library
  - Scapy
```

### Comparing `LocalResolver-1.0.0/README.md` & `LocalResolver-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 # LocalResolver
 
 ## Description
 
 This package implements local hostname resolver tool with scapy (using netbios and LLMNR query).
 
+This tool is useful to:
+ - reverse lookup local IP addresses
+ - resolve manually hostnames/IP from Linux or hardened Windows
+ - resolve hostname with old machines (Windows 2000-2012)
+ - identify:
+     - Machines with old protocols like Netbios or LLMNR,
+     - Hostname spoofer (or two machines with the same name),
+
 ## Requirements
 
 This package require: 
 
  - python3
  - python3 Standard Library
  - Scapy
```

### Comparing `LocalResolver-1.0.0/setup.py` & `LocalResolver-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="LocalResolver",
-    version="1.0.0",
+    version="1.0.1",
     py_modules=["LocalResolver"],
     install_requires=["scapy", "PythonToolsKit"],
     author="Maurice Lambert",
     author_email="mauricelambert434@gmail.com",
     maintainer="Maurice Lambert",
     maintainer_email="mauricelambert434@gmail.com",
     description="This package implements local hostname resolver tool with scapy.",
```

