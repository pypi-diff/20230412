# Comparing `tmp/pytorch-symbolic-1.0.5.tar.gz` & `tmp/pytorch-symbolic-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-symbolic-1.0.5.tar", last modified: Sat Dec 10 16:28:24 2022, max compression
+gzip compressed data, was "pytorch-symbolic-1.0.6.tar", last modified: Wed Apr 12 21:54:20 2023, max compression
```

## Comparing `pytorch-symbolic-1.0.5.tar` & `pytorch-symbolic-1.0.6.tar`

### file list

```diff
@@ -1,24 +1,38 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2022-12-10 16:28:24.208041 pytorch-symbolic-1.0.5/
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1052 2022-10-01 23:42:11.000000 pytorch-symbolic-1.0.5/LICENSE.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)     5071 2022-12-10 16:28:24.208041 pytorch-symbolic-1.0.5/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1001)     4240 2022-12-10 16:27:38.000000 pytorch-symbolic-1.0.5/README.md
--rw-r--r--   0 gaha      (1000) gaha      (1001)      188 2022-11-17 10:14:15.000000 pytorch-symbolic-1.0.5/pyproject.toml
-drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2022-12-10 16:28:24.208041 pytorch-symbolic-1.0.5/pytorch_symbolic/
--rw-r--r--   0 gaha      (1000) gaha      (1001)      580 2022-12-10 16:27:22.000000 pytorch-symbolic-1.0.5/pytorch_symbolic/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     4936 2022-11-17 10:14:15.000000 pytorch-symbolic-1.0.5/pytorch_symbolic/code_generator.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)      623 2022-11-17 10:14:15.000000 pytorch-symbolic-1.0.5/pytorch_symbolic/config.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     3727 2022-11-17 10:14:15.000000 pytorch-symbolic-1.0.5/pytorch_symbolic/functions_utility.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)    12693 2022-12-10 16:27:22.000000 pytorch-symbolic-1.0.5/pytorch_symbolic/graph_algorithms.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1610 2022-11-17 10:14:15.000000 pytorch-symbolic-1.0.5/pytorch_symbolic/model_tools.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     2071 2022-11-17 10:14:15.000000 pytorch-symbolic-1.0.5/pytorch_symbolic/symbolic_api_2.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)    19205 2022-11-17 10:14:15.000000 pytorch-symbolic-1.0.5/pytorch_symbolic/symbolic_data.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)    14245 2022-11-17 10:14:15.000000 pytorch-symbolic-1.0.5/pytorch_symbolic/symbolic_model.py
--rw-r--r--   0 gaha      (1000) gaha      (1001)     3900 2022-11-17 10:14:15.000000 pytorch-symbolic-1.0.5/pytorch_symbolic/useful_layers.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2022-12-10 16:28:24.208041 pytorch-symbolic-1.0.5/pytorch_symbolic.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1001)     5071 2022-12-10 16:28:24.000000 pytorch-symbolic-1.0.5/pytorch_symbolic.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1001)      590 2022-12-10 16:28:24.000000 pytorch-symbolic-1.0.5/pytorch_symbolic.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)        1 2022-12-10 16:28:24.000000 pytorch-symbolic-1.0.5/pytorch_symbolic.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)       48 2022-12-10 16:28:24.000000 pytorch-symbolic-1.0.5/pytorch_symbolic.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)       17 2022-12-10 16:28:24.000000 pytorch-symbolic-1.0.5/pytorch_symbolic.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1001)      105 2022-12-10 16:28:24.211375 pytorch-symbolic-1.0.5/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1001)     1261 2022-12-10 16:27:58.000000 pytorch-symbolic-1.0.5/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2023-04-12 21:54:20.691811 pytorch-symbolic-1.0.6/
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1052 2022-10-01 23:42:11.000000 pytorch-symbolic-1.0.6/LICENSE.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     5071 2023-04-12 21:54:20.691811 pytorch-symbolic-1.0.6/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     4240 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/README.md
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      188 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pyproject.toml
+drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2023-04-12 21:54:20.691811 pytorch-symbolic-1.0.6/pytorch_symbolic/
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      580 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     4936 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/code_generator.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      623 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/config.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     3784 2023-04-12 21:11:23.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/functions_utility.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)    12693 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/graph_algorithms.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1610 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/model_tools.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     2146 2023-04-12 21:33:14.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/symbolic_api_2.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)    19582 2023-04-12 21:31:41.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/symbolic_data.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)    14316 2023-04-12 21:34:01.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/symbolic_model.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     3900 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/pytorch_symbolic/useful_layers.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2023-04-12 21:54:20.691811 pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     5071 2023-04-12 21:54:20.000000 pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      993 2023-04-12 21:54:20.000000 pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)        1 2023-04-12 21:54:20.000000 pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)       48 2023-04-12 21:54:20.000000 pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)       17 2023-04-12 21:54:20.000000 pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1001)      105 2023-04-12 21:54:20.691811 pytorch-symbolic-1.0.6/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1261 2023-04-12 21:43:05.000000 pytorch-symbolic-1.0.6/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1001)        0 2023-04-12 21:54:20.691811 pytorch-symbolic-1.0.6/tests/
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     4239 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_add_to_graph.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     8117 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_basic_ops.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     2230 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_creating_examples.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     2269 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_creating_examples_detached.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1751 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_creating_extreme.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     5305 2023-04-12 21:46:38.000000 pytorch-symbolic-1.0.6/tests/test_creating_models.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     3255 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_creating_multi_in_out.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1759 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_docs_automated.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     2887 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_docs_manual.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1365 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_iterating_and_slicing.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1499 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_nontorch_graphs.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     1016 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_raising_assertions.py
+-rw-r--r--   0 gaha      (1000) gaha      (1001)     2428 2022-12-12 10:31:26.000000 pytorch-symbolic-1.0.6/tests/test_reusing_nodes.py
```

### Comparing `pytorch-symbolic-1.0.5/LICENSE.txt` & `pytorch-symbolic-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.5/PKG-INFO` & `pytorch-symbolic-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-symbolic
-Version: 1.0.5
+Version: 1.0.6
 Summary: Provides symbolic API for model creation in PyTorch.
 Home-page: https://github.com/gahaalt/pytorch-symbolic.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Project-URL: Documentation, https://pytorch-symbolic.readthedocs.io/
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytorch-symbolic-1.0.5/README.md` & `pytorch-symbolic-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.5/pytorch_symbolic/__init__.py` & `pytorch-symbolic-1.0.6/pytorch_symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.5/pytorch_symbolic/code_generator.py` & `pytorch-symbolic-1.0.6/pytorch_symbolic/code_generator.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.5/pytorch_symbolic/config.py` & `pytorch-symbolic-1.0.6/pytorch_symbolic/config.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.5/pytorch_symbolic/functions_utility.py` & `pytorch-symbolic-1.0.6/pytorch_symbolic/functions_utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             navigation[-1].append(k)
             new_dict[k] = _replace_symbolic_with_value(v, extracted, navigation)
             navigation[-1].pop()
         return new_dict
     return container
 
 
