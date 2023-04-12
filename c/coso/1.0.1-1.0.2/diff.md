# Comparing `tmp/coso-1.0.1.tar.gz` & `tmp/coso-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coso-1.0.1.tar", last modified: Tue Apr 11 09:35:16 2023, max compression
+gzip compressed data, was "coso-1.0.2.tar", last modified: Wed Apr 12 12:21:07 2023, max compression
```

## Comparing `coso-1.0.1.tar` & `coso-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 09:35:16.878400 coso-1.0.1/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2020-09-14 09:37:08.000000 coso-1.0.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-11 09:35:16.877026 coso-1.0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5161 2023-04-11 08:26:28.000000 coso-1.0.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 09:35:16.828971 coso-1.0.1/coso.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-11 09:35:16.000000 coso-1.0.1/coso.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      446 2023-04-11 09:35:16.000000 coso-1.0.1/coso.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-11 09:35:16.000000 coso-1.0.1/coso.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-11 09:35:16.000000 coso-1.0.1/coso.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        4 2023-04-11 09:35:16.000000 coso-1.0.1/coso.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       80 2023-02-06 14:52:53.000000 coso-1.0.1/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-11 09:35:16.878944 coso-1.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      956 2023-04-11 09:34:52.000000 coso-1.0.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 09:35:16.874585 coso-1.0.1/src/
--rwxrwxrwx   0 root         (0) root         (0)    20083 2023-02-03 09:38:17.000000 coso-1.0.1/src/VisCoSo.py
--rwxrwxrwx   0 root         (0) root         (0)     3477 2023-02-03 09:38:26.000000 coso-1.0.1/src/VisCoSo_widget.py
--rwxrwxrwx   0 root         (0) root         (0)      163 2023-02-06 14:36:36.000000 coso-1.0.1/src/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11429 2023-02-03 09:39:45.000000 coso-1.0.1/src/cola_parser.py
--rwxrwxrwx   0 root         (0) root         (0)     8197 2023-02-03 09:36:00.000000 coso-1.0.1/src/configuration.py
--rwxrwxrwx   0 root         (0) root         (0)     6447 2023-02-01 02:28:35.000000 coso-1.0.1/src/count.py
--rwxrwxrwx   0 root         (0) root         (0)    15928 2023-02-03 09:36:18.000000 coso-1.0.1/src/gen_plots.py
--rwxrwxrwx   0 root         (0) root         (0)    12744 2023-02-03 09:36:28.000000 coso-1.0.1/src/level_1.py
--rwxrwxrwx   0 root         (0) root         (0)    13329 2023-02-03 09:36:37.000000 coso-1.0.1/src/level_2.py
--rwxrwxrwx   0 root         (0) root         (0)     8708 2023-02-03 09:36:51.000000 coso-1.0.1/src/logger.py
--rwxrwxrwx   0 root         (0) root         (0)     9606 2023-02-02 16:57:05.000000 coso-1.0.1/src/parsetab.py
--rwxrwxrwx   0 root         (0) root         (0)     9515 2023-02-03 09:37:05.000000 coso-1.0.1/src/problem.py
--rwxrwxrwx   0 root         (0) root         (0)    85377 2023-02-03 09:37:17.000000 coso-1.0.1/src/sharpCSP.py
--rwxrwxrwx   0 root         (0) root         (0)     2986 2023-02-03 09:37:23.000000 coso-1.0.1/src/solver.py
--rwxrwxrwx   0 root         (0) root         (0)    43623 2023-02-03 09:37:43.000000 coso-1.0.1/src/tester.py
--rwxrwxrwx   0 root         (0) root         (0)    14266 2023-01-13 13:24:30.000000 coso-1.0.1/src/util.py
--rwxrwxrwx   0 root         (0) root         (0)     9131 2023-02-03 09:38:05.000000 coso-1.0.1/src/venn.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 12:21:07.188989 coso-1.0.2/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2020-09-14 09:37:08.000000 coso-1.0.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-12 12:21:07.188629 coso-1.0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5161 2023-04-11 08:26:28.000000 coso-1.0.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 12:21:07.173005 coso-1.0.2/coso.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5718 2023-04-12 12:21:07.000000 coso-1.0.2/coso.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      473 2023-04-12 12:21:07.000000 coso-1.0.2/coso.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-12 12:21:07.000000 coso-1.0.2/coso.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       40 2023-04-12 12:21:07.000000 coso-1.0.2/coso.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-04-12 12:21:07.000000 coso-1.0.2/coso.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       80 2023-02-06 14:52:53.000000 coso-1.0.2/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-12 12:21:07.189118 coso-1.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      989 2023-04-12 12:07:28.000000 coso-1.0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 12:21:07.187959 coso-1.0.2/src/
+-rwxrwxrwx   0 root         (0) root         (0)      532 2023-04-12 11:48:32.000000 coso-1.0.2/src/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11429 2023-02-03 09:39:45.000000 coso-1.0.2/src/cola_parser.py
+-rwxrwxrwx   0 root         (0) root         (0)     8197 2023-02-03 09:36:00.000000 coso-1.0.2/src/configuration.py
+-rwxrwxrwx   0 root         (0) root         (0)     6447 2023-02-01 02:28:35.000000 coso-1.0.2/src/count.py
+-rwxrwxrwx   0 root         (0) root         (0)    15930 2023-04-12 10:50:48.000000 coso-1.0.2/src/gen_plots.py
+-rwxrwxrwx   0 root         (0) root         (0)     1739 2023-04-12 12:19:19.000000 coso-1.0.2/src/launcher.py
+-rwxrwxrwx   0 root         (0) root         (0)    12744 2023-02-03 09:36:28.000000 coso-1.0.2/src/level_1.py
+-rwxrwxrwx   0 root         (0) root         (0)    13329 2023-02-03 09:36:37.000000 coso-1.0.2/src/level_2.py
+-rwxrwxrwx   0 root         (0) root         (0)     8708 2023-04-12 10:37:47.000000 coso-1.0.2/src/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     9606 2023-02-02 16:57:05.000000 coso-1.0.2/src/parsetab.py
+-rwxrwxrwx   0 root         (0) root         (0)     9515 2023-02-03 09:37:05.000000 coso-1.0.2/src/problem.py
+-rwxrwxrwx   0 root         (0) root         (0)    85377 2023-02-03 09:37:17.000000 coso-1.0.2/src/sharpCSP.py
+-rwxrwxrwx   0 root         (0) root         (0)     2986 2023-02-03 09:37:23.000000 coso-1.0.2/src/solver.py
+-rwxrwxrwx   0 root         (0) root         (0)    43623 2023-02-03 09:37:43.000000 coso-1.0.2/src/tester.py
+-rwxrwxrwx   0 root         (0) root         (0)    14266 2023-01-13 13:24:30.000000 coso-1.0.2/src/util.py
+-rwxrwxrwx   0 root         (0) root         (0)     9131 2023-02-03 09:38:05.000000 coso-1.0.2/src/venn.py
+-rwxrwxrwx   0 root         (0) root         (0)    20083 2023-02-03 09:38:17.000000 coso-1.0.2/src/viscoso.py
+-rwxrwxrwx   0 root         (0) root         (0)     3477 2023-02-03 09:38:26.000000 coso-1.0.2/src/viscoso_widget.py
```

### Comparing `coso-1.0.1/LICENSE` & `coso-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/PKG-INFO` & `coso-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coso
-Version: 1.0.1
+Version: 1.0.2
 Summary: A solver for combinatorics math word problems.
 Home-page: https://github.com/PietroTotis/CoSo
 Author: Pietro Totis
 Author-email: pietro.totis@kuleuven.be
 License: GNU General Public License (GPL)
 Keywords: combinatorics automated reasoning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coso-1.0.1/README.md` & `coso-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/coso.egg-info/PKG-INFO` & `coso-1.0.2/coso.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coso
