# Comparing `tmp/offlinerllib-0.0.5.tar.gz` & `tmp/offlinerllib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offlinerllib-0.0.5.tar", last modified: Fri Mar 17 07:01:55 2023, max compression
+gzip compressed data, was "offlinerllib-0.0.6.tar", last modified: Wed Apr 12 12:38:51 2023, max compression
```

## Comparing `offlinerllib-0.0.5.tar` & `offlinerllib-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:01:55.381367 offlinerllib-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-17 07:01:55.381367 offlinerllib-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:01:55.377367 offlinerllib-0.0.5/offlinerllib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:01:55.377367 offlinerllib-0.0.5/offlinerllib/buffer/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/buffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/buffer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/buffer/d4rl_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:01:55.377367 offlinerllib-0.0.5/offlinerllib/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31219 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/module/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/module/critic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:01:55.381367 offlinerllib-0.0.5/offlinerllib/module/net/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/module/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/module/net/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/module/net/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/module/net/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:01:55.381367 offlinerllib-0.0.5/offlinerllib/policy/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:01:55.381367 offlinerllib-0.0.5/offlinerllib/policy/model_free/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/model_free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/model_free/awac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/model_free/bppo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/model_free/dt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/model_free/edac.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/model_free/inac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/model_free/iql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/model_free/sac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/model_free/sacn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/model_free/td3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/model_free/td3bc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/offlinerllib/policy/model_free/xql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:01:55.377367 offlinerllib-0.0.5/offlinerllib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-17 07:01:55.000000 offlinerllib-0.0.5/offlinerllib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-17 07:01:55.000000 offlinerllib-0.0.5/offlinerllib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 07:01:55.000000 offlinerllib-0.0.5/offlinerllib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-17 07:01:55.000000 offlinerllib-0.0.5/offlinerllib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-17 07:01:55.000000 offlinerllib-0.0.5/offlinerllib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 07:01:55.381367 offlinerllib-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-17 07:01:46.000000 offlinerllib-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.941846 offlinerllib-0.0.6/offlinerllib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.941846 offlinerllib-0.0.6/offlinerllib/buffer/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/buffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/buffer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/buffer/d4rl_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/offlinerllib/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31219 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/module/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/module/critic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/offlinerllib/module/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/module/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/module/net/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/module/net/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/offlinerllib/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/offlinerllib/policy/model_free/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/awac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/bppo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/edac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/inac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/iql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/sacn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/td3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/td3bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/offlinerllib/policy/model_free/xql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:38:51.941846 offlinerllib-0.0.6/offlinerllib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 12:38:51.000000 offlinerllib-0.0.6/offlinerllib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-12 12:38:51.000000 offlinerllib-0.0.6/offlinerllib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:38:51.000000 offlinerllib-0.0.6/offlinerllib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 12:38:51.000000 offlinerllib-0.0.6/offlinerllib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 12:38:51.000000 offlinerllib-0.0.6/offlinerllib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:38:51.945846 offlinerllib-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-12 12:38:44.000000 offlinerllib-0.0.6/setup.py
```

### Comparing `offlinerllib-0.0.5/LICENSE` & `offlinerllib-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.5/PKG-INFO` & `offlinerllib-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offlinerllib
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python module desgined for Offline RL algorithms developing and benchmarking. 
 Home-page: https://github.com/typoverflow/OfflineRLLib
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `offlinerllib-0.0.5/README.md` & `offlinerllib-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.5/offlinerllib/buffer/d4rl_buffer.py` & `offlinerllib-0.0.6/offlinerllib/buffer/d4rl_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         return arr
 
     npad = [(0, 0)] * arr.ndim
     npad[axis] = (0, pad_size)
     return np.pad(arr, pad_width=npad, mode="constant", constant_values=fill_value)
 
 
-class D4RLTransitionBuffer(Buffer, IterableDataset, Dataset):
+class D4RLTransitionBuffer(Buffer, IterableDataset):
     def __init__(self, dataset):
         self.observations = dataset["observations"].astype(np.float32)
         self.actions = dataset["actions"].astype(np.float32)
         self.rewards = dataset["rewards"][:, None].astype(np.float32)
         self.terminals = dataset["terminals"][:, None].astype(np.float32)
         self.next_observations = dataset["next_observations"].astype(np.float32)
         self.size = len(dataset["observations"])
```