-def add_to_graph(func: Callable | nn.Module, *args, **kwds):
+def add_to_graph(func: Callable | nn.Module, *args, custom_name: str | None = None, **kwds):
     """Register a custom func or a module in the computation graph.
 
     This works will arbitrary functions and modules iff at least one Symbolic Data is among ``*args, **kwds``.
 
     This way of registering is flexible, but might add a small slowdown to the call,
     because it adds a wrapper for parsing arguments.
     If this is unacceptable, please create an torch.nn.Module that takes only Symbolic Data arguments.
@@ -89,8 +89,8 @@
         name = func.__name__
     elif hasattr(func, "__class__"):
         name = func.__class__.__name__
     else:
         name = str(func)
     module = useful_layers.NamedLambdaOpLayer(op=wrapper_function, name=f"wrap({name})")
     # This might be a Symbolic Callable, so we use `apply_module` instead of `__call__`
-    return extracted_symbols[0].apply_module(module, *extracted_symbols[1:])
+    return extracted_symbols[0].apply_module(module, *extracted_symbols[1:], custom_name=custom_name)
```

### Comparing `pytorch-symbolic-1.0.5/pytorch_symbolic/graph_algorithms.py` & `pytorch-symbolic-1.0.6/pytorch_symbolic/graph_algorithms.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.5/pytorch_symbolic/model_tools.py` & `pytorch-symbolic-1.0.6/pytorch_symbolic/model_tools.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.5/pytorch_symbolic/symbolic_api_2.py` & `pytorch-symbolic-1.0.6/pytorch_symbolic/symbolic_api_2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 #  Copyright (c) 2022 Szymon Mikler
 
 """
 Enables Symbolic API 2, which allows for registering layers by calling
 layer(*symbolic) instead of symbolic_1(layer, *other_symbolic).
 """
 
+from __future__ import annotations
+
 import logging
 
 from torch import nn
 
 from .symbolic_data import SymbolicData
 
 __nn_module_old_new__ = nn.Module.__new__
 __nn_module_old_call__ = nn.Module.__call__
 
 
-def call_wrapper_for_api_2(self, *args, **kwds):
+def call_wrapper_for_api_2(self, *args, custom_name: str | None = None, **kwds):
     if not any(isinstance(x, SymbolicData) for x in args):
         return __nn_module_old_call__(self, *args, **kwds)
     elif len(kwds) == 0 and all(isinstance(x, SymbolicData) for x in args):
         node = args[0]
-        return node(self, *args[1:])
+        return node(self, *args[1:], custom_name=custom_name)
     else:
         msg = (
-            "Only unnamed SymbolicData are allowed as arguments! "
-            "If you need more flexibility, use `functions_utility.add_to_graph`!"
+            "Only *args are allowed as arguments! "
+            "If you need to use **kwds, try `functions_utility.add_to_graph`!"
         )
         raise UserWarning(msg)
 
 
 class SymbolicAPI2ContextManager:
     def __enter__(self):
         logging.debug("Symbolic API has been enabled!")
```

### Comparing `pytorch-symbolic-1.0.5/pytorch_symbolic/symbolic_data.py` & `pytorch-symbolic-1.0.6/pytorch_symbolic/symbolic_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     def __init__(
         self,
         value: Any,
         parents: Tuple[SymbolicData, ...] = (),
         depth: int = 0,
         layer: nn.Module | None = None,
         batch_size_known: bool = False,
+        custom_name: str | None = None,
     ):
         """Grandfather of all Symbolic datatypes.
 
         Underlying data is a normal Python object, for example a ``dict``.
         You can use methods and operators of the underlying object.
         You can also unpack or index it, if only the underlying data allows it.
 