-Version: 1.0.1
+Version: 1.0.2
 Summary: A solver for combinatorics math word problems.
 Home-page: https://github.com/PietroTotis/CoSo
 Author: Pietro Totis
 Author-email: pietro.totis@kuleuven.be
 License: GNU General Public License (GPL)
 Keywords: combinatorics automated reasoning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coso-1.0.1/src/VisCoSo.py` & `coso-1.0.2/src/viscoso.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/src/VisCoSo_widget.py` & `coso-1.0.2/src/viscoso_widget.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/src/cola_parser.py` & `coso-1.0.2/src/cola_parser.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/src/configuration.py` & `coso-1.0.2/src/configuration.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/src/count.py` & `coso-1.0.2/src/count.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/src/gen_plots.py` & `coso-1.0.2/src/gen_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import seaborn as sns
 import os
 import pandas
 import matplotlib
 import matplotlib.pyplot as plt
 
-plt.style.use("science")
+# plt.style.use("science")
 
 from .util import ROOT_DIR
 
 OUT_DIR = os.path.join(ROOT_DIR, "tests", "results")
 BENCHMARKS = os.path.join(ROOT_DIR, "tests", "benchmarks", "synthetic")
 COSO_STATS_BENCH = os.path.join(OUT_DIR, "subs_results_benchmarks.csv")
 COSO_STATS_EX = os.path.join(OUT_DIR, "subs_results_examples.csv")
```

### Comparing `coso-1.0.1/src/level_1.py` & `coso-1.0.2/src/level_1.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/src/level_2.py` & `coso-1.0.2/src/level_2.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/src/logger.py` & `coso-1.0.2/src/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import itertools
-from .VisCoSo import VisCoSo
+from .viscoso import VisCoSo
 from .level_1 import Multiset
 from .level_2 import LiftedSet
 from .configuration import CCounting
 from .util import *
 
 
 class ActionLog(object):
```

### Comparing `coso-1.0.1/src/parsetab.py` & `coso-1.0.2/src/parsetab.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/src/problem.py` & `coso-1.0.2/src/problem.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/src/sharpCSP.py` & `coso-1.0.2/src/sharpCSP.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/src/solver.py` & `coso-1.0.2/src/solver.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/src/tester.py` & `coso-1.0.2/src/tester.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/src/util.py` & `coso-1.0.2/src/util.py`

 * *Files identical despite different names*

### Comparing `coso-1.0.1/src/venn.py` & `coso-1.0.2/src/venn.py`

 * *Files identical despite different names*

