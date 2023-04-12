# Comparing `tmp/YAMLIndexer-0.1.0.tar.gz` & `tmp/YAMLIndexer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YAMLIndexer-0.1.0.tar", last modified: Fri Mar 25 22:53:12 2022, max compression
+gzip compressed data, was "YAMLIndexer-0.1.1.tar", last modified: Wed Apr 12 14:33:11 2023, max compression
```

## Comparing `YAMLIndexer-0.1.0.tar` & `YAMLIndexer-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 22:53:12.775711 YAMLIndexer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-03-25 22:53:09.000000 YAMLIndexer-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-25 22:53:09.000000 YAMLIndexer-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4713 2022-03-25 22:53:12.775711 YAMLIndexer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3218 2022-03-25 22:53:09.000000 YAMLIndexer-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 22:53:12.775711 YAMLIndexer-0.1.0/YAMLIndexer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4713 2022-03-25 22:53:12.000000 YAMLIndexer-0.1.0/YAMLIndexer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-03-25 22:53:12.000000 YAMLIndexer-0.1.0/YAMLIndexer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-25 22:53:12.000000 YAMLIndexer-0.1.0/YAMLIndexer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-03-25 22:53:12.000000 YAMLIndexer-0.1.0/YAMLIndexer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-25 22:53:12.000000 YAMLIndexer-0.1.0/YAMLIndexer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-25 22:53:12.775711 YAMLIndexer-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-03-25 22:53:09.000000 YAMLIndexer-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-25 22:53:12.775711 YAMLIndexer-0.1.0/yamlindexer/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-03-25 22:53:09.000000 YAMLIndexer-0.1.0/yamlindexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-03-25 22:53:09.000000 YAMLIndexer-0.1.0/yamlindexer/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     4279 2022-03-25 22:53:09.000000 YAMLIndexer-0.1.0/yamlindexer/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-03-25 22:53:09.000000 YAMLIndexer-0.1.0/yamlindexer/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-03-25 22:53:09.000000 YAMLIndexer-0.1.0/yamlindexer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:11.627164 YAMLIndexer-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-12 14:33:09.000000 YAMLIndexer-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:33:09.000000 YAMLIndexer-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-12 14:33:11.627164 YAMLIndexer-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-12 14:33:09.000000 YAMLIndexer-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:11.627164 YAMLIndexer-0.1.1/YAMLIndexer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-12 14:33:11.000000 YAMLIndexer-0.1.1/YAMLIndexer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-12 14:33:11.000000 YAMLIndexer-0.1.1/YAMLIndexer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:33:11.000000 YAMLIndexer-0.1.1/YAMLIndexer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 14:33:11.000000 YAMLIndexer-0.1.1/YAMLIndexer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 14:33:11.000000 YAMLIndexer-0.1.1/YAMLIndexer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:33:11.627164 YAMLIndexer-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-12 14:33:09.000000 YAMLIndexer-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:33:11.627164 YAMLIndexer-0.1.1/yamlindexer/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 14:33:09.000000 YAMLIndexer-0.1.1/yamlindexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-12 14:33:09.000000 YAMLIndexer-0.1.1/yamlindexer/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-12 14:33:09.000000 YAMLIndexer-0.1.1/yamlindexer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-12 14:33:09.000000 YAMLIndexer-0.1.1/yamlindexer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 14:33:09.000000 YAMLIndexer-0.1.1/yamlindexer/version.py
```

### Comparing `YAMLIndexer-0.1.0/LICENSE.txt` & `YAMLIndexer-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `YAMLIndexer-0.1.0/README.md` & `YAMLIndexer-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # YAMLIndexer Module Repository
 
+[![PyPI version](https://img.shields.io/pypi/v/YAMLIndexer.svg?style=flat)](https://pypi.python.org/pypi/YAMLIndexer/)
+[![PyPI downloads](https://img.shields.io/pypi/dm/YAMLIndexer.svg?style=flat)](https://pypi.python.org/pypi/YAMLIndexer/)
 [![example workflow](https://github.com/ruizink/python-yamlindexer/actions/workflows/tests.yaml/badge.svg)](https://github.com/ruizink/python-yamlindexer/actions/workflows/tests.yaml)
 
 Python package to index YAML files for quicker searches
 
 ## Installing
 
 You can install this package using pip.
```

