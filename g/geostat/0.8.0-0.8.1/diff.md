# Comparing `tmp/geostat-0.8.0.tar.gz` & `tmp/geostat-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/whdc/git/geostat/dist/.tmp-i1jhopsr/geostat-0.8.0.tar", last modified: Mon Apr 10 23:28:57 2023, max compression
+gzip compressed data, was "/home/whdc/git/geostat/dist/.tmp-qu2ms_y7/geostat-0.8.1.tar", last modified: Wed Apr 12 16:29:55 2023, max compression
```

## Comparing `geostat-0.8.0.tar` & `geostat-0.8.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-10 23:28:57.117009 geostat-0.8.0/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    11357 2022-08-12 07:59:13.000000 geostat-0.8.0/LICENSE
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-10 23:28:57.117009 geostat-0.8.0/PKG-INFO
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      687 2022-08-12 07:59:13.000000 geostat-0.8.0/README.md
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      679 2023-04-10 23:28:45.000000 geostat-0.8.0/pyproject.toml
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      926 2023-04-10 23:28:57.117009 geostat-0.8.0/setup.cfg
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-10 23:28:57.113009 geostat-0.8.0/src/
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-10 23:28:57.113009 geostat-0.8.0/src/geostat/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      268 2023-04-10 23:06:48.000000 geostat-0.8.0/src/geostat/__init__.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    13134 2023-04-10 22:40:44.000000 geostat-0.8.0/src/geostat/kernel.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    25489 2023-03-05 02:04:42.000000 geostat-0.8.0/src/geostat/krige.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3658 2023-04-10 22:02:47.000000 geostat-0.8.0/src/geostat/mean.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2620 2022-08-16 21:11:34.000000 geostat-0.8.0/src/geostat/mesh.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2557 2023-03-05 02:04:42.000000 geostat-0.8.0/src/geostat/metric.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    22135 2023-04-10 22:15:32.000000 geostat-0.8.0/src/geostat/model.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3424 2023-04-10 21:29:01.000000 geostat-0.8.0/src/geostat/op.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2972 2023-03-05 02:04:15.000000 geostat-0.8.0/src/geostat/param.py
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-10 23:28:57.113009 geostat-0.8.0/src/geostat.egg-info/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-10 23:28:57.000000 geostat-0.8.0/src/geostat.egg-info/PKG-INFO
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      592 2023-04-10 23:28:57.000000 geostat-0.8.0/src/geostat.egg-info/SOURCES.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)        1 2023-04-10 23:28:57.000000 geostat-0.8.0/src/geostat.egg-info/dependency_links.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      143 2023-04-10 23:28:57.000000 geostat-0.8.0/src/geostat.egg-info/requires.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)        8 2023-04-10 23:28:57.000000 geostat-0.8.0/src/geostat.egg-info/top_level.txt
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-10 23:28:57.117009 geostat-0.8.0/tests/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     4635 2023-04-10 21:29:01.000000 geostat-0.8.0/tests/test_antiderivative.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3732 2023-04-10 22:36:21.000000 geostat-0.8.0/tests/test_delta.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     5731 2023-04-10 21:29:01.000000 geostat-0.8.0/tests/test_gp.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     1147 2022-08-12 07:59:13.000000 geostat-0.8.0/tests/test_krige.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3507 2023-04-10 22:36:43.000000 geostat-0.8.0/tests/test_mcmc.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      768 2022-08-12 08:18:35.000000 geostat-0.8.0/tests/test_mesh.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2625 2023-04-10 21:50:09.000000 geostat-0.8.0/tests/test_metric.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2582 2023-04-10 22:14:06.000000 geostat-0.8.0/tests/test_multigp.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3761 2023-04-10 21:52:59.000000 geostat-0.8.0/tests/test_trend.py
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-12 16:29:55.875049 geostat-0.8.1/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    11357 2022-08-12 07:59:13.000000 geostat-0.8.1/LICENSE
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-12 16:29:55.875049 geostat-0.8.1/PKG-INFO
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      687 2022-08-12 07:59:13.000000 geostat-0.8.1/README.md
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      679 2023-04-12 16:29:33.000000 geostat-0.8.1/pyproject.toml
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      926 2023-04-12 16:29:55.875049 geostat-0.8.1/setup.cfg
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-12 16:29:55.875049 geostat-0.8.1/src/
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-12 16:29:55.875049 geostat-0.8.1/src/geostat/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      268 2023-04-12 16:29:22.000000 geostat-0.8.1/src/geostat/__init__.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    16578 2023-04-12 07:07:58.000000 geostat-0.8.1/src/geostat/kernel.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    25489 2023-03-05 02:04:42.000000 geostat-0.8.1/src/geostat/krige.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3658 2023-04-10 22:02:47.000000 geostat-0.8.1/src/geostat/mean.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2620 2022-08-16 21:11:34.000000 geostat-0.8.1/src/geostat/mesh.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2557 2023-03-05 02:04:42.000000 geostat-0.8.1/src/geostat/metric.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    22135 2023-04-10 22:15:32.000000 geostat-0.8.1/src/geostat/model.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3424 2023-04-10 21:29:01.000000 geostat-0.8.1/src/geostat/op.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3167 2023-04-12 00:49:25.000000 geostat-0.8.1/src/geostat/param.py
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-12 16:29:55.875049 geostat-0.8.1/src/geostat.egg-info/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-12 16:29:55.000000 geostat-0.8.1/src/geostat.egg-info/PKG-INFO
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      592 2023-04-12 16:29:55.000000 geostat-0.8.1/src/geostat.egg-info/SOURCES.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)        1 2023-04-12 16:29:55.000000 geostat-0.8.1/src/geostat.egg-info/dependency_links.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      143 2023-04-12 16:29:55.000000 geostat-0.8.1/src/geostat.egg-info/requires.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)        8 2023-04-12 16:29:55.000000 geostat-0.8.1/src/geostat.egg-info/top_level.txt
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-12 16:29:55.875049 geostat-0.8.1/tests/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     4635 2023-04-10 21:29:01.000000 geostat-0.8.1/tests/test_antiderivative.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3732 2023-04-10 22:36:21.000000 geostat-0.8.1/tests/test_delta.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     5731 2023-04-10 21:29:01.000000 geostat-0.8.1/tests/test_gp.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     1147 2022-08-12 07:59:13.000000 geostat-0.8.1/tests/test_krige.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3507 2023-04-10 22:36:43.000000 geostat-0.8.1/tests/test_mcmc.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      768 2022-08-12 08:18:35.000000 geostat-0.8.1/tests/test_mesh.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2625 2023-04-10 21:50:09.000000 geostat-0.8.1/tests/test_metric.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2582 2023-04-10 22:14:06.000000 geostat-0.8.1/tests/test_multigp.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3761 2023-04-10 21:52:59.000000 geostat-0.8.1/tests/test_trend.py
```

### Comparing `geostat-0.8.0/LICENSE` & `geostat-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/PKG-INFO` & `geostat-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geostat
-Version: 0.8.0
+Version: 0.8.1
 Summary: Model spatial data with Gaussian processes
 Home-page: https://code.usgs.gov/mjstephens/geostat
 Author: Michael J. Stephens, Will Chang
 Author-email: "Michael J. Stephens" <mjstephens@usgs.gov>, Will Chang <will@hypergradient.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `geostat-0.8.0/README.md` & `geostat-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/pyproject.toml` & `geostat-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geostat"
-version = "0.8.0"
+version = "0.8.1"
 description = "Model spatial data with Gaussian processes"
 readme = "README.md"
 authors = [
   {name="Michael J. Stephens", email="mjstephens@usgs.gov"},
   {name="Will Chang", email="will@hypergradient.ai"}
 ]
 license = { file = "LICENSE" }
```

