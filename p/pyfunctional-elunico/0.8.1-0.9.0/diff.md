# Comparing `tmp/pyfunctional-elunico-0.8.1.tar.gz` & `tmp/pyfunctional-elunico-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfunctional-elunico-0.8.1.tar", last modified: Sun Nov 27 00:31:03 2022, max compression
+gzip compressed data, was "pyfunctional-elunico-0.9.0.tar", last modified: Wed Dec  7 14:29:37 2022, max compression
```

## Comparing `pyfunctional-elunico-0.8.1.tar` & `pyfunctional-elunico-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2022-11-27 00:31:03.538502 pyfunctional-elunico-0.8.1/
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1060 2022-11-26 17:23:15.000000 pyfunctional-elunico-0.8.1/LICENSE
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      133 2022-11-26 17:23:31.000000 pyfunctional-elunico-0.8.1/MANIFEST.in
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)     2151 2022-11-27 00:31:03.538232 pyfunctional-elunico-0.8.1/PKG-INFO
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1690 2022-11-26 20:19:03.000000 pyfunctional-elunico-0.8.1/README.md
-drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2022-11-27 00:31:03.536357 pyfunctional-elunico-0.8.1/pyfunctional/
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      146 2022-11-27 00:30:53.000000 pyfunctional-elunico-0.8.1/pyfunctional/__init__.py
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      624 2022-11-26 20:29:21.000000 pyfunctional-elunico-0.8.1/pyfunctional/pftyping.py
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)     2777 2022-11-26 20:41:54.000000 pyfunctional-elunico-0.8.1/pyfunctional/pyfunctional.py
-drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2022-11-27 00:31:03.537852 pyfunctional-elunico-0.8.1/pyfunctional_elunico.egg-info/
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)     2151 2022-11-27 00:31:03.000000 pyfunctional-elunico-0.8.1/pyfunctional_elunico.egg-info/PKG-INFO
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      308 2022-11-27 00:31:03.000000 pyfunctional-elunico-0.8.1/pyfunctional_elunico.egg-info/SOURCES.txt
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)        1 2022-11-27 00:31:03.000000 pyfunctional-elunico-0.8.1/pyfunctional_elunico.egg-info/dependency_links.txt
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)       13 2022-11-27 00:31:03.000000 pyfunctional-elunico-0.8.1/pyfunctional_elunico.egg-info/top_level.txt
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      103 2022-11-26 17:23:02.000000 pyfunctional-elunico-0.8.1/pyproject.toml
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)       38 2022-11-27 00:31:03.538586 pyfunctional-elunico-0.8.1/setup.cfg
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      726 2022-11-27 00:30:59.000000 pyfunctional-elunico-0.8.1/setup.py
+drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2022-12-07 14:29:37.875627 pyfunctional-elunico-0.9.0/
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1060 2022-11-26 17:23:15.000000 pyfunctional-elunico-0.9.0/LICENSE
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      133 2022-11-26 17:23:31.000000 pyfunctional-elunico-0.9.0/MANIFEST.in
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)     2479 2022-12-07 14:29:37.875246 pyfunctional-elunico-0.9.0/PKG-INFO
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)     2018 2022-12-07 12:01:32.000000 pyfunctional-elunico-0.9.0/README.md
+drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2022-12-07 14:29:37.873134 pyfunctional-elunico-0.9.0/pyfunctional/
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      146 2022-11-27 00:30:53.000000 pyfunctional-elunico-0.9.0/pyfunctional/__init__.py
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      624 2022-11-26 20:29:21.000000 pyfunctional-elunico-0.9.0/pyfunctional/pftyping.py
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)     3227 2022-12-07 11:56:34.000000 pyfunctional-elunico-0.9.0/pyfunctional/pyfunctional.py
+drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2022-12-07 14:29:37.874859 pyfunctional-elunico-0.9.0/pyfunctional_elunico.egg-info/
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)     2479 2022-12-07 14:29:37.000000 pyfunctional-elunico-0.9.0/pyfunctional_elunico.egg-info/PKG-INFO
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      308 2022-12-07 14:29:37.000000 pyfunctional-elunico-0.9.0/pyfunctional_elunico.egg-info/SOURCES.txt
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)        1 2022-12-07 14:29:37.000000 pyfunctional-elunico-0.9.0/pyfunctional_elunico.egg-info/dependency_links.txt
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)       13 2022-12-07 14:29:37.000000 pyfunctional-elunico-0.9.0/pyfunctional_elunico.egg-info/top_level.txt
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      103 2022-11-26 17:23:02.000000 pyfunctional-elunico-0.9.0/pyproject.toml
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)       38 2022-12-07 14:29:37.875721 pyfunctional-elunico-0.9.0/setup.cfg
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      726 2022-12-07 14:29:33.000000 pyfunctional-elunico-0.9.0/setup.py
```

### Comparing `pyfunctional-elunico-0.8.1/LICENSE` & `pyfunctional-elunico-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfunctional-elunico-0.8.1/PKG-INFO` & `pyfunctional-elunico-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pyfunctional-elunico
-Version: 0.8.1
+Version: 0.9.0
 Summary: A small collection of functions I find useful
 Home-page: https://github.com/elunico/pyfunctional
 Author: Thomas Povinelli
 Author-email: tompov227@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfunctional
 
