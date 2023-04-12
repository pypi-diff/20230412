# Comparing `tmp/arraymap-0.1.0.tar.gz` & `tmp/arraymap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraymap-0.1.0.tar", last modified: Wed Apr 12 15:14:45 2023, max compression
+gzip compressed data, was "arraymap-0.1.1.tar", last modified: Wed Apr 12 15:54:20 2023, max compression
```

## Comparing `arraymap-0.1.0.tar` & `arraymap-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-04-12 15:14:45.067151 arraymap-0.1.0/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1150 2023-04-12 01:20:18.000000 arraymap-0.1.0/LICENSE.md
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       19 2022-08-22 21:16:28.000000 arraymap-0.1.0/MANIFEST.in
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      652 2023-04-12 15:14:45.067151 arraymap-0.1.0/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      300 2023-04-12 15:12:53.000000 arraymap-0.1.0/README.md
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    65288 2023-04-12 01:20:18.000000 arraymap-0.1.0/arraymap.c
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-04-12 15:14:45.067151 arraymap-0.1.0/arraymap.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      652 2023-04-12 15:14:44.000000 arraymap-0.1.0/arraymap.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      230 2023-04-12 15:14:44.000000 arraymap-0.1.0/arraymap.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-04-12 15:14:44.000000 arraymap-0.1.0/arraymap.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        9 2023-04-12 15:14:44.000000 arraymap-0.1.0/arraymap.egg-info/top_level.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       76 2023-04-12 15:14:45.067151 arraymap-0.1.0/setup.cfg
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1041 2023-04-12 15:11:16.000000 arraymap-0.1.0/setup.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-04-12 15:14:45.067151 arraymap-0.1.0/test/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4907 2023-04-12 01:23:56.000000 arraymap-0.1.0/test/test_property.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14714 2023-04-12 01:23:56.000000 arraymap-0.1.0/test/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:54:20.002659 arraymap-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-12 15:54:17.000000 arraymap-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 15:54:17.000000 arraymap-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-12 15:54:20.002659 arraymap-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-12 15:54:17.000000 arraymap-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    60734 2023-04-12 15:54:17.000000 arraymap-0.1.1/arraymap.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:54:20.002659 arraymap-0.1.1/arraymap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-12 15:54:19.000000 arraymap-0.1.1/arraymap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 15:54:19.000000 arraymap-0.1.1/arraymap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:54:19.000000 arraymap-0.1.1/arraymap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 15:54:19.000000 arraymap-0.1.1/arraymap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-12 15:54:20.002659 arraymap-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-12 15:54:17.000000 arraymap-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:54:20.002659 arraymap-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-12 15:54:17.000000 arraymap-0.1.1/test/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-04-12 15:54:17.000000 arraymap-0.1.1/test/test_unit.py
```

### Comparing `arraymap-0.1.0/LICENSE.md` & `arraymap-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arraymap-0.1.0/PKG-INFO` & `arraymap-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,38 @@
-Metadata-Version: 2.1
-Name: arraymap
-Version: 0.1.0
-Summary: Dictionary-like lookup from NumPy array values to their integer positions
-Home-page: https://github.com/static-frame/arraymap
-Author: Christopher Ariza, Brandt Bucher
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 
 arraymap
 ============
 
 The ArrayMap library provides dictionary-like lookup from NumPy array values to their integer positions. The hash table design and C implementation is based on [AutoMap](https://github.com/brandtbucher/automap), with extensive additions for direct support of NumPy arrays.
 
 
+Code: https://github.com/static-frame/arraymap
+
+Packages: https://pypi.org/project/arraymap
+
+
+
+Dependencies
+--------------
+
+ArrayMap requires the following:
+
+- Python >= 3.7
+- NumPy >= 1.18.5
+
+
+
+What is New in ArrayMap
+-------------------------
+
+
+0.1.1
+-------
+
+Added `__version__` to module; releasing wheels.
+
 
+0.1.0
+-------
 
+Initial release with NumPy integration.
```

### Comparing `arraymap-0.1.0/arraymap.c` & `arraymap-0.1.1/arraymap.c`

 * *Files 9% similar despite different names*

```diff
@@ -1,117 +1,12 @@
-// TODO: Rewrite performance tests using pyperf.
-// TODO: Group similar functionality.
-// TODO: Check refcounts when calling into hash and comparison functions.
-// TODO: Check allocation and cleanup.
-// TODO: Subinterpreter support.
-// TODO: Docstrings and stubs.
-// TODO: GC support.
 
+// For background on the hashtable design first implemented in AutoMap, see the following:
+// https://github.com/brandtbucher/automap/blob/b787199d38d6bfa1b55484e5ea1e89b31cc1fa72/automap.c#L12
 
-/*******************************************************************************
 
-Our use cases differ significantly from Python's general-purpose dict type, even
-when setting aside the whole immutable/grow-only and contiguous-integer-values
-stuff.
-
-What we don't care about:
-
-  - Memory usage. Python's dicts are used literally everywhere, so a tiny
-    reduction in the footprint of the average dict results in a significant gain
-    for *all* Python programs. We are happy to instead trade a few extra bytes
-    of RAM for a more cache-friendly hash table design. Since we don't store
-    values, we are still close to the same size on average!
-
-  - Worst-case performance. Again, Python's dicts are used for literally
-    everything, so they need to be able to gracefully handle lots of hash
-    collisions, whether resulting from bad hash algorithms, heterogeneous keys
-    with badly-combining hash algorithms, or maliciously-formed input. We can
-    safely assume that our use cases don't need to worry about these issues, and
-    instead choose lookup and collision resolution strategies that utilize cache
-    lines more effectively. This extends to the case of lookups for nonexistent
-    keys as well; we can assume that if our users are looking for something,
-    they know that it's probably there.
-
-What we do care about:
-
-  - Creation and update time. This is *by far* the most expensive operation you
-    do on a mapping. More on this below.
-
-  - The speed of lookups that result in hits. This is what the mapping is used
-    for, so it *must* be good. More on this below.
-
-  - Iteration order and speed. You really can't beat a Python list or tuple
-    here, so we can just store the keys in one of them to avoid reinventing the
-    wheel. We use a list since it allows us to grow more efficiently.
-
-So what we need is a hash table that's easy to insert into and easy to scan.
-
-Here's how it works. A vanilla Python dict of the form:
-
-{a: 0, b: 1, c: 2}
-
-...basically looks like this (assume the hashes are 3, 6, and 9):
-
-Indices: [-, 2, -, 0, -, -, 1,  -]
-
-Hashes:  [3, 6, 9, -, -]
-Keys:    [a, b, c, -, -]
-Values:  [0, 1, 2  -, -]
-
-It's pretty standard; keys, values, and cached hashes are stored in sequential
-order, and their offsets are placed in the Indices table at position
-HASH % TABLE_SIZE. Though it's not used here, collisions are resolved by jumping
-around the table according to the following recurrence:
-
-NEXT_INDEX = (5 * CURRENT_INDEX + 1 + (HASH >>= 5)) % TABLE_SIZE
-
-This is good in the face of bad hash algorithms, but is sorta expensive. It's
-also unable to utilize cache lines at all, since it's basically random (it's
-literally based on random number generation)!
-
-To contrast, the same table looks something like this for us:
-
-Indices: [-, -, -, 0, -, -, 1, -, -, 2, -, -, -, -, -, -, -, -, -]
-Hashes:  [-, -, -, 3, -, -, 6, -, -, 9, -, -, -, -, -, -, -, -, -]
-
-Keys:    [a,  b,  c]
-
-Right away you can see that we don't need to store the values, because they
-match the indices (by design).
-
-Notice that even though we allocated enough space in our table for 19 entries,
-we still insert them into initial position HASH % 4.  This leaves the whole
-15-element tail chunk of the table free for colliding keys. So, what's a good
-collision-resolution strategy?
-
-NEXT_INDEX = CURRENT_INDEX + 1
-
-It's just a sequential scan! That means *every* collision-resolution lookup is
-hot in L1 cache (and can even be predicted and speculatively executed). The
-indices and hashes are actually interleaved for better cache locality as well.
-
-We repeat this scan 15 times. We don't even have to worry about wrapping around
-the edge of the table during this part, since we've left enough free space
-(equal to the number of scans) to safely run over the end. It's wasteful for a
-small example like this, but for more realistic sizes it's just about perfect.
-
-We then jump to another spot in the table using a version of the recurrence
-above:
-
-NEXT_INDEX = (5 * (CURRENT_INDEX - 15) + 1 + (HASH >>= 1)) % TABLE_SIZE
-
-...and repeat the whole thing over again. This collision resolution strategy is
-similar to what Python's sets do, so we still handle some nasty collisions and
-missing keys well.
-
-There are a couple of other tricks that we use (like globally caching integer
-objects from value lookups), but the hardware-friendly hash table design is what
-really gives us our awesome performance.
-
-*******************************************************************************/
 # include <math.h>
 # define PY_SSIZE_T_CLEAN
 # include "Python.h"
 
 # define PY_ARRAY_UNIQUE_SYMBOL AK_ARRAY_API
 # define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 
@@ -2206,24 +2101,25 @@
             "ValueError for non-unique values.",
             PyExc_ValueError,
             NULL);
     if (NonUniqueError == NULL) {
         return NULL;
     }
 
