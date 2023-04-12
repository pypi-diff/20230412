# Comparing `tmp/dissect.shellitem-3.4.dev2.tar.gz` & `tmp/dissect.shellitem-3.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.shellitem-3.4.dev2.tar", last modified: Thu Mar 16 13:04:37 2023, max compression
+gzip compressed data, was "dissect.shellitem-3.5.dev1.tar", last modified: Tue Apr 11 17:44:53 2023, max compression
```

## Comparing `dissect.shellitem-3.4.dev2.tar` & `dissect.shellitem-3.5.dev1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:37.839378 dissect.shellitem-3.4.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-16 13:04:37.839378 dissect.shellitem-3.4.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:37.835378 dissect.shellitem-3.4.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:37.835378 dissect.shellitem-3.4.dev2/dissect/shellitem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/dissect/shellitem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:37.839378 dissect.shellitem-3.4.dev2/dissect/shellitem/lnk/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/dissect/shellitem/lnk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/dissect/shellitem/lnk/c_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)    17444 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/dissect/shellitem/lnk/lnk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:37.839378 dissect.shellitem-3.4.dev2/dissect/shellitem/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/dissect/shellitem/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/dissect/shellitem/tools/lnk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:37.835378 dissect.shellitem-3.4.dev2/dissect.shellitem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-16 13:04:37.000000 dissect.shellitem-3.4.dev2/dissect.shellitem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-16 13:04:37.000000 dissect.shellitem-3.4.dev2/dissect.shellitem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:04:37.000000 dissect.shellitem-3.4.dev2/dissect.shellitem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-16 13:04:37.000000 dissect.shellitem-3.4.dev2/dissect.shellitem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-16 13:04:37.000000 dissect.shellitem-3.4.dev2/dissect.shellitem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:04:37.000000 dissect.shellitem-3.4.dev2/dissect.shellitem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-16 13:04:27.000000 dissect.shellitem-3.4.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 13:04:37.839378 dissect.shellitem-3.4.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:37.839378 dissect.shellitem-3.4.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:04:37.839378 dissect.shellitem-3.4.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/tests/data/downloads.win81.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/tests/data/local.directory.seven.lnk
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/tests/data/remote.directory.xp.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/tests/data/remote.file.xp.lnk
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/tests/test_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-16 13:04:21.000000 dissect.shellitem-3.4.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/dissect/shellitem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/dissect/shellitem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/dissect/shellitem/lnk/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/dissect/shellitem/lnk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/dissect/shellitem/lnk/c_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17346 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/dissect/shellitem/lnk/lnk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/dissect/shellitem/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/dissect/shellitem/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/dissect/shellitem/tools/lnk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-11 17:44:53.000000 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-11 17:44:53.000000 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:44:53.000000 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 17:44:53.000000 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 17:44:53.000000 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 17:44:53.000000 dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-11 17:44:43.000000 dissect.shellitem-3.5.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:53.203187 dissect.shellitem-3.5.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/data/downloads.win81.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/data/local.directory.seven.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/data/remote.directory.xp.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/data/remote.file.xp.lnk
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tests/test_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-11 17:44:39.000000 dissect.shellitem-3.5.dev1/tox.ini
```

### Comparing `dissect.shellitem-3.4.dev2/LICENSE` & `dissect.shellitem-3.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.4.dev2/PKG-INFO` & `dissect.shellitem-3.5.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.shellitem
-Version: 3.4.dev2
+Version: 3.5.dev1
 Summary: A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.shellitem
 Project-URL: repository, https://github.com/fox-it/dissect.shellitem
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.shellitem-3.4.dev2/README.md` & `dissect.shellitem-3.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.4.dev2/dissect/shellitem/lnk/c_lnk.py` & `dissect.shellitem-3.5.dev1/dissect/shellitem/lnk/c_lnk.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.4.dev2/dissect/shellitem/lnk/lnk.py` & `dissect.shellitem-3.5.dev1/dissect/shellitem/lnk/lnk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
-from io import BytesIO
-from pathlib import Path
+from io import BufferedReader, BytesIO
 from struct import unpack
