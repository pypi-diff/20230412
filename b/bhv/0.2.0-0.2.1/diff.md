# Comparing `tmp/bhv-0.2.0.tar.gz` & `tmp/bhv-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.2.0.tar", last modified: Sat Apr  8 19:21:00 2023, max compression
+gzip compressed data, was "bhv-0.2.1.tar", last modified: Wed Apr 12 17:38:49 2023, max compression
```

## Comparing `bhv-0.2.0.tar` & `bhv-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-04-08 19:21:00.370536 bhv-0.2.0/
--rw-r--r--   0 adam      (1000) adam      (1000)     1060 2023-04-08 19:21:00.370536 bhv-0.2.0/PKG-INFO
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-04-08 19:21:00.370536 bhv-0.2.0/bhv/
--rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.2.0/bhv/__init__.py
--rw-r--r--   0 adam      (1000) adam      (1000)    10798 2023-04-07 21:10:32.000000 bhv-0.2.0/bhv/abstract.py
--rw-r--r--   0 adam      (1000) adam      (1000)     9571 2023-04-07 20:52:10.000000 bhv-0.2.0/bhv/np.py
--rw-r--r--   0 adam      (1000) adam      (1000)     7088 2023-04-07 20:52:10.000000 bhv-0.2.0/bhv/pytorch.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1980 2023-04-07 21:03:27.000000 bhv-0.2.0/bhv/shared.py
--rw-r--r--   0 adam      (1000) adam      (1000)     6120 2023-04-07 20:52:10.000000 bhv-0.2.0/bhv/symbolic.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-04-08 19:21:00.370536 bhv-0.2.0/bhv.egg-info/
--rw-r--r--   0 adam      (1000) adam      (1000)     1060 2023-04-08 19:21:00.000000 bhv-0.2.0/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)      229 2023-04-08 19:21:00.000000 bhv-0.2.0/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-04-08 19:21:00.000000 bhv-0.2.0/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       73 2023-04-08 19:21:00.000000 bhv-0.2.0/bhv.egg-info/requires.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-04-08 19:21:00.000000 bhv-0.2.0/bhv.egg-info/top_level.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-04-08 19:21:00.370536 bhv-0.2.0/setup.cfg
--rw-r--r--   0 adam      (1000) adam      (1000)     1331 2023-04-07 21:27:02.000000 bhv-0.2.0/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-12 17:38:49.661271 bhv-0.2.1/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1005 2023-04-12 17:38:49.661271 bhv-0.2.1/PKG-INFO
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-12 17:38:49.661271 bhv-0.2.1/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-11 14:49:00.000000 bhv-0.2.1/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11023 2023-04-12 17:37:58.000000 bhv-0.2.1/bhv/abstract.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1635 2023-04-11 14:49:00.000000 bhv-0.2.1/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     9571 2023-04-12 17:37:58.000000 bhv-0.2.1/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     7088 2023-04-12 17:37:58.000000 bhv-0.2.1/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2022 2023-04-11 14:49:00.000000 bhv-0.2.1/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8626 2023-04-12 17:37:58.000000 bhv-0.2.1/bhv/symbolic.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-12 17:38:49.661271 bhv-0.2.1/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1005 2023-04-12 17:38:49.000000 bhv-0.2.1/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      246 2023-04-12 17:38:49.000000 bhv-0.2.1/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-04-12 17:38:49.000000 bhv-0.2.1/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-04-12 17:38:49.000000 bhv-0.2.1/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-04-12 17:38:49.000000 bhv-0.2.1/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-04-12 17:38:49.661271 bhv-0.2.1/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-04-12 17:38:05.000000 bhv-0.2.1/setup.py
```

### Comparing `bhv-0.2.0/PKG-INFO` & `bhv-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.0
+Version: 0.2.1
 Summary: Boolean Hypervectors
-Home-page: UNKNOWN
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
-License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: Free for non-commercial use
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -23,8 +20,7 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Provides-Extra: torch
 Provides-Extra: torch-hd
 Provides-Extra: numpy
 
 Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).