### Comparing `YAMLIndexer-0.1.0/setup.py` & `YAMLIndexer-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `YAMLIndexer-0.1.0/yamlindexer/cache.py` & `YAMLIndexer-0.1.1/yamlindexer/cache.py`

 * *Files identical despite different names*

### Comparing `YAMLIndexer-0.1.0/yamlindexer/core.py` & `YAMLIndexer-0.1.1/yamlindexer/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import os
 import json
-import dpath.util
+import dpath
 from glob import iglob
 from typing import Any, Optional, List, Dict, Set
 try:
     import ryaml
     HAS_RYAML = True
 except ImportError:
     import yaml
@@ -17,18 +17,18 @@
 
 
 class YAMLIndex():
 
     root_path = os.getcwd()
     globs = ['**/*.yml', '**/*.yaml']
     encoding = 'utf-8'
-    index = dict()  # type: Any
+    index: Dict[Any, Any] = dict()
     cache = None
 
-    def __init__(self, root_path: str = None, globs: list = None, cache: Optional[bool] = None,
+    def __init__(self, root_path: Optional[str] = None, globs: Optional[list] = None, cache: Optional[bool] = None,
                  cache_ttl: Optional[int] = None, encoding: Optional[str] = None):
         if root_path is not None:
             self.root_path = root_path
         if globs is not None:
             self.globs = globs
         if encoding is not None:
             self.encoding = encoding
@@ -58,50 +58,50 @@
                 self.cache.load()
             except (FileNotFoundError, yicache.YAMLIndexCacheExpired):
                 self.index = self._index_files()
                 self.cache.save()
 
     def search(self, filter: dict) -> list:
         # TODO: make sure to replace separator if filter_leaf_paths contain /
-        res = list()  # type: List[Set]
+        res: List[Set] = list()
         for f, sep in yiutils.leaf_paths(filter):
             res.append(set(self.search_dpath(f, separator=sep)))
 
         return list(set.intersection(*res))
 
     def search_one_of(self, filters: List[dict], separator: Optional[str] = '/') -> list:
-        res = set()  # type: Set[str]
+        res: Set[str] = set()
         for f in filters:
             res = res.union(set(self.search(f)))
         return list(res)
 
     def search_kv(self, **filters: str) -> list:
         # TODO: rewrite to avoid loops
-        res = set()  # type: Set[str]
+        res: Set[str] = set()
         for k, v in filters.items():
             res = res.union(set(self.index.get(k, {}).get(v, [])))
 
         for k, v in filters.items():
             res = res & set(set(self.index.get(k, {}).get(v, [])))
 
         return list(res)
 
     def search_dpath(self, query, **kwargs) -> list:
-        res = set()  # type: Set[str]
+        res: Set[str] = set()
         dpath.options.ALLOW_EMPTY_STRING_KEYS = True
-        search = dpath.util.values(self.index, query, **kwargs)
+        search = dpath.values(self.index, query, **kwargs)
         for r in search:
             res = res.union(set([x for _, x in dpath.segments.leaves(r)]))
         return list(res)
 
     def _index_files(self) -> dict:
-        files = list()  # type: List[str]
+        files: List[str] = list()
         for g in self.globs:
             files.extend(iglob(os.path.join(self.root_path, g), recursive=True))
-        index = dict()  # type: Dict[str, Dict[str, List[str]]]
+        index: Dict[str, Dict[str, List[str]]] = dict()
         for p in files:
             with open(p, 'r', encoding=self.encoding) as f:
                 if HAS_RYAML:
                     yamlf = ryaml.load(f)
                 else:
                     try:
                         yamlf = yaml.load(f, Loader=yaml.CSafeLoader)
@@ -109,14 +109,16 @@
                         yamlf = yaml.load(f, Loader=yaml.SafeLoader)
                 index = self._push_to_index(yamlf, p, index)
 
         return index
 
     def _push_to_index(self, data: dict, path: str, index=dict()) -> dict:
         # TODO: add tests
+        if type(data) is list:
+            data = {k: v for k, v in enumerate(data)}
         for k, v in data.items():
             if isinstance(v, list):
                 index.setdefault(k, {})
                 index[k] = self._push_to_index({str(i): v[i] for i in range(len(v))}, path, index[k])
             elif isinstance(v, dict):
                 index.setdefault(k, {})
                 index[k] = self._push_to_index(v, path, index[k])
```

### Comparing `YAMLIndexer-0.1.0/yamlindexer/utils.py` & `YAMLIndexer-0.1.1/yamlindexer/utils.py`

 * *Files identical despite different names*

