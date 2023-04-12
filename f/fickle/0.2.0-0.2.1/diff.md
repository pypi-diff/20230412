# Comparing `tmp/fickle-0.2.0.tar.gz` & `tmp/fickle-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fickle-0.2.0.tar", last modified: Fri Mar 31 04:34:18 2023, max compression
+gzip compressed data, was "fickle-0.2.1.tar", last modified: Wed Apr 12 08:41:22 2023, max compression
```

## Comparing `fickle-0.2.0.tar` & `fickle-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-31 04:34:18.664497 fickle-0.2.0/
--rw-r--r--   0 user      (1000) user      (1000)       37 2023-03-31 04:34:09.000000 fickle-0.2.0/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     3364 2023-03-31 04:34:18.664497 fickle-0.2.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2511 2023-03-31 02:29:03.000000 fickle-0.2.0/README.md
--rw-r--r--   0 user      (1000) user      (1000)       50 2023-03-31 02:29:03.000000 fickle-0.2.0/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)      105 2023-03-31 04:34:18.664497 fickle-0.2.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      726 2023-03-31 02:29:03.000000 fickle-0.2.0/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-31 04:34:18.654497 fickle-0.2.0/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-31 04:34:18.664497 fickle-0.2.0/src/fickle/
--rw-r--r--   0 user      (1000) user      (1000)       92 2023-03-31 02:29:03.000000 fickle-0.2.0/src/fickle/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      189 2023-03-31 02:29:03.000000 fickle-0.2.0/src/fickle/exc.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-31 04:34:18.664497 fickle-0.2.0/src/fickle/ext/
--rw-r--r--   0 user      (1000) user      (1000)      143 2023-03-31 02:29:03.000000 fickle-0.2.0/src/fickle/ext/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     6576 2023-03-31 02:29:03.000000 fickle-0.2.0/src/fickle/ext/marshmallow.py
--rw-r--r--   0 user      (1000) user      (1000)     5624 2023-03-31 02:29:03.000000 fickle-0.2.0/src/fickle/ext/pytorch.py
--rw-r--r--   0 user      (1000) user      (1000)    25622 2023-03-31 02:29:03.000000 fickle-0.2.0/src/fickle/firewall.py
--rw-r--r--   0 user      (1000) user      (1000)     8353 2023-03-31 02:29:03.000000 fickle-0.2.0/src/fickle/unpickler.py
--rw-r--r--   0 user      (1000) user      (1000)      788 2023-03-31 02:29:03.000000 fickle-0.2.0/src/fickle/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-31 04:34:18.664497 fickle-0.2.0/src/fickle.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3364 2023-03-31 04:34:18.000000 fickle-0.2.0/src/fickle.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      495 2023-03-31 04:34:18.000000 fickle-0.2.0/src/fickle.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-03-31 04:34:18.000000 fickle-0.2.0/src/fickle.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        6 2023-03-31 04:34:18.000000 fickle-0.2.0/src/fickle.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2023-03-31 04:34:18.000000 fickle-0.2.0/src/fickle.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-31 04:34:18.664497 fickle-0.2.0/tests/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-03-31 02:29:03.000000 fickle-0.2.0/tests/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      337 2023-03-31 02:29:03.000000 fickle-0.2.0/tests/conftest.py
--rw-r--r--   0 user      (1000) user      (1000)     1550 2023-03-31 02:29:03.000000 fickle-0.2.0/tests/test_danger.py
--rw-r--r--   0 user      (1000) user      (1000)     1725 2023-03-31 02:29:03.000000 fickle-0.2.0/tests/test_roundtrip.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:41:22.318241 fickle-0.2.1/
+-rw-r--r--   0 user      (1000) user      (1000)       37 2023-03-31 04:34:09.000000 fickle-0.2.1/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     3364 2023-04-12 08:41:22.318241 fickle-0.2.1/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2511 2023-03-31 02:29:03.000000 fickle-0.2.1/README.md
+-rw-r--r--   0 user      (1000) user      (1000)       50 2023-03-31 02:29:03.000000 fickle-0.2.1/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)      105 2023-04-12 08:41:22.318241 fickle-0.2.1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      726 2023-04-12 08:41:14.000000 fickle-0.2.1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:41:22.318241 fickle-0.2.1/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:41:22.318241 fickle-0.2.1/src/fickle/
+-rw-r--r--   0 user      (1000) user      (1000)       92 2023-03-31 02:29:03.000000 fickle-0.2.1/src/fickle/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      189 2023-03-31 02:29:03.000000 fickle-0.2.1/src/fickle/exc.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:41:22.318241 fickle-0.2.1/src/fickle/ext/
+-rw-r--r--   0 user      (1000) user      (1000)      143 2023-03-31 02:29:03.000000 fickle-0.2.1/src/fickle/ext/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     6576 2023-03-31 02:29:03.000000 fickle-0.2.1/src/fickle/ext/marshmallow.py
+-rw-r--r--   0 user      (1000) user      (1000)     5970 2023-04-12 08:41:14.000000 fickle-0.2.1/src/fickle/ext/pytorch.py
+-rw-r--r--   0 user      (1000) user      (1000)    25680 2023-04-12 08:41:14.000000 fickle-0.2.1/src/fickle/firewall.py
+-rw-r--r--   0 user      (1000) user      (1000)     8353 2023-03-31 02:29:03.000000 fickle-0.2.1/src/fickle/unpickler.py
+-rw-r--r--   0 user      (1000) user      (1000)      788 2023-03-31 02:29:03.000000 fickle-0.2.1/src/fickle/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:41:22.318241 fickle-0.2.1/src/fickle.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3364 2023-04-12 08:41:21.000000 fickle-0.2.1/src/fickle.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      495 2023-04-12 08:41:22.000000 fickle-0.2.1/src/fickle.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-12 08:41:21.000000 fickle-0.2.1/src/fickle.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        6 2023-04-12 08:41:21.000000 fickle-0.2.1/src/fickle.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2023-04-12 08:41:21.000000 fickle-0.2.1/src/fickle.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:41:22.318241 fickle-0.2.1/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-03-31 02:29:03.000000 fickle-0.2.1/tests/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      337 2023-03-31 02:29:03.000000 fickle-0.2.1/tests/conftest.py
+-rw-r--r--   0 user      (1000) user      (1000)     1550 2023-03-31 02:29:03.000000 fickle-0.2.1/tests/test_danger.py
+-rw-r--r--   0 user      (1000) user      (1000)     1725 2023-03-31 02:29:03.000000 fickle-0.2.1/tests/test_roundtrip.py
```

### Comparing `fickle-0.2.0/PKG-INFO` & `fickle-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fickle
-Version: 0.2.0
+Version: 0.2.1
 Summary: load pickled data as safely as possible
 Home-page: UNKNOWN
 Author: Eduard Christian Dumitrescu
 Author-email: eduard.c.dumitrescu@gmail.com
 License: MIT
 Description: # Fickle: Firewalled Pickle
