# Comparing `tmp/pypose-0.4.1.tar.gz` & `tmp/pypose-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypose-0.4.1.tar", last modified: Mon Apr  3 16:38:18 2023, max compression
+gzip compressed data, was "pypose-0.4.2.tar", last modified: Wed Apr 12 04:19:37 2023, max compression
```

## Comparing `pypose-0.4.1.tar` & `pypose-0.4.2.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:38:18.704745 pypose-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-04-03 16:38:04.000000 pypose-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-03 16:38:18.704745 pypose-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-04-03 16:38:04.000000 pypose-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:38:18.696745 pypose-0.4.1/pypose/
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:38:18.696745 pypose-0.4.1/pypose/basics/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/basics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/basics/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:38:18.700745 pypose-0.4.1/pypose/lietensor/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/lietensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/lietensor/basics.py
--rw-r--r--   0 runner    (1001) docker     (123)    33855 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/lietensor/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/lietensor/function.py
--rw-r--r--   0 runner    (1001) docker     (123)    28351 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/lietensor/gradcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)    43215 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/lietensor/lietensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31560 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/lietensor/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)   109992 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/lietensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:38:18.700745 pypose-0.4.1/pypose/module/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24653 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/module/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/module/ekf.py
--rw-r--r--   0 runner    (1001) docker     (123)    22445 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/module/imu_preintegrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/module/lqr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/module/pf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/module/ukf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:38:18.704745 pypose-0.4.1/pypose/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/optim/corrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/optim/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/optim/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    24664 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/optim/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/optim/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/optim/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/optim/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:38:18.704745 pypose-0.4.1/pypose/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-04-03 16:38:04.000000 pypose-0.4.1/pypose/utils/collect_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:38:18.696745 pypose-0.4.1/pypose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-03 16:38:18.000000 pypose-0.4.1/pypose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-03 16:38:18.000000 pypose-0.4.1/pypose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 16:38:18.000000 pypose-0.4.1/pypose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-03 16:38:18.000000 pypose-0.4.1/pypose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-03 16:38:18.000000 pypose-0.4.1/pypose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 16:38:18.000000 pypose-0.4.1/pypose.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:38:18.704745 pypose-0.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-03 16:38:04.000000 pypose-0.4.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-03 16:38:04.000000 pypose-0.4.1/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 16:38:18.704745 pypose-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-03 16:38:04.000000 pypose-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.694546 pypose-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-04-12 04:19:20.000000 pypose-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-12 04:19:37.694546 pypose-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-04-12 04:19:20.000000 pypose-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.686546 pypose-0.4.2/pypose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.686546 pypose-0.4.2/pypose/basics/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/basics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/basics/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.686546 pypose-0.4.2/pypose/function/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/function/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/function/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.690546 pypose-0.4.2/pypose/lietensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/lietensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/lietensor/basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33855 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/lietensor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43215 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/lietensor/lietensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31560 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/lietensor/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109672 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/lietensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.690546 pypose-0.4.2/pypose/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24653 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22445 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/imu_preintegrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/lqr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/pf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/pnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/ukf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.690546 pypose-0.4.2/pypose/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/corrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24664 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.690546 pypose-0.4.2/pypose/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/utils/collect_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.686546 pypose-0.4.2/pypose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-12 04:19:37.000000 pypose-0.4.2/pypose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-12 04:19:37.000000 pypose-0.4.2/pypose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:19:37.000000 pypose-0.4.2/pypose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-12 04:19:37.000000 pypose-0.4.2/pypose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 04:19:37.000000 pypose-0.4.2/pypose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:19:37.000000 pypose-0.4.2/pypose.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.694546 pypose-0.4.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 04:19:20.000000 pypose-0.4.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 04:19:20.000000 pypose-0.4.2/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 04:19:37.694546 pypose-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-12 04:19:20.000000 pypose-0.4.2/setup.py
```

### Comparing `pypose-0.4.1/LICENSE` & `pypose-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/PKG-INFO` & `pypose-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypose
-Version: 0.4.1
+Version: 0.4.2
 Summary: To connect classic robotics with modern learning methods.
 Home-page: https://pypose.org
 Download-URL: https://github.com/pypose/pypose
 Author: Chen Wang
 Author-email: chenwang@dr.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/pypose/pypose/issues
```

### Comparing `pypose-0.4.1/README.md` & `pypose-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/__init__.py` & `pypose-0.4.2/pypose/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from .lietensor import identity_like, identity_SO3, identity_so3, identity_SE3, identity_se3
 from .lietensor import identity_Sim3, identity_sim3, identity_RxSO3, identity_rxso3
 from .lietensor import add, add_, mul, Exp, Log, Inv, Mul, Retr, Act, Adj, AdjT, Jinvp, Jr
 from .lietensor import SO3_type, so3_type, SE3_type, se3_type
 from .lietensor import Sim3_type, sim3_type, RxSO3_type, rxso3_type
 from .lietensor import tensor, translation, rotation, scale, matrix, euler
 from .lietensor import mat2SO3, mat2SE3, mat2Sim3, mat2RxSO3, from_matrix, matrix, euler2SO3, vec2skew
-from .lietensor import gradcheck, gradgradcheck
-from .lietensor.function import *
-from . import module, optim
+from .function import *
 from .basics import *
+from . import module
+from . import optim
 
 
 min_torch = '2.0'
 assert version.parse(min_torch) <= version.parse(torch.__version__), \
     f'PyTorch=={torch.__version__} is used but incompatible. ' \
     f'Please install torch>={min_torch}.'
```

### Comparing `pypose-0.4.1/pypose/basics/ops.py` & `pypose-0.4.2/pypose/basics/ops.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/lietensor/__init__.py` & `pypose-0.4.2/pypose/lietensor/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 from .utils import identity_like, identity_SO3, identity_so3, identity_SE3, identity_se3
 from .utils import identity_Sim3, identity_sim3, identity_RxSO3, identity_rxso3
 from .utils import SO3, so3, SE3, se3, Sim3, sim3, RxSO3, rxso3
 from .utils import Exp, Log, Inv, Mul, Retr, Act, Adj, AdjT, Jinvp, Jr
 from .basics import vec2skew, add, add_, mul
 from .convert import tensor, translation, rotation, scale, matrix, euler
 from .convert import mat2SO3, mat2SE3, mat2Sim3, mat2RxSO3, from_matrix, matrix, euler2SO3
-from .gradcheck import gradcheck, gradgradcheck
```

### Comparing `pypose-0.4.1/pypose/lietensor/basics.py` & `pypose-0.4.2/pypose/lietensor/basics.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/lietensor/convert.py` & `pypose-0.4.2/pypose/lietensor/convert.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/lietensor/function.py` & `pypose-0.4.2/pypose/function/linalg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import torch
-from . import LieTensor
-'''
-This function file includes functions using LieTensor attributes.
-'''
+from .. import LieTensor
+
 
 def bvv(lvec, rvec, *, out=None):
     r'''
     Performs batched vector-vector product, which results in matrices.
 
     Args:
         lvec (:obj:`Tensor`): left vectors to be multiplied.
@@ -105,8 +103,8 @@
     '''
     assert mat.ndim >= 2 and lvec.ndim >= 1 and rvec.ndim >= 1, 'Shape invalid'
     assert lvec.shape[-1] == mat.shape[-2] and mat.shape[-1] == rvec.shape[-1]
     lvec = lvec.tensor() if isinstance(lvec, LieTensor) else lvec
     mat = mat.tensor() if isinstance(mat, LieTensor) else mat
     rvec = rvec.tensor() if isinstance(rvec, LieTensor) else rvec
     lvec, rvec = lvec.unsqueeze(-1), rvec.unsqueeze(-1)
