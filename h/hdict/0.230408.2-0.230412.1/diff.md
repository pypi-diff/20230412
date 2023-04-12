# Comparing `tmp/hdict-0.230408.2.tar.gz` & `tmp/hdict-0.230412.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdict-0.230408.2.tar", max compression
+gzip compressed data, was "hdict-0.230412.1.tar", max compression
```

## Comparing `hdict-0.230408.2.tar` & `hdict-0.230412.1.tar`

### file list

```diff
@@ -1,36 +1,42 @@
--rw-r--r--   0        0        0    35149 2022-12-26 01:24:40.000000 hdict-0.230408.2/LICENSE
--rw-r--r--   0        0        0     7464 2023-04-08 04:19:10.268200 hdict-0.230408.2/README.md
--rw-r--r--   0        0        0     1177 2023-04-08 04:19:16.104278 hdict-0.230408.2/pyproject.toml
--rw-r--r--   0        0        0    14147 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/__init__.py
--rw-r--r--   0        0        0      223 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/abs/__init__.py
--rw-r--r--   0        0        0     2506 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/applyout.py
--rw-r--r--   0        0        0     3389 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/aux_frozendict.py
--rw-r--r--   0        0        0        0 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/__init__.py
--rw-r--r--   0        0        0      714 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/argument/__init__.py
--rw-r--r--   0        0        0     9033 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/argument/apply.py
--rw-r--r--   0        0        0     2862 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/argument/aux_apply.py
--rw-r--r--   0        0        0     1463 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/argument/default.py
--rw-r--r--   0        0        0     2162 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/argument/field.py
--rw-r--r--   0        0        0     2328 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/argument/sample.py
--rw-r--r--   0        0        0     2026 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/entry/__init__.py
--rw-r--r--   0        0        0     1473 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/entry/aux_closure.py
--rw-r--r--   0        0        0     3379 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/entry/closure.py
--rw-r--r--   0        0        0      515 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/entry/lazy.py
--rw-r--r--   0        0        0     2717 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/entry/subvalue.py
--rw-r--r--   0        0        0     2249 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/value.py
--rw-r--r--   0        0        0     7367 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/customjson.py
--rw-r--r--   0        0        0        0 2023-03-19 02:22:28.761130 hdict-0.230408.2/src/hdict/data/__init__.py
--rw-r--r--   0        0        0     8146 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/data/dataset.py
--rw-r--r--   0        0        0     1619 2023-03-19 04:58:08.124551 hdict-0.230408.2/src/hdict/data/load.py
--rw-r--r--   0        0        0     1909 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/empty_.py
--rw-r--r--   0        0        0     3100 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/expr.py
--rw-r--r--   0        0        0    16616 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/frozenhdict.py
--rw-r--r--   0        0        0    16799 2023-04-08 04:16:53.238376 hdict-0.230408.2/src/hdict/hdict_.py
--rw-r--r--   0        0        0     3855 2023-01-29 20:20:35.027416 hdict-0.230408.2/src/hdict/hoshfication.py
--rw-r--r--   0        0        0     1334 2023-01-29 00:09:41.512891 hdict-0.230408.2/src/hdict/indexeddict.py
--rw-r--r--   0        0        0     3956 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/multioutput.py
--rw-r--r--   0        0        0     2311 2023-03-15 00:26:20.740920 hdict-0.230408.2/src/hdict/pandas_handling.py
--rw-r--r--   0        0        0        0 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/persistence/__init__.py
--rw-r--r--   0        0        0     1059 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/persistence/cache.py
--rw-r--r--   0        0        0     8836 1970-01-01 00:00:00.000000 hdict-0.230408.2/setup.py
--rw-r--r--   0        0        0     8385 1970-01-01 00:00:00.000000 hdict-0.230408.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-26 01:24:40.000000 hdict-0.230412.1/LICENSE
+-rw-r--r--   0        0        0     7464 2023-04-12 20:18:28.595382 hdict-0.230412.1/README.md
+-rw-r--r--   0        0        0     1369 2023-04-12 20:32:48.504269 hdict-0.230412.1/pyproject.toml
+-rw-r--r--   0        0        0    15593 2023-04-10 02:17:58.720650 hdict-0.230412.1/src/hdict/__init__.py
+-rw-r--r--   0        0        0      223 2023-04-08 04:05:25.273250 hdict-0.230412.1/src/hdict/abs/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-08 04:05:25.273250 hdict-0.230412.1/src/hdict/content/__init__.py
+-rw-r--r--   0        0        0      755 2023-04-08 19:59:38.981761 hdict-0.230412.1/src/hdict/content/argument/__init__.py
+-rw-r--r--   0        0        0    13865 2023-04-12 20:17:41.450684 hdict-0.230412.1/src/hdict/content/argument/apply.py
+-rw-r--r--   0        0        0     3121 2023-04-09 21:56:47.979809 hdict-0.230412.1/src/hdict/content/argument/aux_apply.py
+-rw-r--r--   0        0        0     1483 2023-04-10 01:15:22.584449 hdict-0.230412.1/src/hdict/content/argument/default.py
+-rw-r--r--   0        0        0     1318 2023-04-08 19:30:32.031213 hdict-0.230412.1/src/hdict/content/argument/entry.py
+-rw-r--r--   0        0        0     2162 2023-04-08 04:05:25.273250 hdict-0.230412.1/src/hdict/content/argument/field.py
+-rw-r--r--   0        0        0     2328 2023-04-08 04:05:25.273250 hdict-0.230412.1/src/hdict/content/argument/sample.py
+-rw-r--r--   0        0        0     3855 2023-01-29 20:20:35.027416 hdict-0.230412.1/src/hdict/content/aux_value.py
+-rw-r--r--   0        0        0     2011 2023-04-12 03:04:01.496598 hdict-0.230412.1/src/hdict/content/entry/__init__.py
+-rw-r--r--   0        0        0     1965 2023-04-12 20:17:41.358683 hdict-0.230412.1/src/hdict/content/entry/aux_closure.py
+-rw-r--r--   0        0        0     1346 2023-04-12 20:17:41.358683 hdict-0.230412.1/src/hdict/content/entry/cached.py
+-rw-r--r--   0        0        0     4337 2023-04-12 20:17:41.418684 hdict-0.230412.1/src/hdict/content/entry/closure.py
+-rw-r--r--   0        0        0     2836 2023-04-12 20:17:41.342683 hdict-0.230412.1/src/hdict/content/entry/subvalue.py
+-rw-r--r--   0        0        0      541 2023-04-12 20:17:41.322682 hdict-0.230412.1/src/hdict/content/entry/wrapper.py
+-rw-r--r--   0        0        0     2254 2023-04-09 16:29:46.578822 hdict-0.230412.1/src/hdict/content/value.py
+-rw-r--r--   0        0        0        0 2023-04-09 16:23:36.171526 hdict-0.230412.1/src/hdict/data/__init__.py
+-rw-r--r--   0        0        0    10419 2023-04-12 20:17:41.442684 hdict-0.230412.1/src/hdict/data/aux_frozendict.py
+-rw-r--r--   0        0        0     2211 2023-04-12 20:12:17.393861 hdict-0.230412.1/src/hdict/data/empty_.py
+-rw-r--r--   0        0        0    20295 2023-04-12 20:17:41.534686 hdict-0.230412.1/src/hdict/data/frozenhdict.py
+-rw-r--r--   0        0        0    25386 2023-04-12 19:38:21.121053 hdict-0.230412.1/src/hdict/data/hdict_.py
+-rw-r--r--   0        0        0        0 2023-03-19 02:22:28.761130 hdict-0.230412.1/src/hdict/dataset/__init__.py
+-rw-r--r--   0        0        0     6523 2023-04-12 20:17:41.354683 hdict-0.230412.1/src/hdict/dataset/dataset.py
+-rw-r--r--   0        0        0     4273 2023-04-12 20:17:41.334683 hdict-0.230412.1/src/hdict/dataset/pandas_handling.py
+-rw-r--r--   0        0        0        0 2023-04-09 16:15:22.403037 hdict-0.230412.1/src/hdict/expression/__init__.py
+-rw-r--r--   0        0        0     3543 2023-04-12 20:17:41.362683 hdict-0.230412.1/src/hdict/expression/expr.py
+-rw-r--r--   0        0        0        0 2023-04-09 16:21:52.487456 hdict-0.230412.1/src/hdict/expression/step/__init__.py
+-rw-r--r--   0        0        0     2280 2023-04-10 01:05:51.172495 hdict-0.230412.1/src/hdict/expression/step/applyout.py
+-rw-r--r--   0        0        0     2529 2023-04-09 16:42:55.111337 hdict-0.230412.1/src/hdict/expression/step/cache.py
+-rw-r--r--   0        0        0      395 2023-04-12 20:17:41.330683 hdict-0.230412.1/src/hdict/expression/step/edict.py
+-rw-r--r--   0        0        0     2198 2023-04-12 20:17:41.370683 hdict-0.230412.1/src/hdict/expression/step/step.py
+-rw-r--r--   0        0        0        0 2023-04-08 04:05:25.273250 hdict-0.230412.1/src/hdict/persistence/__init__.py
+-rw-r--r--   0        0        0     1223 2023-04-09 01:26:32.621571 hdict-0.230412.1/src/hdict/persistence/stored.py
+-rw-r--r--   0        0        0        0 2023-04-09 16:30:09.274848 hdict-0.230412.1/src/hdict/text/__init__.py
+-rw-r--r--   0        0        0     7455 2023-04-12 19:38:03.344816 hdict-0.230412.1/src/hdict/text/customjson.py
+-rw-r--r--   0        0        0     8993 1970-01-01 00:00:00.000000 hdict-0.230412.1/setup.py
+-rw-r--r--   0        0        0     8508 1970-01-01 00:00:00.000000 hdict-0.230412.1/PKG-INFO
```

### Comparing `hdict-0.230408.2/LICENSE` & `hdict-0.230412.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hdict-0.230408.2/README.md` & `hdict-0.230412.1/README.md`

 * *Files identical despite different names*

### Comparing `hdict-0.230408.2/pyproject.toml` & `hdict-0.230412.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 [tool.poetry]
 name = "hdict"
