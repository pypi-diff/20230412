# Comparing `tmp/cochleogram-0.1.6.tar.gz` & `tmp/cochleogram-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochleogram-0.1.6.tar", last modified: Wed Mar 22 17:56:06 2023, max compression
+gzip compressed data, was "cochleogram-0.1.7.tar", last modified: Wed Apr 12 16:25:11 2023, max compression
```

## Comparing `cochleogram-0.1.6.tar` & `cochleogram-0.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:56:06.472419 cochleogram-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:56:06.468419 cochleogram-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:56:06.468419 cochleogram-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-22 17:55:54.000000 cochleogram-0.1.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-03-22 17:55:54.000000 cochleogram-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-03-22 17:56:06.472419 cochleogram-0.1.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:56:06.472419 cochleogram-0.1.6/cochleogram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18043 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/gui.enaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:56:06.472419 cochleogram-0.1.6/cochleogram/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/icons/cells.png
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/icons/exclude.png
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/icons/main-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/icons/make_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/icons/spiral.png
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/icons/tile.png
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/presenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-03-22 17:55:54.000000 cochleogram-0.1.6/cochleogram/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-22 17:56:06.000000 cochleogram-0.1.6/cochleogram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:56:06.472419 cochleogram-0.1.6/cochleogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-03-22 17:56:06.000000 cochleogram-0.1.6/cochleogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-22 17:56:06.000000 cochleogram-0.1.6/cochleogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 17:56:06.000000 cochleogram-0.1.6/cochleogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-22 17:56:06.000000 cochleogram-0.1.6/cochleogram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-22 17:56:06.000000 cochleogram-0.1.6/cochleogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-22 17:56:06.000000 cochleogram-0.1.6/cochleogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-22 17:55:54.000000 cochleogram-0.1.6/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-22 17:55:54.000000 cochleogram-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-03-22 17:55:54.000000 cochleogram-0.1.6/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 17:56:06.472419 cochleogram-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:25:11.276329 cochleogram-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:25:11.272329 cochleogram-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:25:11.272329 cochleogram-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-12 16:24:59.000000 cochleogram-0.1.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-12 16:24:59.000000 cochleogram-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-12 16:25:11.276329 cochleogram-0.1.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:25:11.272329 cochleogram-0.1.7/cochleogram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/gui.enaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:25:11.276329 cochleogram-0.1.7/cochleogram/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/cells.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/exclude.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/main-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/make_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/spiral.png
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/tile.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:25:11.276329 cochleogram-0.1.7/cochleogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 16:24:59.000000 cochleogram-0.1.7/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-12 16:24:59.000000 cochleogram-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-12 16:24:59.000000 cochleogram-0.1.7/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:25:11.276329 cochleogram-0.1.7/setup.cfg
```

### Comparing `cochleogram-0.1.6/.github/workflows/publish-to-pypi.yml` & `cochleogram-0.1.7/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/.gitignore` & `cochleogram-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/PKG-INFO` & `cochleogram-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.1.6
+Version: 0.1.7
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.1.6/cochleogram/gui.enaml` & `cochleogram-0.1.7/cochleogram/gui.enaml`

 * *Files 1% similar despite different names*

```diff
@@ -402,24 +402,34 @@
             title = '&File'
             Action:
                 text = 'Open processed dataset\tCtrl+O'
                 triggered ::
                     open_processed_dataset(window)
 
             Action:
-                text = 'Process LIF file\tCtrl+P'
+                text = 'Process 20x LIF file\tCtrl+P'
                 triggered ::
                     path = FileDialogEx.get_open_file_name(window, current_path=window.current_path)
                     if path:
                         pp = ProgressWindow()
                         pp.show()
                         cb = lambda x, pp=pp: setattr(pp, 'progress', x)
                         deferred_call(util.process_lif, path, reprocess=True, cb=cb)
 
             Action:
+                text = 'Process 63x LIF file\tCtrl+P'
+                triggered ::
+                    path = FileDialogEx.get_open_file_name(window, current_path=window.current_path)
+                    if path:
+                        pp = ProgressWindow()
+                        pp.show()
+                        cb = lambda x, pp=pp: setattr(pp, 'progress', x)
+                        deferred_call(util.lif_to_ims, path, reprocess=True, cb=cb)
+
+            Action:
                 text = 'Save analysis\tCtrl+S'
                 triggered ::
                     save_state(window, window.presenters)
 
             Action:
                 text = 'Load analysis\tCtrl+L'
                 triggered ::
```

### Comparing `cochleogram-0.1.6/cochleogram/icons/cells.png` & `cochleogram-0.1.7/cochleogram/icons/cells.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/cochleogram/icons/exclude.png` & `cochleogram-0.1.7/cochleogram/icons/exclude.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/cochleogram/icons/main-icon.png` & `cochleogram-0.1.7/cochleogram/icons/main-icon.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/cochleogram/icons/make_icons.py` & `cochleogram-0.1.7/cochleogram/icons/make_icons.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/cochleogram/icons/spiral.png` & `cochleogram-0.1.7/cochleogram/icons/spiral.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/cochleogram/icons/tile.png` & `cochleogram-0.1.7/cochleogram/icons/tile.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/cochleogram/instructions.html` & `cochleogram-0.1.7/cochleogram/instructions.html`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/cochleogram/main.py` & `cochleogram-0.1.7/cochleogram/main.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/cochleogram/model.py` & `cochleogram-0.1.7/cochleogram/model.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/cochleogram/plot.py` & `cochleogram-0.1.7/cochleogram/plot.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/cochleogram/presenter.py` & `cochleogram-0.1.7/cochleogram/presenter.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/cochleogram/util.py` & `cochleogram-0.1.7/cochleogram/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from importlib.metadata import version
 import json
 import re
 from pathlib import Path
 import pickle
+import subprocess
 
 from matplotlib import path as mpath
 import numpy as np
 import pandas as pd
 from scipy import ndimage, optimize, signal
 
 
@@ -403,7 +404,28 @@
     '''
     xo, yo = arc_origin(x, y)
     angles = np.unwrap(np.arctan2(y-yo, x-xo))
     sign = np.sign(np.diff(angles))
     if np.any(sign != sign[0]):
         raise ValueError('Cannot determine direction of arc')
     return sign[0]
+
+
+def _find_ims_converter():
+    path = Path(r'C:\Program Files\Bitplane')
+    return str(next(path.glob('**/ImarisConvert.exe')))
+
+
+def lif_to_ims(filename, reprocess=False, cb=None):
+    filename = Path(filename)
+    converter = _find_ims_converter()
+    if cb is None:
+        cb = lambda x: x
+    stacks = [(i, s) for i, s in enumerate(list_lif_stacks(filename)) if s.startswith('IHC')]
+    n_stacks = len(stacks)
+    for j, (ii, stack_name) in enumerate(stacks):
+        outfile = filename.parent / filename.stem / f'{filename.stem}_{stack_name}.ims'
+        outfile.parent.mkdir(exist_ok=True, parents=True)
+        args = [converter, '-i', str(filename), '-ii', str(ii), '-o', str(outfile)]
+        subprocess.check_output(args)
+        progress = int((j + 1) / n_stacks * 100)
+        cb(progress)
```

### Comparing `cochleogram-0.1.6/cochleogram.egg-info/PKG-INFO` & `cochleogram-0.1.7/cochleogram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.1.6
+Version: 0.1.7
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.1.6/cochleogram.egg-info/SOURCES.txt` & `cochleogram-0.1.7/cochleogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/pyproject.toml` & `cochleogram-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.6/readme.rst` & `cochleogram-0.1.7/readme.rst`

 * *Files identical despite different names*