### Comparing `geostat-0.8.0/setup.cfg` & `geostat-0.8.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = geostat
-version = 0.8.0
+version = 0.8.1
 author = Michael J. Stephens, Will Chang
 author_email = mjstephens@usgs.gov, will@hypergradient.ai
 description = Python package for performing kriging and Gaussian processes with geoscience-oriented utilities.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://code.usgs.gov/mjstephens/geostat
 project_urls =
```

### Comparing `geostat-0.8.0/src/geostat/kernel.py` & `geostat-0.8.1/src/geostat/kernel.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     warnings.filterwarnings("ignore", category=DeprecationWarning)
     import tensorflow as tf
     from tensorflow.linalg import LinearOperatorFullMatrix as LOFullMatrix
     from tensorflow.linalg import LinearOperatorBlockDiag as LOBlockDiag
 
 from .op import Op
 from .metric import Euclidean, PerAxisDist2, ed
-from .param import get_parameter_values, ppp, upp, bpp
+from .param import get_parameter_values, ppp, upp, bpp, ppp_list
 from .mean import get_trend_coefs
 
 __all__ = ['Kernel']
 
 def block_diag(blocks):
     """Return a dense block-diagonal matrix."""
     return LOBlockDiag([LOFullMatrix(b) for b in blocks]).to_dense()