@@ -34,36 +35,41 @@
         Parameters
         ----------
         value
         parents
         depth
         layer
         batch_size_known
+        custom_name
 
         Attributes
         ----------
         v : Any
             Underlying data that is used during model tracing
         layer : nn.Module
             A torch.nn.Module that transforms parents' values into this value. Also it's the incoming edge.
         depth : int
             Maximum of parents' depths plus one
         batch_size_known : bool
             In case of Input, whether batch size was provided by the user.
             For non-Input nodes, batch size is known iff all parents' batch sizes are known.
+        custom_name : str
+            Instead of using the default name for the undelying layer, user can provide his own.
         """
         global _SYMBOLIC_DATA_COUNTER
         self._execution_order_idx = _SYMBOLIC_DATA_COUNTER
         _SYMBOLIC_DATA_COUNTER += 1
 
         # We use Symbolic Data for inheriting only
         assert self.__class__ is not SymbolicData, "Symbolic Data should not be created directly!"
 
         self._value = value
         self._underlying_type_name = type(value).__name__
+        self._custom_provided_name = custom_name
+
         self.layer = layer
         self.depth = depth
         self.batch_size_known = batch_size_known
 
         self._children: List[SymbolicData] = []
         self._parents: Tuple[SymbolicData, ...] = parents
         self._layer_full_siblings: Tuple[SymbolicData, ...] = (self,)
@@ -126,15 +132,18 @@
 
     @property
     def children(self) -> Tuple[SymbolicData, ...]:
         """Acces the tuple of children of this node."""
         return tuple(self._children)
 
     def apply_module(
-        self, layer: nn.Module, *others: SymbolicData
+        self,
+        layer: nn.Module,
+        *others: SymbolicData,
+        custom_name: str | None = None,
     ) -> SymbolicData | Tuple[SymbolicData, ...]:
         """Register a new layer in the graph. Layer must be nn.Module."""
         assert all([isinstance(other, SymbolicData) for other in others]), "Works with SymbolicData only!"
 
         parents = (self, *others)
         new_depth = max(parent.depth for parent in parents) + 1
         with torch.no_grad():
@@ -144,14 +153,15 @@
 
         new_layer_node = cls(
             value=new_value,
             parents=parents,
             layer=layer,
             depth=new_depth,
             batch_size_known=self.batch_size_known,
+            custom_name=custom_name,
         )
         for parent in parents:
             parent._children.append(new_layer_node)
             logging.debug(f"Added {new_layer_node} as child of {parent}")
         return new_layer_node
 
     def _recalculate_value(self):
@@ -246,16 +256,16 @@
         if isinstance(idx, SymbolicData):
             layer = useful_layers.SliceLayerSymbolicIdx()
             return layer(self, idx)
         else:
             layer = useful_layers.SliceLayer(idx)
             return layer(self)
 
-    def __call__(self, *args):
-        return self.apply_module(*args)
+    def __call__(self, *args, custom_name: str | None = None):
+        return self.apply_module(*args, custom_name=custom_name)
 
     def __repr__(self):
         addr = f"{self.__class__.__name__} at {hex(id(self))};"
         info = f"{len(self._parents)} parents; {len(self._children)} children"
         return "<" + addr + " " + info + ">"
 
     def __hash__(self):
@@ -534,17 +544,15 @@
         batch_size_known = False
 
     value = torch.rand(batch_size, *shape) * (max_value - min_value) + min_value
     value = value.to(dtype)
     return SymbolicTensor(value=value, batch_size_known=batch_size_known)
 
 
-def CustomInput(
-    data: Any,
-) -> SymbolicData:
+def CustomInput(data: Any) -> SymbolicData:
     """Input to Symbolic Model. Creates Symbolic Data as a root node in the graph.
 
     This should be used when Input won't work.
 
     Parameters
     ----------
     data
