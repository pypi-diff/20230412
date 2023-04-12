# Comparing `tmp/xs_transformers-1.0.5-py3-none-any.whl.zip` & `tmp/xs_transformers-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5512842 bytes, number of entries: 997
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-12 06:11 xs_transformers/__init__.py
+Zip file size: 5512849 bytes, number of entries: 997
+-rw-rw-r--  2.0 unx       16 b- defN 23-Apr-12 06:13 xs_transformers/__init__.py
 -rw-rw-r--  2.0 unx     6812 b- defN 23-Apr-12 06:10 xs_transformers/activations.py
 -rw-rw-r--  2.0 unx     4335 b- defN 23-Apr-12 06:10 xs_transformers/activations_tf.py
 -rw-rw-r--  2.0 unx    49246 b- defN 23-Apr-12 06:10 xs_transformers/configuration_utils.py
 -rw-rw-r--  2.0 unx    21413 b- defN 23-Apr-12 06:10 xs_transformers/convert_graph_to_onnx.py
 -rw-rw-r--  2.0 unx    17091 b- defN 23-Apr-12 06:10 xs_transformers/convert_pytorch_checkpoint_to_tf2.py
 -rw-rw-r--  2.0 unx    47424 b- defN 23-Apr-12 06:10 xs_transformers/convert_slow_tokenizer.py
 -rw-rw-r--  2.0 unx     5351 b- defN 23-Apr-12 06:10 xs_transformers/convert_slow_tokenizers_checkpoints_to_fast.py
@@ -988,12 +988,12 @@
 -rw-rw-r--  2.0 unx    48418 b- defN 23-Apr-12 06:10 xs_transformers/utils/hub.py
 -rw-rw-r--  2.0 unx    39864 b- defN 23-Apr-12 06:10 xs_transformers/utils/import_utils.py
 -rw-rw-r--  2.0 unx     9659 b- defN 23-Apr-12 06:10 xs_transformers/utils/logging.py
 -rw-rw-r--  2.0 unx     2302 b- defN 23-Apr-12 06:10 xs_transformers/utils/model_parallel_utils.py
 -rw-rw-r--  2.0 unx    15195 b- defN 23-Apr-12 06:10 xs_transformers/utils/notebook.py
 -rw-rw-r--  2.0 unx    50691 b- defN 23-Apr-12 06:10 xs_transformers/utils/sentencepiece_model_pb2.py
 -rw-rw-r--  2.0 unx     4555 b- defN 23-Apr-12 06:10 xs_transformers/utils/versions.py
--rw-rw-r--  2.0 unx      187 b- defN 23-Apr-12 06:11 xs_transformers-1.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 06:11 xs_transformers-1.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Apr-12 06:11 xs_transformers-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx   110566 b- defN 23-Apr-12 06:11 xs_transformers-1.0.5.dist-info/RECORD
-997 files, 25037918 bytes uncompressed, 5330530 bytes compressed:  78.7%
+-rw-rw-r--  2.0 unx      187 b- defN 23-Apr-12 06:13 xs_transformers-1.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 06:13 xs_transformers-1.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Apr-12 06:13 xs_transformers-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx   110567 b- defN 23-Apr-12 06:13 xs_transformers-1.0.6.dist-info/RECORD
+997 files, 25037926 bytes uncompressed, 5330537 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -2973,20 +2973,20 @@
 
 Filename: xs_transformers/utils/sentencepiece_model_pb2.py
 Comment: 
 
 Filename: xs_transformers/utils/versions.py
 Comment: 
 
-Filename: xs_transformers-1.0.5.dist-info/METADATA
+Filename: xs_transformers-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: xs_transformers-1.0.5.dist-info/WHEEL
+Filename: xs_transformers-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: xs_transformers-1.0.5.dist-info/top_level.txt
+Filename: xs_transformers-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xs_transformers-1.0.5.dist-info/RECORD
+Filename: xs_transformers-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xs_transformers/__init__.py