-version = "0.230408.2"
+version = "0.230412.1"
 description = "A versatile dictionary based on a novel paradigm useful for computing, caching, experiments, distributed data, among others."
 authors = ["davips <dpsabc@gmail.com>"]
 license = "GPLv3"
 readme = 'README.md'
 packages = [
     { include = "hdict", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+hosh = "^2.230205.2"
 indexed = "^1.3.0"  # indexed dict
 lange = "^1.230203.2"
+
 # Optional dependencies.
-pandas = { version = "^1.5.2", optional = true }
-hosh = "^2.230205.2"
+pandas = { version = "^2.0.0", optional = true }
 shelchemy = { version = "^0.220906.3", optional = true }
 safeserializer = { version = "^0.230202.1", optional = true }
 lz4 = { version = "^4.3.2", optional = true }
+scikit-learn = { version = "^1.2.2", optional = true }
+liac-arff = { version = "^2.5.0", optional = true }
 
 [tool.poetry.extras]    #[tool.poetry.group.extras.dependencies]
-full = ["pandas", "shelchemy", "safeserializer", "lz4"]
+full = ["pandas", "shelchemy", "safeserializer", "lz4", "scikit-learn", "liac-arff"]
 
 [tool.poetry.group.dev.dependencies]
 autoreadme = "^0.2102.20"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 black = "^22.6.0"
 pdoc3 = "^0.10.0"
 pylint = "^2.7.4"
+testfixtures = "^7.1.0"
 ipython = "^8.9.0"
-pandas = "^1.5.3"
-arff = "^0.9"
+pandas = "^2.0.0"
 shelchemy = "^0.220906.5"
 safeserializer = "^0.230202.1"
 lz4 = "^4.3.2"
+scikit-learn = "^1.2.2"
+liac-arff = "^2.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hdict-0.230408.2/src/hdict/__init__.py` & `hdict-0.230412.1/src/hdict/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,20 +21,21 @@
 #  time spent here.
 #
 from typing import TypeVar
 
 from hdict.content.argument.apply import apply
 from hdict.content.argument.field import field
 from hdict.content.argument.sample import sample
-from hdict.empty_ import Empty_
+from hdict.data.empty_ import Empty_
 from hdict.content.value import value
-from hdict.frozenhdict import frozenhdict
-from hdict.hdict_ import hdict_
+from hdict.data.frozenhdict import frozenhdict
+from hdict.data.hdict_ import hdict_
+from hdict.expression.step.cache import cache
 
-__all__ = ["hdict", "_", "Ø", "apply", "field", "sample", "frozenhdict", "value"]
+__all__ = ["hdict", "_", "Ø", "apply", "field", "sample", "frozenhdict", "value", "cache"]
 
 VT = TypeVar("VT")
 
 
 class hdict(hdict_):
     """
     Function id is reversed before application.
@@ -161,23 +162,20 @@
     >>> from hdict import value
     >>> d.evaluate()
     >>> d = hdict(x=2)
     >>> g = lambda x, y: [x + y, x / y]
     >>> d["z"] = apply(f, 2, y=3)
     >>> d["w", "v"] = apply(f, field("x"), y=33)
     >>> d["f"] = f
-    >>> cache = {}
     >>> d = d >> apply(field("f"), field("x"), y=default(3), nonexistent_parameter=7)("w3", "v3") # TODO: nonexistent parameter should raise an exception
     >>> d >>= apply(field("f"), field("x"), y=default(3))("w", "v")
     >>> d["w2", "v2"] = apply(field("f"), field("x"), y=default(3))
     >>> d >>= {"z": apply(f, field("x"), y=3), ("w", "v"): apply(g, y=7)}
     >>> d >>= apply(f, field("x"), y=3)("z9") * apply(g, y=7)("w9", "v9")
     >>> pp = apply(f, field("x"), y=3)("z") >> apply(g, y=7)("w", "v")
-    >>> type(pp)
-    <class 'hdict.expr.Expr'>
     >>> d >>= {"x": 3} >> pp >> apply(g, y=7)("w", "v")
     >>> from hdict import _
     >>> a1 = apply(f, y=_[1, 2, 4, ..., 128])
     >>> a2 = apply(f, _[0, 3, 6, ..., 9], y=_[0, 3, 6, ..., 9])
     >>> ppp = hdict() >> a2.sample()("k", "t")
     >>> ppp.show(colored=False)
     {
@@ -340,15 +338,15 @@
     True
     >>> hdict(x=3) != hdict(y=3)
     True
     >>> del d["x"]
     >>> list(d)
     ['y']
     >>> e = d >> apply(lambda y: y*7)("y")
-    >>> from hdict.hoshfication import f2hosh
+    >>> from hdict.content.aux_value import f2hosh
     >>> print(f2hosh(lambda y: y*7))
     54YCMDJIlsIvMQ.KJtT-vFyjg83Zgfj2xSHOgCj8
     >>> print(e)
     {y: "λ(4)"}
     >>> e.evaluate()
     >>> print(e)
     {y: 28}
@@ -394,14 +392,64 @@
         _id: q5J7ZUr3gs0bKrG4AxVEY2q0-XH3Suvw5X8-j6do,
         _ids: {
             a: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             y: -2A0hTRBN1wtIKQxLzRcYDBkhv1hu-dMY-24Jye9,
             x: gak9o6ZS9plw9l63f0WtAFnr52.1HycGhc3En2MR
         }
     }
+    >>> def f():
+    ...     print("busy")
+    ...     return 23
+    >>> storage = {}
+    >>> d >>= apply(f).o >> cache(storage, "x", "y")
+    >>> d.y
+    28
+    >>> d.show(colored=False)
+    {
+        a: 5,
+        y: 28,
+        x: ↑↓ cached at `dict`·,
+        o: λ(),
+        _id: Lvc0oqaeG42YNbEHLovwwDD7u3kMV0QTN6EXCmh1,
+        _ids: {
+            a: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
+            y: -2A0hTRBN1wtIKQxLzRcYDBkhv1hu-dMY-24Jye9,
+            x: gak9o6ZS9plw9l63f0WtAFnr52.1HycGhc3En2MR,
+            o: tvj9HwT9g5Ud9SKoUqDJI1zw5ut7VRRTrSEe9fUt
+        }
+    }
+    >>> d.evaluated.show(colored=False)
+    busy
+    {
+        a: 5,
+        y: 28,
+        x: 5,
+        o: 23,
+        _id: Lvc0oqaeG42YNbEHLovwwDD7u3kMV0QTN6EXCmh1,
+        _ids: {
+            a: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
+            y: -2A0hTRBN1wtIKQxLzRcYDBkhv1hu-dMY-24Jye9,
+            x: gak9o6ZS9plw9l63f0WtAFnr52.1HycGhc3En2MR,
+            o: tvj9HwT9g5Ud9SKoUqDJI1zw5ut7VRRTrSEe9fUt
+        }
+    }
+    >>> d.evaluated.show(colored=False)
+    {
+        a: 5,
+        y: 28,
+        x: 5,
+        o: 23,
+        _id: Lvc0oqaeG42YNbEHLovwwDD7u3kMV0QTN6EXCmh1,
+        _ids: {
+            a: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
+            y: -2A0hTRBN1wtIKQxLzRcYDBkhv1hu-dMY-24Jye9,
+            x: gak9o6ZS9plw9l63f0WtAFnr52.1HycGhc3En2MR,
+            o: tvj9HwT9g5Ud9SKoUqDJI1zw5ut7VRRTrSEe9fUt
+        }
+    }
     """
 
 
 class Empty(Empty_):
     """
     >>> from hdict import _
     >>> d = _ >> {"x": 5} >> dict(y=7)
```

### Comparing `hdict-0.230408.2/src/hdict/content/argument/__init__.py` & `hdict-0.230412.1/src/hdict/content/argument/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
     def sample(self, rnd: int | Random = None):
         return self
 
 
 class AbsBaseArgument(AbsArgument):
     """
-    Normal function argument provided by the user: value*, field, apply
+    Normal function argument provided by the user: `value`*, `field`, `apply`; or from advanced use: `entry`
 
     Exceptionally, 'field' is a subclass that can also be piped through '>>'
     *value also inherits AbsReadyEntry
     """
 
 
 class AbsMetaArgument(AbsArgument):
     """
-    Special temporary argument-like directive provided by the user: default, sample
+    Special temporary argument-like directive provided by the user: `default`, `sample`
     """
```

### Comparing `hdict-0.230408.2/src/hdict/content/argument/aux_apply.py` & `hdict-0.230412.1/src/hdict/content/argument/aux_apply.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,22 @@
+from indexed import IndexedOrderedDict
+
 from hdict.content.argument import AbsArgument
-from hdict.indexeddict import IndexedDict
+
+
+class IndexedDict(IndexedOrderedDict):
+    """
+    Wrapper with a cleaner repr(esentation) of IndexedOrderedDict.
+
+    >>> IndexedDict([('a', 'a'), ('b', 'b')])
+    {'a': 'a', 'b': 'b'}
+    """
+
+    def __repr__(self):
+        return repr(dict(self.items()))
 
 
 class Arg:
     def __init__(self, position: int):
         self.position = position
 
     def __hash__(self):
```

### Comparing `hdict-0.230408.2/src/hdict/content/argument/default.py` & `hdict-0.230412.1/src/hdict/content/argument/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 from hdict.abs import AbsAny
 from hdict.content.argument import AbsMetaArgument
 
 
 class default(AbsMetaArgument):
     def __init__(self, value: object | Callable):
         self.value = value
-        if isinstance(value, AbsAny):
+        if isinstance(value, AbsAny):  # pragma: no cover
             raise Exception(f"Cannot use a `{type(value).__name__}` as a default function value.")
 
     def __repr__(self):
         return f"default({repr(self.value)})"
```

### Comparing `hdict-0.230408.2/src/hdict/content/argument/field.py` & `hdict-0.230412.1/src/hdict/content/argument/field.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230408.2/src/hdict/content/argument/sample.py` & `hdict-0.230412.1/src/hdict/content/argument/sample.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230408.2/src/hdict/content/entry/__init__.py` & `hdict-0.230412.1/src/hdict/content/entry/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,30 +26,27 @@
 from hosh import Hosh
 
 from hdict.abs import AbsAny
 
 
 @dataclass
 class Unevaluated:
-    n = 0
-
-
-Unevaluated = Unevaluated()
+    pass
 
 
 class AbsEntry(AbsAny):
     """
     hdict final entry at internal level: value*, SubValue, Closure
 
     *value also inherits AbsBaseArgument because 'value' objects have a meaning outside of hdict (external level)
     """
 
     value: object | Callable  # REMINDER: 'callable' is here for appliable contents, like storing a raw lambda
     hosh: Hosh
-    _value = Unevaluated
+    _value = Unevaluated()
 
     @property
     def id(self):  # pragma: no cover
         return self.hosh.id
 
     def evaluate(self):
         _ = self.value
@@ -58,8 +55,8 @@
     def isevaluated(self):
         """
         >>> from hdict import apply
         >>> from hdict.content.entry.closure import Closure
         >>> Closure(apply(lambda x, y: x + y), {"x": 3, "y": 5}, []).isevaluated
         False
         """
-        return self._value != Unevaluated
+        return not isinstance(self._value, Unevaluated)
```

### Comparing `hdict-0.230408.2/src/hdict/content/entry/aux_closure.py` & `hdict-0.230412.1/src/hdict/content/entry/aux_closure.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 from __future__ import annotations
 
-from hdict.aux_frozendict import MissingFieldException
 from hdict.content.argument import AbsBaseArgument
 
 
 def handle_arg(key, val, data, discarded_defaults, out, torepr):
     """Return handled arg and value of pseudocircular entry"""
     from hdict.content.argument.default import default
     from hdict.content.value import value
-    from hdict.aux_frozendict import handle_item
+    from hdict.data.aux_frozendict import handle_item
     from hdict import field
+    from hdict.data.aux_frozendict import MissingFieldException
+
+    from hdict.content.argument.entry import entry
+    from hdict.content.entry.subvalue import SubValue
 
     match val:
         case default(value=v):
             if key in data:
                 arg = data[key]
                 # REMINDER: `discarded_defaults` exists only for __repr__ purposes
                 discarded_defaults.add(key)
             else:
                 arg = value(v)
             if key in out:
                 torepr[key] = arg
                 return arg
         case field(name=name) if name in out:  # Override case of handle_item if pseudocircular reference.
-            if name not in data:
+            if name not in data:  # pragma: no cover
                 raise MissingFieldException(f"Missing pseudocircular field `{name}`")
-            arg = handle_item(str(key), val, data)
+            arg = handle_item(str(key), data[name], data)  # key passed for no purpose here AFAIR
             torepr[key] = arg
             return arg
+        case entry(name=name):
+            from hdict.content.entry.wrapper import Wrapper
+
+            if name not in data:  # pragma: no cover
+                raise MissingFieldException(f"Missing pseudocircular field `{name}`")
+            content = handle_item(str(key), data[name], data)
+            arg = Wrapper(content)
+            torepr[f"·{name}"] = arg
+            return arg
         case AbsBaseArgument():
             arg = handle_item(str(key), val, data)
-        case _:
+        case _:  # pragma: no cover
             raise Exception(f"Cannot handle argument of type `{type(val).__name__}`")
     torepr[key] = val
     return arg
-
-
-def isint(s):
-    try:
-        int(s)
-        return True
-    except ValueError:
-        return False
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hdict-0.230408.2/src/hdict/content/entry/closure.py` & `hdict-0.230412.1/src/hdict/content/entry/closure.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from hosh import ø
 
 from hdict.content.argument import AbsArgument
 from hdict.content.argument.apply import apply
 from hdict.content.argument.default import default
 from hdict.content.entry import AbsEntry, Unevaluated
 from hdict.content.entry.aux_closure import handle_arg
-from hdict.customjson import truncate
+from hdict.text.customjson import truncate
 
 
 class Closure(AbsEntry):
     def __init__(self, application: apply, data: dict[str, AbsEntry], out: list):
-        from hdict.aux_frozendict import handle_item
+        from hdict.data.aux_frozendict import handle_item
 
         self.application = application
         self.out = out
         self.torepr = {}
         hosh = ø
         arg = None
         fargs, fkwargs, discarded_defaults = {}, {}, set()
@@ -37,15 +37,19 @@
         if application.isfield:
             appliable_entry = handle_item(application.appliable.name, application.appliable, data)
             hosh *= appliable_entry.hosh.rev
 
             def f():
                 args = (x.value for x in fargs.values())
                 kwargs = {k: v.value for k, v in fkwargs.items()}
-                return appliable_entry.value(*args, **kwargs)
+                try:
+                    return appliable_entry.value(*args, **kwargs)
+                except TypeError as e:  # pragma: no cover
+                    if "required positional argument" in str(e):
+                        raise Exception(f"{str(e)}\n" f"HINT: If you are applying a field, " f"you should make the function parameters explicit, e.g.: `apply(f, parameter1, parameter2)`.")
 
         else:
             hosh *= application.ahosh
             appliable_function = application.appliable
 
             def f():
                 args = (x.value for x in fargs.values())
@@ -54,37 +58,54 @@
 
         self.f = f
         self.hosh = hosh
         self.discarded_defaults = discarded_defaults
 
     @property
     def value(self):
-        if self._value == Unevaluated:
+        if isinstance(self._value, Unevaluated):
             self._value = self.f()
             # del self.application  # TODO: delete clasure.application inside each subvalue?
         return self._value
 
-    def __repr__(self):
+    def __repr__(self, out=None):
         from hdict import value
         from hdict import field
+        from hdict.content.entry.wrapper import Wrapper
 
+        if out is None:
+            out = []
+        out = out + self.out
         lst = []
         for param, content in self.torepr.items():
             pre = "" if isinstance(param, int) else f"{param}="
+
             match content:
                 case value():
                     lst.append(truncate(repr(content), width=7))
+
                 case default() if param in self.discarded_defaults:
                     lst.append(f"{param}")
                 case default(value=v):
                     lst.append(f"{param}={v}")
-                case field(name) if name in self.out:
-                    lst.append(f"{repr(content)}")
+
+                # case field(name) if name in out:
+                #     lst.append(repr(content))
                 case field(name) if name == param:
                     lst.append(f"{param}")
                 case field(name):
                     lst.append(f"{pre}{name}")
+
+                case Wrapper(entry_):
+                    if isinstance(entry_, Closure):
+                        lst.append(entry_.__repr__(out))
+                    else:
+                        lst.append(param)
+                case Closure():
+                    lst.append(f"{pre}{content.value if content.isevaluated else content.__repr__(out)}")
                 case AbsArgument():
                     lst.append(f"{pre}{repr(content)}")
-                case _:
+                case AbsEntry():
+                    lst.append(f"{pre}{repr(content)}")
+                case _:  # pragma: no cover
                     raise Exception(type(content))
         return f"λ({' '.join(lst)})"
```

### Comparing `hdict-0.230408.2/src/hdict/content/entry/subvalue.py` & `hdict-0.230412.1/src/hdict/content/entry/subvalue.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,38 +16,49 @@
 #  along with hdict.  If not, see <http://www.gnu.org/licenses/>.
 #
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
+from dataclasses import dataclass
+
 from hdict.content.entry import AbsEntry
 
 
+@dataclass
 class SubValue(AbsEntry):
     """
     A field containing part of other field
 
     >>> from hdict import value
     >>> v = SubValue(value([3]), 0, 1)
     >>> v
     [3]→0
     >>> v.value
     3
+    >>> v
+    3
     """
 
-    def __init__(self, parent: AbsEntry, index: int, n: int, source: str = None):
-        self.parent, self.index, self.n, self.source = parent, index, n, source
-        self.hosh = parent.hosh[index:n]
+    parent: AbsEntry
+    index: int
+    n: int
+    source: str = None
+
+    # target: str = None
+
+    def __post_init__(self):
+        self.hosh = self.parent.hosh[self.index : self.n]
 
     @property
     def value(self):
         from hdict.content.entry import Unevaluated
 
-        if self._value is Unevaluated:
+        if isinstance(self._value, Unevaluated):
             value = self.parent.value
             if isinstance(value, (list, tuple)):
                 if len(value) < self.n:  # pragma: no cover
                     raise Exception(f"Number of output fields ('{self.n}') should not exceed number of resulting list elements ('{len(value)}').")
                 self._value = value[self.index]
             elif isinstance(value, dict):
                 if len(value) != self.n:  # pragma: no cover
@@ -58,8 +69,9 @@
             else:  # pragma: no cover
                 raise Exception(f"Cannot infer subvalue '{self.index}' of type '{type(value).__name__} {value}.")
         return self._value
 
     def __repr__(self):
         if self.isevaluated:
             return repr(self._value)
+        # t = self.parent if self.target is None else self.target
         return f"{self.parent}→{str(self.index if self.source is None else self.source)}"
```

### Comparing `hdict-0.230408.2/src/hdict/content/value.py` & `hdict-0.230412.1/src/hdict/content/value.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
 from hosh import Hosh
 
 from hdict.content.argument import AbsBaseArgument
 from hdict.content.entry import AbsEntry
-from hdict.hoshfication import v2hosh
+from hdict.content.aux_value import v2hosh
 
 
 class value(AbsBaseArgument, AbsEntry):
     """
     Wrapper for any Python object except AbsAny instances
 
     >>> x = 5
```

### Comparing `hdict-0.230408.2/src/hdict/customjson.py` & `hdict-0.230412.1/src/hdict/text/customjson.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,16 @@
             }
         },
         _id: VRlid5klewaC1bro7soJEr8Ynmt-N9YCNjW8iPN0,
         _ids: {
             d: fBb9FHVYpHC7vyM-B8UrXuN4oCcQ4Y7pnQ6oSK3J,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             ell: P1oPe-8hTjTdV6gKov4oIQnmTUXyD2fU6E7C8MS6,
-            df: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb
+            df: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb,
+            df_: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb
         }
     }
     >>> from numpy import array
     >>> hdict(b=b, z=9, c=(c:=array([1,2,3])), d=Series(c), dd=array([[1, 2], [3, 4]])).show(colored=False)
     {
         b: {
             d: {
@@ -111,15 +112,16 @@
                 }
             },
             _id: VRlid5klewaC1bro7soJEr8Ynmt-N9YCNjW8iPN0,
             _ids: {
                 d: fBb9FHVYpHC7vyM-B8UrXuN4oCcQ4Y7pnQ6oSK3J,
                 y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
                 ell: P1oPe-8hTjTdV6gKov4oIQnmTUXyD2fU6E7C8MS6,
-                df: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb
+                df: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb,
+                df_: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb
             }
         },
         z: 9,
         c: "‹[1 2 3]›",
         d: "‹{0: 1, 1: 2, 2: 3}›",
         dd: "‹[[1 2] [3 4]]›",
         _id: 75i4qCm0ZAOdRV9TWDeUNQ7GuGmWWMQ8dndlVEsm,