-
```

### Comparing `bhv-0.2.0/bhv/abstract.py` & `bhv-0.2.1/bhv/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 
     @classmethod
     def majority3(cls, x, y, z) -> Self:
         return cls.majority([x, y, z])
 
     @classmethod
     def majority(cls, vs: list[Self]) -> Self:
+        assert len(vs) % 2 == 1,  "The majority function which is only defined on uneven length inputs, see maj_bundle"
         half = len(vs)//2
         disjunction = list(accumulate(vs[:half-1:-1], or_))[1:]
         conjunction = list(accumulate(vs[:half-1:-1], and_))[1:]
 
         @cache
         def rec(ons, offs):
             if ons + 1 > half:
@@ -293,14 +294,18 @@
     ONE: Self
 
 
 class MemoizedPermutation:
     _permutations: 'dict[int | tuple[int, ...], Self]'
 
     @classmethod
+    def nrandom(cls, n) -> list[Self]:
+        return [cls.random() for _ in range(n)]
+
+    @classmethod
     def random(cls) -> Self:
         raise NotImplementedError()
 
     def __mul__(self, other: Self) -> Self:
         raise NotImplementedError()
 
     def __invert__(self) -> Self:
```

### Comparing `bhv-0.2.0/bhv/np.py` & `bhv-0.2.1/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.0/bhv/pytorch.py` & `bhv-0.2.1/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.0/bhv/shared.py` & `bhv-0.2.1/bhv/shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 DIMENSION = 8192
 
 from dataclasses import fields, is_dataclass
 from base64 import _urlsafe_encode_translation
 import hashlib
 import binascii
