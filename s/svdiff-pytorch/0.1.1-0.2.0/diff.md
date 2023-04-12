# Comparing `tmp/svdiff-pytorch-0.1.1.tar.gz` & `tmp/svdiff-pytorch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svdiff-pytorch-0.1.1.tar", last modified: Sat Apr  8 14:09:38 2023, max compression
+gzip compressed data, was "svdiff-pytorch-0.2.0.tar", last modified: Wed Apr 12 13:40:29 2023, max compression
```

## Comparing `svdiff-pytorch-0.1.1.tar` & `svdiff-pytorch-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:09:38.836530 svdiff-pytorch-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-08 14:09:38.836530 svdiff-pytorch-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 14:09:38.836530 svdiff-pytorch-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:09:38.832530 svdiff-pytorch-0.1.1/svdiff_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/svdiff_pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:09:38.836530 svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19847 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    28096 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/cross_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/dual_transformer_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)    30179 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/transformer_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    99385 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/unet_2d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    31416 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/svdiff_pytorch/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-08 14:09:29.000000 svdiff-pytorch-0.1.1/svdiff_pytorch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 14:09:38.836530 svdiff-pytorch-0.1.1/svdiff_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-08 14:09:38.000000 svdiff-pytorch-0.1.1/svdiff_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-08 14:09:38.000000 svdiff-pytorch-0.1.1/svdiff_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 14:09:38.000000 svdiff-pytorch-0.1.1/svdiff_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-08 14:09:38.000000 svdiff-pytorch-0.1.1/svdiff_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-08 14:09:38.000000 svdiff-pytorch-0.1.1/svdiff_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:40:29.875095 svdiff-pytorch-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-12 13:40:29.875095 svdiff-pytorch-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 13:40:29.875095 svdiff-pytorch-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:40:29.871095 svdiff-pytorch-0.2.0/svdiff_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:40:29.875095 svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19875 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28124 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/cross_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/dual_transformer_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30195 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/transformer_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99401 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/unet_2d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31444 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/pipeline_stable_diffusion_ddim_inversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:40:29.875095 svdiff-pytorch-0.2.0/svdiff_pytorch/transformers_models_clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/transformers_models_clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56985 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/transformers_models_clip/modeling_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-12 13:40:20.000000 svdiff-pytorch-0.2.0/svdiff_pytorch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:40:29.871095 svdiff-pytorch-0.2.0/svdiff_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-12 13:40:29.000000 svdiff-pytorch-0.2.0/svdiff_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-12 13:40:29.000000 svdiff-pytorch-0.2.0/svdiff_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:40:29.000000 svdiff-pytorch-0.2.0/svdiff_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 13:40:29.000000 svdiff-pytorch-0.2.0/svdiff_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 13:40:29.000000 svdiff-pytorch-0.2.0/svdiff_pytorch.egg-info/top_level.txt
```

### Comparing `svdiff-pytorch-0.1.1/LICENSE` & `svdiff-pytorch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svdiff-pytorch-0.1.1/setup.py` & `svdiff-pytorch-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 
 setup(
     name="svdiff-pytorch",
-    version="0.1.1",
+    version="0.2.0",
     author="Makoto Shing",
     url="https://github.com/mkshing/svdiff-pytorch",
     description="Implementation of 'SVDiff: Compact Parameter Space for Diffusion Fine-Tuning'",
     install_requires=[
     "diffusers==0.14.0",
     "accelerate",
     "torchvision",
```

### Comparing `svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/attention.py` & `svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import torch
 import torch.nn.functional as F
 from torch import nn
 
 from diffusers.utils.import_utils import is_xformers_available
 from svdiff_pytorch.diffusers_models.cross_attention import CrossAttention
 from diffusers.models.embeddings import CombinedTimestepLabelEmbeddings
-from svdiff_pytorch.layers import SVDLinear
+from svdiff_pytorch.layers import SVDLinear, SVDGroupNorm, SVDLayerNorm
 
 
 if is_xformers_available():
     import xformers
     import xformers.ops
 else:
     xformers = None
@@ -58,15 +58,15 @@
         eps: float = 1e-5,
     ):
         super().__init__()
         self.channels = channels
 
         self.num_heads = channels // num_head_channels if num_head_channels is not None else 1
         self.num_head_size = num_head_channels
-        self.group_norm = nn.GroupNorm(num_channels=channels, num_groups=norm_num_groups, eps=eps, affine=True)
+        self.group_norm = SVDGroupNorm(num_channels=channels, num_groups=norm_num_groups, eps=eps, affine=True)
 
         # define q,k,v as linear layers
         self.query = SVDLinear(channels, channels)
         self.key = SVDLinear(channels, channels)
         self.value = SVDLinear(channels, channels)
 
         self.rescale_output_factor = rescale_output_factor
@@ -248,30 +248,30 @@
             self.attn2 = None
 
         if self.use_ada_layer_norm:
             self.norm1 = AdaLayerNorm(dim, num_embeds_ada_norm)
         elif self.use_ada_layer_norm_zero:
             self.norm1 = AdaLayerNormZero(dim, num_embeds_ada_norm)
         else:
-            self.norm1 = nn.LayerNorm(dim, elementwise_affine=norm_elementwise_affine)
+            self.norm1 = SVDLayerNorm(dim, elementwise_affine=norm_elementwise_affine)
 
         if cross_attention_dim is not None:
             # We currently only use AdaLayerNormZero for self attention where there will only be one attention block.
             # I.e. the number of returned modulation chunks from AdaLayerZero would not make sense if returned during
             # the second cross attention block.
             self.norm2 = (
                 AdaLayerNorm(dim, num_embeds_ada_norm)
                 if self.use_ada_layer_norm
-                else nn.LayerNorm(dim, elementwise_affine=norm_elementwise_affine)
+                else SVDLayerNorm(dim, elementwise_affine=norm_elementwise_affine)
             )
         else:
             self.norm2 = None
 
         # 3. Feed-forward
-        self.norm3 = nn.LayerNorm(dim, elementwise_affine=norm_elementwise_affine)
+        self.norm3 = SVDLayerNorm(dim, elementwise_affine=norm_elementwise_affine)
 
     def forward(
         self,
         hidden_states,
         encoder_hidden_states=None,
         timestep=None,
         attention_mask=None,
@@ -449,15 +449,15 @@
     """
 
     def __init__(self, embedding_dim, num_embeddings):
         super().__init__()
         self.emb = nn.Embedding(num_embeddings, embedding_dim)
         self.silu = nn.SiLU()
         self.linear = SVDLinear(embedding_dim, embedding_dim * 2)
-        self.norm = nn.LayerNorm(embedding_dim, elementwise_affine=False)
+        self.norm = SVDLayerNorm(embedding_dim, elementwise_affine=False)
 
     def forward(self, x, timestep):
         emb = self.linear(self.silu(self.emb(timestep)))
         scale, shift = torch.chunk(emb, 2)
         x = self.norm(x) * (1 + scale) + shift
         return x
 
@@ -470,15 +470,15 @@
     def __init__(self, embedding_dim, num_embeddings):
         super().__init__()
 
         self.emb = CombinedTimestepLabelEmbeddings(num_embeddings, embedding_dim)
 
         self.silu = nn.SiLU()
         self.linear = SVDLinear(embedding_dim, 6 * embedding_dim, bias=True)
-        self.norm = nn.LayerNorm(embedding_dim, elementwise_affine=False, eps=1e-6)
+        self.norm = SVDLayerNorm(embedding_dim, elementwise_affine=False, eps=1e-6)
 
     def forward(self, x, timestep, class_labels, hidden_dtype=None):
         emb = self.linear(self.silu(self.emb(timestep, class_labels, hidden_dtype=hidden_dtype)))
         shift_msa, scale_msa, gate_msa, shift_mlp, scale_mlp, gate_mlp = emb.chunk(6, dim=1)
         x = self.norm(x) * (1 + scale_msa[:, None]) + shift_msa[:, None]
         return x, gate_msa, shift_mlp, scale_mlp, gate_mlp
```

### Comparing `svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/cross_attention.py` & `svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/cross_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 
 from diffusers.utils import deprecate, logging
 from diffusers.utils.import_utils import is_xformers_available
-from svdiff_pytorch.layers import SVDLinear
+from svdiff_pytorch.layers import SVDLinear, SVDGroupNorm, SVDLayerNorm
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
 if is_xformers_available():
     import xformers
@@ -76,20 +76,20 @@
         # is split across the batch axis to save memory
         # You can set slice_size with `set_attention_slice`
         self.sliceable_head_dim = heads
 
         self.added_kv_proj_dim = added_kv_proj_dim
 
         if norm_num_groups is not None:
-            self.group_norm = nn.GroupNorm(num_channels=inner_dim, num_groups=norm_num_groups, eps=1e-5, affine=True)
+            self.group_norm = SVDGroupNorm(num_channels=inner_dim, num_groups=norm_num_groups, eps=1e-5, affine=True)
         else:
             self.group_norm = None
 
         if cross_attention_norm:
-            self.norm_cross = nn.LayerNorm(cross_attention_dim)
+            self.norm_cross = SVDLayerNorm(cross_attention_dim)
 
         self.to_q = SVDLinear(query_dim, inner_dim, bias=bias)
         self.to_k = SVDLinear(cross_attention_dim, inner_dim, bias=bias)
         self.to_v = SVDLinear(cross_attention_dim, inner_dim, bias=bias)
 
         if self.added_kv_proj_dim is not None:
             self.add_k_proj = SVDLinear(added_kv_proj_dim, cross_attention_dim)
```

### Comparing `svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/dual_transformer_2d.py` & `svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/dual_transformer_2d.py`

 * *Files identical despite different names*

### Comparing `svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/embeddings.py` & `svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/embeddings.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         self.flatten = flatten
         self.layer_norm = layer_norm
 
         self.proj = nn.Conv2d(
             in_channels, embed_dim, kernel_size=(patch_size, patch_size), stride=patch_size, bias=bias
         )
         if layer_norm:
-            self.norm = nn.LayerNorm(embed_dim, elementwise_affine=False, eps=1e-6)
+            self.norm = SVDLayerNorm(embed_dim, elementwise_affine=False, eps=1e-6)
         else:
             self.norm = None
 
         pos_embed = get_2d_sincos_pos_embed(embed_dim, int(num_patches**0.5))
         self.register_buffer("pos_embed", torch.from_numpy(pos_embed).float().unsqueeze(0), persistent=False)
 
     def forward(self, latent):
```

### Comparing `svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/resnet.py` & `svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/resnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from svdiff_pytorch.diffusers_models.attention import AdaGroupNorm
-from svdiff_pytorch.layers import SVDConv1d, SVDConv2d, SVDLinear
+from svdiff_pytorch.layers import SVDConv1d, SVDConv2d, SVDLinear, SVDGroupNorm, SVDLayerNorm
 
 
 class Upsample1D(nn.Module):
     """
     An upsampling layer with an optional convolution.
 
     Parameters:
@@ -468,15 +468,15 @@
 
         if groups_out is None:
             groups_out = groups
 
         if self.time_embedding_norm == "ada_group":
             self.norm1 = AdaGroupNorm(temb_channels, in_channels, groups, eps=eps)
         else:
-            self.norm1 = torch.nn.GroupNorm(num_groups=groups, num_channels=in_channels, eps=eps, affine=True)
+            self.norm1 = SVDGroupNorm(num_groups=groups, num_channels=in_channels, eps=eps, affine=True)
 
         self.conv1 = SVDConv2d(in_channels, out_channels, kernel_size=3, stride=1, padding=1)
 
         if temb_channels is not None:
             if self.time_embedding_norm == "default":
                 self.time_emb_proj = SVDLinear(temb_channels, out_channels)
             elif self.time_embedding_norm == "scale_shift":
@@ -487,15 +487,15 @@
                 raise ValueError(f"unknown time_embedding_norm : {self.time_embedding_norm} ")
         else:
             self.time_emb_proj = None
 
         if self.time_embedding_norm == "ada_group":
             self.norm2 = AdaGroupNorm(temb_channels, out_channels, groups_out, eps=eps)
         else:
-            self.norm2 = torch.nn.GroupNorm(num_groups=groups_out, num_channels=out_channels, eps=eps, affine=True)
+            self.norm2 = SVDGroupNorm(num_groups=groups_out, num_channels=out_channels, eps=eps, affine=True)
 
         self.dropout = torch.nn.Dropout(dropout)
         conv_2d_out_channels = conv_2d_out_channels or out_channels
         self.conv2 = SVDConv2d(out_channels, conv_2d_out_channels, kernel_size=3, stride=1, padding=1)
 
         if non_linearity == "swish":
             self.nonlinearity = lambda x: F.silu(x)
@@ -605,15 +605,15 @@
     Conv1d --> GroupNorm --> Mish
     """
 
     def __init__(self, inp_channels, out_channels, kernel_size, n_groups=8):
         super().__init__()
 
         self.conv1d = SVDConv1d(inp_channels, out_channels, kernel_size, padding=kernel_size // 2)
-        self.group_norm = nn.GroupNorm(n_groups, out_channels)
+        self.group_norm = SVDGroupNorm(n_groups, out_channels)
         self.mish = nn.Mish()
 
     def forward(self, x):
         x = self.conv1d(x)
         x = rearrange_dims(x)
         x = self.group_norm(x)
         x = rearrange_dims(x)
```

### Comparing `svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/transformer_2d.py` & `svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/transformer_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from diffusers.configuration_utils import ConfigMixin, register_to_config
 from diffusers.models.embeddings import ImagePositionalEmbeddings
 from diffusers.utils import BaseOutput, deprecate
 from svdiff_pytorch.diffusers_models.attention import BasicTransformerBlock
 from diffusers.models.embeddings import PatchEmbed
 from diffusers.models.modeling_utils import ModelMixin
-from svdiff_pytorch.layers import SVDConv1d, SVDConv2d, SVDLinear
+from svdiff_pytorch.layers import SVDConv1d, SVDConv2d, SVDLinear, SVDGroupNorm, SVDLayerNorm
 
 
 @dataclass
 class Transformer2DModelOutput(BaseOutput):
     """
     Args:
         sample (`torch.FloatTensor` of shape `(batch_size, num_channels, height, width)` or `(batch size, num_vector_embeds - 1, num_latent_pixels)` if [`Transformer2DModel`] is discrete):
@@ -139,15 +139,15 @@
                 f" {patch_size}. Make sure that `in_channels`, `num_vector_embeds` or `num_patches` is not None."
             )
 
         # 2. Define input layers
         if self.is_input_continuous:
             self.in_channels = in_channels
 
-            self.norm = torch.nn.GroupNorm(num_groups=norm_num_groups, num_channels=in_channels, eps=1e-6, affine=True)
+            self.norm = SVDGroupNorm(num_groups=norm_num_groups, num_channels=in_channels, eps=1e-6, affine=True)
             if use_linear_projection:
                 self.proj_in = SVDLinear(in_channels, inner_dim)
             else:
                 self.proj_in = SVDConv2d(in_channels, inner_dim, kernel_size=1, stride=1, padding=0)
         elif self.is_input_vectorized:
             assert sample_size is not None, "Transformer2DModel over discrete input must provide sample_size"
             assert num_vector_embeds is not None, "Transformer2DModel over discrete input must provide num_embed"
@@ -201,18 +201,18 @@
         if self.is_input_continuous:
             # TODO: should use out_channels for continous projections
             if use_linear_projection:
                 self.proj_out = SVDLinear(inner_dim, in_channels)
             else:
                 self.proj_out = SVDConv2d(inner_dim, in_channels, kernel_size=1, stride=1, padding=0)
         elif self.is_input_vectorized:
-            self.norm_out = nn.LayerNorm(inner_dim)
+            self.norm_out = SVDLayerNorm(inner_dim)
             self.out = SVDLinear(inner_dim, self.num_vector_embeds - 1)
         elif self.is_input_patches:
-            self.norm_out = nn.LayerNorm(inner_dim, elementwise_affine=False, eps=1e-6)
+            self.norm_out = SVDLayerNorm(inner_dim, elementwise_affine=False, eps=1e-6)
             self.proj_out_1 = SVDLinear(inner_dim, 2 * inner_dim)
             self.proj_out_2 = SVDLinear(inner_dim, patch_size * patch_size * self.out_channels)
 
     def forward(
         self,
         hidden_states,
         encoder_hidden_states=None,
```

### Comparing `svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/unet_2d_blocks.py` & `svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/unet_2d_blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from torch import nn
 
 from svdiff_pytorch.diffusers_models.attention import AdaGroupNorm, AttentionBlock
 from svdiff_pytorch.diffusers_models.cross_attention import CrossAttention, CrossAttnAddedKVProcessor
 from svdiff_pytorch.diffusers_models.dual_transformer_2d import DualTransformer2DModel
 from svdiff_pytorch.diffusers_models.resnet import Downsample2D, FirDownsample2D, FirUpsample2D, KDownsample2D, KUpsample2D, ResnetBlock2D, Upsample2D
 from svdiff_pytorch.diffusers_models.transformer_2d import Transformer2DModel
-from svdiff_pytorch.layers import SVDConv1d, SVDConv2d, SVDLinear
+from svdiff_pytorch.layers import SVDConv1d, SVDConv2d, SVDLinear, SVDLayerNorm, SVDGroupNorm
 
 
 def get_down_block(
     down_block_type,
     num_layers,
     in_channels,
     out_channels,
@@ -2085,15 +2085,15 @@
                 output_scale_factor=output_scale_factor,
                 pre_norm=resnet_pre_norm,
                 use_in_shortcut=True,
                 up=True,
                 kernel="fir",
             )
             self.skip_conv = SVDConv2d(out_channels, 3, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-            self.skip_norm = torch.nn.GroupNorm(
+            self.skip_norm = SVDGroupNorm(
                 num_groups=min(out_channels // 4, 32), num_channels=out_channels, eps=resnet_eps, affine=True
             )
             self.act = nn.SiLU()
         else:
             self.resnet_up = None
             self.skip_conv = None
             self.skip_norm = None
@@ -2182,15 +2182,15 @@
                 output_scale_factor=output_scale_factor,
                 pre_norm=resnet_pre_norm,
                 use_in_shortcut=True,
                 up=True,
                 kernel="fir",
             )
             self.skip_conv = SVDConv2d(out_channels, 3, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
-            self.skip_norm = torch.nn.GroupNorm(
+            self.skip_norm = SVDGroupNorm(
                 num_groups=min(out_channels // 4, 32), num_channels=out_channels, eps=resnet_eps, affine=True
             )
             self.act = nn.SiLU()
         else:
             self.resnet_up = None
             self.skip_conv = None
             self.skip_norm = None
```

### Comparing `svdiff-pytorch-0.1.1/svdiff_pytorch/diffusers_models/unet_2d_condition.py` & `svdiff-pytorch-0.2.0/svdiff_pytorch/diffusers_models/unet_2d_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     DownBlock2D,
     UNetMidBlock2DCrossAttn,
     UNetMidBlock2DSimpleCrossAttn,
     UpBlock2D,
     get_down_block,
     get_up_block,
 )
-from svdiff_pytorch.layers import SVDConv1d, SVDConv2d, SVDLinear
+from svdiff_pytorch.layers import SVDConv1d, SVDConv2d, SVDLinear, SVDGroupNorm, SVDLayerNorm
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
 @dataclass
 class UNet2DConditionOutput(BaseOutput):
@@ -344,15 +344,15 @@
                 resnet_time_scale_shift=resnet_time_scale_shift,
             )
             self.up_blocks.append(up_block)
             prev_output_channel = output_channel
 
         # out
         if norm_num_groups is not None:
-            self.conv_norm_out = nn.GroupNorm(
+            self.conv_norm_out = SVDGroupNorm(
                 num_channels=block_out_channels[0], num_groups=norm_num_groups, eps=norm_eps
             )
             self.conv_act = nn.SiLU()
         else:
             self.conv_norm_out = None
             self.conv_act = None
```

### Comparing `svdiff-pytorch-0.1.1/svdiff_pytorch/utils.py` & `svdiff-pytorch-0.2.0/svdiff_pytorch/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,18 +9,19 @@
     LMSDiscreteScheduler,
     DDIMScheduler,
     PNDMScheduler,
     DPMSolverMultistepScheduler,
     EulerDiscreteScheduler,
     EulerAncestralDiscreteScheduler,
 )
+from transformers import CLIPTextModel, CLIPTextConfig
 from diffusers import UNet2DConditionModel
 from safetensors.torch import safe_open
-from huggingface_hub import hf_hub_download
-from svdiff_pytorch import UNet2DConditionModelForSVDiff
+import huggingface_hub
+from svdiff_pytorch import UNet2DConditionModelForSVDiff, CLIPTextModelForSVDiff
 
 
 
 def load_unet_for_svdiff(pretrained_model_name_or_path, spectral_shifts_ckpt=None, hf_hub_kwargs=None, **kwargs):
     """
     https://github.com/huggingface/diffusers/blob/v0.14.0/src/diffusers/models/modeling_utils.py#L541
     """
@@ -34,15 +35,15 @@
     torch_dtype = kwargs["torch_dtype"] if "torch_dtype" in kwargs else None
     spectral_shifts_weights = {n: torch.zeros(p.shape) for n, p in model.named_parameters() if "delta" in n}
     state_dict.update(spectral_shifts_weights)
     # move the params from meta device to cpu
     missing_keys = set(model.state_dict().keys()) - set(state_dict.keys())
     if len(missing_keys) > 0:
         raise ValueError(
-            f"Cannot load {cls} from {pretrained_model_name_or_path} because the following keys are"
+            f"Cannot load {model.__class__.__name__} from {pretrained_model_name_or_path} because the following keys are"
             f" missing: \n {', '.join(missing_keys)}. \n Please make sure to pass"
             " `low_cpu_mem_usage=False` and `device_map=None` if you want to randomely initialize"
             " those weights or else make sure your checkpoint file is correct."
         )
 
     for param_name, param in state_dict.items():
         accepts_dtype = "dtype" in set(inspect.signature(set_module_tensor_to_device).parameters.keys())
@@ -53,36 +54,105 @@
     
     if spectral_shifts_ckpt:
         if os.path.isdir(spectral_shifts_ckpt):
             spectral_shifts_ckpt = os.path.join(spectral_shifts_ckpt, "spectral_shifts.safetensors")
         elif not os.path.exists(spectral_shifts_ckpt):
             # download from hub
             hf_hub_kwargs = {} if hf_hub_kwargs is None else hf_hub_kwargs
-            spectral_shifts_ckpt = hf_hub_download(spectral_shifts_ckpt, filename="spectral_shifts.safetensors", **hf_hub_kwargs)
+            spectral_shifts_ckpt = huggingface_hub.hf_hub_download(spectral_shifts_ckpt, filename="spectral_shifts.safetensors", **hf_hub_kwargs)
         assert os.path.exists(spectral_shifts_ckpt)
 
         with safe_open(spectral_shifts_ckpt, framework="pt", device="cpu") as f:
             for key in f.keys():
                 # spectral_shifts_weights[key] = f.get_tensor(key)
                 accepts_dtype = "dtype" in set(inspect.signature(set_module_tensor_to_device).parameters.keys())
                 if accepts_dtype:
                     set_module_tensor_to_device(model, key, param_device, value=f.get_tensor(key), dtype=torch_dtype)
                 else:
                     set_module_tensor_to_device(model, key, param_device, value=f.get_tensor(key))
-        print(f"Resume from {spectral_shifts_ckpt}")
+        print(f"Resumed from {spectral_shifts_ckpt}")
     if "torch_dtype"in kwargs:
         model = model.to(kwargs["torch_dtype"])
     model.register_to_config(_name_or_path=pretrained_model_name_or_path)
     # Set model in evaluation mode to deactivate DropOut modules by default
     model.eval()
     del original_model
     torch.cuda.empty_cache()
     return model
 
 
+
+def load_text_encoder_for_svdiff(
+        pretrained_model_name_or_path,
+        spectral_shifts_ckpt=None,
+        hf_hub_kwargs=None,
+        **kwargs
+    ):
+    """
+    https://github.com/huggingface/diffusers/blob/v0.14.0/src/diffusers/models/modeling_utils.py#L541
+    """
+    config = CLIPTextConfig.from_pretrained(pretrained_model_name_or_path, **kwargs)
+    original_model = CLIPTextModel.from_pretrained(pretrained_model_name_or_path, **kwargs)
+    state_dict = original_model.state_dict()
+    with accelerate.init_empty_weights():
+        model = CLIPTextModelForSVDiff(config)
+    # load pre-trained weights
+    param_device = "cpu"
+    torch_dtype = kwargs["torch_dtype"] if "torch_dtype" in kwargs else None
+    spectral_shifts_weights = {n: torch.zeros(p.shape) for n, p in model.named_parameters() if "delta" in n}
+    state_dict.update(spectral_shifts_weights)
+    # move the params from meta device to cpu
+    missing_keys = set(model.state_dict().keys()) - set(state_dict.keys())
+    if len(missing_keys) > 0:
+        raise ValueError(
+            f"Cannot load {model.__class__.__name__} from {pretrained_model_name_or_path} because the following keys are"
+            f" missing: \n {', '.join(missing_keys)}. \n Please make sure to pass"
+            " `low_cpu_mem_usage=False` and `device_map=None` if you want to randomely initialize"
+            " those weights or else make sure your checkpoint file is correct."
+        )
+
+    for param_name, param in state_dict.items():
+        accepts_dtype = "dtype" in set(inspect.signature(set_module_tensor_to_device).parameters.keys())
+        if accepts_dtype:
+            set_module_tensor_to_device(model, param_name, param_device, value=param, dtype=torch_dtype)
+        else:
+            set_module_tensor_to_device(model, param_name, param_device, value=param)
+    
+    if spectral_shifts_ckpt:
+        if os.path.isdir(spectral_shifts_ckpt):
+            spectral_shifts_ckpt = os.path.join(spectral_shifts_ckpt, "spectral_shifts_te.safetensors")
+        elif not os.path.exists(spectral_shifts_ckpt):
+            # download from hub
+            hf_hub_kwargs = {} if hf_hub_kwargs is None else hf_hub_kwargs
+            try:
+                spectral_shifts_ckpt = huggingface_hub.hf_hub_download(spectral_shifts_ckpt, filename="spectral_shifts_te.safetensors", **hf_hub_kwargs)
+            except huggingface_hub.utils.EntryNotFoundError:
+                spectral_shifts_ckpt = None
+        # load state dict only if `spectral_shifts_te.safetensors` exists
+        if os.path.exists(spectral_shifts_ckpt):
+            with safe_open(spectral_shifts_ckpt, framework="pt", device="cpu") as f:
+                for key in f.keys():
+                    # spectral_shifts_weights[key] = f.get_tensor(key)
+                    accepts_dtype = "dtype" in set(inspect.signature(set_module_tensor_to_device).parameters.keys())
+                    if accepts_dtype:
+                        set_module_tensor_to_device(model, key, param_device, value=f.get_tensor(key), dtype=torch_dtype)
+                    else:
+                        set_module_tensor_to_device(model, key, param_device, value=f.get_tensor(key))
+            print(f"Resumed from {spectral_shifts_ckpt}")
+        
+    if "torch_dtype"in kwargs:
+        model = model.to(kwargs["torch_dtype"])
+    # model.register_to_config(_name_or_path=pretrained_model_name_or_path)
+    # Set model in evaluation mode to deactivate DropOut modules by default
+    model.eval()
+    del original_model
+    torch.cuda.empty_cache()
+    return model
+
+
 
 def image_grid(imgs, rows, cols):
     assert len(imgs) == rows * cols
     w, h = imgs[0].size
     grid = Image.new('RGB', size=(cols * w, rows * h))
     for i, img in enumerate(imgs):
         grid.paste(img, box=(i % cols * w, i // cols * h))
```

### Comparing `svdiff-pytorch-0.1.1/svdiff_pytorch.egg-info/SOURCES.txt` & `svdiff-pytorch-0.2.0/svdiff_pytorch.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 LICENSE
 README.md
 setup.py
 svdiff_pytorch/__init__.py
 svdiff_pytorch/layers.py
+svdiff_pytorch/pipeline_stable_diffusion_ddim_inversion.py
 svdiff_pytorch/utils.py
 svdiff_pytorch.egg-info/PKG-INFO
 svdiff_pytorch.egg-info/SOURCES.txt
 svdiff_pytorch.egg-info/dependency_links.txt
 svdiff_pytorch.egg-info/requires.txt
 svdiff_pytorch.egg-info/top_level.txt
 svdiff_pytorch/diffusers_models/__init__.py
 svdiff_pytorch/diffusers_models/attention.py
 svdiff_pytorch/diffusers_models/cross_attention.py
 svdiff_pytorch/diffusers_models/dual_transformer_2d.py
 svdiff_pytorch/diffusers_models/embeddings.py
 svdiff_pytorch/diffusers_models/resnet.py
 svdiff_pytorch/diffusers_models/transformer_2d.py
 svdiff_pytorch/diffusers_models/unet_2d_blocks.py
-svdiff_pytorch/diffusers_models/unet_2d_condition.py
+svdiff_pytorch/diffusers_models/unet_2d_condition.py
+svdiff_pytorch/transformers_models_clip/__init__.py
+svdiff_pytorch/transformers_models_clip/modeling_clip.py
```