+Find it [on PyPI](https://pypi.org/project/pyfunctional-elunico/)
+
 This is a collection of functional tools I like to use in Python
 
 ## Contents
 
 ```python
 alleq(iterable: Iterable[S]) -> bool
 ```
@@ -50,14 +52,16 @@
   args: Iterable[Any],
   kwargs: Dict[Any, Any]
 ) -> T
 ```
 
 a function that takes a callable, a default value, a list of excpetion types, an arg tuple, and a kwarg dict and calls the callable, catching the exceptions specified, and returning the function value on success, the default value on a known caught exception, and allowing any other none-accounted for exceptions bubble up.
 
+---
+
 ```python
 rreduce(
     reduction: Callable[[R, E], R],
     indexable: Indexable,
     initvalue: Union[R, Sentinel] = sentinel
 ) -> R
 ```
@@ -69,7 +73,23 @@
 ```python
 from typing import Protocol
 
 class Indexable(Protocol):
   def __getitem__(self, index: int) -> Any: ...
   def __len__(self) -> int: ...
 ```
+
+---
+
+```python
+def commute(fn: Callable[[S, T], R]) -> Callable[[T, S], R]
+```
+
+Commutes the operands of a binary function. Does not (yet) work for varargs or functions other than 2-arity
+
+---
+
+```python
+def identity(x: T) -> T
+```
+
+The identity function
```

### Comparing `pyfunctional-elunico-0.8.1/README.md` & `pyfunctional-elunico-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # pyfunctional
 
+Find it [on PyPI](https://pypi.org/project/pyfunctional-elunico/)
+
 This is a collection of functional tools I like to use in Python
 
 ## Contents
 
 ```python
 alleq(iterable: Iterable[S]) -> bool
 ```
@@ -36,14 +38,16 @@
   args: Iterable[Any],
   kwargs: Dict[Any, Any]
 ) -> T
 ```
 
 a function that takes a callable, a default value, a list of excpetion types, an arg tuple, and a kwarg dict and calls the callable, catching the exceptions specified, and returning the function value on success, the default value on a known caught exception, and allowing any other none-accounted for exceptions bubble up.
 
+---
+
 ```python
 rreduce(
     reduction: Callable[[R, E], R],
     indexable: Indexable,
     initvalue: Union[R, Sentinel] = sentinel
 ) -> R
 ```
@@ -55,7 +59,23 @@
 ```python
 from typing import Protocol
 
 class Indexable(Protocol):
   def __getitem__(self, index: int) -> Any: ...
   def __len__(self) -> int: ...
 ```
+
+---
+
+```python
+def commute(fn: Callable[[S, T], R]) -> Callable[[T, S], R]
+```
+
+Commutes the operands of a binary function. Does not (yet) work for varargs or functions other than 2-arity
+
+---
+
+```python
+def identity(x: T) -> T
+```
+
+The identity function
```

