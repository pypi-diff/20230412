# Comparing `tmp/bible_alignments-0.2.2.tar.gz` & `tmp/bible_alignments-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bible_alignments-0.2.2.tar", max compression
+gzip compressed data, was "bible_alignments-0.2.3.tar", max compression
```

## Comparing `bible_alignments-0.2.2.tar` & `bible_alignments-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    20131 2023-02-22 04:20:29.147219 bible_alignments-0.2.2/LICENSE
--rw-r--r--   0        0        0      900 2023-03-01 18:19:16.168100 bible_alignments-0.2.2/README.md
--rw-r--r--   0        0        0     1706 2023-04-12 01:03:41.258550 bible_alignments-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      554 2023-02-22 04:20:29.528825 bible_alignments-0.2.2/src/.github/actions/run-checks/action.yml
--rw-r--r--   0        0        0     2033 2023-02-22 04:20:29.529037 bible_alignments-0.2.2/src/.github/actions/setup-poetry-env/action.yml
--rw-r--r--   0        0        0      975 2023-02-22 04:20:29.529246 bible_alignments-0.2.2/src/.github/workflows/on-merge-to-main.yml
--rw-r--r--   0        0        0      949 2023-02-22 04:20:29.529365 bible_alignments-0.2.2/src/.github/workflows/on-pull-request.yml
--rw-r--r--   0        0        0     1964 2023-02-22 04:20:29.529486 bible_alignments-0.2.2/src/.github/workflows/on-release-main.yml
--rw-r--r--   0        0        0      351 2023-02-22 04:20:29.529608 bible_alignments-0.2.2/src/.github/workflows/validate-codecov-config.yml
--rw-r--r--   0        0        0    16557 2023-02-28 20:36:24.715176 bible_alignments-0.2.2/src/01-Exploration.ipynb
--rw-r--r--   0        0        0        0 2023-02-24 04:25:37.140718 bible_alignments-0.2.2/src/__init__.py
--rw-r--r--   0        0        0     4810 2023-03-16 20:46:04.251808 bible_alignments-0.2.2/src/catalog.py
--rw-r--r--   0        0        0      247 2023-02-24 04:25:33.130530 bible_alignments-0.2.2/src/config.py
--rw-r--r--   0        0        0        0 2023-02-22 04:20:29.529807 bible_alignments-0.2.2/src/format/__init__.py
--rw-r--r--   0        0        0     5829 2023-02-22 04:20:29.529962 bible_alignments-0.2.2/src/format/grapecity.py
--rw-r--r--   0        0        0     1992 2023-03-29 23:00:01.348555 bible_alignments-0.2.2/src/gcsource.py
--rw-r--r--   0        0        0     2184 2023-03-01 17:24:10.055644 bible_alignments-0.2.2/src/gctarget.py
--rw-r--r--   0        0        0     4306 2023-02-28 18:53:54.606669 bible_alignments-0.2.2/src/grapecity.py
--rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 bible_alignments-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    20131 2023-02-22 04:20:29.147219 bible_alignments-0.2.3/LICENSE
+-rw-r--r--   0        0        0      900 2023-03-01 18:19:16.168100 bible_alignments-0.2.3/README.md
+-rw-r--r--   0        0        0     1706 2023-04-12 01:53:22.142719 bible_alignments-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      554 2023-02-22 04:20:29.528825 bible_alignments-0.2.3/src/.github/actions/run-checks/action.yml
+-rw-r--r--   0        0        0     2033 2023-02-22 04:20:29.529037 bible_alignments-0.2.3/src/.github/actions/setup-poetry-env/action.yml
+-rw-r--r--   0        0        0      975 2023-02-22 04:20:29.529246 bible_alignments-0.2.3/src/.github/workflows/on-merge-to-main.yml
+-rw-r--r--   0        0        0      949 2023-02-22 04:20:29.529365 bible_alignments-0.2.3/src/.github/workflows/on-pull-request.yml
+-rw-r--r--   0        0        0     1964 2023-02-22 04:20:29.529486 bible_alignments-0.2.3/src/.github/workflows/on-release-main.yml
+-rw-r--r--   0        0        0      351 2023-02-22 04:20:29.529608 bible_alignments-0.2.3/src/.github/workflows/validate-codecov-config.yml
+-rw-r--r--   0        0        0    16557 2023-02-28 20:36:24.715176 bible_alignments-0.2.3/src/01-Exploration.ipynb
+-rw-r--r--   0        0        0        0 2023-02-24 04:25:37.140718 bible_alignments-0.2.3/src/__init__.py
+-rw-r--r--   0        0        0     4810 2023-03-16 20:46:04.251808 bible_alignments-0.2.3/src/catalog.py
+-rw-r--r--   0        0        0      247 2023-02-24 04:25:33.130530 bible_alignments-0.2.3/src/config.py
+-rw-r--r--   0        0        0        0 2023-02-22 04:20:29.529807 bible_alignments-0.2.3/src/format/__init__.py
+-rw-r--r--   0        0        0     5829 2023-02-22 04:20:29.529962 bible_alignments-0.2.3/src/format/grapecity.py
+-rw-r--r--   0        0        0     2134 2023-04-12 01:30:26.702956 bible_alignments-0.2.3/src/gcsource.py
+-rw-r--r--   0        0        0     2193 2023-04-12 01:30:54.463180 bible_alignments-0.2.3/src/gctarget.py
+-rw-r--r--   0        0        0     4268 2023-04-12 01:39:06.347815 bible_alignments-0.2.3/src/grapecity.py
+-rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 bible_alignments-0.2.3/PKG-INFO
```

### Comparing `bible_alignments-0.2.2/LICENSE` & `bible_alignments-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.2/README.md` & `bible_alignments-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.2/pyproject.toml` & `bible_alignments-0.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bible-alignments"
-version = "0.2.2"
+version = "0.2.3"
 description = "Word-level alignments for Bibles, including both automatic alignments and manually corrected alignments."
 authors = ["Sean Boisen <sean.boisen@clear.bible>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["Bible", "alignment", "Bible alignment"]
 repository = "https://github.com/Clear-Bible/bible-alignments"
 #documentation = "https://sboisen.github.io/alignments/"
```

### Comparing `bible_alignments-0.2.2/src/.github/actions/run-checks/action.yml` & `bible_alignments-0.2.3/src/.github/actions/run-checks/action.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.2/src/.github/actions/setup-poetry-env/action.yml` & `bible_alignments-0.2.3/src/.github/actions/setup-poetry-env/action.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.2/src/.github/workflows/on-merge-to-main.yml` & `bible_alignments-0.2.3/src/.github/workflows/on-merge-to-main.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.2/src/.github/workflows/on-pull-request.yml` & `bible_alignments-0.2.3/src/.github/workflows/on-pull-request.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.2/src/.github/workflows/on-release-main.yml` & `bible_alignments-0.2.3/src/.github/workflows/on-release-main.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.2/src/01-Exploration.ipynb` & `bible_alignments-0.2.3/src/01-Exploration.ipynb`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.2/src/catalog.py` & `bible_alignments-0.2.3/src/catalog.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.2/src/format/grapecity.py` & `bible_alignments-0.2.3/src/format/grapecity.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.2/src/gcsource.py` & `bible_alignments-0.2.3/src/gcsource.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-"""Manage the source data for Grape City (gc) alignments."""
+"""Manage the source data for Grape City (gc) alignments.
+
+>>> from src import gcsource
+# read NA/27 GNT data for the LEB alignment
+>>> rd = gcsource.Reader(sourceid="NA27", targetid="LEB")
+"""
 
 from collections import UserDict
 from csv import DictReader
 from dataclasses import dataclass
 
-import config
+from src import config
 
 # these attribute names match the source data for simplicity
 
 
 @dataclass
 class Source:
     """Manage source data for a word/morph."""
```

### Comparing `bible_alignments-0.2.2/src/gctarget.py` & `bible_alignments-0.2.3/src/gctarget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Manage the target data for Grape City (gc) alignments."""
 
 from collections import UserDict
 from csv import DictReader
 from dataclasses import dataclass
 
-import config
+from src import config
 
 # these attribute names match the source data for simplicity
 
 
 @dataclass
 class Target:
     """Manage target data for a word."""
```

### Comparing `bible_alignments-0.2.2/src/grapecity.py` & `bible_alignments-0.2.3/src/grapecity.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 minor differences from authoritative editions.
 
 """
 
 from collections import UserDict
 from dataclasses import dataclass, field
 import json
-from pathlib import Path
 from typing import Union
-import tomli
 
 from src import config, gcsource, gctarget
 
 # from . import config, gcsource, gctarget
 
 # type that's either None (undefined) or a float. This allows 0.0 as a
 # declared value.
```

### Comparing `bible_alignments-0.2.2/PKG-INFO` & `bible_alignments-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bible-alignments
-Version: 0.2.2
+Version: 0.2.3
 Summary: Word-level alignments for Bibles, including both automatic alignments and manually corrected alignments.
 Home-page: https://github.com/Clear-Bible/bible-alignments
 License: MIT
 Keywords: Bible,alignment,Bible alignment
 Author: Sean Boisen
 Author-email: sean.boisen@clear.bible
 Requires-Python: >=3.10,<4.0
```