```

### Comparing `fickle-0.2.0/README.md` & `fickle-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fickle-0.2.0/src/fickle/ext/marshmallow.py` & `fickle-0.2.1/src/fickle/ext/marshmallow.py`

 * *Files identical despite different names*

### Comparing `fickle-0.2.0/src/fickle/ext/pytorch.py` & `fickle-0.2.1/src/fickle/ext/pytorch.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 This is a module implementing loading for a decent subset of the format.
 """
 
 import dataclasses
 import functools
 import operator
 import pathlib
-import warnings
 import zipfile
 from contextlib import contextmanager
 from contextvars import ContextVar
 from typing import Tuple
 
 import attr
 import numpy as np
@@ -48,72 +47,57 @@
     stride: Tuple[int]
     requires_grad: bool
     backward_hooks: object
     storage_manager: "StorageManager" = dataclasses.field(
         default_factory=lambda: storage_manager_var.get(None)
     )
 
-    # do not add "object" to the list below, because then it will try to load
-    # python objects using pickle
-    ALLOWED_DTYPES = {
-        "float16",
-        "float32",
-        "int8",
-        "int16",
-        "int32",
-        "int64",
-        "uint8",
-        "uint16",
-        "uint32",
-        "uint64",
-    }
+    PYTORCH_DTYPE_TO_ITEMSIZE = {"bfloat16": 2, "bool": 1}
+    PYTORCH_DTYPE_TO_ITEMSIZE.update((f"float{n * 8}", n) for n in (2, 4, 8))
+    PYTORCH_DTYPE_TO_ITEMSIZE.update((f"complex{n * 8}", n) for n in (8, 16))
+    PYTORCH_DTYPE_TO_ITEMSIZE.update((f"int{n * 8}", n) for n in (1, 2, 4, 8))
+    PYTORCH_DTYPE_TO_ITEMSIZE.update((f"uint{n * 8}", n) for n in (1, 2, 4, 8))
 
     @functools.cached_property
-    def dtype(self):
+    def numpy_dtype(self):
         dtype = self.storage.dtype
-        if dtype not in self.ALLOWED_DTYPES:
-            warnings.warn(f"not loading dtype {dtype!r}", InvalidDTypeWarning)
-            return None
+        if dtype not in self.PYTORCH_DTYPE_TO_ITEMSIZE:
+            raise ValueError("invalid dtype: {dtype!r}")
 
         return np.dtype(dtype).newbyteorder("<")
 
     @property
-    def obj_key(self):
-        return self.storage.key
-
-    def _byte_size(self):
-        return functools.reduce(operator.mul, self.size, self.dtype.itemsize)
+    def size_in_bytes(self) -> int:
+        itemsize = self.PYTORCH_DTYPE_TO_ITEMSIZE[self.storage.dtype]
+        return functools.reduce(operator.mul, self.size, itemsize)
 
     def _load_from_file(self, fileobj):
-        byte_size = self._byte_size()
+        byte_size = self.size_in_bytes
         fileobj.seek(self.storage_offset)
         buf: bytes = fileobj.read(byte_size)
         if len(buf) != byte_size:
             raise ValueError(f"expected {len(buf)} bytes, got {byte_size}")
-        return self._load_from_buffer(buf)
-
-    def _load_from_buffer(self, buffer):
-        dt = self.dtype
-        if dt is None:
-            return
+        return buf
 
-        return np.frombuffer(buffer, self.dtype).reshape(self.size)
+    def _buffer_to_numpy(self, buffer):
+        return np.frombuffer(buffer, self.numpy_dtype).reshape(self.size)
 
     def _load_from_zipfile(self):
-        if self.dtype is None:
-            return
-
-        with self.storage_manager.open(f"data/{self.obj_key}") as f:
+        with self.storage_manager.open(f"data/{self.storage.key}") as f:
             return self._load_from_file(f)
 
     @property
     def array(self):
-        if self.dtype is None:
-            raise AssertionError("invalid dtype")
+        if self.numpy_dtype is None:
+            raise ValueError(f"invalid dtype {self.storage.dtype!r}")
+
+        return self._buffer_to_numpy(self.buffer)
 
+    @property
+    def buffer(self):
         return self._load_from_zipfile()
 
 
 @attr.s
 class StorageInfo:
     dtype: str = attr.ib()
     key: str = attr.ib()
@@ -158,18 +142,26 @@
         stride = mext.XListAsPyTuple(fields.Integer())
         requires_grad = fields.Boolean()
         backward_hooks = fields.Raw()
 
 
 class StorageHandler(Handler):
     imports = {
+        "torch:BFloat16Storage": "bfloat16",
         "torch:HalfStorage": "float16",
         "torch:FloatStorage": "float32",
+        "torch:DoubleStorage": "float64",
+        "torch:ComplexFloatStorage": "complex64",
+        "torch:ComplexDoubleStorage": "complex128",
+        "torch:BoolStorage": "bool",
+        "torch:CharStorage": "int8",
+        "torch:ShortStorage": "int16",
         "torch:IntStorage": "int32",
         "torch:LongStorage": "int64",
+        "torch:ByteStorage": "uint8",
     }
     imports_register_instance = False
 
 
 class PyTorchFirewall(DefaultFirewall):
     def get_autoregister_handlers(self):
         handlers = super().get_autoregister_handlers()
```

### Comparing `fickle-0.2.0/src/fickle/firewall.py` & `fickle-0.2.1/src/fickle/firewall.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     "ImportRequest",
     "BaseHandler",
     "Handler",
     "Import",
     "Literal",
     "Factory",
     "Method",
+    "Unknown",
+    "UnknownImport",
+    "UnknownHandler",
     "UseDefault",
     "ListHandler",
     "DictHandler",
     "SetHandler",
     "OrderedDictHandler",
     "CodecsEncodeHandler",
     "ComplexHandler",
```

### Comparing `fickle-0.2.0/src/fickle/unpickler.py` & `fickle-0.2.1/src/fickle/unpickler.py`

 * *Files identical despite different names*

### Comparing `fickle-0.2.0/src/fickle/util.py` & `fickle-0.2.1/src/fickle/util.py`

 * *Files identical despite different names*

### Comparing `fickle-0.2.0/src/fickle.egg-info/PKG-INFO` & `fickle-0.2.1/src/fickle.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fickle
-Version: 0.2.0
+Version: 0.2.1
 Summary: load pickled data as safely as possible
 Home-page: UNKNOWN
 Author: Eduard Christian Dumitrescu
 Author-email: eduard.c.dumitrescu@gmail.com
 License: MIT
 Description: # Fickle: Firewalled Pickle
```

### Comparing `fickle-0.2.0/tests/test_danger.py` & `fickle-0.2.1/tests/test_danger.py`

 * *Files identical despite different names*

### Comparing `fickle-0.2.0/tests/test_roundtrip.py` & `fickle-0.2.1/tests/test_roundtrip.py`

 * *Files identical despite different names*