### Comparing `pyfunctional-elunico-0.8.1/pyfunctional/pftyping.py` & `pyfunctional-elunico-0.9.0/pyfunctional/pftyping.py`

 * *Files identical despite different names*

### Comparing `pyfunctional-elunico-0.8.1/pyfunctional/pyfunctional.py` & `pyfunctional-elunico-0.9.0/pyfunctional/pyfunctional.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import functools
 from pyfunctional.pftyping import *
 
 
 def attempt(
         block: Callable[[Any], T],
         default: Optional[T] = None,
         catch: Union[Type[BaseException], Tuple[Type[BaseException]]] = (Exception,),
@@ -96,7 +97,26 @@
 ) -> R:
     if initvalue is sentinel and len(indexable) == 0:
         raise ValueError("rreduce() of empty sequence with no initial value")
     acc = initvalue if initvalue is not sentinel else indexable[-1]
     for i in range(-2 if initvalue is sentinel else -1, -len(indexable) - 1, -1):
         acc = reduction(acc, indexable[i])
     return acc
+
+
+def commute(fn: Callable[[S, T], R]) -> Callable[[T, S], R]:
+    if not callable(fn):
+        raise TypeError("Cannot commute non callable object {}".format(fn))
+
+    if fn.__code__.argcount != 2:
+        # todo: support varargs
+        raise ValueError("Function must have exactly 2 arguments not")
+
+    @functools.wraps(fn)
+    def inside(a, b):
+        return fn(b, a)
+
+    return inside
+
+
+def identity(x: T) -> T:
+    return x
```

### Comparing `pyfunctional-elunico-0.8.1/pyfunctional_elunico.egg-info/PKG-INFO` & `pyfunctional-elunico-0.9.0/pyfunctional_elunico.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pyfunctional-elunico
-Version: 0.8.1
+Version: 0.9.0
 Summary: A small collection of functions I find useful
 Home-page: https://github.com/elunico/pyfunctional
 Author: Thomas Povinelli
 Author-email: tompov227@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfunctional
 
+Find it [on PyPI](https://pypi.org/project/pyfunctional-elunico/)
+
 This is a collection of functional tools I like to use in Python
 
 ## Contents
 
 ```python
 alleq(iterable: Iterable[S]) -> bool
 ```
@@ -50,14 +52,16 @@
   args: Iterable[Any],
   kwargs: Dict[Any, Any]
 ) -> T
 ```
 
 a function that takes a callable, a default value, a list of excpetion types, an arg tuple, and a kwarg dict and calls the callable, catching the exceptions specified, and returning the function value on success, the default value on a known caught exception, and allowing any other none-accounted for exceptions bubble up.
 
+---
+
 ```python
 rreduce(
     reduction: Callable[[R, E], R],
     indexable: Indexable,
     initvalue: Union[R, Sentinel] = sentinel
 ) -> R
 ```
@@ -69,7 +73,23 @@
 ```python
 from typing import Protocol
 
 class Indexable(Protocol):
   def __getitem__(self, index: int) -> Any: ...
   def __len__(self) -> int: ...
 ```
+
+---
+
+```python
+def commute(fn: Callable[[S, T], R]) -> Callable[[T, S], R]
+```
+
+Commutes the operands of a binary function. Does not (yet) work for varargs or functions other than 2-arity
+
+---
+
+```python
+def identity(x: T) -> T
+```
+
+The identity function
```

### Comparing `pyfunctional-elunico-0.8.1/setup.py` & `pyfunctional-elunico-0.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfunctional-elunico",
-    version="0.8.1",
+    version="0.9.0",
     author="Thomas Povinelli",
     author_email="tompov227@gmail.com",
     description="A small collection of functions I find useful",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/elunico/pyfunctional",
```