-    return torch.atleast_1d((lvec.mT @ mat @ rvec).squeeze_(-1).squeeze_(-1))
+    return torch.atleast_1d((lvec.mT @ mat @ rvec).squeeze_(-1).squeeze_(-1))
```

### Comparing `pypose-0.4.1/pypose/lietensor/lietensor.py` & `pypose-0.4.2/pypose/lietensor/lietensor.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/lietensor/operation.py` & `pypose-0.4.2/pypose/lietensor/operation.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/lietensor/utils.py` & `pypose-0.4.2/pypose/lietensor/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 SO3 = _LieTensor_wrapper_add_docstr(functools.partial(LieTensor, ltype=SO3_type),
     r'''Internally, SO3 LieTensors are stored as unit quaternions:
 
     .. math::
         \mathrm{data}[*, :] = [q_x, q_y, q_z, q_w],
 
     where :math:`q_x^2 + q_y^2 + q_z^2 + q_w^2 = 1`.
-    
+
     Note:
         Normalization is not required at initialization as it is done internally
         by the library right before further computation. However, the normalized
         quaternion will not be written back to the tensor storage to prevent
         in-place data alteration.
 
     Examples:
@@ -277,15 +277,15 @@
             Default: if ``None``, defaults to the device of input.
 
         requires_grad (bool, optional): If autograd should record operations on the returned
             tensor. Default: ``False``.
 
         memory_format (torch.memory_format, optional): the desired memory format of returned
             Tensor. Default: ``torch.preserve_format``.
-    
+
     Note:
         The parameter sigma (:math:`\sigma`) can either be:
 
         - a single ``float`` -- in which all the elements in the LieType share the same
           sigma.
 
         - a ``tuple`` of a number of floats -- in which case, the specific sigma for
@@ -362,24 +362,24 @@
 
     Note:
         The uniform distributed points :math:`[\delta_x', \delta_y', \delta_z']` on a sphere
         are sampled using:
 
         .. math::
             \delta_x' = \frac{x_0}{d}, \delta_y' = \frac{y_0}{d}, \delta_z' = \frac{z_0}{d},
-        
+
         where
 
         .. math::
             x_0, y_0, z_0 \sim \mathcal{N}(0, \sigma),
 
         .. math::
             d = \sqrt{(x^2_0+y^2_0+z^2_0)}.
 
-        Note that the point :math:`[x_0, y_0, z_0]` follows 3-D Gaussian distribution, 
+        Note that the point :math:`[x_0, y_0, z_0]` follows 3-D Gaussian distribution,
         which is centrosymmetry with respect to :math:`(0, 0, 0)`. Therefore, we have
         :math:`\delta_x'^2+\delta_y'^2+\delta_z'^2=1` and the normalized points follow
         uniform distribution on a standard sphere, i.e.,
         :math:`[\delta_x', \delta_y', \delta_z'] \sim \mathcal{U}_{\mathrm{s}}`.
         The point :math:`[\delta_x', \delta_y', \delta_z']` can also represent an evenly
         sampled rotation axis.
 
@@ -409,15 +409,15 @@
     return so3_type.randn(*lsize, sigma=sigma, **kwargs)
 
 
 def randn_SO3(*lsize, sigma=1.0, **kwargs):
     r'''
     Returns :obj:`SO3_type` LieTensor filled with the Exponential map of the random
     :obj:`so3_type` LieTensor.
-    
+
     .. math::
         \begin{aligned}
         \mathrm{data}[*, :] &= \mathrm{Exp}([\delta_x, \delta_y, \delta_z]) \\
                             &= \mathrm{Exp}([\delta_x', \delta_y', \delta_z'] \cdot \theta),
         \end{aligned}
 
     where :math:`[\delta_x', \delta_y', \delta_z']` is generated from uniform distribution
@@ -427,24 +427,24 @@
 
     For detailed explanation, please see :meth:`pypose.randn_so3()` and :meth:`pypose.Exp()`.
 
     Args:
         lsize (int...): a sequence of integers defining the lshape of the output tensor.
             Can be a variable number of arguments or a collection like a list or tuple.
 
-        sigma (float, optional): standard deviation for the angle of the generated rotation. 
+        sigma (float, optional): standard deviation for the angle of the generated rotation.
             Default: ``1.0``.
 
         requires_grad (bool, optional): If autograd should record operations on
             the returned tensor. Default: ``False``.
 
         generator (torch.Generator, optional): a pseudorandom number generator for sampling
 
         dtype (torch.dtype, optional): the desired data type of returned tensor.
-            Default: ``None``. 
+            Default: ``None``.
             If ``None``, uses a global default (see :meth:`torch.set_default_tensor_type()`).
 
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: ``torch.strided``.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: ``None``. If ``None``, uses the current device for the default tensor
@@ -476,40 +476,40 @@
         [0, 0, 1] (shown in blue).
     '''
     return SO3_type.randn(*lsize, sigma=sigma, **kwargs)
 
 
 def randn_se3(*lsize, sigma=1.0, **kwargs):
     r'''
-    Returns :obj:`se3_type` LieTensor filled with random numbers. 
+    Returns :obj:`se3_type` LieTensor filled with random numbers.
 
     .. math::
         \mathrm{data}[*, :] = [\tau_x, \tau_y, \tau_z, \delta_x, \delta_y, \delta_z],
-    
-    where translation :math:`[\tau_x, \tau_y, \tau_z]` is generated from a normal distribution 
+
+    where translation :math:`[\tau_x, \tau_y, \tau_z]` is generated from a normal distribution
     :math:`\mathcal{N}(0, \sigma_t)`, rotation :math:`[\delta_x, \delta_y, \delta_z]` is
     generated using :meth:`pypose.randn_so3()` with standard deviation :math:`\sigma_r`.
     Note that standard deviations :math:`\sigma_t` and :math:`\sigma_r` are
     specified by ``sigma`` (:math:`\sigma`), where :math:`\sigma = (\sigma_t, \sigma_r)`.
 
     Args:
         lsize (int...): a sequence of integers defining the lshape of the output tensor.
             Can be a variable number of arguments or a collection like a list or tuple.
 
-        sigma (float or (float...), optional): standard deviation 
-            (:math:`\sigma_t` and :math:`\sigma_r`) 
+        sigma (float or (float...), optional): standard deviation
+            (:math:`\sigma_t` and :math:`\sigma_r`)
             for the two normal distribution. Default: ``1.0``.
 
         requires_grad (bool, optional): If autograd should record operations on
             the returned tensor. Default: ``False``.
 
         generator (torch.Generator, optional): a pseudorandom number generator for sampling
 
         dtype (torch.dtype, optional): the desired data type of returned tensor.
-            Default: ``None``. If ``None``, uses a global default 
+            Default: ``None``. If ``None``, uses a global default
             (see :meth:`torch.set_default_tensor_type()`).
 
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: ``torch.strided``.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: ``None``. If ``None``, uses the current device for the default tensor
@@ -518,23 +518,23 @@
 
     Returns:
         LieTensor: a :obj:`se3_type` LieTensor.
 
     Note:
         The parameter :math:`\sigma` can either be:
 
-        - a single ``float`` -- in which all the elements in the :obj:`se3_type` 
-          share the same sigma, i.e., 
+        - a single ``float`` -- in which all the elements in the :obj:`se3_type`
+          share the same sigma, i.e.,
           :math:`\sigma_{\rm{t}}` = :math:`\sigma_{\rm{r}}` = :math:`\sigma`.
-        - a ``tuple`` of two floats -- in which case, the specific sigmas are 
-          assigned independently, i.e., 
+        - a ``tuple`` of two floats -- in which case, the specific sigmas are
+          assigned independently, i.e.,
           :math:`\sigma` = (:math:`\sigma_{\rm{t}}`, :math:`\sigma_{\rm{r}}`).
-        - a ``tuple`` of four floats -- in which case, the specific sigmas for 
-          each translation data are assigned independently, i.e., 
-          :math:`\sigma` = (:math:`\sigma_{\rm{tx}}`, :math:`\sigma_{\rm{ty}}`, 
+        - a ``tuple`` of four floats -- in which case, the specific sigmas for
+          each translation data are assigned independently, i.e.,
+          :math:`\sigma` = (:math:`\sigma_{\rm{tx}}`, :math:`\sigma_{\rm{ty}}`,
           :math:`\sigma_{\rm{tz}}`, :math:`\sigma_{\rm{r}}`).
 
     Example:
 
         For :math:`\sigma = (\sigma_t, \sigma_r)`
 
         >>> pp.randn_se3(2, sigma=(1.0, 0.5))
@@ -556,38 +556,38 @@
     r'''
     Returns :obj:`SE3_type` LieTensor filled with the Exponential map of the random
     :obj:`se3_type` LieTensor generated using :meth:`pypose.randn_se3()`.
 
     .. math::
         \mathrm{data}[*, :] = \mathrm{Exp}([\tau_x, \tau_y, \tau_z, \delta_x, \delta_y, \delta_z]),
 
-    where :math:`[\tau_x, \tau_y, \tau_z]` is generated from a normal distribution 
+    where :math:`[\tau_x, \tau_y, \tau_z]` is generated from a normal distribution
     :math:`\mathcal{N}(0, \sigma_t)`, :math:`[\delta_x, \delta_y, \delta_z]` is
     generated using :meth:`pypose.randn_so3()` with with standard deviation
     :math:`\sigma_r`, and :math:`\mathrm{Exp}()` is the Exponential map. Note that standard
     deviations :math:`\sigma_t` and :math:`\sigma_r` are specified by ``sigma`` (:math:`\sigma`),
     where :math:`\sigma = (\sigma_t, \sigma_r)`.
 
     For detailed explanation, please see :meth:`pypose.randn_se3()` and :meth:`pypose.Exp()`.
 
     Args:
         lsize (int...): a sequence of integers defining the lshape of the output tensor.
             Can be a variable number of arguments or a collection like a list or tuple.
 
-        sigma (float or (float...), optional): standard deviation 
+        sigma (float or (float...), optional): standard deviation
             (:math:`\sigma_t` and :math:`\sigma_r`) for the two normal distribution.
             Default: ``1.0``.
 
         requires_grad (bool, optional): If autograd should record operations on
             the returned tensor. Default: ``False``.
 
         generator (torch.Generator, optional): a pseudorandom number generator for sampling
 
         dtype (torch.dtype, optional): the desired data type of returned tensor.
-            Default: ``None``. If None, uses a global default 
+            Default: ``None``. If None, uses a global default
             (see :meth:`torch.set_default_tensor_type()`).
 
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: ``torch.strided``.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: ``None``. If ``None``, uses the current device for the default tensor
@@ -596,23 +596,23 @@
 
     Returns:
         LieTensor: a :obj:`SE3_type` LieTensor
 
     Note:
         The parameter :math:`\sigma` can either be:
 
-        - a single ``float`` -- in which all the elements in the :obj:`SE3_type` 
-          share the same sigma, i.e., 
+        - a single ``float`` -- in which all the elements in the :obj:`SE3_type`
+          share the same sigma, i.e.,
           :math:`\sigma_{\rm{t}}` = :math:`\sigma_{\rm{r}}` = :math:`\sigma`.
-        - a ``tuple`` of two floats -- in which case, the specific sigmas are 
+        - a ``tuple`` of two floats -- in which case, the specific sigmas are
           assigned independently, i.e.,
           :math:`\sigma` = (:math:`\sigma_{\rm{t}}`, :math:`\sigma_{\rm{r}}`).
         - a ``tuple`` of four floats -- in which case, the specific sigmas for
-          each translation data are assigned independently, i.e., 
-          :math:`\sigma` = (:math:`\sigma_{\rm{tx}}`, :math:`\sigma_{\rm{ty}}`, 
+          each translation data are assigned independently, i.e.,
+          :math:`\sigma` = (:math:`\sigma_{\rm{tx}}`, :math:`\sigma_{\rm{ty}}`,
           :math:`\sigma_{\rm{tz}}`, :math:`\sigma_{\rm{r}}`).
 
     Example:
 
         For :math:`\sigma = (\sigma_t, \sigma_r)`
 
         >>> pp.randn_SE3(2, sigma=(1.0, 2.0))
@@ -628,41 +628,41 @@
                 [ 0.2613, -2.7613,  0.2151, -0.8802,  0.2619,  0.3044,  0.2531]])
     '''
     return SE3_type.randn(*lsize, sigma=sigma, **kwargs)
 
 
 def randn_sim3(*lsize, sigma=1.0, **kwargs):
     r'''
-    Returns :obj:`sim3_type` LieTensor filled with random numbers. 
+    Returns :obj:`sim3_type` LieTensor filled with random numbers.
 
     .. math::
         \mathrm{data}[*, :] = [\tau_x, \tau_y, \tau_z, \delta_x, \delta_y, \delta_z, \log s],
 
-    where translation :math:`[\tau_x, \tau_y, \tau_z]` is generated from a normal distribution 
+    where translation :math:`[\tau_x, \tau_y, \tau_z]` is generated from a normal distribution
     :math:`\mathcal{N}(0, \sigma_t)`, rotation :math:`[\delta_x, \delta_y, \delta_z]` is
     generated using :meth:`pypose.randn_so3()` with standard deviation :math:`\sigma_r`,
     scale :math:`\log s` is generated from a normal distribution :math:`\mathcal{N}(0, \sigma_s)`.
     Note that standard deviations :math:`\sigma_t`, :math:`\sigma_r`, and :math:`\sigma_s` are
     specified by ``sigma`` (:math:`\sigma`), where :math:`\sigma=(\sigma_t,\sigma_r,\sigma_s)`.
 
     Args:
         lsize (int...): a sequence of integers defining the lshape of the output tensor.
             Can be a variable number of arguments or a collection like a list or tuple.
 
-        sigma (float or (float...), optional): standard deviation (:math:`\sigma_t`, 
+        sigma (float or (float...), optional): standard deviation (:math:`\sigma_t`,
             :math:`\sigma_r`, and :math:`\sigma_s`) for the three normal distribution.
             Default: ``1.0``.
 
         requires_grad (bool, optional): If autograd should record operations on
             the returned tensor. Default: ``False``.
 
         generator (torch.Generator, optional): a pseudorandom number generator for sampling.
 
         dtype (torch.dtype, optional): the desired data type of returned tensor.
-            Default: ``None``. If ``None``, uses a global default 
+            Default: ``None``. If ``None``, uses a global default
             (see :meth:`torch.set_default_tensor_type()`).
 
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: ``torch.strided``.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: ``None``. If ``None``, uses the current device for the default tensor
@@ -671,25 +671,25 @@
 
     Returns:
         LieTensor: a ``sim3_type`` LieTensor.
 
     Note:
         The parameter :math:`\sigma` can either be:
 
-        - a single ``float`` -- in which all the elements in the :obj:`sim3_type` 
-          share the same sigma, i.e., 
-          :math:`\sigma_{\rm{t}}` = :math:`\sigma_{\rm{r}}` = :math:`\sigma_{\rm{s}}` 
+        - a single ``float`` -- in which all the elements in the :obj:`sim3_type`
+          share the same sigma, i.e.,
+          :math:`\sigma_{\rm{t}}` = :math:`\sigma_{\rm{r}}` = :math:`\sigma_{\rm{s}}`
           = :math:`\sigma`.
-        - a ``tuple`` of three floats -- in which case, the specific sigmas for 
-          the three parts are assigned independently, i.e., 
-          :math:`\sigma` = (:math:`\sigma_{\rm{t}}`, :math:`\sigma_{\rm{r}}`, 
+        - a ``tuple`` of three floats -- in which case, the specific sigmas for
+          the three parts are assigned independently, i.e.,
+          :math:`\sigma` = (:math:`\sigma_{\rm{t}}`, :math:`\sigma_{\rm{r}}`,
           :math:`\sigma_{\rm{s}}`).
-        - a ``tuple`` of five floats -- in which case, the specific sigmas for 
+        - a ``tuple`` of five floats -- in which case, the specific sigmas for
           each translation data are also assigned independently, i.e.,
-          :math:`\sigma` = (:math:`\sigma_{\rm{tx}}`, :math:`\sigma_{\rm{ty}}`, 
+          :math:`\sigma` = (:math:`\sigma_{\rm{tx}}`, :math:`\sigma_{\rm{ty}}`,
           :math:`\sigma_{\rm{tz}}`, :math:`\sigma_{\rm{r}}`, :math:`\sigma_{\rm{s}}`).
 
     Example:
         For :math:`\sigma = (\sigma_{\rm{t}}, \sigma_{\rm{r}}, \sigma_{\rm{s}})`
 
         >>> pp.randn_sim3(sigma=(1.0, 1.0, 2.0))
         sim3Type LieTensor:
@@ -711,15 +711,15 @@
     Returns :obj:`Sim3_type` LieTensor filled with the Exponential map of the random
     :obj:`sim3_type` LieTensor generated using :meth:`randn_sim3()`.
 
     .. math::
         \mathrm{data}[*, :] = \mathrm{Exp}([\tau_x, \tau_y, \tau_z, \delta_x,
         \delta_y, \delta_z, \log s]),
 
-    where translation :math:`[\tau_x, \tau_y, \tau_z]` is generated from a normal distribution 
+    where translation :math:`[\tau_x, \tau_y, \tau_z]` is generated from a normal distribution
     :math:`\mathcal{N}(0, \sigma_t)`, rotation :math:`[\delta_x, \delta_y, \delta_z]` is
     generated using :meth:`pypose.randn_so3()` with with standard deviation
     :math:`\sigma_r`, scale :math:`\log s` is generated from a normal distribution
     :math:`\mathcal{N}(0, \sigma_s)`, and :math:`\mathrm{Exp}()` is the Exponential
     map. Note that standard deviations :math:`\sigma_t`, :math:`\sigma_r`, and
     :math:`\sigma_s` are specified by ``sigma`` (:math:`\sigma`), where
     :math:`\sigma = (\sigma_t, \sigma_r, \sigma_s)`.
@@ -727,24 +727,24 @@
     For detailed explanation, please see :meth:`pypose.randn_sim3()` and :meth:`pypose.Exp()`.
 
     Args:
         lsize (int...): a sequence of integers defining the lshape of the output tensor.
             Can be a variable number of arguments or a collection like a list or tuple.
 
         sigma (float or (float...), optional): standard deviation
-            (:math:`\sigma_t`, :math:`\sigma_r`, and :math:`\sigma_s`) 
+            (:math:`\sigma_t`, :math:`\sigma_r`, and :math:`\sigma_s`)
             for the three normal distribution. Default: ``1.0``.
 
         requires_grad (bool, optional): If autograd should record operations on
             the returned tensor. Default: ``False``.
 
         generator (torch.Generator, optional): a pseudorandom number generator for sampling
 
         dtype (torch.dtype, optional): the desired data type of returned tensor.
-            Default: ``None``. If ``None``, uses a global default 
+            Default: ``None``. If ``None``, uses a global default
             (see :meth:`torch.set_default_tensor_type()`).
 
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: ``torch.strided``.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: ``None``. If ``None``, uses the current device for the default tensor
@@ -753,25 +753,25 @@
 
     Returns:
         LieTensor: a :obj:`Sim_type` LieTensor
 
     Note:
         The parameter :math:`\sigma` can either be:
 
-        - a single ``float`` -- in which all the elements in the :obj:`Sim3_type` 
-          share the same sigma, i.e., 
-          :math:`\sigma_{\rm{t}}` = :math:`\sigma_{\rm{r}}` 
+        - a single ``float`` -- in which all the elements in the :obj:`Sim3_type`
+          share the same sigma, i.e.,
+          :math:`\sigma_{\rm{t}}` = :math:`\sigma_{\rm{r}}`
           = :math:`\sigma_{\rm{s}}` = :math:`\sigma`.
-        - a ``tuple`` of three floats -- in which case, the specific sigmas 
-          for the three parts are assigned independently, i.e., 
-          :math:`\sigma` = (:math:`\sigma_{\rm{t}}`, :math:`\sigma_{\rm{r}}`, 
+        - a ``tuple`` of three floats -- in which case, the specific sigmas
+          for the three parts are assigned independently, i.e.,
+          :math:`\sigma` = (:math:`\sigma_{\rm{t}}`, :math:`\sigma_{\rm{r}}`,
           :math:`\sigma_{\rm{s}}`).
-        - a ``tuple`` of five floats -- in which case, the specific sigmas 
+        - a ``tuple`` of five floats -- in which case, the specific sigmas
           for each translation data are also assigned independently, i.e.,
-          :math:`\sigma` = (:math:`\sigma_{\rm{tx}}`, :math:`\sigma_{\rm{ty}}`, 
+          :math:`\sigma` = (:math:`\sigma_{\rm{tx}}`, :math:`\sigma_{\rm{ty}}`,
           :math:`\sigma_{\rm{tz}}`, :math:`\sigma_{\rm{r}}`, :math:`\sigma_{\rm{s}}`).
 
     Example:
         For :math:`\sigma = (\sigma_{\rm{t}}, \sigma_{\rm{r}}, \sigma_{\rm{s}})`
 
         >>> pp.randn_Sim3(sigma=(1.0, 1.0, 2.0))
         Sim3Type LieTensor:
@@ -786,39 +786,39 @@
                 [ 0.2106, -0.0694, -0.0574, -0.2902, -0.4806, -0.0815,  0.8235,  0.0134]])
     '''
     return Sim3_type.randn(*lsize, sigma=sigma, **kwargs)
 
 
 def randn_rxso3(*lsize, sigma=1.0, **kwargs):
     r'''
-    Returns :obj:`rxso3_type` LieTensor filled with random numbers. 
+    Returns :obj:`rxso3_type` LieTensor filled with random numbers.
 
     .. math::
         \mathrm{data}[*, :] = [\delta_x, \delta_y, \delta_z, \log s],
 
     where rotation :math:`[\delta_x, \delta_y, \delta_z]` is
     generated using :meth:`pypose.randn_so3()` with standard deviation :math:`\sigma_r`,
     scale :math:`\log s` is generated from a normal distribution :math:`\mathcal{N}(0, \sigma_s)`.
     Note that standard deviations :math:`\sigma_r` and :math:`\sigma_s` are
     specified by ``sigma`` (:math:`\sigma`), where :math:`\sigma = (\sigma_r, \sigma_s)`.
 
     Args:
         lsize (int...): a sequence of integers defining the lshape of the output tensor.
             Can be a variable number of arguments or a collection like a list or tuple.
 
-        sigma (float or (float...), optional): standard deviation (:math:`\sigma_r`, 
+        sigma (float or (float...), optional): standard deviation (:math:`\sigma_r`,
             and :math:`\sigma_s`) for the two normal distribution. Default: ``1.0``.
 
         requires_grad (bool, optional): If autograd should record operations on
             the returned tensor. Default: ``False``.
 
         generator (torch.Generator, optional): a pseudorandom number generator for sampling
 
         dtype (torch.dtype, optional): the desired data type of returned tensor.
-            Default: ``None``. If ``None``, uses a global default 
+            Default: ``None``. If ``None``, uses a global default
             (see :meth:`torch.set_default_tensor_type()`).
 
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: ``torch.strided``.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: ``None``. If ``None``, uses the current device for the default tensor
@@ -827,19 +827,19 @@
 
     Returns:
         LieTensor: a :obj:`rxso3_type` LieTensor
 
     Note:
         The parameter :math:`\sigma` can either be:
 
-        - a single ``float`` -- in which all the elements in the :obj:`rxso3_type` share 
-          the same sigma, i.e., :math:`\sigma_{\rm{r}}` = :math:`\sigma_{\rm{s}}` 
+        - a single ``float`` -- in which all the elements in the :obj:`rxso3_type` share
+          the same sigma, i.e., :math:`\sigma_{\rm{r}}` = :math:`\sigma_{\rm{s}}`
           = :math:`\sigma`.
-        - a ``tuple`` of two floats -- in which case, the specific sigmas for the two parts 
-          are assigned independently, i.e., :math:`\sigma` = (:math:`\sigma_{\rm{r}}`, 
+        - a ``tuple`` of two floats -- in which case, the specific sigmas for the two parts
+          are assigned independently, i.e., :math:`\sigma` = (:math:`\sigma_{\rm{r}}`,
           :math:`\sigma_{\rm{s}}`).
 
     Example:
 
         For :math:`\sigma = (\sigma_r, \sigma_s)`
 
         >>> pp.randn_rxso3(2, sigma=(1.0, 2.0))
@@ -849,15 +849,15 @@
     '''
     return rxso3_type.randn(*lsize, sigma=sigma, **kwargs)
 
 
 def randn_RxSO3(*lsize, sigma=1.0, **kwargs):
     r'''
     Returns :obj:`RxSO3_type` LieTensor filled with the Exponential map of the random
-    :obj:`rxso3_type` LieTensor. The :obj:`rxso3_type` LieTensor is generated using 
+    :obj:`rxso3_type` LieTensor. The :obj:`rxso3_type` LieTensor is generated using
     :meth:`randn_rxso3()`.
 
     .. math::
         \mathrm{data}[*, :] = \mathrm{Exp}([\delta_x, \delta_y, \delta_z, \log s]),
 
     where rotation :math:`[\delta_x, \delta_y, \delta_z]` is generated using
     :meth:`pypose.randn_so3()` with standard deviation :math:`\sigma_r`, scale :math:`\log s`
@@ -866,24 +866,24 @@
     :math:`\sigma_r` and :math:`\sigma_s` are specified by ``sigma`` (:math:`\sigma`), where
     :math:`\sigma = (\sigma_r, \sigma_s)`.
 
     Args:
         lsize (int...): a sequence of integers defining the lshape of the output tensor.
             Can be a variable number of arguments or a collection like a list or tuple.
 
-        sigma (float or (float...), optional): standard deviation (:math:`\sigma_r`, 
+        sigma (float or (float...), optional): standard deviation (:math:`\sigma_r`,
             and :math:`\sigma_s`) for the two normal distribution. Default: ``1.0``.
 
         requires_grad (bool, optional): If autograd should record operations on
             the returned tensor. Default: ``False``.
 
         generator (torch.Generator, optional): a pseudorandom number generator for sampling
 
         dtype (torch.dtype, optional): the desired data type of returned tensor.
-            Default: ``None``. If ``None``, uses a global default 
+            Default: ``None``. If ``None``, uses a global default
             (see :meth:`torch.set_default_tensor_type()`).
 
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: ``torch.strided``.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: "None". If None, uses the current device for the default tensor
@@ -892,19 +892,19 @@
 
     Returns:
         LieTensor: a :obj:`RxSO3_type` LieTensor
 
     Note:
         The parameter :math:`\sigma` can either be:
 
-        - a single ``float`` -- in which all the elements in the :obj:`RxSO3_type` share 
-          the same sigma, i.e., :math:`\sigma_{\rm{r}}` = :math:`\sigma_{\rm{s}}` = 
+        - a single ``float`` -- in which all the elements in the :obj:`RxSO3_type` share
+          the same sigma, i.e., :math:`\sigma_{\rm{r}}` = :math:`\sigma_{\rm{s}}` =
           :math:`\sigma`.
-        - a ``tuple`` of two floats -- in which case, the specific sigmas for the two parts 
-          are assigned independently, i.e., :math:`\sigma` = (:math:`\sigma_{\rm{r}}`, 
+        - a ``tuple`` of two floats -- in which case, the specific sigmas for the two parts
+          are assigned independently, i.e., :math:`\sigma` = (:math:`\sigma_{\rm{r}}`,
           :math:`\sigma_{\rm{s}}`).
 
     Example:
 
         For :math:`\sigma = (\sigma_r, \sigma_s)`
 
         >>> pp.randn_RxSO3(2, sigma=(1.0, 2.0))
@@ -916,15 +916,15 @@
 
 
 def identity_like(liegroup, **kwargs):
     r'''
      Returns identity LieTensor with the same :obj:`lsize` and :obj:`ltype` as the given LieTensor.
 
     Args:
-        liegroup (LieTensor): the size of liegroup will determine the size of the output tensor. 
+        liegroup (LieTensor): the size of liegroup will determine the size of the output tensor.
 
     Args:
         requires_grad (bool, optional): If autograd should record operations on
             the returned tensor. Default: False.
 
         generator (torch.Generator, optional): a pseudorandom number generator for sampling
 
@@ -934,15 +934,15 @@
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: torch.strided.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: if None, uses the current device for the default tensor
             type (see :meth:`torch.set_default_tensor_type()`). device will be the CPU
             for CPU tensor types and the current CUDA device for CUDA tensor types.
-    
+
     Example:
         >>> x = pp.randn_SO3(3, device="cuda:0", dtype=torch.double, requires_grad=True)
         >>> pp.identity_like(x, device="cpu")
         SO3Type LieTensor:
         tensor([[0., 0., 0., 1.],
                 [0., 0., 0., 1.],
                 [0., 0., 0., 1.]])
@@ -973,18 +973,18 @@
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: torch.strided.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: if None, uses the current device for the default tensor
             type (see :meth:`torch.set_default_tensor_type()`). device will be the CPU
             for CPU tensor types and the current CUDA device for CUDA tensor types.
-    
+
     Returns:
         LieTensor: a :obj:`SO3_type` LieTensor
-    
+
     Example:
         >>> pp.identity_SO3()
         SO3Type LieTensor:
         tensor([0., 0., 0., 1.])
 
         >>> pp.identity_SO3(2)
         SO3Type LieTensor:
@@ -998,15 +998,15 @@
     '''
     return SO3_type.identity(*lsize, **kwargs)
 
 
 def identity_so3(*lsize, **kwargs):
     r'''
     Returns identity :obj:`so3_type` LieTensor with the given :obj:`lsize`.
-    
+
     See :obj:`so3()` for implementation details.
 
     Args:
         lsize (int..., optional): a sequence of integers defining the :obj:`LieTensor.lshape` of
             the output LieTensor. Can be a variable number of arguments or a collection like a
             list or tuple. If not given, a single :obj:`so3_type` item will be returned.
 
@@ -1022,18 +1022,18 @@
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: torch.strided.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: if None, uses the current device for the default tensor
             type (see :meth:`torch.set_default_tensor_type()`). device will be the CPU
             for CPU tensor types and the current CUDA device for CUDA tensor types.
-    
+
     Returns:
         LieTensor: a :obj:`so3_type` LieTensor
-    
+
     Example:
         >>> pp.identity_so3()
         so3Type LieTensor:
         tensor([0., 0., 0.])
 
         >>> pp.identity_so3(2)
         so3Type LieTensor:
@@ -1047,22 +1047,22 @@
     '''
     return so3_type.identity(*lsize, **kwargs)
 
 
 def identity_SE3(*lsize, **kwargs):
     r'''
     Returns identity :obj:`SE3_type` LieTensor with the given :obj:`lsize`.
-    
+
     See :obj:`SE3()` for implementation details.
 
     Args:
         lsize (int..., optional): a sequence of integers defining the :obj:`LieTensor.lshape` of
             the output LieTensor. Can be a variable number of arguments or a collection like a
             list or tuple. If not given, a single :obj:`SE3_type` item will be returned.
-    
+
     Args:
 
         requires_grad (bool, optional): If autograd should record operations on
             the returned tensor. Default: False.
 
         generator (torch.Generator, optional): a pseudorandom number generator for sampling
 
@@ -1072,18 +1072,18 @@
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: torch.strided.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: if None, uses the current device for the default tensor
             type (see :meth:`torch.set_default_tensor_type()`). device will be the CPU
             for CPU tensor types and the current CUDA device for CUDA tensor types.
-    
+
     Returns:
         LieTensor: a :obj:`SE3_type` LieTensor
-    
+
     Example:
         >>> pp.identity_SE3()
         SE3Type LieTensor:
         tensor([0., 0., 0., 0., 0., 0., 1.])
 
         >>> pp.identity_SE3(2)
         SE3Type LieTensor:
@@ -1097,17 +1097,17 @@
     '''
     return SE3_type.identity(*lsize, **kwargs)
 
 
 def identity_se3(*lsize, **kwargs):
     r'''
     Returns identity :obj:`se3_type` LieTensor with the given :obj:`lsize`.
-    
+
     See :obj:`se3()` for implementation details.
-    
+
     Args:
         lsize (int..., optional): a sequence of integers defining the :obj:`LieTensor.lshape` of
             the output LieTensor. Can be a variable number of arguments or a collection like a
             list or tuple. If not given, a single :obj:`se3_type` item will be returned.
 
     Args:
         requires_grad (bool, optional): If autograd should record operations on
@@ -1121,18 +1121,18 @@
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: torch.strided.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: if None, uses the current device for the default tensor
             type (see :meth:`torch.set_default_tensor_type()`). device will be the CPU
             for CPU tensor types and the current CUDA device for CUDA tensor types.
-    
+
     Returns:
         LieTensor: a :obj:`se3_type` LieTensor
-    
+
     Example:
         >>> pp.identity_se3()
         se3Type LieTensor:
         tensor([0., 0., 0., 0., 0., 0.])
 
         >>> pp.identity_se3(2)
         se3Type LieTensor:
@@ -1146,15 +1146,15 @@
     '''
     return se3_type.identity(*lsize, **kwargs)
 
 
 def identity_sim3(*lsize, **kwargs):
     r'''
     Returns identity :obj:`sim3_type` LieTensor with the given :obj:`lsize`.
-    
+
     See :obj:`sim3()` for implementation details.
 
     Args:
         lsize (int..., optional): a sequence of integers defining the :obj:`LieTensor.lshape` of
             the output LieTensor. Can be a variable number of arguments or a collection like a
             list or tuple. If not given, a single :obj:`sim3_type` item will be returned.
 
@@ -1170,18 +1170,18 @@
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: torch.strided.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: if None, uses the current device for the default tensor
             type (see :meth:`torch.set_default_tensor_type()`). device will be the CPU
             for CPU tensor types and the current CUDA device for CUDA tensor types.
-    
+
     Returns:
         LieTensor: a :obj:`sim3_type` LieTensor
-        
+
     Example:
         >>> pp.identity_sim3()
         sim3Type LieTensor:
         tensor([0., 0., 0., 0., 0., 0., 0.])
 
         >>> pp.identity_sim3(2)
         sim3Type LieTensor:
@@ -1195,15 +1195,15 @@
     '''
     return sim3_type.identity(*lsize, **kwargs)
 
 
 def identity_Sim3(*lsize, **kwargs):
     r'''
     Returns identity :obj:`Sim3_type` LieTensor with the given :obj:`lsize`.
-    
+
     See :obj:`Sim3()` for implementation details.
 
     Args:
         lsize (int..., optional): a sequence of integers defining the :obj:`LieTensor.lshape` of
             the output LieTensor. Can be a variable number of arguments or a collection like a
             list or tuple. If not given, a single :obj:`Sim3_type` item will be returned.
 
@@ -1219,18 +1219,18 @@
         layout (torch.layout, optional): the desired layout of returned Tensor.
             Default: torch.strided.
 
         device (torch.device, optional): the desired device of returned tensor.
             Default: if None, uses the current device for the default tensor
             type (see :meth:`torch.set_default_tensor_type()`). device will be the CPU
             for CPU tensor types and the current CUDA device for CUDA tensor types.
-    
+
     Returns:
         LieTensor: a :obj:`Sim3_type` LieTensor
-        
+
     Example:
         >>> pp.identity_Sim3()
         Sim3Type LieTensor:
         tensor([0., 0., 0., 0., 0., 0., 1., 1.])
 
         >>> pp.identity_Sim3(2)
         Sim3Type LieTensor:
@@ -1238,21 +1238,21 @@
                 [0., 0., 0., 0., 0., 0., 1., 1.]])
 
         >>> pp.identity_Sim3(2, 1)
         Sim3Type LieTensor:
         tensor([[[0., 0., 0., 0., 0., 0., 1., 1.]],
                 [[0., 0., 0., 0., 0., 0., 1., 1.]]])
     '''
-    return Sim3_type.identity(*lsize, **kwargs)    
+    return Sim3_type.identity(*lsize, **kwargs)
 
 
 def identity_rxso3(*size, **kwargs):
     r'''
     Returns identity :obj:`rxso3_type` LieTensor with the given :obj:`lsize`.
-    
+
     See :obj:`rxSO3()` for implementation details.
 
     Args:
         lsize (int..., optional): a sequence of integers defining the :obj:`LieTensor.lshape` of
             the output LieTensor. Can be a variable number of arguments or a collection like a
             list or tuple. If not given, a single :obj:`rxso3_type` item will be returned.
 
@@ -1292,15 +1292,15 @@
                 [[0., 0., 0., 0.]]])
     '''
     return rxso3_type.identity(*size, **kwargs)
 
 
 def identity_RxSO3(*size, **kwargs):
     r'''Returns identity :obj:`RxSO3_type` LieTensor with the given :obj:`lsize`.
