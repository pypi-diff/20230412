# Comparing `tmp/vector_quantize_pytorch-1.1.2.tar.gz` & `tmp/vector_quantize_pytorch-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.1.2.tar", last modified: Sat Mar 11 19:17:13 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.1.4.tar", last modified: Wed Apr 12 20:09:51 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.1.2.tar` & `vector_quantize_pytorch-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:17:13.705819 vector_quantize_pytorch-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-11 19:17:03.000000 vector_quantize_pytorch-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-11 19:17:13.705819 vector_quantize_pytorch-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-03-11 19:17:03.000000 vector_quantize_pytorch-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 19:17:13.705819 vector_quantize_pytorch-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-11 19:17:03.000000 vector_quantize_pytorch-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:17:13.701818 vector_quantize_pytorch-1.1.2/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-11 19:17:03.000000 vector_quantize_pytorch-1.1.2/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-11 19:17:03.000000 vector_quantize_pytorch-1.1.2/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-03-11 19:17:03.000000 vector_quantize_pytorch-1.1.2/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    21351 2023-03-11 19:17:03.000000 vector_quantize_pytorch-1.1.2/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 19:17:13.705819 vector_quantize_pytorch-1.1.2/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-11 19:17:13.000000 vector_quantize_pytorch-1.1.2/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-11 19:17:13.000000 vector_quantize_pytorch-1.1.2/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 19:17:13.000000 vector_quantize_pytorch-1.1.2/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-11 19:17:13.000000 vector_quantize_pytorch-1.1.2/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-11 19:17:13.000000 vector_quantize_pytorch-1.1.2/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:09:51.841647 vector_quantize_pytorch-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-12 20:09:51.837647 vector_quantize_pytorch-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:09:51.841647 vector_quantize_pytorch-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:09:51.837647 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21351 2023-04-12 20:09:43.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:09:51.837647 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-12 20:09:51.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-12 20:09:51.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:09:51.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 20:09:51.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 20:09:51.000000 vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.1.2/LICENSE` & `vector_quantize_pytorch-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.1.2/PKG-INFO` & `vector_quantize_pytorch-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.1.2
+Version: 1.1.4
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.1.2/README.md` & `vector_quantize_pytorch-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.1.2/setup.py` & `vector_quantize_pytorch-1.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.1.2',
+  version = '1.1.4',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.1.2/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,26 +21,33 @@
         self.num_codebooks = num_codebooks
 
         rand_projs = torch.empty(num_codebooks, dim, codebook_dim)
         nn.init.xavier_normal_(rand_projs)
 
         self.register_buffer('rand_projs', rand_projs)
 
+        # in section 3 of https://arxiv.org/abs/2202.01855
+        # "The input data is normalized to have 0 mean and standard deviation of 1 ... to prevent collapse"
+
+        self.norm = nn.LayerNorm(dim, elementwise_affine = False)
+
         self.vq = VectorQuantize(
             dim = codebook_dim * num_codebooks,
             heads = num_codebooks,
             codebook_size = codebook_size,
             use_cosine_sim = True,
             separate_codebook_per_head = True,
             **kwargs
         )
 
     @torch.no_grad()
     def forward(self, x):
 
+        x = self.norm(x)
+
         x = einsum('b n d, h d e -> b n h e', x, self.rand_projs)
         x, ps = pack([x], 'b n *')
 
         self.vq.eval()
         _, indices, _ = self.vq(x)
 
         return indices
```

### Comparing `vector_quantize_pytorch-1.1.2/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.1.2/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.1.4/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.1.2/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.1.4/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.1.2
+Version: 1.1.4
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

