# Comparing `tmp/hdict-0.230211.1.tar.gz` & `tmp/hdict-0.230408.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdict-0.230211.1.tar", max compression
+gzip compressed data, was "hdict-0.230408.2.tar", max compression
```

## Comparing `hdict-0.230211.1.tar` & `hdict-0.230408.2.tar`

### file list

```diff
@@ -1,28 +1,36 @@
--rw-r--r--   0        0        0    35149 2022-12-26 01:24:40.000000 hdict-0.230211.1/LICENSE
--rw-r--r--   0        0        0     7464 2023-02-11 03:56:43.250754 hdict-0.230211.1/README.md
--rw-r--r--   0        0        0      888 2023-02-11 03:56:44.846779 hdict-0.230211.1/pyproject.toml
--rw-r--r--   0        0        0     2159 2023-02-11 03:52:30.506793 hdict-0.230211.1/src/hdict/__init__.py
--rw-r--r--   0        0        0     1512 2023-02-11 03:56:40.210706 hdict-0.230211.1/src/hdict/aux.py
--rw-r--r--   0        0        0     1059 2023-02-05 05:22:49.478479 hdict-0.230211.1/src/hdict/cache.py
--rw-r--r--   0        0        0       49 2023-02-10 08:27:44.147222 hdict-0.230211.1/src/hdict/content/__init__.py
--rw-r--r--   0        0        0     1035 2023-01-29 23:16:59.637251 hdict-0.230211.1/src/hdict/content/abs/__init__.py
--rw-r--r--   0        0        0     1637 2023-02-09 13:35:23.344817 hdict-0.230211.1/src/hdict/content/abs/abscloneable.py
--rw-r--r--   0        0        0     1262 2023-02-04 16:45:35.569809 hdict-0.230211.1/src/hdict/content/abs/abscontent.py
--rw-r--r--   0        0        0     1073 2023-02-05 05:22:49.478479 hdict-0.230211.1/src/hdict/content/abs/abssampleable.py
--rw-r--r--   0        0        0    11113 2023-02-10 14:48:15.656196 hdict-0.230211.1/src/hdict/content/apply.py
--rw-r--r--   0        0        0     2823 2023-02-11 03:56:40.210706 hdict-0.230211.1/src/hdict/content/applyout.py
--rw-r--r--   0        0        0     2182 2023-02-05 05:22:49.502479 hdict-0.230211.1/src/hdict/content/default.py
--rw-r--r--   0        0        0     4270 2023-02-11 01:47:38.152264 hdict-0.230211.1/src/hdict/content/field.py
--rw-r--r--   0        0        0    10925 2023-02-10 08:32:15.219087 hdict-0.230211.1/src/hdict/content/handling.py
--rw-r--r--   0        0        0     2356 2023-02-10 15:30:29.216349 hdict-0.230211.1/src/hdict/content/sample.py
--rw-r--r--   0        0        0     3704 2023-02-09 14:39:00.084804 hdict-0.230211.1/src/hdict/content/subcontent.py
--rw-r--r--   0        0        0     2085 2023-02-05 03:06:37.917960 hdict-0.230211.1/src/hdict/content/value.py
--rw-r--r--   0        0        0     7387 2023-02-11 00:10:43.735846 hdict-0.230211.1/src/hdict/customjson.py
--rw-r--r--   0        0        0    15323 2023-02-11 03:56:40.270707 hdict-0.230211.1/src/hdict/frozenhdict.py
--rw-r--r--   0        0        0    24842 2023-02-11 03:56:40.234707 hdict-0.230211.1/src/hdict/hdict_.py
--rw-r--r--   0        0        0     3855 2023-01-29 20:20:35.027416 hdict-0.230211.1/src/hdict/hoshfication.py
--rw-r--r--   0        0        0     1334 2023-01-29 00:09:41.512891 hdict-0.230211.1/src/hdict/indexeddict.py
--rw-r--r--   0        0        0     2309 2023-02-11 01:37:25.179690 hdict-0.230211.1/src/hdict/pandas_handling.py
--rw-r--r--   0        0        0     5886 2023-02-11 03:56:40.238707 hdict-0.230211.1/src/hdict/pipeline.py
--rw-r--r--   0        0        0     8624 1970-01-01 00:00:00.000000 hdict-0.230211.1/setup.py
--rw-r--r--   0        0        0     8186 1970-01-01 00:00:00.000000 hdict-0.230211.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-26 01:24:40.000000 hdict-0.230408.2/LICENSE
+-rw-r--r--   0        0        0     7464 2023-04-08 04:19:10.268200 hdict-0.230408.2/README.md
+-rw-r--r--   0        0        0     1177 2023-04-08 04:19:16.104278 hdict-0.230408.2/pyproject.toml
+-rw-r--r--   0        0        0    14147 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/__init__.py
+-rw-r--r--   0        0        0      223 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/abs/__init__.py
+-rw-r--r--   0        0        0     2506 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/applyout.py
+-rw-r--r--   0        0        0     3389 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/aux_frozendict.py
+-rw-r--r--   0        0        0        0 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/__init__.py
+-rw-r--r--   0        0        0      714 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/argument/__init__.py
+-rw-r--r--   0        0        0     9033 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/argument/apply.py
+-rw-r--r--   0        0        0     2862 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/argument/aux_apply.py
+-rw-r--r--   0        0        0     1463 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/argument/default.py
+-rw-r--r--   0        0        0     2162 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/argument/field.py
+-rw-r--r--   0        0        0     2328 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/argument/sample.py
+-rw-r--r--   0        0        0     2026 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/entry/__init__.py
+-rw-r--r--   0        0        0     1473 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/entry/aux_closure.py
+-rw-r--r--   0        0        0     3379 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/entry/closure.py
+-rw-r--r--   0        0        0      515 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/entry/lazy.py
+-rw-r--r--   0        0        0     2717 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/entry/subvalue.py
+-rw-r--r--   0        0        0     2249 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/content/value.py
+-rw-r--r--   0        0        0     7367 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/customjson.py
+-rw-r--r--   0        0        0        0 2023-03-19 02:22:28.761130 hdict-0.230408.2/src/hdict/data/__init__.py
+-rw-r--r--   0        0        0     8146 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/data/dataset.py
+-rw-r--r--   0        0        0     1619 2023-03-19 04:58:08.124551 hdict-0.230408.2/src/hdict/data/load.py
+-rw-r--r--   0        0        0     1909 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/empty_.py
+-rw-r--r--   0        0        0     3100 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/expr.py
+-rw-r--r--   0        0        0    16616 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/frozenhdict.py
+-rw-r--r--   0        0        0    16799 2023-04-08 04:16:53.238376 hdict-0.230408.2/src/hdict/hdict_.py
+-rw-r--r--   0        0        0     3855 2023-01-29 20:20:35.027416 hdict-0.230408.2/src/hdict/hoshfication.py
+-rw-r--r--   0        0        0     1334 2023-01-29 00:09:41.512891 hdict-0.230408.2/src/hdict/indexeddict.py
+-rw-r--r--   0        0        0     3956 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/multioutput.py
+-rw-r--r--   0        0        0     2311 2023-03-15 00:26:20.740920 hdict-0.230408.2/src/hdict/pandas_handling.py
+-rw-r--r--   0        0        0        0 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/persistence/__init__.py
+-rw-r--r--   0        0        0     1059 2023-04-08 04:05:25.273250 hdict-0.230408.2/src/hdict/persistence/cache.py
+-rw-r--r--   0        0        0     8836 1970-01-01 00:00:00.000000 hdict-0.230408.2/setup.py
+-rw-r--r--   0        0        0     8385 1970-01-01 00:00:00.000000 hdict-0.230408.2/PKG-INFO
```

### Comparing `hdict-0.230211.1/LICENSE` & `hdict-0.230408.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdict-0.230211.1/README.md` & `hdict-0.230408.2/README.md`

 * *Files identical despite different names*

### Comparing `hdict-0.230211.1/pyproject.toml` & `hdict-0.230408.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hdict"
-version = "0.230211.1"
+version = "0.230408.2"
 description = "A versatile dictionary based on a novel paradigm useful for computing, caching, experiments, distributed data, among others."
 authors = ["davips <dpsabc@gmail.com>"]
 license = "GPLv3"
 readme = 'README.md'
 packages = [
     { include = "hdict", from = "src" }
 ]
@@ -12,24 +12,31 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 indexed = "^1.3.0"  # indexed dict
 lange = "^1.230203.2"
 # Optional dependencies.
 pandas = { version = "^1.5.2", optional = true }
 hosh = "^2.230205.2"
+shelchemy = { version = "^0.220906.3", optional = true }
+safeserializer = { version = "^0.230202.1", optional = true }
+lz4 = { version = "^4.3.2", optional = true }
 
 [tool.poetry.extras]    #[tool.poetry.group.extras.dependencies]
-full = ["pandas"]
+full = ["pandas", "shelchemy", "safeserializer", "lz4"]
 
 [tool.poetry.group.dev.dependencies]
 autoreadme = "^0.2102.20"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 black = "^22.6.0"
 pdoc3 = "^0.10.0"
 pylint = "^2.7.4"
 ipython = "^8.9.0"
 pandas = "^1.5.3"
+arff = "^0.9"
+shelchemy = "^0.220906.5"
+safeserializer = "^0.230202.1"
+lz4 = "^4.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hdict-0.230211.1/src/hdict/__init__.py` & `hdict-0.230408.2/src/hdict/empty_.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,43 +16,42 @@
 #  along with hdict.  If not, see <http://www.gnu.org/licenses/>.
 #
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
-from types import NoneType
-from typing import Union
 