+import sys
+
+sys.setrecursionlimit(75_000)
 
 
 def stable_hash(d) -> bytes:
     """
     Python's `hash` is not stable. That's a problem if you want to use it for persistence and inter-run consistency.
     This one is hand rolled, so don't fully trust it. In fact, if you see anything suspicious, please let me know.
     :param d: Something you want to hash
```

### Comparing `bhv-0.2.0/bhv/symbolic.py` & `bhv-0.2.1/bhv/symbolic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,47 @@
 from dataclasses import dataclass, field, fields
 from .abstract import *
 from .shared import stable_hashcode
 
 
-class SymbolicPermutation(MemoizedPermutation):
+class Symbolic:
+    def nodename(self, **kwargs):
+        return f"{type(self).__name__.upper()}"
+
+    def nodeid(self, structural=False, **kwargs):
+        return f"{type(self).__name__}{stable_hashcode(self).replace('-', '') if structural else str(id(self))}"
+
+    def children(self, **kwargs):
+        return [(getattr(self, f.name), f.name) for f in fields(self) if issubclass(f.type, Symbolic)]
+
+    def graphviz(self, structural=False, done=None, **kwargs):
+        noden = self.nodeid(structural, **kwargs)
+        if done is None:
+            done = set()
+        if noden in done:
+            return
+        done.add(noden)
+        kwargs |= dict(done=done, structural=structural)
+        nodecs = self.children(**kwargs)
+        print(f"{noden} [label=\"{self.nodename(**kwargs)}\"];")
+        for c, label in nodecs:
+            print(f"{noden} -> {c.nodeid(**kwargs)} [label=\"{label}\"];")
+            c.graphviz(**kwargs)
+
+    def show(self, **kwargs):
+        """
+        Shows the expression tree code-style.
+        Only works on referentially transparent DAGs.
+        :param kwargs: drawing options
+        :return: str
+        """
+        raise NotImplementedError()
+
+
+class SymbolicPermutation(Symbolic, MemoizedPermutation):
     _permutations: 'dict[int | tuple[int, ...], Self]' = {}
 
     @classmethod
     def random(cls) -> 'SymbolicPermutation':
         return PermRandom()
 
     def __mul__(self, other: 'SymbolicPermutation') -> 'SymbolicPermutation':
@@ -18,65 +52,57 @@
 
     def __call__(self, hv: 'SymbolicBHV') -> 'SymbolicBHV':
         return PermApply(self, hv)
 
 @dataclass
 class PermVar(SymbolicPermutation):
     name: str
-    def nodename(self, **kwards):
-        return f"{self.name}"
+    def nodename(self, **kwargs):
+        return self.name
+
+    def show(self, symbolic_var=False, **kwargs):
+        return f"ParmVar(\"{self.name}\")" if symbolic_var else self.name
 @dataclass
 class PermUnit(SymbolicPermutation):
-    pass
+    def show(self, impl="", **kwargs):
+        return impl + "UNIT"
 SymbolicPermutation.UNIT = PermUnit()
 randpermid = 0
 def next_perm_id():
     global randpermid
     randpermid += 1
     return randpermid
 @dataclass
 class PermRandom(SymbolicPermutation):
     id: int = field(default_factory=next_perm_id)
+
+    def show(self, impl="", **kwargs):
+        return impl + "random()"
 @dataclass
 class PermCompose(SymbolicPermutation):
     l: 'SymbolicPermutation'
     r: 'SymbolicPermutation'
+
+    def show(self, **kwargs):
+        return f"({self.l.show(**kwargs)} * {self.r.show(**kwargs)})"
 @dataclass
 class PermInvert(SymbolicPermutation):
     p: 'SymbolicPermutation'
+
+    def show(self, **kwargs):
+        return f"(~{self.p.show(**kwargs)})"
 @dataclass
 class PermApply(SymbolicPermutation):
     p: 'SymbolicPermutation'
     v: 'SymbolicBHV'
 
+    def show(self, **kwargs):
+        return f"{self.p.show(**kwargs)}({self.v.show(**kwargs)})"
 
-class SymbolicBHV(AbstractBHV):
-    def nodename(self, **kwargs):
-        return f"{type(self).__name__.upper()}"
-
-    def nodeid(self, structural=False, **kwargs):
-        return f"{type(self).__name__}{stable_hashcode(self).replace('-', '') if structural else str(id(self))}"
-
-    def children(self, **kwargs):
-        return [(getattr(self, f.name), f.name) for f in fields(self) if issubclass(f.type, SymbolicBHV)]
-
-    def graphviz(self, structural=False, done=None, **kwargs):
-        noden = self.nodeid(structural, **kwargs)
-        if done is None:
-            done = set()
-        if noden in done:
-            return
-        done.add(noden)
-        kwargs |= dict(done=done, structural=structural)
-        nodecs = self.children(**kwargs)
-        print(f"{noden} [label=\"{self.nodename(**kwargs)}\"];")
-        for c, label in nodecs:
-            print(f"{noden} -> {c.nodeid(**kwargs)};")
-            c.graphviz(**kwargs)
-
+class SymbolicBHV(Symbolic, AbstractBHV):
     @classmethod
     def rand(cls) -> Self:
         return Rand()
 
     @classmethod
     def rand2(cls, power=1) -> Self:
         return Rand2(power)
@@ -150,78 +176,125 @@
 
 
 
 @dataclass
 class Var(SymbolicBHV):
     name: str
     def nodename(self, **kwards):
-        return f"{self.name}"
+        return self.name
+
+    def show(self, symbolic_var=False, **kwargs):
+        return f"Var(\"{self.name}\")" if symbolic_var else self.name
 @dataclass
 class Zero(SymbolicBHV):
-    pass
+    def show(self, impl="", **kwargs):
+        return impl + "ZERO"
 @dataclass
 class One(SymbolicBHV):
-    pass
+    def show(self, impl="", **kwargs):
+        return impl + "ONE"
 SymbolicBHV.ZERO = Zero()
 SymbolicBHV.ONE = One()
 randid = 0
 def next_id():
     global randid
     randid += 1
     return randid
 @dataclass
 class Rand(SymbolicBHV):
     id: int = field(default_factory=next_id)
+
+    def show(self, impl="", **kwargs):
+        return impl + "rand()"
 @dataclass
 class Rand2(SymbolicBHV):
     power: int
+
+    def show(self, impl="", **kwargs):
+        return impl + f"rand2({self.power})"
 @dataclass
 class Random(SymbolicBHV):
     active: float
+
+    def show(self, impl="", **kwargs):
+        return impl + f"random({self.active})"
 @dataclass
 class Majority(SymbolicBHV):
     vs: list[SymbolicBHV]
+
+    def show(self, impl="", **kwargs):
+        return impl + f"majority({[v.show(**kwargs) for v in self.vs]})"
 @dataclass
 class Permute(SymbolicBHV):
-    id: int
+    id: 'int | tuple[int, ...]'
     v: SymbolicBHV
+
+    def show(self, **kwargs):
+        return f"{self.v.show(**kwargs)}.permute({self.id})"
 @dataclass
 class Eq:
     l: SymbolicBHV
     r: SymbolicBHV
+
+    def show(self, **kwargs):
+        return f"({self.l.show(**kwargs)} == {self.r.show(**kwargs)})"
 @dataclass
 class Xor(SymbolicBHV):
     l: SymbolicBHV
     r: SymbolicBHV
+
+    def show(self, **kwargs):
+        return f"({self.l.show(**kwargs)} ^ {self.r.show(**kwargs)})"
 @dataclass
 class And(SymbolicBHV):
     l: SymbolicBHV
     r: SymbolicBHV
+
+    def show(self, **kwargs):
+        return f"({self.l.show(**kwargs)} & {self.r.show(**kwargs)})"
 @dataclass
 class Or(SymbolicBHV):
     l: SymbolicBHV
     r: SymbolicBHV
+
+    def show(self, **kwargs):
+        return f"({self.l.show(**kwargs)} | {self.r.show(**kwargs)})"
 @dataclass
 class Invert(SymbolicBHV):
     v: SymbolicBHV
+
+    def show(self, **kwargs):
+        return f"(~{self.v.show(**kwargs)})"
 @dataclass
 class Select(SymbolicBHV):
     cond: SymbolicBHV
     when1: SymbolicBHV
     when0: SymbolicBHV
     def nodename(self, compact_select=True, **kwargs):
         return f"ON {self.cond.nodename()}" if compact_select else super().nodename(**kwargs)
     def children(self, compact_select=True, **kwargs):
         return [(self.when1, "1"), (self.when0, "0")] if compact_select else super().nodename(**kwargs)
+
+    def show(self, **kwargs):
+        return f"{self.cond.show(**kwargs)}.select({self.when1.show(**kwargs)}, {self.when0.show(**kwargs)})"
 @dataclass
 class Mix(SymbolicBHV):
     frac: float
     l: SymbolicBHV
     r: SymbolicBHV
+
+    def show(self, **kwargs):
+        return f"{self.l.show(**kwargs)}.mix({self.r.show(**kwargs)}, {self.frac})"
 @dataclass
-class Active:
+class Active(SymbolicBHV):
     v: SymbolicBHV
+
+    def show(self, **kwargs):
+        return f"{self.v.show(**kwargs)}.active()"
 @dataclass
-class BiasRel:
+class BiasRel(SymbolicBHV):
     rel: SymbolicBHV
     l: SymbolicBHV
     r: SymbolicBHV
+
+    def show(self, **kwargs):
+        return f"{self.l.show(**kwargs)}.mix({self.r.show(**kwargs)}, {self.rel.show(**kwargs)})"
```

### Comparing `bhv-0.2.0/bhv.egg-info/PKG-INFO` & `bhv-0.2.1/bhv.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.0
+Version: 0.2.1
 Summary: Boolean Hypervectors
-Home-page: UNKNOWN
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
-License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: Free for non-commercial use
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -23,8 +20,7 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Provides-Extra: torch
 Provides-Extra: torch-hd
 Provides-Extra: numpy
 
 Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).
-
```

### Comparing `bhv-0.2.0/setup.py` & `bhv-0.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
```