-    
+
     See :obj:`RxSO3()` for implementation details.
 
     Args:
         lsize (int..., optional): a sequence of integers defining the :obj:`LieTensor.lshape` of
             the output LieTensor. Can be a variable number of arguments or a collection like a
             list or tuple. If not given, a single :obj:`RxSO3_type` item will be returned.
 
@@ -1426,15 +1426,15 @@
       (input :math:`\mathbf{x}` is an instance of :meth:`se3`):
 
         Let :math:`\bm{\tau}_i`, :math:`\bm{\phi}_i` be the translation and rotation parts
         of :math:`\mathbf{x}_i`, respectively; :math:`\mathbf{y}` be the output.
 
         .. math::
             \mathbf{y}_i = \left[\mathbf{J}_i\bm{\tau}_i, \mathrm{Exp}(\bm{\phi}_i)\right],
-        
+
         where :math:`\mathrm{Exp}` is the Exponential map for :obj:`so3_type` input and
         :math:`\mathbf{J}_i` is the left Jacobian for :obj:`so3_type` input.
 
     * Input :math:`\mathbf{x}`'s :obj:`ltype` is :obj:`rxso3_type`
       (input :math:`\mathbf{x}` is an instance of :meth:`rxso3`):
 
         Let :math:`\bm{\phi}_i`, :math:`\sigma_i` be the rotation and scale parts of