-from hosh import Hosh
-
-from hdict.content.apply import apply
-from hdict.content.default import default
-from hdict.content.field import field
-from hdict.content.sample import sample
-from hdict.content.value import value
+from hdict.content.argument.field import field
+from hdict.content.argument.sample import sample
 from hdict.frozenhdict import frozenhdict
-from hdict.hdict_ import hdict
-
 
-class _(frozenhdict):
-    Ø = frozenhdict()
 
-    def __call__(self, f_or_dictionary: Union[callable, "apply", field] = None, *applied_args, fhosh: Hosh = None, **kwargs):
-        if isinstance(f_or_dictionary, (NoneType, dict)):
-            if fhosh is not None:  # pragma: no cover
-                raise Exception(f"Cannot use '_()' as hdict constructor and provide 'fhosh' at the same time.")
-            if f_or_dictionary is None:
-                f_or_dictionary = kwargs
-                kwargs = {}
-            return hdict(f_or_dictionary, **kwargs)
-        return apply(f_or_dictionary, *applied_args, fhosh=fhosh, **kwargs)
+class Empty_(frozenhdict):
+    """
+    >>> from hdict import _
+    >>> d = _ >> {"x": 5} >> dict(y=7)
+    >>> type(_), type(d)
+    (<class 'hdict.Empty'>, <class 'hdict.hdict'>)
+    >>> d.show(colored=False)
+    {
+        x: 5,
+        y: 7,
+        _id: A0G3Y7KNMLihDvpSJ3tB.zxshc6u1CbbiiYjCAAA,
+        _ids: {
+            x: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
+            y: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf
+        }
+    }
+    """
 
     def __getattr__(self, item):
         return field(item)
 
     def __getitem__(self, item):
         return sample(*item)
 
-
-_ = _()
-Ø = _.Ø
+    def __rshift__(self, other):
+        res = super().__rshift__(other)
+        if res is NotImplemented:
+            return res
+        return res.unfrozen
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hdict-0.230211.1/src/hdict/cache.py` & `hdict-0.230408.2/src/hdict/persistence/cache.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230211.1/src/hdict/content/abs/__init__.py` & `hdict-0.230408.2/src/hdict/indexeddict.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,7 +16,21 @@
 #  along with hdict.  If not, see <http://www.gnu.org/licenses/>.
 #
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
+
+from indexed import IndexedOrderedDict
+
+
+class IndexedDict(IndexedOrderedDict):
+    """
+    Wrapper with a cleaner representation of IndexedOrderedDict.
+
+    >>> IndexedDict([('a', 'a'), ('b', 'b')])
+    {'a': 'a', 'b': 'b'}
+    """
+
+    def __repr__(self):
+        return repr(dict(self.items()))
```

### Comparing `hdict-0.230211.1/src/hdict/content/abs/abscloneable.py` & `hdict-0.230408.2/src/hdict/content/argument/default.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,32 +16,21 @@
 #  along with hdict.  If not, see <http://www.gnu.org/licenses/>.
 #
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
+from typing import Callable
 
-from abc import abstractmethod, ABC
+from hdict.abs import AbsAny
+from hdict.content.argument import AbsMetaArgument
 
-from hdict.content.abs.abscontent import AbsContent
 
+class default(AbsMetaArgument):
+    def __init__(self, value: object | Callable):
+        self.value = value
+        if isinstance(value, AbsAny):
+            raise Exception(f"Cannot use a `{type(value).__name__}` as a default function value.")
 
-class AbsCloneable(ABC, AbsContent):
-    _finished = False
-
-    @property
-    def finished(self):
-        return self._finished
-
-    @abstractmethod
-    def start_clone(self):
-        """
-        This enables frozendict construct to handle content dependencies without changing state of the original content objects.
-        Make a clone
-        """
-
-    @abstractmethod
-    def finish_clone(self, data, out, previous):
-        """
-        Update dependencies to point to already handled contents.
-        """
+    def __repr__(self):
+        return f"default({repr(self.value)})"
```

### Comparing `hdict-0.230211.1/src/hdict/content/abs/abscontent.py` & `hdict-0.230408.2/src/hdict/data/load.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2023. Davi Pereira dos Santos
+#  Copyright (c) 2021. Davi Pereira dos Santos
 #  This file is part of the hdict project.
 #  Please respect the license - more about this in the section (*) below.
 #
 #  hdict is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
@@ -16,22 +16,27 @@
 #  along with hdict.  If not, see <http://www.gnu.org/licenses/>.
 #
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
+from hdict.data.dataset import load
 
-from hosh import Hosh
 
+def file2df(name):
+    if name.endswith(".arff"):
+        relation = None
+        with open(name) as f:
+            for line in f:
+                if line[:9].upper() == "@RELATION":
+                    relation = line[9:-1]
+                    break
+        with open(name) as f:
+            df = load(f)
+        return df, relation or name
+    elif name.endswith(".csv"):
+        from pandas import read_csv
 
-class AbsContent:
-    value: object
-    hosh: Hosh
-    isevaluated: bool
-
-    @property
-    def id(self):  # pragma: no cover
-        return self.hosh.id
-
-    def evaluate(self):
-        _ = self.value
+        return read_csv(name), name
+    else:  # pragma: no cover
+        raise Exception(f"Unknown extension {name.split('.')[-1]}.")
```

### Comparing `hdict-0.230211.1/src/hdict/content/apply.py` & `hdict-0.230408.2/src/hdict/content/argument/apply.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,247 +16,204 @@
 #  along with hdict.  If not, see <http://www.gnu.org/licenses/>.
 #
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
+from __future__ import annotations
 
-from functools import reduce
 from inspect import isfunction
 from inspect import signature
 from itertools import chain
-from operator import mul
 from random import Random
-from typing import Union
 
-from hdict.content.abs.abscloneable import AbsCloneable
-from hdict.content.abs.abssampleable import AbsSampleable
-from hdict.content.field import field
-from hdict.content.handling import Unevaluated, handle_args
-from hdict.content.value import value
+from hosh import Hosh
+
+from hdict.content.argument import AbsBaseArgument, AbsArgument
+from hdict.content.argument.field import field
 from hdict.customjson import truncate
 from hdict.hoshfication import f2hosh
-from hosh import Hosh
-from hosh.misc import hoshes
 
 
-# TODO: discard dependencies after evaluation, to avoid wasted memory, e.g., even after the deps are deleted from hdict
-class apply(AbsCloneable, AbsSampleable):
+class apply(AbsBaseArgument):
     """
     Function application
 
-    Single output application can be defined through attribute: 'apply(f).my_output_field'.
+    Single output application is defined by attribute: 'apply(f).my_output_field'.
+    Multioutput application is defined by a call: 'apply(f)("output_field1", "output_field2")'.
 
-    >>> from hdict import apply
+    >>> from hdict import apply, value
     >>> f = lambda a, b: a**b
     >>> v = apply(f, 5, b=7)
     >>> v
     λ(5 7)
     >>> g = lambda x, y: x**y
-    >>> v.isevaluated
-    False
     >>> apply(g, y=value(7777), x=v)
     λ(x=λ(5 7) 7777)
 
     >>> v2 = apply(f, a=v, b=value(7))
     >>> v2
     λ(a=λ(5 7) 7)
-    >>> v.finish_clone({}, "", {})
-    >>> v.value, v2
-    (78125, λ(a=78125 7))
-    >>> v2.finish_clone({}, "", {})
-    >>> v2.value, v2
-    (17763568394002504646778106689453125, 17763568394002504646778106689453125)
+    >>> v.enclosure({}, "j").value
+    78125
+    >>> v2.enclosure({}, "j")
+    λ(a=λ(5 7) 7)
+    >>> v2.enclosure({}, "j").value
+    17763568394002504646778106689453125
 
     >>> f = lambda a,b, c=1,d=2,e=13: 0
     >>> apply(f).requirements
-    {'a': field('a'), 'b': field('b'), 'c': default(1), 'd': default(2), 'e': default(13)}
+    {'a': field(a), 'b': field(b), 'c': default(1), 'd': default(2), 'e': default(13)}
     >>> ap = apply(f,3)
     >>> ap.requirements
-    {'a': 3, 'b': field('b'), 'c': default(1), 'd': default(2), 'e': default(13)}
+    {'a': 3, 'b': field(b), 'c': default(1), 'd': default(2), 'e': default(13)}
     >>> ap
     λ(3 b c=default(1) d=default(2) e=default(13))
-    >>> ap.finish_clone({"b": value(77)}, "", {})
+    >>> ap.enclosure({"b": value(77)}, "j")
+    λ(3 b c=1 d=2 e=13)
     >>> ap
     λ(3 b c=default(1) d=default(2) e=default(13))
-    >>> from hdict.content.handling import handle_values
     >>> d = {"f": ap, "b": 5, "d": 1, "e": field("b")}
     >>> d
-    {'f': λ(3 b c=default(1) d=default(2) e=default(13)), 'b': 5, 'd': 1, 'e': field('b')}
-    >>> handle_values(d, {})
+    {'f': λ(3 b c=default(1) d=default(2) e=default(13)), 'b': 5, 'd': 1, 'e': field(b)}
+    >>> from hdict.aux_frozendict import handle_items
+    >>> handle_items(d, previous={"b": 5})
+    {'b': 5, 'f': λ(3 b c=1 d=2 e=13), 'd': 1, 'e': 5}
     >>> d
-    {'f': λ(3 b 1 d b), 'b': 5, 'd': 1, 'e': b}
+    {'f': λ(3 b c=default(1) d=default(2) e=default(13)), 'b': 5, 'd': 1, 'e': field(b)}
     >>> apply(f,3,4).requirements
     {'a': 3, 'b': 4, 'c': default(1), 'd': default(2), 'e': default(13)}
     >>> apply(f,3,4,5).requirements
     {'a': 3, 'b': 4, 'c': 5, 'd': default(2), 'e': default(13)}
     >>> apply(f,3,4,5,6).requirements
     {'a': 3, 'b': 4, 'c': 5, 'd': 6, 'e': default(13)}
     >>> apply(f,3,4,5,6,7).requirements
     {'a': 3, 'b': 4, 'c': 5, 'd': 6, 'e': 7}
     >>> apply(f,d=5).requirements
-    {'a': field('a'), 'b': field('b'), 'c': default(1), 'd': 5, 'e': default(13)}
+    {'a': field(a), 'b': field(b), 'c': default(1), 'd': 5, 'e': default(13)}
     >>> f = lambda a,b, *contentarg, c=1,d=2,e=13, **kwargs: 0
     >>> apply(f,3,4,5,6,7,8).requirements
     {'a': 3, 'b': 4, 'c': 5, 'd': 6, 'e': 7, _5: 8}
     >>> apply(f,x=3,e=4,d=5,c=6,b=7,a=8).requirements
     {'a': 8, 'b': 7, 'c': 6, 'd': 5, 'e': 4, 'x': 3}
     >>> apply(f,3,c=77,x=5).requirements
-    {'a': 3, 'b': field('b'), 'c': 77, 'd': default(2), 'e': default(13), 'x': 5}
+    {'a': 3, 'b': field(b), 'c': 77, 'd': default(2), 'e': default(13), 'x': 5}
     >>> apply(f,b=77,x=5).requirements
-    {'a': field('a'), 'b': 77, 'c': default(1), 'd': default(2), 'e': default(13), 'x': 5}
+    {'a': field(a), 'b': 77, 'c': default(1), 'd': default(2), 'e': default(13), 'x': 5}
     """
 