```

### Comparing `pytorch-symbolic-1.0.5/pytorch_symbolic/symbolic_model.py` & `pytorch-symbolic-1.0.6/pytorch_symbolic/symbolic_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,14 @@
             outputs = (outputs,)
         assert all(isinstance(x, SymbolicData) for x in outputs), "Only SymbolicData allowed in outputs!"
         self.outputs: Tuple[SymbolicData, ...] = tuple(outputs)
 
         # Initialize helper variables
         self._layer_type_counts: Dict[str, int] = {}
         self._node_to_layer_name: Dict[SymbolicData, str] = {}
-        self._layer_name_to_node: Dict[str, SymbolicData] = {}
         self._execution_order_nodes: List[SymbolicData] = []
         self._execution_order_layers: List[nn.Module] = []
         self._figure_out_execution_order()
 
         if enable_forward_codegen is None:
             enable_forward_codegen = config.CODEGEN_BY_DEFAULT
         self._enable_forward_codegen = enable_forward_codegen
@@ -323,15 +322,19 @@
         # We remove all nodes with already executed layer from execution order
         execution_order_nodes = self._remove_repeated_execution(execution_order_nodes)
 
         self._execution_order_nodes = execution_order_nodes
         self._execution_order_layers = [node.layer for node in self._execution_order_nodes]
 
         for idx, node in enumerate(self._execution_order_nodes):
-            layer_name = node.layer._get_name()
+            if node._custom_provided_name is not None:
+                layer_name = node._custom_provided_name
+            else:
+                layer_name = node.layer._get_name()
+
             self._layer_type_counts.setdefault(layer_name, 0)
             self._layer_type_counts[layer_name] += 1
             full_layer_name = f"{layer_name}_{self._layer_type_counts[layer_name]}"
             self._node_to_layer_name[node] = full_layer_name
             self.add_module(name=full_layer_name, module=node.layer)
 
     def __deepcopy__(self, memo):
```

### Comparing `pytorch-symbolic-1.0.5/pytorch_symbolic/useful_layers.py` & `pytorch-symbolic-1.0.6/pytorch_symbolic/useful_layers.py`

 * *Files identical despite different names*

### Comparing `pytorch-symbolic-1.0.5/pytorch_symbolic.egg-info/PKG-INFO` & `pytorch-symbolic-1.0.6/pytorch_symbolic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-symbolic
-Version: 1.0.5
+Version: 1.0.6
 Summary: Provides symbolic API for model creation in PyTorch.
 Home-page: https://github.com/gahaalt/pytorch-symbolic.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Project-URL: Documentation, https://pytorch-symbolic.readthedocs.io/
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytorch-symbolic-1.0.5/setup.py` & `pytorch-symbolic-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="UTF-8")
 
 setup(
     name="pytorch-symbolic",
-    version="1.0.5",
+    version="1.0.6",
     url="https://github.com/gahaalt/pytorch-symbolic.git",
     project_urls={
         "Documentation": "https://pytorch-symbolic.readthedocs.io/",
     },
     author="Szymon Mikler",
     author_email="sjmikler@gmail.com",
     license="MIT",
```