@@ -141,33 +143,32 @@
         _ids: {
             s: kDsYXHYuZJ9o7GXZLx6lYu0GpEqyrCmBpt0xoy60,
             t: kDsYXHYuZJ9o7GXZLx6lYu0GpEqyrCmBpt0xoy60,
             u: kDsYXHYuZJ9o7GXZLx6lYu0GpEqyrCmBpt0xoy60,
             v: kDsYXHYuZJ9o7GXZLx6lYu0GpEqyrCmBpt0xoy60
         }
     }
+    >>> str(hdict(s={1,3,2}, t={3,1,2}, u={2,1,3}, v={2,1,3}))
+    '{s: "{1, 2, 3}", t: "{1, 2, 3}", u: "{1, 2, 3}", v: "{1, 2, 3}"}'
     """
 
     width = 200
 
     def default(self, obj):
         if obj is not None:
             # from hoshmap import FrozenIdict, Idict
             # if isinstance(obj, Idict):
             #     return obj.frozen.asdicts
             # if isinstance(obj, FrozenIdict):
             #     return obj.asdicts
             if obj is Ellipsis:
                 return "..."
             if isinstance(obj, AbsEntry) and obj.isevaluated:
-                # from hoshmap import FrozenIdict, Idict
-                # if isinstance(obj.value, Idict):
-                #     return obj.value.frozen.asdicts
-                # if isinstance(obj.value, FrozenIdict):
-                #     return obj.value.asdicts
+                if isinstance(obj.value, dict):
+                    return obj.value.asdicts_noid
                 return obj.value
             # if isinstance(obj, FunctionType):
             #     return str(obj)
             if not isinstance(obj, (dict, list, str, int, float, bytearray, bool)):
                 if type(obj).__name__ in ["DataFrame", "Series"]:
                     # ‹str()› is to avoid nested identation
                     return f"‹{truncate(str(obj.to_dict()), self.width)}›"
```

### Comparing `hdict-0.230408.2/src/hdict/data/dataset.py` & `hdict-0.230412.1/src/hdict/dataset/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #  time spent here.
 #
 
 # library arff2pandas simply disappeared...
 import re
 
 
-def isplit(source, sep=None, regex=False):
+def isplit(source, sep=None, regex=False):  # pragma: no cover
     """
     https://stackoverflow.com/a/9773142/9681577
 
     generator version of str.split()
 
     :param source:
         source string (unicode or bytes)
