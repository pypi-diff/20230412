# Comparing `tmp/hcpdiff-0.1.3.tar.gz` & `tmp/hcpdiff-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcpdiff-0.1.3.tar", last modified: Wed Apr 12 07:54:34 2023, max compression
+gzip compressed data, was "hcpdiff-0.1.4.tar", last modified: Wed Apr 12 08:19:41 2023, max compression
```

## Comparing `hcpdiff-0.1.3.tar` & `hcpdiff-0.1.4.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:34.417190 hcpdiff-0.1.3/
--rw-rw-rw-   0        0        0    11558 2023-04-11 12:44:40.000000 hcpdiff-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     4041 2023-04-12 07:54:34.416182 hcpdiff-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3304 2023-04-12 06:39:19.000000 hcpdiff-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:34.369891 hcpdiff-0.1.3/cfgs/
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:34.371904 hcpdiff-0.1.3/cfgs/infer/
--rw-rw-rw-   0        0        0      179 2023-04-11 09:59:00.000000 hcpdiff-0.1.3/cfgs/infer/change_vae.yaml
--rw-rw-rw-   0        0        0      651 2023-04-11 09:59:00.000000 hcpdiff-0.1.3/cfgs/infer/euler_a.yaml
--rw-rw-rw-   0        0        0     1413 2023-04-11 09:59:00.000000 hcpdiff-0.1.3/cfgs/infer/v1.yaml
--rw-rw-rw-   0        0        0     9971 2023-03-22 01:36:55.000000 hcpdiff-0.1.3/cfgs/te_struct.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:34.373904 hcpdiff-0.1.3/cfgs/train/
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:34.379896 hcpdiff-0.1.3/cfgs/train/examples/
--rw-rw-rw-   0        0        0     1846 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/cfgs/train/examples/CustomDiffusion.yaml
--rw-rw-rw-   0        0        0     2680 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/cfgs/train/examples/DreamArtist++.yaml
--rw-rw-rw-   0        0        0     1334 2023-04-12 06:39:19.000000 hcpdiff-0.1.3/cfgs/train/examples/DreamArtist.yaml
--rw-rw-rw-   0        0        0     1644 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/cfgs/train/examples/DreamBooth.yaml
--rw-rw-rw-   0        0        0     1124 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/cfgs/train/examples/TextualInversion.yaml
--rw-rw-rw-   0        0        0     1178 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/cfgs/train/examples/fine-tuning.yaml
--rw-rw-rw-   0        0        0     1397 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/cfgs/train/examples/locon.yaml
--rw-rw-rw-   0        0        0     1228 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/cfgs/train/examples/lora_conventional.yaml
--rw-rw-rw-   0        0        0     2904 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/cfgs/train/train_base.yaml
--rw-rw-rw-   0        0        0      987 2023-04-11 08:41:31.000000 hcpdiff-0.1.3/cfgs/train/tuning_base.yaml
--rw-rw-rw-   0        0        0    46121 2023-03-22 01:36:55.000000 hcpdiff-0.1.3/cfgs/unet_struct.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:34.383904 hcpdiff-0.1.3/hcpdiff/
--rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:34.392116 hcpdiff-0.1.3/hcpdiff/data/
--rw-rw-rw-   0        0        0      138 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/data/__init__.py
--rw-rw-rw-   0        0        0     8678 2023-04-11 12:47:28.000000 hcpdiff-0.1.3/hcpdiff/data/bucket.py
--rw-rw-rw-   0        0        0     5678 2023-04-12 06:39:19.000000 hcpdiff-0.1.3/hcpdiff/data/pair_dataset.py
--rw-rw-rw-   0        0        0     1686 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:34.399115 hcpdiff-0.1.3/hcpdiff/models/
--rw-rw-rw-   0        0        0      290 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/models/__init__.py
--rw-rw-rw-   0        0        0     1422 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/models/cfg_context.py
--rw-rw-rw-   0        0        0     3068 2023-04-11 12:47:28.000000 hcpdiff-0.1.3/hcpdiff/models/layers.py
--rw-rw-rw-   0        0        0     7732 2023-04-11 12:47:28.000000 hcpdiff-0.1.3/hcpdiff/models/lora.py
--rw-rw-rw-   0        0        0     7065 2023-04-11 12:47:28.000000 hcpdiff-0.1.3/hcpdiff/models/lora_layers.py
--rw-rw-rw-   0        0        0     4678 2023-04-11 12:47:28.000000 hcpdiff-0.1.3/hcpdiff/models/plugin.py
--rw-rw-rw-   0        0        0     3582 2023-04-11 12:47:28.000000 hcpdiff-0.1.3/hcpdiff/models/text_emb_ex.py
--rw-rw-rw-   0        0        0     5507 2023-04-11 12:47:28.000000 hcpdiff-0.1.3/hcpdiff/models/textencoder_ex.py
--rw-rw-rw-   0        0        0     2360 2023-04-11 12:47:28.000000 hcpdiff-0.1.3/hcpdiff/models/tokenizer_ex.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:34.403108 hcpdiff-0.1.3/hcpdiff/tools/
--rw-rw-rw-   0        0        0        0 2023-04-12 06:39:19.000000 hcpdiff-0.1.3/hcpdiff/tools/__init__.py
--rw-rw-rw-   0        0        0     1981 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/tools/create_embedding.py
--rw-rw-rw-   0        0        0     1718 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/tools/gen_from_ptlist.py
--rw-rw-rw-   0        0        0      654 2023-04-12 07:50:43.000000 hcpdiff-0.1.3/hcpdiff/tools/init_proj.py
--rw-rw-rw-   0        0        0     4585 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/tools/merge_model_part.py
--rw-rw-rw-   0        0        0    23465 2023-04-11 12:47:28.000000 hcpdiff-0.1.3/hcpdiff/train_ac.py
--rw-rw-rw-   0        0        0     1827 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/train_ac_single.py
--rw-rw-rw-   0        0        0     9171 2023-04-11 12:47:28.000000 hcpdiff-0.1.3/hcpdiff/train_colo.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:34.409115 hcpdiff-0.1.3/hcpdiff/utils/
--rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/utils/__init__.py
--rw-rw-rw-   0        0        0     2865 2023-04-12 06:39:19.000000 hcpdiff-0.1.3/hcpdiff/utils/caption_tools.py
--rw-rw-rw-   0        0        0     7789 2023-04-11 12:47:28.000000 hcpdiff-0.1.3/hcpdiff/utils/cfg_net_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:34.411107 hcpdiff-0.1.3/hcpdiff/utils/ckpt_manager/
--rw-rw-rw-   0        0        0       82 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/utils/ckpt_manager/__init__.py
--rw-rw-rw-   0        0        0     2390 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/utils/ckpt_manager/ckpt_pkl.py
--rw-rw-rw-   0        0        0     1833 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py
--rw-rw-rw-   0        0        0      860 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/utils/colo_utils.py
--rw-rw-rw-   0        0        0     3065 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/utils/ema.py
--rw-rw-rw-   0        0        0      448 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/utils/emb_utils.py
--rw-rw-rw-   0        0        0     8680 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/utils/img_size_tool.py
--rw-rw-rw-   0        0        0     6623 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/utils/utils.py
--rw-rw-rw-   0        0        0     4215 2023-04-11 12:30:15.000000 hcpdiff-0.1.3/hcpdiff/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:34.388115 hcpdiff-0.1.3/hcpdiff.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-04-12 07:54:34.000000 hcpdiff-0.1.3/hcpdiff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1863 2023-04-12 07:54:34.000000 hcpdiff-0.1.3/hcpdiff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 07:54:34.000000 hcpdiff-0.1.3/hcpdiff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-04-12 07:54:34.000000 hcpdiff-0.1.3/hcpdiff.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      225 2023-04-12 07:54:34.000000 hcpdiff-0.1.3/hcpdiff.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 07:54:34.000000 hcpdiff-0.1.3/hcpdiff.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 07:54:34.416182 hcpdiff-0.1.3/prompt_tuning_template/
--rw-rw-rw-   0        0        0       14 2023-04-03 03:15:56.000000 hcpdiff-0.1.3/prompt_tuning_template/caption.txt
--rw-rw-rw-   0        0        0       14 2023-02-21 02:34:54.000000 hcpdiff-0.1.3/prompt_tuning_template/name.txt
--rw-rw-rw-   0        0        0       55 2023-02-21 02:36:10.000000 hcpdiff-0.1.3/prompt_tuning_template/name_2pt_caption.txt
--rw-rw-rw-   0        0        0       25 2023-03-22 03:52:13.000000 hcpdiff-0.1.3/prompt_tuning_template/name_caption.txt
--rw-rw-rw-   0        0        0      915 2023-04-02 01:48:02.000000 hcpdiff-0.1.3/prompt_tuning_template/object.txt
--rw-rw-rw-   0        0        0      890 2023-04-11 08:41:31.000000 hcpdiff-0.1.3/prompt_tuning_template/style.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 07:54:34.417190 hcpdiff-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1833 2023-04-12 07:54:32.000000 hcpdiff-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:19:41.823330 hcpdiff-0.1.4/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 12:44:40.000000 hcpdiff-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     4041 2023-04-12 08:19:41.822321 hcpdiff-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3304 2023-04-12 06:39:19.000000 hcpdiff-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 08:19:41.773590 hcpdiff-0.1.4/cfgs/
+drwxrwxrwx   0        0        0        0 2023-04-12 08:19:41.776691 hcpdiff-0.1.4/cfgs/infer/
+-rw-rw-rw-   0        0        0      179 2023-04-11 09:59:00.000000 hcpdiff-0.1.4/cfgs/infer/change_vae.yaml
+-rw-rw-rw-   0        0        0      651 2023-04-11 09:59:00.000000 hcpdiff-0.1.4/cfgs/infer/euler_a.yaml
+-rw-rw-rw-   0        0        0     1413 2023-04-11 09:59:00.000000 hcpdiff-0.1.4/cfgs/infer/v1.yaml
+-rw-rw-rw-   0        0        0     9971 2023-03-22 01:36:55.000000 hcpdiff-0.1.4/cfgs/te_struct.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 08:19:41.778705 hcpdiff-0.1.4/cfgs/train/
+drwxrwxrwx   0        0        0        0 2023-04-12 08:19:41.784699 hcpdiff-0.1.4/cfgs/train/examples/
+-rw-rw-rw-   0        0        0     1846 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/cfgs/train/examples/CustomDiffusion.yaml
+-rw-rw-rw-   0        0        0     2680 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/cfgs/train/examples/DreamArtist++.yaml
+-rw-rw-rw-   0        0        0     1334 2023-04-12 06:39:19.000000 hcpdiff-0.1.4/cfgs/train/examples/DreamArtist.yaml
+-rw-rw-rw-   0        0        0     1644 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/cfgs/train/examples/DreamBooth.yaml
+-rw-rw-rw-   0        0        0     1124 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/cfgs/train/examples/TextualInversion.yaml
+-rw-rw-rw-   0        0        0     1178 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/cfgs/train/examples/fine-tuning.yaml
+-rw-rw-rw-   0        0        0     1397 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/cfgs/train/examples/locon.yaml
+-rw-rw-rw-   0        0        0     1228 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/cfgs/train/examples/lora_conventional.yaml
+-rw-rw-rw-   0        0        0     2904 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/cfgs/train/train_base.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-11 08:41:31.000000 hcpdiff-0.1.4/cfgs/train/tuning_base.yaml
+-rw-rw-rw-   0        0        0    46121 2023-03-22 01:36:55.000000 hcpdiff-0.1.4/cfgs/unet_struct.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 08:19:41.788699 hcpdiff-0.1.4/hcpdiff/
+-rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:19:41.796145 hcpdiff-0.1.4/hcpdiff/data/
+-rw-rw-rw-   0        0        0      138 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/data/__init__.py
+-rw-rw-rw-   0        0        0     8678 2023-04-11 12:47:28.000000 hcpdiff-0.1.4/hcpdiff/data/bucket.py
+-rw-rw-rw-   0        0        0     5678 2023-04-12 06:39:19.000000 hcpdiff-0.1.4/hcpdiff/data/pair_dataset.py
+-rw-rw-rw-   0        0        0     1686 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:19:41.803153 hcpdiff-0.1.4/hcpdiff/models/
+-rw-rw-rw-   0        0        0      290 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/models/__init__.py
+-rw-rw-rw-   0        0        0     1422 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/models/cfg_context.py
+-rw-rw-rw-   0        0        0     3068 2023-04-11 12:47:28.000000 hcpdiff-0.1.4/hcpdiff/models/layers.py
+-rw-rw-rw-   0        0        0     7732 2023-04-11 12:47:28.000000 hcpdiff-0.1.4/hcpdiff/models/lora.py
+-rw-rw-rw-   0        0        0     7065 2023-04-11 12:47:28.000000 hcpdiff-0.1.4/hcpdiff/models/lora_layers.py
+-rw-rw-rw-   0        0        0     4678 2023-04-11 12:47:28.000000 hcpdiff-0.1.4/hcpdiff/models/plugin.py
+-rw-rw-rw-   0        0        0     3582 2023-04-11 12:47:28.000000 hcpdiff-0.1.4/hcpdiff/models/text_emb_ex.py
+-rw-rw-rw-   0        0        0     5507 2023-04-11 12:47:28.000000 hcpdiff-0.1.4/hcpdiff/models/textencoder_ex.py
+-rw-rw-rw-   0        0        0     2360 2023-04-11 12:47:28.000000 hcpdiff-0.1.4/hcpdiff/models/tokenizer_ex.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:19:41.808153 hcpdiff-0.1.4/hcpdiff/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-12 06:39:19.000000 hcpdiff-0.1.4/hcpdiff/tools/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-04-12 08:16:29.000000 hcpdiff-0.1.4/hcpdiff/tools/convert_caption_txt2json.py
+-rw-rw-rw-   0        0        0     1981 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/tools/create_embedding.py
+-rw-rw-rw-   0        0        0     1718 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/tools/gen_from_ptlist.py
+-rw-rw-rw-   0        0        0      654 2023-04-12 07:55:01.000000 hcpdiff-0.1.4/hcpdiff/tools/init_proj.py
+-rw-rw-rw-   0        0        0     4585 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/tools/merge_model_part.py
+-rw-rw-rw-   0        0        0    23465 2023-04-11 12:47:28.000000 hcpdiff-0.1.4/hcpdiff/train_ac.py
+-rw-rw-rw-   0        0        0     1827 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/train_ac_single.py
+-rw-rw-rw-   0        0        0     9171 2023-04-11 12:47:28.000000 hcpdiff-0.1.4/hcpdiff/train_colo.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:19:41.814146 hcpdiff-0.1.4/hcpdiff/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/utils/__init__.py
+-rw-rw-rw-   0        0        0     2865 2023-04-12 06:39:19.000000 hcpdiff-0.1.4/hcpdiff/utils/caption_tools.py
+-rw-rw-rw-   0        0        0     7789 2023-04-11 12:47:28.000000 hcpdiff-0.1.4/hcpdiff/utils/cfg_net_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:19:41.817145 hcpdiff-0.1.4/hcpdiff/utils/ckpt_manager/
+-rw-rw-rw-   0        0        0       82 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/utils/ckpt_manager/__init__.py
+-rw-rw-rw-   0        0        0     2390 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/utils/ckpt_manager/ckpt_pkl.py
+-rw-rw-rw-   0        0        0     1833 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py
+-rw-rw-rw-   0        0        0      860 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/utils/colo_utils.py
+-rw-rw-rw-   0        0        0     3065 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/utils/ema.py
+-rw-rw-rw-   0        0        0      448 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/utils/emb_utils.py
+-rw-rw-rw-   0        0        0     8680 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/utils/img_size_tool.py
+-rw-rw-rw-   0        0        0     6623 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/utils/utils.py
+-rw-rw-rw-   0        0        0     4215 2023-04-11 12:30:15.000000 hcpdiff-0.1.4/hcpdiff/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:19:41.793145 hcpdiff-0.1.4/hcpdiff.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-04-12 08:19:41.000000 hcpdiff-0.1.4/hcpdiff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1905 2023-04-12 08:19:41.000000 hcpdiff-0.1.4/hcpdiff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 08:19:41.000000 hcpdiff-0.1.4/hcpdiff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-04-12 08:19:41.000000 hcpdiff-0.1.4/hcpdiff.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      225 2023-04-12 08:19:41.000000 hcpdiff-0.1.4/hcpdiff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-12 08:19:41.000000 hcpdiff-0.1.4/hcpdiff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 08:19:41.821321 hcpdiff-0.1.4/prompt_tuning_template/
+-rw-rw-rw-   0        0        0       14 2023-04-03 03:15:56.000000 hcpdiff-0.1.4/prompt_tuning_template/caption.txt
+-rw-rw-rw-   0        0        0       14 2023-02-21 02:34:54.000000 hcpdiff-0.1.4/prompt_tuning_template/name.txt
+-rw-rw-rw-   0        0        0       55 2023-02-21 02:36:10.000000 hcpdiff-0.1.4/prompt_tuning_template/name_2pt_caption.txt
+-rw-rw-rw-   0        0        0       25 2023-03-22 03:52:13.000000 hcpdiff-0.1.4/prompt_tuning_template/name_caption.txt
+-rw-rw-rw-   0        0        0      915 2023-04-02 01:48:02.000000 hcpdiff-0.1.4/prompt_tuning_template/object.txt
+-rw-rw-rw-   0        0        0      890 2023-04-11 08:41:31.000000 hcpdiff-0.1.4/prompt_tuning_template/style.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 08:19:41.823330 hcpdiff-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1833 2023-04-12 08:19:39.000000 hcpdiff-0.1.4/setup.py
```

### Comparing `hcpdiff-0.1.3/LICENSE` & `hcpdiff-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/PKG-INFO` & `hcpdiff-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.1.3
+Version: 0.1.4
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hcpdiff-0.1.3/README.md` & `hcpdiff-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/infer/euler_a.yaml` & `hcpdiff-0.1.4/cfgs/infer/euler_a.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/infer/v1.yaml` & `hcpdiff-0.1.4/cfgs/infer/v1.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/te_struct.txt` & `hcpdiff-0.1.4/cfgs/te_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/train/examples/CustomDiffusion.yaml` & `hcpdiff-0.1.4/cfgs/train/examples/CustomDiffusion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/train/examples/DreamArtist++.yaml` & `hcpdiff-0.1.4/cfgs/train/examples/DreamArtist++.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/train/examples/DreamArtist.yaml` & `hcpdiff-0.1.4/cfgs/train/examples/DreamArtist.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/train/examples/DreamBooth.yaml` & `hcpdiff-0.1.4/cfgs/train/examples/DreamBooth.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/train/examples/TextualInversion.yaml` & `hcpdiff-0.1.4/cfgs/train/examples/TextualInversion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/train/examples/fine-tuning.yaml` & `hcpdiff-0.1.4/cfgs/train/examples/fine-tuning.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/train/examples/locon.yaml` & `hcpdiff-0.1.4/cfgs/train/examples/locon.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/train/examples/lora_conventional.yaml` & `hcpdiff-0.1.4/cfgs/train/examples/lora_conventional.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/train/train_base.yaml` & `hcpdiff-0.1.4/cfgs/train/train_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/train/tuning_base.yaml` & `hcpdiff-0.1.4/cfgs/train/tuning_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/cfgs/unet_struct.txt` & `hcpdiff-0.1.4/cfgs/unet_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/data/bucket.py` & `hcpdiff-0.1.4/hcpdiff/data/bucket.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/data/pair_dataset.py` & `hcpdiff-0.1.4/hcpdiff/data/pair_dataset.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/data/utils.py` & `hcpdiff-0.1.4/hcpdiff/data/utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/models/cfg_context.py` & `hcpdiff-0.1.4/hcpdiff/models/cfg_context.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/models/layers.py` & `hcpdiff-0.1.4/hcpdiff/models/layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/models/lora.py` & `hcpdiff-0.1.4/hcpdiff/models/lora.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/models/lora_layers.py` & `hcpdiff-0.1.4/hcpdiff/models/lora_layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/models/plugin.py` & `hcpdiff-0.1.4/hcpdiff/models/plugin.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/models/text_emb_ex.py` & `hcpdiff-0.1.4/hcpdiff/models/text_emb_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/models/textencoder_ex.py` & `hcpdiff-0.1.4/hcpdiff/models/textencoder_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/models/tokenizer_ex.py` & `hcpdiff-0.1.4/hcpdiff/models/tokenizer_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/tools/create_embedding.py` & `hcpdiff-0.1.4/hcpdiff/tools/create_embedding.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/tools/gen_from_ptlist.py` & `hcpdiff-0.1.4/hcpdiff/tools/gen_from_ptlist.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/tools/init_proj.py` & `hcpdiff-0.1.4/hcpdiff/tools/init_proj.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/tools/merge_model_part.py` & `hcpdiff-0.1.4/hcpdiff/tools/merge_model_part.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/train_ac.py` & `hcpdiff-0.1.4/hcpdiff/train_ac.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/train_ac_single.py` & `hcpdiff-0.1.4/hcpdiff/train_ac_single.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/train_colo.py` & `hcpdiff-0.1.4/hcpdiff/train_colo.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/utils/caption_tools.py` & `hcpdiff-0.1.4/hcpdiff/utils/caption_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/utils/cfg_net_tools.py` & `hcpdiff-0.1.4/hcpdiff/utils/cfg_net_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/utils/ckpt_manager/ckpt_pkl.py` & `hcpdiff-0.1.4/hcpdiff/utils/ckpt_manager/ckpt_pkl.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py` & `hcpdiff-0.1.4/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/utils/colo_utils.py` & `hcpdiff-0.1.4/hcpdiff/utils/colo_utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/utils/ema.py` & `hcpdiff-0.1.4/hcpdiff/utils/ema.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/utils/img_size_tool.py` & `hcpdiff-0.1.4/hcpdiff/utils/img_size_tool.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/utils/utils.py` & `hcpdiff-0.1.4/hcpdiff/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff/visualizer.py` & `hcpdiff-0.1.4/hcpdiff/visualizer.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/hcpdiff.egg-info/PKG-INFO` & `hcpdiff-0.1.4/hcpdiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.1.3
+Version: 0.1.4
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hcpdiff-0.1.3/hcpdiff.egg-info/SOURCES.txt` & `hcpdiff-0.1.4/hcpdiff.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 hcpdiff/models/lora.py
 hcpdiff/models/lora_layers.py
 hcpdiff/models/plugin.py
 hcpdiff/models/text_emb_ex.py
 hcpdiff/models/textencoder_ex.py
 hcpdiff/models/tokenizer_ex.py
 hcpdiff/tools/__init__.py
+hcpdiff/tools/convert_caption_txt2json.py
 hcpdiff/tools/create_embedding.py
 hcpdiff/tools/gen_from_ptlist.py
 hcpdiff/tools/init_proj.py
 hcpdiff/tools/merge_model_part.py
 hcpdiff/utils/__init__.py
 hcpdiff/utils/caption_tools.py
 hcpdiff/utils/cfg_net_tools.py
```

### Comparing `hcpdiff-0.1.3/prompt_tuning_template/object.txt` & `hcpdiff-0.1.4/prompt_tuning_template/object.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/prompt_tuning_template/style.txt` & `hcpdiff-0.1.4/prompt_tuning_template/style.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.3/setup.py` & `hcpdiff-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             file_dict[prefix+root].append(os.path.join(root, name))
     return [(k, v) for k, v in file_dict.items()]
 
 
 setuptools.setup(
     name="hcpdiff",
     py_modules=["hcpdiff"],
-    version="0.1.3",
+    version="0.1.4",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A universal Stable-Diffusion toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/7eu7d7/HCP-Diffusion",
     packages=setuptools.find_packages(),
```