```diff
@@ -1 +1 @@
-import *
+from . import *
```

## Comparing `xs_transformers-1.0.5.dist-info/RECORD` & `xs_transformers-1.0.6.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-xs_transformers/__init__.py,sha256=sTq3cIex3PUw4ljaF8WnKqGX193qhIZ1qgD_uJWHc8Y,9
+xs_transformers/__init__.py,sha256=Il5Q9ATdX8yXqVxtP_nYqUhExzxPC_qk_WXQ_4h0exg,16
 xs_transformers/activations.py,sha256=mgbgtQrRDNytgZWQ6cU9eVZIspgiJpdMQBbo8YUO8MI,6812
 xs_transformers/activations_tf.py,sha256=4N5QTqb7cDzBU91ws9s4vksN0JqMRhETIUPdOn4oy7I,4335
 xs_transformers/configuration_utils.py,sha256=FEfETyni6wafz-aPR9K85G57X3EhSPYgDGma6eknVA8,49246
 xs_transformers/convert_graph_to_onnx.py,sha256=Djz3K_kv43MA08US54VIQD-Al3xwIwmUoXxjzjVoiMg,21413
 xs_transformers/convert_pytorch_checkpoint_to_tf2.py,sha256=JwsaQrrgiMkZg-Fb0gzBMhS1A-AKLj4vt_DW2K8y7ew,17091
 xs_transformers/convert_slow_tokenizer.py,sha256=_GIwXon-YH9JNT8OVahDnlmd0gZTw9nKuzo3R0j3PGA,47424
 xs_transformers/convert_slow_tokenizers_checkpoints_to_fast.py,sha256=Qq1TEapuc_biLXS7kmu0tAFlzIfezbviUsHkNkNe0x8,5351
@@ -987,11 +987,11 @@
 xs_transformers/utils/hub.py,sha256=TIFBG6iqatKDl6PkRnuA4yPtqV09ABXkZpwJEHkLwNE,48418
 xs_transformers/utils/import_utils.py,sha256=3ts7ajPYq6Np5tPl3ED-NjSMHnlvfZSP1tK15F-Z28Y,39864
 xs_transformers/utils/logging.py,sha256=bEdFOlEVY8-Cmz5IweOQZyZJCjRmHlZYplP9-I9zUOU,9659
 xs_transformers/utils/model_parallel_utils.py,sha256=hkGwAWnCq2pe5ZVAmuolLMAgyg82vJ0fRjvLai_jRZ4,2302
 xs_transformers/utils/notebook.py,sha256=Qq36tiFrOkeC3xqMOOfBuiOzejYgTRmagtWcBHzgu90,15195
 xs_transformers/utils/sentencepiece_model_pb2.py,sha256=ElK3eT5vwvUs1-YseCPIxCIHNToaaJm-BW_fK974bMc,50691
 xs_transformers/utils/versions.py,sha256=9-fs315vSGtSOdqqnNnXGxRhiqnJd1hdqsdLuPtKda8,4555
-xs_transformers-1.0.5.dist-info/METADATA,sha256=-MyltUvpkUKMyci4tCZjoHYetHSjTPTILrzycfSO3sE,187
-xs_transformers-1.0.5.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-xs_transformers-1.0.5.dist-info/top_level.txt,sha256=GbvsOoxLuzRiLg-y8sBDCUlUwUuZH1dbwGhzP_PdksA,16
-xs_transformers-1.0.5.dist-info/RECORD,,
+xs_transformers-1.0.6.dist-info/METADATA,sha256=LAFvSdBGkWPD6qJiYc9C0Ll-xiVLfIz-tdA_K0qL2_8,187
+xs_transformers-1.0.6.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+xs_transformers-1.0.6.dist-info/top_level.txt,sha256=GbvsOoxLuzRiLg-y8sBDCUlUwUuZH1dbwGhzP_PdksA,16
+xs_transformers-1.0.6.dist-info/RECORD,,
```

