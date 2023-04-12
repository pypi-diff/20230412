# Comparing `tmp/pure_safetensors-0.2.0.tar.gz` & `tmp/pure_safetensors-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_safetensors-0.2.0.tar", last modified: Mon Apr 10 08:59:53 2023, max compression
+gzip compressed data, was "pure_safetensors-0.3.0.tar", last modified: Wed Apr 12 08:38:33 2023, max compression
```

## Comparing `pure_safetensors-0.2.0.tar` & `pure_safetensors-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 08:59:53.166548 pure_safetensors-0.2.0/
--rw-r--r--   0 user      (1000) user      (1000)     3660 2023-04-10 08:59:53.166548 pure_safetensors-0.2.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2741 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/README.md
--rw-r--r--   0 user      (1000) user      (1000)       50 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)      110 2023-04-10 08:59:53.166548 pure_safetensors-0.2.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      756 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 08:59:53.166548 pure_safetensors-0.2.0/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 08:59:53.166548 pure_safetensors-0.2.0/src/pure_safetensors/
--rw-r--r--   0 user      (1000) user      (1000)       35 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/src/pure_safetensors/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      163 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/src/pure_safetensors/exc.py
--rw-r--r--   0 user      (1000) user      (1000)     6921 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/src/pure_safetensors/mmap.py
--rw-r--r--   0 user      (1000) user      (1000)     1570 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/src/pure_safetensors/numpy.py
--rw-r--r--   0 user      (1000) user      (1000)    24148 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/src/pure_safetensors/safetensors.py
--rw-r--r--   0 user      (1000) user      (1000)     1158 2023-04-10 08:57:54.000000 pure_safetensors-0.2.0/src/pure_safetensors/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 08:59:53.166548 pure_safetensors-0.2.0/src/pure_safetensors.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3660 2023-04-10 08:59:52.000000 pure_safetensors-0.2.0/src/pure_safetensors.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      447 2023-04-10 08:59:52.000000 pure_safetensors-0.2.0/src/pure_safetensors.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-10 08:59:52.000000 pure_safetensors-0.2.0/src/pure_safetensors.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       36 2023-04-10 08:59:52.000000 pure_safetensors-0.2.0/src/pure_safetensors.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-10 08:59:52.000000 pure_safetensors-0.2.0/src/pure_safetensors.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:38:33.558594 pure_safetensors-0.3.0/
+-rw-r--r--   0 user      (1000) user      (1000)     4165 2023-04-12 08:38:33.558594 pure_safetensors-0.3.0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     3174 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/README.md
+-rw-r--r--   0 user      (1000) user      (1000)       50 2023-04-10 08:57:54.000000 pure_safetensors-0.3.0/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)      110 2023-04-12 08:38:33.558594 pure_safetensors-0.3.0/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      756 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:38:33.548594 pure_safetensors-0.3.0/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:38:33.548594 pure_safetensors-0.3.0/src/pure_safetensors/
+-rw-r--r--   0 user      (1000) user      (1000)       35 2023-04-10 08:57:54.000000 pure_safetensors-0.3.0/src/pure_safetensors/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2270 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/__main__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2329 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/adapter.py
+-rw-r--r--   0 user      (1000) user      (1000)      163 2023-04-10 08:57:54.000000 pure_safetensors-0.3.0/src/pure_safetensors/exc.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:38:33.558594 pure_safetensors-0.3.0/src/pure_safetensors/ext/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/ext/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3305 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/ext/torch.py
+-rw-r--r--   0 user      (1000) user      (1000)     4194 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/mmap.py
+-rw-r--r--   0 user      (1000) user      (1000)     1472 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/numpy.py
+-rw-r--r--   0 user      (1000) user      (1000)    26018 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/safetensors.py
+-rw-r--r--   0 user      (1000) user      (1000)     1159 2023-04-12 08:38:25.000000 pure_safetensors-0.3.0/src/pure_safetensors/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-12 08:38:33.558594 pure_safetensors-0.3.0/src/pure_safetensors.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     4165 2023-04-12 08:38:33.000000 pure_safetensors-0.3.0/src/pure_safetensors.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      583 2023-04-12 08:38:33.000000 pure_safetensors-0.3.0/src/pure_safetensors.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-12 08:38:33.000000 pure_safetensors-0.3.0/src/pure_safetensors.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       36 2023-04-12 08:38:33.000000 pure_safetensors-0.3.0/src/pure_safetensors.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-12 08:38:33.000000 pure_safetensors-0.3.0/src/pure_safetensors.egg-info/top_level.txt
```

### Comparing `pure_safetensors-0.2.0/PKG-INFO` & `pure_safetensors-0.3.0/src/pure_safetensors.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pure_safetensors
-Version: 0.2.0
+Name: pure-safetensors
+Version: 0.3.0
 Summary: Pure-Python safetensors
 Home-page: UNKNOWN
 Author: Eduard Christian Dumitrescu
 Author-email: eduard.c.dumitrescu@gmail.com
 License: MIT
 Description: # pure_safetensors
         