@@ -39,15 +39,15 @@
 
     :param regex:
         if True, will treat sep as regular expression.
 
     :returns:
         generator yielding elements of string.
     """
-    if sep is None:
+    if sep is None:  # pragma: no cover
         # mimic default python behavior
         source = source.strip()
         sep = "\\s+"
         if isinstance(source, bytes):
             sep = sep.encode("ascii")
         regex = True
     if regex:
@@ -99,51 +99,50 @@
 def loads(s):
     import arff as liacarff
 
     data = liacarff.loads(s)
     return liac2pandas(data)
 
 
-def df2liac(df, relation="data", description=""):
+def df2liac(df, relation="data", description=""):  # pragma: no cover
     attrs = []
     for col in df.columns:
         attr = col.split("@")
         if attr[1].count("{") > 0 and attr[1].count("}") > 0:
             vals = attr[1].replace("{", "").replace("}", "").split(",")
             attrs.append((attr[0], vals))
         else:
             attrs.append((attr[0], attr[1]))
 
     data = list(df.values)
     result = {"attributes": attrs, "data": data, "description": description, "relation": relation}
     return result
 
 
-def dump(df, fp):
-    import arff as liacarff
-
-    arff = df2liac(df)
-    liacarff.dump(arff, fp)
-
-
-def dumps(df):
-    import arff as liacarff
-
-    arff = df2liac(df)
-    return liacarff.dumps(arff)
+# def dump(df, fp):  # TODO: save arff/CSV from hdict
+#     import arff as liacarff
+#
+#     arff = df2liac(df)
+#     liacarff.dump(arff, fp)
+#
+#
+# def dumps(df):  # TODO: output arff/CSV from hdict
+#     import arff as liacarff
+#
+#     arff = df2liac(df)
+#     return liacarff.dumps(arff)
 
 
-def df2Xy(input="df", Xout="X", yout="y", **kwargs):
+def df2Xy(df):
     from sklearn.preprocessing import LabelEncoder
 
     le = LabelEncoder()
-    df = kwargs[input]
     X_ = df.drop(df.columns[[-1]], axis=1)
     y_ = le.fit_transform(df[df.columns[-1]])
-    return {Xout: X_, yout: y_, "_history": ...}
+    return {"X": X_, "y": y_}
 
 
 #
 #
 # def df2arff(input="df", output="arff", **kwargs):
 #     """
 #     >>> from idict import let, idict
@@ -200,45 +199,7 @@
 #     """
 #     from sklearn.datasets import fetch_openml
 #
 #     X, y = fetch_openml(name=name, version=version, as_frame=True, return_X_y=True)
 #     return {Xout: X, yout: y, "_history": ...}
 #
 #
-# def arff2df(input="arff", output="df", **kwargs):
-#     r"""
-#     >>> from idict import let, idict
-#     >>> d = idict.fromminiarff(output=["arff"], output_format="arff")
-#     >>> d.arff
-#     '@RELATION mini\n@ATTRIBUTE attr1\tREAL\n@ATTRIBUTE attr2 \tREAL\n@ATTRIBUTE class \t{0,1}\n@DATA\n5.1,3.5,0\n3.1,4.5,1'
-#     >>> d >>= arff2df  # doctest: +SKIP
-#     >>> d.show(colored=False)    # doctest: +SKIP +ELLIPSIS
-#     {
-#         "df": "→(input output arff)",
-#         "_name": "→(input output arff)",
-#         "_history": "idict---------arff2pandas-1.0.1--arff2df",
-#         "arff": "@RELATION mini\n@ATTRIBUTE attr1\tREAL\n@ATTRIBUTE attr2 \tREAL\n@ATTRIBUTE class \t{0,1}\n@DATA\n5.1,3.5,0\n3.1,4.5,1",
-#         "_id": "XraBH1sOCC.9ohqV3hfIRTE5FV3.0.1--arff2df",
-#         "_ids": {
-#             "df": "VNy1otmyPSLXWCKAYbZRtNqMdW3.0.1--arff2df",
-#             "_name": "K4gZ2YDXBHOHwPzYufHChxkfhSz7ZAr--YbuHM-o",
-#             "_history": "VaU.REn8zFBQtEWngL.FYvWCowT0aeZPmXg35hCs",
-#             "arff": "Z._c3e2b235b697e9734b9ec13084129dc30e45b (content: Ev_8bb973161e5ae900c5743b3c332b4a64d1955)"
-#         }
-#     }
-#     >>> d.df   # doctest: +SKIP
-#        attr1@REAL  attr2@REAL class@{0,1}
-#     0         5.1         3.5           0
-#     1         3.1         4.5           1
-#     """
-#     relation = "<Unnamed>"
-#     with StringIO() as f:
-#         f.write(kwargs[input])
-#         text = f.getvalue()
-#         df = loads(text)
-#         for line in isplit(text, "\n"):
-#             if line[:9].upper() == "@RELATION":
-#                 relation = line[9:].strip()
-#                 break
-#
-#     return {output: df, "_name": relation, "_history": ...}
-#
```

### Comparing `hdict-0.230408.2/src/hdict/data/load.py` & `hdict-0.230412.1/src/hdict/persistence/stored.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2021. Davi Pereira dos Santos
+#  Copyright (c) 2023. Davi Pereira dos Santos
 #  This file is part of the hdict project.
 #  Please respect the license - more about this in the section (*) below.
 #
 #  hdict is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
@@ -16,27 +16,18 @@
 #  along with hdict.  If not, see <http://www.gnu.org/licenses/>.
 #
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
-from hdict.data.dataset import load
+from dataclasses import dataclass
 
+from hdict.abs import AbsAny
 
-def file2df(name):
-    if name.endswith(".arff"):
-        relation = None
-        with open(name) as f:
-            for line in f:
-                if line[:9].upper() == "@RELATION":
-                    relation = line[9:-1]
-                    break
-        with open(name) as f:
-            df = load(f)
-        return df, relation or name
-    elif name.endswith(".csv"):
-        from pandas import read_csv
 
-        return read_csv(name), name
-    else:  # pragma: no cover
-        raise Exception(f"Unknown extension {name.split('.')[-1]}.")
+@dataclass
+class Stored(AbsAny):
+    content: object
+
+    def __post_init__(self):
+        self.kind = type(self.content)
```

### Comparing `hdict-0.230408.2/src/hdict/empty_.py` & `hdict-0.230412.1/src/hdict/data/empty_.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
 
 from hdict.content.argument.field import field
 from hdict.content.argument.sample import sample
-from hdict.frozenhdict import frozenhdict
+from hdict.data.frozenhdict import frozenhdict
 
 
 class Empty_(frozenhdict):
     """
     >>> from hdict import _
     >>> d = _ >> {"x": 5} >> dict(y=7)
     >>> type(_), type(d)
@@ -38,20 +38,30 @@
         y: 7,
         _id: A0G3Y7KNMLihDvpSJ3tB.zxshc6u1CbbiiYjCAAA,
         _ids: {
             x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf
         }
     }
+    >>> str(_ * {})
+    '⦑{} » {}⦒'
     """
 
     def __getattr__(self, item):
         return field(item)
 
     def __getitem__(self, item):
         return sample(*item)
 
     def __rshift__(self, other):
         res = super().__rshift__(other)
