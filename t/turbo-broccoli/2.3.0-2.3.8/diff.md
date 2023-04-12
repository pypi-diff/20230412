# Comparing `tmp/turbo_broccoli-2.3.0.tar.gz` & `tmp/turbo_broccoli-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_broccoli-2.3.0.tar", last modified: Fri Mar 31 03:58:37 2023, max compression
+gzip compressed data, was "turbo_broccoli-2.3.8.tar", last modified: Wed Apr 12 04:11:51 2023, max compression
```

## Comparing `turbo_broccoli-2.3.0.tar` & `turbo_broccoli-2.3.8.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:58:37.622752 turbo_broccoli-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-03-31 03:58:37.622752 turbo_broccoli-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 03:58:37.622752 turbo_broccoli-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:58:37.618752 turbo_broccoli-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25383 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_bokeh.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_nodecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    52428 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/tests/test_tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:58:37.622752 turbo_broccoli-2.3.0/turbo_broccoli/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/bokeh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/guard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13472 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/turbo_broccoli.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-31 03:58:28.000000 turbo_broccoli-2.3.0/turbo_broccoli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 03:58:37.622752 turbo_broccoli-2.3.0/turbo_broccoli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-03-31 03:58:37.000000 turbo_broccoli-2.3.0/turbo_broccoli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-31 03:58:37.000000 turbo_broccoli-2.3.0/turbo_broccoli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 03:58:37.000000 turbo_broccoli-2.3.0/turbo_broccoli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-31 03:58:37.000000 turbo_broccoli-2.3.0/turbo_broccoli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:11:51.169348 turbo_broccoli-2.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18239 2023-04-12 04:11:51.169348 turbo_broccoli-2.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 04:11:51.169348 turbo_broccoli-2.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:11:51.165347 turbo_broccoli-2.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25383 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_nodecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52428 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:11:51.169348 turbo_broccoli-2.3.8/turbo_broccoli/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/turbo_broccoli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:11:51.169348 turbo_broccoli-2.3.8/turbo_broccoli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18239 2023-04-12 04:11:51.000000 turbo_broccoli-2.3.8/turbo_broccoli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-12 04:11:51.000000 turbo_broccoli-2.3.8/turbo_broccoli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:11:51.000000 turbo_broccoli-2.3.8/turbo_broccoli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 04:11:51.000000 turbo_broccoli-2.3.8/turbo_broccoli.egg-info/top_level.txt
```

### Comparing `turbo_broccoli-2.3.0/LICENSE` & `turbo_broccoli-2.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/PKG-INFO` & `turbo_broccoli-2.3.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: turbo_broccoli
-Version: 2.3.0
-Summary: JSON (de)serialization extensions
-Home-page: https://github.com/altaris/turbo-broccoli
-Author: Cédric Ho Thanh
-Author-email: altaris@users.noreply.github.com
-Project-URL: Issues, https://github.com/altaris/turbo-broccoli/issues
-Platform: any
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Turbo Broccoli 🥦
 
 [![PyPI](https://img.shields.io/pypi/v/turbo-broccoli)](https://pypi.org/project/turbo-broccoli/)
 ![License](https://img.shields.io/github/license/altaris/turbo-broccoli)
 [![Code
 style](https://img.shields.io/badge/style-black-black)](https://pypi.org/project/black)
 ![hehe](https://img.shields.io/badge/project%20name%20by-github-pink)
@@ -74,219 +56,187 @@
 ```py
 json.loads(json_string, cls=tb.TurboBroccoliDecoder)
 
 # or even simpler:
 tb.from_json(json_string)
 ```
 
-## Guarded calls
-
-Consider an expensive function `f` that returns a TurboBroccoli/JSON-izable
-`dict`. Wrapping/decorating `f` using `produces_document` essentially saves the
-result at a specified path and when possible, loads it instead of calling `f`.
-For example:
-
-```py
-_f = produces_document(f, "foo.json")
-_f(*args, **kwargs)
-```
-
-will only call `f` if the `foo.json` does not exist, and otherwise, loads and
-returns `foo.json`. However, if `foo.json` exists and was produced by calling
-`_f(*args, **kwargs)`, then
-
-```py
-_f(*args2, **kwargs2)
-```
-
-will still return the same result. If you want to keep a different file for
-each `args`/`kwargs`, set `check_args` to `True` as in
-
-```py
-_f = produces_document(f, "foo.json")
-_f(*args, **kwargs)
-```
-
-In this case, the arguments must be TurboBroccoli/JSON-izable, i.e. the
-document
-
-```
-{
-    "args": args,
-    "kwargs": kwargs,
-}
-```
-
-must be TurboBroccoli/JSON-izable. The resulting file is no longer
-`foo.json` but rather `foo.json/<hash>` where `hash` is the MD5
-hash of the serialization of the `args`/`kwargs` document above.
-
-If instead of a function you wish to guard an entire block of code, use
-`GuardedBlockHandler`:
-
-```py
-from turbo_broccoli import GuardedBlockHandler
-h = GuardedBlockHandler("foo.json")
-for _ in h.guard():
-    # This whole block will be skipped if foo.json exists
-    # If not, don't forget to set the results:
-    h.result = ...
-# In any case, the results of the block are now available in h.result
-```
-
-I know the syntax isn't the prettiest. It would be more natural to use a `with
-h.guard():` syntax but python doesn't allow for context managers that don't
-yield...
-
 ## Supported types
 
-- `bytes`
+### Basic types
+
+- [`bytes`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/bytes.html#to_json)
 
-- `collections.deque`, `collections.namedtuple`
+- `dict` with non `str` keys
 
-- Dataclasses. Serialization is straightforward:
+- [Collections](https://altaris.github.io/turbo-broccoli/turbo_broccoli/collections.html#to_json):
+  `collections.deque`, `collections.namedtuple`
 
+- [Dataclasses](https://altaris.github.io/turbo-broccoli/turbo_broccoli/dataclass.html#to_json): serialization is straightforward:
   ```py
   @dataclass
   class C:
       a: int
       b: str
 
   doc = json.dumps({"c": C(a=1, b="Hello")}, cls=tb.TurboBroccoliEncoder)
   ```
-
   For deserialization, first register the class:
-
   ```py
   tb.register_dataclass_type(C)
   json.loads(doc, cls=tb.TurboBroccoliDecoder)
   ```
 
-- _Generic object_, **serialization only**. A generic object is an object that
-  has the `__turbo_broccoli__` attribute. This attribute is expected to be a
-  list of attributes whose values will be serialized. For example,
-
-  ```py
-  class C:
-      __turbo_broccoli__ = ["a"]
-      a: int
-      b: int
-
-  x = C()
-  x.a, x.b = 42, 43
-  json.dumps(x, cls=tb.TurboBroccoliEncoder)
-  ```
+### [Generic objects](https://altaris.github.io/turbo-broccoli/turbo_broccoli/generic.html#to_json)
 
-  produces the following string (modulo indentation):
+**serialization only**. A generic object is an object that
+has the `__turbo_broccoli__` attribute. This attribute is expected to be a list
+of attributes whose values will be serialized. For example,
+```py
+class C:
+    __turbo_broccoli__ = ["a"]
+    a: int
+    b: int
 
-  ```json
-  {
-    "__generic__": {
-      "__version__": 1,
-      "data": {
-        "a": 42
-      }
+x = C()
+x.a, x.b = 42, 43
+json.dumps(x, cls=tb.TurboBroccoliEncoder)
+```
+produces the following string (modulo indentation):
+```json
+{
+  "__generic__": {
+    "__version__": 1,
+    "data": {
+      "a": 42
     }
   }
-  ```
+}
+```
+
+Registered attributes can of course have any type supported by Turbo Broccoli,
+such as numpy arrays. Registered attributes can be `@property` methods.
 
-  Registered attributes can of course have any type supported by Turbo
-  Broccoli, such as numpy arrays. Registered attributes can be `@property`
-  methods.
+### [Keras](https://altaris.github.io/turbo-broccoli/turbo_broccoli/keras.html#to_json)
 
-- [`keras.Model`](https://keras.io/api/models/model/); standard subclasses of
-  [`keras.layers.Layer`](https://keras.io/api/layers/),
+- [`keras.Model`](https://keras.io/api/models/model/);
+
+- standard subclasses of [`keras.layers.Layer`](https://keras.io/api/layers/),
   [`keras.losses.Loss`](https://keras.io/api/losses/),
   [`keras.metrics.Metric`](https://keras.io/api/metrics/), and
-  [`keras.optimizers.Optimizer`](https://keras.io/api/optimizers/)
+  [`keras.optimizers.Optimizer`](https://keras.io/api/optimizers/).
+
+### [Numpy](https://altaris.github.io/turbo-broccoli/turbo_broccoli/numpy.html#to_json)
 
-- `numpy.number`, `numpy.ndarray` with numerical dtype
+`numpy.number`, `numpy.ndarray` with numerical dtype, and `numpy.dtype`.
 
-- `pandas.DataFrame` and `pandas.Series`, but with the following limitations:
+### [Pandas](https://altaris.github.io/turbo-broccoli/turbo_broccoli/pandas.html#to_json)
 
-  1. the following dtypes are not supported: `complex`, `object`, `timedelta`
-  2. the column / series names must be strings and not numbers. The following
-     is not acceptable:
-     ```py
-     df = pd.DataFrame([[1, 2], [3, 4]])
-     ```
-     because
-     ```py
-     print([c for c in df.columns])
-     # [0, 1]
-     print([type(c) for c in df.columns])
-     # [int, int]
-     ```
+`pandas.DataFrame` and `pandas.Series`, but with the following limitations:
 
-- `tensorflow.Tensor` with numerical dtype, but not `tensorflow.RaggedTensor`
+- the following dtypes are not supported: `complex`, `object`, `timedelta`
 
-- `torch.Tensor`, **WARNING**: loaded tensors are automatically placed on the
-  CPU and gradients are lost; `torch.nn.Module`, don't forget to register your
+- the column / series names must be strings and not numbers. The following
+  is not acceptable:
+  ```py
+  df = pd.DataFrame([[1, 2], [3, 4]])
+  ```
+  because
+  ```py
+  print([c for c in df.columns])
+  # [0, 1]
+  print([type(c) for c in df.columns])
+  # [int, int]
+  ```
+
+### [Tensorflow](https://altaris.github.io/turbo-broccoli/turbo_broccoli/tensorflow.html#to_json)
+
+`tensorflow.Tensor` with numerical dtype, but not `tensorflow.RaggedTensor`.
+
+### [Pytorch](https://altaris.github.io/turbo-broccoli/turbo_broccoli/pytorch.html#to_json)
+
+- `torch.Tensor`, **Warning**: loaded tensors are automatically placed on the
+  CPU and gradients are lost;
+
+- `torch.nn.Module`, don't forget to register your
   module type using
-  [`turbo_broccoli.register_pytorch_module_type`]((https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#register_pytorch_module_type)):
-     ```py
-     # Serialization
-     class MyModule(torch.nn.Module):
-        ...
-
-     module = MyModule()  # Must be instantiable without arguments
-     doc = json.dumps(x, cls=tb.TurboBroccoliEncoder)
-
-     # Deserialization
-     tb.register_pytorch_module_type(MyModule)
-     module = json.loads(doc, cls=tb.TurboBroccoliDecoder)
-     ```
-  **WARNING**: It is not possible to register and deserialize [standard pytorch
+  [`turbo_broccoli.register_pytorch_module_type`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#register_pytorch_module_type):
+  ```py
+  # Serialization
+  class MyModule(torch.nn.Module):
+    ...
+
+  module = MyModule()  # Must be instantiable without arguments
+  doc = json.dumps(x, cls=tb.TurboBroccoliEncoder)
+
+  # Deserialization
+  tb.register_pytorch_module_type(MyModule)
+  module = json.loads(doc, cls=tb.TurboBroccoliDecoder)
+  ```
+  **Warning**: It is not possible to register and deserialize [standard pytorch
   module containers](https://pytorch.org/docs/stable/nn.html#containers)
   directly. Wrap them in your own custom module class.
 
-- `scipy.sparse.csr_matrix`
+### [Scipy](https://altaris.github.io/turbo-broccoli/turbo_broccoli/scipy.html#to_json)
+
+Just `scipy.sparse.csr_matrix`. ^^"
+
+### [Scikit-learn](https://altaris.github.io/turbo-broccoli/turbo_broccoli/sklearn.html#to_json)
+
+`sklearn` estimators (i.e. that descent from
+[`sklean.base.BaseEstimator`](https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html)).
+To make sure which class is supported, take a look at the [unit
+tests](https://github.com/altaris/turbo-broccoli/blob/main/tests/test_sklearn.py)
+Doesn't work with:
+
+- All CV classes because the `score_` attribute is a dict indexed with
+  `np.int64`, which `json.JSONEncoder._iterencode_dict` rejects.
+
+- All estimator classes that have mandatory arguments: `ClassifierChain`,
+  `ColumnTransformer`, `FeatureUnion`, `GridSearchCV`,
+  `MultiOutputClassifier`, `MultiOutputRegressor`, `OneVsOneClassifier`,
+  `OneVsRestClassifier`, `OutputCodeClassifier`, `Pipeline`,
+  `RandomizedSearchCV`, `RegressorChain`, `RFE`, `RFECV`, `SelectFromModel`,
+  `SelfTrainingClassifier`, `SequentialFeatureSelector`, `SparseCoder`,
+  `StackingClassifier`, `StackingRegressor`, `VotingClassifier`,
+  `VotingRegressor`.
+
+- Everything that is parametrized by an arbitrary object/callable/estimator:
+  `FunctionTransformer`, `TransformedTargetRegressor`.
+
+- Everything that stores a random state (in the form of a `RandomState`
+  object): `BisectingKMeans`, `MiniBatchDictionaryLearning`,
+  `LatentDirichletAllocation`, `NeighborhoodComponentsAnalysis`,
+  `MLPClassifier`, `MLPRegressor`, `SparseRandomProjection`,
+  `GaussianRandomProjection`.
+
+- Everything with trees and forest since `Tree` objects are not JSON
+  serializable: `ExtraTreesClassifier`, `ExtraTreesRegressor`,
+  `RandomForestClassifier`, `RandomForestRegressor`, `RandomTreesEmbedding`,
+  `IsolationForest`, `AdaBoostClassifier`, `AdaBoostRegressor`,
+  `DecisionTreeClassifier`, `DecisionTreeRegressor`.
+
+- Other classes that have non JSON-serializable attributes:
 
-- **EXPERIMENTAL** `sklearn` estimators (i.e. that descent from
-  [`sklean.base.BaseEstimator`](https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html)).
-  To make sure which class is supported, take a look at the [unit
-  tests](https://github.com/altaris/turbo-broccoli/blob/main/tests/test_sklearn.py)
-  Doesn't work with:
-  * All CV classes because the `score_` attribute is a dict indexed with
-    `np.int64`, which `json.JSONEncoder._iterencode_dict` rejects.
-  * All estimator classes that have mandatory arguments: `ClassifierChain`,
-    `ColumnTransformer`, `FeatureUnion`, `GridSearchCV`,
-    `MultiOutputClassifier`, `MultiOutputRegressor`, `OneVsOneClassifier`,
-    `OneVsRestClassifier`, `OutputCodeClassifier`, `Pipeline`,
-    `RandomizedSearchCV`, `RegressorChain`, `RFE`, `RFECV`, `SelectFromModel`,
-    `SelfTrainingClassifier`, `SequentialFeatureSelector`, `SparseCoder`,
-    `StackingClassifier`, `StackingRegressor`, `VotingClassifier`,
-    `VotingRegressor`.
-  * Everything that is parametrized by an arbitrary object/callable/estimator:
-    `FunctionTransformer`, `TransformedTargetRegressor`.
-  * Everything that stores a random state (in the form of a `RandomState`
-    object): `BisectingKMeans`, `MiniBatchDictionaryLearning`,
-    `LatentDirichletAllocation`, `NeighborhoodComponentsAnalysis`,
-    `MLPClassifier`, `MLPRegressor`, `SparseRandomProjection`,
-    `GaussianRandomProjection`.
-  * Everything with trees and forest since `Tree` objects are not JSON
-    serializable: `ExtraTreesClassifier`, `ExtraTreesRegressor`,
-    `RandomForestClassifier`, `RandomForestRegressor`, `RandomTreesEmbedding`,
-    `IsolationForest`, `AdaBoostClassifier`, `AdaBoostRegressor`,
-    `DecisionTreeClassifier`, `DecisionTreeRegressor`.
-  * Other classes that have non JSON-serializable attributes:
     | Class                       | Non-serializable attr.    |
     | --------------------------- | ------------------------- |
     | `Birch`                     | `_CFNode`                 |
     | `GaussianProcessRegressor`  | `Sum`                     |
     | `GaussianProcessClassifier` | `Product`                 |
     | `Perceptron`                | `Hinge`                   |
     | `SGDClassifier`             | `Hinge`                   |
     | `SGDOneClassSVM`            | `Hinge`                   |
     | `PoissonRegressor`          | `HalfPoissonLoss`         |
     | `GammaRegressor`            | `HalfGammaLoss`           |
     | `TweedieRegressor`          | `HalfTweedieLossIdentity` |
     | `KernelDensity`             | `KDTree`                  |
     | `SplineTransformer`         | `BSpline`                 |
-  * Some classes have AttributeErrors?
+
+- Some classes have `AttributeErrors`?
+
     | Class                         | Attribute      |
     | ----------------------------- | -------------- |
     | `IsotonicRegression`          | `f_`           |
     | `KernelPCA`                   | `_centerer`    |
     | `KNeighborsClassifier`        | `_y`           |
     | `KNeighborsRegressor`         | `_y`           |
     | `KNeighborsTransformer`       | `_tree`        |
@@ -299,46 +249,53 @@
     | `OneClassSVM`                 | `_sparse`      |
     | `PowerTransformer`            | `_scaler`      |
     | `RadiusNeighborsClassifier`   | `_tree`        |
     | `RadiusNeighborsRegressor`    | `_tree`        |
     | `RadiusNeighborsTransformer`  | `_tree`        |
     | `SVC`                         | `_sparse`      |
     | `SVR`                         | `_sparse`      |
-  * Other errors:
-    * `FastICA`: I'm not sure why...
-    * `BaggingClassifier`: `IndexError: only integers, slices (:), ellipsis
-      (...), numpy.newaxis (None) and integer or boolean arrays are valid
-      indices`.
-    * `GradientBoostingClassifier`: `Exception: dtype object is not covered`.
-    * `GradientBoostingRegressor`: `Exception: dtype object is not covered`.
-    * `HistGradientBoostingClassifier`: Problems with deserialization of
-      `_BinMapper` object?
-    * `PassiveAggressiveClassifier`: some unknown label type error...
-    * `KBinsDiscretizer`: `Exception: dtype object is not covered`.
-    * `KBinsDiscretizer`: `Exception: dtype object is not covered`.
 
-- [Bokeh figures](https://docs.bokeh.org/en/latest) and
-  [models](https://docs.bokeh.org/en/latest/docs/reference/models.html).
+- Other errors:
 
-## Secrets
+  - `FastICA`: I'm not sure why...
+
+  - `BaggingClassifier`: `IndexError: only integers, slices (:), ellipsis
+    (...), numpy.newaxis (None) and integer or boolean arrays are valid
+    indices`.
+
+  - `GradientBoostingClassifier`, `GradientBoostingRegressor`: `Exception:
+    dtype object is not covered`.
+
+  - `HistGradientBoostingClassifier`: Problems with deserialization of
+    `_BinMapper` object?
+
+  - `PassiveAggressiveClassifier`: some unknown label type error...
+
+  - `KBinsDiscretizer`: `Exception: dtype object is not covered`.
+
+### [Bokeh](https://altaris.github.io/turbo-broccoli/turbo_broccoli/bokeh.html#to_json)
+
+Bokeh [figures](https://docs.bokeh.org/en/latest) and
+[models](https://docs.bokeh.org/en/latest/docs/reference/models.html).
+
+## [Secrets](https://altaris.github.io/turbo-broccoli/turbo_broccoli/secret.html#to_json)
 
 Basic Python types can be wrapped in their corresponding secret type according
 to the following table
 
 | Python type | Secret type                         |
 | ----------- | ----------------------------------- |
 | `dict`      | `turbo_broccoli.secret.SecretDict`  |
 | `float`     | `turbo_broccoli.secret.SecretFloat` |
 | `int`       | `turbo_broccoli.secret.SecretInt`   |
 | `list`      | `turbo_broccoli.secret.SecretList`  |
 | `str`       | `turbo_broccoli.secret.SecretStr`   |
 
 The secret value can be recovered with the `get_secret_value` method. At
 serialization, the this value will be encrypted. For example,
-
 ```py
 # See https://pynacl.readthedocs.io/en/latest/secret/#key
 import nacl.secret
 import nacl.utils
 
 key = nacl.utils.random(nacl.secret.SecretBox.KEY_SIZE)
 
@@ -349,18 +306,16 @@
 
 x = {
     "user": "alice",
     "password": SecretStr("dolphin")
 }
 json.dumps(x, cls=tb.TurboBroccoliEncoder)
 ```
-
 produces the following string (modulo indentation and modulo the encrypted
 content):
-
 ```json
 {
   "user": "alice",
   "password": {
     "__secret__": {
       "__version__": 1,
       "data": {
@@ -376,15 +331,15 @@
 
 Deserialization decrypts the secrets, but they stay wrapped inside the secret
 types above. If the wrong key is provided, an exception is raised. If no key is
 provided, the secret values are replaced by a
 `turbo_broccoli.secret.LockedSecret`. Internally, Turbo Broccoli uses
 [`pynacl`](https://pynacl.readthedocs.io/en/latest/)'s
 [`SecretBox`](https://pynacl.readthedocs.io/en/latest/secret/#nacl.secret.SecretBox).
-**WARNING**: In the case of `SecretDict` and `SecretList`, the values contained
+**Warning**: In the case of `SecretDict` and `SecretList`, the values contained
 within must be JSON-serializable **without** Turbo Broccoli. See also the
 `TB_SHARED_KEY` environment variable below.
 
 ## Environment variables
 
 Some behaviors of Turbo Broccoli can be tweaked by setting specific environment
 variables. If you want to modify these parameters programatically, do not do so
@@ -393,34 +348,30 @@
 
 - `TB_ARTIFACT_PATH` (default: `./`; see also
   [`turbo_broccoli.set_artifact_path`]((https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#set_artifact_path)),
   [`turbo_broccoli.environment.get_artifact_path`]((https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#get_artifact_path))):
   During serialization, Turbo Broccoli may create artifacts to which the JSON
   object will point to. The artifacts will be stored in `TB_ARTIFACT_PATH`. For
   example, if `arr` is a big numpy array,
-
   ```py
   obj = {"an_array": arr}
   json.dumps(obj, cls=tb.TurboBroccoliEncoder)
   ```
-
   will generate the following string (modulo indentation and id)
-
   ```json
   {
       "an_array": {
           "__numpy__": {
               "__type__": "ndarray",
               "__version__": 3,
               "id": "70692d08-c4cf-4231-b3f0-0969ea552d5a"
           }
       }
   }
   ```
-
   and a `70692d08-c4cf-4231-b3f0-0969ea552d5a` file has been created in
   `TB_ARTIFACT_PATH`.
 
 - `TB_KERAS_FORMAT` (default: `tf`, valid values are `json`, `h5`, and `tf`;
   see also
   [`turbo_broccoli.set_keras_format`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#set_keras_format),
   [`turbo_broccoli.environment.get_keras_format`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#get_keras_format)):
@@ -440,87 +391,111 @@
 
 - `TB_NODECODE` (default: empty; see also
   [`turbo_broccoli.set_nodecode`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#set_nodecode),
   [`turbo_broccoli.environment.is_nodecode`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#is_nodecode)):
   Comma-separated list of types to not deserialize, for example
   `bytes,numpy.ndarray`. Excludable types are:
 
+  - `bokeh`, `bokeh.buffer`, `bokeh.generic`,
+
   - `bytes`,
-  - `dataclass.<dataclass_name>` (case sensitive),
-  - `collections.deque`, `collections.namedtuple`,
-  - `keras.model`, `keras.layer`, `keras.loss`, `keras.metric`,
+
+  - `dict`,
+
+  - `collections`, `collections.deque`, `collections.namedtuple`,
+
+  - `dataclass`, `dataclass.<dataclass_name>` (case sensitive),
+
+  - `generic`,
+
+  - `keras`, `keras.model`, `keras.layer`, `keras.loss`, `keras.metric`,
     `keras.optimizer`,
-  - `numpy.ndarray`, `numpy.number`,
-  - `pandas.dataframe`, `pandas.series`, **WARNING: excluding
-    `pandas.dataframe` will crash any deserialization of `pandas.series`**
-  - `tensorflow.sparse_tensor`, `tensorflow.tensor`, `tensorflow.variable`.
-    **WARNING**: excluding `numpy.ndarray` will may crash deserialization of
-    Tensorflow and Pandas types.
+
+  - `numpy`, `numpy.ndarray`, `numpy.number`, `numpy.dtype`,
+
+  - `pandas`, `pandas.dataframe`, `pandas.series`, **Warning**: excluding
+    `pandas.dataframe` will crash any deserialization of `pandas.series`,
+
+  - `pytorch`, `pytorch.tensor`, `pytorch.module`,
+
+  - `scipy`, `scipy.csr_matrix`,
+
+  - `secret`,
+
+  - `sklearn`, `sklearn.estimator`, `sklearn.estimator.<estimator name>` (case
+    sensitive, see the list of supported sklearn estimators), `sklearn.tree`,
+
+  - `tensorflow`, `tensorflow.sparse_tensor`, `tensorflow.tensor`,
+    `tensorflow.variable`.
 
 - `TB_SHARED_KEY` (default: empty; see also
   [`turbo_broccoli.set_shared_key`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#set_shared_key),
   [`turbo_broccoli.environment.get_shared_key`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#get_shared_key)):
   Secret key used to encrypt secrets. The encryption uses [`pynacl`'s
   `SecretBox`](https://pynacl.readthedocs.io/en/latest/secret/#nacl.secret.SecretBox).
   An exception is raised when attempting to serialize a secret type while no
   key is set.
 
+## Guarded calls
+
+This is so cool. Check out
+[`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler),
+[`turbo_broccoli.guarded_call`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#guarded_call),
+and
+[`turbo_broccoli.produces_document`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#produces_document).
+
 # Contributing
 
 ## Dependencies
 
 - `python3.9` or newer;
+
 - `requirements.txt` for runtime dependencies;
+
 - `requirements.dev.txt` for development dependencies.
+
 - `make` (optional);
 
 Simply run
-
 ```sh
 virtualenv venv -p python3.9
 . ./venv/bin/activate
 pip install --upgrade pip
 pip install -r requirements.txt
 pip install -r requirements.dev.txt
 ```
 
 ## Documentation
 
 Simply run
-
 ```sh
 make docs
 ```
 
 This will generate the HTML doc of the project, and the index file should be at
 `docs/index.html`. To have it directly in your browser, run
-
 ```sh
 make docs-browser
 ```
 
 ## Code quality
 
 Don't forget to run
-
 ```sh
 make
 ```
-
 to format the code following [black](https://pypi.org/project/black/),
 typecheck it using [mypy](http://mypy-lang.org/), and check it against coding
 standards using [pylint](https://pylint.org/).
 
 ## Unit tests
 
 Run
-
 ```sh
 make test
 ```
-
 to have [pytest](https://docs.pytest.org/) run the unit tests in `tests/`.
 
 # Credits
 
 This project takes inspiration from
 [Crimson-Crow/json-numpy](https://github.com/Crimson-Crow/json-numpy).
```

### Comparing `turbo_broccoli-2.3.0/README.md` & `turbo_broccoli-2.3.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: turbo_broccoli
+Version: 2.3.8
+Summary: JSON (de)serialization extensions
+Home-page: https://github.com/altaris/turbo-broccoli
+Author: Cédric Ho Thanh
+Author-email: altaris@users.noreply.github.com
+Project-URL: Issues, https://github.com/altaris/turbo-broccoli/issues
+Platform: any
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Turbo Broccoli 🥦
 
 [![PyPI](https://img.shields.io/pypi/v/turbo-broccoli)](https://pypi.org/project/turbo-broccoli/)
 ![License](https://img.shields.io/github/license/altaris/turbo-broccoli)
 [![Code
 style](https://img.shields.io/badge/style-black-black)](https://pypi.org/project/black)
 ![hehe](https://img.shields.io/badge/project%20name%20by-github-pink)
@@ -56,219 +74,187 @@
 ```py
 json.loads(json_string, cls=tb.TurboBroccoliDecoder)
 
 # or even simpler:
 tb.from_json(json_string)
 ```
 
-## Guarded calls
-
-Consider an expensive function `f` that returns a TurboBroccoli/JSON-izable
-`dict`. Wrapping/decorating `f` using `produces_document` essentially saves the
-result at a specified path and when possible, loads it instead of calling `f`.
-For example:
-
-```py
-_f = produces_document(f, "foo.json")
-_f(*args, **kwargs)
-```
-
-will only call `f` if the `foo.json` does not exist, and otherwise, loads and
-returns `foo.json`. However, if `foo.json` exists and was produced by calling
-`_f(*args, **kwargs)`, then
-
-```py
-_f(*args2, **kwargs2)
-```
-
-will still return the same result. If you want to keep a different file for
-each `args`/`kwargs`, set `check_args` to `True` as in
-
-```py
-_f = produces_document(f, "foo.json")
-_f(*args, **kwargs)
-```
-
-In this case, the arguments must be TurboBroccoli/JSON-izable, i.e. the
-document
-
-```
-{
-    "args": args,
-    "kwargs": kwargs,
-}
-```
-
-must be TurboBroccoli/JSON-izable. The resulting file is no longer
-`foo.json` but rather `foo.json/<hash>` where `hash` is the MD5
-hash of the serialization of the `args`/`kwargs` document above.
-
-If instead of a function you wish to guard an entire block of code, use
-`GuardedBlockHandler`:
-
-```py
-from turbo_broccoli import GuardedBlockHandler
-h = GuardedBlockHandler("foo.json")
-for _ in h.guard():
-    # This whole block will be skipped if foo.json exists
-    # If not, don't forget to set the results:
-    h.result = ...
-# In any case, the results of the block are now available in h.result
-```
-
-I know the syntax isn't the prettiest. It would be more natural to use a `with
-h.guard():` syntax but python doesn't allow for context managers that don't
-yield...
-
 ## Supported types
 
-- `bytes`
+### Basic types
+
+- [`bytes`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/bytes.html#to_json)
 
-- `collections.deque`, `collections.namedtuple`
+- `dict` with non `str` keys
 
-- Dataclasses. Serialization is straightforward:
+- [Collections](https://altaris.github.io/turbo-broccoli/turbo_broccoli/collections.html#to_json):
+  `collections.deque`, `collections.namedtuple`
 
+- [Dataclasses](https://altaris.github.io/turbo-broccoli/turbo_broccoli/dataclass.html#to_json): serialization is straightforward:
   ```py
   @dataclass
   class C:
       a: int
       b: str
 
   doc = json.dumps({"c": C(a=1, b="Hello")}, cls=tb.TurboBroccoliEncoder)
   ```
-
   For deserialization, first register the class:
-
   ```py
   tb.register_dataclass_type(C)
   json.loads(doc, cls=tb.TurboBroccoliDecoder)
   ```
 
-- _Generic object_, **serialization only**. A generic object is an object that
-  has the `__turbo_broccoli__` attribute. This attribute is expected to be a
-  list of attributes whose values will be serialized. For example,
-
-  ```py
-  class C:
-      __turbo_broccoli__ = ["a"]
-      a: int
-      b: int
-
-  x = C()
-  x.a, x.b = 42, 43
-  json.dumps(x, cls=tb.TurboBroccoliEncoder)
-  ```
+### [Generic objects](https://altaris.github.io/turbo-broccoli/turbo_broccoli/generic.html#to_json)
 
-  produces the following string (modulo indentation):
+**serialization only**. A generic object is an object that
+has the `__turbo_broccoli__` attribute. This attribute is expected to be a list
+of attributes whose values will be serialized. For example,
+```py
+class C:
+    __turbo_broccoli__ = ["a"]
+    a: int
+    b: int
 
-  ```json
-  {
-    "__generic__": {
-      "__version__": 1,
-      "data": {
-        "a": 42
-      }
+x = C()
+x.a, x.b = 42, 43
+json.dumps(x, cls=tb.TurboBroccoliEncoder)
+```
+produces the following string (modulo indentation):
+```json
+{
+  "__generic__": {
+    "__version__": 1,
+    "data": {
+      "a": 42
     }
   }
-  ```
+}
+```
+
+Registered attributes can of course have any type supported by Turbo Broccoli,
+such as numpy arrays. Registered attributes can be `@property` methods.
 
-  Registered attributes can of course have any type supported by Turbo
-  Broccoli, such as numpy arrays. Registered attributes can be `@property`
-  methods.
+### [Keras](https://altaris.github.io/turbo-broccoli/turbo_broccoli/keras.html#to_json)
 
-- [`keras.Model`](https://keras.io/api/models/model/); standard subclasses of
-  [`keras.layers.Layer`](https://keras.io/api/layers/),
+- [`keras.Model`](https://keras.io/api/models/model/);
+
+- standard subclasses of [`keras.layers.Layer`](https://keras.io/api/layers/),
   [`keras.losses.Loss`](https://keras.io/api/losses/),
   [`keras.metrics.Metric`](https://keras.io/api/metrics/), and
-  [`keras.optimizers.Optimizer`](https://keras.io/api/optimizers/)
+  [`keras.optimizers.Optimizer`](https://keras.io/api/optimizers/).
+
+### [Numpy](https://altaris.github.io/turbo-broccoli/turbo_broccoli/numpy.html#to_json)
 
-- `numpy.number`, `numpy.ndarray` with numerical dtype
+`numpy.number`, `numpy.ndarray` with numerical dtype, and `numpy.dtype`.
 
-- `pandas.DataFrame` and `pandas.Series`, but with the following limitations:
+### [Pandas](https://altaris.github.io/turbo-broccoli/turbo_broccoli/pandas.html#to_json)
 
-  1. the following dtypes are not supported: `complex`, `object`, `timedelta`
-  2. the column / series names must be strings and not numbers. The following
-     is not acceptable:
-     ```py
-     df = pd.DataFrame([[1, 2], [3, 4]])
-     ```
-     because
-     ```py
-     print([c for c in df.columns])
-     # [0, 1]
-     print([type(c) for c in df.columns])
-     # [int, int]
-     ```
+`pandas.DataFrame` and `pandas.Series`, but with the following limitations:
 
-- `tensorflow.Tensor` with numerical dtype, but not `tensorflow.RaggedTensor`
+- the following dtypes are not supported: `complex`, `object`, `timedelta`
 
-- `torch.Tensor`, **WARNING**: loaded tensors are automatically placed on the
-  CPU and gradients are lost; `torch.nn.Module`, don't forget to register your
+- the column / series names must be strings and not numbers. The following
+  is not acceptable:
+  ```py
+  df = pd.DataFrame([[1, 2], [3, 4]])
+  ```
+  because
+  ```py
+  print([c for c in df.columns])
+  # [0, 1]
+  print([type(c) for c in df.columns])
+  # [int, int]
+  ```
+
+### [Tensorflow](https://altaris.github.io/turbo-broccoli/turbo_broccoli/tensorflow.html#to_json)
+
+`tensorflow.Tensor` with numerical dtype, but not `tensorflow.RaggedTensor`.
+
+### [Pytorch](https://altaris.github.io/turbo-broccoli/turbo_broccoli/pytorch.html#to_json)
+
+- `torch.Tensor`, **Warning**: loaded tensors are automatically placed on the
+  CPU and gradients are lost;
+
+- `torch.nn.Module`, don't forget to register your
   module type using
-  [`turbo_broccoli.register_pytorch_module_type`]((https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#register_pytorch_module_type)):
-     ```py
-     # Serialization
-     class MyModule(torch.nn.Module):
-        ...
-
-     module = MyModule()  # Must be instantiable without arguments
-     doc = json.dumps(x, cls=tb.TurboBroccoliEncoder)
-
-     # Deserialization
-     tb.register_pytorch_module_type(MyModule)
-     module = json.loads(doc, cls=tb.TurboBroccoliDecoder)
-     ```
-  **WARNING**: It is not possible to register and deserialize [standard pytorch
+  [`turbo_broccoli.register_pytorch_module_type`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#register_pytorch_module_type):
+  ```py
+  # Serialization
+  class MyModule(torch.nn.Module):
+    ...
+
+  module = MyModule()  # Must be instantiable without arguments
+  doc = json.dumps(x, cls=tb.TurboBroccoliEncoder)
+
+  # Deserialization
+  tb.register_pytorch_module_type(MyModule)
+  module = json.loads(doc, cls=tb.TurboBroccoliDecoder)
+  ```
+  **Warning**: It is not possible to register and deserialize [standard pytorch
   module containers](https://pytorch.org/docs/stable/nn.html#containers)
   directly. Wrap them in your own custom module class.
 
-- `scipy.sparse.csr_matrix`
+### [Scipy](https://altaris.github.io/turbo-broccoli/turbo_broccoli/scipy.html#to_json)
+
+Just `scipy.sparse.csr_matrix`. ^^"
+
+### [Scikit-learn](https://altaris.github.io/turbo-broccoli/turbo_broccoli/sklearn.html#to_json)
+
+`sklearn` estimators (i.e. that descent from
+[`sklean.base.BaseEstimator`](https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html)).
+To make sure which class is supported, take a look at the [unit
+tests](https://github.com/altaris/turbo-broccoli/blob/main/tests/test_sklearn.py)
+Doesn't work with:
+
+- All CV classes because the `score_` attribute is a dict indexed with
+  `np.int64`, which `json.JSONEncoder._iterencode_dict` rejects.
+
+- All estimator classes that have mandatory arguments: `ClassifierChain`,
+  `ColumnTransformer`, `FeatureUnion`, `GridSearchCV`,
+  `MultiOutputClassifier`, `MultiOutputRegressor`, `OneVsOneClassifier`,
+  `OneVsRestClassifier`, `OutputCodeClassifier`, `Pipeline`,
+  `RandomizedSearchCV`, `RegressorChain`, `RFE`, `RFECV`, `SelectFromModel`,
+  `SelfTrainingClassifier`, `SequentialFeatureSelector`, `SparseCoder`,
+  `StackingClassifier`, `StackingRegressor`, `VotingClassifier`,
+  `VotingRegressor`.
+
+- Everything that is parametrized by an arbitrary object/callable/estimator:
+  `FunctionTransformer`, `TransformedTargetRegressor`.
+
+- Everything that stores a random state (in the form of a `RandomState`
+  object): `BisectingKMeans`, `MiniBatchDictionaryLearning`,
+  `LatentDirichletAllocation`, `NeighborhoodComponentsAnalysis`,
+  `MLPClassifier`, `MLPRegressor`, `SparseRandomProjection`,
+  `GaussianRandomProjection`.
+
+- Everything with trees and forest since `Tree` objects are not JSON
+  serializable: `ExtraTreesClassifier`, `ExtraTreesRegressor`,
+  `RandomForestClassifier`, `RandomForestRegressor`, `RandomTreesEmbedding`,
+  `IsolationForest`, `AdaBoostClassifier`, `AdaBoostRegressor`,
+  `DecisionTreeClassifier`, `DecisionTreeRegressor`.
+
+- Other classes that have non JSON-serializable attributes:
 
-- **EXPERIMENTAL** `sklearn` estimators (i.e. that descent from
-  [`sklean.base.BaseEstimator`](https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html)).
-  To make sure which class is supported, take a look at the [unit
-  tests](https://github.com/altaris/turbo-broccoli/blob/main/tests/test_sklearn.py)
-  Doesn't work with:
-  * All CV classes because the `score_` attribute is a dict indexed with
-    `np.int64`, which `json.JSONEncoder._iterencode_dict` rejects.
-  * All estimator classes that have mandatory arguments: `ClassifierChain`,
-    `ColumnTransformer`, `FeatureUnion`, `GridSearchCV`,
-    `MultiOutputClassifier`, `MultiOutputRegressor`, `OneVsOneClassifier`,
-    `OneVsRestClassifier`, `OutputCodeClassifier`, `Pipeline`,
-    `RandomizedSearchCV`, `RegressorChain`, `RFE`, `RFECV`, `SelectFromModel`,
-    `SelfTrainingClassifier`, `SequentialFeatureSelector`, `SparseCoder`,
-    `StackingClassifier`, `StackingRegressor`, `VotingClassifier`,
-    `VotingRegressor`.
-  * Everything that is parametrized by an arbitrary object/callable/estimator:
-    `FunctionTransformer`, `TransformedTargetRegressor`.
-  * Everything that stores a random state (in the form of a `RandomState`
-    object): `BisectingKMeans`, `MiniBatchDictionaryLearning`,
-    `LatentDirichletAllocation`, `NeighborhoodComponentsAnalysis`,
-    `MLPClassifier`, `MLPRegressor`, `SparseRandomProjection`,
-    `GaussianRandomProjection`.
-  * Everything with trees and forest since `Tree` objects are not JSON
-    serializable: `ExtraTreesClassifier`, `ExtraTreesRegressor`,
-    `RandomForestClassifier`, `RandomForestRegressor`, `RandomTreesEmbedding`,
-    `IsolationForest`, `AdaBoostClassifier`, `AdaBoostRegressor`,
-    `DecisionTreeClassifier`, `DecisionTreeRegressor`.
-  * Other classes that have non JSON-serializable attributes:
     | Class                       | Non-serializable attr.    |
     | --------------------------- | ------------------------- |
     | `Birch`                     | `_CFNode`                 |
     | `GaussianProcessRegressor`  | `Sum`                     |
     | `GaussianProcessClassifier` | `Product`                 |
     | `Perceptron`                | `Hinge`                   |
     | `SGDClassifier`             | `Hinge`                   |
     | `SGDOneClassSVM`            | `Hinge`                   |
     | `PoissonRegressor`          | `HalfPoissonLoss`         |
     | `GammaRegressor`            | `HalfGammaLoss`           |
     | `TweedieRegressor`          | `HalfTweedieLossIdentity` |
     | `KernelDensity`             | `KDTree`                  |
     | `SplineTransformer`         | `BSpline`                 |
-  * Some classes have AttributeErrors?
+
+- Some classes have `AttributeErrors`?
+
     | Class                         | Attribute      |
     | ----------------------------- | -------------- |
     | `IsotonicRegression`          | `f_`           |
     | `KernelPCA`                   | `_centerer`    |
     | `KNeighborsClassifier`        | `_y`           |
     | `KNeighborsRegressor`         | `_y`           |
     | `KNeighborsTransformer`       | `_tree`        |
@@ -281,46 +267,53 @@
     | `OneClassSVM`                 | `_sparse`      |
     | `PowerTransformer`            | `_scaler`      |
     | `RadiusNeighborsClassifier`   | `_tree`        |
     | `RadiusNeighborsRegressor`    | `_tree`        |
     | `RadiusNeighborsTransformer`  | `_tree`        |
     | `SVC`                         | `_sparse`      |
     | `SVR`                         | `_sparse`      |
-  * Other errors:
-    * `FastICA`: I'm not sure why...
-    * `BaggingClassifier`: `IndexError: only integers, slices (:), ellipsis
-      (...), numpy.newaxis (None) and integer or boolean arrays are valid
-      indices`.
-    * `GradientBoostingClassifier`: `Exception: dtype object is not covered`.
-    * `GradientBoostingRegressor`: `Exception: dtype object is not covered`.
-    * `HistGradientBoostingClassifier`: Problems with deserialization of
-      `_BinMapper` object?
-    * `PassiveAggressiveClassifier`: some unknown label type error...
-    * `KBinsDiscretizer`: `Exception: dtype object is not covered`.
-    * `KBinsDiscretizer`: `Exception: dtype object is not covered`.
 
-- [Bokeh figures](https://docs.bokeh.org/en/latest) and
-  [models](https://docs.bokeh.org/en/latest/docs/reference/models.html).
+- Other errors:
 
-## Secrets
+  - `FastICA`: I'm not sure why...
+
+  - `BaggingClassifier`: `IndexError: only integers, slices (:), ellipsis
+    (...), numpy.newaxis (None) and integer or boolean arrays are valid
+    indices`.
+
+  - `GradientBoostingClassifier`, `GradientBoostingRegressor`: `Exception:
+    dtype object is not covered`.
+
+  - `HistGradientBoostingClassifier`: Problems with deserialization of
+    `_BinMapper` object?
+
+  - `PassiveAggressiveClassifier`: some unknown label type error...
+
+  - `KBinsDiscretizer`: `Exception: dtype object is not covered`.
+
+### [Bokeh](https://altaris.github.io/turbo-broccoli/turbo_broccoli/bokeh.html#to_json)
+
+Bokeh [figures](https://docs.bokeh.org/en/latest) and
+[models](https://docs.bokeh.org/en/latest/docs/reference/models.html).
+
+## [Secrets](https://altaris.github.io/turbo-broccoli/turbo_broccoli/secret.html#to_json)
 
 Basic Python types can be wrapped in their corresponding secret type according
 to the following table
 
 | Python type | Secret type                         |
 | ----------- | ----------------------------------- |
 | `dict`      | `turbo_broccoli.secret.SecretDict`  |
 | `float`     | `turbo_broccoli.secret.SecretFloat` |
 | `int`       | `turbo_broccoli.secret.SecretInt`   |
 | `list`      | `turbo_broccoli.secret.SecretList`  |
 | `str`       | `turbo_broccoli.secret.SecretStr`   |
 
 The secret value can be recovered with the `get_secret_value` method. At
 serialization, the this value will be encrypted. For example,
-
 ```py
 # See https://pynacl.readthedocs.io/en/latest/secret/#key
 import nacl.secret
 import nacl.utils
 
 key = nacl.utils.random(nacl.secret.SecretBox.KEY_SIZE)
 
@@ -331,18 +324,16 @@
 
 x = {
     "user": "alice",
     "password": SecretStr("dolphin")
 }
 json.dumps(x, cls=tb.TurboBroccoliEncoder)
 ```
-
 produces the following string (modulo indentation and modulo the encrypted
 content):
-
 ```json
 {
   "user": "alice",
   "password": {
     "__secret__": {
       "__version__": 1,
       "data": {
@@ -358,15 +349,15 @@
 
 Deserialization decrypts the secrets, but they stay wrapped inside the secret
 types above. If the wrong key is provided, an exception is raised. If no key is
 provided, the secret values are replaced by a
 `turbo_broccoli.secret.LockedSecret`. Internally, Turbo Broccoli uses
 [`pynacl`](https://pynacl.readthedocs.io/en/latest/)'s
 [`SecretBox`](https://pynacl.readthedocs.io/en/latest/secret/#nacl.secret.SecretBox).
-**WARNING**: In the case of `SecretDict` and `SecretList`, the values contained
+**Warning**: In the case of `SecretDict` and `SecretList`, the values contained
 within must be JSON-serializable **without** Turbo Broccoli. See also the
 `TB_SHARED_KEY` environment variable below.
 
 ## Environment variables
 
 Some behaviors of Turbo Broccoli can be tweaked by setting specific environment
 variables. If you want to modify these parameters programatically, do not do so
@@ -375,34 +366,30 @@
 
 - `TB_ARTIFACT_PATH` (default: `./`; see also
   [`turbo_broccoli.set_artifact_path`]((https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#set_artifact_path)),
   [`turbo_broccoli.environment.get_artifact_path`]((https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#get_artifact_path))):
   During serialization, Turbo Broccoli may create artifacts to which the JSON
   object will point to. The artifacts will be stored in `TB_ARTIFACT_PATH`. For
   example, if `arr` is a big numpy array,
-
   ```py
   obj = {"an_array": arr}
   json.dumps(obj, cls=tb.TurboBroccoliEncoder)
   ```
-
   will generate the following string (modulo indentation and id)
-
   ```json
   {
       "an_array": {
           "__numpy__": {
               "__type__": "ndarray",
               "__version__": 3,
               "id": "70692d08-c4cf-4231-b3f0-0969ea552d5a"
           }
       }
   }
   ```
-
   and a `70692d08-c4cf-4231-b3f0-0969ea552d5a` file has been created in
   `TB_ARTIFACT_PATH`.
 
 - `TB_KERAS_FORMAT` (default: `tf`, valid values are `json`, `h5`, and `tf`;
   see also
   [`turbo_broccoli.set_keras_format`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#set_keras_format),
   [`turbo_broccoli.environment.get_keras_format`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#get_keras_format)):
@@ -422,87 +409,111 @@
 
 - `TB_NODECODE` (default: empty; see also
   [`turbo_broccoli.set_nodecode`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#set_nodecode),
   [`turbo_broccoli.environment.is_nodecode`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#is_nodecode)):
   Comma-separated list of types to not deserialize, for example
   `bytes,numpy.ndarray`. Excludable types are:
 
+  - `bokeh`, `bokeh.buffer`, `bokeh.generic`,
+
   - `bytes`,
-  - `dataclass.<dataclass_name>` (case sensitive),
-  - `collections.deque`, `collections.namedtuple`,
-  - `keras.model`, `keras.layer`, `keras.loss`, `keras.metric`,
+
+  - `dict`,
+
+  - `collections`, `collections.deque`, `collections.namedtuple`,
+
+  - `dataclass`, `dataclass.<dataclass_name>` (case sensitive),
+
+  - `generic`,
+
+  - `keras`, `keras.model`, `keras.layer`, `keras.loss`, `keras.metric`,
     `keras.optimizer`,
-  - `numpy.ndarray`, `numpy.number`,
-  - `pandas.dataframe`, `pandas.series`, **WARNING: excluding
-    `pandas.dataframe` will crash any deserialization of `pandas.series`**
-  - `tensorflow.sparse_tensor`, `tensorflow.tensor`, `tensorflow.variable`.
-    **WARNING**: excluding `numpy.ndarray` will may crash deserialization of
-    Tensorflow and Pandas types.
+
+  - `numpy`, `numpy.ndarray`, `numpy.number`, `numpy.dtype`,
+
+  - `pandas`, `pandas.dataframe`, `pandas.series`, **Warning**: excluding
+    `pandas.dataframe` will crash any deserialization of `pandas.series`,
+
+  - `pytorch`, `pytorch.tensor`, `pytorch.module`,
+
+  - `scipy`, `scipy.csr_matrix`,
+
+  - `secret`,
+
+  - `sklearn`, `sklearn.estimator`, `sklearn.estimator.<estimator name>` (case
+    sensitive, see the list of supported sklearn estimators), `sklearn.tree`,
+
+  - `tensorflow`, `tensorflow.sparse_tensor`, `tensorflow.tensor`,
+    `tensorflow.variable`.
 
 - `TB_SHARED_KEY` (default: empty; see also
   [`turbo_broccoli.set_shared_key`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#set_shared_key),
   [`turbo_broccoli.environment.get_shared_key`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#get_shared_key)):
   Secret key used to encrypt secrets. The encryption uses [`pynacl`'s
   `SecretBox`](https://pynacl.readthedocs.io/en/latest/secret/#nacl.secret.SecretBox).
   An exception is raised when attempting to serialize a secret type while no
   key is set.
 
+## Guarded calls
+
+This is so cool. Check out
+[`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler),
+[`turbo_broccoli.guarded_call`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#guarded_call),
+and
+[`turbo_broccoli.produces_document`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#produces_document).
+
 # Contributing
 
 ## Dependencies
 
 - `python3.9` or newer;
+
 - `requirements.txt` for runtime dependencies;
+
 - `requirements.dev.txt` for development dependencies.
+
 - `make` (optional);
 
 Simply run
-
 ```sh
 virtualenv venv -p python3.9
 . ./venv/bin/activate
 pip install --upgrade pip
 pip install -r requirements.txt
 pip install -r requirements.dev.txt
 ```
 
 ## Documentation
 
 Simply run
-
 ```sh
 make docs
 ```
 
 This will generate the HTML doc of the project, and the index file should be at
 `docs/index.html`. To have it directly in your browser, run
-
 ```sh
 make docs-browser
 ```
 
 ## Code quality
 
 Don't forget to run
-
 ```sh
 make
 ```
-
 to format the code following [black](https://pypi.org/project/black/),
 typecheck it using [mypy](http://mypy-lang.org/), and check it against coding
 standards using [pylint](https://pylint.org/).
 
 ## Unit tests
 
 Run
-
 ```sh
 make test
 ```
-
 to have [pytest](https://docs.pytest.org/) run the unit tests in `tests/`.
 
 # Credits
 
 This project takes inspiration from
 [Crimson-Crow/json-numpy](https://github.com/Crimson-Crow/json-numpy).
```

### Comparing `turbo_broccoli-2.3.0/setup.py` & `turbo_broccoli-2.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 """Setup script"""
 
 import setuptools
 
 name = "turbo_broccoli"
-version = "2.3.0"
+version = "2.3.8"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as f:
     requirements = f.read().split()
```

### Comparing `turbo_broccoli-2.3.0/tests/test_bokeh.py` & `turbo_broccoli-2.3.8/tests/test_bokeh.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/tests/test_collections.py` & `turbo_broccoli-2.3.8/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/tests/test_dataclass.py` & `turbo_broccoli-2.3.8/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/tests/test_generic.py` & `turbo_broccoli-2.3.8/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/tests/test_keras.py` & `turbo_broccoli-2.3.8/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/tests/test_nodecode.py` & `turbo_broccoli-2.3.8/tests/test_nodecode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+# pylint: disable=missing-class-docstring
 # pylint: disable=missing-function-docstring
 """Decode exclusion tests"""
 
 from collections import deque
+from dataclasses import dataclass
 
 import numpy as np
 import pandas as pd
 import tensorflow as tf
-from turbo_broccoli.environment import set_nodecode
-
 from common import from_json, to_json
-from test_dataclass import C, D
 from test_keras import _build_model
 from test_pandas import _assert_equal as assert_equal_pd
 
+from turbo_broccoli.environment import register_dataclass_type, set_nodecode
+
 
 def _basic_dict() -> dict:
     return {"a_list": [1, "2", None], "a_str": "abcd", "an_int": 42}
 
 
 def test_nodecode_nothing():
     set_nodecode("")
@@ -30,18 +31,32 @@
     x = {"b": "Hello 🌎".encode("utf8"), **_basic_dict()}
     y = {"b": None, **_basic_dict()}
     assert y == from_json(to_json(x))
     set_nodecode("")
 
 
 def test_nodecode_dataclass():
+    @dataclass
+    class C:
+        a_byte_str: bytes
+        a_list: list
+        a_str: str
+        an_int: int
+
+    @dataclass
+    class D:
+        a_dataclass: C
+        a_float: float
+
+    register_dataclass_type(C)
+    register_dataclass_type(D)
     set_nodecode("dataclass.C")
     c = C(a_byte_str=b"", a_list=[], a_str="", an_int=0)
-    x = {"dcc": c, "dcd": D(a_dataclass=c, a_float=1.2), **_basic_dict()}
-    y = {"dcc": None, "dcd": D(a_dataclass=None, a_float=1.2), **_basic_dict()}
+    x = {"c": c, "d": D(a_dataclass=c, a_float=1.2), **_basic_dict()}
+    y = {"c": None, "d": D(a_dataclass=None, a_float=1.2), **_basic_dict()}
     assert y == from_json(to_json(x))
     set_nodecode("")
 
 
 def test_nodecode_collections():
     set_nodecode("collections.deque")
     x = {"deq": deque(range(100)), **_basic_dict()}
```

### Comparing `turbo_broccoli-2.3.0/tests/test_numpy.py` & `turbo_broccoli-2.3.8/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/tests/test_pandas.py` & `turbo_broccoli-2.3.8/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/tests/test_pytorch.py` & `turbo_broccoli-2.3.8/tests/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/tests/test_scipy.py` & `turbo_broccoli-2.3.8/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/tests/test_secret.py` & `turbo_broccoli-2.3.8/tests/test_secret.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/tests/test_sklearn.py` & `turbo_broccoli-2.3.8/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/tests/test_tensorflow.py` & `turbo_broccoli-2.3.8/tests/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/__init__.py` & `turbo_broccoli-2.3.8/turbo_broccoli/__init__.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/bokeh.py` & `turbo_broccoli-2.3.8/turbo_broccoli/bokeh.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 """Bokeh objects (de)serialization utilities."""
 __docformat__ = "google"
 
 from typing import Any, Callable, List, Tuple
 
-from bokeh.plotting import figure as Figure
+from bokeh.core.serialization import (
+    Buffer,
+    Deserializer,
+    Serialized,
+    Serializer,
+)
 from bokeh.models import Model
-from bokeh.core.serialization import Buffer
-from bokeh.core.serialization import Deserializer, Serialized, Serializer
+from bokeh.plotting import figure as Figure
+
+from turbo_broccoli.utils import (
+    DeserializationError,
+    TypeNotSupported,
+    raise_if_nodecode,
+)
 
 
 def _buffer_to_json(obj: Buffer) -> dict:
     """Serializes a bokeh object.into a JSON document."""
     return {
         "__type__": "buffer",
         "__version__": 1,
@@ -72,22 +82,25 @@
 
 def from_json(dct: dict) -> Any:
     """
     Deserializes a dict Serializes a bokeh object. See `to_json` for the
     specification `dct` is expected to follow. In particular, note that `dct`
     must contain the key `__bokeh__`.
     """
+    raise_if_nodecode("bokeh")
     DECODERS = {
         "buffer": _json_to_buffer,
         "generic": _json_to_generic,
     }
     try:
-        return DECODERS[dct["__bokeh__"]["__type__"]](dct["__bokeh__"])
+        type_name = dct["__bokeh__"]["__type__"]
+        raise_if_nodecode("bokeh." + type_name)
+        return DECODERS[type_name](dct["__bokeh__"])
     except KeyError as exc:
-        raise TypeError("Not a valid figure document") from exc
+        raise DeserializationError() from exc
 
 
 def to_json(obj: Any) -> dict:
     """
     Serializes a bokeh object.
 
     The return dict has the following structure
@@ -95,26 +108,26 @@
         {
             "__bokeh__": {...},
         }
 
     where the `{...}` dict contains the actual data, and whose structure
     depends on the precise type of `obj`.
 
-    * `bokeh.plotting._figure.figure` or `bokeh.models.Model`:
+    - `bokeh.plotting._figure.figure` or `bokeh.models.Model`:
 
         {
             "__bokeh__": {
                 "__type__": "generic",
                 "__version__": 1,
                 "content": {...},
                 "buffers": [...],
             }
         }
 
-    * `bokeh.core.serialization.Buffer`: (for internal use)
+    - `bokeh.core.serialization.Buffer`: (for internal use)
 
         {
             "__bokeh__": {
                 "__type__": "buffer",
                 "__version__": 1,
                 "id": <str>,
                 "data": <bytes>,
@@ -126,8 +139,8 @@
         (Buffer, _buffer_to_json),
         (Figure, _generic_to_json),
         (Model, _generic_to_json),
     ]
     for t, f in ENCODERS:
         if isinstance(obj, t):
             return {"__bokeh__": f(obj)}
-    raise TypeError("Not a supported figure type")
+    raise TypeNotSupported()
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/bytes.py` & `turbo_broccoli-2.3.8/turbo_broccoli/bytes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """bytes (de)serialization utilities."""
 __docformat__ = "google"
 
-from typing import Any, Optional
-
 from base64 import b64decode, b64encode
+from typing import Any, Optional
 
-from turbo_broccoli.environment import is_nodecode
+from turbo_broccoli.utils import (
+    DeserializationError,
+    TypeNotSupported,
+    raise_if_nodecode,
+)
 
 
 def _bytes_from_json_v1(dct: dict) -> bytes:
     """
     Deserializes a dict into a bytes object following the v1 specification.
     """
     return b64decode(dct["data"])
@@ -17,23 +20,22 @@
 
 def from_json(dct: dict) -> Optional[bytes]:
     """
     Deserializes a dict into a bytes object. See `to_json` for the
     specification `dct` is expected to follow. In particular, note that `dct`
     must contain the key `__bytes__`.
     """
-    if is_nodecode("bytes"):
-        return None
+    raise_if_nodecode("bytes")
     DECODERS = {
         1: _bytes_from_json_v1,
     }
     try:
         return DECODERS[dct["__bytes__"]["__version__"]](dct["__bytes__"])
     except KeyError as exc:
-        raise TypeError("Not a valid bytes document") from exc
+        raise DeserializationError() from exc
 
 
 def to_json(obj: Any) -> dict:
     """
     Serializes a Python `bytes` object into JSON using a base 64 + ASCII scheme.
 
     The return dict has the following structure
@@ -49,8 +51,8 @@
     if isinstance(obj, bytes):
         return {
             "__bytes__": {
                 "__version__": 1,
                 "data": b64encode(obj).decode("ascii"),
             },
         }
-    raise TypeError("Not a valid bytes object")
+    raise TypeNotSupported()
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/collections.py` & `turbo_broccoli-2.3.8/turbo_broccoli/collections.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """Python standard collections (de)serialization"""
 __docformat__ = "google"
 
 from collections import deque, namedtuple
 from typing import Any, Callable, List, Optional, Tuple
 
-from turbo_broccoli.environment import is_nodecode
+from turbo_broccoli.utils import (
+    DeserializationError,
+    TypeNotSupported,
+    raise_if_nodecode,
+)
 
 
 def _deque_to_json(deq: deque) -> dict:
     """Converts a deque into a JSON document."""
     return {
         "__type__": "deque",
         "__version__": 1,
@@ -57,15 +61,19 @@
     `tup` argument is truly a namedtuple by checking that it has the following
     attributes: `_asdict`, `_field_defaults`, `_fields`, `_make`, `_replace`.
     See
     https://docs.python.org/3/library/collections.html#collections.namedtuple .
     """
     attributes = ["_asdict", "_field_defaults", "_fields", "_make", "_replace"]
     if not all(map(lambda a: hasattr(tup, a), attributes)):
-        raise TypeError("Not a namedtuple")
+        raise TypeNotSupported(
+            "This object does not have all the attributes expected from a "
+            "namedtuple. The expected attributes are `_asdict`, "
+            "`_field_defaults`, `_fields`, `_make`, and `_replace`."
+        )
     return {
         "__type__": "namedtuple",
         "__version__": 1,
         "class": tup.__class__.__name__,
         "data": tup._asdict(),  # type: ignore
     }
 
@@ -78,19 +86,18 @@
     """
     DECODERS = {
         "deque": _json_to_deque,
         "namedtuple": _json_to_namedtuple,
     }
     try:
         type_name = dct["__collections__"]["__type__"]
-        if is_nodecode("collections." + type_name):
-            return None
+        raise_if_nodecode("collections." + type_name)
         return DECODERS[type_name](dct["__collections__"])
     except KeyError as exc:
-        raise TypeError("Not a valid collections document") from exc
+        raise DeserializationError() from exc
 
 
 def to_json(obj: Any) -> dict:
     """
     Serializes a Python collection into JSON by cases. See the README for the
     precise list of supported types.
 
@@ -99,38 +106,38 @@
         {
             "__collections__": {...},
         }
 
     where the `{...}` dict contains the actual data, and whose structure
     depends on the precise type of `obj`.
 
-    * `collections.deque`:
+    - `collections.deque`:
 
-        {
-            "__collections__": {
-                "__type__": "deque,
-                "__version__": 1,
-                "data": [...],
-                "maxlen": <int or None>,
+            {
+                "__collections__": {
+                    "__type__": "deque,
+                    "__version__": 1,
+                    "data": [...],
+                    "maxlen": <int or None>,
+                }
             }
-        }
 
-    * `collections.namedtuple`
+    - `collections.namedtuple`
 
-        {
-            "__collections__": {
-                "__type__": "namedtuple,
-                "__version__": 1,
-                "class": <str>,
-                "data": {...},
+            {
+                "__collections__": {
+                    "__type__": "namedtuple,
+                    "__version__": 1,
+                    "class": <str>,
+                    "data": {...},
+                }
             }
-        }
 
     """
     ENCODERS: List[Tuple[type, Callable[[Any], dict]]] = [
         (deque, _deque_to_json),
         (tuple, _namedtuple_to_json),
     ]
     for t, f in ENCODERS:
         if isinstance(obj, t):
             return {"__collections__": f(obj)}
-    raise TypeError("Not a supported collections type")
+    raise TypeNotSupported()
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/dataclass.py` & `turbo_broccoli-2.3.8/turbo_broccoli/dataclass.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 """Dataclass serialization"""
 __docformat__ = "google"
 
 from typing import Any
 
 from turbo_broccoli.environment import (
     get_registered_dataclass_type,
-    is_nodecode,
+)
+from turbo_broccoli.utils import (
+    DeserializationError,
+    TypeNotSupported,
+    raise_if_nodecode,
 )
 
 
 def _json_to_dataclass_v2(dct: dict) -> Any:
     """
     Converts a JSON document following the v2 specification to a dataclass
     object.
     """
-    if is_nodecode("dataclass." + dct["class"]):
-        return None
     return get_registered_dataclass_type(dct["class"])(**dct["data"])
 
 
 def from_json(dct: dict) -> Any:
     """
     Deserializes a dict into a dataclass object. See `to_json` for the
     specification `dct` is expected to follow, and
     `turbo_broccoli.environment.register_dataclass_type`.
     """
+    raise_if_nodecode("dataclass")
     DECODERS = {
         2: _json_to_dataclass_v2,
     }
     try:
+        raise_if_nodecode("dataclass." + dct["__dataclass__"]["class"])
         return DECODERS[dct["__dataclass__"]["__version__"]](
             dct["__dataclass__"]
         )
     except KeyError as exc:
-        raise TypeError("Not a valid dataclass document") from exc
+        raise DeserializationError() from exc
 
 
 def to_json(obj: Any) -> dict:
     """
     Serializes a dataclass into JSON by cases. The return dict has the
     following structure
 
@@ -55,8 +59,8 @@
         return {
             "__dataclass__": {
                 "__version__": 2,
                 "class": obj.__class__.__name__,
                 "data": obj.__dict__,
             },
         }
-    raise TypeError("Not a supported type")
+    raise TypeNotSupported()
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/environment.py` & `turbo_broccoli-2.3.8/turbo_broccoli/environment.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/generic.py` & `turbo_broccoli-2.3.8/turbo_broccoli/generic.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,35 @@
 `turbo_broccoli.generic.to_json`.
 """
 __docformat__ = "google"
 
 
 from typing import Any, Iterable
 
+from turbo_broccoli.utils import TypeNotSupported, raise_if_nodecode
+
 
 def to_json(obj: Any) -> dict:
-    """Serializes a generic object into JSON by cases."""
+    """
+    Serializes a generic object into JSON by cases. The return dict has the
+    following structure:
+
+        {
+            "__generic__": {
+                "__version__": 1,
+                "data": {...},
+            },
+        }
+
+    """
     if not (
         hasattr(obj, "__turbo_broccoli__")
         and isinstance(obj.__turbo_broccoli__, Iterable)
     ):
-        raise TypeError("Not a generic object")
+        raise TypeNotSupported()
+    raise_if_nodecode("generic")
     return {
         "__generic__": {
             "__version__": 1,
             "data": {k: getattr(obj, k) for k in obj.__turbo_broccoli__},
         },
     }
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/keras.py` & `turbo_broccoli-2.3.8/turbo_broccoli/keras.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 __docformat__ = "google"
 
 from functools import partial
 from typing import Any, Callable, List, Tuple
 from uuid import uuid4
 
 from tensorflow import keras
+
 from turbo_broccoli.environment import (
     get_artifact_path,
     get_keras_format,
-    is_nodecode,
+)
+from turbo_broccoli.utils import (
+    DeserializationError,
+    TypeNotSupported,
+    raise_if_nodecode,
 )
 
 KERAS_LAYERS = {
     "Activation": keras.layers.Activation,
     "ActivityRegularization": keras.layers.ActivityRegularization,
     "Add": keras.layers.Add,
     "AdditiveAttention": keras.layers.AdditiveAttention,
@@ -305,28 +310,28 @@
 
 def from_json(dct: dict) -> Any:
     """
     Deserializes a dict into a Keras object. See `to_json` for the
     specification `dct` is expected to follow. In particular, note that `dct`
     must contain the key `__keras__`.
     """
+    raise_if_nodecode("keras")
     DECODERS = {
         "model": _json_to_model,  # must be first!
         "layer": _json_to_layer,
         "loss": _json_to_loss,
         "metric": _json_to_metric,
         "optimizer": _json_to_optimizer,
     }
     try:
         type_name = dct["__keras__"]["__type__"]
-        if is_nodecode("keras." + type_name):
-            return None
+        raise_if_nodecode("keras." + type_name)
         return DECODERS[type_name](dct["__keras__"])
     except KeyError as exc:
-        raise TypeError("Not a valid Keras document") from exc
+        raise DeserializationError() from exc
 
 
 def to_json(obj: Any) -> dict:
     """
     Serializes a tensorflow object into JSON by cases. See the README for the
     precise list of supported types.
 
@@ -336,15 +341,15 @@
             "__keras__": {...},
         }
 
     where the `{...}` dict contains the actual data, and whose structure
     depends on the precise type of `obj`. Most keras object will simply be
     serialized using `keras.utils.serialize_keras_object`. Here are the exceptions:
 
-    * `keras.Model` (the model must have weights). If `TB_KERAS_FORMAT` is
+    - `keras.Model` (the model must have weights). If `TB_KERAS_FORMAT` is
       `json`, the document will look like
 
             {
                 "__keras__": {
                     "__type__": "model",
                     "__version__": 2,
                     "loss": {...} or null,
@@ -379,8 +384,8 @@
             keras.optimizers.Optimizer,
             partial(_generic_keras_to_json, type_="optimizer"),
         ),
     ]
     for t, f in ENCODERS:
         if isinstance(obj, t):
             return {"__keras__": f(obj)}
-    raise TypeError("Not a supported Keras type")
+    raise TypeNotSupported()
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/numpy.py` & `turbo_broccoli-2.3.8/turbo_broccoli/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,19 @@
 
     warn_about_safetensors()
 
 
 from turbo_broccoli.environment import (
     get_artifact_path,
     get_max_nbytes,
-    is_nodecode,
+)
+from turbo_broccoli.utils import (
+    DeserializationError,
+    TypeNotSupported,
+    raise_if_nodecode,
 )
 
 
 def _json_to_dtype(dct: dict) -> np.dtype:
     """
     Converts a JSON document to a numpy dtype. See `to_json` for the
     specification `dct` is expected to follow. Note that the key `__numpy__`
@@ -200,26 +204,26 @@
 
 def from_json(dct: dict) -> Any:
     """
     Deserializes a dict into a numpy object. See `to_json` for the
     specification `dct` is expected to follow. In particular, note that `dct`
     must contain the key `__numpy__`.
     """
+    raise_if_nodecode("numpy")
     DECODERS = {
         "ndarray": _json_to_ndarray,
         "number": _json_to_number,
         "dtype": _json_to_dtype,
     }
     try:
         type_name = dct["__numpy__"]["__type__"]
-        if is_nodecode("numpy." + type_name):
-            return None
+        raise_if_nodecode("numpy." + type_name)
         return DECODERS[type_name](dct["__numpy__"])
     except KeyError as exc:
-        raise TypeError("Not a valid numpy document") from exc
+        raise DeserializationError() from exc
 
 
 def to_json(obj: Any) -> dict:
     """
     Serializes a `numpy` object into JSON by cases. See the README for the
     precise list of supported types.
 
@@ -228,15 +232,15 @@
         {
             "__numpy__": {...},
         }
 
     where the `{...}` dict contains the actual data, and whose structure
     depends on the precise type of `obj`.
 
-    * `numpy.ndarray`: An array is processed differently depending on its size
+    - `numpy.ndarray`: An array is processed differently depending on its size
       and on the `TB_MAX_NBYTES` environment variable. If the array is
       small, i.e. `arr.nbytes <= TB_MAX_NBYTES`, then it is directly
       stored in the resulting JSON document as
 
             {
                 "__numpy__": {
                     "__type__": "ndarray",
@@ -273,28 +277,28 @@
                 }
             }
 
       By default, `TB_MAX_NBYTES` is `8000` bytes, which should be enough
       to store an array of 1000 `float64`s, and `TB_ARTIFACT_PATH` is `./`.
       `TB_ARTIFACT_PATH` must point to an existing directory.
 
-    * `numpy.number`:
+    - `numpy.number`:
 
             {
                 "__numpy__": {
                     "__type__": "number",
                     "__version__": 2,
                     "value": <float>,
                     "dtype": {...},
                 }
             }
 
         where the `dtype` document follows the specification below.
 
-    * `numpy.dtype`:
+    - `numpy.dtype`:
 
             {
                 "__numpy__": {
                     "__type__": "dtype",
                     "__version__": 1,
                     "dtype": <dtype_to_descr string>,
                 }
@@ -305,8 +309,8 @@
         (np.ndarray, _ndarray_to_json),
         (np.number, _number_to_json),
         (np.dtype, _dtype_to_json),
     ]
     for t, f in ENCODERS:
         if isinstance(obj, t):
             return {"__numpy__": f(obj)}
-    raise TypeError("Not a supported numpy type")
+    raise TypeNotSupported()
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/pandas.py` & `turbo_broccoli-2.3.8/turbo_broccoli/pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,24 @@
 __docformat__ = "google"
 
 import json
 from typing import Any, Callable, List, Tuple
 from uuid import uuid4
 
 import pandas as pd
+
 from turbo_broccoli.environment import (
     get_artifact_path,
     get_max_nbytes,
     get_pandas_format,
-    is_nodecode,
+)
+from turbo_broccoli.utils import (
+    DeserializationError,
+    TypeNotSupported,
+    raise_if_nodecode,
 )
 
 
 def _dataframe_to_json(df: pd.DataFrame) -> dict:
     """Converts a pandas dataframe into a JSON document."""
     # Sometimes column names are int, so cannot be used as keys in a JSON
     # document. Eventhough int column names are not supported, this is
@@ -115,25 +120,25 @@
 
 def from_json(dct: dict) -> Any:
     """
     Deserializes a dict into a pandas object. See `to_json` for the
     specification `dct` is expected to follow. In particular, note that `dct`
     must contain the key `__pandas__`.
     """
+    raise_if_nodecode("pandas")
     DECODERS = {
         "dataframe": _json_to_dataframe,
         "series": _json_to_series,
     }
     try:
         type_name = dct["__pandas__"]["__type__"]
-        if is_nodecode("pandas." + type_name):
-            return None
+        raise_if_nodecode("pandas." + type_name)
         return DECODERS[type_name](dct["__pandas__"])
     except KeyError as exc:
-        raise TypeError("Not a valid pandas document") from exc
+        raise DeserializationError() from exc
 
 
 def to_json(obj: Any) -> dict:
     """
     Serializes a pandas object into JSON by cases. See the README for the
     precise list of supported types.
 
@@ -142,15 +147,15 @@
         {
             "__pandas__": {...},
         }
 
     where the `{...}` dict contains the actual data, and whose structure
     depends on the precise type of `obj`.
 
-    * `pandas.DataFrame`: A dataframe is processed differently depending on its
+    - `pandas.DataFrame`: A dataframe is processed differently depending on its
       size and on the `TB_MAX_NBYTES` environment variable. If the dataframe is
       small, i.e. at most `TB_MAX_NBYTES` bytes, then it is directly stored in
       the resulting JSON document as
 
             {
                 "__pandas__": {
                     "__type__": "dataframe",
@@ -181,15 +186,15 @@
                         ...
                     ],
                     "id": <UUID4 str>,
                     "format": <str>
                 }
             }
 
-    * `pandas.Series`: A series will be converted to a dataframe before being
+    - `pandas.Series`: A series will be converted to a dataframe before being
       serialized. The final document will look like this
 
             {
                 "__pandas__": {
                     "__type__": "series",
                     "__version__": 1,
                     "data": {...},
@@ -222,8 +227,8 @@
     ENCODERS: List[Tuple[type, Callable[[Any], dict]]] = [
         (pd.DataFrame, _dataframe_to_json),
         (pd.Series, _series_to_json),
     ]
     for t, f in ENCODERS:
         if isinstance(obj, t):
             return {"__pandas__": f(obj)}
-    raise TypeError("Not a supported pandas type")
+    raise TypeNotSupported()
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/pytorch.py` & `turbo_broccoli-2.3.8/turbo_broccoli/pytorch.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 import torch
 
 from turbo_broccoli.environment import (
     get_artifact_path,
     get_max_nbytes,
     get_registered_pytorch_module_type,
 )
+from turbo_broccoli.utils import (
+    DeserializationError,
+    TypeNotSupported,
+    raise_if_nodecode,
+)
 
 
 def _json_to_module(dct: dict) -> torch.nn.Module:
     """
     Converts a JSON document to a `pytorch` module. See `to_json` for the
     specification `dct` is expected to follow. Note that the key `__pytorch__`
     should not be present.
@@ -97,22 +102,25 @@
 
 def from_json(dct: dict) -> Any:
     """
     Deserializes a dict into a `pytorch` object. See `to_json` for the
     specification `dct` is expected to follow. In particular, note that `dct`
     must contain the key `__pytorch__`.
     """
+    raise_if_nodecode("pytorch")
     DECODERS = {
         "tensor": _json_to_tensor,
         "module": _json_to_module,
     }
     try:
-        return DECODERS[dct["__pytorch__"]["__type__"]](dct["__pytorch__"])
+        type_name = dct["__pytorch__"]["__type__"]
+        raise_if_nodecode("pytorch." + type_name)
+        return DECODERS[type_name](dct["__pytorch__"])
     except KeyError as exc:
-        raise TypeError("Not a valid pytorch document") from exc
+        raise DeserializationError() from exc
 
 
 def to_json(obj: Any) -> dict:
     """
     Serializes a tensor into JSON by cases. See the README for the precise list
     of supported types.
 
@@ -120,16 +128,49 @@
 
         {
             "__pytorch__": {...},
         }
 
     where the `{...}` dict contains the actual data, and whose structure
     depends on the precise type of `obj`.
+
+    - Tensor:
+
+            {
+                "__pytorch__": {
+                    "__type__": "tensor",
+                    "__version__": 1,
+                    "data": <bytes>,
+                }
+            }
+
+      or if the underlying data is too large resulting in an artifact being
+      created:
+
+            {
+                "__pytorch__": {
+                    "__type__": "tensor",
+                    "__version__": 1,
+                    "id": <UUID4 str>,
+                }
+            }
+
+    - Module:
+
+            {
+                "__pytorch__": {
+                    "__type__": "module",
+                    "__version__": 1,
+                    "class": <class name>,
+                    "state": {...},
+                }
+            }
+
     """
     ENCODERS: List[Tuple[type, Callable[[Any], dict]]] = [
         (torch.nn.Module, _module_to_json),
         (torch.Tensor, _tensor_to_json),
     ]
     for t, f in ENCODERS:
         if isinstance(obj, t):
             return {"__pytorch__": f(obj)}
-    raise TypeError("Not a supported tensor type")
+    raise TypeNotSupported()
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/scipy.py` & `turbo_broccoli-2.3.8/turbo_broccoli/dict.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,63 @@
-"""scipy objects"""
+"""Serialization of dicts with non string keys"""
 __docformat__ = "google"
 
-from typing import Any, Callable, List, Tuple
+from typing import Any
 
-from scipy.sparse import csr_matrix
+from turbo_broccoli.utils import (
+    DeserializationError,
+    TypeNotSupported,
+    raise_if_nodecode,
+)
 
 
-def _csr_matrix_to_json(m: csr_matrix) -> dict:
-    """Converts a csr_matrix into a JSON document."""
-    return {
-        "__type__": "csr_matrix",
-        "__version__": 1,
-        "data": m.data,
-        "dtype": m.dtype,
-        "indices": m.indices,
-        "indptr": m.indptr,
-        "shape": m.shape,
-    }
-
-
-def _json_to_csr_matrix(dct: dict) -> csr_matrix:
+def _json_to_dict_v1(dct: dict) -> dict:
     """
-    Converts a JSON document to a csr_matrix. See `to_json` for the
-    specification `dct` is expected to follow. Note that the key `__scipy__`
-    should not be present.
+    Converts a JSON document representing a dict with non-string keys to a dict
+    following the v1 specification. In particular, note that `dct` must not
+    contain the key `__dict__`.
     """
-    DECODERS = {
-        1: _json_to_csr_matrix_v1,
-    }
-    return DECODERS[dct["__version__"]](dct)
-
-
-def _json_to_csr_matrix_v1(dct: dict) -> csr_matrix:
-    """
-    Converts a JSON document to a csr_matrix following the v1 specification.
-    """
-    return csr_matrix(
-        (dct["data"], dct["indices"], dct["indptr"]),
-        shape=dct["shape"],
-        dtype=dct["dtype"],
-    )
+    return {item["key"]: item["val"] for item in dct["items"]}
 
 
 def from_json(dct: dict) -> Any:
     """
-    Deserializes a dict into a csr_matrix. See `to_json` for the specification
-    `dct` is expected to follow. In particular, note that `dct` must contain
-    the key `__csr_matrix__`.
+    Deserializes a dict into a non-string key dict. See `to_json` for the
+    specification `dct` is expected to follow. In particular, note that `dct`
+    must contain the key `__dict__`.
     """
+    raise_if_nodecode("dict")
     DECODERS = {
-        "csr_matrix": _json_to_csr_matrix,
+        1: _json_to_dict_v1,
     }
     try:
-        return DECODERS[dct["__scipy__"]["__type__"]](dct["__scipy__"])
+        return DECODERS[dct["__dict__"]["__version__"]](dct["__dict__"])
     except KeyError as exc:
-        raise TypeError("Not a valid scipy document") from exc
+        raise DeserializationError() from exc
 
 
 def to_json(obj: Any) -> dict:
     """
-    Serializes a Scipy object into JSON by cases. See the README for the
-    precise list of supported types.
-
-    The return dict has the following structure
+    Serializes a dict with non-string keys into JSON. The return dict has the
+    following structure
 
         {
-            "__scipy__": {...},
+            "__dict__": {
+                "__version__": 1,
+                "items": [
+                    {"key": {...}, "val": {...}},
+                    ...
+                ]
+            },
         }
 
-    where the `{...}` dict contains the actual data, and whose structure
-    depends on the precise type of `obj`.
     """
-    ENCODERS: List[Tuple[type, Callable[[Any], dict]]] = [
-        (csr_matrix, _csr_matrix_to_json),
-    ]
-    for t, f in ENCODERS:
-        if isinstance(obj, t):
-            return {"__scipy__": f(obj)}
-    raise TypeError("Not a supported scipy type")
+    if not isinstance(obj, dict):
+        raise TypeNotSupported()
+    if all(map(lambda x: isinstance(x, str), obj.keys())):
+        raise TypeNotSupported("All keys are strings")
+    return {
+        "__dict__": {
+            "__version__": 1,
+            "items": [{"key": key, "val": val} for key, val in obj.items()],
+        },
+    }
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/secret.py` & `turbo_broccoli-2.3.8/turbo_broccoli/secret.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import json
 from typing import Any, NoReturn
 
 from nacl.secret import SecretBox
 
 from turbo_broccoli.environment import get_shared_key
+from turbo_broccoli.utils import TypeNotSupported, raise_if_nodecode
 
 
 class Secret:
     """
     A wrapper for a basic Python variable whose value is considered to be
     secret. Similar API as [`pydantic`'s secret
     types](https://pydantic-docs.helpmanual.io/usage/types/#secret-types)
@@ -90,14 +91,15 @@
 
 def from_json(dct: dict) -> Any:
     """
     Deserializes a dict into a secret Python type. See `to_json` for the
     specification `dct` is expected to follow. In particular, note that `dct`
     must contain the key `__secret__`.
     """
+    raise_if_nodecode("secret")
     DECODERS = {
         1: _from_json_v1,
     }
     obj = DECODERS[dct["__secret__"]["__version__"]](dct["__secret__"])
     if isinstance(obj, LockedSecret):
         return obj
     TYPES = {
@@ -108,26 +110,27 @@
         str: SecretStr,
     }
     return TYPES[type(obj)](obj)
 
 
 def to_json(obj: Secret) -> dict:
     """
-    Encrypts a JSON **string representation** of a secret document into a new
-    JSON document with the following structure:
+    Encrypts a JSON **string representation** of a secret document into a
+    new JSON document with the following structure:
 
-        {
-            "__secret__": {
-                "__version__": 1,
-                "data": <encrypted bytes>,
+            {
+                "__secret__": {
+                    "__version__": 1,
+                    "data": <encrypted bytes>,
+                }
             }
-        }
+
     """
     if not isinstance(obj, Secret):
-        raise TypeError("Not a valid secret type")
+        raise TypeNotSupported()
     key = get_shared_key()
     if key is None:
         raise RuntimeError(
             "Attempting to serialize a secret type but no shared key is set. "
             "Use either turbo_broccoli.environment.set_shared_key or the "
             "TB_SHARED_KEY environment variable."
         )
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/sklearn.py` & `turbo_broccoli-2.3.8/turbo_broccoli/sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,20 @@
     semi_supervised,
     svm,
     tree,
 )
 from sklearn.base import BaseEstimator
 from sklearn.tree._tree import Tree
 
+from turbo_broccoli.utils import (
+    DeserializationError,
+    TypeNotSupported,
+    raise_if_nodecode,
+)
+
 _SKLEARN_SUBMODULES = [
     # calibration,
     cluster,
     covariance,
     cross_decomposition,
     datasets,
     decomposition,
@@ -194,37 +200,40 @@
 
 
 def _json_to_sklearn_tree_v1(dct: dict) -> BaseEstimator:
     """
     Converts a JSON document to a sklearn tree following the v1 specification.
 
     See also:
-        * https://github.com/scikit-learn/scikit-learn/blob/9aaed498795f68e5956ea762fef9c440ca9eb239/sklearn/tree/_tree.pxd
-        * https://github.com/scikit-learn/scikit-learn/blob/9aaed498795f68e5956ea762fef9c440ca9eb239/sklearn/tree/_classes.py#L349
+        - https://github.com/scikit-learn/scikit-learn/blob/9aaed498795f68e5956ea762fef9c440ca9eb239/sklearn/tree/_tree.pxd
+        - https://github.com/scikit-learn/scikit-learn/blob/9aaed498795f68e5956ea762fef9c440ca9eb239/sklearn/tree/_classes.py#L349
     """
     obj = Tree(dct["n_features"], dct["n_classes"], dct["n_outputs"])
     for k in _SKLEARN_TREE_ATTRIBUTES:
         setattr(obj, k, dct[k])
     return obj
 
 
 def from_json(dct: dict) -> BaseEstimator:
     """
     Deserializes a dict into a sklearn estimator. See `to_json` for the
     specification `dct` is expected to follow. In particular, note that `dct`
     must contain the key `__sklearn__`.
     """
+    raise_if_nodecode("sklearn")
     DECODERS = {
         "estimator": _json_to_sklearn_estimator,
         "tree": _json_to_sklearn_tree,
     }
     try:
-        return DECODERS[dct["__sklearn__"]["__type__"]](dct["__sklearn__"])
+        type_name = dct["__sklearn__"]["__type__"]
+        raise_if_nodecode("sklearn." + type_name)
+        return DECODERS[type_name](dct["__sklearn__"])
     except KeyError as exc:
-        raise TypeError("Not a valid sklearn document") from exc
+        raise DeserializationError() from exc
 
 
 def to_json(obj: BaseEstimator) -> dict:
     """
     Serializes a sklearn estimator into JSON by cases. See the README for the
     precise list of supported types.
 
@@ -246,8 +255,8 @@
     ENCODERS: List[Tuple[type, Callable[[Any], dict]]] = [
         (BaseEstimator, _sklearn_estimator_to_json),
         (Tree, _sklearn_tree_to_json),
     ]
     for t, f in ENCODERS:
         if isinstance(obj, t):
             return {"__sklearn__": f(obj)}
-    raise TypeError("Not a supported sklearn type")
+    raise TypeNotSupported()
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/tensorflow.py` & `turbo_broccoli-2.3.8/turbo_broccoli/tensorflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,19 @@
     from turbo_broccoli.utils import warn_about_safetensors
 
     warn_about_safetensors()
 
 from turbo_broccoli.environment import (
     get_artifact_path,
     get_max_nbytes,
-    is_nodecode,
+)
+from turbo_broccoli.utils import (
+    DeserializationError,
+    TypeNotSupported,
+    raise_if_nodecode,
 )
 
 
 def _json_to_sparse_tensor(dct: dict) -> tf.Tensor:
     """Converts a JSON document to a tensorflow tensor."""
     DECODERS = {
         1: _json_to_sparse_tensor_v1,
@@ -183,102 +187,110 @@
 
 def from_json(dct: dict) -> Any:
     """
     Deserializes a dict into a tensorflow object. See `to_json` for the
     specification `dct` is expected to follow. In particular, note that `dct`
     must contain the key `__tensorflow__`.
     """
+    raise_if_nodecode("tensorflow")
     DECODERS = {
         "sparse_tensor": _json_to_sparse_tensor,
         "tensor": _json_to_tensor,
         "variable": _json_to_variable,
     }
     try:
         type_name = dct["__tensorflow__"]["__type__"]
-        if is_nodecode("tensorflow." + type_name):
-            return None
+        raise_if_nodecode("tensorflow." + type_name)
         return DECODERS[type_name](dct["__tensorflow__"])
     except KeyError as exc:
-        raise TypeError("Not a valid tensorflow document") from exc
+        raise DeserializationError() from exc
 
 
 def to_json(obj: Any) -> dict:
     """
     Serializes a tensorflow object into JSON by cases. See the README for the
     precise list of supported types.
 
     The return dict has the following structure
 
         {
-            "__tensorflow__": {...},
+            "__tensorflow__": {...}
         }
 
     where the `{...}` dict contains the actual data, and whose structure
     depends on the precise type of `obj`.
 
-    * `tf.RaggedTensor`: Not supported.
+    - `tf.RaggedTensor`: Not supported.
 
-    * `tf.SparseTensor`:
+    - `tf.SparseTensor`:
 
             {
-                "__type__": "sparse_tensor",
-                "__version__": 1,
-                "indices": {...},
-                "values": {...},
-                "shape": {...},
+                "__tensorflow__": {
+                    "__type__": "sparse_tensor",
+                    "__version__": 1,
+                    "indices": {...},
+                    "values": {...},
+                    "shape": {...},
+                }
             }
 
       where the first two `{...}` placeholders result in the serialization of
       `tf.Tensor` (see below).
 
-    * other `tf.Tensor` subtypes:
+    - other `tf.Tensor` subtypes:
 
             {
-                "__type__": "tensor",
-                "__version__": 1,
-                "dtype": <str>,
-                "numpy": {...},
+                "__tensorflow__": {
+                    "__type__": "tensor",
+                    "__version__": 1,
+                    "dtype": <str>,
+                    "numpy": {...},
+                }
             }
 
       or, if the `safetensors` package is available:
 
             {
-                "__type__": "tensor",
-                "__version__": 2,
-                "dtype": <str>,
-                "data": {...},
+                "__tensorflow__": {
+                    "__type__": "tensor",
+                    "__version__": 2,
+                    "dtype": <str>,
+                    "data": {...},
+                }
             }
 
       On the other hand, if the `safetensors` package is available, and if the
       tensor is too large (i.e. the number of bytes exceeds `TB_MAX_NBYTES` or
       the value set by `turbo_broccoli.environment.set_max_nbytes`), then the
       content of the tensor is stored in a binary artefact´. Said file is saved
       to the path specified by the `TB_ARTIFACT_PATH` environment variable with
       a random UUID4 as filename. The resulting JSON document looks like
 
             {
-                "__numpy__": {
+                "__tensorflow__": {
                     "__type__": "tensor",
                     "__version__": 2,
                     "id": <UUID4 str>,
                 }
             }
 
       By default, `TB_MAX_NBYTES` is `8000` bytes, which should be enough
       to store an array of 1000 `float64`s, and `TB_ARTIFACT_PATH` is `./`.
       `TB_ARTIFACT_PATH` must point to an existing directory.
 
-    * `tf.Variable`:
+    - `tf.Variable`:
 
             {
-                "__type__": "tensor",
-                "__version__": 2,
-                "name": <str>,
-                "value": {...},
-                "trainable": <bool>,
+                "__tensorflow__": {
+                    "__type__": "tensor",
+                    "__version__": 2,
+                    "name": <str>,
+                    "value": {...},
+                    "trainable": <bool>,
+                }
             }
 
       where `{...}` is the document produced by serializing the value tensor of
       the variable.
 
     """
     ENCODERS: List[Tuple[type, Callable[[Any], dict]]] = [
@@ -286,8 +298,8 @@
         (tf.SparseTensor, _sparse_tensor_to_json),
         (tf.Tensor, _tensor_to_json),
         (tf.Variable, _variable_to_json),
     ]
     for t, f in ENCODERS:
         if isinstance(obj, t):
             return {"__tensorflow__": f(obj)}
-    raise TypeError("Not a supported tensorflow type")
+    raise TypeNotSupported()
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli/turbo_broccoli.py` & `turbo_broccoli-2.3.8/turbo_broccoli/turbo_broccoli.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from typing import Any, Callable, Dict, List, Union
 
 
 import turbo_broccoli.bytes
 import turbo_broccoli.collections
 import turbo_broccoli.dataclass
 import turbo_broccoli.generic
+import turbo_broccoli.dict
+from turbo_broccoli.utils import TypeIsNodecode, TypeNotSupported
 
 try:
     import turbo_broccoli.keras
 
     HAS_KERAS = True
 except ModuleNotFoundError:
     HAS_KERAS = False
@@ -86,14 +88,15 @@
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(object_hook=self._hook, *args, **kwargs)
 
     def _hook(self, dct):
         """Deserialization hook"""
         DECODERS: Dict[str, Callable[[dict], Any]] = {
+            "__dict__": turbo_broccoli.dict.from_json,
             "__bytes__": turbo_broccoli.bytes.from_json,
         }
         if HAS_KERAS:
             DECODERS["__keras__"] = turbo_broccoli.keras.from_json
         if HAS_NUMPY:
             DECODERS["__numpy__"] = turbo_broccoli.numpy.from_json
         if HAS_PANDAS:
@@ -111,15 +114,18 @@
         if HAS_BOKEH:
             DECODERS["__bokeh__"] = turbo_broccoli.bokeh.from_json
         # Intentionally put last
         DECODERS["__collections__"] = turbo_broccoli.collections.from_json
         DECODERS["__dataclass__"] = turbo_broccoli.dataclass.from_json
         for t, f in DECODERS.items():
             if t in dct:
-                return f(dct)
+                try:
+                    return f(dct)
+                except TypeIsNodecode:
+                    return None
         return dct
 
 
 class TurboBroccoliEncoder(json.JSONEncoder):
     """
     TurboBroccoli's custom JSON decoder class. See the README for the list of
     supported types.
@@ -153,30 +159,32 @@
             turbo_broccoli.collections.to_json,
             turbo_broccoli.dataclass.to_json,
             turbo_broccoli.generic.to_json,
         ]
         for f in ENCODERS:
             try:
                 return f(o)
-            except TypeError:
+            except TypeNotSupported:
                 pass
         return super().default(o)
 
     def encode(self, o: Any) -> str:
         """
-        Reimplementation of encode just to treat the `namedtuple` case. An
-        object is considered a namedtuple if it is an instance of `tuple` and
-        has the following attributes: `_asdict`, `_field_defaults`, `_fields`,
-        `_make`, `_replace`. In this case,
-        `turbo_broccoli.collections._namedtuple_to_json` is called directly.
+        Reimplementation of encode just to treat exceptional cases that need to
+        be handled before `JSONEncoder.encode`.
         """
-        attrs = ["_asdict", "_field_defaults", "_fields", "_make", "_replace"]
-        if isinstance(o, tuple) and all(map(lambda a: hasattr(o, a), attrs)):
-            d = turbo_broccoli.collections._namedtuple_to_json(o)
-            return super().encode({"__collections__": d})
+        PRIORITY_ENCODERS: List[Callable[[Any], dict]] = [
+            turbo_broccoli.dict.to_json,
+            turbo_broccoli.collections.to_json,
+        ]
+        for f in PRIORITY_ENCODERS:
+            try:
+                return super().encode(f(o))
+            except TypeNotSupported:
+                pass
         return super().encode(o)
 
 
 def from_json(doc: str) -> Any:
     """Converts a JSON document string back to a Python object"""
     return json.loads(doc, cls=TurboBroccoliDecoder)
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli.egg-info/PKG-INFO` & `turbo_broccoli-2.3.8/turbo_broccoli.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo-broccoli
-Version: 2.3.0
+Version: 2.3.8
 Summary: JSON (de)serialization extensions
 Home-page: https://github.com/altaris/turbo-broccoli
 Author: Cédric Ho Thanh
 Author-email: altaris@users.noreply.github.com
 Project-URL: Issues, https://github.com/altaris/turbo-broccoli/issues
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
@@ -74,219 +74,187 @@
 ```py
 json.loads(json_string, cls=tb.TurboBroccoliDecoder)
 
 # or even simpler:
 tb.from_json(json_string)
 ```
 
-## Guarded calls
-
-Consider an expensive function `f` that returns a TurboBroccoli/JSON-izable
-`dict`. Wrapping/decorating `f` using `produces_document` essentially saves the
-result at a specified path and when possible, loads it instead of calling `f`.
-For example:
-
-```py
-_f = produces_document(f, "foo.json")
-_f(*args, **kwargs)
-```
-
-will only call `f` if the `foo.json` does not exist, and otherwise, loads and
-returns `foo.json`. However, if `foo.json` exists and was produced by calling
-`_f(*args, **kwargs)`, then
-
-```py
-_f(*args2, **kwargs2)
-```
-
-will still return the same result. If you want to keep a different file for
-each `args`/`kwargs`, set `check_args` to `True` as in
-
-```py
-_f = produces_document(f, "foo.json")
-_f(*args, **kwargs)
-```
-
-In this case, the arguments must be TurboBroccoli/JSON-izable, i.e. the
-document
-
-```
-{
-    "args": args,
-    "kwargs": kwargs,
-}
-```
-
-must be TurboBroccoli/JSON-izable. The resulting file is no longer
-`foo.json` but rather `foo.json/<hash>` where `hash` is the MD5
-hash of the serialization of the `args`/`kwargs` document above.
-
-If instead of a function you wish to guard an entire block of code, use
-`GuardedBlockHandler`:
-
-```py
-from turbo_broccoli import GuardedBlockHandler
-h = GuardedBlockHandler("foo.json")
-for _ in h.guard():
-    # This whole block will be skipped if foo.json exists
-    # If not, don't forget to set the results:
-    h.result = ...
-# In any case, the results of the block are now available in h.result
-```
-
-I know the syntax isn't the prettiest. It would be more natural to use a `with
-h.guard():` syntax but python doesn't allow for context managers that don't
-yield...
-
 ## Supported types
 
-- `bytes`
+### Basic types
+
+- [`bytes`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/bytes.html#to_json)
 
-- `collections.deque`, `collections.namedtuple`
+- `dict` with non `str` keys
 
-- Dataclasses. Serialization is straightforward:
+- [Collections](https://altaris.github.io/turbo-broccoli/turbo_broccoli/collections.html#to_json):
+  `collections.deque`, `collections.namedtuple`
 
+- [Dataclasses](https://altaris.github.io/turbo-broccoli/turbo_broccoli/dataclass.html#to_json): serialization is straightforward:
   ```py
   @dataclass
   class C:
       a: int
       b: str
 
   doc = json.dumps({"c": C(a=1, b="Hello")}, cls=tb.TurboBroccoliEncoder)
   ```
-
   For deserialization, first register the class:
-
   ```py
   tb.register_dataclass_type(C)
   json.loads(doc, cls=tb.TurboBroccoliDecoder)
   ```
 
-- _Generic object_, **serialization only**. A generic object is an object that
-  has the `__turbo_broccoli__` attribute. This attribute is expected to be a
-  list of attributes whose values will be serialized. For example,
-
-  ```py
-  class C:
-      __turbo_broccoli__ = ["a"]
-      a: int
-      b: int
-
-  x = C()
-  x.a, x.b = 42, 43
-  json.dumps(x, cls=tb.TurboBroccoliEncoder)
-  ```
+### [Generic objects](https://altaris.github.io/turbo-broccoli/turbo_broccoli/generic.html#to_json)
 
-  produces the following string (modulo indentation):
+**serialization only**. A generic object is an object that
+has the `__turbo_broccoli__` attribute. This attribute is expected to be a list
+of attributes whose values will be serialized. For example,
+```py
+class C:
+    __turbo_broccoli__ = ["a"]
+    a: int
+    b: int
 
-  ```json
-  {
-    "__generic__": {
-      "__version__": 1,
-      "data": {
-        "a": 42
-      }
+x = C()
+x.a, x.b = 42, 43
+json.dumps(x, cls=tb.TurboBroccoliEncoder)
+```
+produces the following string (modulo indentation):
+```json
+{
+  "__generic__": {
+    "__version__": 1,
+    "data": {
+      "a": 42
     }
   }
-  ```
+}
+```
 
-  Registered attributes can of course have any type supported by Turbo
-  Broccoli, such as numpy arrays. Registered attributes can be `@property`
-  methods.
+Registered attributes can of course have any type supported by Turbo Broccoli,
+such as numpy arrays. Registered attributes can be `@property` methods.
 
-- [`keras.Model`](https://keras.io/api/models/model/); standard subclasses of
-  [`keras.layers.Layer`](https://keras.io/api/layers/),
+### [Keras](https://altaris.github.io/turbo-broccoli/turbo_broccoli/keras.html#to_json)
+
+- [`keras.Model`](https://keras.io/api/models/model/);
+
+- standard subclasses of [`keras.layers.Layer`](https://keras.io/api/layers/),
   [`keras.losses.Loss`](https://keras.io/api/losses/),
   [`keras.metrics.Metric`](https://keras.io/api/metrics/), and
-  [`keras.optimizers.Optimizer`](https://keras.io/api/optimizers/)
+  [`keras.optimizers.Optimizer`](https://keras.io/api/optimizers/).
+
+### [Numpy](https://altaris.github.io/turbo-broccoli/turbo_broccoli/numpy.html#to_json)
+
+`numpy.number`, `numpy.ndarray` with numerical dtype, and `numpy.dtype`.
+
+### [Pandas](https://altaris.github.io/turbo-broccoli/turbo_broccoli/pandas.html#to_json)
+
+`pandas.DataFrame` and `pandas.Series`, but with the following limitations:
 
-- `numpy.number`, `numpy.ndarray` with numerical dtype
+- the following dtypes are not supported: `complex`, `object`, `timedelta`
 
-- `pandas.DataFrame` and `pandas.Series`, but with the following limitations:
+- the column / series names must be strings and not numbers. The following
+  is not acceptable:
+  ```py
+  df = pd.DataFrame([[1, 2], [3, 4]])
+  ```
+  because
+  ```py
+  print([c for c in df.columns])
+  # [0, 1]
+  print([type(c) for c in df.columns])
+  # [int, int]
+  ```
 
-  1. the following dtypes are not supported: `complex`, `object`, `timedelta`
-  2. the column / series names must be strings and not numbers. The following
-     is not acceptable:
-     ```py
-     df = pd.DataFrame([[1, 2], [3, 4]])
-     ```
-     because
-     ```py
-     print([c for c in df.columns])
-     # [0, 1]
-     print([type(c) for c in df.columns])
-     # [int, int]
-     ```
+### [Tensorflow](https://altaris.github.io/turbo-broccoli/turbo_broccoli/tensorflow.html#to_json)
 
-- `tensorflow.Tensor` with numerical dtype, but not `tensorflow.RaggedTensor`
+`tensorflow.Tensor` with numerical dtype, but not `tensorflow.RaggedTensor`.
 
-- `torch.Tensor`, **WARNING**: loaded tensors are automatically placed on the
-  CPU and gradients are lost; `torch.nn.Module`, don't forget to register your
+### [Pytorch](https://altaris.github.io/turbo-broccoli/turbo_broccoli/pytorch.html#to_json)
+
+- `torch.Tensor`, **Warning**: loaded tensors are automatically placed on the
+  CPU and gradients are lost;
+
+- `torch.nn.Module`, don't forget to register your
   module type using
-  [`turbo_broccoli.register_pytorch_module_type`]((https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#register_pytorch_module_type)):
-     ```py
-     # Serialization
-     class MyModule(torch.nn.Module):
-        ...
-
-     module = MyModule()  # Must be instantiable without arguments
-     doc = json.dumps(x, cls=tb.TurboBroccoliEncoder)
-
-     # Deserialization
-     tb.register_pytorch_module_type(MyModule)
-     module = json.loads(doc, cls=tb.TurboBroccoliDecoder)
-     ```
-  **WARNING**: It is not possible to register and deserialize [standard pytorch
+  [`turbo_broccoli.register_pytorch_module_type`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#register_pytorch_module_type):
+  ```py
+  # Serialization
+  class MyModule(torch.nn.Module):
+    ...
+
+  module = MyModule()  # Must be instantiable without arguments
+  doc = json.dumps(x, cls=tb.TurboBroccoliEncoder)
+
+  # Deserialization
+  tb.register_pytorch_module_type(MyModule)
+  module = json.loads(doc, cls=tb.TurboBroccoliDecoder)
+  ```
+  **Warning**: It is not possible to register and deserialize [standard pytorch
   module containers](https://pytorch.org/docs/stable/nn.html#containers)
   directly. Wrap them in your own custom module class.
 
-- `scipy.sparse.csr_matrix`
+### [Scipy](https://altaris.github.io/turbo-broccoli/turbo_broccoli/scipy.html#to_json)
+
+Just `scipy.sparse.csr_matrix`. ^^"
+
+### [Scikit-learn](https://altaris.github.io/turbo-broccoli/turbo_broccoli/sklearn.html#to_json)
+
+`sklearn` estimators (i.e. that descent from
+[`sklean.base.BaseEstimator`](https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html)).
+To make sure which class is supported, take a look at the [unit
+tests](https://github.com/altaris/turbo-broccoli/blob/main/tests/test_sklearn.py)
+Doesn't work with:
+
+- All CV classes because the `score_` attribute is a dict indexed with
+  `np.int64`, which `json.JSONEncoder._iterencode_dict` rejects.
+
+- All estimator classes that have mandatory arguments: `ClassifierChain`,
+  `ColumnTransformer`, `FeatureUnion`, `GridSearchCV`,
+  `MultiOutputClassifier`, `MultiOutputRegressor`, `OneVsOneClassifier`,
+  `OneVsRestClassifier`, `OutputCodeClassifier`, `Pipeline`,
+  `RandomizedSearchCV`, `RegressorChain`, `RFE`, `RFECV`, `SelectFromModel`,
+  `SelfTrainingClassifier`, `SequentialFeatureSelector`, `SparseCoder`,
+  `StackingClassifier`, `StackingRegressor`, `VotingClassifier`,
+  `VotingRegressor`.
+
+- Everything that is parametrized by an arbitrary object/callable/estimator:
+  `FunctionTransformer`, `TransformedTargetRegressor`.
+
+- Everything that stores a random state (in the form of a `RandomState`
+  object): `BisectingKMeans`, `MiniBatchDictionaryLearning`,
+  `LatentDirichletAllocation`, `NeighborhoodComponentsAnalysis`,
+  `MLPClassifier`, `MLPRegressor`, `SparseRandomProjection`,
+  `GaussianRandomProjection`.
+
+- Everything with trees and forest since `Tree` objects are not JSON
+  serializable: `ExtraTreesClassifier`, `ExtraTreesRegressor`,
+  `RandomForestClassifier`, `RandomForestRegressor`, `RandomTreesEmbedding`,
+  `IsolationForest`, `AdaBoostClassifier`, `AdaBoostRegressor`,
+  `DecisionTreeClassifier`, `DecisionTreeRegressor`.
+
+- Other classes that have non JSON-serializable attributes:
 
-- **EXPERIMENTAL** `sklearn` estimators (i.e. that descent from
-  [`sklean.base.BaseEstimator`](https://scikit-learn.org/stable/modules/generated/sklearn.base.BaseEstimator.html)).
-  To make sure which class is supported, take a look at the [unit
-  tests](https://github.com/altaris/turbo-broccoli/blob/main/tests/test_sklearn.py)
-  Doesn't work with:
-  * All CV classes because the `score_` attribute is a dict indexed with
-    `np.int64`, which `json.JSONEncoder._iterencode_dict` rejects.
-  * All estimator classes that have mandatory arguments: `ClassifierChain`,
-    `ColumnTransformer`, `FeatureUnion`, `GridSearchCV`,
-    `MultiOutputClassifier`, `MultiOutputRegressor`, `OneVsOneClassifier`,
-    `OneVsRestClassifier`, `OutputCodeClassifier`, `Pipeline`,
-    `RandomizedSearchCV`, `RegressorChain`, `RFE`, `RFECV`, `SelectFromModel`,
-    `SelfTrainingClassifier`, `SequentialFeatureSelector`, `SparseCoder`,
-    `StackingClassifier`, `StackingRegressor`, `VotingClassifier`,
-    `VotingRegressor`.
-  * Everything that is parametrized by an arbitrary object/callable/estimator:
-    `FunctionTransformer`, `TransformedTargetRegressor`.
-  * Everything that stores a random state (in the form of a `RandomState`
-    object): `BisectingKMeans`, `MiniBatchDictionaryLearning`,
-    `LatentDirichletAllocation`, `NeighborhoodComponentsAnalysis`,
-    `MLPClassifier`, `MLPRegressor`, `SparseRandomProjection`,
-    `GaussianRandomProjection`.
-  * Everything with trees and forest since `Tree` objects are not JSON
-    serializable: `ExtraTreesClassifier`, `ExtraTreesRegressor`,
-    `RandomForestClassifier`, `RandomForestRegressor`, `RandomTreesEmbedding`,
-    `IsolationForest`, `AdaBoostClassifier`, `AdaBoostRegressor`,
-    `DecisionTreeClassifier`, `DecisionTreeRegressor`.
-  * Other classes that have non JSON-serializable attributes:
     | Class                       | Non-serializable attr.    |
     | --------------------------- | ------------------------- |
     | `Birch`                     | `_CFNode`                 |
     | `GaussianProcessRegressor`  | `Sum`                     |
     | `GaussianProcessClassifier` | `Product`                 |
     | `Perceptron`                | `Hinge`                   |
     | `SGDClassifier`             | `Hinge`                   |
     | `SGDOneClassSVM`            | `Hinge`                   |
     | `PoissonRegressor`          | `HalfPoissonLoss`         |
     | `GammaRegressor`            | `HalfGammaLoss`           |
     | `TweedieRegressor`          | `HalfTweedieLossIdentity` |
     | `KernelDensity`             | `KDTree`                  |
     | `SplineTransformer`         | `BSpline`                 |
-  * Some classes have AttributeErrors?
+
+- Some classes have `AttributeErrors`?
+
     | Class                         | Attribute      |
     | ----------------------------- | -------------- |
     | `IsotonicRegression`          | `f_`           |
     | `KernelPCA`                   | `_centerer`    |
     | `KNeighborsClassifier`        | `_y`           |
     | `KNeighborsRegressor`         | `_y`           |
     | `KNeighborsTransformer`       | `_tree`        |
@@ -299,46 +267,53 @@
     | `OneClassSVM`                 | `_sparse`      |
     | `PowerTransformer`            | `_scaler`      |
     | `RadiusNeighborsClassifier`   | `_tree`        |
     | `RadiusNeighborsRegressor`    | `_tree`        |
     | `RadiusNeighborsTransformer`  | `_tree`        |
     | `SVC`                         | `_sparse`      |
     | `SVR`                         | `_sparse`      |
-  * Other errors:
-    * `FastICA`: I'm not sure why...
-    * `BaggingClassifier`: `IndexError: only integers, slices (:), ellipsis
-      (...), numpy.newaxis (None) and integer or boolean arrays are valid
-      indices`.
-    * `GradientBoostingClassifier`: `Exception: dtype object is not covered`.
-    * `GradientBoostingRegressor`: `Exception: dtype object is not covered`.
-    * `HistGradientBoostingClassifier`: Problems with deserialization of
-      `_BinMapper` object?
-    * `PassiveAggressiveClassifier`: some unknown label type error...
-    * `KBinsDiscretizer`: `Exception: dtype object is not covered`.
-    * `KBinsDiscretizer`: `Exception: dtype object is not covered`.
 
-- [Bokeh figures](https://docs.bokeh.org/en/latest) and
-  [models](https://docs.bokeh.org/en/latest/docs/reference/models.html).
+- Other errors:
 
-## Secrets
+  - `FastICA`: I'm not sure why...
+
+  - `BaggingClassifier`: `IndexError: only integers, slices (:), ellipsis
+    (...), numpy.newaxis (None) and integer or boolean arrays are valid
+    indices`.
+
+  - `GradientBoostingClassifier`, `GradientBoostingRegressor`: `Exception:
+    dtype object is not covered`.
+
+  - `HistGradientBoostingClassifier`: Problems with deserialization of
+    `_BinMapper` object?
+
+  - `PassiveAggressiveClassifier`: some unknown label type error...
+
+  - `KBinsDiscretizer`: `Exception: dtype object is not covered`.
+
+### [Bokeh](https://altaris.github.io/turbo-broccoli/turbo_broccoli/bokeh.html#to_json)
+
+Bokeh [figures](https://docs.bokeh.org/en/latest) and
+[models](https://docs.bokeh.org/en/latest/docs/reference/models.html).
+
+## [Secrets](https://altaris.github.io/turbo-broccoli/turbo_broccoli/secret.html#to_json)
 
 Basic Python types can be wrapped in their corresponding secret type according
 to the following table
 
 | Python type | Secret type                         |
 | ----------- | ----------------------------------- |
 | `dict`      | `turbo_broccoli.secret.SecretDict`  |
 | `float`     | `turbo_broccoli.secret.SecretFloat` |
 | `int`       | `turbo_broccoli.secret.SecretInt`   |
 | `list`      | `turbo_broccoli.secret.SecretList`  |
 | `str`       | `turbo_broccoli.secret.SecretStr`   |
 
 The secret value can be recovered with the `get_secret_value` method. At
 serialization, the this value will be encrypted. For example,
-
 ```py
 # See https://pynacl.readthedocs.io/en/latest/secret/#key
 import nacl.secret
 import nacl.utils
 
 key = nacl.utils.random(nacl.secret.SecretBox.KEY_SIZE)
 
@@ -349,18 +324,16 @@
 
 x = {
     "user": "alice",
     "password": SecretStr("dolphin")
 }
 json.dumps(x, cls=tb.TurboBroccoliEncoder)
 ```
-
 produces the following string (modulo indentation and modulo the encrypted
 content):
-
 ```json
 {
   "user": "alice",
   "password": {
     "__secret__": {
       "__version__": 1,
       "data": {
@@ -376,15 +349,15 @@
 
 Deserialization decrypts the secrets, but they stay wrapped inside the secret
 types above. If the wrong key is provided, an exception is raised. If no key is
 provided, the secret values are replaced by a
 `turbo_broccoli.secret.LockedSecret`. Internally, Turbo Broccoli uses
 [`pynacl`](https://pynacl.readthedocs.io/en/latest/)'s
 [`SecretBox`](https://pynacl.readthedocs.io/en/latest/secret/#nacl.secret.SecretBox).
-**WARNING**: In the case of `SecretDict` and `SecretList`, the values contained
+**Warning**: In the case of `SecretDict` and `SecretList`, the values contained
 within must be JSON-serializable **without** Turbo Broccoli. See also the
 `TB_SHARED_KEY` environment variable below.
 
 ## Environment variables
 
 Some behaviors of Turbo Broccoli can be tweaked by setting specific environment
 variables. If you want to modify these parameters programatically, do not do so
@@ -393,34 +366,30 @@
 
 - `TB_ARTIFACT_PATH` (default: `./`; see also
   [`turbo_broccoli.set_artifact_path`]((https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#set_artifact_path)),
   [`turbo_broccoli.environment.get_artifact_path`]((https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#get_artifact_path))):
   During serialization, Turbo Broccoli may create artifacts to which the JSON
   object will point to. The artifacts will be stored in `TB_ARTIFACT_PATH`. For
   example, if `arr` is a big numpy array,
-
   ```py
   obj = {"an_array": arr}
   json.dumps(obj, cls=tb.TurboBroccoliEncoder)
   ```
-
   will generate the following string (modulo indentation and id)
-
   ```json
   {
       "an_array": {
           "__numpy__": {
               "__type__": "ndarray",
               "__version__": 3,
               "id": "70692d08-c4cf-4231-b3f0-0969ea552d5a"
           }
       }
   }
   ```
-
   and a `70692d08-c4cf-4231-b3f0-0969ea552d5a` file has been created in
   `TB_ARTIFACT_PATH`.
 
 - `TB_KERAS_FORMAT` (default: `tf`, valid values are `json`, `h5`, and `tf`;
   see also
   [`turbo_broccoli.set_keras_format`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#set_keras_format),
   [`turbo_broccoli.environment.get_keras_format`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#get_keras_format)):
@@ -440,87 +409,111 @@
 
 - `TB_NODECODE` (default: empty; see also
   [`turbo_broccoli.set_nodecode`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#set_nodecode),
   [`turbo_broccoli.environment.is_nodecode`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#is_nodecode)):
   Comma-separated list of types to not deserialize, for example
   `bytes,numpy.ndarray`. Excludable types are:
 
+  - `bokeh`, `bokeh.buffer`, `bokeh.generic`,
+
   - `bytes`,
-  - `dataclass.<dataclass_name>` (case sensitive),
-  - `collections.deque`, `collections.namedtuple`,
-  - `keras.model`, `keras.layer`, `keras.loss`, `keras.metric`,
+
+  - `dict`,
+
+  - `collections`, `collections.deque`, `collections.namedtuple`,
+
+  - `dataclass`, `dataclass.<dataclass_name>` (case sensitive),
+
+  - `generic`,
+
+  - `keras`, `keras.model`, `keras.layer`, `keras.loss`, `keras.metric`,
     `keras.optimizer`,
-  - `numpy.ndarray`, `numpy.number`,
-  - `pandas.dataframe`, `pandas.series`, **WARNING: excluding
-    `pandas.dataframe` will crash any deserialization of `pandas.series`**
-  - `tensorflow.sparse_tensor`, `tensorflow.tensor`, `tensorflow.variable`.
-    **WARNING**: excluding `numpy.ndarray` will may crash deserialization of
-    Tensorflow and Pandas types.
+
+  - `numpy`, `numpy.ndarray`, `numpy.number`, `numpy.dtype`,
+
+  - `pandas`, `pandas.dataframe`, `pandas.series`, **Warning**: excluding
+    `pandas.dataframe` will crash any deserialization of `pandas.series`,
+
+  - `pytorch`, `pytorch.tensor`, `pytorch.module`,
+
+  - `scipy`, `scipy.csr_matrix`,
+
+  - `secret`,
+
+  - `sklearn`, `sklearn.estimator`, `sklearn.estimator.<estimator name>` (case
+    sensitive, see the list of supported sklearn estimators), `sklearn.tree`,
+
+  - `tensorflow`, `tensorflow.sparse_tensor`, `tensorflow.tensor`,
+    `tensorflow.variable`.
 
 - `TB_SHARED_KEY` (default: empty; see also
   [`turbo_broccoli.set_shared_key`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#set_shared_key),
   [`turbo_broccoli.environment.get_shared_key`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/environment.html#get_shared_key)):
   Secret key used to encrypt secrets. The encryption uses [`pynacl`'s
   `SecretBox`](https://pynacl.readthedocs.io/en/latest/secret/#nacl.secret.SecretBox).
   An exception is raised when attempting to serialize a secret type while no
   key is set.
 
+## Guarded calls
+
+This is so cool. Check out
+[`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler),
+[`turbo_broccoli.guarded_call`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#guarded_call),
+and
+[`turbo_broccoli.produces_document`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#produces_document).
+
 # Contributing
 
 ## Dependencies
 
 - `python3.9` or newer;
+
 - `requirements.txt` for runtime dependencies;
+
 - `requirements.dev.txt` for development dependencies.
+
 - `make` (optional);
 
 Simply run
-
 ```sh
 virtualenv venv -p python3.9
 . ./venv/bin/activate
 pip install --upgrade pip
 pip install -r requirements.txt
 pip install -r requirements.dev.txt
 ```
 
 ## Documentation
 
 Simply run
-
 ```sh
 make docs
 ```
 
 This will generate the HTML doc of the project, and the index file should be at
 `docs/index.html`. To have it directly in your browser, run
-
 ```sh
 make docs-browser
 ```
 
 ## Code quality
 
 Don't forget to run
-
 ```sh
 make
 ```
-
 to format the code following [black](https://pypi.org/project/black/),
 typecheck it using [mypy](http://mypy-lang.org/), and check it against coding
 standards using [pylint](https://pylint.org/).
 
 ## Unit tests
 
 Run
-
 ```sh
 make test
 ```
-
 to have [pytest](https://docs.pytest.org/) run the unit tests in `tests/`.
 
 # Credits
 
 This project takes inspiration from
 [Crimson-Crow/json-numpy](https://github.com/Crimson-Crow/json-numpy).
```

### Comparing `turbo_broccoli-2.3.0/turbo_broccoli.egg-info/SOURCES.txt` & `turbo_broccoli-2.3.8/turbo_broccoli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 requirements.txt
 setup.py
 tests/test_bokeh.py
 tests/test_bytes.py
 tests/test_collections.py
 tests/test_dataclass.py
+tests/test_dict.py
 tests/test_generic.py
 tests/test_guard.py
 tests/test_keras.py
 tests/test_nodecode.py
 tests/test_numpy.py
 tests/test_pandas.py
 tests/test_pytorch.py
@@ -19,14 +20,15 @@
 tests/test_sklearn.py
 tests/test_tensorflow.py
 turbo_broccoli/__init__.py
 turbo_broccoli/bokeh.py
 turbo_broccoli/bytes.py
 turbo_broccoli/collections.py
 turbo_broccoli/dataclass.py
+turbo_broccoli/dict.py
 turbo_broccoli/environment.py
 turbo_broccoli/generic.py
 turbo_broccoli/guard.py
 turbo_broccoli/keras.py
 turbo_broccoli/numpy.py
 turbo_broccoli/pandas.py
 turbo_broccoli/pytorch.py
```

