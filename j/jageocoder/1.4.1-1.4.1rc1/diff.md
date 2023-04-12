# Comparing `tmp/jageocoder-1.4.1.tar.gz` & `tmp/jageocoder-1.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jageocoder-1.4.1.tar", max compression
+gzip compressed data, was "jageocoder-1.4.1rc1.tar", max compression
```

## Comparing `jageocoder-1.4.1.tar` & `jageocoder-1.4.1rc1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0      113 2022-12-31 11:33:15.983839 jageocoder-1.4.1/LICENSE
--rw-r--r--   0        0        0    11683 2023-03-11 02:17:26.824886 jageocoder-1.4.1/README.md
--rw-r--r--   0        0        0     1362 2023-04-12 00:30:42.254389 jageocoder-1.4.1/jageocoder/__init__.py
--rw-r--r--   0        0        0     5792 2023-04-11 18:53:18.498307 jageocoder-1.4.1/jageocoder/__main__.py
--rw-r--r--   0        0        0     2574 2022-12-31 11:33:15.993839 jageocoder-1.4.1/jageocoder/address.py
--rw-r--r--   0        0        0    12277 2023-04-11 18:53:13.918307 jageocoder-1.4.1/jageocoder/aza_master.py
--rw-r--r--   0        0        0      339 2023-04-11 18:53:13.918307 jageocoder-1.4.1/jageocoder/base.py
--rw-r--r--   0        0        0      676 2023-04-11 18:53:13.918307 jageocoder-1.4.1/jageocoder/dataset.py
--rw-r--r--   0        0        0      691 2022-12-31 11:33:15.993839 jageocoder-1.4.1/jageocoder/exceptions.py
--rw-r--r--   0        0        0    18862 2023-04-11 18:53:18.498307 jageocoder-1.4.1/jageocoder/itaiji.py
--rw-r--r--   0        0        0    14220 2022-12-31 11:33:15.993839 jageocoder-1.4.1/jageocoder/itaiji_dic.json
--rw-r--r--   0        0        0    12242 2023-04-11 18:53:18.498307 jageocoder-1.4.1/jageocoder/module.py
--rw-r--r--   0        0        0    29242 2023-04-12 00:23:43.894432 jageocoder-1.4.1/jageocoder/node.py
--rw-r--r--   0        0        0      991 2023-04-11 18:53:13.918307 jageocoder-1.4.1/jageocoder/note.py
--rw-r--r--   0        0        0     2643 2023-04-11 18:53:18.498307 jageocoder-1.4.1/jageocoder/result.py
--rw-r--r--   0        0        0    16746 2023-04-12 00:23:34.204433 jageocoder-1.4.1/jageocoder/rev.py
--rw-r--r--   0        0        0     7854 2022-12-31 11:33:15.993839 jageocoder-1.4.1/jageocoder/strlib.py
--rw-r--r--   0        0        0    51920 2023-04-11 18:53:18.498307 jageocoder-1.4.1/jageocoder/tree.py
--rw-r--r--   0        0        0     5185 2023-04-11 18:53:13.918307 jageocoder-1.4.1/jageocoder/trie.py
--rw-r--r--   0        0        0     1068 2023-04-12 00:30:49.614389 jageocoder-1.4.1/pyproject.toml
--rw-r--r--   0        0        0    13429 1970-01-01 00:00:00.000000 jageocoder-1.4.1/setup.py
--rw-r--r--   0        0        0    13004 1970-01-01 00:00:00.000000 jageocoder-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      113 2023-03-13 04:34:17.970010 jageocoder-1.4.1rc1/LICENSE
+-rw-r--r--   0        0        0    11683 2023-03-13 04:34:17.970010 jageocoder-1.4.1rc1/README.md
+-rw-r--r--   0        0        0     1365 2023-04-07 01:57:33.442274 jageocoder-1.4.1rc1/jageocoder/__init__.py
+-rw-r--r--   0        0        0     5792 2023-04-07 01:40:25.133090 jageocoder-1.4.1rc1/jageocoder/__main__.py
+-rw-r--r--   0        0        0     2574 2023-03-13 04:34:17.974010 jageocoder-1.4.1rc1/jageocoder/address.py
+-rw-r--r--   0        0        0    12277 2023-04-07 01:18:05.462895 jageocoder-1.4.1rc1/jageocoder/aza_master.py
+-rw-r--r--   0        0        0      339 2023-04-07 01:18:05.462895 jageocoder-1.4.1rc1/jageocoder/base.py
+-rw-r--r--   0        0        0      676 2023-04-07 01:18:05.462895 jageocoder-1.4.1rc1/jageocoder/dataset.py
+-rw-r--r--   0        0        0      691 2023-03-13 04:34:17.974010 jageocoder-1.4.1rc1/jageocoder/exceptions.py
+-rw-r--r--   0        0        0    18862 2023-04-07 01:47:15.772927 jageocoder-1.4.1rc1/jageocoder/itaiji.py
+-rw-r--r--   0        0        0    14220 2023-03-13 04:34:17.974010 jageocoder-1.4.1rc1/jageocoder/itaiji_dic.json
+-rw-r--r--   0        0        0    12242 2023-04-07 01:40:58.365275 jageocoder-1.4.1rc1/jageocoder/module.py
+-rw-r--r--   0        0        0    29136 2023-04-07 01:18:05.466894 jageocoder-1.4.1rc1/jageocoder/node.py
+-rw-r--r--   0        0        0      991 2023-04-07 01:18:05.466894 jageocoder-1.4.1rc1/jageocoder/note.py
+-rw-r--r--   0        0        0     2643 2023-04-07 01:49:25.338650 jageocoder-1.4.1rc1/jageocoder/result.py
+-rw-r--r--   0        0        0    16727 2023-04-07 01:55:47.264507 jageocoder-1.4.1rc1/jageocoder/rev.py
+-rw-r--r--   0        0        0     7854 2023-03-13 04:34:17.974010 jageocoder-1.4.1rc1/jageocoder/strlib.py
+-rw-r--r--   0        0        0    51920 2023-04-07 01:46:02.292036 jageocoder-1.4.1rc1/jageocoder/tree.py
+-rw-r--r--   0        0        0     5185 2023-04-07 01:18:05.466894 jageocoder-1.4.1rc1/jageocoder/trie.py
+-rw-r--r--   0        0        0     1071 2023-04-07 01:57:24.862130 jageocoder-1.4.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    13007 1970-01-01 00:00:00.000000 jageocoder-1.4.1rc1/PKG-INFO
```

### Comparing `jageocoder-1.4.1/README.md` & `jageocoder-1.4.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/jageocoder/__init__.py` & `jageocoder-1.4.1rc1/jageocoder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 running the following steps.
 
     >>> import jageocoder
     >>> jageocoder.init()
     >>> jageocoder.searchNode('<Japanese-address>')
 """
 
-__version__ = '1.4.1'  # The package version
+__version__ = '1.4.1rc1'  # The package version
 __dictionary_version__ = '20220519'  # Compatible dictionary version
 __author__ = 'Takeshi Sagara <sagara@info-proto.com>'
 
 __all__ = [
     'init',
     'free',
     'is_initialized',
```

### Comparing `jageocoder-1.4.1/jageocoder/__main__.py` & `jageocoder-1.4.1rc1/jageocoder/__main__.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/jageocoder/address.py` & `jageocoder-1.4.1rc1/jageocoder/address.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/jageocoder/aza_master.py` & `jageocoder-1.4.1rc1/jageocoder/aza_master.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/jageocoder/dataset.py` & `jageocoder-1.4.1rc1/jageocoder/dataset.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/jageocoder/exceptions.py` & `jageocoder-1.4.1rc1/jageocoder/exceptions.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/jageocoder/itaiji.py` & `jageocoder-1.4.1rc1/jageocoder/itaiji.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/jageocoder/itaiji_dic.json` & `jageocoder-1.4.1rc1/jageocoder/itaiji_dic.json`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/jageocoder/module.py` & `jageocoder-1.4.1rc1/jageocoder/module.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/jageocoder/node.py` & `jageocoder-1.4.1rc1/jageocoder/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-from __future__ import annotations
 from functools import lru_cache
 import json
 import logging
 import re
-from typing import List, Optional, TYPE_CHECKING
+from typing import List, Optional
 
 from sqlalchemy import Column, Float, ForeignKey, Integer, SmallInteger, String, Text
 from sqlalchemy import or_
 from sqlalchemy.orm import deferred
 from sqlalchemy.orm import backref, relationship
 
 from jageocoder.address import AddressLevel
 from jageocoder.aza_master import AzaMaster
 from jageocoder.base import Base, get_session
 from jageocoder.dataset import Dataset  #
 from jageocoder.itaiji import Converter
 from jageocoder.result import Result
 from jageocoder.strlib import strlib
 
-if TYPE_CHECKING:
-    from jageocoder.tree import AddressTree
 
 logger = logging.getLogger(__name__)
 default_itaiji_converter = Converter()  # With default settings
 
 
 class AddressNode(Base):
     """