@@ -120,14 +120,100 @@
         v = get_parameter_values(self.fa, p)
         return v['sill'] * gamma_exp(e['d2'] / tf.square(v['range']), v['gamma'])
 
     def reg(self, p):
         v = get_parameter_values(self.fa, p)
         return v['range']
 
+@tf.custom_gradient
+def ramp(x):
+    ax = tf.abs(x)
+    def grad(upstream):
+        return upstream * tf.where(ax < 1., -tf.sign(x), 0.)
+    return tf.maximum(0., 1. - ax), grad
+
+class Ramp(Kernel):
+    def __init__(self, range='range', sill='sill', scale=None, metric=None):
+        fa = dict(sill=sill, range=range, scale=scale)
+        autoinputs = scale_to_metric(scale, metric)
+        super().__init__(fa, dict(d2=autoinputs))
+
+    def vars(self):
+        return ppp(self.fa['sill']) + ppp(self.fa['range'])
+
+    def call(self, p, e):
+        v = get_parameter_values(self.fa, p)
+        # return v['sill'] * tf.clip_by_value(1. - tf.sqrt(e['d2']) / v['range'], 0., 1.)
+        return v['sill'] * ramp(tf.sqrt(e['d2']) / v['range'])
+
+    def reg(self, p):
+        v = get_parameter_values(self.fa, p)
+        return v['range']
+
+# @tf.custom_gradient
+# def rampstack(x, sills, ranges):
+#     """
+#     `x` has arbitrary shape [...].
+#     `sills` and `ranges` both have shape [K].
+#     """
+#     ax = ed(tf.abs(x)) # [..., 1]
+#     y = sills * tf.maximum(0., 1. - ax / ranges) # [..., K]
+#     def grad(upstream):
+#         ax = ed(tf.abs(x)) # [..., 1]
+#         y = sills * tf.maximum(0., 1. - ax / ranges) # [..., K]
+#         K = tf.shape(sills)[0]
+#         grad_x = upstream * tf.reduce_sum(tf.where(ax < ranges, -tf.sign(ed(x)), 0.), -1) # [...]
+#         grad_sills = tf.reduce_sum(tf.reshape(ed(upstream) * y, [-1, K]), 0) # [K}
+#         grad_ranges = tf.where(ax < ranges, sills * ax / tf.square(ranges), 0.) # [..., K}
+#         grad_ranges = tf.reduce_sum(tf.reshape(ed(upstream) * grad_ranges, [-1, K]), 0) # [K]
+#         return grad_x, grad_sills, grad_ranges
+#     return tf.reduce_sum(y, -1), grad
+
+@tf.custom_gradient
+def rampstack(x, sills, ranges):
+    """
+    `x` has arbitrary shape [...], but must be non-negative.
+    `sills` and `ranges` both have shape [K].
+    """
+    ax = ed(tf.abs(x)) # [..., 1]
+    y = sills * tf.maximum(0., 1. - ax / ranges) # [..., K]
+    def grad(upstream):
+        ax = ed(tf.abs(x)) # [..., 1]
+        y = sills * tf.maximum(0., 1. - ax / ranges) # [..., K]
+        K = tf.shape(sills)[0]
+        small = ax < ranges
+        grad_x = upstream * tf.reduce_sum(tf.where(small, -tf.sign(ed(x)) * (sills / ranges), 0.), -1) # [...]
+        grad_sills = tf.einsum('ak,a->k', tf.reshape(y, [-1, K]), tf.reshape(upstream, [-1]))
+        grad_ranges = tf.where(small, ax * (sills / tf.square(ranges)), 0.) # [..., K}
+        grad_ranges = tf.einsum('ak,a->k', tf.reshape(grad_ranges, [-1, K]), tf.reshape(upstream, [-1]))
+        return grad_x, grad_sills, grad_ranges
+    return tf.reduce_sum(y, -1), grad
+
+class RampStack(Kernel):
+    def __init__(self, range='range', sill='sill', scale=None, metric=None):
+        fa = dict(sill=sill, range=range, scale=scale)
+        autoinputs = scale_to_metric(scale, metric)
+        super().__init__(fa, dict(d2=autoinputs))
+
+    def vars(self):
+        return ppp_list(self.fa['sill']) + ppp_list(self.fa['range'])
+
+    def call(self, p, e):
+        v = get_parameter_values(self.fa, p)
+        if isinstance(v['sill'], (tuple, list)):
+            v['sill'] = tf.stack(v['sill'])
+        if isinstance(v['range'], (tuple, list)):
+            v['range'] = tf.stack(v['range'])
+
+        return rampstack(tf.sqrt(e['d2']), v['sill'], v['range'])
+
+    def reg(self, p):
+        v = get_parameter_values(self.fa, p)
+        return v['range']
+
 class Wiener(Kernel):
     def __init__(self, axis, start):
 
         self.axis = axis
         self.start = start
 
         # Include the element of scale corresponding to the axis of