@@ -1452,35 +1452,35 @@
         :meth:`rxso3` parts of :math:`\mathbf{x}_i`, respectively.
         :math:`\bm{\phi}_i = \theta_i\mathbf{n}_i`, :math:`\sigma_i` be the rotation
         and scale parts of :math:`^{s}\bm{\phi}_i`, :math:`\boldsymbol{\Phi}_i` be the skew matrix
         of :math:`\bm{\phi}_i`; :math:`s_i = e^\sigma_i`, :math:`\mathbf{y}` be the output.
 
         .. math::
             \mathbf{y}_i = \left[^{s}\mathbf{W}_i\bm{\tau}_i, \mathrm{Exp}(^{s}\bm{\phi}_i)\right],
-        
+
         where
 
         .. math::
             ^s\mathbf{W}_i = A\boldsymbol{\Phi}_i + B\boldsymbol{\Phi}_i^2 + C\mathbf{I}
 
         in which if :math:`\|\sigma_i\| \geq \text{eps}`:
 
         .. math::
             A = \left\{
-                    \begin{array}{ll} 
+                    \begin{array}{ll}
                         \frac{s_i\sin\theta_i\sigma_i + (1-s_i\cos\theta_i)\theta_i}
                         {\theta_i(\sigma_i^2 + \theta_i^2)}, \quad \|\theta_i\| \geq \text{eps}, \\
                         \frac{(\sigma_i-1)s_i+1}{\sigma_i^2}, \quad \|\theta_i\| < \text{eps},
                     \end{array}
                 \right.
 
         .. math::
-            B = 
+            B =
             \left\{
-                \begin{array}{ll} 
+                \begin{array}{ll}
                     \left( C - \frac{(s_i\cos\theta_i-1)\sigma+ s_i\sin\theta_i\sigma_i}
                     {\theta_i^2+\sigma_i^2}\right)\frac{1}{\theta_i^2}, \quad \|\theta_i\|
                         \geq \text{eps}, \\
                     \frac{s_i\sigma_i^2/2 + s_i-1-\sigma_i s_i}{\sigma_i^3}, \quad \|\theta_i\|
                         < \text{eps},
                 \end{array}
             \right.
@@ -1488,32 +1488,32 @@
         .. math::
             C = \frac{e^{\sigma_i} - 1}{\sigma_i}\mathbf{I}
 
         otherwise:
 
         .. math::
             A = \left\{
-                    \begin{array}{ll} 
+                    \begin{array}{ll}
                         \frac{1-\cos\theta_i}{\theta_i^2}, \quad \|\theta_i\| \geq \text{eps}, \\
                         \frac{1}{2}, \quad \|\theta_i\| < \text{eps},
                     \end{array}
                 \right.
 
         .. math::
             B = \left\{
-                    \begin{array}{ll} 
+                    \begin{array}{ll}
                         \frac{\theta_i - \sin\theta_i}{\theta_i^3}, \quad \|\theta_i\|
                             \geq \text{eps}, \\
                         \frac{1}{6}, \quad \|\theta_i\| < \text{eps},
                     \end{array}
                 \right.
 
         .. math::
             C = 1
-    
+
     Note:
         The detailed explanation of the above :math:`\mathrm{Exp}`: calculation can be found
         in the paper:
 
         * Grassia, F. Sebastian., `Practical Parameterization of Rotations using the
           Exponential Map <https://www.tandfonline.com/doi/pdf/10.1080/10867651.1998.10487493>`_,
           Journal of graphics tools, 1998.
@@ -1528,15 +1528,15 @@
         Given :math:`\mathbf{x}=\theta\mathbf{n}`, to find its corresponding quaternion
         :math:`\mathbf{q}`, we first calculate the rotation angle :math:`\theta` using:
 
             .. math::
                 \theta = \|\mathbf{x}\|.
 
         Then, the corresponding quaternion is:
-        
+
             .. math::
                 \mathbf{q} = \left[\frac{\sin(\|\mathbf{x}\|/2)}{\|\mathbf{x}\|} \mathbf{x},
                     \cos(\|\mathbf{x}\|/2) \right].
 
         If :math:`\|\mathbf{x}\|` is small (:math:`\|\mathbf{x}\|\le \text{eps}`),
         we use the Taylor Expansion form of :math:`\sin(\|\mathbf{x}\|/2)` and
         :math:`\cos(\|\mathbf{x}\|/2)`.
@@ -1625,45 +1625,45 @@
           - :math:`\mathcal{g}\in\mathbb{R}^{*\times7}`
           - :obj:`sim3_type`
         * - :obj:`RxSO3_type`
           - :math:`\mathcal{G}\in\mathbb{R}^{*\times5}`
           - :math:`\mapsto`
           - :math:`\mathcal{g}\in\mathbb{R}^{*\times4}`
           - :obj:`rxso3_type`
-    
+
     Warning:
         This function :func:`Log()` is different from :func:`log()`, which returns
         a new torch tensor with the logarithm of the elements of the input tensor.
 
     * If input :math:`\mathbf{x}`'s :obj:`ltype` is :obj:`SO3_type`
       (input :math:`\mathbf{x}` is an instance of :meth:`SO3`):
 
         Let :math:`w_i`, :math:`\boldsymbol{\nu}_i` be the scalar and vector parts of
         :math:`\mathbf{x}_i`, respectively; :math:`\mathbf{y}` be the output.
 
         If :math:`\|\boldsymbol{\nu}_i\| > \text{eps}`:
 
         .. math::
-            \mathbf{y}_i = 
+            \mathbf{y}_i =
                 \left\{
-                    \begin{array}{ll} 
+                    \begin{array}{ll}
                         2\frac{\mathrm{arctan}(\|\boldsymbol{\nu}_i\|/w_i)}{\|
-                        \boldsymbol{\nu}_i\|}\boldsymbol{\nu}_i, 
+                        \boldsymbol{\nu}_i\|}\boldsymbol{\nu}_i,
                             \quad \|w_i\| > \text{eps}, \\
                         \mathrm{pm}(w_i) \frac{\pi}{\|\boldsymbol{\nu}_i\|}
                             \boldsymbol{\nu}_i, \quad \|w_i\| \leq \text{eps},
                     \end{array}
                 \right.
 
         otherwise:
 
         .. math::
-            \mathbf{y}_i = 2\left( \frac{1}{w_i} - 
+            \mathbf{y}_i = 2\left( \frac{1}{w_i} -
                 \frac{\|\boldsymbol{\nu}_i\|^2}{3w_i^3}\right)\boldsymbol{\nu}_i.
-        
+
         where :math:`\mathrm{pm}` is the plus or minus (:math:`\pm`) operator
         (refer to :meth:`pm`).
 
     * If input :math:`\mathbf{x}`'s :obj:`ltype` is :obj:`SE3_type`
       (input :math:`\mathbf{x}` is an instance of :meth:`SE3`):
 
         Let :math:`\mathbf{t}_i`, :math:`\mathbf{q}_i` be the translation and rotation parts of
@@ -1704,25 +1704,25 @@
             .. math::
                ^s\mathbf{W}_i = A\boldsymbol{\Phi}_i + B\boldsymbol{\Phi}_i^2 + C\mathbf{I}
 
         in which if :math:`\|\sigma_i\| > \text{eps}`:
 
         .. math::
             A = \left\{
-                    \begin{array}{ll} 
+                    \begin{array}{ll}
                         \frac{s_i\sin\theta_i\sigma_i + (1-s_i\cos\theta_i)\theta_i}
                         {\theta_i(\sigma_i^2 + \theta_i^2)}, \quad \|\theta_i\| > \text{eps}, \\
                         \frac{(\sigma_i-1)s_i+1}{\sigma_i^2}, \quad \|\theta_i\| \leq \text{eps},
                     \end{array}
                 \right.
 
         .. math::
-            B = 
+            B =
             \left\{
-                \begin{array}{ll} 
+                \begin{array}{ll}
                     \left( C - \frac{(s_i\cos\theta_i-1)\sigma+ s_i\sin\theta_i\sigma_i}
                     {\theta_i^2+\sigma_i^2}\right)\frac{1}{\theta_i^2},
                         \quad \|\theta_i\| > \text{eps}, \\
                     \frac{s_i\sigma_i^2/2 + s_i-1-\sigma_i s_i}{\sigma_i^3},
                         \quad \|\theta_i\| \leq \text{eps},
                 \end{array}
             \right.
@@ -1730,23 +1730,23 @@
         .. math::
             C = \frac{e^{\sigma_i} - 1}{\sigma_i}\mathbf{I}
 
         otherwise:
 
         .. math::
             A = \left\{
-                    \begin{array}{ll} 
+                    \begin{array}{ll}
                         \frac{1-\cos\theta_i}{\theta_i^2}, \quad \|\theta_i\| > \text{eps}, \\
                         \frac{1}{2}, \quad \|\theta_i\| \leq \text{eps},
                     \end{array}
                 \right.
 
         .. math::
             B = \left\{
-                    \begin{array}{ll} 
+                    \begin{array}{ll}
                         \frac{\theta_i - \sin\theta_i}{\theta_i^3},
                             \quad \|\theta_i\| > \text{eps}, \\
                         \frac{1}{6}, \quad \|\theta_i\| \leq \text{eps},
                     \end{array}
                 \right.
 
         .. math::
@@ -1764,32 +1764,32 @@
         unit norm :math:`\mathbf{q}` can be represented as
 
             .. math::
                 \mathbf{q} = \left[\sin(\theta/2) \mathbf{n}, \cos(\theta/2) \right]
 
         Therefore, given a quaternion :math:`\mathbf{q}=[\boldsymbol{\nu}, w]`, where
         :math:`\boldsymbol{\nu}` is the vector part, :math:`w` is the scalar part, to find
-        the corresponding rotation vector, the rotation angle :math:`\theta` can be obtained as 
+        the corresponding rotation vector, the rotation angle :math:`\theta` can be obtained as
 
             .. math::
                 \theta = 2\mathrm{arctan}(\|\boldsymbol{\nu}\|/w),~\|\boldsymbol{\nu}\|
-                = \sin(\theta/2), 
+                = \sin(\theta/2),
 
         The unit rotation axis :math:`\mathbf{n}` can be obtained as :math:`\mathbf{n} =
         \frac{\boldsymbol{\nu}}{{\|\boldsymbol{\nu}\|}}`.
-        Hence, the corresponding rotation vector is 
+        Hence, the corresponding rotation vector is
 
             .. math::
                 \theta \mathbf{n} = 2\frac{\mathrm{arctan}
                 (\|\boldsymbol{\nu}\|/w)}{\|\boldsymbol{\nu}\|}\boldsymbol{\nu}.
 
         More details about :math:`^s\mathbf{W}_i` in :obj:`Sim3_type` can be found in Eq. (5.7):
 
         * H. Strasdat, `Local accuracy and global consistency for efficient visual SLAM
-          <http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.640.199&rep=rep1&type=pdf>`_, 
+          <http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.640.199&rep=rep1&type=pdf>`_,
           Dissertation. Department of Computing, Imperial College London, 2012.
 
     Example:
 
         * :math:`\mathrm{Log}`: :obj:`SO3` :math:`\mapsto` :obj:`so3`
 
             >>> x = pp.randn_SO3()
@@ -1920,15 +1920,15 @@
     * If input :math:`\mathbf{x}`'s :obj:`ltype` is :obj:`Sim3_type` (input :math:`\mathbf{x}`
       is an instance of :meth:`Sim3`):
 
         Let :math:`\mathbf{t}_i`, :math:`^s\mathbf{q}_i` be the translation and :obj:`RxSO3` parts
         of :math:`\mathbf{x}_i`, respectively;  :math:`\mathbf{y}` be the output.
 
         .. math::
-            \mathbf{y}_i = \left[-\mathrm{Inv}(^s\mathbf{q}_i)*\mathbf{t}_i, 
+            \mathbf{y}_i = \left[-\mathrm{Inv}(^s\mathbf{q}_i)*\mathbf{t}_i,
             \mathrm{Inv}(^s\mathbf{q}_i) \right]
 
     * If input :math:`\mathbf{x}`'s :obj:`ltype` is :obj:`so3_type` or :obj:`se3_type` or
       :obj:`sim3_type` or :obj:`rxso3_type` (input :math:`\mathbf{x}` is an instance of :meth:`so3`
       or :meth:`se3` or :meth:`sim3` or :meth:`rxso3`):
 
         .. math::
@@ -2045,15 +2045,15 @@
 @assert_ltype
 def Retr(X, a):
     r"""Perform batched retraction with a given direction.
 
     .. math::
         Y_i = \mathrm{Exp}(a_i) * X_i,
 
-    where :math:`\mathrm{Exp}` means the exponetial map. See :obj:`pypose.Exp` for more details. 
+    where :math:`\mathrm{Exp}` means the exponetial map. See :obj:`pypose.Exp` for more details.
 
     Args:
         X (LieTensor): the input LieTensor to retract (Lie Group)
 
         a (LieTensor): the direction of the retraction (Lie Algebra)
 
     Return:
@@ -2150,15 +2150,15 @@
     """
     return X.Act(p)
 
 
 @assert_ltype
 def Adj(input, p):
     r"""
-    The dot product between the Adjoint matrix at the point given by an input (Lie Group) and 
+    The dot product between the Adjoint matrix at the point given by an input (Lie Group) and
     the second point (Lie Algebra).
 
     .. math::
         \mathrm{Adj}: (\mathcal{G}, \mathcal{g}) \mapsto \mathcal{g}
 
     Args:
         input (LieTensor): the input LieTensor (Lie Group)
@@ -2191,15 +2191,15 @@
           - :math:`\mapsto`
           - :math:`\mathcal{g}\in\mathbb{R}^{*\times7}`
           - :obj:`sim3_type`
         * - (:obj:`RxSO3_type`, :obj:`rxso3_type`)
           - :math:`(\mathcal{G}\in\mathbb{R}^{*\times5}, \mathcal{g}\in\mathbb{R}^{*\times4})`
           - :math:`\mapsto`
           - :math:`\mathcal{g}\in\mathbb{R}^{*\times4}`
-          - :obj:`rxso3_type` 
+          - :obj:`rxso3_type`
 
     Let the input be (:math:`\mathbf{x}`, :math:`\mathbf{p}`), :math:`\mathbf{y}` be the output.
 
         .. math::
             \mathbf{y}_i = \mathrm{Adj}(\mathbf{x}_i)\mathbf{p}_i,
 
         where, :math:`\mathrm{Adj}(\mathbf{x}_i)` is the adjoint matrix of the Lie group of
@@ -2207,15 +2207,15 @@
 
     * If input (:math:`\mathbf{x}`, :math:`\mathbf{p}`)'s :obj:`ltype` are :obj:`SO3_type` and
       :obj:`so3_type` (input :math:`\mathbf{x}` is an instance of :meth:`SO3`, :math:`\mathbf{p}`
       is an instance of :meth:`so3`). Given :math:`\mathbf{x}_i \in` :math:`\textrm{SO(3)}`.
       The adjoint transformation is given by:
 
         .. math::
-            \mathrm{Adj}(\mathbf{x}_i) = \mathbf{x}_i 
+            \mathrm{Adj}(\mathbf{x}_i) = \mathbf{x}_i
 
         In the case of :math:`\textrm{SO3}`, the adjoint transformation for an element is the same
         rotation matrix used to represent the element. Rotating a tangent vector by an element
         "moves" it from the tangent space on the right side of the element to the tangent space on
         the left.
 
     * If input (:math:`\mathbf{x}`, :math:`\mathbf{p}`)'s :obj:`ltype` are :obj:`SE3_type`
@@ -2224,99 +2224,99 @@
       :math:`\textrm{SO(3)}` and :math:`\mathbf{t}_i \in \mathbb{R}^{3\times3}` represent the
       rotation and translation part of the group. Let :math:`\mathbf{t}_{i\times}` be the skew
       matrix (:meth:`pypose.vec2skew`) of :math:`\mathbf{t}_i`.
       The adjoint transformation is given by:
 
         .. math::
             \mathrm{Adj}(\mathbf{x}_i) = \left[
-                                \begin{array}{cc} 
+                                \begin{array}{cc}
                                     \mathbf{R}_i & \mathbf{t}_{i\times}\mathbf{R}_i \\
                                     0 & \mathbf{R}_i
                                 \end{array}
                              \right] \in \mathbb{R}^{6\times6}
 
         where,
 
         .. math::
             \mathbf{x}_i = \left[
-                                \begin{array}{cc} 
+                                \begin{array}{cc}
                                     \mathbf{R}_i& \mathbf{t}_i \\
                                     0 & 1
                                 \end{array}
-                             \right] \in \mathrm{SE(3)}  
+                             \right] \in \mathrm{SE(3)}
 
     * If input (:math:`\mathbf{x}`, :math:`\mathbf{p}`)'s :obj:`ltype` are :obj:`Sim3_type` and
       :obj:`sim3_type` (input :math:`\mathbf{x}` is an instance of :meth:`Sim3`, :math:`\mathbf{p}`
       is an instance of :meth:`sim3`). Let :math:`\mathbf{R}_i\in` :math:`\textrm{SO(3)}`,
       :math:`\mathbf{t}_i \in \mathbb{R}^{3\times3}`, and :math:`s_i \in \mathbb{R}^+` represent
       the rotation, translation, and scale parts of the group. Let :math:`\mathbf{t}_{i\times}`
       be the skew matrix (:meth:`pypose.vec2skew`) of :math:`\mathbf{t}_i`. The adjoint
       transformation is given by:
 
         .. math::
             \mathrm{Adj}(\mathbf{x}_i) = \left[
-                        \begin{array}{cc} 
+                        \begin{array}{cc}
                             s_i\mathbf{R}_i& \mathbf{t}_{i\times}\mathbf{R}_i& -\mathbf{t}_i \\
                             0 & \mathbf{R}_i& 0 \\
                             0 & 0 & 1
                         \end{array}
                         \right] \in \mathbb{R}^{7\times7}
 
         where,
 
         .. math::
             \mathbf{x}_i = \left[
-                                \begin{array}{cc} 
+                                \begin{array}{cc}
                                     s_i\mathbf{R}_i & \mathbf{t}_i \\
                                     0 & 1
                                 \end{array}
-                             \right] \in \textrm{Sim(3)}    
+                             \right] \in \textrm{Sim(3)}
 
     * If input (:math:`\mathbf{x}`, :math:`\mathbf{p}`)'s :obj:`ltype` are :obj:`RxSO3_type`
       and :obj:`rxso3_type` (input :math:`\mathbf{x}` is an instance of :meth:`RxSO3`,
       :math:`\mathbf{p}` is an instance of :meth:`rxso3`). Let :math:`\mathbf{R}_i \in`
       :math:`\textrm{SO(3)}`, and :math:`s_i \in \mathbb{R}^+` represent the rotation and
       scale parts of the group. The adjoint transformation is given by:
 
         .. math::
             \mathrm{Adj}(\mathbf{x}_i) = \left[
-                                \begin{array}{cc} 
+                                \begin{array}{cc}
                                     \mathbf{R}_i & 0 \\
                                     0 & 1
                                 \end{array}
                              \right] \in \mathbb{R}^{4\times4}
 
         where,
 
         .. math::
             \mathbf{x}_i = \left[
-                                \begin{array}{cc} 
+                                \begin{array}{cc}
                                     s_i\mathbf{R}_i & 0 \\
                                     0 & 1
                                 \end{array}
                              \right] \in \mathrm{RxSO(3)}
 
         In the case of :math:`\textrm{RxSO3}` group, the adjoint transformation is the same as
         the rotation matrix of the group i.e. the :math:`\textrm{SO3}` part of the group.
 
     Note:
         The adjoint operator is a linear map which moves an element
         :math:`\mathbf{p} \in \mathcal{g}` in the right tangent space of
         :math:`\mathbf{x} \in \mathcal{G}` to the left tangent space.
 
         .. math::
-            \mathrm{Exp}(\mathrm{Adj}(\mathbf{x}) \mathbf{p}) * \mathbf{x} 
+            \mathrm{Exp}(\mathrm{Adj}(\mathbf{x}) \mathbf{p}) * \mathbf{x}
             = \mathbf{x} * \mathrm{Exp}(\mathbf{p})
-        
+
         It can be easily verified:
 
             >>> x, p = pp.randn_SO3(), pp.randn_so3()
             >>> torch.allclose(x*p.Exp(), x.Adj(p).Exp()*x)
             True
-        
+
         One can refer to Eq. (8) of the following paper:
 
         * Zachary Teed et al., `Tangent Space Backpropagation for 3D Transformation Groups
           <https://arxiv.org/pdf/2103.12032.pdf>`_, IEEE/CVF Conference on Computer Vision
           and Pattern Recognition (CVPR), 2021.
 
     Note:
@@ -2324,18 +2324,18 @@
         space around one element to the tangent space of another.
         One can refer to this paper for more details:
 
         * J. Sola et al., `A micro Lie theory for state estimation in
           robotics <https://arxiv.org/abs/1812.01537>`_, arXiv preprint arXiv:1812.01537 (2018).
 
         The following thesis and the tutorial serve as a good reading material to learn more
-        about deriving the adjoint matrices for different transformation groups. 
+        about deriving the adjoint matrices for different transformation groups.
 
         * Strasdat, H., 2012. `Local accuracy and global consistency for efficient visual SLAM
-          <https://www.doc.ic.ac.uk/~ajd/Publications/Strasdat-H-2012-PhD-Thesis.pdf>`_, 
+          <https://www.doc.ic.ac.uk/~ajd/Publications/Strasdat-H-2012-PhD-Thesis.pdf>`_,
           (Doctoral dissertation, Department of Computing, Imperial College London).
 
         * `Lie Groups for 2D and 3D Transformations.
           <https://www.ethaneade.org/lie.pdf>`_, by Ethan Eade.
 
     Example:
 
@@ -2431,34 +2431,34 @@
 
     Let the input be (:math:`\mathbf{x}`, :math:`\mathbf{p}`), :math:`\mathbf{y}` be the output.
 
         .. math::
             \mathbf{y}_i = \mathbf{J}^{-1}_i(\mathbf{x}_i)\mathbf{p}_i,
 
         where :math:`\mathbf{J}^{-1}_i(\mathbf{x}_i)` is the inverse of left Jacobian of
-        :math:`\mathbf{x}_i`. 
+        :math:`\mathbf{x}_i`.
 
     * If input (:math:`\mathbf{x}`, :math:`\mathbf{p}`)'s :obj:`ltype` are :obj:`SO3_type`
       and :obj:`so3_type` (input :math:`\mathbf{x}` is an instance of :meth:`SO3`,
       :math:`\mathbf{p}` is an instance of :meth:`so3`).
       Let :math:`\boldsymbol{\phi}_i = \theta_i\mathbf{n}_i` be the corresponding Lie Algebra
       of :math:`\mathbf{x}_i`, :math:`\boldsymbol{\Phi}_i` be the skew matrix
       (:meth:`pypose.vec2skew`) of :math:`\boldsymbol{\phi}_i`:
 
         .. math::
             \mathbf{J}^{-1}_i(\mathbf{x}_i) = \mathbf{I} - \frac{1}{2}\boldsymbol{\Phi}_i +
             \mathrm{coef}\boldsymbol{\Phi}_i^2
 
       where :math:`\mathbf{I}` is the identity matrix with the same dimension as
-      :math:`\boldsymbol{\Phi}_i`, and 
+      :math:`\boldsymbol{\Phi}_i`, and
 
         .. math::
             \mathrm{coef} =
                 \left\{
-                \begin{array}{ll} 
+                \begin{array}{ll}
                     \frac{1}{\theta_i^2} -
                     \frac{\cos{\frac{\theta_i}{2}}}{2\theta\sin{\frac{\theta_i}{2}}},
                     \quad \|\theta_i\| > \text{eps}, \\
                     \frac{1}{12},
                     \quad \|\theta_i\| \leq \text{eps}
                 \end{array}
                 \right.
@@ -2470,102 +2470,102 @@
       of the SO3 part of :math:`\mathbf{x}_i`, :math:`\boldsymbol{\tau}_i` be the Lie Algebra
       of the translation part of :math:`\mathbf{x}_i`; :math:`\boldsymbol{\Phi}_i` and
       :math:`\boldsymbol{\Tau}_i` be the skew matrices, respectively:
 
         .. math::
             \mathbf{J}^{-1}_i(\mathbf{x}_i) =
                 \left[
-                \begin{array}{cc} 
-                    \mathbf{J}_i^{-1}(\boldsymbol{\Phi}_i) & 
+                \begin{array}{cc}
+                    \mathbf{J}_i^{-1}(\boldsymbol{\Phi}_i) &
                             - \mathbf{J}_i^{-1}(\boldsymbol{\Phi}_i)
-                    \mathbf{Q}_i(\boldsymbol{\tau}_i, \boldsymbol{\phi}_i) 
+                    \mathbf{Q}_i(\boldsymbol{\tau}_i, \boldsymbol{\phi}_i)
                         \mathbf{J}_i^{-1}(\boldsymbol{\Phi}_i) \\
                     \mathbf{0} & \mathbf{J}_i^{-1}(\boldsymbol{\Phi}_i)
                 \end{array}
                 \right]
 
         where :math:`\mathbf{J}_i^{-1}(\boldsymbol{\Phi}_i)` is the inverse of left Jacobian
-        of the SO3 part of :math:`\mathbf{x}_i`. 
-        :math:`\mathbf{Q}_i(\boldsymbol{\tau}_i, \boldsymbol{\phi}_i)` is 
+        of the SO3 part of :math:`\mathbf{x}_i`.
+        :math:`\mathbf{Q}_i(\boldsymbol{\tau}_i, \boldsymbol{\phi}_i)` is
 
         .. math::
             \begin{align*}
-                \mathbf{Q}_i(\boldsymbol{\tau}_i, \boldsymbol{\phi}_i) = 
+                \mathbf{Q}_i(\boldsymbol{\tau}_i, \boldsymbol{\phi}_i) =
                     \frac{1}{2}\boldsymbol{\Tau}_i &+ c_1
-                (\boldsymbol{\Phi_i\Tau_i} + \boldsymbol{\Tau_i\Phi_i} 
+                (\boldsymbol{\Phi_i\Tau_i} + \boldsymbol{\Tau_i\Phi_i}
                     + \boldsymbol{\Phi_i\Tau_i\Phi_i}) \\
-                 &+ c_2 (\boldsymbol{\Phi_i^2\Tau_i} + \boldsymbol{\Tau_i\Phi_i^2} 
+                 &+ c_2 (\boldsymbol{\Phi_i^2\Tau_i} + \boldsymbol{\Tau_i\Phi_i^2}
                     - 3\boldsymbol{\Phi_i\Tau_i\Phi_i})\\
-                 &+ c_3 (\boldsymbol{\Phi_i\Tau_i\Phi_i^2} + \boldsymbol{\Phi_i^2\Tau_i\Phi_i})  
+                 &+ c_3 (\boldsymbol{\Phi_i\Tau_i\Phi_i^2} + \boldsymbol{\Phi_i^2\Tau_i\Phi_i})
             \end{align*}
 
         where,
 
         .. math::
             c_1 = \left\{
-                    \begin{array}{ll} 
+                    \begin{array}{ll}
                         \frac{\theta_i - \sin\theta_i}{\theta_i^3},
                             \quad \|\theta_i\| > \text{eps}, \\
                         \frac{1}{6}-\frac{1}{120}\theta_i^2,
                         \quad \|\theta_i\| \leq \text{eps}
                     \end{array}
                     \right.
 
         .. math::
             c_2 = \left\{
-                    \begin{array}{ll} 
+                    \begin{array}{ll}
                         \frac{\theta_i^2 +2\cos\theta_i - 2}{2\theta_i^4},
                             \quad \|\theta_i\| > \text{eps}, \\
                         \frac{1}{24}-\frac{1}{720}\theta_i^2,
                         \quad \|\theta_i\| \leq \text{eps}
                     \end{array}
                     \right.
 
         .. math::
             c_3 = \left\{
-                    \begin{array}{ll} 
-                        \frac{2\theta_i - 3\sin\theta_i + \theta_i\cos\theta_i}{2\theta_i^5}, 
+                    \begin{array}{ll}
+                        \frac{2\theta_i - 3\sin\theta_i + \theta_i\cos\theta_i}{2\theta_i^5},
                         \quad \|\theta_i\| > \text{eps}, \\
                         \frac{1}{120}-\frac{1}{2520}\theta_i^2,
                         \quad \|\theta_i\| \leq \text{eps}
                     \end{array}
-                    \right.           
+                    \right.
 
     * If input (:math:`\mathbf{x}`, :math:`\mathbf{p}`)'s :obj:`ltype` are :obj:`Sim3_type`
       and :obj:`sim3_type` (input :math:`\mathbf{x}` is an instance of :meth:`Sim3`,
       :math:`\mathbf{p}` is an instance of :meth:`sim3`). The inverse of left Jacobian can
       be approximated as:
 
         .. math::
-            \mathbf{J}^{-1}_i(\mathbf{x}_i) = 
+            \mathbf{J}^{-1}_i(\mathbf{x}_i) =
                 \sum_{n=0}(-1)^n\frac{B_n}{n!}(\boldsymbol{\xi}_i^{\curlywedge})^n
 
         where :math:`B_n` is the Bernoulli number: :math:`B_0 = 1`, :math:`B_1 = -\frac{1}{2}`,
         :math:`B_2 = \frac{1}{6}`, :math:`B_3 = 0`, :math:`B_4 = -\frac{1}{30}`.
         :math:`\boldsymbol{\xi}_i^{\curlywedge} = \mathrm{adj}(\boldsymbol{\xi}_i^{\wedge})`
         and :math:`\mathrm{adj}` is the adjoint of the Lie algebra :math:`\mathfrak{sim}(3)`,
         e.g., :math:`\boldsymbol{\xi}_i \in \mathfrak{sim}(3)`. Notice that if notate
         :math:`\boldsymbol{X}_i = \mathrm{Adj}(\mathbf{x}_i)` and :math:`\mathrm{Adj}` is the
         adjoint of the Lie group :math:`\mathrm{Sim}(3)`, there is a nice property:
         :math:`\mathrm{Adj}(\mathrm{Exp}(\boldsymbol{\xi}_i^{\curlywedge})) =
-        \mathrm{Exp}(\mathrm{adj}(\boldsymbol{\xi}_i^{\wedge}))`, 
+        \mathrm{Exp}(\mathrm{adj}(\boldsymbol{\xi}_i^{\wedge}))`,
         or :math:`\boldsymbol{X}_i = \mathrm{Exp}(\boldsymbol{\xi}_i^{\curlywedge})`.
-        
+
 
     * If input (:math:`\mathbf{x}`, :math:`\mathbf{p}`)'s :obj:`ltype` are :obj:`RxSO3_type`
       and :obj:`rxso3_type` (input :math:`\mathbf{x}` is an instance of :meth:`RxSO3`,
       :math:`\mathbf{p}` is an instance of :meth:`rxso3`). Let :math:`\boldsymbol{\phi}_i`
       be the corresponding Lie Algebra of the SO3 part of :math:`\mathbf{x}_i`,
       :math:`\boldsymbol{\Phi}_i` be the skew matrix (:meth:`pypose.vec2skew`), The inverse
       of left Jacobian of :math:`\mathbf{x}_i` is the same as that for the SO3 part of
       :math:`\mathbf{x}_i`.
 
         .. math::
             \mathbf{J}^{-1}_i(\mathbf{x}_i) = \left[
-                                \begin{array}{cc} 
+                                \begin{array}{cc}
                                     \mathbf{J}_i^{-1}(\boldsymbol{\Phi}_i) & \mathbf{0} \\
                                     \mathbf{0} & 1
                                 \end{array}
                              \right]
 
         where :math:`\mathbf{J}_i^{-1}(\boldsymbol{\Phi}_i)` is the
         inverse of left Jacobian of the SO3 part of :math:`\mathbf{x}_i`.
@@ -2574,19 +2574,19 @@
         :math:`\mathrm{Jinvp}` is usually used in the Baker-Campbell-Hausdorff formula
         (BCH formula) when performing LieTensor multiplication.
         One can refer to this paper for more details:
 
         * J. Sola et al., `A micro Lie theory for state estimation in
           robotics <https://arxiv.org/abs/1812.01537>`_, arXiv preprint arXiv:1812.01537 (2018).
 
-        In particular, Eq. (146) is the math used in the :obj:`SO3_type`, :obj:`so3_type` scenario; 
+        In particular, Eq. (146) is the math used in the :obj:`SO3_type`, :obj:`so3_type` scenario;
         Eq. (179b) and Eq. (180) are the math used in the :obj:`SE3_type`, :obj:`se3_type` scenario.
 
         For Lie groups such as :obj:`Sim3_type`, :obj:`sim3_type`,
-        there is no analytic expression for the left Jacobian and its inverse. 
+        there is no analytic expression for the left Jacobian and its inverse.
         Numerical approximation is used based on series expansion.
         One can refer to Eq. (26) of this paper for more details about the approximation:
 
         * Z. Teed et al., `Tangent Space Backpropagation for 3D Transformation Groups.
           <https://arxiv.org/pdf/2103.12032.pdf>`_, in IEEE/CVF Conference on Computer Vision and
           Pattern Recognition (CVPR) (2021).
```

### Comparing `pypose-0.4.1/pypose/module/dynamics.py` & `pypose-0.4.2/pypose/module/dynamics.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/module/ekf.py` & `pypose-0.4.2/pypose/module/ekf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/module/imu_preintegrator.py` & `pypose-0.4.2/pypose/module/imu_preintegrator.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/module/lqr.py` & `pypose-0.4.2/pypose/module/lqr.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/module/pf.py` & `pypose-0.4.2/pypose/module/pf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/module/ukf.py` & `pypose-0.4.2/pypose/module/ukf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/optim/corrector.py` & `pypose-0.4.2/pypose/optim/corrector.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/optim/functional.py` & `pypose-0.4.2/pypose/optim/functional.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/optim/kernel.py` & `pypose-0.4.2/pypose/optim/kernel.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/optim/optimizer.py` & `pypose-0.4.2/pypose/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/optim/scheduler.py` & `pypose-0.4.2/pypose/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/optim/solver.py` & `pypose-0.4.2/pypose/optim/solver.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/optim/strategy.py` & `pypose-0.4.2/pypose/optim/strategy.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose/utils/collect_env.py` & `pypose-0.4.2/pypose/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.1/pypose.egg-info/PKG-INFO` & `pypose-0.4.2/pypose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypose
-Version: 0.4.1
+Version: 0.4.2
 Summary: To connect classic robotics with modern learning methods.
 Home-page: https://pypose.org
 Download-URL: https://github.com/pypose/pypose
 Author: Chen Wang
 Author-email: chenwang@dr.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/pypose/pypose/issues
```

### Comparing `pypose-0.4.1/pypose.egg-info/SOURCES.txt` & `pypose-0.4.2/pypose.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 pypose.egg-info/SOURCES.txt
 pypose.egg-info/dependency_links.txt
 pypose.egg-info/requires.txt
 pypose.egg-info/top_level.txt
 pypose.egg-info/zip-safe
 pypose/basics/__init__.py
 pypose/basics/ops.py
+pypose/function/__init__.py
+pypose/function/geometry.py
+pypose/function/linalg.py
 pypose/lietensor/__init__.py
 pypose/lietensor/basics.py
 pypose/lietensor/convert.py
-pypose/lietensor/function.py
-pypose/lietensor/gradcheck.py
 pypose/lietensor/lietensor.py
 pypose/lietensor/operation.py
 pypose/lietensor/utils.py
 pypose/module/__init__.py
 pypose/module/dynamics.py
 pypose/module/ekf.py
 pypose/module/imu_preintegrator.py
 pypose/module/lqr.py
 pypose/module/pf.py
+pypose/module/pnp.py
 pypose/module/ukf.py
 pypose/optim/__init__.py
 pypose/optim/corrector.py
 pypose/optim/functional.py
 pypose/optim/kernel.py
 pypose/optim/optimizer.py
 pypose/optim/scheduler.py
```

### Comparing `pypose-0.4.1/setup.py` & `pypose-0.4.2/setup.py`

 * *Files identical despite different names*