-        if res is NotImplemented:
+        if res is NotImplemented:  # pragma: no cover
+            return res
+        if isinstance(res, frozenhdict):
+            res = res.unfrozen
+        return res
+
+    def __mul__(self, other):
+        res = super().__mul__(other)
+        if res is NotImplemented:  # pragma: no cover
             return res
         return res.unfrozen
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hdict-0.230408.2/src/hdict/expr.py` & `hdict-0.230412.1/src/hdict/expression/expr.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,118 @@
 from functools import reduce
-from itertools import chain
 from operator import rshift
 from random import Random
 
 from hdict.abs import AbsAny
+from hdict.expression.step.step import AbsStep
 
 
-class Expr(AbsAny):
+class Expr(AbsStep):
     """
-    Expressions enable the creation of pipelines of steps
+    Expressions enable the creation of pipelines of steps (or nested expressions)
 
     Pipelines should be sampled or fed a hdict to become a resulting hdict.
+
+    >>> from hdict import hdict
+    >>> from hdict.expression.expr import Expr
+    >>> e = Expr() >> hdict()
+    >>> e.show(colored=False)
+    ⦑{
+        _id: 0000000000000000000000000000000000000000,
+        _ids: {}
+    }⦒
+    >>> e = Expr() >> dict()
+    >>> e.show(colored=False)
+    ⦑{}⦒
     """
 
     def __init__(self, *steps):
         self.steps = steps
 
     def sample(self, rnd: int | Random = None, solve=True):
         from hdict.content.argument import AbsArgument
-        from hdict.applyout import ApplyOut
+        from hdict.expression.step.applyout import ApplyOut
+        from hdict import cache, hdict
+        from hdict.expression.step.edict import EDict
 
         lst = []
         for step in self:
             match step:
                 case AbsArgument() | ApplyOut():
                     lst.append(step.sample(rnd))
-                case AbsAny():
-                    raise Exception(f"{type(step)}")
-                case dict():
-                    dct = step.copy()
+                case cache():
+                    lst.append(step)
+                case EDict():
+                    dct = step.dct.copy()
                     for k, v in dct.items():
                         if isinstance(v, AbsArgument):
                             dct[k] = dct[k].sample(rnd)
-                    lst.append(dct)
-                case _:
+                    lst.append(EDict(dct))
+                case AbsAny():  # pragma: no cover
+                    raise Exception(f"{type(step)}")
+                case _:  # pragma: no cover
                     raise Exception(f"")
         expr = Expr.fromiter(lst)
         return expr.solve() if solve else expr
 
     def __invert__(self):
         return self.sample()
 
     @staticmethod
     def fromiter(lst):
         new = Expr()
         new.steps = lst
         return new
 
     def solve(self):
-        return reduce(rshift, self)
+        from hdict.expression.step.edict import EDict
 
-    def roperate(self, left, solve):
-        from hdict import hdict, frozenhdict
-
-        match left:
-            case hdict() | frozenhdict():
-                expr = Expr(left, self)
-            case dict():
-                expr = Expr(hdict(left), self)
-            case _:
-                return NotImplemented  # pragma: no cover
-        return expr.solve() if solve else expr
+        gen = (step.dct if isinstance(step, EDict) else step for step in self)
+        return reduce(rshift, gen)
 
-    def __rrshift__(self, left):
-        return self.roperate(left, True)
+    @property
+    def unfrozen(self):
+        from hdict import frozenhdict
 
-    def __rmul__(self, left):
-        return self.roperate(left, False)
+        gen = (step.unfrozen if isinstance(step, frozenhdict) else step for step in self)
+        return Expr.fromiter(gen)
 
     def __iter__(self):
         for step in self.steps:
             if isinstance(step, Expr):
                 yield from step
             else:
                 yield step
 
-    def __repr__(self):
-        return " » ".join(repr(step) for step in self)
-
-    def __str__(self):
-        out = []
-        for step in self:
-            out.append(str(step))
-        return " » ".join(out)
-
     def show(self, colored=True, key_quotes=False):
         r"""Print textual representation of an expression"""
         print(self.astext(colored, key_quotes))
 
     def astext(self, colored=True, key_quotes=False):
         r"""
         Textual representation of an expression
 
         >>> p = Expr({"b":2}, {"a":1})
         >>> p
-        {'b': 2} » {'a': 1}
+        ⦑{'b': 2} » {'a': 1}⦒
         >>> p.show()
-        {'b': 2} » {'a': 1}
+        ⦑{'b': 2} » {'a': 1}⦒
         """
-        from hdict.frozenhdict import frozenhdict
+        from hdict.data.frozenhdict import frozenhdict
         from hdict import hdict
 
         out = []
         for step in self:
             if isinstance(step, (frozenhdict, hdict)):
                 out.append(step.astext(colored=colored, key_quotes=key_quotes))
             else:
                 out.append(repr(step))
-        return " » ".join(out)
+        return "⦑" + " » ".join(out) + "⦒"
+
+    def __repr__(self):
+        return "⦑" + " » ".join(repr(step) for step in self) + "⦒"
+
+    def __str__(self):
+        out = []
+        for step in self:
+            out.append(str(step))
+        return "⦑" + " » ".join(out) + "⦒"
```

### Comparing `hdict-0.230408.2/src/hdict/frozenhdict.py` & `hdict-0.230412.1/src/hdict/data/frozenhdict.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,29 +20,31 @@
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
 
 import json
 import re
 from collections import UserDict
+from io import StringIO
 from typing import TypeVar, Union
 
-from hdict.content.entry import AbsEntry
-from hdict.customjson import CustomJSONEncoder, stringfy
+from hdict.dataset.dataset import loads, isplit
+from hdict.dataset.pandas_handling import file2df
+from hdict.text.customjson import CustomJSONEncoder, stringfy
 
 VT = TypeVar("VT")
 
 
 class frozenhdict(UserDict, dict[str, VT]):
     """
     Immutable hdict.
 
     Any nested 'hdict' value will be frozen to avoid inconsistency between the hdict id (inner id) and the frozenhdict id (outer id).
 
-    >>> from hdict.frozenhdict import frozenhdict
+    >>> from hdict import frozenhdict
     >>> d = frozenhdict({"x": 3}, y=5)
     >>> from hosh._internals_appearance import decolorize
     >>> print(decolorize(repr(d)))  # This is equivalent to just 'd', without colors.
     {
         x: 3,
         y: 5,
         _id: r5A2Mh6vRRO5rxi5nfXv1myeguGSTmqHuHev38qM,
@@ -52,25 +54,25 @@
         }
     }
     >>> d.data
     {'x': 3, 'y': 5}
     >>> from hdict import _, apply
     >>> d *= apply(lambda v, x: v - x).z
     >>> str(d)
-    '{x: 3, y: 5} » z=λ(v x)'
+    '⦑{x: 3, y: 5} » z=λ(v x)⦒'
     >>> d.show(colored=False)
-    {
+    ⦑{
         x: 3,
         y: 5,
         _id: r5A2Mh6vRRO5rxi5nfXv1myeguGSTmqHuHev38qM,
         _ids: {
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2
         }
-    } » z=λ(v x)
+    } » z=λ(v x)⦒
     >>> d = {"v": 7} * d
     >>> d.solve().show(colored=False)
     {
         v: 7,
         x: 3,
         y: 5,
         z: λ(v x),
@@ -110,59 +112,107 @@
             a: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             v: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             z: .beBfajsUjKto9qdBCKsLmBgsaNPpJiyz24P9.qg
         }
     }
+    >>> from hdict.content.entry import AbsEntry, Unevaluated
+    >>> from hdict import frozenhdict
     """
 
     _evaluated = None
     _asdict, _asdicts, _asdicts_noid = None, None, None
 
     # noinspection PyMissingConstructor
     def __init__(self, /, _dictionary=None, _previous=None, **kwargs):
         from hdict.content.entry import AbsEntry
-        from hdict.aux_frozendict import handle_identity
-        from hdict.aux_frozendict import handle_items
+        from hdict.data.aux_frozendict import handle_identity
+        from hdict.data.aux_frozendict import handle_items
 
         if _previous is None:
             _previous = {}
 
         # TODO: check if _dictionary keys is 'str'; regex to check if k is an identifier;
         data = _dictionary or {}
         # REMINDER: Inside data, the only 'dict' entries are "_id" and "_ids", the rest are AbsEntry objects.
         self.data: dict[str, AbsEntry | str | dict[str, str]]
         self.data = handle_items(data, kwargs, previous=_previous)
         self.hosh, self.ids = handle_identity(self.data)
         self.id = self.hosh.id
+        self.raw = self.data
+
+    def __rmul__(self, left):
+        from hdict import frozenhdict
+        from hdict.expression.step.edict import EDict
+        from hdict.expression.expr import Expr
 
-    def __rrshift__(self, other):
         from hdict import hdict
 
-        if isinstance(other, dict) and not isinstance(other, (hdict, frozenhdict)):
-            return frozenhdict(other) >> self
+        if isinstance(left, dict) and not isinstance(left, (hdict, frozenhdict)):
+            return Expr(EDict(left), self)
         return NotImplemented  # pragma: no cover
 
-    def __rshift__(self, other):
-        from hdict import hdict
-        from hdict.applyout import ApplyOut
+    def __mul__(self, other):
+        from hdict import hdict, frozenhdict
+        from hdict.expression.step.edict import EDict
+        from hdict.expression.expr import Expr
+        from hdict.expression.step.step import AbsStep
+
+        match other:
+            case AbsStep() | hdict() | frozenhdict():
+                return Expr(self, other)
+            case dict():
+                return Expr(self, EDict(other))
+            case _:  # pragma: no cover
+                return NotImplemented
 
-        # Merge keeping ids.
-        if isinstance(other, hdict):
-            other = other.frozen
-        if isinstance(other, frozenhdict):
-            other = other.data
-        if isinstance(other, ApplyOut):
-            other = {other.out: other.nested}
+    def __rrshift__(self, left):
+        from hdict import hdict
 