-    PyObject *arraymap = PyModule_Create(&arraymap_module);
+    PyObject *m = PyModule_Create(&arraymap_module);
     if (
-        !arraymap
+        !m
+        || PyModule_AddStringConstant(m, "__version__", Py_STRINGIFY(AM_VERSION))
         || PyType_Ready(&AMType)
         || PyType_Ready(&FAMIType)
         || PyType_Ready(&FAMVType)
         || PyType_Ready(&FAMType)
-        || PyModule_AddObject(arraymap, "AutoMap", (PyObject *)&AMType)
-        || PyModule_AddObject(arraymap, "FrozenAutoMap", (PyObject *)&FAMType)
-        || PyModule_AddObject(arraymap, "NonUniqueError", NonUniqueError)
+        || PyModule_AddObject(m, "AutoMap", (PyObject *)&AMType)
+        || PyModule_AddObject(m, "FrozenAutoMap", (PyObject *)&FAMType)
+        || PyModule_AddObject(m, "NonUniqueError", NonUniqueError)
     ) {
-        Py_XDECREF(arraymap);
+        Py_XDECREF(m);
         return NULL;
     }
-    return arraymap;
+    return m;
 }
```

### Comparing `arraymap-0.1.0/arraymap.egg-info/PKG-INFO` & `arraymap-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,49 @@
 Metadata-Version: 2.1
 Name: arraymap
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dictionary-like lookup from NumPy array values to their integer positions
 Home-page: https://github.com/static-frame/arraymap
 Author: Christopher Ariza, Brandt Bucher
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
 arraymap
 ============
 
 The ArrayMap library provides dictionary-like lookup from NumPy array values to their integer positions. The hash table design and C implementation is based on [AutoMap](https://github.com/brandtbucher/automap), with extensive additions for direct support of NumPy arrays.
 
 
+Code: https://github.com/static-frame/arraymap
 
+Packages: https://pypi.org/project/arraymap
 
 
+
+Dependencies
+--------------
+
+ArrayMap requires the following:
+
+- Python >= 3.7
+- NumPy >= 1.18.5
+
+
+
+What is New in ArrayMap
+-------------------------
+
+
+0.1.1
+-------
+
+Added `__version__` to module; releasing wheels.
+
+
+0.1.0
+-------
+
+Initial release with NumPy integration.
+
```

### Comparing `arraymap-0.1.0/setup.py` & `arraymap-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import setuptools
 import typing as tp
 import site
 import os
 
+
+AM_VERSION = "0.1.1"
+
+
 with open("README.md") as file:
     LONG_DESCRIPTION = file.read()
 
 
 def get_ext_dir(*components: tp.Iterable[str]) -> tp.Sequence[str]:
     dirs = []
     for sp in site.getsitepackages():
@@ -17,23 +21,24 @@
 
 
 extension = setuptools.Extension(
     "arraymap",
     ["arraymap.c"],
     include_dirs=get_ext_dir("numpy", "core", "include"),
     library_dirs=get_ext_dir("numpy", "core", "lib"),
+    define_macros=[("AM_VERSION", AM_VERSION)],
     libraries=["npymath"],  # not including mlib at this time
 )
 
 
 setuptools.setup(
     author="Christopher Ariza, Brandt Bucher",
+    version=AM_VERSION,
     description="Dictionary-like lookup from NumPy array values to their integer positions",
     ext_modules=[extension],
     license="MIT",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     name="arraymap",
     python_requires=">=3.7.0",
     url="https://github.com/static-frame/arraymap",
-    version="0.1.0",
 )
```

### Comparing `arraymap-0.1.0/test/test_property.py` & `arraymap-0.1.1/test/test_property.py`

 * *Files identical despite different names*

### Comparing `arraymap-0.1.0/test/test_unit.py` & `arraymap-0.1.1/test/test_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 import sys
 import numpy as np
 
 from arraymap import AutoMap
 from arraymap import FrozenAutoMap
 from arraymap import NonUniqueError
 
+def test_version():
+    import arraymap
+    assert isinstance(arraymap.__version__, str)
+
+
+# ------------------------------------------------------------------------------
+
 
 def test_am_extend():
     am1 = AutoMap(("a", "b"))
     am2 = am1 | AutoMap(("c", "d"))
     assert list(am2.keys()) == ["a", "b", "c", "d"]
```