-    out = None
-    _value = Unevaluated
-    _hosh = None
+    _sampleable, isfield, _requirements = None, False, None
+
+    def __init__(self, appliable: callable | apply | field, *applied_args, fhosh: Hosh = None, _sampleable=None, **applied_kwargs):
+        from hdict.content.argument.aux_apply import handle_args
 
-    def __init__(self, f: Union[callable, "apply", field], *applied_args, fhosh: Hosh = None, **applied_kwargs):
-        self.f = f
+        self.appliable = appliable
         if isinstance(fhosh, str):  # pragma: no cover
             fhosh = Hosh.fromid(fhosh)
-        if isinstance(f, apply):  # "clone" mode
-            fun = f.fun
-            self.f = f.f
-            self.fhosh = f.fhosh
-            self.args = {k: req.start_clone() if isinstance(req, AbsCloneable) else req for k, req in f.args.items()}
-            self.kwargs = {k: req.start_clone() if isinstance(req, AbsCloneable) else req for k, req in f.kwargs.items()}
-            from hdict.content.default import default
-        elif isinstance(f, field):  # "function will be provided by hdict"-mode constrains 'applied_args'
+
+        if isinstance(appliable, apply):  # "clone" mode
+            self.fhosh = fhosh or appliable.fhosh
+            self.fargs, self.fkwargs = appliable.fargs.copy(), appliable.fkwargs.copy()
+            self.isfield = appliable.isfield
+            self._sampleable = appliable.sampleable if _sampleable is None else _sampleable
+            self.appliable = appliable.appliable
+        elif isinstance(appliable, field):
+            # TODO: o que era isso mesmo?::  "function will be provided by hdict"-mode constrains 'applied_args'
             self.fhosh = fhosh
-            fun = lambda *args, **kwargs: f.value(*args, **kwargs)
-            self.args, self.kwargs = handle_args(None, applied_args, applied_kwargs)
-        elif callable(fun := f):
-            if not isfunction(fun):  # "not function" means "custom callable"
-                if not hasattr(fun, "__call__"):  # pragma: no cover
-                    raise Exception(f"Cannot infer method to apply non custom callable type '{type(fun)}'.")
-                if not hasattr(fun, "hosh"):  # pragma: no cover
-                    raise Exception(f"Missing 'hosh' attribute while applying custom callable class '{type(fun)}'")
+            self.fargs, self.fkwargs = handle_args(None, applied_args, applied_kwargs)
+            self.isfield = True
+            self._sampleable = _sampleable
+        elif callable(appliable):
+            if not isfunction(appliable):  # "not function" means "custom callable"
+                if not hasattr(appliable, "__call__"):  # pragma: no cover
+                    raise Exception(f"Cannot infer method to apply non custom callable type '{type(appliable).__name__}'.")
+                if not hasattr(appliable, "hosh"):  # pragma: no cover
+                    raise Exception(f"Missing 'hosh' attribute while applying custom callable class '{type(appliable).__name__}'")
                 # noinspection PyUnresolvedReferences
-                sig = signature(fun.__call__)
-                self.fhosh = fhosh
+                sig = signature(appliable.__call__)
+                # noinspection PyUnresolvedReferences
+                self.fhosh = fhosh or appliable.hosh
             else:
-                self.fhosh = f2hosh(fun) if fhosh is None else fhosh
-                sig = signature(fun)
+                self.fhosh = f2hosh(appliable) if fhosh is None else fhosh
+                sig = signature(appliable)
 
             # Separate positional parameters from named parameters looking at 'f' signature.
-            self.args, self.kwargs = handle_args(sig, applied_args, applied_kwargs)
+            self.fargs, self.fkwargs = handle_args(sig, applied_args, applied_kwargs)
+            self._sampleable = _sampleable
         else:  # pragma: no cover
-            raise Exception(f"Cannot apply type '{type(f)}'.")
-        self._fun = fun
-        self.requirements = {k: v for k, v in sorted((self.args | self.kwargs).items())}
-        # Requirements (dependencies stub) are alphabetically sorted to ensure we keep the same resulting hosh no matter in which order the parameters are defined in the function.
-
-    @property
-    def ahosh(self):
-        return self.fhosh.rev  # 'f' identified as an appliable function
-
-    def start_clone(self):
-        if self.finished:  # pragma: no cover
-            raise Exception(f"Cannot clone a finished content.")
-        return apply(self)
-
-    def finish_clone(self, data, out, previous):
-        if self.finished:  # pragma: no cover
-            raise Exception(f"Cannot finish an application twice.")
-        if isinstance(self.f, apply):  # pragma: no cover
-            raise Exception(f"Why applying another apply object?")
-        if isinstance(self.f, AbsCloneable) and not self.f.finished:
-            self.f.finish_clone(data, out, previous)
-        if self.fhosh is None:
-            self.fhosh = self.f.hosh
-        reqs = self.requirements
-        for kreq, req in reqs.items():
-            if isinstance(req, field) and req.name == out:
-                if kreq not in previous:  # pragma: no cover
-                    raise Exception(f"Application at '{out}' depends on a previous '{out}' value, which does not exist.")
-                reqs[kreq] = previous[kreq]
-                if kreq in self.args:
-                    self.args[kreq] = previous[kreq]
-                elif kreq in self.kwargs:
-                    self.kwargs[kreq] = previous[kreq]
-            if isinstance(req, AbsCloneable) and not req.finished:
-                req.finish_clone(data, out, previous)
-        self._finished = True
-
-    @property
-    def hosh(self):
-        if not self.finished:  # pragma: no cover
-            from hdict import sample
-
-            if any(isinstance(x, sample) for x in self.requirements.values()):
-                raise Exception(f"Cannot know the identity of this hdict or apply object before sampling. Provided callable:", self.f)
-            raise Exception(f"Cannot know apply.hosh before finishing object apply. Provided callable:", self.f)
-        if self._hosh is None:
-            self._hosh = reduce(mul, chain(hoshes(self.requirements.values()), [self.ahosh]))
-        return self._hosh
+            raise Exception(f"Cannot apply type '{type(appliable).__name__}'.")
 
     @property
-    def value(self):
-        if self._value == Unevaluated:
-            if not self.finished:  # pragma: no cover
-                raise Exception(f"Cannot access apply.value before finishing object '{self.fhosh}'.")
-            args = (x.value for x in self.args.values())
-            kwargs = {k: v.value for k, v in self.kwargs.items()}
-            self._value = self._fun(*args, **kwargs)
-        return self._value
+    def sampleable(self):
+        if self._sampleable is None:
+            gen = (req.sampleable for req in self.fargs.values())
+            kwgen = (req.sampleable for req in self.fkwargs.values())
+            self._sampleable = any(gen) or any(kwgen)
+        return self._sampleable
 
     @property
-    def fun(self):
-        return self._fun
+    def ahosh(self):
+        return self.fhosh.rev  # 'f' identified as an appliable function
 
-    @property
-    def isevaluated(self):
-        return self._value != Unevaluated
+    def clone(self, _sampleable=None):
+        return apply(self, _sampleable=_sampleable)
 
     def sample(self, rnd: int | Random = None):
-        clone = self.start_clone()
-        args = clone.args
-        kwargs = clone.kwargs
-        reqs = clone.requirements
-        for k, v in args.items():
-            if isinstance(v, AbsSampleable):
-                args[k] = reqs[k] = v.sample(rnd)
-        for k, v in kwargs.items():
-            if isinstance(v, AbsSampleable):
-                kwargs[k] = reqs[k] = v.sample(rnd)
+        if not self.sampleable:
+            return self
+        clone = self.clone(_sampleable=False)
+        for k, v in clone.fargs.items():
+            clone.fargs[k] = v.sample(rnd)
+        for k, v in clone.fkwargs.items():
+            clone.fkwargs[k] = v.sample(rnd)
         return clone
 