-        if isinstance(other, dict):
-            return frozenhdict(other, _previous=self.data)
+        if isinstance(left, dict) and not isinstance(left, (hdict, frozenhdict)):
+            return frozenhdict(left) >> self
         return NotImplemented  # pragma: no cover
 
+    def __rshift__(self, other):
+        # If merging, keep ids.
+        from hdict import hdict
+        from hdict.expression.step.applyout import ApplyOut
+        from hdict.expression.step.cache import cache
+        from hdict.content.entry.cached import Cached
+
+        from hdict.content.argument.apply import apply
+
+        if isinstance(other, apply):  # pragma: no cover
+            raise Exception(f"Cannot apply without specifying output(s).\n" f"Hint: d >> apply(f)('output_field1', 'output_field2')")
+        from hdict.content.argument import AbsArgument
+
+        if isinstance(other, AbsArgument):  # pragma: no cover
+            raise Exception(f"Cannot pipe {type(other).__name__} without specifying output.\n" f"Hint: d >> {'field name': object}\n" f"Hint: d['field name'] = object")
+
+        from hdict.expression.expr import Expr
+
+        match other:
+            case hdict() | frozenhdict():
+                dct = other.raw
+            case ApplyOut(nested, out):
+                dct = {out: nested}
+            case cache(storage=storage, fields=fields):
+                if not fields:
+                    fields = (k for k, v in self.raw.items() if not v.isevaluated)
+                dct = {k: Cached(self.ids[k], storage, self.raw[k]) for k in fields}
+            case dict():
+                dct = other
+            case Expr():
+                return Expr(self, other).solve()
+            case _:  # pragma: no cover
+                return NotImplemented
+
+        return frozenhdict(dct, _previous=self.data)
+
     def __getitem__(self, item):  # pragma: no cover
         return self.data[item].value
 
     def __getattr__(self, item):  # pragma: no cover
         if item in self.data:
             return self.data[item].value
         return self.__getattribute__(item)
@@ -185,14 +235,15 @@
             _id: bi5Qdbh-zgA1ZQdxGhxqjaKaQROtxk1VCPRZhMOq,
             _ids: {
                 x: 0123456789012345678901234567890123456789
             }
         }
         """
         from hdict.content.value import value
+        from hdict.content.entry import AbsEntry
 
         data = {}
         for k, v in dictionary.items():
             if isinstance(v, AbsEntry):
                 if k in ids and ids[k] != v.id:  # pragma: no cover
                     raise Exception(f"Conflicting ids provided for key '{k}': ival.id={v.id}; ids[{k}]={ids[k]}")
                 data[k] = v
@@ -284,14 +335,15 @@
                 dic[k] = v.asdicts_noid if isinstance(v, (hdict, frozenhdict)) else v
             self._asdicts_noid = dic
         return self._asdicts_noid
 
     @property
     def asdicts_hoshes_noneval(self):
         from hdict import value
+        from hdict.content.entry import AbsEntry
 
         hoshes = set()
         dic = {}
         for k, val in self.data.items():
             if isinstance(val, AbsEntry):
                 hoshes.add(val.hosh)
             if isinstance(val, value):
@@ -312,18 +364,23 @@
         r"""Textual representation of a frozenidict object"""
         dicts, hoshes = self.asdicts_hoshes_noneval
         txt = json.dumps(dicts, indent=4, ensure_ascii=False, cls=CustomJSONEncoder)
 
         # Put colors after json, to avoid escaping ansi codes.  TODO: check how HTML behaves here
         for h in hoshes:
             txt = txt.replace(f'"{h.id}"', repr(h)) if colored else txt.replace(f'"{h.id}"', h.id)
-        txt = re.sub(r'(": )"(λ.+?)"(?=,\n)', '": \\2', txt)
+
+        # Remove quotes.
+        txt = re.sub(r'(": )"(λ.+?)"(?=,\n)', '": \\2', txt)  # Closure
+        txt = re.sub(r'(": )"(·.+?)"(?=,\n)', '": \\2', txt)  # Wrapper
+        txt = re.sub(r'(": )"(↑↓ cached at `.+?·)"(?=,\n)', '": \\2', txt)  # cache
         if not key_quotes:
-            txt = re.sub(r'(?<!: )"([\-a-zA-Z0-9_ ]+?)"(?=: )', "\\1", txt)
-        return txt.replace('"§«§lazy', "").replace('lazy§«§"', "")
+            txt = re.sub(r'(?<!: )"([\-a-zA-Z0-9_ ]+?)"(?=: )', "\\1", txt)  # keys
+
+        return txt
 
     def show(self, colored=True, key_quotes=False):
         r"""Print textual representation of a frozenidict object"""
         print(self.astext(colored, key_quotes))
 
     def copy(self):  # pragma: no cover
         raise Exception("A FrozenIdict doesn't need copies")
@@ -357,118 +414,159 @@
 
     def items(self, evaluate=True):
         """Generator over field-value pairs"""
         for k, val in self.data.items():
             # if not k.startswith("_"):
             yield k, (val.value if evaluate else val)
 
-    def save(self, cache: dict):
+    def save(self, storage: dict):
         """
         Store an entire frozenidict
         """
+        from hdict.content.entry.cached import kindid
+        from hdict.persistence.stored import Stored
+
         data = {self.id: self.ids}
         for field, fid in self.ids.items():
             value = self[field]
-            if isinstance(value, frozenhdict):
-                value.save(cache)
+            if field.endswith("_"):
+                # TODO check existence of the counterpart
+                data[kindid(fid)] = str(type(value))
+            elif isinstance(value, frozenhdict):
+                value.save(storage)
             else:
-                data[fid] = value
-        cache.update(data)
+                data[fid] = Stored(value)
+        storage.update(data)
 
     @staticmethod
-    def load(id, cache: dict | list, lazy=True) -> Union["frozenhdict", None]:
+    def load(id, storage: dict, lazy=True) -> Union["frozenhdict", None]:
         """
         Fetch an entire frozenidict
         """
         if len(id) != 40:  # pragma: no cover
             raise Exception(f"id should have lenght of 40, not {len(id)}")
-        return frozenhdict.fetch(id, cache, lazy, ishdict=True)
+        return frozenhdict.fetch(id, storage, lazy, ishdict=True)
 
     @staticmethod
-    def fetch(id, cache, lazy=True, ishdict=False) -> Union["frozenhdict", None]:
+    def fetch(id: str, storage: dict, lazy=True, ishdict=False) -> Union["frozenhdict", None]:
         """
         Fetch a single entry
 
         When cache is a list, traverse it from the end (right item to the left item).
         """
-        from hdict.content.entry.lazy import Lazy
-
-        caches = cache if isinstance(cache, list) else [cache]
-        while id not in (cache := caches.pop()):
-            if not caches:
-                raise Exception(f"id '{id}' not found in the provided cache {cache.keys()}.")
-        obj = cache[id]
+        from hdict.content.entry.cached import Cached
+        from hdict.content.entry.cached import getkind
+        from hdict.data.aux_frozendict import handle_mirror
+        from hdict.persistence.stored import Stored
+
+        if id not in storage:
+            return None
+        obj = storage[id]
         if isinstance(obj, dict):
             ishdict = True  # Set to True, because now we have a nested frozenhdict
-        elif ishdict:
-            raise Exception(f"Wrong content for idict expected under id {id}: {type(obj)}.")
+        elif ishdict or not isinstance(obj, Stored):  # pragma: no cover
+            raise Exception(f"Wrong content for hdict expected under id {id}: {type(obj)}.")
 
         if ishdict:
             ids = obj
             data = {}
+            mirrored = set()
             for field, fid in ids.items():
-                data[field] = Lazy(fid, cache) if lazy else frozenhdict.fetch(fid, cache, lazy, False)
+                if field.endswith("_"):
+                    mirrored.add(field[:-1])
+                    continue
+                if lazy:
+                    data[field] = Cached(fid, storage)
+                else:
+                    obj = frozenhdict.fetch(fid, storage, lazy=False, ishdict=False)
+                    if obj is None:  # pragma: no cover
+                        print(storage.keys())
+                        raise Exception(f"Incomplete hdict: id '{id}' not found in the provided cache.")
+                    data[field] = obj
+            for field in mirrored:
+                obj = data[field]
+                kind = obj.kind if isinstance(obj, Cached) else getkind(storage, obj.hosh)
+                data[field + "_"] = handle_mirror(field, data, ids[field], kind)
             return frozenhdict.fromdict(data, ids)
-        return obj
+
+        return obj.content
+
+    @property
+    def asdf(self):
+        """
+        Represent hdict as a DataFrame if possible
+        """
+        from pandas import DataFrame
+
+        data = dict(self)
+        index = data.pop("index")
+        return DataFrame(data, index=index)
+
+    @staticmethod
+    def fromfile(name, fields=None, format="df", named=None):
+        r"""
+        Input format is defined by file extension: .arff, .csv
+        """
+        from hdict.data.aux_frozendict import handle_format
+
+        df, name = file2df(name)
+        return handle_format(format, fields, df, named and name)
+
+    @staticmethod
+    def fromtext(text: str, fields=None, format="df", named=None):
+        r"""
+        Input format is defined by file extension: .arff, .csv
+        """
+        from hdict import frozenhdict
+
+        if text.startswith("@"):
+            name = "<Unnamed>"
+            with StringIO() as f:
+                f.write(text)
+                text = f.getvalue()
+                df = loads(text)
+                for line in isplit(text, "\n"):
+                    if line[:9].upper() == "@RELATION":
+                        name = line[9:].strip()
+                        break
+        else:
+            from testfixtures import TempDirectory
+
+            with TempDirectory() as tmp:
+                tmp.write(
+                    "temp.csv",
+                    text.encode(),
+                )
+                return frozenhdict.fromfile(tmp.path + "/temp.csv", fields, format, named)
+
+        from hdict.data.aux_frozendict import handle_format
+
+        return handle_format(format, fields, df, named and name)
 
     def __eq__(self, other):
         if isinstance(other, dict):
             if "_id" in other:
                 return self.id == other["_id"]
             if list(self.keys()) != list(other.keys()):
                 return False
             from hdict import hdict
 
             if isinstance(other, (frozenhdict, hdict)):
                 return self.id == other.id
             return dict(self) == other
-        raise TypeError(f"Cannot compare {type(self).__name__} and {type(other).__name__}")  # pragma: no cover
+        return NotImplemented  # pragma: no cover
 
     def __ne__(self, other):
         return not (self == other)
 
     def __repr__(self):
         return self.astext()
 
     def __str__(self):
         return stringfy(self.data)
 
     def __iter__(self):
         for k in self.data:
-            # if not k.startswith("_"):
             yield k
 
     def __hash__(self):
         return hash(self.hosh)
-
-    def __mul__(self, other):
-        from hdict.expr import Expr
-
-        return Expr(self, other)
-
-    # def metakeys(self):
-    #     """Generator of keys which start with '_'"""
-    #     return (k for k in self.data if k.startswith("_") and k not in ["_id", "_ids"])
-    #
-    # def metavalues(self, evaluate=True):
-    #     """Generator of field values (keys don't start with '_')"""
-    #     return ((v.value if evaluate else v) for k, v in self.data.items() if k.startswith("_") and k not in ["_id", "_ids"])
-    #
-    # def metaitems(self, evaluate=True):
-    #     """Generator over field-value pairs"""
-    #     for k, ival in self.data.items():
-    #         if k.startswith("_") and k not in ["_id", "_ids"]:
-    #             yield k, (ival.value if evaluate else ival)
-    #
-    # def entries(self, evaluate=True):
-    #     """Iterator over all items"""
-    #     yield from self.items(evaluate)
-    #     yield from self.metaitems(evaluate)
-    #
-    # @cached_property
-    # def fields(self):
-    #     return list(self.keys())
-    #
-    # @cached_property
-    # def metafields(self):
-    #     """List of keys which start with '_'"""
-    #     return [k for k in self.data if k.startswith("_") and k not in ["_id", "_ids"]]
```

### Comparing `hdict-0.230408.2/src/hdict/hoshfication.py` & `hdict-0.230412.1/src/hdict/content/aux_value.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230408.2/setup.py` & `hdict-0.230412.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,31 +7,37 @@
 packages = \
 ['hdict',
  'hdict.abs',
  'hdict.content',
  'hdict.content.argument',
  'hdict.content.entry',
  'hdict.data',
- 'hdict.persistence']
+ 'hdict.dataset',
+ 'hdict.expression',
+ 'hdict.expression.step',
+ 'hdict.persistence',
+ 'hdict.text']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['hosh>=2.230205.2,<3.0.0', 'indexed>=1.3.0,<2.0.0', 'lange>=1.230203.2,<2.0.0']
 
 extras_require = \