### Comparing `offlinerllib-0.0.5/offlinerllib/module/actor.py` & `offlinerllib-0.0.6/offlinerllib/module/actor.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.5/offlinerllib/module/critic.py` & `offlinerllib-0.0.6/offlinerllib/module/critic.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     reduce :  A unary function which specifies how to aggregate the output values. Default is torch.min along the 0 dimension. 
     device :  The device which the model runs on. Default is cpu. 
     ***(any args of MLP)
     """
     _reduce_fn_ = {
         "min": lambda x: torch.min(x, dim=0)[0],
         "max": lambda x: torch.max(x, dim=0)[0], 
-        "mean": lambda x: torch.mean(x, dim=0)[0]
+        "mean": lambda x: torch.mean(x, dim=0)
     }
     def __init__(
         self, 
         backend: nn.Module, 
         input_dim: int, 
         output_dim: int=1, 
         critic_num: int=2,
```

### Comparing `offlinerllib-0.0.5/offlinerllib/module/net/basic.py` & `offlinerllib-0.0.6/offlinerllib/module/net/basic.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,17 +69,18 @@
         dtype: Optional[Any] = None
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         super().__init__()
         self.in_features = in_features
         self.out_features = out_features
         self.ensemble_size = ensemble_size
+        self.add_bias = bias
         self.register_parameter("weight", torch.nn.Parameter(torch.empty([ensemble_size, in_features, out_features], **factory_kwargs)))
         if bias:
-            self.register_parameter("bias", torch.nn.Parameter(torch.empty([ensemble_size, 1, out_features], **factory_kwargs)))
+            self.register_parameter("bias", torch.nn.Parameter(torch.empty([ensemble_size, out_features], **factory_kwargs)))
         else:
             self.register_parameter("bias", None)
         self.reset_parameters()
         
     def reset_parameters(self):
         for i in range(self.ensemble_size):
             torch.nn.init.kaiming_uniform_(self.weight[i], a=math.sqrt(5))
@@ -91,17 +92,30 @@
         
     def forward(self, input: torch.Tensor):
         if self.bias is None:
             bias = 0
         else:
             bias = self.bias
         if input.shape[0] != self.ensemble_size:
-            return torch.einsum('ij,bjk->bik', input, self.weight) + bias
+            res = torch.einsum('...j,bjk->b...k', input, self.weight)
+            if self.add_bias:
+                broadcast_length = len(input.shape)-1
+                return res + bias.reshape([self.ensemble_size]+[1]*broadcast_length+[self.out_features])
+            else:
+                return res
         else:
-            return torch.einsum('bij,bjk->bik', input, self.weight) + bias
+            res = torch.einsum('b...j,bjk->b...k', input, self.weight)
+            if self.add_bias:
+                broadcast_length = len(input.shape)-2
+                return res + bias.reshape([self.ensemble_size]+[1]*broadcast_length+[self.out_features])
+            else:
+                return res
+    
+    def __repr__(self):
+        return f"EnsembleLinear(in_features={self.in_features}, out_features={self.out_features}, bias={self.add_bias})"
 
 
 class NoisyLinear(nn.Linear):
     """
     An linear module which supports for noisy parameters.
     
     Parameters
```

### Comparing `offlinerllib-0.0.5/offlinerllib/module/net/mlp.py` & `offlinerllib-0.0.6/offlinerllib/module/net/mlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 activation_list = activation
             else:
                 activation_list = [activation for _ in range(len(hidden_dims))]
         else:
             activation_list = [None]*len(hidden_dims)
         
         if dropout:
-            if isinstance(dropout. list):
+            if isinstance(dropout, list):
                 assert len(dropout) == len(hidden_dims)
                 dropout_list = dropout
             else:
                 dropout_list = [dropout for _ in range(len(hidden_dims))]
         else:
             dropout_list = [None]*len(hidden_dims)
                         
@@ -143,15 +143,15 @@
                 activation_list = activation
             else:
                 activation_list = [activation for _ in range(len(hidden_dims))]
         else:
             activation_list = [None]*len(hidden_dims)
             
         if dropout:
