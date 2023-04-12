# Comparing `tmp/blip-vit-fork-0.0.2.tar.gz` & `tmp/blip-vit-fork-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blip-vit-fork-0.0.2.tar", last modified: Thu Feb  2 17:46:49 2023, max compression
+gzip compressed data, was "blip-vit-fork-0.0.3.tar", last modified: Wed Apr 12 11:58:05 2023, max compression
```

## Comparing `blip-vit-fork-0.0.2.tar` & `blip-vit-fork-0.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 17:46:49.888690 blip-vit-fork-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-02 17:46:49.888690 blip-vit-fork-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 17:46:49.884690 blip-vit-fork-0.0.2/blip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 17:46:49.888690 blip-vit-fork-0.0.2/blip/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/configs/bert_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/configs/caption_coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/configs/med_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/configs/nlvr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/configs/nocaps.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/configs/pretrain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/configs/retrieval_coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/configs/retrieval_flickr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/configs/retrieval_msrvtt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/configs/vqa.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 17:46:49.888690 blip-vit-fork-0.0.2/blip/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/data/coco_karpathy_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/data/flickr30k_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/data/nlvr_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/data/nocaps_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/data/pretrain_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/data/video_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/data/vqa_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 17:46:49.888690 blip-vit-fork-0.0.2/blip/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/models/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/models/blip_itm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/models/blip_nlvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/models/blip_pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/models/blip_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/models/blip_vqa.py
--rw-r--r--   0 runner    (1001) docker     (123)    41786 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/models/med.py
--rw-r--r--   0 runner    (1001) docker     (123)    36738 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/models/nlvr_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/blip/models/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 17:46:49.888690 blip-vit-fork-0.0.2/blip_vit_fork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-02 17:46:49.000000 blip-vit-fork-0.0.2/blip_vit_fork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-02-02 17:46:49.000000 blip-vit-fork-0.0.2/blip_vit_fork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 17:46:49.000000 blip-vit-fork-0.0.2/blip_vit_fork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-02 17:46:49.000000 blip-vit-fork-0.0.2/blip_vit_fork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-02 17:46:49.000000 blip-vit-fork-0.0.2/blip_vit_fork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/cog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-02 17:46:49.888690 blip-vit-fork-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-02 17:46:37.000000 blip-vit-fork-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:58:05.437614 blip-vit-fork-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 11:58:05.437614 blip-vit-fork-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:58:05.433614 blip-vit-fork-0.0.3/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:58:05.433614 blip-vit-fork-0.0.3/blip/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/configs/bert_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/configs/caption_coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/configs/med_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/configs/nlvr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/configs/nocaps.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/configs/pretrain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/configs/retrieval_coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/configs/retrieval_flickr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/configs/retrieval_msrvtt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/configs/vqa.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:58:05.437614 blip-vit-fork-0.0.3/blip/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/data/coco_karpathy_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/data/flickr30k_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/data/nlvr_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/data/nocaps_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/data/pretrain_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/data/vqa_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:58:05.437614 blip-vit-fork-0.0.3/blip/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/models/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/models/blip_itm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/models/blip_nlvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/models/blip_pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/models/blip_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/models/blip_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41786 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/models/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36738 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/models/nlvr_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/blip/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:58:05.437614 blip-vit-fork-0.0.3/blip_vit_fork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 11:58:05.000000 blip-vit-fork-0.0.3/blip_vit_fork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-12 11:58:05.000000 blip-vit-fork-0.0.3/blip_vit_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:58:05.000000 blip-vit-fork-0.0.3/blip_vit_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 11:58:05.000000 blip-vit-fork-0.0.3/blip_vit_fork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 11:58:05.000000 blip-vit-fork-0.0.3/blip_vit_fork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/cog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 11:58:05.437614 blip-vit-fork-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-12 11:57:55.000000 blip-vit-fork-0.0.3/setup.py
```

### Comparing `blip-vit-fork-0.0.2/LICENSE.txt` & `blip-vit-fork-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/README.md` & `blip-vit-fork-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/configs/caption_coco.yaml` & `blip-vit-fork-0.0.3/blip/configs/caption_coco.yaml`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/configs/retrieval_coco.yaml` & `blip-vit-fork-0.0.3/blip/configs/retrieval_coco.yaml`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/configs/retrieval_flickr.yaml` & `blip-vit-fork-0.0.3/blip/configs/retrieval_flickr.yaml`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/configs/vqa.yaml` & `blip-vit-fork-0.0.3/blip/configs/vqa.yaml`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/data/__init__.py` & `blip-vit-fork-0.0.3/blip/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/data/coco_karpathy_dataset.py` & `blip-vit-fork-0.0.3/blip/data/coco_karpathy_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/data/flickr30k_dataset.py` & `blip-vit-fork-0.0.3/blip/data/flickr30k_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/data/nlvr_dataset.py` & `blip-vit-fork-0.0.3/blip/data/nlvr_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/data/nocaps_dataset.py` & `blip-vit-fork-0.0.3/blip/data/nocaps_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/data/pretrain_dataset.py` & `blip-vit-fork-0.0.3/blip/data/pretrain_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/data/utils.py` & `blip-vit-fork-0.0.3/blip/data/utils.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/data/video_dataset.py` & `blip-vit-fork-0.0.3/blip/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/data/vqa_dataset.py` & `blip-vit-fork-0.0.3/blip/data/vqa_dataset.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/models/blip.py` & `blip-vit-fork-0.0.3/blip/models/blip.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,32 +80,38 @@
                                        return_dict=True,
                                        )
             return output.last_hidden_state
 
 
 class BLIP_Decoder(nn.Module):
     def __init__(self,
-                 med_config='configs/med_config.json',
+                 med_config=None,
                  image_size=384,
                  vit='base',
                  vit_grad_ckpt=False,
                  vit_ckpt_layer=0,
                  prompt='a picture of ',
                  ):
         """
         Args:
             med_config (str): path for the mixture of encoder-decoder model's configuration file
             image_size (int): input image size
             vit (str): model size of vision transformer
         """
         super().__init__()
