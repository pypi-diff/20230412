# Comparing `tmp/bigsort-0.0.6.tar.gz` & `tmp/bigsort-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigsort-0.0.6.tar", last modified: Tue Mar  7 15:30:14 2023, max compression
+gzip compressed data, was "bigsort-0.0.7.tar", last modified: Wed Apr 12 14:41:38 2023, max compression
```

## Comparing `bigsort-0.0.6.tar` & `bigsort-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 15:30:14.098833 bigsort-0.0.6/
--rw-rw-rw-   0        0        0     1310 2023-03-07 15:30:14.096832 bigsort-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-07 15:30:14.095828 bigsort-0.0.6/bigsort.egg-info/
--rw-rw-rw-   0        0        0     1310 2023-03-07 15:30:13.000000 bigsort-0.0.6/bigsort.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-03-07 15:30:14.000000 bigsort-0.0.6/bigsort.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 15:30:13.000000 bigsort-0.0.6/bigsort.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-03-07 15:30:13.000000 bigsort-0.0.6/bigsort.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-03-07 15:30:13.000000 bigsort-0.0.6/bigsort.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-07 15:30:13.000000 bigsort-0.0.6/bigsort.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10954 2023-03-07 15:19:48.000000 bigsort-0.0.6/bigsort.py
--rw-rw-rw-   0        0        0       42 2023-03-07 15:30:14.098833 bigsort-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      993 2023-03-07 15:27:13.000000 bigsort-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:41:38.007960 bigsort-0.0.7/
+-rw-rw-rw-   0        0        0     1310 2023-04-12 14:41:38.007010 bigsort-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 14:41:38.005012 bigsort-0.0.7/bigsort.egg-info/
+-rw-rw-rw-   0        0        0     1310 2023-04-12 14:41:37.000000 bigsort-0.0.7/bigsort.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-04-12 14:41:37.000000 bigsort-0.0.7/bigsort.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:41:37.000000 bigsort-0.0.7/bigsort.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-12 14:41:37.000000 bigsort-0.0.7/bigsort.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-12 14:41:37.000000 bigsort-0.0.7/bigsort.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-12 14:41:37.000000 bigsort-0.0.7/bigsort.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10564 2023-04-12 14:41:27.000000 bigsort-0.0.7/bigsort.py
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:41:38.008215 bigsort-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      993 2023-04-12 14:39:29.000000 bigsort-0.0.7/setup.py
```

### Comparing `bigsort-0.0.6/PKG-INFO` & `bigsort-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigsort
-Version: 0.0.6
+Version: 0.0.7
 Summary: sort big file or streams
 Home-page: https://github.com/laohur/bigsort
 Author: laohur
 Author-email: laohur@gmail.com
 License: [Anti-996 License](https: // github.com/996icu/996.ICU/blob/master/LICENSE)
 Keywords: bigsort,sort,external sort,big file sort
 Requires-Python: >=3.0
```

### Comparing `bigsort-0.0.6/bigsort.egg-info/PKG-INFO` & `bigsort-0.0.7/bigsort.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigsort
-Version: 0.0.6
+Version: 0.0.7
 Summary: sort big file or streams
 Home-page: https://github.com/laohur/bigsort
 Author: laohur
 Author-email: laohur@gmail.com
 License: [Anti-996 License](https: // github.com/996icu/996.ICU/blob/master/LICENSE)
 Keywords: bigsort,sort,external sort,big file sort
 Requires-Python: >=3.0
```

### Comparing `bigsort-0.0.6/bigsort.py` & `bigsort-0.0.7/bigsort.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 import operator
 import sys
 import psutil
 import os
-import bisect
 import argparse
 import random
 import tempfile
 import math
 from multiprocessing import Queue, Process
 
 import logzero
 from logzero import logger
 logzero.loglevel(logzero.INFO)
-# logzero.loglevel(logzero.ERROR)
-
 
 def free():
     available = psutil.virtual_memory().available
     return available
 
-
 def _keyFn(x):
     return x
 
 
 def sortArray(array, sortType, keyFn=_keyFn):
     if sortType == 'R':
         random.shuffle(array)
@@ -43,30 +39,14 @@
         if cmp(keyFn(arr[m]), val):
             l = m
         else:
             r = m
     return r
 
 
-def splitList(queue, sortType, pivot, nSplit, keyFn):
-    if sortType == 'R':
-        random.shuffle(queue)
-    if pivot == None:
-        return queue, []
-    if sortType == 'R':
-        idx = len(queue)//nSplit
-    elif sortType == 'i':
-        idx = bisect(queue, pivot, cmp=lambda x, y: x <= y, keyFn=keyFn)
-    elif sortType == 'd':
-        idx = bisect(queue, pivot, cmp=lambda x, y: x >= y, keyFn=keyFn)
-    lines = queue[:idx]
-    queue = [] if idx == len(queue) else queue[idx:]
-    return lines, queue
-
-
 class Block:
     def __init__(self, path, bucket, sortType, step, buffering, keyFn) -> None:
         self.path = path
         if not os.path.exists(path):
             os.makedirs(path)
         self.n_line = len(bucket)
         bucket = sortArray(bucket, sortType, keyFn)
@@ -161,56 +141,58 @@
         n_read = 0
         n_write = 0
         for i, node in enumerate(Nodes):
             bucket = node.catch()
             queue += bucket
             pivot = Nodes[i+1].head if i != len(Nodes)-1 else None
             queue = sortArray(queue, self.sortType, self.keyFn)
-            lines, queue = splitList(queue, self.sortType, pivot, self.nSplit, self.keyFn)
+            if pivot == None:
+                idx=len(queue)
+            elif self.sortType == 'R':
+                idx = len(queue)//self.nSplit
+            elif self.sortType == 'i':
+                idx = bisect(queue, pivot, cmp=lambda x, y: x <= y, keyFn=self.keyFn)
+            elif self.sortType == 'd':
+                idx = bisect(queue, pivot, cmp=lambda x, y: x >= y, keyFn=self.keyFn)
+
             r1 = len(bucket)
-            w1 = len(lines)
+            w1 =idx
             n_read += r1
             n_write += w1
             logger.info(f"Node:{i}/{len(Nodes)} n_read:{n_read} -- n_write:{n_write} queue:{len(queue)}  r1:{r1} -> w1:{w1}   {r1-w1} ")
-            yield lines
+            for j in range(idx):
+                yield queue[j]
+            queue =  queue[idx:]            
         logger.info(f"reduce done! n_read:{n_read} --> n_write:{n_write} ")
 
-    def outflow(self, reciver):
-        last = None
-        for bucket in reciver:
-            for x in bucket:
-                self.n_readed += 1
-                if self.n_writed >= self.nHead >= 0:
-                    return
-                if self.unique and x == last:
-                    continue
-                last = x
-                self.n_writed += 1
-                yield x
-        logger.info(f" n_readed:{self.n_readed} n_writed:{self.n_writed}")
-
-    def sort(self, reader, tmpDir):
+    def sort(self, reader,writer, tmpDir):
         Nodes = self.map(reader, tmpDir)
 
         Nodes = [(self.keyFn(x.head), self.keyFn(x.tail), i, x) for i, x in enumerate(Nodes)]
         Nodes = sortArray(Nodes, self.sortType, _keyFn)
         Nodes = [x[-1] for x in Nodes]
-
         reciver = self.reduce(Nodes)
-        lines = self.outflow(reciver)
 
-        return lines
+        last = None
+        for x in reciver:
+            self.n_readed += 1
+            if self.n_writed >= self.nHead >= 0:
+                break
+            if self.unique and x == last:
+                continue
+            last = x
+            self.n_writed += 1
+            writer.write(x)
+        logger.info(f" n_readed:{self.n_readed} n_writed:{self.n_writed}")
 
 
 def bigsort(reader, writer, sortType='i', unique=False, keyFn=_keyFn, nHead=-1, budget=0.8, tmpDir=None, nSplit=10, nLine=10000):
     temp_dir = tempfile.TemporaryDirectory(dir=tmpDir)
     sorter = BigSort(sortType=sortType, unique=unique, keyFn=keyFn, nHead=nHead, budget=budget, tmpDir=tmpDir, nSplit=nSplit, nLine=nLine)
-    lines = sorter.sort(reader, temp_dir.name)
-    for l in lines:
-        writer.write(l)
+    sorter.sort(reader,writer, temp_dir.name)
     temp_dir.cleanup()
 
 
 def sortFile(src=None, tgt=None, sortType='i', unique=False, keyFn=_keyFn, nHead=-1, budget=0.8, tmpDir=None, nSplit=10, nLine=10000, buffering=1024*1024):
     if not src:
         reader = sys.stdin
     else:
@@ -229,15 +211,14 @@
 OrderingFn = {
     '<': operator.le,
     '<=': operator.lt,
     '==': operator.eq,
     '!=': operator.ne,
     '>=': operator.ge,
     '>': operator.gt,
-
 }
 
 
 def check(reader, Ordering='<=', keyFn=_keyFn):
     cmp = OrderingFn[Ordering]
     last = None
     i = -1
```

### Comparing `bigsort-0.0.6/setup.py` & `bigsort-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     long_description = f.read()
 
 
 setup(
     name="bigsort",
     # packages=find_packages(),
     py_modules=['bigsort'],
-    version='0.0.6',
+    version='0.0.7',
     description='sort big file or streams',
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires='>=3.0',
     install_requires=[
         "psutil",
         "logzero"
```