-{'full': ['pandas>=1.5.2,<2.0.0',
+{'full': ['pandas>=2.0.0,<3.0.0',
           'shelchemy>=0.220906.3,<0.220907.0',
           'safeserializer>=0.230202.1,<0.230203.0',
-          'lz4>=4.3.2,<5.0.0']}
+          'lz4>=4.3.2,<5.0.0',
+          'scikit-learn>=1.2.2,<2.0.0',
+          'liac-arff>=2.5.0,<3.0.0']}
 
 setup_kwargs = {
     'name': 'hdict',
-    'version': '0.230408.2',
+    'version': '0.230412.1',
     'description': 'A versatile dictionary based on a novel paradigm useful for computing, caching, experiments, distributed data, among others.',
     'long_description': '![test](https://github.com/davips/hdict/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hdict)\n<a href="https://pypi.org/project/hdict">\n<img src="https://img.shields.io/pypi/v/hdict.svg?label=release&color=blue&style=flat-square" alt="pypi">\n</a>\n![Python version](https://img.shields.io/badge/python-3.10...-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n<!--- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845) --->\n[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/hdict)\n[![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hdict)](https://pepy.tech/project/hdict)\n\n# hdict { A _unique_ data structure }\n[Website](https://hosh.page) | \n[Latest Release](https://pypi.org/project/hdict) |\n[Current Code](https://github.com/davips/hdict) |\n[API Documentation](https://davips.github.io/hdict)\n\nPlease see the [website](https://hosh.page) for more detailed usage information.\n\n## Overview\n**Shortly**: A data structure based on a novel identification paradigm useful for frictionless computing, experiments, distributed data, among others.\n\n**Formally**: Hosh-based cacheable lazy dict with predictable/deterministic universally (probabilistically guaranteed) unique identifiers.\n\n\n### Context\n\n  * [hosh](https://pypi.org/project/hosh): identification engine at the core of `hdict`\n  * previous projects: [hoshmap](https://pypi.org/project/hoshmap), [idict](https://pypi.org/project/idict), [ldict](https://pypi.org/project/ldict), [garoupa](https://pypi.org/project/garoupa)\n\n### The concept\n\n`hdict` is like an ordinary `dict` with `str` keys. \nEach entry, called _field_, and the `hdict` itself, are identified by 40-digit hashes (see [hosh](https://pypi.org/project/hosh)).\nA `hdict` object (say `d`) provides two extra entries: `_id` (hdict identifier) and `_ids` (field identifiers),\naccessible through square brackets or through the shortcuts `d.id` and `d.ids`.\n\n**`hdict` creation**\n<details>\n<p>\n\n```python3\nfrom hdict import hdict\n\n# From named arguments.\nd = hdict(x=5, y=7, z=10)\n\n# From a dict object.\nd = hdict({"x": 5, "y": 7, "z": 10})\n\n# From an empty \'hdict\' object.\nd = hdict() >> {"x": 5} >> {"y": 7, "z": 10}\n\n# All three options have the same result.\nd.show(colored=False)\n"""\n{\n    x: 5,\n    y: 7,\n    z: 10,\n    _id: BN-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn,\n    _ids: {\n        x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,\n        y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,\n        z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m\n    }\n}\n"""\n```\n\n```python3\n\nfrom hosh import setup\n\n# For better integration within the documentation, we change the color theme.\nsetup(dark_theme=False)\n\nd.show(colored=False)\n\n"""\n{\n    x: 5,\n    y: 7,\n    z: 10,\n    _id: BN-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn,\n    _ids: {\n        x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,\n        y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,\n        z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m\n    }\n}\n"""\n```\n\n\n</p>\n</details>\n\nA field contains a value or a function application.\nA field pointing to an application is only evaluated on demand, i.e., lazily.\n\n<!-- ------------------------------------------------------------------------ \nValue objects can have custom identifiers as well, if provided whithin the entry `ids`. \nOtherwise, identifiers for functions and values will be calculated through blake3 hashing of their content.\nFor functions, the bytecode is used as content.\nFor this reason, such functions should be simple, with minimal external dependencies or\nwith their import statements inside the function body.\nThis decreases the odds of using two functions with identical local code (and, therefore, identical identifiers)\nperforming different calculations.\n\ntransformation steps done through the operator `>>`, which symbolizes the ordering of the steps.\n* **value insertion** - represented by dict-like objects\n* **function application** - represented by ordinary Python functions\n\nFunctions, `hdict`s, and values have a deterministic UUID\n(called _hosh_ - **o**perable **h**a**sh**). \nIdentifiers (hoshes) for `hdict`s and values are predictable through the\nmagic available [here](https://pypi.org/project/garoupa).\nAn `hdict` is completely defined by its key-value pairs so that\nit can be converted from/to a built-in `dict`.\n\n\n------------------------------------------------------------------------  -->\n\nPlease refer to our [website](https://hosh.page) for more examples.\n\n\n## Installation\n### ...as a standalone lib\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI...\npip install --upgrade pip\npip install -U hdict\n\n# use the flag \'full\' for extra functionality (recommended if working with persistence or some special values like DataFrames)\npip install -U hdict[full]\n\n# ...or, install from updated source code.\npip install git+https://github.com/davips/hdict\n```\n\n### ...from source\n```bash\ngit clone https://github.com/davips/hdict\ncd hdict\npoetry install\n\n# use the flag \'full\' for extra functionality (recommended if working with persistence or some special values like DataFrames)  \npoetry install -E full\n```\n\n## Examples\n\nPlease refer to our [website](https://hosh.page) for examples.\n\n\n\n## Development\n### Licensing\nThe initial license choosen is GPL. Please contact the developer for other licensing needs.\n\n### Versioning\nThe version is a has a meaningful calendar component (`minor=yymmdd`), but it is still compatible with semantic versioning.\nFor instance, the version `0.230215.1` means `major=0`, `minor=230215`, `micro/patch=1`.\nNotes:\n * While `major=0`, some compatibility breaking changes may occur.\n * From `major=1` onwards, compatibility breaking changes increment it, and update the minor version to reflect the release date.\n * New (non breaking) features update only the minor version to reflect the release date.\n * Bug fixes (including breaking ones) increment only the micro version.\n\n### Contributing\n#### Collaboration\nWe have ongoing research applying this tool to machine learning and clinical academic experiments.\nAlthough, the scope of application is broad as it encompasses software development in general.\nFeel free to contact us if you are interested in the project/concept or have a suggestion/interesting problem to be solved.\n\n#### Donation\nCurrently there are no established forms of donation.\nExpenses:\n  * Programming hours\n  * Support\n  * Custom features\n  * Domain name maintenance yearly costs\n\n### Acknowledgement\nThis work was based on a previous research supported by Fapesp under supervision of\nProf. André C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 – 2019/01735-0)\nuntil 2021-03-31.\n\nWe would like to thank the providers of free tools that make this project feasible:\n  * github for hosting the code repository freely\n  * Oracle for hosting the website freely\n  * Developers of Mint, XFCE, and GNU/Linux for the operating system\n  * JetBrains for Intellij IDEA Community Edition\n  * Developers of Python packages listed in our project.toml\n',
     'author': 'davips',
     'author_email': 'dpsabc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,47 +1,48 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['hdict', 'hdict.abs', 'hdict.content',
-'hdict.content.argument', 'hdict.content.entry', 'hdict.data',
-'hdict.persistence'] package_data = \ {'': ['*']} install_requires = \
-['hosh>=2.230205.2,<3.0.0', 'indexed>=1.3.0,<2.0.0',
-'lange>=1.230203.2,<2.0.0'] extras_require = \ {'full':
-['pandas>=1.5.2,<2.0.0', 'shelchemy>=0.220906.3,<0.220907.0',
-'safeserializer>=0.230202.1,<0.230203.0', 'lz4>=4.3.2,<5.0.0']} setup_kwargs =
-{ 'name': 'hdict', 'version': '0.230408.2', 'description': 'A versatile
-dictionary based on a novel paradigm useful for computing, caching,
-experiments, distributed data, among others.', 'long_description': '![test]
-(https://github.com/davips/hdict/workflows/test/badge.svg)\n[![codecov](https:/
-/codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)](https://codecov.io/
-gh/davips/hdict)\n\n[pypi]\n\n![Python version](https://img.shields.io/badge/
-python-3.10...-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/
-License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n\n[![arXiv]
-(https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)]
-(https://arxiv.org/abs/2109.06028)\n[![API documentation](https://
-img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/
-hdict)\n[![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)]
-(https://hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hdict)]
-(https://pepy.tech/project/hdict)\n\n# hdict { A _unique_ data structure }\n
-[Website](https://hosh.page) | \n[Latest Release](https://pypi.org/project/
-hdict) |\n[Current Code](https://github.com/davips/hdict) |\n[API
-Documentation](https://davips.github.io/hdict)\n\nPlease see the [website]
-(https://hosh.page) for more detailed usage information.\n\n##
-Overview\n**Shortly**: A data structure based on a novel identification
-paradigm useful for frictionless computing, experiments, distributed data,
-among others.\n\n**Formally**: Hosh-based cacheable lazy dict with predictable/
-deterministic universally (probabilistically guaranteed) unique
-identifiers.\n\n\n### Context\n\n * [hosh](https://pypi.org/project/hosh):
-identification engine at the core of `hdict`\n * previous projects: [hoshmap]
-(https://pypi.org/project/hoshmap), [idict](https://pypi.org/project/idict),
-[ldict](https://pypi.org/project/ldict), [garoupa](https://pypi.org/project/
-garoupa)\n\n### The concept\n\n`hdict` is like an ordinary `dict` with `str`
-keys. \nEach entry, called _field_, and the `hdict` itself, are identified by
-40-digit hashes (see [hosh](https://pypi.org/project/hosh)).\nA `hdict` object
-(say `d`) provides two extra entries: `_id` (hdict identifier) and `_ids`
-(field identifiers),\naccessible through square brackets or through the
-shortcuts `d.id` and `d.ids`.\n\n**`hdict` creation**\n\n
+'hdict.content.argument', 'hdict.content.entry', 'hdict.data', 'hdict.dataset',
+'hdict.expression', 'hdict.expression.step', 'hdict.persistence', 'hdict.text']
+package_data = \ {'': ['*']} install_requires = \ ['hosh>=2.230205.2,<3.0.0',
+'indexed>=1.3.0,<2.0.0', 'lange>=1.230203.2,<2.0.0'] extras_require = \
+{'full': ['pandas>=2.0.0,<3.0.0', 'shelchemy>=0.220906.3,<0.220907.0',
+'safeserializer>=0.230202.1,<0.230203.0', 'lz4>=4.3.2,<5.0.0', 'scikit-
+learn>=1.2.2,<2.0.0', 'liac-arff>=2.5.0,<3.0.0']} setup_kwargs = { 'name':
+'hdict', 'version': '0.230412.1', 'description': 'A versatile dictionary based
+on a novel paradigm useful for computing, caching, experiments, distributed
+data, among others.', 'long_description': '![test](https://github.com/davips/
+hdict/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/davips/
+hdict/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hdict)\n\n
+[pypi]\n\n![Python version](https://img.shields.io/badge/python-3.10...-
+blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-
+blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n\n[![arXiv](https://
+img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://
+arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/
+API-autogenerated-a030a0.svg)](https://davips.github.io/hdict)\n[![Manual]
+(https://img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://
+hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hdict)](https://
+pepy.tech/project/hdict)\n\n# hdict { A _unique_ data structure }\n[Website]
+(https://hosh.page) | \n[Latest Release](https://pypi.org/project/hdict) |\n
+[Current Code](https://github.com/davips/hdict) |\n[API Documentation](https://
+davips.github.io/hdict)\n\nPlease see the [website](https://hosh.page) for more
+detailed usage information.\n\n## Overview\n**Shortly**: A data structure based
+on a novel identification paradigm useful for frictionless computing,
+experiments, distributed data, among others.\n\n**Formally**: Hosh-based
+cacheable lazy dict with predictable/deterministic universally
+(probabilistically guaranteed) unique identifiers.\n\n\n### Context\n\n *
+[hosh](https://pypi.org/project/hosh): identification engine at the core of
+`hdict`\n * previous projects: [hoshmap](https://pypi.org/project/hoshmap),
+[idict](https://pypi.org/project/idict), [ldict](https://pypi.org/project/
+ldict), [garoupa](https://pypi.org/project/garoupa)\n\n### The
+concept\n\n`hdict` is like an ordinary `dict` with `str` keys. \nEach entry,
+called _field_, and the `hdict` itself, are identified by 40-digit hashes (see
+[hosh](https://pypi.org/project/hosh)).\nA `hdict` object (say `d`) provides
+two extra entries: `_id` (hdict identifier) and `_ids` (field
+identifiers),\naccessible through square brackets or through the shortcuts
+`d.id` and `d.ids`.\n\n**`hdict` creation**\n\n
 \n\n```python3\nfrom hdict import hdict\n\n# From named arguments.\nd = hdict
 (x=5, y=7, z=10)\n\n# From a dict object.\nd = hdict({"x": 5, "y": 7, "z":
 10})\n\n# From an empty \'hdict\' object.\nd = hdict() >> {"x": 5} >> {"y": 7,
 "z": 10}\n\n# All three options have the same result.\nd.show
 (colored=False)\n"""\n{\n x: 5,\n y: 7,\n z: 10,\n _id: BN-
 3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn,\n _ids: {\n x: ecvgo-
 CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,\n y: eJCW9jGsdZTD6-
```

### Comparing `hdict-0.230408.2/PKG-INFO` & `hdict-0.230412.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: hdict
-Version: 0.230408.2
+Version: 0.230412.1
 Summary: A versatile dictionary based on a novel paradigm useful for computing, caching, experiments, distributed data, among others.
 License: GPLv3
 Author: davips
 Author-email: dpsabc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: full
 Requires-Dist: hosh (>=2.230205.2,<3.0.0)
 Requires-Dist: indexed (>=1.3.0,<2.0.0)
 Requires-Dist: lange (>=1.230203.2,<2.0.0)
+Requires-Dist: liac-arff (>=2.5.0,<3.0.0) ; extra == "full"
 Requires-Dist: lz4 (>=4.3.2,<5.0.0) ; extra == "full"
-Requires-Dist: pandas (>=1.5.2,<2.0.0) ; extra == "full"
+Requires-Dist: pandas (>=2.0.0,<3.0.0) ; extra == "full"
 Requires-Dist: safeserializer (>=0.230202.1,<0.230203.0) ; extra == "full"
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0) ; extra == "full"
 Requires-Dist: shelchemy (>=0.220906.3,<0.220907.0) ; extra == "full"
 Description-Content-Type: text/markdown
 
 ![test](https://github.com/davips/hdict/workflows/test/badge.svg)
 [![codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hdict)
 <a href="https://pypi.org/project/hdict">
 <img src="https://img.shields.io/pypi/v/hdict.svg?label=release&color=blue&style=flat-square" alt="pypi">
```

#### html2text {}

```diff
@@ -1,23 +1,25 @@
-Metadata-Version: 2.1 Name: hdict Version: 0.230408.2 Summary: A versatile
+Metadata-Version: 2.1 Name: hdict Version: 0.230412.1 Summary: A versatile
 dictionary based on a novel paradigm useful for computing, caching,
 experiments, distributed data, among others. License: GPLv3 Author: davips
 Author-email: dpsabc@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: full Requires-Dist: hosh
 (>=2.230205.2,<3.0.0) Requires-Dist: indexed (>=1.3.0,<2.0.0) Requires-Dist:
-lange (>=1.230203.2,<2.0.0) Requires-Dist: lz4 (>=4.3.2,<5.0.0) ; extra ==
-"full" Requires-Dist: pandas (>=1.5.2,<2.0.0) ; extra == "full" Requires-Dist:
-safeserializer (>=0.230202.1,<0.230203.0) ; extra == "full" Requires-Dist:
-shelchemy (>=0.220906.3,<0.220907.0) ; extra == "full" Description-Content-
-Type: text/markdown ![test](https://github.com/davips/hdict/workflows/test/
-badge.svg) [![codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/
-badge.svg)](https://codecov.io/gh/davips/hdict) [pypi] ![Python version](https:
-//img.shields.io/badge/python-3.10...-blue.svg) [![license: GPL v3](https://
+lange (>=1.230203.2,<2.0.0) Requires-Dist: liac-arff (>=2.5.0,<3.0.0) ; extra
+== "full" Requires-Dist: lz4 (>=4.3.2,<5.0.0) ; extra == "full" Requires-Dist:
+pandas (>=2.0.0,<3.0.0) ; extra == "full" Requires-Dist: safeserializer
+(>=0.230202.1,<0.230203.0) ; extra == "full" Requires-Dist: scikit-learn
+(>=1.2.2,<2.0.0) ; extra == "full" Requires-Dist: shelchemy
+(>=0.220906.3,<0.220907.0) ; extra == "full" Description-Content-Type: text/
+markdown ![test](https://github.com/davips/hdict/workflows/test/badge.svg) [!
+[codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)]
+(https://codecov.io/gh/davips/hdict) [pypi] ![Python version](https://
+img.shields.io/badge/python-3.10...-blue.svg) [![license: GPL v3](https://
 img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
 3.0)  [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-
 b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) [![API
 documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)]
 (https://davips.github.io/hdict) [![Manual](https://img.shields.io/badge/
 manual-handcrafted-a030a0.svg)](https://hosh.page) [![Downloads](https://
 static.pepy.tech/badge/hdict)](https://pepy.tech/project/hdict) # hdict { A
```