@@ -166,15 +163,15 @@
 
         filtered_children = self.children.filter(*conds).order_by(
             AddressNode.id)
         logger.debug("  -> {} found.".format(filtered_children.count()))
         return filtered_children
 
     def search_recursive(
-        self, index: str, tree: AddressTree,  # noqa
+        self, index: str, tree: 'AddressTree',  # noqa
         processed_nodes: Optional[List['AddressNode']] = None
     ) -> List[Result]:
         """
         Search nodes recursively that match the specified address notation.
 
         Parameters
         ----------
@@ -347,15 +344,15 @@
 
         logger.debug("node:{} returns {}".format(self.name, candidates))
         return candidates
 
     def _get_candidates_from_child(
             self, child: 'AddressNode',
             index: str, optional_prefix: str,
-            tree: AddressTree,  # noqa
+            tree: 'AddressTree',  # noqa
             processed_nodes: List['AddressNode']) -> list:
         """
         Get candidates from the child.
 
         Parameters
         ----------
         child: AddressNode
@@ -422,15 +419,15 @@
                 l_optional_prefix + match_len + cand.nchars))
 
         return candidates
 
     def get_omissible_index(
             self,
             index: str,
-            tree: AddressTree,  # noqa
+            tree: 'AddressTree',  # noqa
             processed_nodes: List['AddressNode']) -> str:
         """
         Obtains an optional leading substring from the search string index.
 
         Parameters
         ----------
         index: str
```

### Comparing `jageocoder-1.4.1/jageocoder/note.py` & `jageocoder-1.4.1rc1/jageocoder/note.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/jageocoder/result.py` & `jageocoder-1.4.1rc1/jageocoder/result.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/jageocoder/rev.py` & `jageocoder-1.4.1rc1/jageocoder/rev.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from logging import getLogger
 import math
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Union
 
 from geographiclib.geodesic import Geodesic
 from sqlalchemy.sql import text
 
 from jageocoder.address import AddressLevel
 from jageocoder.node import AddressNode
 from jageocoder.tree import AddressTree
 
 logger = getLogger(__name__)
 
 
 def p_contained(
-        p: Tuple[float, float],
-        p0: Tuple[float, float],
-        p1: Tuple[float, float],
-        p2: Tuple[float, float]) -> bool:
+        p: List[float, float],
+        p0: List[float, float],
+        p1: List[float, float],
+        p2: List[float, float]) -> bool:
     """
     Determine if the point p is inside the triangle (p0, p1, p2).
 
     Parameters
     ----------
     p: (float, float)
         x and y coordinates of point p.