+    def enclosure(self, data, key):
+        from hdict.content.entry.closure import Closure
+
+        return Closure(self, data, [key])
+
     def __call__(self, *out, **kwout):
-        from hdict.content.applyout import applyOut
+        from hdict.applyout import ApplyOut
 
         if out and kwout:  # pragma: no cover
-            raise Exception(f"Cannot mix translated and non translated outputs.")
+            raise Exception(f"Cannot mix translated (**kwargs) and non translated (*args) outputs.")
         if len(out) == 1:
             out = out[0]
-        return applyOut(self, out or tuple(kwout.items()))
+        return ApplyOut(self, out or tuple(kwout.items()))
 
     def __getattr__(self, item):
         # REMINDER: Work around getattribute missing all properties.
-        if item not in ["isevaluated", "fun", "value", "hosh", "ahosh"]:
-            from hdict.content.applyout import applyOut
+        if item not in ["ahosh", "requirements", "hosh"]:
+            from hdict.applyout import ApplyOut
 
-            return applyOut(self, item)
+            return ApplyOut(self, item)
         return self.__getattribute__(item)  # pragma: no cover
 
     def __rshift__(self, other):  # pragma: no cover
-        raise Exception(f"Cannot apply before specifying the output field.")
+        raise Exception(f"Cannot pipeline an application before specifying the output field.")
 
     def __rrshift__(self, other):  # pragma: no cover
         raise Exception(f"Cannot apply before specifying the output field.")
 
     def __repr__(self):
-        if not self.isevaluated:
-            from hdict.content.default import default
+        from hdict import value
 
-            lst = []
-            for param, content in self.requirements.items():
-                if isinstance(content, field):
-                    txt = content.name
-                elif isinstance(content, (apply, default)):
-                    txt = f"{param}={repr(content)}"
-                else:
-                    txt = truncate(repr(content), width=7)
-                lst.append(txt)
-            return f"λ({' '.join(lst)})"
-        return repr(self._value)
+        lst = []
+        for param, content in sorted(chain(self.fargs.items(), self.fkwargs.items())):
+            match content:
+                case field(name=param):
+                    lst.append(f"{param}")
+                case value():
+                    lst.append(truncate(repr(content), width=7))
+                case AbsArgument():
+                    lst.append(f"{param}={repr(content)}")
+                case _:
+                    raise Exception(f"")
+        return f"λ({' '.join(lst)})"
+
+    @property
+    def requirements(self):
+        if self._requirements is None:
+            self._requirements = {k: v for k, v in sorted(chain(self.fargs.items(), self.fkwargs.items()))}
+        return self._requirements
```

### Comparing `hdict-0.230211.1/src/hdict/content/sample.py` & `hdict-0.230408.2/src/hdict/content/argument/sample.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,47 +17,49 @@
 #
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
 
-from dataclasses import dataclass
-from math import inf
 from random import Random
 
 from lange.tricks import list2progression
 
-from hdict.content.abs.abscontent import AbsContent
-from hdict.content.abs.abssampleable import AbsSampleable
+from hdict.content.value import value
+from ..argument import AbsMetaArgument
 
 
-@dataclass
-class sample(AbsContent, AbsSampleable):
+class sample(AbsMetaArgument):
     """
+    A lazily evaluated list of values
+
     >>> (s := sample(1, 2, 3, ..., 9).values)
     [1 2 .+. 9]
     >>> (s := sample(2, 4, 8, ..., 1024).values)
     [2 4 .*. 1024]
     >>> (s := sample(2, -4, 8, ..., 12).values)
     [2 -4 8]
     """
 
+    sampleable = True
+
     def __init__(self, *values: list[int | float], rnd: int | Random = 0, maxdigits=28):
         self.rnd = rnd
-        # TODO: accept non numeric types (categoric)?
+        # TODO: accept list of non numeric types (categoric)?
         prog = list2progression(values, maxdigits=maxdigits)
         if prog.n.is_infinite():  # pragma: no cover
             raise Exception(f"Cannot sample from an infinite list: {prog}")
         self.values = prog
 
     def sample(self, rnd: int | Random = None):
-        from hdict.content.value import value
-
         if rnd is None:
             rnd = self.rnd
         if isinstance(rnd, int):
             rnd = Random(rnd)
         if not isinstance(rnd, Random):  # pragma: no cover
             raise Exception(f"Sampling needs an integer seed or a Random object.")
         idx = rnd.randint(0, self.values.n - 1)
         return value(self.values[idx])
+
+    def __repr__(self):
+        return f"~{self.values}"
```

### Comparing `hdict-0.230211.1/src/hdict/content/value.py` & `hdict-0.230408.2/src/hdict/content/value.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,44 +16,50 @@
 #  along with hdict.  If not, see <http://www.gnu.org/licenses/>.
 #
 #  (*) Removing authorship by any means, e.g. by distribution of derived
 #  works or verbatim, obfuscated, compiled or rewritten versions of any
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
+from hosh import Hosh
 
-from hdict.content.abs.abscontent import AbsContent
+from hdict.content.argument import AbsBaseArgument
+from hdict.content.entry import AbsEntry
 from hdict.hoshfication import v2hosh
-from hosh import Hosh
 
 
-class value(AbsContent):
+class value(AbsBaseArgument, AbsEntry):
     """
+    Wrapper for any Python object except AbsAny instances
+
     >>> x = 5
     >>> from hdict.content.value import value
     >>> v = value(x, "1234567890123456789012345678901234567890")
     >>> v
     5
     >>> v.hosh.id
     '1234567890123456789012345678901234567890'
 
     """
 
+    isevaluated = True
+
     def __init__(self, val: object, hosh: Hosh | str = None, hdict=None):
         """
 
         Args:
             val:
             hosh:
             hdict:  optional reference to the object if it has a hdict counterpart (e.g.: pandas DF)
         """
-        if isinstance(val, AbsContent):  # pragma: no cover
-            raise Exception(f"Cannot nest AbsContent object inside a 'value' object: '{type(val)}")
-        self.value = val
+        from hdict.abs import AbsAny
+
+        if isinstance(val, AbsAny):  # pragma: no cover
+            raise Exception(f"Cannot handle objects of type '{type(val).__name__}' as raw values for hdict.")
+        self.value = self._value = val
         if isinstance(hosh, str):
             hosh = Hosh.fromid(hosh)
         self.hosh = v2hosh(self.value) if hosh is None else hosh
         self.hdict = hdict
-        self.isevaluated = True
 
     def __repr__(self):
         return repr(self.value)
```

### Comparing `hdict-0.230211.1/src/hdict/customjson.py` & `hdict-0.230408.2/src/hdict/customjson.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
 import json
 import re
 from json import JSONEncoder
 