-            if isinstance(dropout. list):
+            if isinstance(dropout, list):
                 assert len(dropout) == len(hidden_dims)
                 dropout_list = dropout
             else:
                 dropout_list = [dropout for _ in range(len(hidden_dims))]
         else:
             dropout_list = [None]*len(hidden_dims)
```

### Comparing `offlinerllib-0.0.5/offlinerllib/policy/model_free/awac.py` & `offlinerllib-0.0.6/offlinerllib/policy/model_free/awac.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.5/offlinerllib/policy/model_free/bppo.py` & `offlinerllib-0.0.6/offlinerllib/policy/model_free/bppo.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.5/offlinerllib/policy/model_free/dt.py` & `offlinerllib-0.0.6/offlinerllib/policy/model_free/dt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from operator import itemgetter
 from typing import Any, Dict, Optional, Union
 
 import torch
 
-from offlinerllib.module.net.attention import Transformer
+from offlinerllib.module.net.attention.dt import DecisionTransformer
 from offlinerllib.policy import BasePolicy
 from offlinerllib.utils.misc import convert_to_tensor
 
 
 class DecisionTransformerPolicy(BasePolicy):
     """
     Decision Transformer: Reinforcement Learning via Sequence Modeling <Ref: https://arxiv.org/abs/2106.01345>
     """
     def __init__(
         self, 
-        dt: Transformer, 
+        dt: DecisionTransformer, 
         dt_optim: torch.optim, 
         state_dim: int, 
         action_dim: int, 
         seq_len: int, 
         episode_len: int, 
         device: Union[str, torch.device] = "cpu"
     ) -> None:
```

### Comparing `offlinerllib-0.0.5/offlinerllib/policy/model_free/edac.py` & `offlinerllib-0.0.6/offlinerllib/policy/model_free/edac.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.5/offlinerllib/policy/model_free/inac.py` & `offlinerllib-0.0.6/offlinerllib/policy/model_free/inac.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.5/offlinerllib/policy/model_free/iql.py` & `offlinerllib-0.0.6/offlinerllib/policy/model_free/iql.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.5/offlinerllib/policy/model_free/sac.py` & `offlinerllib-0.0.6/offlinerllib/policy/model_free/sac.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.5/offlinerllib/policy/model_free/sacn.py` & `offlinerllib-0.0.6/offlinerllib/policy/model_free/sacn.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.5/offlinerllib/policy/model_free/td3.py` & `offlinerllib-0.0.6/offlinerllib/policy/model_free/td3.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.5/offlinerllib/policy/model_free/td3bc.py` & `offlinerllib-0.0.6/offlinerllib/policy/model_free/td3bc.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.5/offlinerllib/policy/model_free/xql.py` & `offlinerllib-0.0.6/offlinerllib/policy/model_free/xql.py`

 * *Files identical despite different names*

### Comparing `offlinerllib-0.0.5/offlinerllib.egg-info/PKG-INFO` & `offlinerllib-0.0.6/offlinerllib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offlinerllib
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python module desgined for Offline RL algorithms developing and benchmarking. 
 Home-page: https://github.com/typoverflow/OfflineRLLib
 Author: typoverflow
 Author-email: typoverflow@outlook.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `offlinerllib-0.0.5/offlinerllib.egg-info/SOURCES.txt` & `offlinerllib-0.0.6/offlinerllib.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 offlinerllib/buffer/__init__.py
 offlinerllib/buffer/base.py
 offlinerllib/buffer/d4rl_buffer.py
 offlinerllib/module/__init__.py
 offlinerllib/module/actor.py
 offlinerllib/module/critic.py
 offlinerllib/module/net/__init__.py
-offlinerllib/module/net/attention.py
 offlinerllib/module/net/basic.py
 offlinerllib/module/net/mlp.py
 offlinerllib/policy/__init__.py
 offlinerllib/policy/base.py
 offlinerllib/policy/model_free/__init__.py
 offlinerllib/policy/model_free/awac.py
 offlinerllib/policy/model_free/bppo.py
```

### Comparing `offlinerllib-0.0.5/setup.py` & `offlinerllib-0.0.6/setup.py`

 * *Files identical despite different names*