@@ -47,18 +47,18 @@
     if 0 < s < area and 0 < t < area and 0 < area - s - t < area:
         return True
 
     return False
 
 
 def get_circumcircle(
-    p0: Tuple[float, float],
-    p1: Tuple[float, float],
-    p2: Tuple[float, float]
-) -> Tuple[float, float, float]:
+    p0: List[float, float],
+    p1: List[float, float],
+    p2: List[float, float]
+) -> List[float, float, float]:
     """
     Calculate the coordinates and radius of the circumcircle
     of the triangle (p0, p1, p2).
 
     Parameters
     ----------
     p0, p1, p2: (float, float)
@@ -84,18 +84,18 @@
     x = xt / c
     y = yt / c
     r2 = (x - p0[0]) * (x - p0[0]) + (y - p0[1]) * (y - p0[1])
     return [x, y, r2]
 
 
 def p_contained_circumcircle(
-    p: Tuple[float, float],
-    p0: Tuple[float, float],
-    p1: Tuple[float, float],
-    p2: Tuple[float, float]
+    p: List[float, float],
+    p0: List[float, float],
+    p1: List[float, float],
+    p2: List[float, float]
 ) -> bool:
     """
     Determine if the point p is inside the circumcircle of
     triangle (p0, p1, p2).
 
     Parameters
     ----------
```

### Comparing `jageocoder-1.4.1/jageocoder/strlib.py` & `jageocoder-1.4.1rc1/jageocoder/strlib.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/jageocoder/tree.py` & `jageocoder-1.4.1rc1/jageocoder/tree.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/jageocoder/trie.py` & `jageocoder-1.4.1rc1/jageocoder/trie.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1/pyproject.toml` & `jageocoder-1.4.1rc1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jageocoder"
-version = "1.4.1"
+version = "1.4.1rc1"
 description = "A Japanese-address geocoder for Python."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 repository = "https://github.com/t-sagara/jageocoder/"
 license = "The MIT License"
 readme = "README.md"
 documentation = "https://jageocoder.readthedocs.io/"
 packages = [
```

### Comparing `jageocoder-1.4.1/PKG-INFO` & `jageocoder-1.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jageocoder
-Version: 1.4.1
+Version: 1.4.1rc1
 Summary: A Japanese-address geocoder for Python.
 Home-page: https://github.com/t-sagara/jageocoder/
 License: The MIT License
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