-from hdict.content.abs.abscontent import AbsContent
+from hdict.content.entry import AbsEntry
 
 
 class CustomJSONEncoder(JSONEncoder):
     """
     >>> from hdict import hdict
     >>> a = hdict(x=3)
     >>> hdict(d=a, y=5).show(colored=False)
@@ -49,77 +49,77 @@
     }
     >>> from pandas.core.frame import DataFrame, Series
     >>> df = DataFrame([[1,2],[3,4]])
     >>> df
        0  1
     0  1  2
     1  3  4
-    >>> b = hdict(d=a, y=5, df=df, ell=...)
+    >>> b = hdict(d=a, y=5, df_=df, ell=...)
     >>> b.show(colored=False)
     {
         d: {
             x: 3,
             _id: fBb9FHVYpHC7vyM-B8UrXuN4oCcQ4Y7pnQ6oSK3J,
             _ids: {
                 x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr
             }
         },
         y: 5,
-        df: "‹{0: {0: 1, 1: 3}, 1: {0: 2, 1: 4}}›",
+        df_: "‹{0: {0: 1, 1: 3}, 1: {0: 2, 1: 4}}›",
         ell: "...",
-        df_: {
+        df: {
             index: "‹{0: 0, 1: 1}›",
             0: "‹{0: 1, 1: 3}›",
             1: "‹{0: 2, 1: 4}›",
             _id: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb,
             _ids: {
                 index: DQa5yWRkGo-9FLqmaST8pbElYdUEgqF8xPvip6-3,
                 0: 8ianf2LAQlxK7ZFvdOX.avsuK4L9FjUiMC7sM2Lm,
                 1: IIffH-qkWUFB.-VFd0z6BBrIpfvNuc8GPxlQYgg3
             }
         },
         _id: VRlid5klewaC1bro7soJEr8Ynmt-N9YCNjW8iPN0,
         _ids: {
             d: fBb9FHVYpHC7vyM-B8UrXuN4oCcQ4Y7pnQ6oSK3J,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
-            df: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb,
-            ell: P1oPe-8hTjTdV6gKov4oIQnmTUXyD2fU6E7C8MS6
+            ell: P1oPe-8hTjTdV6gKov4oIQnmTUXyD2fU6E7C8MS6,
+            df: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb
         }
     }
     >>> from numpy import array
     >>> hdict(b=b, z=9, c=(c:=array([1,2,3])), d=Series(c), dd=array([[1, 2], [3, 4]])).show(colored=False)
     {
         b: {
             d: {
                 x: 3,
                 _id: fBb9FHVYpHC7vyM-B8UrXuN4oCcQ4Y7pnQ6oSK3J,
                 _ids: {
                     x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr
                 }
             },
             y: 5,
-            df: "‹{0: {0: 1, 1: 3}, 1: {0: 2, 1: 4}}›",
+            df_: "‹{0: {0: 1, 1: 3}, 1: {0: 2, 1: 4}}›",
             ell: "...",
-            df_: {
+            df: {
                 index: "‹{0: 0, 1: 1}›",
                 0: "‹{0: 1, 1: 3}›",
                 1: "‹{0: 2, 1: 4}›",
                 _id: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb,
                 _ids: {
                     index: DQa5yWRkGo-9FLqmaST8pbElYdUEgqF8xPvip6-3,
                     0: 8ianf2LAQlxK7ZFvdOX.avsuK4L9FjUiMC7sM2Lm,
                     1: IIffH-qkWUFB.-VFd0z6BBrIpfvNuc8GPxlQYgg3
                 }
             },
             _id: VRlid5klewaC1bro7soJEr8Ynmt-N9YCNjW8iPN0,
             _ids: {
                 d: fBb9FHVYpHC7vyM-B8UrXuN4oCcQ4Y7pnQ6oSK3J,
                 y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
-                df: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb,
-                ell: P1oPe-8hTjTdV6gKov4oIQnmTUXyD2fU6E7C8MS6
+                ell: P1oPe-8hTjTdV6gKov4oIQnmTUXyD2fU6E7C8MS6,
+                df: Zrz1JpxxZz7HIZDWPjdZEvMsqClGQnH7qcIqzhOb
             }
         },
         z: 9,
         c: "‹[1 2 3]›",
         d: "‹{0: 1, 1: 2, 2: 3}›",
         dd: "‹[[1 2] [3 4]]›",
         _id: 75i4qCm0ZAOdRV9TWDeUNQ7GuGmWWMQ8dndlVEsm,
@@ -154,28 +154,28 @@
             # from hoshmap import FrozenIdict, Idict
             # if isinstance(obj, Idict):
             #     return obj.frozen.asdicts
             # if isinstance(obj, FrozenIdict):
             #     return obj.asdicts
             if obj is Ellipsis:
                 return "..."
-            if isinstance(obj, AbsContent) and obj.isevaluated:
+            if isinstance(obj, AbsEntry) and obj.isevaluated:
                 # from hoshmap import FrozenIdict, Idict
                 # if isinstance(obj.value, Idict):
                 #     return obj.value.frozen.asdicts
                 # if isinstance(obj.value, FrozenIdict):
                 #     return obj.value.asdicts
                 return obj.value
             # if isinstance(obj, FunctionType):
             #     return str(obj)
             if not isinstance(obj, (dict, list, str, int, float, bytearray, bool)):
-                if obj.__class__.__name__ in ["DataFrame", "Series"]:
+                if type(obj).__name__ in ["DataFrame", "Series"]:
                     # ‹str()› is to avoid nested identation
                     return f"‹{truncate(str(obj.to_dict()), self.width)}›"
-                if obj.__class__.__name__ == "ndarray":
+                if type(obj).__name__ == "ndarray":
                     txt = str(obj).replace("\n", "")
                     return f"‹{truncate(txt, self.width)}›"
                 return truncate(str(obj).replace("\n", ""), self.width)
         return JSONEncoder.default(self, obj)  # pragma: no cover
 
 
 # class CustomJSONDecoder(JSONDecoder):
```

### Comparing `hdict-0.230211.1/src/hdict/frozenhdict.py` & `hdict-0.230408.2/src/hdict/frozenhdict.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,65 +20,73 @@
 #  part of this work is illegal and it is unethical regarding the effort and
 #  time spent here.
 #
 
 import json
 import re
 from collections import UserDict
-from typing import TypeVar
+from typing import TypeVar, Union
 
-from hdict.aux import handle_rshift
-from hdict.content import MissingFieldException
+from hdict.content.entry import AbsEntry
 from hdict.customjson import CustomJSONEncoder, stringfy
-from hdict.pipeline import pipeline
 
 VT = TypeVar("VT")
 
 
 class frozenhdict(UserDict, dict[str, VT]):
     """
     Immutable hdict.
 
     Any nested 'hdict' value will be frozen to avoid inconsistency between the hdict id (inner id) and the frozenhdict id (outer id).
 
     >>> from hdict.frozenhdict import frozenhdict
     >>> d = frozenhdict({"x": 3}, y=5)
+    >>> from hosh._internals_appearance import decolorize
+    >>> print(decolorize(repr(d)))  # This is equivalent to just 'd', without colors.
+    {
+        x: 3,
+        y: 5,
+        _id: r5A2Mh6vRRO5rxi5nfXv1myeguGSTmqHuHev38qM,
+        _ids: {
+            x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
+            y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2
+        }
+    }
     >>> d.data
-    {'x': 3, 'y': 5, '_id': 'r5A2Mh6vRRO5rxi5nfXv1myeguGSTmqHuHev38qM', '_ids': {'x': 'KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr', 'y': 'ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2'}}
-    >>> from hdict import _
-    >>> d >>= _(lambda v, x: v - x).z
+    {'x': 3, 'y': 5}
+    >>> from hdict import _, apply
+    >>> d *= apply(lambda v, x: v - x).z
     >>> str(d)
-    '{x: 3, y: 5, _id: "r5A2Mh6vRRO5rxi5nfXv1myeguGSTmqHuHev38qM", _ids: {x: "KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr", y: "ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2"}} » z=λ(v x)'
+    '{x: 3, y: 5} » z=λ(v x)'
     >>> d.show(colored=False)
     {
         x: 3,
         y: 5,
         _id: r5A2Mh6vRRO5rxi5nfXv1myeguGSTmqHuHev38qM,
         _ids: {
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2
-        },
-        v: ✗ missing ✗
+        }
     } » z=λ(v x)
-    >>> d = {"v": 7} >> d
-    >>> d.show(colored=False)
+    >>> d = {"v": 7} * d
+    >>> d.solve().show(colored=False)
     {
         v: 7,
         x: 3,
         y: 5,
         z: λ(v x),
         _id: -a24f2g4z-c-tPEss6G8WEd7h8zMopCCsCdQowjL,
         _ids: {
             v: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             z: .beBfajsUjKto9qdBCKsLmBgsaNPpJiyz24P9.qg
         }
     }
-    >>> d = _() >> d
+    >>> d = _ >> d
     >>> d.show(colored=False)
     {
         v: 7,
         x: 3,
         y: 5,
         z: λ(v x),
         _id: -a24f2g4z-c-tPEss6G8WEd7h8zMopCCsCdQowjL,
@@ -87,77 +95,76 @@
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             z: .beBfajsUjKto9qdBCKsLmBgsaNPpJiyz24P9.qg
         }
     }
     >>> d = {"a": 5} >> d
     >>> d.show(colored=False)