@@ -14,25 +14,27 @@
         
         We try to keep dependencies light:
         
         - [attrs](https://pypi.org/project/attrs/) dataclass library (2881 LoC)
         - [marshmallow](https://pypi.org/project/marshmallow/) serialization and validation library (2647 LoC)
         - [sortedcollections](https://pypi.org/project/sortedcollections/) tiny sorted collections library (339 LoC) built on top of [sortedcontainers](https://pypi.org/project/sortedcontainers/) (1493 LoC)
         - (optional) [sparsefile](https://pypi.org/project/sparsefile/) sparse file library (191 LoC)
+        - (optional) [fickle](https://pypi.org/project/fickle/) whitelist-based firewall for safe pickle loading, used for PyTorch model conversion (926 LoC)
         
         Optionally, this library integrates with NumPy (if available). PyTorch integration is planned, someday.
         
         To run the tests, you'll need `pytest`, `numpy`, and optionally `hypothesis`.
         
         # Examples
         
         ```python
         from pure_safetensors import SafeTensors
         
-        with SafeTensors("/path/to/example.safetensors", "r+") as sf, sf.as_numpy() as arrays:
+        with SafeTensors("/path/to/example.safetensors", "r+") as sf:
+            arrays = sf.as_numpy()
             arrays["hello"][3, :] += 420.69
             arrays["world"] = arrays["hello"][0:2] * 10
         
             # assign multiple arrays! much faster!
             arrays.update(
                 {
                     "q": my_array_1,
@@ -41,14 +43,20 @@
                 }
             )
         
             # delete arrays! such wonders!
             del arrays["v"]
         ```
         
+        Do you have an existing PyTorch checkpoint model that you would like to safetensors? Then try running:
+        
+        ```sh
+        python3 -m pure_safetensors import-pytorch /path/to/model.ckpt /path/to/model.safetensors
+        ```
+        
         # Bugs
         
         The space allocator is a greedy algorithm based on first-fit-decreasing bin packing. So if you add/remove tensors to an existing file, it may leave too much empty space behind.
         
         PyTorch support isn't implemented yet.
         
         # Alternatives
@@ -57,14 +65,15 @@
         - [Narsil/pure_torch.py](https://gist.github.com/Narsil/3edeec2669a5e94e4707aa0f901d2282)
         - [Narsil/safetensors.cpp](https://gist.github.com/Narsil/5d6bf307995158ad2c4994f323967284)
         
         |                                                 | pure_safetensors | safetensors | pure_torch.py | safetensors.cpp |
         |-------------------------------------------------|------------------|-------------|---------------|-----------------|
         | Written in pure Python?                         | ✅ | ❌ | ✅ | — |
         | Supports NumPy (without PyTorch)?               | ✅ | ✅ | ❌ | — |
+        | Supports PyTorch?                               | ❌ | ✅ | ✅ | — |
         | Can work without numpy or pytorch?              | ✅ | ✅ | ❌ | — |
         | Can write safetensors files?                    | ✅ | ✅ | ❌ | ❌ |
         | Can modify file in-place to add/remove tensors? | ✅ | ❌ | ❌ | ❌ |
         | Has test suite?                                 | ✅ | ✅ | ❌ | ❌ |
         | Stable API?                                     | 🤷 | ✅ | ❔ | ❔ |
         | Automatically makes files sparse to save space? | ✅ | ❌ | ❌ | ❌ |
         | Works on platforms without mmap?                | ✅ | ❌ | ❌ | ❌ |
```

### Comparing `pure_safetensors-0.2.0/README.md` & `pure_safetensors-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 
 We try to keep dependencies light:
 
 - [attrs](https://pypi.org/project/attrs/) dataclass library (2881 LoC)
 - [marshmallow](https://pypi.org/project/marshmallow/) serialization and validation library (2647 LoC)
 - [sortedcollections](https://pypi.org/project/sortedcollections/) tiny sorted collections library (339 LoC) built on top of [sortedcontainers](https://pypi.org/project/sortedcontainers/) (1493 LoC)
 - (optional) [sparsefile](https://pypi.org/project/sparsefile/) sparse file library (191 LoC)
+- (optional) [fickle](https://pypi.org/project/fickle/) whitelist-based firewall for safe pickle loading, used for PyTorch model conversion (926 LoC)
 
 Optionally, this library integrates with NumPy (if available). PyTorch integration is planned, someday.
 
 To run the tests, you'll need `pytest`, `numpy`, and optionally `hypothesis`.
 
 # Examples
 
 ```python
 from pure_safetensors import SafeTensors
 
-with SafeTensors("/path/to/example.safetensors", "r+") as sf, sf.as_numpy() as arrays:
+with SafeTensors("/path/to/example.safetensors", "r+") as sf:
+    arrays = sf.as_numpy()
     arrays["hello"][3, :] += 420.69
     arrays["world"] = arrays["hello"][0:2] * 10
 
     # assign multiple arrays! much faster!
     arrays.update(
         {
             "q": my_array_1,
@@ -33,14 +35,20 @@
         }
     )
 
     # delete arrays! such wonders!
     del arrays["v"]
 ```
 
+Do you have an existing PyTorch checkpoint model that you would like to safetensors? Then try running:
+
+```sh
+python3 -m pure_safetensors import-pytorch /path/to/model.ckpt /path/to/model.safetensors
+```
+
 # Bugs
 
 The space allocator is a greedy algorithm based on first-fit-decreasing bin packing. So if you add/remove tensors to an existing file, it may leave too much empty space behind.
 
 PyTorch support isn't implemented yet.
 
 # Alternatives
@@ -49,14 +57,15 @@
 - [Narsil/pure_torch.py](https://gist.github.com/Narsil/3edeec2669a5e94e4707aa0f901d2282)
 - [Narsil/safetensors.cpp](https://gist.github.com/Narsil/5d6bf307995158ad2c4994f323967284)
 
 |                                                 | pure_safetensors | safetensors | pure_torch.py | safetensors.cpp |
 |-------------------------------------------------|------------------|-------------|---------------|-----------------|
 | Written in pure Python?                         | ✅ | ❌ | ✅ | — |
 | Supports NumPy (without PyTorch)?               | ✅ | ✅ | ❌ | — |
+| Supports PyTorch?                               | ❌ | ✅ | ✅ | — |
 | Can work without numpy or pytorch?              | ✅ | ✅ | ❌ | — |
 | Can write safetensors files?                    | ✅ | ✅ | ❌ | ❌ |
 | Can modify file in-place to add/remove tensors? | ✅ | ❌ | ❌ | ❌ |
 | Has test suite?                                 | ✅ | ✅ | ❌ | ❌ |
 | Stable API?                                     | 🤷 | ✅ | ❔ | ❔ |
 | Automatically makes files sparse to save space? | ✅ | ❌ | ❌ | ❌ |
 | Works on platforms without mmap?                | ✅ | ❌ | ❌ | ❌ |
```

### Comparing `pure_safetensors-0.2.0/setup.py` & `pure_safetensors-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text("utf-8")
 
 setup(
     name="pure_safetensors",
     description="Pure-Python safetensors",
-    version="0.2.0",
+    version="0.3.0",
     author="Eduard Christian Dumitrescu",
     author_email="eduard.c.dumitrescu@gmail.com",
     install_requires=["attrs", "marshmallow", "sortedcollections"],
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     license="MIT",
     classifiers=[
```

### Comparing `pure_safetensors-0.2.0/src/pure_safetensors/numpy.py` & `pure_safetensors-0.3.0/src/pure_safetensors/numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Tuple
 
 import attr
 import numpy
 
 from .safetensors import dtypes, DType, SafeTensorInfo
-from .mmap import BaseAdapter, _Buffer
+from .adapter import BaseAdapter, _Buffer
 
 
 @attr.s(eq=False)
 class NumpyAdapter(BaseAdapter):
     bfloat16_as_uint16: bool = attr.ib(default=False)
 
-    numpy_dtypes_map = {dt.numpy_name: dt for dt in dtypes.values()}
+    NUMPY_DTYPES_MAP = {dt.numpy_name: dt for dt in dtypes.values()}
 
     def map_tensor_dtype_to_numpy(self, dtype: DType):
         dtype_name = dtype.numpy_name
 
         if dtype_name == "bfloat16" and self.bfloat16_as_uint16:
             dtype_name = "u2"
 
@@ -24,29 +24,25 @@
     def _user_data_to_safetensor_info(self, array):
         if type(array) is tuple:
             array, dtype = array
         else:
             dtype = None
 
         if dtype is None:
-            dtype = self.numpy_dtypes_map[array.dtype.name]
+            dtype = self.NUMPY_DTYPES_MAP[array.dtype.name]
 
         return SafeTensorInfo(dtype=dtype, start=0, end=0, shape=array.shape)
 
     def _copy_user_data_into_existing_tensor(self, data: object, key: str):
         self[key][...] = data
 
-    def memory_buffer_as_numpy_array(
+    def _memory_buffer_as_numpy_array(
         self, tensor: SafeTensorInfo, buffer: _Buffer
     ) -> Tuple[numpy.ndarray]:
         dtype = self.map_tensor_dtype_to_numpy(tensor.dtype)
         shape = tensor.shape
 
-        cls = numpy.ndarray
-        array = cls.__new__(cls, shape=shape, dtype=dtype, buffer=buffer, order="C")
-
-        return array.reshape(shape)
+        return numpy.frombuffer(buffer, dtype=dtype).reshape(shape)
 
     def __getitem__(self, key):
-        tensor = self.s.tensors[key]
-        mmapping = self.get_memory_mapping_for_tensor(key)
-        return self.memory_buffer_as_numpy_array(tensor, mmapping.buffer)
+        tensor, mem_mapping = self.s.get_memory_mapping_for_tensor(key)
+        return self._memory_buffer_as_numpy_array(tensor, mem_mapping.buffer)
```

### Comparing `pure_safetensors-0.2.0/src/pure_safetensors/safetensors.py` & `pure_safetensors-0.3.0/src/pure_safetensors/safetensors.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,34 @@
 
 import attr
 import marshmallow
 from marshmallow import fields
 import sortedcollections
 import warnings
 
+from .mmap import (
+    FakeMemoryMappingFactory,
+    MemoryMapping,
+    MemoryMappingFactory,
+    RealMemoryMappingFactory,
+    mmap,
+)
 from .exc import SafeTensorError, SafeTensorHeaderError, SafeTensorEmptyFileError
 from .util import align, samefile_copy
 
 try:
     import sparsefile
 except ImportError:
     sparsefile = None
 
 
+# you can use this global variable to control whether the OS mmap is used
+use_mmap = mmap is not None
+
+
 @attr.s(eq=False)
 class SafeTensors:
     """
     This object is not thread-safe, and safetensor file structure should not be
     modified by different threads or processes at the same time.
 
     Resizing the file may result in a crash:
@@ -47,18 +58,22 @@
 
     _valid_modes = frozenset(("r", "r+", "x+", "w+", "c"))
 
     file: IO = attr.ib()
     mode: str = attr.ib()
     sparse: bool = attr.ib(default=None)
     settings: "Settings" = attr.ib(factory=lambda: Settings(), kw_only=True)
+    use_mmap: bool = attr.ib(factory=lambda: use_mmap)
 
-    map: "FileMap"
+    mappings: Dict[str, MemoryMapping] = attr.ib(init=False, factory=dict)
 
+    map: "FileMap"
     tensors: "Dict[str, SafeTensorInfo]"
+    _memory_mapping_factory: MemoryMappingFactory
+
     _close_on_exit: bool = False
 
     def _open_file(self):
         self.file = open(self.file, self.mode.replace("c", "r") + "b")
 
     def __attrs_post_init__(self):
         if not hasattr(self.file, "read"):
@@ -66,30 +81,36 @@
             self._open_file()
             self._close_on_exit = True
 
         # replace "x+" with "w+" since they are equivalent after the file is created
         if self.mode == "x+":
             self.mode = "w+"
 
+        self._init_memory_mapping_factory()
+
         # load file or write empty header if creating new file
         self._initialize_structure()
 
+    def _init_memory_mapping_factory(self):
+        cls = RealMemoryMappingFactory if self.use_mmap else FakeMemoryMappingFactory
+        self._memory_mapping_factory = cls(file=self.file, mode=self.mode)
+
     @mode.validator
     def check(self, attribute, value):
         if value not in self._valid_modes:
             raise ValueError(f"{value!r} not in {self._valid_modes!r}")
 
-    @property
-    def readonly(self):
-        return "+" not in self.mode
-
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
+        self.close()
+
+    def close(self):
+        self.flush(free=True)
         if self._close_on_exit:
             self.file.close()
 
     def _initialize_structure(self):
         if self.mode != "w+":
             try:
                 self._read_header()
@@ -137,15 +158,15 @@
         """
         return self.map.metadata
 
     @metadata.setter
     def metadata(self, metadata):
         new_map = self.map.copy()
         new_map.metadata = metadata
-        new_map.allocate_tensors()
+        new_map.modify()  # move tensors if necessary
         self._write_header(new_map)
 
     @property
     def tensors(self):
         """
         Do not mutate this property! Make a copy and then assign to this property.
         """
@@ -163,15 +184,15 @@
                 del st_numpy["my_tensor_name"]
         """
         from .numpy import NumpyAdapter
 
         return NumpyAdapter(self, **kw)
 
     def as_buffer(self, **kw):
-        from .mmap import BufferAdapter
+        from .adapter import BufferAdapter
 
         return BufferAdapter(self, **kw)
 
     def create_or_replace_or_delete_tensors(
         self, tensors: "Dict[str, Optional[SafeTensorInfo]]"
     ) -> None:
         """
@@ -233,14 +254,45 @@
                 # opportunistic
                 if not sparsefile.maybe_sparse(self.file, start, length):
                     # failed to make it sparse, give up
                     break
             else:
                 sparsefile.ensure_sparse(self.file, start, length)
 
+    def _open_memory_mapping(self, offset: int, length: int) -> MemoryMapping:
+        return self._memory_mapping_factory.map(offset=offset, length=length)
+
+    def get_memory_mapping_for_tensor(
+        self, key: str
+    ) -> "Tuple[SafeTensorInfo, MemoryMapping]":
+        """
+        Map the tensor given by ``key`` in memory.
+        """
+        tensor = self.tensors[key]
+        mapping = self.mappings.get(key, None)
+        if mapping is None:
+            self.mappings[key] = mapping = self._open_memory_mapping(
+                offset=tensor.start, length=tensor.end - tensor.start
+            )
+        return (tensor, mapping)
+
+    def flush(self, keys=None, free: bool = False) -> None:
+        """
+        Ensure that tensor data is written to disk. If ``free == True``, then
+        remove the memory mapping from the cached memory mappings.
+        """
+        mappings = self.mappings
+        keys = tuple(mappings.keys()) if keys is None else keys
+        for key in keys:
+            mapping = mappings.get(key, None)
+            if mapping is not None:
+                mapping.flush()
+                if free:
+                    mappings.pop(key, None)
+
 
 @attr.s
 class DType:
     name: str = attr.ib()
     kind: str = attr.ib()
     size_in_bytes: int = attr.ib()
     numpy_name: str = attr.ib()
```

### Comparing `pure_safetensors-0.2.0/src/pure_safetensors/util.py` & `pure_safetensors-0.3.0/src/pure_safetensors/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,9 +35,10 @@
             f.seek(src)
             data = f.read(to_read).ljust(to_read, b"\0")
             f.seek(dst)
             f.write(data)
             src += to_read
             dst += to_read
 
+
 def get_file_size(file: IO) -> int:
     return os.fstat(file.fileno()).st_size
```

### Comparing `pure_safetensors-0.2.0/src/pure_safetensors.egg-info/PKG-INFO` & `pure_safetensors-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pure-safetensors
-Version: 0.2.0
+Name: pure_safetensors
+Version: 0.3.0
 Summary: Pure-Python safetensors
 Home-page: UNKNOWN
 Author: Eduard Christian Dumitrescu
 Author-email: eduard.c.dumitrescu@gmail.com
 License: MIT
 Description: # pure_safetensors
         
@@ -14,25 +14,27 @@
         
         We try to keep dependencies light:
         
         - [attrs](https://pypi.org/project/attrs/) dataclass library (2881 LoC)
         - [marshmallow](https://pypi.org/project/marshmallow/) serialization and validation library (2647 LoC)
         - [sortedcollections](https://pypi.org/project/sortedcollections/) tiny sorted collections library (339 LoC) built on top of [sortedcontainers](https://pypi.org/project/sortedcontainers/) (1493 LoC)
         - (optional) [sparsefile](https://pypi.org/project/sparsefile/) sparse file library (191 LoC)
+        - (optional) [fickle](https://pypi.org/project/fickle/) whitelist-based firewall for safe pickle loading, used for PyTorch model conversion (926 LoC)
         
         Optionally, this library integrates with NumPy (if available). PyTorch integration is planned, someday.
         
         To run the tests, you'll need `pytest`, `numpy`, and optionally `hypothesis`.
         
         # Examples
         
         ```python
         from pure_safetensors import SafeTensors
         
-        with SafeTensors("/path/to/example.safetensors", "r+") as sf, sf.as_numpy() as arrays:
+        with SafeTensors("/path/to/example.safetensors", "r+") as sf:
+            arrays = sf.as_numpy()
             arrays["hello"][3, :] += 420.69
             arrays["world"] = arrays["hello"][0:2] * 10
         
             # assign multiple arrays! much faster!
             arrays.update(
                 {
                     "q": my_array_1,
@@ -41,14 +43,20 @@
                 }
             )
         
             # delete arrays! such wonders!
             del arrays["v"]
         ```
         
+        Do you have an existing PyTorch checkpoint model that you would like to safetensors? Then try running:
+        
+        ```sh
+        python3 -m pure_safetensors import-pytorch /path/to/model.ckpt /path/to/model.safetensors
+        ```
+        
         # Bugs
         
         The space allocator is a greedy algorithm based on first-fit-decreasing bin packing. So if you add/remove tensors to an existing file, it may leave too much empty space behind.
         
         PyTorch support isn't implemented yet.
         
         # Alternatives
@@ -57,14 +65,15 @@
         - [Narsil/pure_torch.py](https://gist.github.com/Narsil/3edeec2669a5e94e4707aa0f901d2282)
         - [Narsil/safetensors.cpp](https://gist.github.com/Narsil/5d6bf307995158ad2c4994f323967284)
         
         |                                                 | pure_safetensors | safetensors | pure_torch.py | safetensors.cpp |
         |-------------------------------------------------|------------------|-------------|---------------|-----------------|
         | Written in pure Python?                         | ✅ | ❌ | ✅ | — |
         | Supports NumPy (without PyTorch)?               | ✅ | ✅ | ❌ | — |
+        | Supports PyTorch?                               | ❌ | ✅ | ✅ | — |
         | Can work without numpy or pytorch?              | ✅ | ✅ | ❌ | — |
         | Can write safetensors files?                    | ✅ | ✅ | ❌ | ❌ |
         | Can modify file in-place to add/remove tensors? | ✅ | ❌ | ❌ | ❌ |
         | Has test suite?                                 | ✅ | ✅ | ❌ | ❌ |
         | Stable API?                                     | 🤷 | ✅ | ❔ | ❔ |
         | Automatically makes files sparse to save space? | ✅ | ❌ | ❌ | ❌ |
         | Works on platforms without mmap?                | ✅ | ❌ | ❌ | ❌ |
```