+
+        if med_config is None: 
+            med_config = os.path.join(
+                os.path.dirname(os.path.dirname(__file__)), "configs", "med_config.json"
+            )
+        if isinstance(med_config, str):
+            med_config = BertConfig.from_json_file(med_config)
         
         self.visual_encoder, vision_width = create_vit(vit, image_size, vit_grad_ckpt, vit_ckpt_layer)
         self.tokenizer = init_tokenizer()
-        med_config = BertConfig.from_json_file(med_config)
         med_config.encoder_width = vision_width
         self.text_decoder = BertLMHeadModel(config=med_config)
         
         self.prompt = prompt
         self.prompt_length = len(self.tokenizer(self.prompt).input_ids) - 1
     
     def forward(self, image, caption):
```

### Comparing `blip-vit-fork-0.0.2/blip/models/blip_itm.py` & `blip-vit-fork-0.0.3/blip/models/blip_itm.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/models/blip_nlvr.py` & `blip-vit-fork-0.0.3/blip/models/blip_nlvr.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/models/blip_pretrain.py` & `blip-vit-fork-0.0.3/blip/models/blip_pretrain.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/models/blip_retrieval.py` & `blip-vit-fork-0.0.3/blip/models/blip_retrieval.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/models/blip_vqa.py` & `blip-vit-fork-0.0.3/blip/models/blip_vqa.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/models/med.py` & `blip-vit-fork-0.0.3/blip/models/med.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/models/nlvr_encoder.py` & `blip-vit-fork-0.0.3/blip/models/nlvr_encoder.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip/models/vit.py` & `blip-vit-fork-0.0.3/blip/models/vit.py`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/blip_vit_fork.egg-info/SOURCES.txt` & `blip-vit-fork-0.0.3/blip_vit_fork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blip-vit-fork-0.0.2/setup.py` & `blip-vit-fork-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 _REQUIREMENTS_TXT = _read_reqs("requirements.txt")
 
 
 setuptools.setup(
     name='blip-vit-fork',
-    version='0.0.2',
+    version='0.0.3',
     install_requires=_REQUIREMENTS_TXT,
     include_package_data=True,
     package_data={'': [
         '*.txt',
         '*.yaml',
         '*.json'
     ]},
```