-    {'a': 5} » {
+    {
+        a: 5,
         v: 7,
         x: 3,
         y: 5,
         z: λ(v x),
-        _id: -a24f2g4z-c-tPEss6G8WEd7h8zMopCCsCdQowjL,
+        _id: ELQZugqdug6eCOLZSPaimnGqgmhRjJoDLD8cOlYR,
         _ids: {
+            a: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             v: eJCW9jGsdZTD6-AD9opKwjPIOWZ4R.T0CG2kdyzf,
             x: KGWjj0iyLAn1RG6RTGtsGE3omZraJM6xO.kvG5pr,
             y: ecvgo-CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2,
             z: .beBfajsUjKto9qdBCKsLmBgsaNPpJiyz24P9.qg
         }
     }
     """
 
     _evaluated = None
-    _asdict, _asdicts = None, None
+    _asdict, _asdicts, _asdicts_noid = None, None, None
 
     # noinspection PyMissingConstructor
     def __init__(self, /, _dictionary=None, _previous=None, **kwargs):
-        from hdict.content.handling import handle_values
-        from hdict.content.abs.abscontent import AbsContent
-        from hdict.content.handling import handle_identity
+        from hdict.content.entry import AbsEntry
+        from hdict.aux_frozendict import handle_identity
+        from hdict.aux_frozendict import handle_items
 
         if _previous is None:
             _previous = {}
 
+        # TODO: check if _dictionary keys is 'str'; regex to check if k is an identifier;
         data = _dictionary or {}
-        data.update(kwargs)
-        if "_id" in data.keys() or "_ids" in data.keys():  # pragma: no cover
-            raise Exception(f"Hosh-indexed dict cannot have a field named '_id'/'_ids': {data.keys()}")
-        handle_values(data, _previous)
-
-        # REMINDER: Inside data, the only 'dict' entries are "_id" and "_ids", the rest is AbsContent.
-        self.data: dict[str, AbsContent | str | dict[str, str]] = data
-
-        # REMINDER: "lazy hoshes" are only available after handling values (call above).
+        # REMINDER: Inside data, the only 'dict' entries are "_id" and "_ids", the rest are AbsEntry objects.
+        self.data: dict[str, AbsEntry | str | dict[str, str]]
+        self.data = handle_items(data, kwargs, previous=_previous)
         self.hosh, self.ids = handle_identity(self.data)
-        self.data["_id"] = self.id = self.hosh.id
-        self.data["_ids"] = self.ids
+        self.id = self.hosh.id
 
     def __rrshift__(self, other):
-        from hdict.hdict_ import hdict
+        from hdict import hdict
 
         if isinstance(other, dict) and not isinstance(other, (hdict, frozenhdict)):
-            return pipeline(hdict() >> other, self)
+            return frozenhdict(other) >> self
         return NotImplemented  # pragma: no cover
 
     def __rshift__(self, other):
-        from hdict.content.applyout import applyOut
+        from hdict import hdict
+        from hdict.applyout import ApplyOut
 
-        try:
-            return handle_rshift(self, other)
-        except MissingFieldException as e:
-            # REMINDER: dict includes hdict/frozenhdict.
-            if isinstance(other, (pipeline, dict, applyOut)):
-                return pipeline(self, other, missing={self.id: e.args[0]})
-            else:  # pragma: no cover
-                print(type(other))
-                raise e from None
+        # Merge keeping ids.
+        if isinstance(other, hdict):
+            other = other.frozen
+        if isinstance(other, frozenhdict):
+            other = other.data
+        if isinstance(other, ApplyOut):
+            other = {other.out: other.nested}
+
+        if isinstance(other, dict):
+            return frozenhdict(other, _previous=self.data)
+        return NotImplemented  # pragma: no cover
 
     def __getitem__(self, item):  # pragma: no cover
-        return self.data[item] if item in ["_id", "_ids"] else self.data[item].value
+        return self.data[item].value
 
     def __getattr__(self, item):  # pragma: no cover
         if item in self.data:
             return self.data[item].value
         return self.__getattribute__(item)
 
     def __setitem__(self, key: str, value):  # pragma: no cover
@@ -177,115 +184,146 @@
             x: 5,
             _id: bi5Qdbh-zgA1ZQdxGhxqjaKaQROtxk1VCPRZhMOq,
             _ids: {
                 x: 0123456789012345678901234567890123456789
             }
         }
         """
-        from hdict.content.abs.abscontent import AbsContent
         from hdict.content.value import value
 
         data = {}
         for k, v in dictionary.items():
-            if isinstance(v, AbsContent):
+            if isinstance(v, AbsEntry):
                 if k in ids and ids[k] != v.id:  # pragma: no cover
                     raise Exception(f"Conflicting ids provided for key '{k}': ival.id={v.id}; ids[{k}]={ids[k]}")
                 data[k] = v
             else:
                 data[k] = value(v, ids[k] if k in ids else None)
         return frozenhdict(data)
 
     @property
     def evaluated(self):
         if self._evaluated is None:
-            self._evaluated = self.evaluate()
+            for k, val in self.data.items():
+                val.evaluate()
+            self._evaluated = self
         return self
 
     def evaluate(self):
-        from hdict import apply
-
-        for k, val in self.data.items():
-            if isinstance(val, apply):
-                val.evaluate()
-        return self
+        _ = self.evaluated
 
     @property
     def asdict(self):
         """
+        Convert to 'dict', including ids.
+
+        This evaluates all fields.
+        HINT: Use 'dict(d)' to convert a 'hdict' to a 'dict' excluding ids.
+
         >>> from hdict import hdict, value
         >>> d = hdict.fromdict({"x": value(5, hosh="0123456789012345678901234567890123456789")}, {"x": "0123456789012345678901234567890123456789"})
         >>> d.asdict
         {'x': 5, '_id': 'bi5Qdbh-zgA1ZQdxGhxqjaKaQROtxk1VCPRZhMOq', '_ids': {'x': '0123456789012345678901234567890123456789'}}
         """
         if self._asdict is None:
-            dic = {k: v for k, v in self.items()}
+            dic = dict(self.items())
             dic["_id"] = self.id
             dic["_ids"] = self.ids.copy()
             self._asdict = dic
         return self._asdict
 
     @property
     def asdicts(self):
         """
-        Recurse into nested frozenhdicts (REMINDER: hdict is never nested)
+        Convert to 'dict' recursing into nested frozenhdicts, including ids.
+
+        This evaluates all fields.
+        REMINDER: hdict is never nested, frozenhdict is used instead
+        HINT: Use 'asdicts_noid' to recursively convert a 'hdict' to a 'dict' excluding ids.
 
         >>> from hdict import value, hdict
         >>> d = hdict(x=value(5, hosh="0123456789012345678901234567890123456789"))
-        >>> d.asdicts
-        {'x': 5, '_id': 'bi5Qdbh-zgA1ZQdxGhxqjaKaQROtxk1VCPRZhMOq', '_ids': {'x': '0123456789012345678901234567890123456789'}}
+        >>> e = hdict(d=d)
+        >>> e.asdicts
+        {'d': {'x': 5, '_id': 'bi5Qdbh-zgA1ZQdxGhxqjaKaQROtxk1VCPRZhMOq', '_ids': {'x': '0123456789012345678901234567890123456789'}}, '_id': 'GGhKhUmGhISaoHevn39hb-pLZEMoAc3KzE6Z0.IH', '_ids': {'d': 'bi5Qdbh-zgA1ZQdxGhxqjaKaQROtxk1VCPRZhMOq'}}
+        >>> dict(e) == e
+        True
         """
         if self._asdicts is None:
+            from hdict import hdict
+
             dic = {}
             for k, v in self.items():
-                dic[k] = v.asdicts if isinstance(v, frozenhdict) else v
+                dic[k] = v.asdicts if isinstance(v, (hdict, frozenhdict)) else v
             dic["_id"] = self.id
             dic["_ids"] = self.ids.copy()
             self._asdicts = dic
         return self._asdicts
 
     @property
+    def asdicts_noid(self):
+        """
+        Convert to 'dict' recursing into nested frozenhdicts, excluding ids.
+
+        REMINDER: hdict is never nested, frozenhdict is used instead
+        HINT: Use 'asdicts' to recursively convert a 'hdict' 'd' to 'dict' including ids.
+
+        >>> from hdict import value, hdict
+        >>> d = hdict(x=value(5, hosh="0123456789012345678901234567890123456789"))
+        >>> e = hdict(d=d)
+        >>> e.asdicts_noid
+        {'d': {'x': 5}}
+        >>> dict(e) == e
+        True
+
+        """
+        if self._asdicts_noid is None:
+            from hdict import hdict
+
+            dic = {}
+            for k, v in self.items():
+                dic[k] = v.asdicts_noid if isinstance(v, (hdict, frozenhdict)) else v
+            self._asdicts_noid = dic
+        return self._asdicts_noid
+
+    @property
     def asdicts_hoshes_noneval(self):
-        from hdict.content.abs.abscloneable import AbsCloneable
+        from hdict import value
 
         hoshes = set()
         dic = {}
         for k, val in self.data.items():
-            if k not in ["_id", "_ids"]:
+            if isinstance(val, AbsEntry):
                 hoshes.add(val.hosh)
-                if isinstance(val, AbsCloneable):
-                    dic[k] = val
+            if isinstance(val, value):
+                v = val.value
+                if isinstance(v, frozenhdict):
+                    dic[k], subhoshes = v.asdicts_hoshes_noneval
+                    hoshes.update(subhoshes)
                 else:
-                    v = val.value
-                    if isinstance(v, frozenhdict):
-                        dic[k], subhoshes = v.asdicts_hoshes_noneval
-                        hoshes.update(subhoshes)
-                    else:
-                        dic[k] = v
+                    dic[k] = v
+            else:
+                dic[k] = val
         hoshes.add(self.hosh)
         dic["_id"] = self.id
         dic["_ids"] = self.ids.copy()
         return dic, hoshes
 
-    def astext(self, colored=True, key_quotes=False, extra_items=None):
+    def astext(self, colored=True, key_quotes=False):
         r"""Textual representation of a frozenidict object"""
         dicts, hoshes = self.asdicts_hoshes_noneval
-        if extra_items:
-            dicts.update(extra_items)
         txt = json.dumps(dicts, indent=4, ensure_ascii=False, cls=CustomJSONEncoder)
 
         # Put colors after json, to avoid escaping ansi codes.  TODO: check how HTML behaves here
         for h in hoshes:
             txt = txt.replace(f'"{h.id}"', repr(h)) if colored else txt.replace(f'"{h.id}"', h.id)
         txt = re.sub(r'(": )"(λ.+?)"(?=,\n)', '": \\2', txt)
         if not key_quotes:
             txt = re.sub(r'(?<!: )"([\-a-zA-Z0-9_ ]+?)"(?=: )', "\\1", txt)
-        if extra_items:
-            for v in extra_items.values():
-                txt = txt.replace(f'"{v}"', f"{v}")
-        return txt
+        return txt.replace('"§«§lazy', "").replace('lazy§«§"', "")
 
     def show(self, colored=True, key_quotes=False):
         r"""Print textual representation of a frozenidict object"""
         print(self.astext(colored, key_quotes))
 
     def copy(self):  # pragma: no cover
         raise Exception("A FrozenIdict doesn't need copies")
@@ -305,96 +343,112 @@
         """Generator of keys which don't start with '_'"
         >>> from hdict import hdict
         >>> list(hdict(x=3, y=5).keys())
         ['x', 'y']
         >>> list(hdict(x=3, y=5).values())
         [3, 5]
         """
-        return (k for k in self.data if not k.startswith("_"))
+        # return (k for k in self.data if not k.startswith("_"))
+        return self.data.keys()
 
     def values(self, evaluate=True):
         """Generator of field values (keys that don't start with '_')"""
-        return ((v.value if evaluate else v) for k, v in self.data.items() if not k.startswith("_"))
+        return ((v.value if evaluate else v) for k, v in self.data.items())
+        # return ((v.value if evaluate else v) for k, v in self.data.items() if not k.startswith("_"))
 
     def items(self, evaluate=True):
         """Generator over field-value pairs"""
         for k, val in self.data.items():
-            if not k.startswith("_"):
-                yield k, (val.value if evaluate else val)
+            # if not k.startswith("_"):
+            yield k, (val.value if evaluate else val)
 
-    # @cached_property
-    # def aslist(self):
-    #     return list(self.values())
-    #
-    # @staticmethod
-    # def fromid(id, cache) -> Union["frozenhdict", None]:
-    #     return frozenhdict.fetch(id, cache, isidict=True)
-    #
-    # @staticmethod
-    # def fetch(id, cache, isidict=False) -> Union["frozenhdict", None]:
-    #     caches = cache if isinstance(cache, list) else [cache]
-    #     while id not in (cache := caches.pop(0)):
-    #         if not caches:
-    #             raise Exception(f"id '{id}' not found in the provided cache {cache.keys()}.")
-    #
-    #     obj = cache[id]
-    #     if isinstance(obj, dict):
-    #         if "_ids" not in obj:
-    #             raise Exception(f"Wrong content for idict under id {id}: missing '_ids' fields ({obj.keys()}).")
-    #         isidict = True
-    #     elif isidict:
-    #         raise Exception(f"Wrong content for idict expected under id {id}: {type(obj)}.")
-    #
-    #     # TODO: adopt lazy fetch: CacheableiVal as 'return' value
-    #     if isidict:
-    #         ids = obj["_ids"]
-    #         data = {}
-    #         for k, v in ids.items():
-    #             data[k] = frozenhdict.fetch(v, cache)
-    #         return frozenhdict.fromdict(data, ids)
-    #     return obj
+    def save(self, cache: dict):
+        """
+        Store an entire frozenidict
+        """
+        data = {self.id: self.ids}
+        for field, fid in self.ids.items():
+            value = self[field]
+            if isinstance(value, frozenhdict):
+                value.save(cache)
+            else:
+                data[fid] = value
+        cache.update(data)
+
+    @staticmethod
+    def load(id, cache: dict | list, lazy=True) -> Union["frozenhdict", None]:
+        """
+        Fetch an entire frozenidict
+        """
+        if len(id) != 40:  # pragma: no cover
+            raise Exception(f"id should have lenght of 40, not {len(id)}")
+        return frozenhdict.fetch(id, cache, lazy, ishdict=True)
+
+    @staticmethod
+    def fetch(id, cache, lazy=True, ishdict=False) -> Union["frozenhdict", None]:
+        """
+        Fetch a single entry
+
+        When cache is a list, traverse it from the end (right item to the left item).
+        """
+        from hdict.content.entry.lazy import Lazy
+
+        caches = cache if isinstance(cache, list) else [cache]
+        while id not in (cache := caches.pop()):
+            if not caches:
+                raise Exception(f"id '{id}' not found in the provided cache {cache.keys()}.")
+        obj = cache[id]
+        if isinstance(obj, dict):
+            ishdict = True  # Set to True, because now we have a nested frozenhdict
+        elif ishdict:
+            raise Exception(f"Wrong content for idict expected under id {id}: {type(obj)}.")
+
+        if ishdict:
+            ids = obj
+            data = {}
+            for field, fid in ids.items():
+                data[field] = Lazy(fid, cache) if lazy else frozenhdict.fetch(fid, cache, lazy, False)
+            return frozenhdict.fromdict(data, ids)
+        return obj
 
     def __eq__(self, other):
         if isinstance(other, dict):
             if "_id" in other:
                 return self.id == other["_id"]
             if list(self.keys()) != list(other.keys()):
                 return False
-        if isinstance(other, dict):
-            self.evaluate()
-            data = self.asdict
-            del data["_id"]
-            del data["_ids"]
-            return data == other
-        raise TypeError(f"Cannot compare {type(self)} and {type(other)}")  # pragma: no cover
+            from hdict import hdict
+
+            if isinstance(other, (frozenhdict, hdict)):
+                return self.id == other.id
+            return dict(self) == other
+        raise TypeError(f"Cannot compare {type(self).__name__} and {type(other).__name__}")  # pragma: no cover
 
     def __ne__(self, other):
         return not (self == other)
 
-    # def __reduce__(self):
-    #     # TODO: pickling idicts shouldn't be necessary after cache[id]=DFiVal is implemented
-    #     dic = self.data.copy()
-    #     ids = dic.pop("_ids").copy()
-    #     del dic["_id"]
-    #     return self.fromdict, (dic, ids)
-
     def __repr__(self):
         return self.astext()
 
     def __str__(self):
         return stringfy(self.data)
 
     def __iter__(self):
         for k in self.data:
-            if not k.startswith("_"):
-                yield k
+            # if not k.startswith("_"):
+            yield k
 
     def __hash__(self):
         return hash(self.hosh)
 
+    def __mul__(self, other):
+        from hdict.expr import Expr
+
+        return Expr(self, other)
+
     # def metakeys(self):
     #     """Generator of keys which start with '_'"""
     #     return (k for k in self.data if k.startswith("_") and k not in ["_id", "_ids"])
     #
     # def metavalues(self, evaluate=True):
     #     """Generator of field values (keys don't start with '_')"""
     #     return ((v.value if evaluate else v) for k, v in self.data.items() if k.startswith("_") and k not in ["_id", "_ids"])
```

### Comparing `hdict-0.230211.1/src/hdict/hoshfication.py` & `hdict-0.230408.2/src/hdict/hoshfication.py`

 * *Files identical despite different names*

### Comparing `hdict-0.230211.1/src/hdict/pandas_handling.py` & `hdict-0.230408.2/src/hdict/pandas_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 
 
 def explode_df(df) -> value:
     """
     >>> from pandas import DataFrame
     >>> from hdict import hdict
     >>> df = DataFrame({"x": [1,2,3], "y": [5,6,7]}, index=["a", "b", "c"])
-    >>> d = hdict(df=df)
+    >>> d = hdict(df_=df)
     >>> d.show(colored=False)
     {
-        df: "‹{'x': {'a': 1, 'b': 2, 'c': 3}, 'y': {'a': 5, 'b': 6, 'c': 7}}›",
-        df_: {
+        df_: "‹{'x': {'a': 1, 'b': 2, 'c': 3}, 'y': {'a': 5, 'b': 6, 'c': 7}}›",
+        df: {
             index: "‹{'a': 'a', 'b': 'b', 'c': 'c'}›",
             x: "‹{'a': 1, 'b': 2, 'c': 3}›",
             y: "‹{'a': 5, 'b': 6, 'c': 7}›",
             _id: CO3m4w1vqM.etZXkoHQoNxA.PS.kQI-LomW.H6VC,
             _ids: {
                 index: HBNoEs58wCDhsdWWisp0sjMwsWmNMXuwaGFE9UAt,
                 x: 3F.7UkfLr2tpB-FxATaRJYIpbYpg9oa1r5M31M0j,
@@ -45,15 +45,15 @@
             }
         },
         _id: qMP.-f8p3zIrmTuOOqBLCVurT6uIIfihnR3rZne4,
         _ids: {
             df: CO3m4w1vqM.etZXkoHQoNxA.PS.kQI-LomW.H6VC
         }
     }
-    >>> d.df
+    >>> d.df_
        x  y
     a  1  5
     b  2  6
     c  3  7
     """
     from hdict.frozenhdict import frozenhdict
     from hdict import value
```

### Comparing `hdict-0.230211.1/setup.py` & `hdict-0.230408.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['hdict', 'hdict.content', 'hdict.content.abs']
+['hdict',
+ 'hdict.abs',
+ 'hdict.content',
+ 'hdict.content.argument',
+ 'hdict.content.entry',
+ 'hdict.data',
+ 'hdict.persistence']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['hosh>=2.230205.2,<3.0.0', 'indexed>=1.3.0,<2.0.0', 'lange>=1.230203.2,<2.0.0']
 
 extras_require = \
-{'full': ['pandas>=1.5.2,<2.0.0']}
+{'full': ['pandas>=1.5.2,<2.0.0',
+          'shelchemy>=0.220906.3,<0.220907.0',
+          'safeserializer>=0.230202.1,<0.230203.0',
+          'lz4>=4.3.2,<5.0.0']}
 
 setup_kwargs = {
     'name': 'hdict',
-    'version': '0.230211.1',
+    'version': '0.230408.2',
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
@@ -1,29 +1,33 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['hdict', 'hdict.content', 'hdict.content.abs']
-package_data = \ {'': ['*']} install_requires = \ ['hosh>=2.230205.2,<3.0.0',
-'indexed>=1.3.0,<2.0.0', 'lange>=1.230203.2,<2.0.0'] extras_require = \
-{'full': ['pandas>=1.5.2,<2.0.0']} setup_kwargs = { 'name': 'hdict', 'version':
-'0.230211.1', 'description': 'A versatile dictionary based on a novel paradigm
-useful for computing, caching, experiments, distributed data, among others.',
-'long_description': '![test](https://github.com/davips/hdict/workflows/test/
-badge.svg)\n[![codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/
-badge.svg)](https://codecov.io/gh/davips/hdict)\n\n[pypi]\n\n![Python version]
-(https://img.shields.io/badge/python-3.10...-blue.svg)\n[![license: GPL v3]
-(https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
-licenses/gpl-3.0)\n\n\n[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-
-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)\n[![API
-documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)]
-(https://davips.github.io/hdict)\n[![Manual](https://img.shields.io/badge/
-manual-handcrafted-a030a0.svg)](https://hosh.page)\n[![Downloads](https://
-static.pepy.tech/badge/hdict)](https://pepy.tech/project/hdict)\n\n# hdict { A
-_unique_ data structure }\n[Website](https://hosh.page) | \n[Latest Release]
-(https://pypi.org/project/hdict) |\n[Current Code](https://github.com/davips/
-hdict) |\n[API Documentation](https://davips.github.io/hdict)\n\nPlease see the
-[website](https://hosh.page) for more detailed usage information.\n\n##
+'src'} packages = \ ['hdict', 'hdict.abs', 'hdict.content',
+'hdict.content.argument', 'hdict.content.entry', 'hdict.data',
+'hdict.persistence'] package_data = \ {'': ['*']} install_requires = \
+['hosh>=2.230205.2,<3.0.0', 'indexed>=1.3.0,<2.0.0',
+'lange>=1.230203.2,<2.0.0'] extras_require = \ {'full':
+['pandas>=1.5.2,<2.0.0', 'shelchemy>=0.220906.3,<0.220907.0',
+'safeserializer>=0.230202.1,<0.230203.0', 'lz4>=4.3.2,<5.0.0']} setup_kwargs =
+{ 'name': 'hdict', 'version': '0.230408.2', 'description': 'A versatile
+dictionary based on a novel paradigm useful for computing, caching,
+experiments, distributed data, among others.', 'long_description': '![test]
+(https://github.com/davips/hdict/workflows/test/badge.svg)\n[![codecov](https:/
+/codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)](https://codecov.io/
+gh/davips/hdict)\n\n[pypi]\n\n![Python version](https://img.shields.io/badge/
+python-3.10...-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/
+License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n\n[![arXiv]
+(https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)]
+(https://arxiv.org/abs/2109.06028)\n[![API documentation](https://
+img.shields.io/badge/API-autogenerated-a030a0.svg)](https://davips.github.io/
+hdict)\n[![Manual](https://img.shields.io/badge/manual-handcrafted-a030a0.svg)]
+(https://hosh.page)\n[![Downloads](https://static.pepy.tech/badge/hdict)]
+(https://pepy.tech/project/hdict)\n\n# hdict { A _unique_ data structure }\n
+[Website](https://hosh.page) | \n[Latest Release](https://pypi.org/project/
+hdict) |\n[Current Code](https://github.com/davips/hdict) |\n[API
+Documentation](https://davips.github.io/hdict)\n\nPlease see the [website]
+(https://hosh.page) for more detailed usage information.\n\n##
 Overview\n**Shortly**: A data structure based on a novel identification
 paradigm useful for frictionless computing, experiments, distributed data,
 among others.\n\n**Formally**: Hosh-based cacheable lazy dict with predictable/
 deterministic universally (probabilistically guaranteed) unique
 identifiers.\n\n\n### Context\n\n * [hosh](https://pypi.org/project/hosh):
 identification engine at the core of `hdict`\n * previous projects: [hoshmap]
 (https://pypi.org/project/hoshmap), [idict](https://pypi.org/project/idict),
```

### Comparing `hdict-0.230211.1/PKG-INFO` & `hdict-0.230408.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: hdict
-Version: 0.230211.1
+Version: 0.230408.2
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
+Requires-Dist: lz4 (>=4.3.2,<5.0.0) ; extra == "full"
 Requires-Dist: pandas (>=1.5.2,<2.0.0) ; extra == "full"
+Requires-Dist: safeserializer (>=0.230202.1,<0.230203.0) ; extra == "full"
+Requires-Dist: shelchemy (>=0.220906.3,<0.220907.0) ; extra == "full"
 Description-Content-Type: text/markdown
 
 ![test](https://github.com/davips/hdict/workflows/test/badge.svg)
 [![codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hdict)
 <a href="https://pypi.org/project/hdict">
 <img src="https://img.shields.io/pypi/v/hdict.svg?label=release&color=blue&style=flat-square" alt="pypi">
 </a>
```

#### html2text {}

```diff
@@ -1,45 +1,47 @@
-Metadata-Version: 2.1 Name: hdict Version: 0.230211.1 Summary: A versatile
+Metadata-Version: 2.1 Name: hdict Version: 0.230408.2 Summary: A versatile
 dictionary based on a novel paradigm useful for computing, caching,
 experiments, distributed data, among others. License: GPLv3 Author: davips
 Author-email: dpsabc@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: full Requires-Dist: hosh
 (>=2.230205.2,<3.0.0) Requires-Dist: indexed (>=1.3.0,<2.0.0) Requires-Dist:
-lange (>=1.230203.2,<2.0.0) Requires-Dist: pandas (>=1.5.2,<2.0.0) ; extra ==
-"full" Description-Content-Type: text/markdown ![test](https://github.com/
-davips/hdict/workflows/test/badge.svg) [![codecov](https://codecov.io/gh/
-davips/hdict/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/hdict)
-[pypi] ![Python version](https://img.shields.io/badge/python-3.10...-blue.svg)
-[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)]
-(https://www.gnu.org/licenses/gpl-3.0)  [![arXiv](https://img.shields.io/badge/
-arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/
-2109.06028) [![API documentation](https://img.shields.io/badge/API-
-autogenerated-a030a0.svg)](https://davips.github.io/hdict) [![Manual](https://
-img.shields.io/badge/manual-handcrafted-a030a0.svg)](https://hosh.page) [!
-[Downloads](https://static.pepy.tech/badge/hdict)](https://pepy.tech/project/
-hdict) # hdict { A _unique_ data structure } [Website](https://hosh.page) |
-[Latest Release](https://pypi.org/project/hdict) | [Current Code](https://
-github.com/davips/hdict) | [API Documentation](https://davips.github.io/hdict)
-Please see the [website](https://hosh.page) for more detailed usage
-information. ## Overview **Shortly**: A data structure based on a novel
-identification paradigm useful for frictionless computing, experiments,
-distributed data, among others. **Formally**: Hosh-based cacheable lazy dict
-with predictable/deterministic universally (probabilistically guaranteed)
-unique identifiers. ### Context * [hosh](https://pypi.org/project/hosh):
-identification engine at the core of `hdict` * previous projects: [hoshmap]
-(https://pypi.org/project/hoshmap), [idict](https://pypi.org/project/idict),
-[ldict](https://pypi.org/project/ldict), [garoupa](https://pypi.org/project/
-garoupa) ### The concept `hdict` is like an ordinary `dict` with `str` keys.
-Each entry, called _field_, and the `hdict` itself, are identified by 40-digit
-hashes (see [hosh](https://pypi.org/project/hosh)). A `hdict` object (say `d`)
-provides two extra entries: `_id` (hdict identifier) and `_ids` (field
-identifiers), accessible through square brackets or through the shortcuts
-`d.id` and `d.ids`. **`hdict` creation**
+lange (>=1.230203.2,<2.0.0) Requires-Dist: lz4 (>=4.3.2,<5.0.0) ; extra ==
+"full" Requires-Dist: pandas (>=1.5.2,<2.0.0) ; extra == "full" Requires-Dist:
+safeserializer (>=0.230202.1,<0.230203.0) ; extra == "full" Requires-Dist:
+shelchemy (>=0.220906.3,<0.220907.0) ; extra == "full" Description-Content-
+Type: text/markdown ![test](https://github.com/davips/hdict/workflows/test/
+badge.svg) [![codecov](https://codecov.io/gh/davips/hdict/branch/main/graph/
+badge.svg)](https://codecov.io/gh/davips/hdict) [pypi] ![Python version](https:
+//img.shields.io/badge/python-3.10...-blue.svg) [![license: GPL v3](https://
+img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
+3.0)  [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-
+b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) [![API
+documentation](https://img.shields.io/badge/API-autogenerated-a030a0.svg)]
+(https://davips.github.io/hdict) [![Manual](https://img.shields.io/badge/
+manual-handcrafted-a030a0.svg)](https://hosh.page) [![Downloads](https://
+static.pepy.tech/badge/hdict)](https://pepy.tech/project/hdict) # hdict { A
+_unique_ data structure } [Website](https://hosh.page) | [Latest Release]
+(https://pypi.org/project/hdict) | [Current Code](https://github.com/davips/
+hdict) | [API Documentation](https://davips.github.io/hdict) Please see the
+[website](https://hosh.page) for more detailed usage information. ## Overview
+**Shortly**: A data structure based on a novel identification paradigm useful
+for frictionless computing, experiments, distributed data, among others.
+**Formally**: Hosh-based cacheable lazy dict with predictable/deterministic
+universally (probabilistically guaranteed) unique identifiers. ### Context *
+[hosh](https://pypi.org/project/hosh): identification engine at the core of
+`hdict` * previous projects: [hoshmap](https://pypi.org/project/hoshmap),
+[idict](https://pypi.org/project/idict), [ldict](https://pypi.org/project/
+ldict), [garoupa](https://pypi.org/project/garoupa) ### The concept `hdict` is
+like an ordinary `dict` with `str` keys. Each entry, called _field_, and the
+`hdict` itself, are identified by 40-digit hashes (see [hosh](https://pypi.org/
+project/hosh)). A `hdict` object (say `d`) provides two extra entries: `_id`
+(hdict identifier) and `_ids` (field identifiers), accessible through square
+brackets or through the shortcuts `d.id` and `d.ids`. **`hdict` creation**
 ```python3 from hdict import hdict # From named arguments. d = hdict(x=5, y=7,
 z=10) # From a dict object. d = hdict({"x": 5, "y": 7, "z": 10}) # From an
 empty 'hdict' object. d = hdict() >> {"x": 5} >> {"y": 7, "z": 10} # All three
 options have the same result. d.show(colored=False) """ { x: 5, y: 7, z: 10,
 _id: BN-3Q3Z.2Q.9nsbIYnOI75HT7xhgjvF6wErwBPTn, _ids: { x: ecvgo-
 CBPi7wRWIxNzuo1HgHQCbdvR058xi6zmr2, y: eJCW9jGsdZTD6-
 AD9opKwjPIOWZ4R.T0CG2kdyzf, z: u-Yykj2nDtKaUMGzfqScX5Y14qC7eqJrO7lXrJ1m } } """
```