-from typing import Any, BinaryIO, Optional, Union
+from typing import Any, BinaryIO, Optional
 from uuid import UUID
 
 from dissect.util.stream import RangeStream
 
 from dissect.shellitem.lnk.c_lnk import (
     EXTRA_DATA_BLOCK_SIGNATURES,
     LINK_EXTRA_DATA_HEADER_SIZE,
@@ -364,24 +363,21 @@
         linkinfo: A LnkInfo object.
         stringdata: A LnkStringData object.
         extradata: A LnkExtraData object.
     """
 
     def __init__(
         self,
-        path: Union[str, Path],
+        fh: BufferedReader,
         target_idlist: Optional[LnkTargetIdList] = None,
         linkinfo: Optional[LnkInfo] = None,
         stringdata: Optional[LnkStringData] = None,
         extradata: Optional[LnkExtraData] = None,
     ):
-        if isinstance(path, str):
-            path = Path(path)
-
-        self.fh = path.open("rb")
+        self.fh = fh
 
         self.flags = None
         self.link_header = self._parse_header(self.fh)
         self.target_idlist = LnkTargetIdList()
         self.linkinfo = LnkInfo()
         self.stringdata = LnkStringData()
         self.extradata = LnkExtraData()
```

### Comparing `dissect.shellitem-3.4.dev2/dissect/shellitem/tools/lnk.py` & `dissect.shellitem-3.5.dev1/dissect/shellitem/tools/lnk.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 log = logging.getLogger(__name__)
 logging.lastResort = None
 logging.raiseExceptions = False
 
 
 def parse(path: Path):
-    lnk_file = Lnk(path)
+    lnk_file = Lnk(path.open("rb"))
     lnk_net_name = lnk_device_name = None
 
     if lnk_file.link_header:
         lnk_path = path
         lnk_name = lnk_file.stringdata.name_string.string if lnk_file.flag("has_name") else None
 
         lnk_mtime = ts.from_unix(path.stat().st_mtime)
```

### Comparing `dissect.shellitem-3.4.dev2/dissect.shellitem.egg-info/PKG-INFO` & `dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.shellitem
-Version: 3.4.dev2
+Version: 3.5.dev1
 Summary: A Dissect module implementing a parser for the Shellitem structures, commonly used by Microsoft Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.shellitem
 Project-URL: repository, https://github.com/fox-it/dissect.shellitem
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.shellitem-3.4.dev2/dissect.shellitem.egg-info/SOURCES.txt` & `dissect.shellitem-3.5.dev1/dissect.shellitem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.4.dev2/pyproject.toml` & `dissect.shellitem-3.5.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.4.dev2/tests/conftest.py` & `dissect.shellitem-3.5.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.4.dev2/tests/data/downloads.win81.lnk` & `dissect.shellitem-3.5.dev1/tests/data/downloads.win81.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.4.dev2/tests/data/local.directory.seven.lnk` & `dissect.shellitem-3.5.dev1/tests/data/local.directory.seven.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.4.dev2/tests/data/remote.directory.xp.lnk` & `dissect.shellitem-3.5.dev1/tests/data/remote.directory.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.4.dev2/tests/data/remote.file.xp.lnk` & `dissect.shellitem-3.5.dev1/tests/data/remote.file.xp.lnk`

 * *Files identical despite different names*

### Comparing `dissect.shellitem-3.4.dev2/tests/test_lnk.py` & `dissect.shellitem-3.5.dev1/tests/test_lnk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dissect.util.ts import uuid1timestamp
 
 from dissect.shellitem.lnk import Lnk, c_lnk
 
 
 def test_xp_remote_lnk_file(xp_remote_lnk_file):
-    lnk_file = Lnk(xp_remote_lnk_file)
+    fh = xp_remote_lnk_file.open("rb")
+    lnk_file = Lnk(fh)
 
     assert lnk_file.link_header.header_size == 0x4C
     assert str(lnk_file.clsid) == "00021401-0000-0000-c000-000000000046"
 
     flags = lnk_file.flags
 
     assert flags & c_lnk.LINK_FLAGS.has_link_target_idlist
@@ -53,15 +54,17 @@
     assert tracker_props.machine_id == b"als-fichiers3\x00\x00\x00"
     assert str(tracker_props.file_droid) == "ea461b34-9877-11da-80bd-000f1ff7c0dc"
     assert str(tracker_props.file_droid_birth) == "ea461b34-9877-11da-80bd-000f1ff7c0dc"
     assert uuid1timestamp(tracker_props.file_droid.time).ctime() == "Wed Feb  8 07:52:55 2006"
 
 
 def test_xp_remote_lnk_dir(xp_remote_lnk_dir):
-    lnk_file = Lnk(xp_remote_lnk_dir)
+    fh = xp_remote_lnk_dir.open("rb")
+    lnk_file = Lnk(fh)
+
     assert lnk_file.link_header.header_size == 0x4C
     assert str(lnk_file.clsid) == "00021401-0000-0000-c000-000000000046"
 
     flags = lnk_file.flags
 
     assert flags & c_lnk.LINK_FLAGS.has_link_target_idlist
     idlist = lnk_file.target_idlist.idlist
@@ -99,15 +102,16 @@
     assert tracker_props.machine_id == b"als-fichiers3\x00\x00\x00"
     assert str(tracker_props.file_droid) == "8ab7e0c5-75c8-11de-b8c9-000f1ff7c0dd"
     assert str(tracker_props.file_droid_birth) == "8ab7e0c5-75c8-11de-b8c9-000f1ff7c0dd"
     assert uuid1timestamp(tracker_props.file_droid.time).ctime() == "Tue Jul 21 07:31:44 2009"
 
 
 def test_win7_local_lnk_dir(win7_local_lnk_dir):
-    lnk_file = Lnk(win7_local_lnk_dir)
+    fh = win7_local_lnk_dir.open("rb")
+    lnk_file = Lnk(fh)
 
     assert lnk_file.link_header.header_size == 0x4C
     assert str(lnk_file.clsid) == "00021401-0000-0000-c000-000000000046"
 
     flags = lnk_file.flags
 
     assert flags & c_lnk.LINK_FLAGS.has_link_target_idlist
@@ -161,15 +165,16 @@
     property_store_props = lnk_file.extradata.extradata["PROPERTY_STORE_PROPS"]
     assert property_store_props.storage_size == 0xAC
     assert property_store_props.version == 0x53505331
     assert str(property_store_props.format_id) == "b725f130-47ef-101a-a5f1-02608c9eebac"
 
 
 def test_common_path_suffix(win81_downloads_lnk_dir):
-    downloads = Lnk(win81_downloads_lnk_dir)
+    fh = win81_downloads_lnk_dir.open("rb")
+    downloads = Lnk(fh)
 
     link_info = downloads.linkinfo.link_info
     link_info_flags = link_info.link_info_flags
     # edge-case were common_network_relative_link_and_pathsuffix indicates no common_path_suffix
     # but when reality says otherwise.
     assert link_info_flags & c_lnk.LINK_INFO_FLAGS.common_network_relative_link_and_pathsuffix == 0
     assert link_info.common_path_suffix == b""
```

### Comparing `dissect.shellitem-3.4.dev2/tox.ini` & `dissect.shellitem-3.5.dev1/tox.ini`

 * *Files identical despite different names*

