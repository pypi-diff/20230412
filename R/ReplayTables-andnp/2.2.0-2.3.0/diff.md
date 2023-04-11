# Comparing `tmp/ReplayTables-andnp-2.2.0.tar.gz` & `tmp/ReplayTables-andnp-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReplayTables-andnp-2.2.0.tar", last modified: Thu Mar 16 20:46:25 2023, max compression
+gzip compressed data, was "ReplayTables-andnp-2.3.0.tar", last modified: Tue Apr 11 22:55:10 2023, max compression
```

## Comparing `ReplayTables-andnp-2.2.0.tar` & `ReplayTables-andnp-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2023-03-16 20:45:53.721524 ReplayTables-andnp-2.2.0/README.md
--rw-r--r--   0        0        0     5174 2023-03-16 20:45:53.721524 ReplayTables-andnp-2.2.0/ReplayTables/Distributions.py
--rw-r--r--   0        0        0     2140 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/ReplayTables/LagBuffer.py
--rw-r--r--   0        0        0     2311 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/ReplayTables/PER.py
--rw-r--r--   0        0        0     1916 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/ReplayTables/ReplayBuffer.py
--rw-r--r--   0        0        0     8232 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/ReplayTables/Table.py
--rw-r--r--   0        0        0        0 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/ReplayTables/__init__.py
--rw-r--r--   0        0        0     3416 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/ReplayTables/_utils/MemoryWriter.py
--rw-r--r--   0        0        0     1772 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/ReplayTables/_utils/RandDict.py
--rw-r--r--   0        0        0     3816 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/ReplayTables/_utils/SumTree.py
--rw-r--r--   0        0        0        0 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/ReplayTables/_utils/__init__.py
--rw-r--r--   0        0        0     1220 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/ReplayTables/_utils/jit.py
--rw-r--r--   0        0        0      887 2023-03-16 20:46:24.161911 ReplayTables-andnp-2.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0     3076 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/tests/test_LagBuffer.py
--rw-r--r--   0        0        0     1944 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/tests/test_PER.py
--rw-r--r--   0        0        0     1878 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/tests/test_ReplayBuffer.py
--rw-r--r--   0        0        0     1537 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/tests/test_Table.py
--rw-r--r--   0        0        0     5621 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/tests/test_View.py
--rw-r--r--   0        0        0        0 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     2987 2023-03-16 20:45:53.725524 ReplayTables-andnp-2.2.0/tests/utils/test_SumTree.py
--rw-r--r--   0        0        0      283 1970-01-01 00:00:00.000000 ReplayTables-andnp-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/README.md
+-rw-r--r--   0        0        0     5174 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/Distributions.py
+-rw-r--r--   0        0        0     2140 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/LagBuffer.py
+-rw-r--r--   0        0        0     2311 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/PER.py
+-rw-r--r--   0        0        0     3622 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/ReplayBuffer.py
+-rw-r--r--   0        0        0     8232 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/Table.py
+-rw-r--r--   0        0        0        0 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/__init__.py
+-rw-r--r--   0        0        0     3416 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/_utils/MemoryWriter.py
+-rw-r--r--   0        0        0     1772 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/_utils/RandDict.py
+-rw-r--r--   0        0        0     3816 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/_utils/SumTree.py
+-rw-r--r--   0        0        0        0 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/_utils/__init__.py
+-rw-r--r--   0        0        0     1220 2023-04-11 22:54:38.383151 ReplayTables-andnp-2.3.0/ReplayTables/_utils/jit.py
+-rw-r--r--   0        0        0      888 2023-04-11 22:55:09.579496 ReplayTables-andnp-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3076 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/test_LagBuffer.py
+-rw-r--r--   0        0        0     1944 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/test_PER.py
+-rw-r--r--   0        0        0     2679 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/test_ReplayBuffer.py
+-rw-r--r--   0        0        0     1537 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/test_Table.py
+-rw-r--r--   0        0        0     5621 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/test_View.py
+-rw-r--r--   0        0        0        0 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2987 2023-04-11 22:54:38.387151 ReplayTables-andnp-2.3.0/tests/utils/test_SumTree.py
+-rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 ReplayTables-andnp-2.3.0/PKG-INFO
```

### Comparing `ReplayTables-andnp-2.2.0/ReplayTables/Distributions.py` & `ReplayTables-andnp-2.3.0/ReplayTables/Distributions.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.2.0/ReplayTables/LagBuffer.py` & `ReplayTables-andnp-2.3.0/ReplayTables/LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.2.0/ReplayTables/PER.py` & `ReplayTables-andnp-2.3.0/ReplayTables/PER.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.2.0/ReplayTables/Table.py` & `ReplayTables-andnp-2.3.0/ReplayTables/Table.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.2.0/ReplayTables/_utils/MemoryWriter.py` & `ReplayTables-andnp-2.3.0/ReplayTables/_utils/MemoryWriter.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.2.0/ReplayTables/_utils/RandDict.py` & `ReplayTables-andnp-2.3.0/ReplayTables/_utils/RandDict.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.2.0/ReplayTables/_utils/SumTree.py` & `ReplayTables-andnp-2.3.0/ReplayTables/_utils/SumTree.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.2.0/ReplayTables/_utils/jit.py` & `ReplayTables-andnp-2.3.0/ReplayTables/_utils/jit.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.2.0/pyproject.toml` & `ReplayTables-andnp-2.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "2.2.0"
+version = "2.3.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
 ]
 
 [tool.pdm]
 source = [
@@ -22,25 +22,25 @@
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "ReplayTables-andnp"
-version = "2.2.0"
+version = "2.3.0"
 description = "A simple replay buffer implementation in python for sampling n-step trajectories"
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "numba>=0.56.4",
     "numpy>=1.23.5",
     "scipy>=1.9.3",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
```

### Comparing `ReplayTables-andnp-2.2.0/tests/test_LagBuffer.py` & `ReplayTables-andnp-2.3.0/tests/test_LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.2.0/tests/test_PER.py` & `ReplayTables-andnp-2.3.0/tests/test_PER.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.2.0/tests/test_ReplayBuffer.py` & `ReplayTables-andnp-2.3.0/tests/test_ReplayBuffer.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import numpy as np
 import pickle
 from typing import NamedTuple
 
 from ReplayTables.ReplayBuffer import ReplayBuffer
 
 class Data(NamedTuple):
-    a: float
-    b: int
+    a: float | np.ndarray
+    b: int | np.ndarray
 
 
 class TestReplayBuffer(unittest.TestCase):
     def test_simple_buffer(self):
         rng = np.random.RandomState(0)
         buffer = ReplayBuffer(5, Data, rng)
 
@@ -45,14 +45,39 @@
         self.assertEqual(buffer.size(), 5)
 
         samples, _, _ = buffer.sample(1000)
         unique = np.unique(samples.b)
         unique.sort()
         self.assertTrue(np.all(unique == np.array([2, 3, 4, 5, 6])))
 
+    def test_getitem(self):
+        rng = np.random.RandomState(0)
+        buffer = ReplayBuffer(10, Data, rng)
+
+        for i in range(15):
+            buffer.add(Data(a=i, b=2 * i))
+
+        # should be the most recently added item
+        got, _, _ = buffer[0]
+        expect = Data(a=np.array([14]), b=np.array([28]))
+        self.assertEqual(got, expect)
+
+        # should be oldest item in buffer
+        got, _, _ = buffer[-1]
+        expect = Data(a=np.array([5]), b=np.array([10]))
+        self.assertEqual(got, expect)
+
+        got, _, _ = buffer[2:7:2]
+        expect = Data(
+            a=np.array([12, 10, 8]),
+            b=np.array([24, 20, 16]),
+        )
+        self.assertTrue(np.all(got.a == expect.a))
+        self.assertTrue(np.all(got.b == expect.b))
+
     def test_pickleable(self):
         rng = np.random.RandomState(0)
         buffer = ReplayBuffer(5, Data, rng)
 
         for i in range(8):
             buffer.add(Data(a=i, b=i))
```

### Comparing `ReplayTables-andnp-2.2.0/tests/test_Table.py` & `ReplayTables-andnp-2.3.0/tests/test_Table.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.2.0/tests/test_View.py` & `ReplayTables-andnp-2.3.0/tests/test_View.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.2.0/tests/utils/test_SumTree.py` & `ReplayTables-andnp-2.3.0/tests/utils/test_SumTree.py`

 * *Files identical despite different names*

