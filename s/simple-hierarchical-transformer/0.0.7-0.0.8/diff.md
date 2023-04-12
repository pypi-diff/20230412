# Comparing `tmp/simple-hierarchical-transformer-0.0.7.tar.gz` & `tmp/simple-hierarchical-transformer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-hierarchical-transformer-0.0.7.tar", last modified: Tue Apr 11 19:36:07 2023, max compression
+gzip compressed data, was "simple-hierarchical-transformer-0.0.8.tar", last modified: Wed Apr 12 02:05:23 2023, max compression
```

## Comparing `simple-hierarchical-transformer-0.0.7.tar` & `simple-hierarchical-transformer-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:36:07.599089 simple-hierarchical-transformer-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 19:35:57.000000 simple-hierarchical-transformer-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 19:36:07.595089 simple-hierarchical-transformer-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-11 19:35:57.000000 simple-hierarchical-transformer-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:36:07.599089 simple-hierarchical-transformer-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-11 19:35:57.000000 simple-hierarchical-transformer-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:36:07.595089 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 19:35:57.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-11 19:35:57.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-04-11 19:35:57.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer/simple_hierarchical_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:36:07.595089 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 19:36:07.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 19:36:07.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:36:07.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 19:36:07.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 19:36:07.000000 simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:05:23.357913 simple-hierarchical-transformer-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 02:05:10.000000 simple-hierarchical-transformer-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-12 02:05:23.357913 simple-hierarchical-transformer-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-12 02:05:10.000000 simple-hierarchical-transformer-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 02:05:23.357913 simple-hierarchical-transformer-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-12 02:05:10.000000 simple-hierarchical-transformer-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:05:23.357913 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 02:05:10.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-12 02:05:10.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-04-12 02:05:10.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer/simple_hierarchical_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:05:23.357913 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-12 02:05:23.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-12 02:05:23.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 02:05:23.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 02:05:23.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-12 02:05:23.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/top_level.txt
```

### Comparing `simple-hierarchical-transformer-0.0.7/LICENSE` & `simple-hierarchical-transformer-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.7/PKG-INFO` & `simple-hierarchical-transformer-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simple-hierarchical-transformer-0.0.7/setup.py` & `simple-hierarchical-transformer-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'simple-hierarchical-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.7',
+  version = '0.0.8',
   license='MIT',
   description = 'Simple Hierarchical Transformer',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/simple-hierarchical-transformer',
   keywords = [
```

### Comparing `simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer/attention.py` & `simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer/attention.py`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer/simple_hierarchical_transformer.py` & `simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer/simple_hierarchical_transformer.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,22 +14,30 @@
 
 # constants
 
 mlist = nn.ModuleList
 
 Linear = partial(nn.Linear, bias = False)
 
+LocalMHA = partial(LocalMHA, causal = True, prenorm = True)
+
 # helper functions
 
 def exists(val):
     return val is not None
 
 def is_power_of_two(n):
     return math.log2(n).is_integer()
 
+def all_unique(arr):
+    return len(set(arr)) == len(arr)
+
+def cast_tuple(t, length = 1):
+    return t if isinstance(t, tuple) else ((t,) * length)
+
 def default(*vals):
     for val in vals:
         if exists(val):
             return val
     return None
 
 def eval_decorator(fn):
@@ -152,76 +160,95 @@
     def forward(self, x):
         x = F.pad(x, (self.causal_padding, 0))
         return self.conv(x)
 
 class Compress(nn.Module):
     def __init__(
         self,
+        *,
         dim,
+        num_tokens,
         compress_factor = 2,
         expansion_factor = 4,
         dim_head = 64,
-        heads = 8
+        heads = 8,
+        ignore_index = 0
     ):
         super().__init__()
-        assert compress_factor > 1 and is_power_of_two(compress_factor)
+        assert compress_factor > 0 and is_power_of_two(compress_factor)
 
+        self.no_compress = compress_factor == 1
         self.compress_factor = compress_factor
+
+        if self.no_compress:
+            self.compress_fn = nn.Identity()
+            return
+
         dim_inner = int(dim * expansion_factor)
 
         self.compress_fn = nn.Sequential(
             Rearrange('b n d -> b d n'),
             CausalConv(dim, dim_inner, compress_factor),
             nn.SiLU(),
             nn.Conv1d(dim_inner, dim, 1),
             Rearrange('b d n -> b n d')
         )
 
-    def forward(self, x):
-        batch, factor = x.shape[0], self.compress_factor
+        self.to_recon = Linear(dim, compress_factor * num_tokens)
+        self.ignore_index = ignore_index
 
-        pooled = self.compress_fn(x)
+    def recon(self, h, ids):
 
-        x = rearrange(x, 'b n d -> b d n 1')
-        x = F.pad(x, (0, 0, factor - 1, 0), value = 0.)
-        unfolded = F.unfold(x, (factor, 1))
-        unfolded = rearrange(unfolded, 'b (d c) n -> (b n) c d', c = factor)
+        if self.no_compress:
+            return torch.zeros((), device = h.device).requires_grad_()
 
-        return pooled, unfolded
+        c = self.compress_factor
+        seq_len = ids.shape[-1]
+
+        recon_logits = self.to_recon(h)
+        recon_logits = rearrange(recon_logits, 'b n (c d) -> (b c) d n', c = c)
+
+        recon_ids = F.pad(ids, (c - 1, 0), value = 0)
+        recon_ids = tuple(recon_ids[:, i:(seq_len + i)] for i in range(c))
+        recon_ids = torch.stack(recon_ids, dim = 1)
+        recon_ids = rearrange(recon_ids, 'b c n -> (b c) n')
+
+        recon_loss = F.cross_entropy(recon_logits, recon_ids, ignore_index = self.ignore_index)
+        return recon_loss
+
+    def forward(self, x):
+        return self.compress_fn(x)
 
 class HierarchicalMerge(nn.Module):
     def __init__(
         self,
         dim,
-        num_hierarchies = 2 # 2 for now
+        num_hierarchies = 2
     ):
         super().__init__()
-        self.norm = RMSNorm(dim)
-        self.h_norm = RMSNorm(dim)
+        self.norms = mlist([RMSNorm(dim) for _ in range(num_hierarchies)])
 
         # simple dsconv for now
 
         self.num_hierarchies = num_hierarchies
-
         self.conv = nn.Conv1d(dim, dim, num_hierarchies, stride = num_hierarchies, groups = dim)
 
-    def forward(self, x, h):
+    def forward(self, tokens):
         """
         einops notations:
         b - batch
         h - hierarchies
         n - sequence length
         d - dimension
         """
         nh = self.num_hierarchies
 
-        x = self.norm(x)
-        h = self.h_norm(h)
+        tokens = [norm(h) for norm, h in zip(self.norms, tokens)]
 
-        x = rearrange([x, h], 'h b n d -> b d (n h)')
+        x = rearrange(tokens, 'h b n d -> b d (n h)')
         x = self.conv(x)
         x = rearrange(x, 'b d n -> b n d')
         return x
 
 # classes
 
 class RMSNorm(nn.Module):
@@ -242,16 +269,15 @@
             RMSNorm(dim),
             Linear(dim, dim_inner),
             nn.GELU(),
             Linear(dim_inner, dim)
         )
 
     def forward(self, x):
-        x = self.net(x)
-        return x
+        return self.net(x)
 
 class Attention(nn.Module):
     def __init__(
         self,
         dim,
         dim_head = 64,
         heads = 8,
@@ -259,135 +285,182 @@
     ):
         super().__init__()
         self.scale = dim_head ** -0.5
         self.heads = heads
         dim_inner = dim_head * heads
 
         self.norm = RMSNorm(dim)
+        self.rotary_emb = RotaryEmbedding(dim_head)
+
         self.attend = Attend(causal = True, use_flash_attn = use_flash_attn)
 
         self.to_qkv = Linear(dim, dim_inner * 3)
         self.to_out = Linear(dim_inner, dim)
 
-    def forward(
-        self,
-        x,
-        rotary_emb = None
-    ):
+    def forward(self, x):
         n = x.shape[-2]
         x = self.norm(x)
 
         q, k, v = self.to_qkv(x).chunk(3, dim = -1)
         q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = self.heads), (q, k, v))
 
-        if exists(rotary_emb):
-            q, k = apply_rotary_pos_emb_qk(rotary_emb, q, k)
+        rotary_emb = self.rotary_emb(n)
+        q, k = apply_rotary_pos_emb_qk(rotary_emb, q, k)
 
         out = self.attend(q, k, v)
 
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
 class HierarchicalAttention(nn.Module):
     def __init__(
         self,
         dim,
         dim_head = 64,
         heads = 8,
         window_size = None,
-        compress_factor = 2
+        compress_factor = 1
     ):
         super().__init__()
-        assert compress_factor > 1 and is_power_of_two(compress_factor)
+        assert is_power_of_two(compress_factor)
         self.compress_factor = compress_factor
+        self.no_compress = compress_factor == 1
 
         attn_klass = Attention
+
         if exists(window_size):
-            attn_klass = partial(LocalMHA, window_size = window_size, causal = True, prenorm = True)
+            attn_klass = partial(LocalMHA, window_size = window_size)
 
         self.attn = attn_klass(dim = dim, dim_head = dim_head, heads = heads)
 
     def forward(self, x):
         c = self.compress_factor
         x, orig_seq_len = pad_seq_to_multiple(x, c)
 
         # hierarchical attention is performed with a simple axial attention
 
         # this, and using a convolution for compressing at the beginning
         # is one of the improvements on top of hourglass transformer
         # the downside is that the savings are only O(c) instead of O(c ** 2)
         # but this should provide better learning per-token
 
-        x = rearrange(x, 'b (n c) d -> (b c) n d', c = c)
+        if not self.no_compress:
+            x = rearrange(x, 'b (n c) d -> (b c) n d', c = c)
 
         x = self.attn(x)
 
-        x = rearrange(x, '(b c) n d -> b (n c) d', c = c)
+        if not self.no_compress:
+            x = rearrange(x, '(b c) n d -> b (n c) d', c = c)
 
         return x[:, :orig_seq_len]
 
 class HierarchicalTransformer(nn.Module):
     def __init__(
         self,
         *,
         num_tokens,
         dim,
         depth,
         seq_len = 2048,
         dim_head = 64,
         heads = 8,
         ff_mult = 4,
-        use_flash_attn = False,
+        hierarchies = 1,
+        predict_hierarchy = None,
+        window_sizes = None,
         ignore_index = 0,
-        compress_factor = 1,
         recon_loss_weight = 0.1,
-        hierarchical_window_size = 64,
-        fine_window_size = 64
+        use_flash_attn = False
     ):
         super().__init__()
-        assert is_power_of_two(compress_factor)
-
         self.seq_len = seq_len
-        self.ignore_index = ignore_index
 
         self.token_emb = nn.Embedding(num_tokens, dim)
-
         self.post_token_emb_norm = RMSNorm(dim)
 
-        should_compress = compress_factor > 1
+        hierarchies = tuple(sorted(cast_tuple(hierarchies)))
 
-        self.compress_factor = compress_factor
-        self.compress = None
+        assert all_unique(hierarchies), 'hierarchies compression factors must be all unique integers'
+        assert all([*map(is_power_of_two, hierarchies)]), 'only powers of two allowed for hierarchies'
 
-        if should_compress:
-            self.compress = Compress(
-                dim,
-                compress_factor = compress_factor
-            )
+        num_hierarchies = len(hierarchies)
+        predict_hierarchy = default(predict_hierarchy, min(hierarchies))
 
-        self.recon_loss_weight = recon_loss_weight
+        self.predict_hierarchy_index = hierarchies.index(predict_hierarchy)
+
+        window_sizes = cast_tuple(window_sizes, num_hierarchies)
+        assert len(window_sizes) == len(hierarchies)
+
+        # hierarchy compressions - 1x just uses the base token_emb weights
+
+        self.compressors = mlist([])
+
+        for hierarchy in hierarchies:
+            self.compressors.append(Compress(
+                dim = dim,
+                num_tokens = num_tokens,
+                compress_factor = hierarchy,
+            ))
+
+        # layers
 
         self.layers = mlist([])
+        self.hierarchical_merges = mlist([])
 
         local_attn = partial(LocalMHA, causal = True, prenorm = True)
 
         for _ in range(depth):
+            hierarchical_layer = mlist([])
 
-            self.layers.append(mlist([
-                HierarchicalAttention(dim = dim, dim_head = dim_head, heads = heads, window_size = hierarchical_window_size, compress_factor = compress_factor),
-                FeedForward(dim = dim, mult = ff_mult),
-                local_attn(dim = dim, dim_head = dim_head, heads = heads, window_size = fine_window_size),
-                FeedForward(dim = dim, mult = ff_mult),
-                HierarchicalMerge(dim = dim)
-            ]))
+            # add a transformer block for each layer in the hierarchy
 
-        self.norm = RMSNorm(dim)
+            for hierarchy, window_size in zip(hierarchies, window_sizes):
+
+                # make sure the window size never exceeds the effective sequence length
+
+                effective_seq_len = seq_len // hierarchy
+
+                if exists(window_size) and window_size > effective_seq_len:
+                    print(f'window size for hierarchy {hierarchy}x is greater than effective sequence length - setting window size to None (which would use normal full attention)')
+                    window_size = None
+
+                # add attention and feedforward
+
+                hierarchical_layer.append(mlist([
+                    HierarchicalAttention(
+                        dim = dim,
+                        dim_head = dim_head,
+                        heads = heads,
+                        window_size = window_size,
+                        compress_factor = hierarchy
+                    ),
+                    FeedForward(dim = dim, mult = ff_mult)
+                ]))
+
+            self.layers.append(hierarchical_layer)
+
+            # for merging the information across hierarchies
+            # for now, only one direction, from all hierarchies to the hierarchy that is being used to make predictions on, set by predict_hierarchy_index above
+
+            merge = HierarchicalMerge(dim = dim, num_hierarchies = num_hierarchies)
+
+            self.hierarchical_merges.append(merge)
+
+        # final post-transformer norms, for all hierarchies
+
+        self.norms = mlist([RMSNorm(dim) for _ in range(num_hierarchies)])
+
+        # to logit, for hierarchy set at predict_hierarchy_index
 
         self.to_logits = Linear(dim, num_tokens)
-        self.to_recon = Linear(dim, compress_factor * num_tokens) if should_compress else None
+
+        # training related loss parameters
+
+        self.ignore_index = ignore_index
+        self.recon_loss_weight = recon_loss_weight
 
     @torch.no_grad()
     @eval_decorator
     def generate(
         self,
         prompt,
         seq_len,
@@ -422,74 +495,86 @@
 
         b - batch
         n - sequence length
         c - compression factor
         d - dimension
         """
 
-        # whether to compress or not
-
-        c = self.compress_factor
-        should_compress = c > 1
-
         # if training, predict next token in sequence
 
         if return_loss:
             ids, labels = ids[:, :-1], ids[:, 1:]
 
-        seq_len = ids.shape[-1]
+        # assert seq len
+
+        assert ids.shape[-1] <= self.seq_len
 
         # get token embeddings, and pad to multiple of compression factor
 
         x = self.token_emb(ids)
 
         # post embedding norm
 
         x = self.post_token_emb_norm(x)
 
-        # compress to hierarchical tokens from the beginning
+        # for every hierarchy, compress token embeddings appropriately to the hierarchical embeddings
+
+        tokens = []
 
-        h = x
-        if exists(self.compress):
-            h, uncompressed = self.compress(x)
+        for compress in self.compressors:
+            tokens.append(compress(x))
 
         # layers
 
-        for h_local_attn, h_ff, local_attn, ff, h_merge in self.layers:
+        for layer, merge in zip(self.layers, self.hierarchical_merges):
+
+            next_tokens = []
+
+            for (attn, ff), h in zip(layer, tokens):
+                h = attn(h) + h
+                h = ff(token_shift(h)) + h
+
+                next_tokens.append(h)
 
-            h = h_local_attn(h) + h
-            h = h_ff(token_shift(h)) + h
+            tokens = next_tokens
 
-            x = local_attn(x) + x
-            x = ff(token_shift(x)) + x
+            # pool the information all hierarchies
+            # and then update the tokens that will be used to make the final autoregressive prediction
 
-            x = h_merge(x, h) + x
+            pooled = merge(tokens)
+            predict_tokens = tokens[self.predict_hierarchy_index]
+            predict_tokens = predict_tokens + pooled
+            tokens[self.predict_hierarchy_index] = predict_tokens
 
         # final norm and logits
 
-        x = self.norm(x)
+        tokens = [norm(t) for norm, t in zip(self.norms, tokens)]
+
+        # select the hierarchical embeddings that will be doing the predicting
+
+        predict_embed = tokens[self.predict_hierarchy_index]
 
-        logits = self.to_logits(x)
+        # logits for predicting next token
+
+        logits = self.to_logits(predict_embed)
 
         if not return_loss:
             return logits
 
-        ce = partial(F.cross_entropy, ignore_index = self.ignore_index)
+        # autoregressive loss (predictive coding)
+
+        logits = rearrange(logits, 'b n c -> b c n')
+        ce_loss = F.cross_entropy(logits, labels, ignore_index = self.ignore_index)
 
         # reconstruction losses for hierarchy tokens -> may remove if see no benefit, which seems to be leaning that way
 
-        recon_loss = torch.zeros((), device = self.device)
-        if should_compress:
-            recon_logits = self.to_recon(h)
-            recon_logits = rearrange(recon_logits, 'b n (c d) -> (b c) d n', c = c)
-
-            recon_ids = F.pad(ids, (c - 1, 0), value = 0)
-            recon_ids = tuple(recon_ids[:, i:(seq_len + i)] for i in range(c))
-            recon_ids = torch.stack(recon_ids, dim = 1)
-            recon_ids = rearrange(recon_ids, 'b c n -> (b c) n')
-            recon_loss = ce(recon_logits, recon_ids)
+        recon_losses = 0
 
-        logits = rearrange(logits, 'b n c -> b c n')
-        ce_loss = ce(logits, labels)
+        for compress, t in zip(self.compressors, tokens):
+            recon_loss = compress.recon(t, ids)
+            recon_losses = recon_losses + recon_loss
+
+        # total loss
 
         total_loss = ce_loss + recon_loss * self.recon_loss_weight
+
         return total_loss, (ce_loss, recon_loss)
```

### Comparing `simple-hierarchical-transformer-0.0.7/simple_hierarchical_transformer.egg-info/PKG-INFO` & `simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