```

### Comparing `geostat-0.8.0/src/geostat/krige.py` & `geostat-0.8.1/src/geostat/krige.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/src/geostat/mean.py` & `geostat-0.8.1/src/geostat/mean.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/src/geostat/mesh.py` & `geostat-0.8.1/src/geostat/mesh.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/src/geostat/metric.py` & `geostat-0.8.1/src/geostat/metric.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/src/geostat/model.py` & `geostat-0.8.1/src/geostat/model.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/src/geostat/op.py` & `geostat-0.8.1/src/geostat/op.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/src/geostat/param.py` & `geostat-0.8.1/src/geostat/param.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,7 +103,15 @@
 
 def bpp(name, lo, hi):
     """Bounded paper parameter (maybe)."""
     if isinstance(name, str):
         return [PaperParameter(name, lo, hi)]
     else:
         return []
+
+def ppp_list(beta):
+    if isinstance(beta, (list, tuple)):
+        return [p for s in beta for p in ppp(s)]
+    elif isinstance(beta, str):
+        return ppp(beta)
+    else:
+        return []
```

### Comparing `geostat-0.8.0/src/geostat.egg-info/PKG-INFO` & `geostat-0.8.1/src/geostat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geostat
-Version: 0.8.0
+Version: 0.8.1
 Summary: Model spatial data with Gaussian processes
 Home-page: https://code.usgs.gov/mjstephens/geostat
 Author: Michael J. Stephens, Will Chang
 Author-email: "Michael J. Stephens" <mjstephens@usgs.gov>, Will Chang <will@hypergradient.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `geostat-0.8.0/src/geostat.egg-info/SOURCES.txt` & `geostat-0.8.1/src/geostat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/tests/test_antiderivative.py` & `geostat-0.8.1/tests/test_antiderivative.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/tests/test_delta.py` & `geostat-0.8.1/tests/test_delta.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/tests/test_gp.py` & `geostat-0.8.1/tests/test_gp.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/tests/test_krige.py` & `geostat-0.8.1/tests/test_krige.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/tests/test_mcmc.py` & `geostat-0.8.1/tests/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/tests/test_mesh.py` & `geostat-0.8.1/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/tests/test_metric.py` & `geostat-0.8.1/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/tests/test_multigp.py` & `geostat-0.8.1/tests/test_multigp.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.0/tests/test_trend.py` & `geostat-0.8.1/tests/test_trend.py`

 * *Files identical despite different names*

