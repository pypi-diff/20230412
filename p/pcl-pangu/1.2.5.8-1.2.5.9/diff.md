# Comparing `tmp/pcl_pangu-1.2.5.8.tar.gz` & `tmp/pcl_pangu-1.2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcl_pangu-1.2.5.8.tar", last modified: Wed Apr 12 09:00:37 2023, max compression
+gzip compressed data, was "pcl_pangu-1.2.5.9.tar", last modified: Wed Apr 12 09:19:44 2023, max compression
```

## Comparing `pcl_pangu-1.2.5.8.tar` & `pcl_pangu-1.2.5.9.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.993130 pcl_pangu-1.2.5.8/
--rw-r--r--   0 root         (0) root         (0)      289 2023-04-12 09:00:37.989130 pcl_pangu-1.2.5.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7675 2023-04-06 01:29:53.000000 pcl_pangu-1.2.5.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.977131 pcl_pangu-1.2.5.8/pcl_pangu/
--rw-r--r--   0 root         (0) root         (0)      208 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.977131 pcl_pangu-1.2.5.8/pcl_pangu/context/
--rw-r--r--   0 root         (0) root         (0)      263 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/context/check_context.py
--rw-r--r--   0 root         (0) root         (0)      452 2023-03-30 08:59:08.000000 pcl_pangu-1.2.5.8/pcl_pangu/context/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.977131 pcl_pangu-1.2.5.8/pcl_pangu/dataset/
--rw-r--r--   0 root         (0) root         (0)      151 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14926 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/dataset/pre_process_chinese.py
--rw-r--r--   0 root         (0) root         (0)     5255 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/dataset/preprocess_data_pangu.py
--rw-r--r--   0 root         (0) root         (0)     3754 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/dataset/txt2bin.py
--rw-r--r--   0 root         (0) root         (0)     7133 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/dataset/txt2mindrecord.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.977131 pcl_pangu-1.2.5.8/pcl_pangu/model/
--rw-r--r--   0 root         (0) root         (0)      130 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.977131 pcl_pangu-1.2.5.8/pcl_pangu/model/alpha/
--rw-r--r--   0 root         (0) root         (0)      259 2023-03-30 09:00:28.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/alpha/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7356 2023-03-30 09:05:32.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/alpha/alpha.py
--rw-r--r--   0 root         (0) root         (0)     7659 2023-04-03 04:58:33.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/alpha/config_alpha.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.977131 pcl_pangu-1.2.5.8/pcl_pangu/model/evolution/
--rw-r--r--   0 root         (0) root         (0)      210 2023-04-03 01:24:00.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/evolution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4576 2023-03-30 10:24:57.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/evolution/config_evolution.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-03-30 10:26:27.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/evolution/evolution.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/launcher_torch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.977131 pcl_pangu-1.2.5.8/pcl_pangu/model/mPangu/
--rw-r--r--   0 root         (0) root         (0)      203 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/mPangu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7213 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/mPangu/config_mPangu.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/mPangu/mPangu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.977131 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15353 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/inference_alpha_ms13.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.981130 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9244 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/dataset.py
--rw-r--r--   0 root         (0) root         (0)    17636 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/generate.py
--rw-r--r--   0 root         (0) root         (0)    58054 2023-04-12 08:40:45.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha.py
--rw-r--r--   0 root         (0) root         (0)     6491 2023-04-12 08:59:55.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_config.py
--rw-r--r--   0 root         (0) root         (0)    12303 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_wrapcell.py
--rw-r--r--   0 root         (0) root         (0)     9209 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/preprocess.py
--rw-r--r--   0 root         (0) root         (0)    68987 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/serialization.py
--rw-r--r--   0 root         (0) root         (0)     2505 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/tokenization_jieba.py
--rw-r--r--   0 root         (0) root         (0)    36469 2023-04-03 06:24:29.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/utils_pangu.py
--rw-r--r--   0 root         (0) root         (0)    26625 2023-04-12 08:52:23.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/train_alpha_ms13.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.981130 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/
--rw-r--r--   0 root         (0) root         (0)     2220 2023-04-06 01:31:51.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference-en.md
--rw-r--r--   0 root         (0) root         (0)     2267 2023-04-06 01:31:51.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference.md
--rw-r--r--   0 root         (0) root         (0)    14695 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8683 2023-04-06 01:31:51.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/README-en.md
--rw-r--r--   0 root         (0) root         (0)     8335 2023-04-06 01:31:51.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/README.md
--rw-r--r--   0 root         (0) root         (0)    31808 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/README_mgt.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.981130 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/
--rw-r--r--   0 root         (0) root         (0)     1408 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23215 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/arguments.py
--rw-r--r--   0 root         (0) root         (0)    11011 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/checkpointing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.981130 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/
--rw-r--r--   0 root         (0) root         (0)      288 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/Makefile
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9841 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/bert_dataset.py
--rw-r--r--   0 root         (0) root         (0)    18923 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/dataset_utils.py
--rw-r--r--   0 root         (0) root         (0)    13647 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/gpt2_dataset.py
--rw-r--r--   0 root         (0) root         (0)    25244 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/helpers.cpp
--rw-r--r--   0 root         (0) root         (0)     5695 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/ict_dataset.py
--rw-r--r--   0 root         (0) root         (0)    19128 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/indexed_dataset.py
--rw-r--r--   0 root         (0) root         (0)     7721 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_dataset_utils.py
--rw-r--r--   0 root         (0) root         (0)     9038 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_index.py
--rw-r--r--   0 root         (0) root         (0)     6203 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/samplers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.981130 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/
--rw-r--r--   0 root         (0) root         (0)      971 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32911 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16.py
--rw-r--r--   0 root         (0) root         (0)     8331 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16util.py
--rw-r--r--   0 root         (0) root         (0)    10504 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/loss_scaler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.981130 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/
--rw-r--r--   0 root         (0) root         (0)     2337 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.cpp
--rw-r--r--   0 root         (0) root         (0)    19953 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 root         (0) root         (0)     2959 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 root         (0) root         (0)     7538 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/global_vars.py
--rw-r--r--   0 root         (0) root         (0)     4182 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/indexer.py
--rw-r--r--   0 root         (0) root         (0)     5909 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/initialize.py
--rw-r--r--   0 root         (0) root         (0)     5054 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/learning_rates.py
--rw-r--r--   0 root         (0) root         (0)     5188 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/memory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.985130 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/
--rw-r--r--   0 root         (0) root         (0)      936 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11546 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/alpha_enhanced_model.py
--rw-r--r--   0 root         (0) root         (0)     8364 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/bert_model.py
--rw-r--r--   0 root         (0) root         (0)     4283 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/classification.py
--rw-r--r--   0 root         (0) root         (0)     5151 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/distributed.py
--rw-r--r--   0 root         (0) root         (0)     2151 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_bias_gelu.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_softmax.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/gpt2_model.py
--rw-r--r--   0 root         (0) root         (0)    27501 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/language_model.py
--rw-r--r--   0 root         (0) root         (0)      995 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/mpu_utils.py
--rw-r--r--   0 root         (0) root         (0)     4752 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/multiple_choice.py
--rw-r--r--   0 root         (0) root         (0)     8874 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/realm_model.py
--rw-r--r--   0 root         (0) root         (0)    36536 2023-03-30 03:27:44.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/transformer.py
--rw-r--r--   0 root         (0) root         (0)     3161 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/utils.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.985130 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/
--rw-r--r--   0 root         (0) root         (0)     2144 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/cross_entropy.py
--rw-r--r--   0 root         (0) root         (0)     4134 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/data.py
--rw-r--r--   0 root         (0) root         (0)     5025 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/grads.py
--rw-r--r--   0 root         (0) root         (0)     5733 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/initialize.py
--rw-r--r--   0 root         (0) root         (0)    16415 2023-03-30 03:21:36.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/layers.py
--rw-r--r--   0 root         (0) root         (0)     4444 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/mappings.py
--rw-r--r--   0 root         (0) root         (0)    13208 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/random.py
--rw-r--r--   0 root         (0) root         (0)     2781 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/utils.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/package_info.py
--rw-r--r--   0 root         (0) root         (0)    16248 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/text_generation_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.985130 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/
--rw-r--r--   0 root         (0) root         (0)      731 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13952 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/bert_tokenization.py
--rw-r--r--   0 root         (0) root         (0)    13780 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/gpt2_tokenization.py
--rw-r--r--   0 root         (0) root         (0)     3389 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenization_jieba.py
--rw-r--r--   0 root         (0) root         (0)     6864 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    21991 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/training.py
--rw-r--r--   0 root         (0) root         (0)     6779 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/utils.py
--rw-r--r--   0 root         (0) root         (0)    23337 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/mergeMpCkpt.py
--rw-r--r--   0 root         (0) root         (0)     3960 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/pretrain_bert.py
--rw-r--r--   0 root         (0) root         (0)     3681 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/pretrain_evolution.py
--rw-r--r--   0 root         (0) root         (0)     3624 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/pretrain_gpt2.py
--rw-r--r--   0 root         (0) root         (0)     5268 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/pretrain_ict.py
--rw-r--r--   0 root         (0) root         (0)       36 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     3106 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/setup.py
--rw-r--r--   0 root         (0) root         (0)     1011 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/testLayerNorm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.985130 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/
--rw-r--r--   0 root         (0) root         (0)    16425 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/change_MspCkpt_ToMgt.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/create_doc_index.py
--rw-r--r--   0 root         (0) root         (0)    10948 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_Pangu.py
--rw-r--r--   0 root         (0) root         (0)    10812 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_epangu.py
--rw-r--r--   0 root         (0) root         (0)     1295 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/linter.py
--rw-r--r--   0 root         (0) root         (0)    11619 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/merge_mp_partitions.py
--rw-r--r--   0 root         (0) root         (0)     7896 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/preprocess_data_pangu.py
--rw-r--r--   0 root         (0) root         (0)     9474 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/splitMergedCkpt_v0.py
--rw-r--r--   0 root         (0) root         (0)     8699 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/split_full_model_into_mp_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.985130 pcl_pangu-1.2.5.8/pcl_pangu/model_converter/
--rw-r--r--   0 root         (0) root         (0)      220 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model_converter/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15563 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model_converter/_numpy_ckpt_2_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1354 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model_converter/merge_pytorch_model.py
--rw-r--r--   0 root         (0) root         (0)     1537 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model_converter/ms_2_numpy.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model_converter/numpy_2_pt.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/model_converter/split_pytorch_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.985130 pcl_pangu-1.2.5.8/pcl_pangu/online/
--rw-r--r--   0 root         (0) root         (0)      212 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/online/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.985130 pcl_pangu-1.2.5.8/pcl_pangu/online/infer/
--rw-r--r--   0 root         (0) root         (0)       86 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/online/infer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3229 2023-04-06 09:12:13.000000 pcl_pangu-1.2.5.8/pcl_pangu/online/infer/infer.py
--rw-r--r--   0 root         (0) root         (0)     2968 2023-04-06 10:11:00.000000 pcl_pangu-1.2.5.8/pcl_pangu/online/infer/pangu_alpha_dto.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-04-06 10:10:09.000000 pcl_pangu-1.2.5.8/pcl_pangu/online/infer/pangu_evolution_dto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.985130 pcl_pangu-1.2.5.8/pcl_pangu/online/modelinfo/
--rw-r--r--   0 root         (0) root         (0)       86 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/online/modelinfo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1166 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/online/modelinfo/modelinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.985130 pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3911 2023-04-04 01:24:04.000000 pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/conver_pt_onnx.py
--rw-r--r--   0 root         (0) root         (0)     3653 2023-03-30 09:53:40.000000 pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/infer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.985130 pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/pangu/
--rw-r--r--   0 root         (0) root         (0)     2125 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/pangu/config.py
--rw-r--r--   0 root         (0) root         (0)     9588 2023-04-03 13:33:22.000000 pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/pangu/model.py
--rw-r--r--   0 root         (0) root         (0)     9132 2023-04-03 13:53:20.000000 pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/pangu/model_onnx_gpu.py
--rw-r--r--   0 root         (0) root         (0)     5040 2023-03-30 09:23:46.000000 pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/pangu/sample.py
--rw-r--r--   0 root         (0) root         (0)     1435 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/pangu/utils.py
--rw-r--r--   0 root         (0) root         (0)     7867 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.985130 pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/
--rw-r--r--   0 root         (0) root         (0)      246 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.985130 pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/bpe_4w_pcl/
--rw-r--r--   0 root         (0) root         (0)   879697 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.model
--rw-r--r--   0 root         (0) root         (0)   717452 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.vocab
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.989130 pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/spm_13w/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/spm_13w/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1991068 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/spm_13w/data_dict.128k.txt
--rw-r--r--   0 root         (0) root         (0)  2423393 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/spm_13w/spm.128k.model.1
--rw-r--r--   0 root         (0) root         (0)    14949 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/spm_13w/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)     2549 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/tokenization_jieba.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:00:37.989130 pcl_pangu-1.2.5.8/pcl_pangu.egg-info/
--rw-r--r--   0 root         (0) root         (0)      289 2023-04-12 09:00:37.000000 pcl_pangu-1.2.5.8/pcl_pangu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8394 2023-04-12 09:00:37.000000 pcl_pangu-1.2.5.8/pcl_pangu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 09:00:37.000000 pcl_pangu-1.2.5.8/pcl_pangu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-04-12 09:00:37.000000 pcl_pangu-1.2.5.8/pcl_pangu.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-12 09:00:37.000000 pcl_pangu-1.2.5.8/pcl_pangu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 09:00:37.993130 pcl_pangu-1.2.5.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1955 2023-04-12 09:00:02.000000 pcl_pangu-1.2.5.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.922655 pcl_pangu-1.2.5.9/
+-rw-r--r--   0 root         (0) root         (0)      289 2023-04-12 09:19:44.922655 pcl_pangu-1.2.5.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7675 2023-04-06 01:29:53.000000 pcl_pangu-1.2.5.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/
+-rw-r--r--   0 root         (0) root         (0)      208 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/context/
+-rw-r--r--   0 root         (0) root         (0)      263 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/context/check_context.py
+-rw-r--r--   0 root         (0) root         (0)      452 2023-03-30 08:59:08.000000 pcl_pangu-1.2.5.9/pcl_pangu/context/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/dataset/
+-rw-r--r--   0 root         (0) root         (0)      151 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14926 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/dataset/pre_process_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     5255 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/dataset/preprocess_data_pangu.py
+-rw-r--r--   0 root         (0) root         (0)     3754 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/dataset/txt2bin.py
+-rw-r--r--   0 root         (0) root         (0)     7133 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/dataset/txt2mindrecord.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/alpha/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-03-30 09:00:28.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7356 2023-03-30 09:05:32.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/alpha/alpha.py
+-rw-r--r--   0 root         (0) root         (0)     7659 2023-04-03 04:58:33.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/alpha/config_alpha.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/evolution/
+-rw-r--r--   0 root         (0) root         (0)      210 2023-04-03 01:24:00.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/evolution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4576 2023-03-30 10:24:57.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/evolution/config_evolution.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-03-30 10:26:27.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/evolution/evolution.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/launcher_torch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/mPangu/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/mPangu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7213 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/mPangu/config_mPangu.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/mPangu/mPangu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15353 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/inference_alpha_ms13.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9244 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    17636 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/generate.py
+-rw-r--r--   0 root         (0) root         (0)    64752 2023-04-12 09:14:56.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha.py
+-rw-r--r--   0 root         (0) root         (0)     6406 2023-04-12 09:14:56.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_config.py
+-rw-r--r--   0 root         (0) root         (0)    12303 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_wrapcell.py
+-rw-r--r--   0 root         (0) root         (0)     9209 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/preprocess.py
+-rw-r--r--   0 root         (0) root         (0)    68987 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/serialization.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/tokenization_jieba.py
+-rw-r--r--   0 root         (0) root         (0)    36469 2023-04-03 06:24:29.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/utils_pangu.py
+-rw-r--r--   0 root         (0) root         (0)    26625 2023-04-12 09:18:43.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/train_alpha_ms13.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-04-06 01:31:51.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference-en.md
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-04-06 01:31:51.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference.md
+-rw-r--r--   0 root         (0) root         (0)    14695 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8683 2023-04-06 01:31:51.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/README-en.md
+-rw-r--r--   0 root         (0) root         (0)     8335 2023-04-06 01:31:51.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/README.md
+-rw-r--r--   0 root         (0) root         (0)    31808 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/README_mgt.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23215 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/arguments.py
+-rw-r--r--   0 root         (0) root         (0)    11011 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/checkpointing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/
+-rw-r--r--   0 root         (0) root         (0)      288 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/Makefile
+-rw-r--r--   0 root         (0) root         (0)       31 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9841 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/bert_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    18923 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/dataset_utils.py
+-rw-r--r--   0 root         (0) root         (0)    13647 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/gpt2_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    25244 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/helpers.cpp
+-rw-r--r--   0 root         (0) root         (0)     5695 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/ict_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    19128 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/indexed_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     7721 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_dataset_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9038 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_index.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/samplers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/
+-rw-r--r--   0 root         (0) root         (0)      971 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32911 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16.py
+-rw-r--r--   0 root         (0) root         (0)     8331 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16util.py
+-rw-r--r--   0 root         (0) root         (0)    10504 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/loss_scaler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.cpp
+-rw-r--r--   0 root         (0) root         (0)    19953 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 root         (0) root         (0)     7538 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/global_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4182 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     5909 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     5054 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/learning_rates.py
+-rw-r--r--   0 root         (0) root         (0)     5188 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/memory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/
+-rw-r--r--   0 root         (0) root         (0)      936 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11546 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/alpha_enhanced_model.py
+-rw-r--r--   0 root         (0) root         (0)     8364 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/bert_model.py
+-rw-r--r--   0 root         (0) root         (0)     4283 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/classification.py
+-rw-r--r--   0 root         (0) root         (0)     5151 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/distributed.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_bias_gelu.py
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_softmax.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/gpt2_model.py
+-rw-r--r--   0 root         (0) root         (0)    27501 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/language_model.py
+-rw-r--r--   0 root         (0) root         (0)      995 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/mpu_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4752 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/multiple_choice.py
+-rw-r--r--   0 root         (0) root         (0)     8874 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/realm_model.py
+-rw-r--r--   0 root         (0) root         (0)    36536 2023-03-30 03:27:44.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/
+-rw-r--r--   0 root         (0) root         (0)     2144 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/cross_entropy.py
+-rw-r--r--   0 root         (0) root         (0)     4134 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/data.py
+-rw-r--r--   0 root         (0) root         (0)     5025 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/grads.py
+-rw-r--r--   0 root         (0) root         (0)     5733 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/initialize.py
+-rw-r--r--   0 root         (0) root         (0)    16415 2023-03-30 03:21:36.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/layers.py
+-rw-r--r--   0 root         (0) root         (0)     4444 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/mappings.py
+-rw-r--r--   0 root         (0) root         (0)    13208 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/random.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/package_info.py
+-rw-r--r--   0 root         (0) root         (0)    16248 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/text_generation_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/
+-rw-r--r--   0 root         (0) root         (0)      731 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13952 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/bert_tokenization.py
+-rw-r--r--   0 root         (0) root         (0)    13780 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/gpt2_tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenization_jieba.py
+-rw-r--r--   0 root         (0) root         (0)     6864 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    21991 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/training.py
+-rw-r--r--   0 root         (0) root         (0)     6779 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/utils.py
+-rw-r--r--   0 root         (0) root         (0)    23337 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/mergeMpCkpt.py
+-rw-r--r--   0 root         (0) root         (0)     3960 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_bert.py
+-rw-r--r--   0 root         (0) root         (0)     3681 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_evolution.py
+-rw-r--r--   0 root         (0) root         (0)     3624 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_gpt2.py
+-rw-r--r--   0 root         (0) root         (0)     5268 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_ict.py
+-rw-r--r--   0 root         (0) root         (0)       36 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     3106 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/testLayerNorm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/
+-rw-r--r--   0 root         (0) root         (0)    16425 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/change_MspCkpt_ToMgt.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/create_doc_index.py
+-rw-r--r--   0 root         (0) root         (0)    10948 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_Pangu.py
+-rw-r--r--   0 root         (0) root         (0)    10812 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_epangu.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/linter.py
+-rw-r--r--   0 root         (0) root         (0)    11619 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/merge_mp_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     7896 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/preprocess_data_pangu.py
+-rw-r--r--   0 root         (0) root         (0)     9474 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/splitMergedCkpt_v0.py
+-rw-r--r--   0 root         (0) root         (0)     8699 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/split_full_model_into_mp_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15563 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/_numpy_ckpt_2_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/merge_pytorch_model.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/ms_2_numpy.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/numpy_2_pt.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/split_pytorch_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/online/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/online/infer/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/infer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2023-04-06 09:12:13.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/infer/infer.py
+-rw-r--r--   0 root         (0) root         (0)     2968 2023-04-06 10:11:00.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/infer/pangu_alpha_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-04-06 10:10:09.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/infer/pangu_evolution_dto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/online/modelinfo/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/modelinfo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/modelinfo/modelinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3911 2023-04-04 01:24:04.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/conver_pt_onnx.py
+-rw-r--r--   0 root         (0) root         (0)     3653 2023-03-30 09:53:40.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/infer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/config.py
+-rw-r--r--   0 root         (0) root         (0)     9588 2023-04-03 13:33:22.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/model.py
+-rw-r--r--   0 root         (0) root         (0)     9132 2023-04-03 13:53:20.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/model_onnx_gpu.py
+-rw-r--r--   0 root         (0) root         (0)     5040 2023-03-30 09:23:46.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/sample.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/utils.py
+-rw-r--r--   0 root         (0) root         (0)     7867 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/bpe_4w_pcl/
+-rw-r--r--   0 root         (0) root         (0)   879697 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.model
+-rw-r--r--   0 root         (0) root         (0)   717452 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.vocab
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.922655 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1991068 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/data_dict.128k.txt
+-rw-r--r--   0 root         (0) root         (0)  2423393 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/spm.128k.model.1
+-rw-r--r--   0 root         (0) root         (0)    14949 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/tokenization_jieba.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.922655 pcl_pangu-1.2.5.9/pcl_pangu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      289 2023-04-12 09:19:44.000000 pcl_pangu-1.2.5.9/pcl_pangu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8394 2023-04-12 09:19:44.000000 pcl_pangu-1.2.5.9/pcl_pangu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 09:19:44.000000 pcl_pangu-1.2.5.9/pcl_pangu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-04-12 09:19:44.000000 pcl_pangu-1.2.5.9/pcl_pangu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-12 09:19:44.000000 pcl_pangu-1.2.5.9/pcl_pangu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 09:19:44.922655 pcl_pangu-1.2.5.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-04-12 09:19:21.000000 pcl_pangu-1.2.5.9/setup.py
```

### Comparing `pcl_pangu-1.2.5.8/README.md` & `pcl_pangu-1.2.5.9/README.md`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/dataset/pre_process_chinese.py` & `pcl_pangu-1.2.5.9/pcl_pangu/dataset/pre_process_chinese.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/dataset/preprocess_data_pangu.py` & `pcl_pangu-1.2.5.9/pcl_pangu/dataset/preprocess_data_pangu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/dataset/txt2bin.py` & `pcl_pangu-1.2.5.9/pcl_pangu/dataset/txt2bin.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/dataset/txt2mindrecord.py` & `pcl_pangu-1.2.5.9/pcl_pangu/dataset/txt2mindrecord.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/alpha/alpha.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/alpha/alpha.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/alpha/config_alpha.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/alpha/config_alpha.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/evolution/config_evolution.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/evolution/config_evolution.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/evolution/evolution.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/evolution/evolution.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/launcher_torch.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/launcher_torch.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/mPangu/config_mPangu.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/mPangu/config_mPangu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/mPangu/mPangu.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/mPangu/mPangu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/inference_alpha_ms13.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/inference_alpha_ms13.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/dataset.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/dataset.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/generate.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/generate.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,125 +1,116 @@
-# Copyright 2021 Huawei Technologies Co., Ltd
+# Copyright 2022 PCL, Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
-"""GPT model"""
+"""PanguAlpha model"""
 import math
+import os
 import numpy as np
 import mindspore.nn as nn
 from mindspore.common.tensor import Tensor
 from mindspore.common.parameter import Parameter
 import mindspore.common.dtype as mstype
-from mindspore.common.initializer import initializer, Normal, Uniform, TruncatedNormal
+from mindspore.common.initializer import initializer, Normal, TruncatedNormal
 from mindspore.ops import operations as P
 from mindspore.ops import functional as F
-import numpy as np
-from mindspore.nn.transformer.transformer import VocabEmbedding
-import copy
-from mindspore.nn.transformer.layers import _Dropout
-
-class EmbeddingLayer(nn.Cell):
-    r"""Embedding layer of the PanGUAlpha Model"""
-    def __init__(self, config):
-        super(EmbeddingLayer, self).__init__()
-        # Only for the pipeline mode, the embedding needs to be row sliced.
-        self.word_embedding = VocabEmbedding(vocab_size=config.vocab_size,
-                                             embedding_size=config.hidden_size,
-                                             param_init=initializer("normal", [config.vocab_size, config.hidden_size],
-                                                                    ),  # dtype=mstype.float32
-                                             parallel_config=config.parallel_config.embedding_dp_mp_config)
-        copied_parallel_config = copy.deepcopy(config.parallel_config)
-        copied_parallel_config.vocab_emb_dp = True
-        self.position_embedding = VocabEmbedding(vocab_size=config.seq_length,
-                                                 embedding_size=config.hidden_size,
-                                                 param_init=initializer("normal",
-                                                                        [config.seq_length, config.hidden_size],
-                                                                        ), # dtype=mstype.float32
-                                                 parallel_config=copied_parallel_config.embedding_dp_mp_config)
-        self.add = P.Add().shard(
-            ((config.parallel_config.data_parallel, 1, 1), (config.parallel_config.data_parallel, 1, 1)))
-        self.dropout = _Dropout(1 - config.dropout_rate)
-        self.dropout.shard(((config.parallel_config.data_parallel, 1, 1),))
-        self.is_first_iteration = True
-        self.use_past = config.use_past
-        self.batch_size = config.batch_size
-
-    def construct(self, input_ids, input_position, init_reset, batch_valid_length):
-        word_embedding, word_table = self.word_embedding(input_ids)
-        if self.use_past and not self.is_first_iteration:
-            _, seq_length = F.shape(input_ids)
-            input_position = batch_valid_length.view(self.batch_size, seq_length)
-        position_embedding, _ = self.position_embedding(input_position)
-        embed = self.add(word_embedding, position_embedding)
-        embed = self.dropout(embed)
-        return embed, word_table
-
-    def get_word_embedding_weight(self):
-        return self.word_embedding.embedding_table
-
-class LayerNormScale(nn.Cell):
-    def __init__(self, normalized_shape, dp=4, eps=1e-5, scale=1e-3):
-        super(LayerNorm, self).__init__()
-        self.gamma = Parameter(initializer('ones', normalized_shape), name="gamma")
-        self.beta = Parameter(initializer('zeros', normalized_shape), name="beta")
-        self.mean = P.ReduceMean(keep_dims=True).shard(((dp, 1, 1),))
-        self.square = P.Square().shard(((dp, 1, 1),))
-        self.sqrt = P.Sqrt().shard(((dp, 1, 1),))
-        self.sub1 = P.Sub().shard(((dp, 1, 1), (dp, 1, 1)))
-        self.sub2 = P.Sub().shard(((dp, 1, 1), (dp, 1, 1)))
-        self.add = P.TensorAdd().shard(((dp, 1, 1), ()))
-        self.eps = eps
-        self.mul = P.Mul().shard(((dp, 1, 1), (1,)))
-        self.add2 = P.TensorAdd().shard(((dp, 1, 1), (1,)))
-        self.real_div = P.RealDiv().shard(((dp, 1, 1), (dp, 1, 1)))
-        self.scale_div = P.RealDiv().shard(((dp, 1, 1), ()))
-        self.scale_mul = P.Mul().shard(((dp, 1, 1), ()))
-        self.scale = scale
-        self.scale_eps = self.eps / (self.scale * self.scale)
+from mindspore import context
+from mindspore.common.seed import _get_graph_seed
+from mindspore._checkparam import Validator
+
+
+class Dropout(nn.Cell):
+    r"""
+        A Dropout Implements with P.DropoutGenMask and  P.DropoutDoMask for parallel training.
+    """
+
+    def __init__(self, keep_prob=0.5, dtype=mstype.float32):
+        super(Dropout, self).__init__()
+        if keep_prob <= 0 or keep_prob > 1:
+            raise ValueError(
+                "dropout probability should be a number in range (0, 1], but got {}".format(
+                    keep_prob))
+        Validator.check_subclass("dtype", dtype, mstype.number_type, self.cls_name)
+        Validator.check_value_type('keep_prob', keep_prob, [float], self.cls_name)
+        self.keep_prob = keep_prob
+        self.is_ascend = context.get_context('device_target') in ["Ascend"]
+        if self.is_ascend:
+            seed0, seed1 = _get_graph_seed(0, "dropout")
+            self.seed0 = seed0
+            self.seed1 = seed1
+            self.dtype = dtype
+            self.get_shape = P.Shape()
+            self.dropout_gen_mask = P.DropoutGenMask(Seed0=self.seed0, Seed1=self.seed1)
+            self.dropout_do_mask = P.DropoutDoMask()
+            self.cast = P.Cast()
+        else:
+            self.dropout = P.Dropout(keep_prob)
 
     def construct(self, x):
-        mean = self.mean(x, -1)
-        diff = self.sub1(x, mean)
-        scale_diff = self.scale_div(diff, self.scale)
-        scale_variance = self.mean(self.square(scale_diff), -1)
-        scale_variance_eps = self.sqrt(self.add(scale_variance, self.scale_eps))
-        variance_eps = self.scale_mul(scale_variance_eps, self.scale)
-        output = self.real_div(diff, variance_eps)
-        rescaled_output = self.add2(self.mul(output, self.gamma), self.beta)
-        return rescaled_output
+        r"""
+           Input: a tensor
+           Returns: a tensor
+        """
+        if not self.training:
+            return x
+
+        if not self.is_ascend:
+            out, _ = self.dropout(x)
+            return out
+
+        if self.keep_prob == 1:
+            return x
+
+        shape = self.get_shape(x)
+        dtype = P.DType()(x)
+        keep_prob = self.cast(self.keep_prob, dtype)
+        output = self.dropout_gen_mask(shape, keep_prob)
+        return self.dropout_do_mask(x, output, keep_prob)
+
+    def extend_repr(self):
+        return 'keep_prob={}, dtype={}'.format(self.keep_prob, self.dtype)
+
+    def shard(self, strategy):
+        if self.is_ascend:
+            self.dropout_gen_mask.shard(strategy)
+            self.dropout_do_mask.shard(strategy)
+        else:
+            self.dropout.shard(strategy)
 
 
 class LayerNorm(nn.Cell):
-    def __init__(self, normalized_shape, dp=4, eps=1e-5, scale=1e-3):
+    r"""
+        A self-defined layer norm operation using reduce sum and reduce mean
+    """
+
+    def __init__(self, normalized_shape, dp=4, eps=1e-5, parallel_optimizer=False):
         super(LayerNorm, self).__init__()
-        self.gamma = Parameter(initializer('ones', normalized_shape), name="gamma")
-        self.beta = Parameter(initializer('zeros', normalized_shape), name="beta")
+        self.gamma = Parameter(initializer('ones', normalized_shape), name="gamma",
+                               parallel_optimizer=parallel_optimizer)
+        self.beta = Parameter(initializer('zeros', normalized_shape), name="beta",
+                              parallel_optimizer=parallel_optimizer)
         self.mean = P.ReduceMean(keep_dims=True).shard(((dp, 1, 1),))
         self.square = P.Square().shard(((dp, 1, 1),))
         self.sqrt = P.Sqrt().shard(((dp, 1, 1),))
         self.sub1 = P.Sub().shard(((dp, 1, 1), (dp, 1, 1)))
-        self.sub2 = P.Sub().shard(((dp, 1, 1), (dp, 1, 1)))
         self.add = P.TensorAdd().shard(((dp, 1, 1), ()))
-        self.eps = eps
         self.mul = P.Mul().shard(((dp, 1, 1), (1,)))
         self.add2 = P.TensorAdd().shard(((dp, 1, 1), (1,)))
         self.real_div = P.RealDiv().shard(((dp, 1, 1), (dp, 1, 1)))
-        self.scale_div = P.RealDiv().shard(((dp, 1, 1), ()))
-        self.scale_mul = P.Mul().shard(((dp, 1, 1), ()))
-        self.scale = scale
+        self.eps = eps
 
     def construct(self, x):
         mean = self.mean(x, -1)
         diff = self.sub1(x, mean)
         variance = self.mean(self.square(diff), -1)
         variance_eps = self.sqrt(self.add(variance, self.eps))
         output = self.real_div(diff, variance_eps)
@@ -143,19 +134,19 @@
 
     # 优化：matmul，dtype, mapping_output
     def __init__(self, config, input_size, output_size, scale=1.0):
         super(Mapping, self).__init__()
         self.output_size = output_size
         self.input_size = input_size
         self.weight = Parameter(initializer(Normal(sigma=0.02 * scale),
-                                            [input_size, output_size]),
+                                            [input_size, output_size], config.param_init_type),
                                 name="mapping_weight")
         self.bias = Parameter(initializer("zeros", [
             output_size,
-        ]),
+        ], config.param_init_type),
                               name="mapping_bias",
                               parallel_optimizer=False)
         self.dtype = config.compute_dtype
         self.cast = P.Cast()
         self.add = P.TensorAdd().shard(((config.dp, 1), (1,)))
         self.matmul = P.MatMul().shard(
             ((config.dp, config.mp), (config.mp, 1)))
@@ -166,25 +157,39 @@
         weight = self.cast(self.weight, self.dtype)
         x = self.matmul(x, weight)
         x = self.add(x, self.cast(self.bias, self.dtype))
         output = P.Reshape()(x, out_shape)
         return output
 
 
-class Mapping_output(nn.Cell):
+class MappingOutput(nn.Cell):
+    """
+    A mapping function with a 3d input
+    Args:
+        input_size: the size of the last dimension of the input tensor
+        output_size: the desired size of the last dimension of the output tensor
+        dtype: the compute datatype
+        scale: the scale factor for initialization
+    Inputs:
+        x: the 3d input
+    Returns:
+        output: Tensor, a 3d tensor after projection
+    """
+
     def __init__(self, config, input_size, output_size, scale=1.0):
-        super(Mapping_output, self).__init__()
+        super(MappingOutput, self).__init__()
         self.output_size = output_size
         self.input_size = input_size
         self.weight = Parameter(initializer(Normal(sigma=0.02 * scale),
-                                            [input_size, output_size]),
+                                            [input_size, output_size],
+                                            config.param_init_type),
                                 name="mapping_weight")
         self.bias = Parameter(initializer("zeros", [
             output_size,
-        ]),
+        ], config.param_init_type),
                               name="mapping_bias")
         self.dtype = config.compute_dtype
         self.cast = P.Cast()
         self.add = P.TensorAdd().shard(((config.dp, config.mp), (config.mp,)))
         self.matmul = P.MatMul().shard(((config.dp, 1), (1, config.mp)))
 
     def construct(self, x):
@@ -193,273 +198,258 @@
         weight = self.cast(self.weight, self.dtype)
         x = self.matmul(x, weight)
         x = self.add(x, self.cast(self.bias, self.dtype))
         output = P.Reshape()(x, out_shape)
         return output
 
 
-class Output(nn.Cell):
+class FeedForwardLayer(nn.Cell):
     """
     The output mapping module for each layer
     Args:
-        config(GPTConfig): the config of network
+        config(PanguAlphaConfig): the config of network
         scale: scale factor for initialization
     Inputs:
         x: output of the self-attention module
     Returns:
         output: Tensor, the output of this layer after mapping
     """
 
     def __init__(self, config, scale=1.0):
-        super(Output, self).__init__()
+        super(FeedForwardLayer, self).__init__()
         input_size = config.embedding_size
         output_size = config.embedding_size * config.expand_ratio
-        self.mapping = Mapping_output(config, input_size, output_size)
+        # Project to expand_ratio*embedding_size
+        self.mapping = MappingOutput(config, input_size, output_size)
+        # Project back to embedding_size
         self.projection = Mapping(config, output_size, input_size, scale)
         self.activation = nn.GELU()
         self.activation.gelu.shard(((config.dp, 1, config.mp),))
-        self.dropout = nn.Dropout(1 - config.dropout_rate)
-        self.dropout.dropout.shard(((config.dp, 1, 1),))
-        # self.dropout.dropout_gen_mask.shard(((config.dp, 1, 1),))
-        # self.dropout.dropout_do_mask.shard(((config.dp, 1, 1),))
+        self.dropout = Dropout(1 - config.dropout_rate)
+        self.dropout.shard(((config.dp, 1, 1),))
 
     def construct(self, x):
+        # [bs, seq_length, expand_ratio*embedding_size]
         hidden = self.activation(self.mapping(x))
         output = self.projection(hidden)
+        # [bs, seq_length, expand_ratio]
         output = self.dropout(output)
         return output
 
 
-class AttentionMask(nn.Cell):
-    """
-    Get the attention matrix for self-attention module
-    Args:
-        config(GPTConfig): the config of network
-    Inputs:
-        input_mask: the mask indicating whether each position is a valid input
-    Returns:
-        attention_mask: the attention mask matrix with shape (batch_size, 1, seq_length, seq_length)
-    """
-
-    def __init__(self, config):
-        super(AttentionMask, self).__init__()
-        self.reshape = P.Reshape()
-        self.mul = P.BatchMatMul().shard(
-            ((config.dp, 1, 1), (config.dp, 1, 1)))  # yzz: use 64, 1, 1?
-        self.expand_dim = P.ExpandDims().shard(((1, 1),))
-        ones = np.ones(shape=(config.seq_length, config.seq_length))
-        self.lower_triangle_mask = Tensor(np.tril(ones), mstype.float32)
-        self.multiply = P.Mul().shard(((config.dp, 1, 1), (1, 1, 1)))
-
-    def construct(self, input_mask):
-        input_shape = P.Shape()(input_mask)
-        shape_right = (input_shape[0], 1, input_shape[1])
-        shape_left = input_shape + (1,)
-        mask_left = self.reshape(input_mask, shape_left)
-        mask_right = self.reshape(input_mask, shape_right)
-        attention_mask = self.mul(mask_left, mask_right)
-        lower_traiangle = self.expand_dim(self.lower_triangle_mask, 0)
-        attention_mask = self.multiply(
-            attention_mask, lower_traiangle)  # bs seq_length seq_length
-        return attention_mask
-
-
 class EmbeddingLookup(nn.Cell):
     """
     The embedding lookup table for vocabulary
-    Args:
-        config(GPTConfig): the config of network
     Inputs:
         input_ids: the tokenized inputs with datatype int32
     Returns:
-        output: Tensor, the embedding vector for the input with shape (batch_size, seq_length, embedding_size)
+        output: Tensor, the embedding vector for the input with shape (batch_size,
+        seq_length, embedding_size)
         self.embedding_table: Tensor, the embedding table for the vocabulary
     """
 
-    def __init__(self, config):
+    def __init__(self):
         super(EmbeddingLookup, self).__init__()
-        self.vocab_size = config.vocab_size
-        self.embedding_size = config.embedding_size
-        try:
-            e_table = np.load('/cache/word_embedding.npy')
-            e_table = Tensor(e_table, mstype.float32)
-            print("###### loading Word embedding Table successed! ######")
-        except:
-            e_table = Tensor(np.ones([self.vocab_size, self.embedding_size], dtype=np.float32))
-        self.embedding_table = Parameter(e_table,
-                                         name="embedding_table")
-        if config.word_emb_dp:
-            self.gather = P.GatherV2().shard(((1, 1), (config.dp, 1)))
-        else:
-            self.gather = P.GatherV2().shard(((1, config.mp), (config.dp, 1)))
-            self.gather.add_prim_attr("reverse_stra", True)
-            print("Using the reverse_stra columns slice", flush=True)
-        self.shape = (-1, config.seq_length, config.embedding_size)
-
-    def construct(self, input_ids):
-        output = self.gather(self.embedding_table, input_ids, 0)
-        return output, self.embedding_table
+        self.gather = P.GatherV2()
+
+    def construct(self, input_ids, table):
+        output = self.gather(table, input_ids, 0)
+        return output
 
 
 class Attention(nn.Cell):
     """
     Self-Attention module for each layer
 
     Args:
-        config(GPTConfig): the config of network
+        config(PanguAlphaConfig): the config of network
         scale: scale factor for initialization
         layer_idx: current layer index
     """
 
     def __init__(self, config, scale=1.0, layer_idx=None):
         super(Attention, self).__init__()
-        self.get_attention_mask = AttentionMask(config)
+        # Output layer
         self.projection = Mapping(config, config.embedding_size,
                                   config.embedding_size, scale)
         self.transpose = P.Transpose().shard(((config.dp, 1, config.mp, 1),))
         self.merger_head_transpose = P.Transpose().shard(
             ((config.dp, config.mp, 1, 1),))
         self.reshape = P.Reshape()
         self.n_head = config.num_heads
+        # embedding size per head
         self.size_per_head = config.embedding_size // self.n_head
         self.concat_k = P.Concat(axis=3)
         self.concat_v = P.Concat(axis=2)
         self.multiply_data = Tensor([
             -10000.0,
         ], dtype=mstype.float32)
         self.batch_matmul = P.BatchMatMul().shard(
             ((config.dp, config.mp, 1, 1), (config.dp, config.mp, 1, 1)))
         self.scale = scale
         self.real_div = P.RealDiv().shard(((config.dp, config.mp, 1, 1), ()))
         self.sub = P.Sub().shard(
-            ((1,), (config.dp, 1, 1, 1))).add_prim_attr("_side_effect", True)
+            ((1,), (config.dp, 1, 1, 1)))
         self.mul = P.Mul().shard(
-            ((config.dp, 1, 1, 1), (1,))).add_prim_attr("_side_effect", True)
+            ((config.dp, 1, 1, 1), (1,)))
         self.add = P.TensorAdd().shard(
             ((config.dp, 1, 1, 1), (config.dp, config.mp, 1, 1)))
+        # Normalize factor for attention, sqrt(dk) as widely used
         if self.scale:
             self.scale_factor = Tensor(math.sqrt(self.size_per_head))
         if layer_idx is not None:
             self.coeff = math.sqrt(layer_idx * math.sqrt(self.size_per_head))
             self.coeff = Tensor(self.coeff)
         self.use_past = config.use_past
-        self.dropout = nn.Dropout(1 - config.dropout_rate)
-        self.dropout.dropout.shard(((config.dp, 1, 1),))
-        # self.dropout.dropout_gen_mask.shard(((config.dp, 1, 1),))
-        # self.dropout.dropout_do_mask.shard(((config.dp, 1, 1),))
-        self.prob_dropout = nn.Dropout(1 - config.dropout_rate)
-        self.prob_dropout.dropout.shard(((config.dp, config.mp, 1, 1),))
-        #         self.prob_dropout.dropout_gen_mask.shard(
-        #             ((config.dp, config.mp, 1, 1),))
-        #         self.prob_dropout.dropout_do_mask.shard(
-        #             ((config.dp, config.mp, 1, 1),))
+        self.dropout = Dropout(1 - config.dropout_rate)
+        self.dropout.shard(((config.dp, 1, 1),))
+        self.prob_dropout = Dropout(1 - config.dropout_rate)
+        self.prob_dropout.shard(((config.dp, config.mp, 1, 1),))
         self.softmax = nn.Softmax()
         self.softmax.softmax.shard(((config.dp, config.mp, 1),))
         self.expand_dims = P.ExpandDims().shard(((config.dp, 1, 1),))
 
+        dense_shape = [config.embedding_size, config.embedding_size]
+        bias_shape = [config.embedding_size]
+        # Query
         self.dense1 = nn.Dense(config.embedding_size,
-                               config.embedding_size).to_float(
-            config.compute_dtype)
+                               config.embedding_size,
+                               weight_init=initializer(init='normal', shape=dense_shape,
+                                                       dtype=config.param_init_type),
+                               bias_init=initializer(init='zeros', shape=bias_shape,
+                                                     dtype=config.param_init_type)).to_float(config.compute_dtype)
         self.dense1.matmul.shard(((config.dp, 1), (config.mp, 1)))
         self.dense1.bias_add.shard(((config.dp, config.mp), (config.mp,)))
+        # Key
         self.dense2 = nn.Dense(config.embedding_size,
-                               config.embedding_size).to_float(
-            config.compute_dtype)
+                               config.embedding_size,
+                               weight_init=initializer(init='normal',
+                                                       shape=dense_shape,
+                                                       dtype=config.param_init_type),
+                               bias_init=initializer(init='zeros',
+                                                     shape=bias_shape,
+                                                     dtype=config.param_init_type)).to_float(config.compute_dtype)
         self.dense2.matmul.shard(((config.dp, 1), (config.mp, 1)))
         self.dense2.bias_add.shard(((config.dp, config.mp), (config.mp,)))
+        # Value
         self.dense3 = nn.Dense(config.embedding_size,
-                               config.embedding_size).to_float(
-            config.compute_dtype)
+                               config.embedding_size,
+                               weight_init=initializer(init='normal',
+                                                       shape=dense_shape,
+                                                       dtype=config.param_init_type),
+                               bias_init=initializer(init='zeros',
+                                                     shape=bias_shape,
+                                                     dtype=config.param_init_type)).to_float(config.compute_dtype)
         self.dense3.matmul.shard(((config.dp, 1), (config.mp, 1)))
         self.dense3.bias_add.shard(((config.dp, config.mp), (config.mp,)))
 
+        self.is_first_iteration = True
+        self.dtype = config.compute_dtype
         self.use_past = config.use_past
         if self.use_past:
-            self.pad_value = 0
+            # operators used for state reuse
             seq_range = np.arange(config.seq_length).reshape(1, 1, -1)
-            self.range = Tensor(seq_range, mstype.int32)
+            self.range = Tensor(np.tile(seq_range, (config.batch_size, 1, 1)), mstype.int32)
             self.seq_length = config.seq_length
+            self.attention_mask = Tensor(np.tril(np.ones(shape=(self.seq_length, self.seq_length))), mstype.int32)
             self.slice = P.StridedSlice().shard(((1, 1, 1, 1),))
             self.not_equal = P.NotEqual().shard(((1, 1, 1, 1), ()))
             self.reducesum = P.ReduceSum().shard(((1, 1, 1, 1),))
             self.expand_dims = P.ExpandDims().shard(((1, 1, 1),))
-            self.tensor_le = P.LessEqual().shard(((1, 1, 1, 1), (1, 1, 1, 1)))
+            self.tensor_le = P.LessEqual().shard(((1, 1, 1), (1, 1, 1)))
             self.add = P.TensorAdd().shard(((1, 1, 1, 1), (1, 1, 1, 1)))
             self.equal = P.Equal().shard(((1, 1, 1), (1, 1, 1)))
             self.sub1 = P.Sub().shard(((1,), ()))
             self.tile = P.Tile().shard(((1, 1, 1, 1),))
-            self.tile1 = P.Tile().shard(((1, 1, 1),))
-            self.is_first_iteration = True
             self.less = P.Less().shard(((1, 1, 1), (1, 1, 1)))
             self.mul1 = P.Mul().shard(((1, 1, 1, 1), (1, 1, 1, 1)))
-            self.dtype = config.compute_dtype
 
     def construct(self, x, attention_mask, key_past=None, value_past=None, batch_valid_length=None):
         """
         self-attention
 
         Inputs:
             x: output of previous layer
-            attention_mask: the attention mask matrix with shape (batch_size,
-            1, seq_length, seq_length)
-            key_past: the previous key of the self-attention module
-            value_past: the previous value of the self-attention module
-            batch_valid_length: the original valid sentence length of the first graph for incremental inference
+            attention_mask: the attention mask matrix with shape (batch_size, 1,
+            seq_length, seq_length)
+            key_past: previous saved key state
+            value_past: previous saved value state
+            batch_valid_length: the valid input seq_length without padding
 
         Returns:
             output: Tensor, the output logit of this layer
             layer_present: Tensor, the feature map of current layer
         """
 
         original_shape = F.shape(x)
         x = F.reshape(x, (-1, original_shape[-1]))
+        # Self attention: query, key, value are derived from the same inputs
         query = self.dense1(x)
         key = self.dense2(x)
         value = self.dense3(x)
+        # [bs, num_heads, seq_length, size_per_head]
         query = self.transpose(
             F.reshape(
                 query,
                 (-1, original_shape[1], self.n_head, self.size_per_head)),
             (0, 2, 1, 3))
+        # [bs, num_heads, size_per_head, seq_length]
         key = self.transpose(
             F.reshape(
                 key, (-1, original_shape[1], self.n_head, self.size_per_head)),
             (0, 2, 3, 1))
+        # [bs, num_heads, seq_length, size_per_head]
         value = self.transpose(
             F.reshape(
                 value,
                 (-1, original_shape[1], self.n_head, self.size_per_head)),
             (0, 2, 1, 3))
 
+        # key and value for current token(s)
         key_present = key
         value_present = value
-        range_vector = None
         if self.use_past:
-            range_vector = self.tile1(self.range, (original_shape[0], 1, 1))
+            # The first graph with the input size of (bs, seq_length)
             if self.is_first_iteration:
-                valid_length_vector = F.cast(self.less(range_vector, batch_valid_length), mstype.float16)
+                # Get the valid input length without padding
+                valid_length_vector = F.cast(self.less(self.range, batch_valid_length.view(1, 1, -1)), self.dtype)
+                # Cover the key and value numbers corresponding to the padding position
                 key_present = self.mul1(key, self.expand_dims(valid_length_vector, 2))
                 value_present = self.mul1(value, self.expand_dims(valid_length_vector, 3))
+            # The second graph with the inpus size of (bs, 1)
+            # the shape of query is (bs, num_heads, 1, size_per_head)
+            # the shape of key is   (bs, num_heads, size_per_head, 1)
+            # the shape of value is (bs, num_heads, 1, size_per_head)
             else:
-                valid_length = self.reducesum(F.cast(self.not_equal(
-                    self.slice(key_past, (0, 0, 0, 0), (original_shape[0], 1, 1, self.seq_length), (1, 1, 1, 1)),
-                    self.pad_value), mstype.float32), (1, 2, 3))
+                # Get the current token position index
+                valid_length = self.reducesum(F.cast(self.not_equal(self.slice(key_past, (0, 0, 0, 0),
+                                                                               (F.shape(x)[0], 1, 1, self.seq_length),
+                                                                               (1, 1, 1, 1)),
+                                                                    0), mstype.float32), (1, 2, 3))
                 valid_length = F.reshape(valid_length, (-1, 1, 1))
-                valid_length_vector = F.cast(self.equal(valid_length, range_vector), self.dtype)
+                valid_length_vector = F.cast(self.equal(valid_length, self.range), self.dtype)
+                # Pad the key and value to seq_length with only the position index not zero
                 current_key = self.mul1(self.tile(key, (1, 1, 1, self.seq_length)),
                                         self.expand_dims(valid_length_vector, 2))
                 current_value = self.mul1(self.tile(value, (1, 1, self.seq_length, 1)),
                                           self.expand_dims(valid_length_vector, 3))
+                # Concat the previous saved state and current state
                 key = self.add(key_past, current_key)
                 value = self.add(value_past, current_value)
+                # Update key_present and value_present for state update
                 key_present = key
                 value_present = value
+                attention_mask = F.reshape(self.attention_mask, (self.seq_length, self.seq_length, 1, 1))
+
         layer_present = (key_present, value_present)
-        attention = self._attn(query, key, value, attention_mask, range_vector)
+        # Self-attention considering attention mask
+        attention = self._attn(query, key, value, attention_mask)
+        # [bs, seq_length, embedding_size]
         attention_merge = self.merge_heads(attention)
+        # Output
         output = self.projection(attention_merge)
         output = self.dropout(output)
         return output, layer_present
 
     def split_heads(self, x, transpose):
         """
         split 3d tensor to 4d and switch certain axes
@@ -488,139 +478,259 @@
         x = self.merger_head_transpose(
             x, (0, 2, 1, 3))  # bs, seq_length, head, size_per_head
         x_shape = P.Shape()(x)
         new_shape = x_shape[:-2] + (x_shape[-2] * x_shape[-1],)
         x_merge = self.reshape(x, new_shape)
         return x_merge
 
-    def _attn(self, query, key, value, attention_mask, range_vector=None):
+    def _attn(self, query, key, value, attention_mask):
         """
         Get the weighted score along the seq_length
 
         Inputs:
             query: the query matrix
             key: the key matrix
             value: the value matrix
             attention_mask: the attention mask matrix with shape (batch_size,
             1, seq_length, seq_length)
-            range_vector: a range vector from 0 to seq_length with shape (batch_size, 1, seq_length)
         Returns:
             weighted_values: Tensor, the weighted sum scores
         """
+        # Normalize query and key before MatMul, default off
         if not self.scale:
             query = query / F.cast(self.coeff, F.dtype(query))
             key = key / F.cast(self.coeff, F.dtype(key))
 
+        # Attention score [bs, num_heads, seq_length_q, seq_length_k]
         score = self.batch_matmul(query, key)
+        # Normalize after query and key MatMul, default on
         if self.scale:
             score = self.real_div(
                 score,
                 P.Cast()(self.scale_factor, P.DType()(score)))
 
         ori_dtype = P.DType()(score)
         score = P.Cast()(score, mstype.float32)
 
+        # for input size of (bs, 1) namely the second graph, the shape of attention_mask matrix should be
+        # (bs, 1, 1, seq_length)
         if self.use_past and not self.is_first_iteration:
-            current_index = self.reducesum(F.cast(
-                self.not_equal(self.slice(key, (0, 0, 0, 0), (F.shape(query)[0], 1, 1, self.seq_length), (1, 1, 1, 1)),
-                               self.pad_value), mstype.float32), (1, 2, 3))
+            # Calculate the current total token
+            current_index = self.reducesum(F.cast(self.not_equal(self.slice(key, (0, 0, 0, 0),
+                                                                            (F.shape(query)[0], 1, 1, self.seq_length),
+                                                                            (1, 1, 1, 1)),
+                                                                 0), mstype.float32), (1, 2, 3))
+            # Get the precise position index
             index = self.sub1(F.cast(current_index, mstype.int32), 1)
             index = F.reshape(index, (-1, 1, 1))
-            index = self.expand_dims(index, 2)
-            attention_mask = F.cast(self.tensor_le(self.expand_dims(range_vector, 2), index), mstype.int32)
-
-            # attention_mask = F.cast(self.tensor_le(range_vector, index), mstype.int32)
-            # attentoin_mask = self.expand_dims(attention_mask, 2)
+            # Calculate the attention_mask matrix via the position index
+            attention_mask = F.cast(self.tensor_le(self.range, index), mstype.int32)
+            attention_mask = self.expand_dims(attention_mask, 2)
 
+        # Minus 10000 for the position where masked to exclude them from softmax
         multiplu_out = self.sub(
             P.Cast()(F.tuple_to_array((1.0,)), P.DType()(score)),
             P.Cast()(attention_mask, P.DType()(score)))
 
         adder = self.mul(multiplu_out, self.multiply_data)
         attention_scores = self.add(adder, score)
 
-        # attention_scores = P.Cast()(attention_scores, ori_dtype)
         shape = F.shape(attention_scores)
+        # attention probs
         attention_probs = self.softmax(
             F.reshape(attention_scores,
-                      (shape[0], -1, shape[-1])))  # yzz modify
+                      (shape[0], -1, shape[-1])))
         attention_probs = P.Cast()(attention_probs, ori_dtype)
         attention_probs = F.reshape(attention_probs, shape)
 
         attention_probs = self.prob_dropout(attention_probs)
+        # Weighted sum output [bs, num_heads, seq_length_q, size_per_head]
         weighted_values = self.batch_matmul(attention_probs, value)
         return weighted_values
 
 
-class Block(nn.Cell):
+class Decoder(nn.Cell):
     """
-    The basic block of GPT network
+    The basic decoder structure of PanguAlpha network
     Args:
-        config(GPTConfig): the config of network
+        config(PanguAlphaConfig): the config of network
         layer_idx: current layer index
     Inputs:
         x: the output of previous layer(input_ids for the first layer)
         attention_mask: the attention mask matrix with shape (batch_size, 1, seq_length, seq_length)
-        layer_past: the previous feature map
+        init_reset: whether reset the previous state
+        batch_valid_length: the valid input seq_length without padding
     Returns:
         output: Tensor, the output logit of this layer
         layer_present: Tensor, the feature map of current layer
     """
 
     def __init__(self, config, layer_idx):
-        super(Block, self).__init__()
+        super(Decoder, self).__init__()
         scale = 1 / math.sqrt(2.0 * config.num_layers)
-        # scale = 1.0
-        if config.self_layernorm:
-            self.layernorm1 = LayerNorm((config.embedding_size,), config.dp).to_float(mstype.float32)
-            self.layernorm2 = LayerNorm((config.embedding_size,), config.dp).to_float(mstype.float32)
-        else:
-            self.layernorm1 = nn.LayerNorm((config.embedding_size,)).to_float(mstype.float32)
-            self.layernorm1.layer_norm.shard(((config.dp, 1, 1), (1,), (1,)))
-            self.layernorm2 = nn.LayerNorm((config.embedding_size,)).to_float(mstype.float32)
-            self.layernorm2.layer_norm.shard(((config.dp, 1, 1), (1,), (1,)))
+        self.layernorm1 = LayerNorm((config.embedding_size,), config.dp).to_float(mstype.float32)
+        self.layernorm2 = LayerNorm((config.embedding_size,), config.dp).to_float(mstype.float32)
 
-        self.layernorm1.gamma.parallel_optimizer = False
-        self.layernorm1.beta.parallel_optimizer = False
         self.attention = Attention(config, scale, layer_idx)
-        self.layernorm2.gamma.parallel_optimizer = False
-        self.layernorm2.beta.parallel_optimizer = False
-        self.output = Output(config, scale)
+        # Feed Forward Network, FFN
+        self.output = FeedForwardLayer(config, scale)
         self.post_layernorm_residual = config.post_layernorm_residual
         self.add = P.TensorAdd().shard(((config.dp, 1, 1), (config.dp, 1, 1)))
-        self.last_add = P.TensorAdd().shard(
-            ((config.dp, 1, 1), (config.dp, 1,
-                                 1))).add_prim_attr("recompute", False)
+        # Last activation of this layer will be saved for recompute in backward process
         self.dtype = config.compute_dtype
-
-    def construct(self, x, input_mask, key_past=None, value_past=None, batch_valid_length=None):
+        self.use_past = config.use_past
+        if self.use_past:
+            # operator used for state reuse
+            self.reducesum = P.ReduceSum().shard(((1, 1, 1, 1),))
+            self.not_equal = P.NotEqual().shard(((1, 1, 1, 1), ()))
+            self.slice = P.StridedSlice().shard(((1, 1, 1, 1),))
+            size_per_head = int(config.embedding_size / config.num_heads)
+            self.key_shape = (config.batch_size, config.num_heads, size_per_head, config.seq_length)
+            self.value_shape = (config.batch_size, config.num_heads, config.seq_length, size_per_head)
+            # parameters saving key and value states
+            self.key_past = Parameter(Tensor(np.zeros(shape=self.key_shape), self.dtype), name="key_past")
+            self.value_past = Parameter(Tensor(np.zeros(shape=self.value_shape), self.dtype), name="value_past")
+            self.tile = P.Tile().shard(((1, 1),))
+            self.mul = P.Mul().shard(((1, 1, 1, 1), (1,)))
+            self.assign = P.Assign().shard(((1, 1, 1, 1), (1, 1, 1, 1)))
+
+    def construct(self, x, input_mask, init_reset=True, batch_valid_length=None):
+        r"""
+        The forward process of the block.
+        """
+        # [bs, seq_length, embedding_size]
         input_x = self.layernorm1(x)
         input_x = F.cast(input_x, self.dtype)
+
+        # indicate whether reset saved states
+        key_reset = None
+        value_reset = None
+
+        if self.use_past:
+            # reset states, init_reset True for reuse and False for reset
+            key_reset = self.assign(self.key_past, self.mul(self.key_past, F.cast(init_reset, self.dtype)))
+            value_reset = self.assign(self.value_past, self.mul(self.value_past, F.cast(init_reset, self.dtype)))
+            # add dependency for desired execution order
+            input_x = F.depend(input_x, key_reset)
+            input_x = F.depend(input_x, value_reset)
         attention, layer_present = self.attention(input_x, input_mask,
-                                                  key_past, value_past, batch_valid_length)
+                                                  self.key_past, self.value_past, batch_valid_length)
+        # For post-layernorm the inputs for residual path are output of self-attention and output of layernorm
         if self.post_layernorm_residual:
             x = self.add(input_x, attention)
+        # For pre-layernorm the inputs for residual path are output of self-attention and input of this layer
         else:
             x = self.add(x, attention)
 
         output_x = self.layernorm2(x)
         output_x = F.cast(output_x, self.dtype)
         mlp_logit = self.output(output_x)
+
+        value_update = None
+        key_update = None
+        if self.use_past:
+            # current key and value
+            key_present, value_present = layer_present
+            # update key and value calculated this step
+            key_update = self.assign(self.key_past, key_present)
+            value_update = self.assign(self.value_past, value_present)
+            # add dependency for desired execution order
+            key_update = F.depend(key_update, key_reset)
+            value_update = F.depend(value_update, value_reset)
+
+        # add dependency for desired execution order
+        mlp_logit = F.depend(mlp_logit, value_update)
+        mlp_logit = F.depend(mlp_logit, key_update)
         if self.post_layernorm_residual:
-            output = self.last_add(output_x, mlp_logit)
+            output = self.add(output_x, mlp_logit)
         else:
-            output = self.last_add(x, mlp_logit)
+            output = self.add(x, mlp_logit)
         return output, layer_present
 
 
+class Embedding(nn.Cell):
+    """
+    Embedding
+    """
+
+    def __init__(self, config):
+        super(Embedding, self).__init__()
+        self.word_embedding = EmbeddingLookup().set_comm_fusion(1)
+        if config.word_emb_dp:
+            self.word_embedding.gather.shard(((1, 1), (config.dp, 1)))
+        else:
+            self.word_embedding.gather.shard(((config.mp, 1), (1, 1)))
+        if config.stage_num > 1:
+            self.position_embedding = nn.Embedding(config.seq_length,
+                                                   config.embedding_size,
+                                                   embedding_table=Normal(0.02)).set_comm_fusion(1)
+        else:
+            # Position embedding
+            if config.load_ckpt_path:
+                # Loading the embedding table from the ckpt path:
+                embedding_path = os.path.join(config.load_ckpt_path, 'position_embedding.npy')
+                if os.path.exists(embedding_path):
+                    p_table = np.load(embedding_path)
+                    position_table_param = Tensor(p_table, mstype.float32)
+                else:
+                    raise ValueError(f"{embedding_path} file not exits, "
+                                     f"please check whether position_embedding file exit.")
+            else:
+                position_table_param = TruncatedNormal(0.02)
+            # Position embedding
+            self.position_embedding = nn.Embedding(
+                config.seq_length,
+                config.embedding_size,
+                embedding_table=position_table_param).set_comm_fusion(1)
+        self.position_embedding.embedding_table.parallel_optimizer = False
+        self.position_embedding.gather.shard(((1, 1), (config.dp,)))
+        self.position_embedding.expand.shard(((config.dp, 1),))
+        self.add = P.TensorAdd().shard(((config.dp, 1, 1), (config.dp, 1, 1)))
+        self.dropout = Dropout(1 - config.dropout_rate)
+        self.dropout.shard(((config.dp, 1, 1),))
+        self.use_past = config.use_past
+        self.is_first_iteration = True
+
+    def construct(self, input_ids, table, input_position, valid_index=None):
+        input_embedding = self.word_embedding(input_ids, table)
+        if self.use_past and not self.is_first_iteration:
+            _, seq_length = F.shape(input_ids)
+            input_position = valid_index.view(1, seq_length)
+        position_embedding = self.position_embedding(input_position)
+        hidden_states = self.add(input_embedding, position_embedding)
+        hidden_states = self.dropout(hidden_states)
+        hidden_states = P.Cast()(hidden_states, mstype.float16)
+        return hidden_states
+
+
+class Mask(nn.Cell):
+    """
+    Mask
+    """
+
+    def __init__(self, config):
+        super(Mask, self).__init__()
+        self.dtype = config.compute_dtype
+        self.expand_dims = P.ExpandDims().shard(((config.dp, 1, 1),))
+
+    def construct(self, attention_mask):
+        attention_mask = self.expand_dims(attention_mask, 1)
+        return attention_mask
+
+
 class QueryLayerAttention(Attention):
+    r"""
+    Self-Attention module using input query vector.
+    """
+
     def construct(self, x, query_hidden_state, attention_mask, key_past=None, value_past=None, batch_valid_length=None):
         original_shape = F.shape(x)
         x = F.reshape(x, (-1, original_shape[-1]))
         query_hidden_state = F.reshape(query_hidden_state, (-1, original_shape[-1]))
+        # For query_layer_attention, query are derived from outputs of previous layer and key, value are derived from an added parameter query_embedding
         query = self.dense1(query_hidden_state)
         key = self.dense2(x)
         value = self.dense3(x)
         query = self.transpose(
             F.reshape(
                 query,
                 (-1, original_shape[1], self.n_head, self.size_per_head)),
@@ -630,378 +740,384 @@
                 key, (-1, original_shape[1], self.n_head, self.size_per_head)),
             (0, 2, 3, 1))
         value = self.transpose(
             F.reshape(
                 value,
                 (-1, original_shape[1], self.n_head, self.size_per_head)),
             (0, 2, 1, 3))
+
         key_present = key
         value_present = value
-        range_vector = None
         if self.use_past:
-            range_vector = self.tile1(self.range, (original_shape[0], 1, 1))
+            # The first graph with the input size of (bs, seq_length)
             if self.is_first_iteration:
-                valid_length_vector = F.cast(self.less(range_vector, batch_valid_length), mstype.float16)
+                # Get the valid input length without padding
+                valid_length_vector = F.cast(self.less(self.range, batch_valid_length.view(1, 1, -1)), self.dtype)
+                # Cover the key and value numbers corresponding to the padding position
                 key_present = self.mul1(key, self.expand_dims(valid_length_vector, 2))
                 value_present = self.mul1(value, self.expand_dims(valid_length_vector, 3))
+            # The second graph with the inpus size of (bs, 1)
+            # the shape of query is (bs, num_heads, 1, size_per_head)
+            # the shape of key is   (bs, num_heads, size_per_head, 1)
+            # the shape of value is (bs, num_heads, 1, size_per_head)
             else:
-                valid_length = self.reducesum(F.cast(self.not_equal(
-                    self.slice(key_past, (0, 0, 0, 0), (original_shape[0], 1, 1, self.seq_length), (1, 1, 1, 1)),
-                    self.pad_value), mstype.float32), (1, 2, 3))
+                # Get the current token position index
+                valid_length = self.reducesum(F.cast(self.not_equal(self.slice(key_past, (0, 0, 0, 0),
+                                                                               (F.shape(x)[0], 1, 1, self.seq_length),
+                                                                               (1, 1, 1, 1)),
+                                                                    0), mstype.float32), (1, 2, 3))
                 valid_length = F.reshape(valid_length, (-1, 1, 1))
-                valid_length_vector = F.cast(self.equal(valid_length, range_vector), self.dtype)
+                valid_length_vector = F.cast(self.equal(valid_length, self.range), self.dtype)
+                # Pad the key and value to seq_length with only the position index not zero
                 current_key = self.mul1(self.tile(key, (1, 1, 1, self.seq_length)),
                                         self.expand_dims(valid_length_vector, 2))
                 current_value = self.mul1(self.tile(value, (1, 1, self.seq_length, 1)),
                                           self.expand_dims(valid_length_vector, 3))
+                # Concat the previous saved state and current state
                 key = self.add(key_past, current_key)
                 value = self.add(value_past, current_value)
+                # Update key_present and value_present for state update
                 key_present = key
                 value_present = value
+                attention_mask = F.reshape(self.attention_mask, (self.seq_length, self.seq_length, 1, 1))
         layer_present = (key_present, value_present)
-        attention = self._attn(query, key, value, attention_mask, range_vector)
+        attention = self._attn(query, key, value, attention_mask)
         attention_merge = self.merge_heads(attention)
         output = self.projection(attention_merge)
         output = self.dropout(output)
         return output, layer_present
 
 
 class QueryLayer(nn.Cell):
+    r"""
+    A block usingooked out position embedding as query vector.
+    This is used as the final block.
+    """
+
     def __init__(self, config):
         super(QueryLayer, self).__init__()
         scale = 1 / math.sqrt(2.0 * config.num_layers)
         self.layernorm1 = LayerNorm((config.embedding_size,), config.dp).to_float(mstype.float32)
         self.layernorm2 = LayerNorm((config.embedding_size,), config.dp).to_float(mstype.float32)
-        self.layernorm1.gamma.parallel_optimizer = False
-        self.layernorm1.beta.parallel_optimizer = False
         self.attention = QueryLayerAttention(config, scale)
-        self.layernorm2.gamma.parallel_optimizer = False
-        self.layernorm2.beta.parallel_optimizer = False
-        self.output = Output(config, scale)
+        self.output = FeedForwardLayer(config, scale)
         self.post_layernorm_residual = config.post_layernorm_residual
         self.add = P.TensorAdd().shard(((config.dp, 1, 1), (config.dp, 1, 1)))
-
-        self.last_add = P.TensorAdd().shard(
-            ((config.dp, 1, 1), (config.dp, 1,
-                                 1))).add_prim_attr("recompute", False)
         self.dtype = config.compute_dtype
-
-    def construct(self, x, query_hidden_state, input_mask, key_past=None, value_past=None, batch_valid_length=None):
+        self.use_past = config.use_past
+        if self.use_past:
+            # operator used for state reuse
+            self.reducesum = P.ReduceSum().shard(((1, 1, 1, 1),))
+            self.not_equal = P.NotEqual().shard(((1, 1, 1, 1), ()))
+            self.slice = P.StridedSlice().shard(((1, 1, 1, 1),))
+            size_per_head = int(config.embedding_size / config.num_heads)
+            self.key_shape = (config.batch_size, config.num_heads, size_per_head, config.seq_length)
+            self.value_shape = (config.batch_size, config.num_heads, config.seq_length, size_per_head)
+            # parameters saving key and value states
+            self.key_past = Parameter(Tensor(np.zeros(shape=self.key_shape), self.dtype), name="key_past")
+            self.value_past = Parameter(Tensor(np.zeros(shape=self.value_shape), self.dtype), name="value_past")
+            self.tile = P.Tile().shard(((1, 1),))
+            self.mul = P.Mul().shard(((1, 1, 1, 1), (1,)))
+            self.assign = P.Assign().shard(((1, 1, 1, 1), (1, 1, 1, 1)))
+
+    def construct(self, x, query_hidden_state, input_mask, init_reset=True, batch_valid_length=None):
+        r"""
+        Query Layer shares a similar structure with normal layer block
+        except that it is not a traditional self-attention.
+        """
         input_x = self.layernorm1(x)
         input_x = F.cast(input_x, self.dtype)
+
+        # indicate whether reset saved states
+        key_reset = None
+        value_reset = None
+
+        if self.use_past:
+            # reset states, init_reset True for reuse and False for reset
+            key_reset = self.assign(self.key_past, self.mul(self.key_past, F.cast(init_reset, self.dtype)))
+            value_reset = self.assign(self.value_past, self.mul(self.value_past, F.cast(init_reset, self.dtype)))
+            # add dependency for desired execution order
+            input_x = F.depend(input_x, key_reset)
+            input_x = F.depend(input_x, value_reset)
+
         attention, layer_present = self.attention(input_x,
                                                   query_hidden_state,
                                                   input_mask,
-                                                  key_past, value_past, batch_valid_length)
+                                                  self.key_past,
+                                                  self.value_past,
+                                                  batch_valid_length)
         if self.post_layernorm_residual:
             x = self.add(input_x, attention)
         else:
             x = self.add(x, attention)
 
         output_x = self.layernorm2(x)
         output_x = F.cast(output_x, self.dtype)
         mlp_logit = self.output(output_x)
+        value_update = None
+        key_update = None
+        if self.use_past:
+            # current key and value
+            key_present, value_present = layer_present
+            # update key and value calculated this step
+            key_update = self.assign(self.key_past, key_present)
+            value_update = self.assign(self.value_past, value_present)
+            # add dependency for desired execution order
+            key_update = F.depend(key_update, key_reset)
+            value_update = F.depend(value_update, value_reset)
+
+        # add dependency for desired execution order
+        mlp_logit = F.depend(mlp_logit, value_update)
+        mlp_logit = F.depend(mlp_logit, key_update)
+
         if self.post_layernorm_residual:
-            output = self.last_add(output_x, mlp_logit)
+            output = self.add(output_x, mlp_logit)
         else:
-            output = self.last_add(x, mlp_logit)
+            output = self.add(x, mlp_logit)
         return output, layer_present
 
 
+class PanguAlphaEmbedding(nn.Cell):
+    """
+    Input embedding, i.e., word embedding and position embedding
+    Args:
+        config(PanguAlphaConfig): the config of network
+    Inputs:
+        input_ids: the tokenized inputs with datatype int32
+        input_mask: the mask indicating whether each position is a valid input
+        input_position: the position index of each token
+        attention_mask: the attention_mask attention for self-attention module
+        valid_index: only used in incremental inference, the position index of current token
+    outputs:
+        hidden_states: Tensor, input embeddings
+        attention_mask: Tensor, attention_mask matrix
+        embedding_table: Tensor, embedding_table with shape of (vocab_size, embedding_size)
+    """
+
+    def __init__(self, config):
+        super(PanguAlphaEmbedding, self).__init__()
+        self.embedding = Embedding(config)
+        if config.stage_num > 1:
+            self.embedding.pipeline_stage = 0
+        self.mask = Mask(config)
+
+    def construct(self, input_ids, input_mask, table, input_position, attention_mask, valid_index=None):
+        """
+        Calculate input embeddings via input token ids and input position
+        """
+        hidden_states = self.embedding(input_ids, table, input_position, valid_index)
+        attention_mask = self.mask(attention_mask)
+        return hidden_states, attention_mask
+
+
 class PanguAlpha_Model(nn.Cell):
     """
-    The backbone of GPT network
+    The backbone of PanguAlpha network
     Args:
-        config(GPTConfig): the config of network
+        config(PanguAlphaConfig): the config of network
     Inputs:
         input_ids: the tokenized inputs with datatype int32
         input_mask: the mask indicating whether each position is a valid input
         layer_past: the previous feature map
     Returns:
         output_state: Tensor, the output logit of backbone
         present_layer: Tensor, the current feature map
         embedding_table: Tensor, the embedding table for the vocabulary
     """
 
     def __init__(self, config):
         super(PanguAlpha_Model, self).__init__()
-        self.get_attention_mask = AttentionMask(config)
-        self.word_embedding = EmbeddingLookup(config).set_comm_fusion(1)
-        try:
-            p_table = np.load('/cache/position_embedding.npy')
-            p_table = Tensor(p_table, mstype.float32)
-            print("###### loading Word embedding Table successed! ######")
-        except:
-            p_table = Tensor(np.ones([config.seq_length, config.embedding_size], dtype=np.float32))
-        self.position_embedding = nn.Embedding(
-            config.seq_length,
-            config.embedding_size,
-            embedding_table=p_table).set_comm_fusion(1)
-        self.word_embedding.embedding_table.parallel_optimizer = False
-        self.position_embedding.embedding_table.parallel_optimizer = False
-        self.position_embedding.gather.shard(((1, 1), (config.dp,)))
-        self.position_embedding.expand.shard(((config.dp, 1),))
-        # self.position_embedding.gather.shard(((config.mp, 1), (1,)))
-        # self.position_embedding.expand.shard(((1, 1),))
+        self.embedding = PanguAlphaEmbedding(config)
         self.blocks = nn.CellList()
-        fusion_group_num = 4
-        fusion_group_size = config.num_layers // fusion_group_num
-        fusion_group_size = max(fusion_group_size, 1)
-
-        num_layers = config.num_layers
-        if config.use_top_query_attention:
-            num_layers -= 1
-        self.num_layers = num_layers
-        print("After setting the layer is:", num_layers, flush=True)
-
-        for i in range(num_layers):
-            per_block = Block(config, i + 1).set_comm_fusion(int(i / fusion_group_size) + 2)
-            per_block.recompute()
-            per_block.attention.dropout.dropout.recompute(False)
-            per_block.attention.prob_dropout.dropout.recompute(False)
-            per_block.output.dropout.dropout.recompute(False)
-            per_block.attention.dropout.dropout.add_prim_attr("_side_effect", True)
-            per_block.attention.prob_dropout.dropout.add_prim_attr("_side_effect", True)
-            per_block.output.dropout.dropout.add_prim_attr("_side_effect", True)
-            self.blocks.append(per_block)
-
-        if config.self_layernorm:
-            self.layernorm = LayerNorm((config.embedding_size,), config.dp).to_float(
-                mstype.float32).set_comm_fusion(
-                int((num_layers - 1) / fusion_group_size) + 2)
-        else:
-            self.layernorm = nn.LayerNorm((config.embedding_size,)).to_float(
-                mstype.float32).set_comm_fusion(
-                int((num_layers - 1) / fusion_group_size) + 2)
-            self.layernorm.layer_norm.shard(((config.dp, 1, 1), (1,), (1,)))
-        self.layernorm.gamma.parallel_optimizer = False
-        self.layernorm.beta.parallel_optimizer = False
         self.use_past = config.use_past
-        self.past = tuple([None] * config.num_layers)
-        self.add = P.TensorAdd().shard(((config.dp, 1, 1), (config.dp, 1, 1)))
-        self.expand_dims = P.ExpandDims().shard(((config.dp, 1, 1),))
         self.dtype = config.compute_dtype
-        self.dropout = nn.Dropout(1 - config.dropout_rate)
-        self.dropout.dropout.shard(((config.dp, 1, 1),))
-        # self.dropout.dropout_gen_mask.shard(((config.dp, 1, 1),))
-        # self.dropout.dropout_do_mask.shard(((config.dp, 1, 1),))
-        self.eod_reset = config.eod_reset
-        if config.use_top_query_attention:
-            print("Using query layer...", flush=True)
-            try:
-                query_table = np.load('/cache/top_query_embedding.npy')
-                query_table = Tensor(query_table, mstype.float32)
-                print("###### loading Word embedding Table successed! ######")
-            except:
-                query_table = Tensor(np.ones([config.seq_length, config.embedding_size], dtype=np.float32))
-            self.top_query_embedding = nn.Embedding(config.seq_length, config.embedding_size, \
-                                                    embedding_table=query_table).set_comm_fusion(
-                int((config.num_layers - 1) / fusion_group_num) + 2)
-            self.top_query_embedding.embedding_table.parallel_optimizer = False
-            self.top_query_embedding.gather.shard(((1, 1), (config.dp,)))
-            self.top_query_embedding.expand.shard(((config.dp, 1),))
-            self.top_query_layer = QueryLayer(config)
-            if config.use_recompute:
-                self.top_query_layer.recompute()
-                self.top_query_layer.output.dropout.dropout.recompute(False)
-                self.top_query_layer.attention.dropout.dropout.recompute(False)
-                self.top_query_layer.attention.prob_dropout.dropout.recompute(False)
-                self.top_query_layer.output.dropout.dropout.add_prim_attr("_side_effect", True)
-                self.top_query_layer.attention.dropout.dropout.add_prim_attr("_side_effect", True)
-                self.top_query_layer.attention.prob_dropout.dropout.add_prim_attr("_side_effect", True)
-            #                 self.top_query_layer.output.dropout.dropout_gen_mask.recompute(False)
-            #                 self.top_query_layer.attention.dropout.dropout_gen_mask.recompute(False)
-            #                 self.top_query_layer.attention.prob_dropout.dropout_gen_mask.recompute(False)
-            #                 self.top_query_layer.output.dropout.dropout_gen_mask.add_prim_attr("_side_effect", True)
-            #                 self.top_query_layer.attention.dropout.dropout_gen_mask.add_prim_attr("_side_effect", True)
-            #                 self.top_query_layer.attention.prob_dropout.dropout_gen_mask.add_prim_attr("_side_effect", True)
-
-            self.top_query_layer.set_comm_fusion(int((config.num_layers - 1) / fusion_group_num) + 2)
-        self.use_top_query_attention = config.use_top_query_attention
-
-        if self.use_past:
-            self.pad_value = 0
-            self.size_per_head = int(config.embedding_size / config.num_heads)
-            key_past = np.zeros(
-                shape=(config.num_layers, config.batch_size, config.num_heads, self.size_per_head, config.seq_length))
-            value_past = np.zeros(
-                shape=(config.num_layers, config.batch_size, config.num_heads, config.seq_length, self.size_per_head))
-            self.dtype = config.compute_dtype
-            self.key_past = Parameter(Tensor(key_past, self.dtype), name="key_past")
-            self.value_past = Parameter(Tensor(value_past, self.dtype), name="value_past")
-            self.reducesum = P.ReduceSum().shard(((1, 1, 1, 1, 1),))
-            self.not_equal = P.NotEqual().shard(((1, 1, 1, 1, 1), ()))
-            self.slice = P.StridedSlice().shard(((1, 1, 1, 1, 1),))
-            self.expand_dims1 = P.ExpandDims().shard(((1, 1, 1, 1),))
-            self.update = P.ScatterUpdate().shard(((1, 1, 1, 1, 1), (1,), (1, 1, 1, 1, 1)))
-            self.num_heads = config.num_heads
-            self.seq_length = config.seq_length
-            self.mul = P.Mul().shard(((1, 1, 1, 1, 1), (1,)))
-            self.assign = P.Assign().shard(((1, 1, 1, 1, 1), (1, 1, 1, 1, 1)))
-            self.is_first_iteration = True
-            self.depend = P.Depend()
-
-    def construct(self, input_ids, input_mask, init_reset=True, batch_valid_length=None, input_position=None,
-                  attention_mask=None,
-                  layer_past=None):
-        """GPT model"""
-        if not self.use_past:
-            layer_past = self.past
-
-        input_embedding, embedding_table = self.word_embedding(input_ids)
-        if not self.eod_reset:
-            batch_size, seq_length = F.shape(input_ids)
-            input_position = F.tuple_to_array(F.make_range(seq_length))
-            input_position = P.Tile()(input_position, (batch_size, 1))
-            attention_mask = self.get_attention_mask(input_mask)
-
-        if self.use_past and not self.is_first_iteration:
-            index = self.reducesum(F.cast(self.not_equal(
-                self.slice(self.key_past, (0, 0, 0, 0, 0), (1, F.shape(input_ids)[0], 1, 1, self.seq_length),
-                           (1, 1, 1, 1, 1)), self.pad_value), mstype.float32), (0, 2, 3, 4))
-            index = F.cast(index, mstype.int32)
-            input_position = F.reshape(index, (-1, 1))
-        position_embedding = self.position_embedding(input_position)
-        hidden_states = self.add(input_embedding, position_embedding)
-        hidden_states = self.dropout(hidden_states)
-        hidden_states = P.Cast()(hidden_states, mstype.float16)
-        attention_mask = self.expand_dims(attention_mask, 1)
+        self.num_layers = config.num_layers
+        self.is_pipeline = (config.stage_num > 1)
+        if self.is_pipeline:
+            self.top_query_embedding_table = Parameter(initializer(TruncatedNormal(0.02),
+                                                                   [config.seq_length, config.embedding_size]),
+                                                       name='embedding_table', parallel_optimizer=False)
+            self.top_query_embedding = EmbeddingLookup()
+            for i in range(config.num_layers):
+                if i == config.num_layers - 1:
+                    self.top_query_embedding_table.comm_fusion = 2
+                    self.top_query_embedding_table.add_pipeline_stage(i * config.stage_num // config.num_layers)
+                    per_block = QueryLayer(config).set_comm_fusion(2)
+                else:
+                    per_block = Decoder(config, i + 1).set_comm_fusion(2)
+                per_block.pipeline_stage = i * config.stage_num // config.num_layers
+                per_block.recompute()
+                self.blocks.append(per_block)
+
+            self.layernorm = LayerNorm((config.embedding_size,), config.dp).to_float(mstype.float32)
+            self.layernorm.set_comm_fusion(2)
+            self.layernorm.pipeline_stage = config.stage_num - 1
+        else:
+            # The input_position representing the position ids will be used as the index
+            # for a query embedding table to obtain top query hidden states, together with the previous outputs of normal
+            # self-attention layers, a new attention layer will be attached to the output of the model
+            if config.load_ckpt_path:
+                # Loading the embedding table from the ckpt path:
+                embedding_path = os.path.join(config.load_ckpt_path, 'top_query_embedding.npy')
+                if os.path.exists(embedding_path):
+                    top_query_table = np.load(embedding_path)
+                    top_query_table_param = Tensor(top_query_table, mstype.float32)
+                else:
+                    raise ValueError(
+                        f"{embedding_path} file not exits, please check whether top_query_embedding file exist.")
+            else:
+                top_query_table_param = TruncatedNormal(0.02)
+            self.top_query_embedding_table = Parameter(initializer(top_query_table_param,
+                                                                   [config.seq_length, config.embedding_size]),
+                                                       name='embedding_table', parallel_optimizer=False)
+            self.top_query_embedding = EmbeddingLookup()
+            # Total fusion groups for HCCL operators. Specifically, the same tyep HCCL operators in same group will be fused.
+            fusion_group_num = 4
+            fusion_group_size = config.num_layers // fusion_group_num
+            fusion_group_size = max(fusion_group_size, 1)
+            for i in range(config.num_layers-1):
+                per_block = Decoder(config, i + 1).set_comm_fusion(int(i / fusion_group_size) + 2)
+                # Each layer will be remoputed in the backward process. The output activation of each layer will be saved,
+                # in other words, in backward process each block will be almosttotally recomputed.
+                per_block.recompute()
+                self.blocks.append(per_block)
+            self.layernorm = LayerNorm((config.embedding_size,), config.dp).to_float(mstype.float32)
+            self.layernorm.set_comm_fusion(int((config.num_layers - 1) / fusion_group_size) + 2)
+
+            self.top_query_layer = QueryLayer(config).set_comm_fusion(
+                int((config.num_layers - 1) / fusion_group_size) + 2)
+            self.top_query_layer.recompute()
+            self.top_query_embedding_table.comm_fusion = int((config.num_layers - 1) / fusion_group_size) + 2
+        self.top_query_embedding.gather.shard(((1, 1), (config.dp,)))
+
+    def construct(self, input_ids, input_mask, table, input_position, attention_mask,
+                  init_reset=True, batch_valid_length=None):
+        """PanguAlpha model"""
+        # embedding for input_ids and the lower triangle like attention_mask matrix
+        hidden_states, attention_mask = self.embedding(input_ids, input_mask, table,
+                                                       input_position, attention_mask,
+                                                       batch_valid_length)
+        for i in range(self.num_layers - 1):
+            hidden_states, _ = self.blocks[i](hidden_states,
+                                              attention_mask, init_reset, batch_valid_length)
+        if self.is_pipeline:
+            top_query_hidden_states = self.top_query_embedding(input_position.view(-1,),
+                                                               self.top_query_embedding_table)
+            hidden_states, _ = self.blocks[self.num_layers - 1](hidden_states, top_query_hidden_states,
+                                                                attention_mask, init_reset, batch_valid_length)
+            output_state = self.layernorm(hidden_states)
+            output_state = F.cast(output_state, self.dtype)
+        else:
+            output_state = self.layernorm(hidden_states)
+            output_state = F.cast(output_state, self.dtype)
+            top_query_hidden_states = self.top_query_embedding(input_position.view(-1,), self.top_query_embedding_table)
+            output_state, _ = self.top_query_layer(output_state, top_query_hidden_states,
+                                                   attention_mask, init_reset, batch_valid_length)
+        return output_state
 
-        a = None
-        b = None
-        if self.use_past:
-            a = self.assign(self.key_past, self.mul(self.key_past, F.cast(init_reset, self.dtype)))
-            b = self.assign(self.value_past, self.mul(self.value_past, F.cast(init_reset, self.dtype)))
-        present_layer = ()
-        for i in range(self.num_layers):
-            key_past = None
-            value_past = None
-            if self.use_past:
-                key_past = self.slice(self.key_past, (i, 0, 0, 0, 0), (
-                    i + 1, F.shape(input_ids)[0], self.num_heads, self.size_per_head, self.seq_length), (1, 1, 1, 1, 1))
-                value_past = self.slice(self.value_past, (i, 0, 0, 0, 0), (
-                    i + 1, F.shape(input_ids)[0], self.num_heads, self.seq_length, self.size_per_head), (1, 1, 1, 1, 1))
-                key_past = F.reshape(key_past,
-                                     (F.shape(input_ids)[0], self.num_heads, self.size_per_head, self.seq_length))
-                value_past = F.reshape(value_past,
-                                       (F.shape(input_ids)[0], self.num_heads, self.seq_length, self.size_per_head))
-            hidden_states, present = self.blocks[i](hidden_states,
-                                                    attention_mask, key_past, value_past, batch_valid_length)
-            key_present, value_present = present
-
-            if self.use_past:
-                c = self.update(self.key_past, F.reshape(P.ScalarToTensor()(i, mstype.int32), (1,)),
-                                self.expand_dims1(key_present, 0))
-                d = self.update(self.value_past, F.reshape(P.ScalarToTensor()(i, mstype.int32), (1,)),
-                                self.expand_dims1(value_present, 0))
-                tmp_ac = self.depend(a, c)
-                tmp_bd = self.depend(b, d)
-        output_state = self.layernorm(hidden_states)
-        output_state = F.cast(output_state, self.dtype)
-        if self.use_top_query_attention:
-            key_past = None
-            value_past = None
-            i = self.num_layers
-            if self.use_past:
-                key_past = self.slice(self.key_past, (i, 0, 0, 0, 0), (
-                    i + 1, F.shape(input_ids)[0], self.num_heads, self.size_per_head, self.seq_length), (1, 1, 1, 1, 1))
-                value_past = self.slice(self.value_past, (i, 0, 0, 0, 0), (
-                    i + 1, F.shape(input_ids)[0], self.num_heads, self.seq_length, self.size_per_head), (1, 1, 1, 1, 1))
-                key_past = F.reshape(key_past,
-                                     (F.shape(input_ids)[0], self.num_heads, self.size_per_head, self.seq_length))
-                value_past = F.reshape(value_past,
-                                       (F.shape(input_ids)[0], self.num_heads, self.seq_length, self.size_per_head))
-            # top_query_hidden_states = self.top_query_embedding(input_position_seq)
-            top_query_hidden_states = self.top_query_embedding(input_position)
-            output_state, present = self.top_query_layer(output_state, top_query_hidden_states,
-                                                         attention_mask, key_past, value_past, batch_valid_length)
-            key_present, value_present = present
-
-            if self.use_past:
-                c = self.update(self.key_past, F.reshape(P.ScalarToTensor()(i, mstype.int32), (1,)),
-                                self.expand_dims1(key_present, 0))
-                d = self.update(self.value_past, F.reshape(P.ScalarToTensor()(i, mstype.int32), (1,)),
-                                self.expand_dims1(value_present, 0))
-                tmp_ac = self.depend(a, c)
-                tmp_bd = self.depend(b, d)
-        return output_state, present_layer, embedding_table
 
-class PanGuHead(nn.Cell):
+class PanguAlpha_Head(nn.Cell):
     """
-    Head for GPT to get the logits of each token in the vocab
+    Head for PanguAlpha to get the logits of each token in the vocab
     Args:
-        config(GPTConfig): the config of network
+        config(PanguAlphaConfig): the config of network
     Inputs:
         state: the output of the backbone
         embedding_table: the embedding table of the vocabulary
     Returns:
         logits: Tensor, the logits of the corresponding inputs
     """
 
     def __init__(self, config):
-        super(PanGuHead, self).__init__()
+        super(PanguAlpha_Head, self).__init__()
         if config.word_emb_dp:
             self.matmul = P.MatMul(transpose_b=True).shard(((config.dp, 1), (1, 1)))
         else:
-            self.matmul = P.MatMul(transpose_b=True).shard(((config.dp, config.mp), (1, config.mp)))
+            self.matmul = P.MatMul(transpose_b=True).shard(((config.dp, 1), (config.mp, 1)))
         self.embedding_size = config.embedding_size
         self.log_softmax = P.LogSoftmax(axis=-1)
         self.dtype = config.compute_dtype
         self.cast = P.Cast()
 
     def construct(self, state, embedding_table):
         state = P.Reshape()(state, (-1, self.embedding_size))
+        # output logits over vocabulary [bs*seq_length, vocab_size]
         logits = self.matmul(state, self.cast(embedding_table, self.dtype))
         return logits
 
 
-class PanguAlphaModel(nn.Cell):
+class PanguAlpha(nn.Cell):
     """
-    The GPT network consisting of two parts the backbone and the head
+    The PanguAlpha network consisting of two parts the backbone and the head
     Args:
-        config(GPTConfig): the config of network
+        config(PanguAlphaConfig): the config of network
     Inputs:
         input_ids: the tokenized inputs
         input_mask: the mask indicating whether each position is a valid input
         past: the previous feature map
     Returns:
         logits: Tensor: the logits of the corresponding inputs with shape (batch_size, seq_length, vocab_size)
     """
 
     def __init__(self, config):
-        super(PanguAlphaModel, self).__init__()
+        super(PanguAlpha, self).__init__()
+        # Network head to get logits over vocabulary
+        self.head = PanguAlpha_Head(config)
+        self.vocab_size = config.vocab_size
+        self.embedding_size = config.embedding_size
         self.backbone = PanguAlpha_Model(config)
-        self.head = PanGuHead(config)
+        if config.stage_num > 1:
+
+            self.head.pipeline_stage = config.stage_num - 1
+            self.embedding_table = Parameter(initializer(Normal(0.02), [self.vocab_size, self.embedding_size]),
+                                             name="embedding_table", parallel_optimizer=False)
+            self.embedding_table.add_pipeline_stage(self.backbone.blocks[0].pipeline_stage)
+            self.embedding_table.add_pipeline_stage(self.head.pipeline_stage)
+        else:
+            if config.load_ckpt_path:
+                # Loading the embedding table from the ckpt path:
+                embedding_path = os.path.join(config.load_ckpt_path, 'word_embedding.npy')
+                if os.path.exists(embedding_path):
+                    e_table = np.load(embedding_path)
+                    e_table = Tensor(e_table, mstype.float32)
+                    self.embedding_table = Parameter(e_table, name="embedding_table", parallel_optimizer=False)
+                else:
+                    raise ValueError(f"{embedding_path} file not exits, "
+                                     f"please check whether word_embedding file exist.")
+            else:
+                self.embedding_table = Parameter(initializer(Normal(0.02), [self.vocab_size, self.embedding_size]),
+                                                 name="embedding_table", parallel_optimizer=False)
 
-    def construct(self, input_ids, input_mask, init_reset=True, batch_valid_length=None, input_position=None,
-                  attention_mask=None, past=None):
-        output_states, _, embedding_table = self.backbone(
-            input_ids, input_mask, init_reset, batch_valid_length, input_position, attention_mask, past)
-        logits = self.head(output_states, embedding_table)
+    def construct(self, input_ids, input_mask, input_position, attention_mask,
+                  init_reset=True, batch_valid_length=None):
+        output_states = self.backbone(input_ids, input_mask, self.embedding_table,
+                                      input_position, attention_mask, init_reset, batch_valid_length)
+        logits = self.head(output_states, self.embedding_table)
         return logits
 
 
 class CrossEntropyLoss(nn.Cell):
     """
     Calculate the cross entropy loss
     Args:
-        config(GPTConfig): the config of the network
+        config(PanguAlphaConfig): the config of the network
     Inputs:
         logits: the output logits of the backbone
         label: the ground truth label of the sample
         input_mask: the mask indicating whether each position is a valid input
     Returns:
         loss: Tensor, the corrsponding cross entropy loss
     """
 
     def __init__(self, config):
         super(CrossEntropyLoss, self).__init__()
         self.mean = P.ReduceMean()
         self.sum = P.ReduceSum().shard(((config.dp, config.mp),))
         self.onehot = P.OneHot().shard(((config.dp, config.mp), (), ()))
+        # on/off value for onehot, for smooth labeling, modify the off_value
         self.on_value = Tensor(1.0, mstype.float32)
         self.off_value = Tensor(0.0, mstype.float32)
         self.vocab_size = config.vocab_size
         self.max = P.ArgMaxWithValue(axis=-1, keep_dims=True).shard(
             ((config.dp, config.mp),))
         self.eps_const = Tensor(1e-24, mstype.float32)
         self.sub = P.Sub().shard(((config.dp, config.mp), (config.dp, 1)))
@@ -1015,164 +1131,203 @@
         self.sum2 = P.ReduceSum().shard(((1,),))
 
         self.mul2 = P.Mul().shard(((1,), (1,)))
         self.add2 = P.TensorAdd()
         self.div2 = P.RealDiv()
 
     def construct(self, logits, label, input_mask):
+        r"""
+        Compute loss using logits, label and input mask
+        """
+        # [bs*seq_length, vocab_size]
         logits = F.cast(logits, mstype.float32)
+        # LogSoftmax for logits over last dimension
         _, logit_max = self.max(logits)
         logit_sub = self.sub(logits, logit_max)
         logit_exp = self.exp(logit_sub)
         exp_sum = self.sum(logit_exp, -1)
         exp_sum = P.Reshape()(exp_sum, (F.shape(exp_sum)[0], 1))
         softmax_result = self.div(logit_exp, exp_sum)
         log_softmax_result = self.log(self.add(softmax_result, self.eps_const))
+
+        # Flatten label to [bs*seq_length]
         label = P.Reshape()(label, (-1,))
+        # Get onehot label [bs*seq_length, vocab_size]
         one_hot_label = self.onehot(label, self.vocab_size, self.on_value,
                                     self.off_value)
+        # Cross-Entropy loss
         loss = self.mul(log_softmax_result, one_hot_label)
         loss_unsum = self.neg(loss)
         loss_reduce = self.sum(loss_unsum, -1)
+        # input_mask indicates whether there is padded inputs and for padded inputs it will not be counted into loss
         input_mask = P.Reshape()(input_mask, (-1,))
         numerator = self.sum2(self.mul2(loss_reduce, input_mask))
 
         denominator = self.add2(
             self.sum2(input_mask),
             P.Cast()(F.tuple_to_array((1e-5,)), mstype.float32))
         loss = self.div2(numerator, denominator)
         return loss
 
 
-class PanGuAlphaWithLoss(nn.Cell):
+class PanguAlphaWithLoss(nn.Cell):
     """
-    GPT training loss
+    PanguAlpha training loss
     Args:
-        network: backbone network of GPT2/3
+        network: backbone network of PanguAlpha
         loss: loss function, e.g., crossentropy
         eos_token: the end_of_sentence token
     Inputs:
         input_ids: the tokenized inputs
         past: the previous feature map
     Returns:
         output: Tensor, the loss of the network
     """
 
     def __init__(self, config, network, loss, eos_token=6):
-        super(PanGuAlphaWithLoss, self).__init__(auto_prefix=False)
+        super(PanguAlphaWithLoss, self).__init__(auto_prefix=False)
         self.network = network
         self.loss = loss
         self.eos_token = eos_token
         self.slice = P.StridedSlice().shard(((config.dp, 1),))
         self.not_equal = P.NotEqual().shard(((config.dp, 1), ()))
         self.batch_size = config.batch_size
         self.len = config.seq_length
-        self.eod_reset = config.eod_reset
-        if self.eod_reset:
-            self.slice_mask = P.StridedSlice().shard(((config.dp, 1, 1),))
-
-    def construct(self, input_ids, input_position=None, attention_mask=None):
-        # tokens = input_ids[:, :-1]
-        tokens = self.slice(input_ids, (0, 0), (self.batch_size, -1), (1, 1))
-
-        if self.eod_reset:
-            input_position = self.slice(input_position, (0, 0), (self.batch_size, self.len), (1, 1))
-            attention_mask = self.slice_mask(attention_mask, (0, 0, 0),
-                                             (self.batch_size, self.len, self.len),
-                                             (1, 1, 1))
-
-        input_mask = F.cast(self.not_equal(tokens, self.eos_token),
-                            mstype.float32)
+        self.micro_batch_step = 1
+        if config.stage_num > 1:
+            self.micro_batch_step = config.micro_size
+
+    def construct(self, input_ids, input_position, attention_mask):
+        tokens = self.slice(input_ids, (0, 0), (self.batch_size // self.micro_batch_step, -1), (1, 1))
+        input_mask = F.cast(self.not_equal(tokens, self.eos_token), mstype.float32)
+        
+        # input_position = self.slice(input_position, (0, 0), (self.batch_size, self.len), (1, 1))
+        # attention_mask = self.slice_mask(attention_mask, (0, 0, 0),
+        #                                  (self.batch_size, self.len, self.len),
+        #                                  (1, 1, 1))
+        
         logits = self.network(tokens, input_mask, input_position, attention_mask)
-        # labels = input_ids[:, 1:]
-        labels = self.slice(input_ids, (0, 1), (self.batch_size, self.len + 1),
-                            (1, 1))
+        labels = self.slice(input_ids, (0, 1), (self.batch_size // self.micro_batch_step,
+                                                self.len + 1), (1, 1))
         output = self.loss(logits, labels, input_mask)
         return output
 
-
-class EvalNet(nn.Cell):
+class PanguAlphaWithLoss_eval_nli(nn.Cell):
     """
-    GPT evaluation net
+    PanguAlpha training loss
     Args:
-        backbone: backbone network of GPT2/3
-        generate: enable generate mode
-        topk_num: the number of topk selection
+        network: backbone network of PanguAlpha
+        loss: loss function, e.g., crossentropy
+        eos_token: the end_of_sentence token
     Inputs:
-        input_ids: the tokenized inpus
-        init_reset: whether to reset key_past and value_past for incremental inference
-        batch_valid_length: the original valid sentence length of the first graph for incremental inference
+        input_ids: the tokenized inputs
+        past: the previous feature map
     Returns:
-        outputs: Tensor, corresponding output for different tasks
+        output: Tensor, the loss of the network
     """
 
-    def __init__(self, backbone, generate=False, topk_num=3, pad_token=9):
-        super(EvalNet, self).__init__(auto_prefix=False)
-        self.backbone = backbone
-        self.argmax = P.Argmax()
-        self.generate = generate
-        self.topk = P.TopK(sorted=True).shard(((1, 1, 1),))
-        self.not_equal = P.NotEqual().shard(((1, 1), ()))
-        self.topk_num = topk_num
-        self.pad_token = pad_token  # config.pad_token
-
-    def construct(self, input_ids, init_reset=True, batch_valid_length=None):
-        """
-            evaluation net
-            input_ids: bs x seq_length
-        """
-        input_mask = F.cast(self.not_equal(input_ids, self.pad_token), mstype.float32)
-        logits = self.backbone(input_ids, input_mask, init_reset, batch_valid_length)
-        bs, seq_length = F.shape(input_ids)
-        logits = F.reshape(logits, (bs, seq_length, -1))
-        value, index = self.topk(logits, self.topk_num)
-        return value, index
-
+    def __init__(self, config, network, loss, eos_token=6):
+        super(PanguAlphaWithLoss_eval_nli, self).__init__(auto_prefix=False)
+        self.network = network
+        self.loss = loss
+        self.eos_token = eos_token
+        self.slice = P.StridedSlice().shard(((config.dp, 1),))
+        self.not_equal = P.NotEqual().shard(((config.dp, 1), ()))
+        self.batch_size = config.batch_size
+        self.len = config.seq_length
+        self.micro_batch_step = 1
+        if config.stage_num > 1:
+            self.micro_batch_step = config.micro_size
 
-class EvalNet_p(nn.Cell):
+    def construct(self, input_ids, input_position=None, attention_mask=None):
+        tokens = self.slice(input_ids, (0, 0), (self.batch_size // self.micro_batch_step, -1), (1, 1))
+        input_mask = F.cast(self.not_equal(tokens, self.eos_token), mstype.float32)
+        
+        input_position = self.slice(input_position, (0, 0), (self.batch_size, self.len), (1, 1))
+        attention_mask = self.slice_mask(attention_mask, (0, 0, 0),
+                                         (self.batch_size, self.len, self.len),
+                                         (1, 1, 1))
+        
+        logits = self.network(tokens, input_mask, input_position, attention_mask)
+        labels = self.slice(input_ids, (0, 1), (self.batch_size // self.micro_batch_step,
+                                                self.len + 1), (1, 1))
+        output = self.loss(logits, labels, input_mask)
+        return output
+    
+class PanguAlphaWithLoss_eval(nn.Cell):
     """
-    GPT evaluation net
+    GPT training loss
     Args:
-        backbone: backbone network of GPT2/3
-        generate: enable generate mode
-        topk_num: the number of topk selection
+        network: backbone network of GPT2/3
+        loss: loss function, e.g., crossentropy
+        eos_token: the end_of_sentence token
     Inputs:
-        input_ids: the tokenized inpus
-        init_reset: whether to reset key_past and value_past for incremental inference
-        batch_valid_length: the original valid sentence length of the first graph for incremental inference
+        input_ids: the tokenized inputs
+        past: the previous feature map
     Returns:
-        outputs: Tensor, corresponding output for different tasks
+        output: Tensor, the loss of the network
     """
+    def __init__(self, config, network, loss, eos_token=128297):
+        super(PanguAlphaWithLoss_eval, self).__init__(auto_prefix=False)
+        self.network = network
+        self.loss = loss
+        self.eos_token = eos_token
+        self.slice = P.StridedSlice().shard(((config.dp, 1),))
+        self.not_equal = P.NotEqual().shard(((config.dp, 1), ()))
+        self.batch_size = config.batch_size
+        self.len = config.seq_length
+        self.slice_mask = P.StridedSlice().shard(((config.dp, 1, 1),))
+            
+    def construct(self, input_ids, mask_ids_input, input_position=None, attention_mask=None):
+        #tokens = input_ids[:, :-1]
+        tokens = self.slice(input_ids, (0, 0), (self.batch_size, -1), (1, 1))
+        
+        input_position = self.slice(input_position, (0, 0), (self.batch_size, self.len), (1, 1))
+        attention_mask = self.slice_mask(attention_mask, (0, 0, 0),
+                                         (self.batch_size, self.len, self.len),
+                                         (1, 1, 1))
+            
+        input_mask = F.cast(self.not_equal(tokens, self.eos_token), mstype.float32)
+        logits = self.network(tokens, input_mask, input_position, attention_mask)
+        #labels = input_ids[:, 1:]
+        labels = self.slice(input_ids, (0, 1), (self.batch_size, self.len + 1), (1, 1))
+        output = self.loss(logits, labels, mask_ids_input)
+        return output
 
-    def __init__(self, backbone, generate=False, pad_token=9, topk_num=3):
-        super(EvalNet_p, self).__init__(auto_prefix=False)
-        self.backbone = backbone
-        self.argmax = P.Argmax()
-        self.generate = generate
-        self.not_equal = P.NotEqual().shard(((1, 1), ()))
-        self.log_max = P.LogSoftmax().shard(((1, 1, 1),))
-        self.topk_num = topk_num
-        self.pad_token = pad_token  # config.pad_token
+class AttentionMask(nn.Cell):
+    """
+    Get the attention matrix for self-attention module
+    Args:
+        seq_length: the pre-defined sequence length
+    Inputs:
+        input_mask: the mask indicating whether each position is a valid input
+    Returns:
+        attention_mask: the attention mask matrix with shape (batch_size, seq_length, seq_length)
+    """
 
-    def construct(self, input_ids, init_reset=True, batch_valid_length=None):
-        """
-            evaluation net
-            input_ids: bs x seq_length
-        """
-        input_mask = F.cast(self.not_equal(input_ids, self.pad_token), mstype.float32)
-        logits = self.backbone(input_ids, input_mask, init_reset, batch_valid_length)
-        bs, seq_length = F.shape(input_ids)
+    def __init__(self, seq_length):
+        super(AttentionMask, self).__init__()
+        self.reshape = P.Reshape()
+        self.mul = P.BatchMatMul().shard(
+            ((1, 1, 1), (1, 1, 1)))
+        self.expand_dim = P.ExpandDims().shard(((1, 1),))
+        ones = np.ones(shape=(seq_length, seq_length))
+        self.lower_triangle_mask = Tensor(np.tril(ones), mstype.float32)
+        self.multiply = P.Mul().shard(((1, 1, 1), (1, 1, 1)))
 
-        logits = F.reshape(logits, (bs, seq_length, -1))
-        if self.generate:
-            outputs = self.log_max(logits)
-            outputs = F.tensor_pow(np.e, outputs)
-        else:
-            outputs = self.argmax(logits)
-        return outputs
+    def construct(self, input_mask):
+        input_shape = P.Shape()(input_mask)
+        shape_right = (input_shape[0], 1, input_shape[1])
+        shape_left = input_shape + (1,)
+        mask_left = self.reshape(input_mask, shape_left)
+        mask_right = self.reshape(input_mask, shape_right)
+        attention_mask = self.mul(mask_left, mask_right)
+        lower_triangle = self.expand_dim(self.lower_triangle_mask, 0)
+        attention_mask = self.multiply(attention_mask, lower_triangle)
+        return attention_mask
 
 
 class EvalNet(nn.Cell):
     """
     PanguAlpha evaluation net
     Args:
         backbone: backbone network of PanguAlpha
@@ -1201,12 +1356,12 @@
         input_mask = F.cast(F.not_equal(input_ids, self.pad_token), mstype.float32)
         bs, seq_length = F.shape(input_ids)
         attention_mask = self.get_attention_mask(input_mask)
         input_position = F.tuple_to_array(F.make_range(seq_length))
         input_position = P.Tile()(input_position, (bs, 1))
         logits = self.backbone(input_ids, input_mask, input_position, attention_mask,
                                init_reset, batch_valid_length)
-        index = current_index.view(1, )
+        index = current_index.view(1,)
         logits = self.gather(logits, index, 0)
         logits = logits.view(bs, 1, -1)
         log_probs = self.log_softmax(logits)
-        return log_probs
+        return log_probs
```

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_config.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,14 @@
                  num_layers=12,
                  num_heads=12,
                  expand_ratio=4,
                  post_layernorm_residual=False,
                  dropout_rate=0.1,
                  compute_dtype=mstype.float16,
                  use_past=False,
-                 self_layernorm=True,
                  word_emb_dp=True,
                  stage_num=16,
                  eod_reset=True,
                  micro_size=32,
                  load_ckpt_path='/cache/ckpt_file',
                  use_top_query_attention=False,
                  param_init_type=mstype.float32):
@@ -56,15 +55,14 @@
         self.post_layernorm_residual = post_layernorm_residual
         self.dropout_rate = dropout_rate
         self.compute_dtype = compute_dtype
         # Whether use incremental inference
         self.use_past = use_past
         self.dp = data_parallel_num
         self.mp = model_parallel_num
-        self.self_layernorm = self_layernorm
         self.stage_num = stage_num
         self.micro_size = micro_size
         self.word_emb_dp = word_emb_dp
         self.eod_reset = eod_reset
         self.use_top_query_attention = use_top_query_attention
         self.param_init_type = param_init_type
         # Used for loading embedding tables
```

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_wrapcell.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_wrapcell.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/preprocess.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/preprocess.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/serialization.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/serialization.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/tokenization_jieba.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/tokenization_jieba.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/src/utils_pangu.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/utils_pangu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_mindspore/train_alpha_ms13.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/train_alpha_ms13.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from mindspore.parallel import set_algo_parameters
 from mindspore.parallel._cost_model_context import _set_multi_subgraphs
 from mindspore.nn.wrap.cell_wrapper import PipelineCell, _VirtualDatasetCell
 from mindspore.train.callback import ModelCheckpoint, CheckpointConfig
 from mindspore.train.serialization import load_checkpoint, load_param_into_net
 
 from src.dataset import create_dataset
-from src.pangu_alpha import PanguAlphaModel, PanGuAlphaWithLoss, CrossEntropyLoss
+from src.pangu_alpha import PanguAlpha, PanguAlphaWithLoss, CrossEntropyLoss
 from src.pangu_alpha_wrapcell import PanguAlphaTrainOneStepWithLossScaleCell
 from src.pangu_alpha_config import PANGUALPHAConfig, set_parse
 from src.utils_pangu import LearningRate, get_args, FP32StateAdamWeightDecay
 from src.utils_pangu import download_data, get_openi_tar, ckpt_tar_openi, ckpt_copy_tar_new, get_ckpt_file_list
 from src.utils_pangu import StrategySaveCallback, CheckpointSaveCallback
 
 try:
@@ -285,17 +285,17 @@
         eod_reset=bool(args_opt.eod_reset), 
         load_ckpt_path=local_npy_path,
         param_init_type=mstype.float32 if args_opt.param_init_type == 'fp32' else mstype.float16,
         word_emb_dp=bool(args_opt.word_emb_dp))
     print("===config is: ", config, flush=True)
 
     # Define network
-    pangu_alpha = PanguAlphaModel(config)
+    pangu_alpha = PanguAlpha(config)
     loss = CrossEntropyLoss(config)
-    pangu_alpha_with_loss = PanGuAlphaWithLoss(config, pangu_alpha, loss)
+    pangu_alpha_with_loss = PanguAlphaWithLoss(config, pangu_alpha, loss)
     pangu_alpha_with_loss = _VirtualDatasetCell(pangu_alpha_with_loss)
 
     # Warm-up and cosine decay learning rate
     lr = LearningRate(learning_rate=args_opt.start_lr, end_learning_rate=args_opt.end_lr,
                       warmup_steps=args_opt.warmup_step, decay_steps=args_opt.decay_steps)
 
     # Set weight decay coefficient, zero for bias and layernorm, 1e-1 for rest
@@ -452,24 +452,23 @@
         mp = args_opt.op_level_model_parallel_num
         # load mp slice modelWeight
 
         if rank_id % 8 == 0:
             maxStepNumber = find_local_ckpt_maxStepNumber(save_dir_rank)
 
             sliced_parameters = []
-
             for i in range(mp):
 
-                save_ckptfile_name = args_opt.ckpt_name_prefix + '_' + str(i)
-                save_dir_rank = os.path.join(args_opt.save_checkpoint_path, f"rank_{i}")
+                save_dir_rank = os.path.join(args_opt.save_checkpoint_path, f"rank_{rank_id}")
                 os.system("ls {}".format(save_dir_rank))
+                save_ckptfile_name = args_opt.ckpt_name_prefix + '_' + str(rank_id)
                 # model_prefix = os.path.join(save_dir_rank, "alpha-2B6_{}-{}_2.ckpt".format(i, maxStepNumber))
                 model_prefix = os.path.join(save_dir_rank, "{}-{}_2.ckpt".format(save_ckptfile_name, maxStepNumber))
-                param_dict = ms.load_checkpoint(model_prefix)
 
+                param_dict = ms.load_checkpoint(model_prefix)
                 adam_names = [item for item in param_dict.keys() if 'adam' in item]
                 for item in adam_names:
                     param_dict.pop(item)
                 param_dict.pop("scale_sense")
                 param_dict.pop("global_step")
                 param_dict.pop("current_iterator_step")
                 param_dict.pop("last_overflow_iterator_step")
```

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference-en.md` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference-en.md`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference.md` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference.md`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/LICENSE` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/LICENSE`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/README-en.md` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/README-en.md`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/README.md` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/README.md`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/README_mgt.md` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/README_mgt.md`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/__init__.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/__init__.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/arguments.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/arguments.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/checkpointing.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/checkpointing.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/bert_dataset.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/bert_dataset.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/dataset_utils.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/gpt2_dataset.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/gpt2_dataset.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/helpers.cpp` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/helpers.cpp`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/ict_dataset.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/ict_dataset.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/indexed_dataset.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_dataset_utils.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_index.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_index.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/data/samplers.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/samplers.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/__init__.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/__init__.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16util.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16util.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/loss_scaler.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/loss_scaler.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/__init__.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.cpp` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.h` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax_cuda.cu` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/global_vars.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/global_vars.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/indexer.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/indexer.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/initialize.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/initialize.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/learning_rates.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/learning_rates.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/memory.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/memory.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/__init__.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/alpha_enhanced_model.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/alpha_enhanced_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/bert_model.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/bert_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/classification.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/classification.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/distributed.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/distributed.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_bias_gelu.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_bias_gelu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_softmax.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_softmax.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/gpt2_model.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/gpt2_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/language_model.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/language_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/mpu_utils.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/mpu_utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/multiple_choice.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/realm_model.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/realm_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/transformer.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/transformer.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/model/utils.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/module.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/module.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/__init__.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/__init__.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/cross_entropy.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/data.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/data.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/grads.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/grads.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/initialize.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/initialize.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/layers.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/layers.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/mappings.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/mappings.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/random.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/random.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/utils.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/package_info.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/package_info.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/text_generation_utils.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/text_generation_utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/__init__.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/bert_tokenization.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/bert_tokenization.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/gpt2_tokenization.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/gpt2_tokenization.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenization_jieba.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenization_jieba.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenizer.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/training.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/training.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/megatron/utils.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/mergeMpCkpt.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/mergeMpCkpt.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/pretrain_bert.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_bert.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/pretrain_evolution.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_evolution.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/pretrain_gpt2.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_gpt2.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/pretrain_ict.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_ict.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/setup.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/setup.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/testLayerNorm.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/testLayerNorm.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/change_MspCkpt_ToMgt.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/change_MspCkpt_ToMgt.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/create_doc_index.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/create_doc_index.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_Pangu.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_Pangu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_epangu.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_epangu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/linter.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/linter.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/merge_mp_partitions.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/merge_mp_partitions.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/preprocess_data_pangu.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/preprocess_data_pangu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/splitMergedCkpt_v0.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/splitMergedCkpt_v0.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model/panguAlpha_pytorch/tools/split_full_model_into_mp_model.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/split_full_model_into_mp_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model_converter/_numpy_ckpt_2_pytorch.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model_converter/_numpy_ckpt_2_pytorch.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model_converter/merge_pytorch_model.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model_converter/merge_pytorch_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model_converter/ms_2_numpy.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model_converter/ms_2_numpy.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model_converter/numpy_2_pt.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model_converter/numpy_2_pt.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/model_converter/split_pytorch_model.py` & `pcl_pangu-1.2.5.9/pcl_pangu/model_converter/split_pytorch_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/online/infer/infer.py` & `pcl_pangu-1.2.5.9/pcl_pangu/online/infer/infer.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/online/infer/pangu_alpha_dto.py` & `pcl_pangu-1.2.5.9/pcl_pangu/online/infer/pangu_alpha_dto.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/online/infer/pangu_evolution_dto.py` & `pcl_pangu-1.2.5.9/pcl_pangu/online/infer/pangu_evolution_dto.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/online/modelinfo/modelinfo.py` & `pcl_pangu-1.2.5.9/pcl_pangu/online/modelinfo/modelinfo.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/conver_pt_onnx.py` & `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/conver_pt_onnx.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/infer.py` & `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/infer.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/pangu/config.py` & `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/config.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/pangu/model.py` & `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/pangu/model_onnx_gpu.py` & `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/model_onnx_gpu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/pangu/sample.py` & `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/sample.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/pangu/utils.py` & `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/onnx_inference/test.py` & `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/test.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.model` & `pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.model`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.vocab` & `pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.vocab`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/spm_13w/data_dict.128k.txt` & `pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/data_dict.128k.txt`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/spm_13w/spm.128k.model.1` & `pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/spm.128k.model.1`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/spm_13w/tokenizer.py` & `pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu/tokenizer/tokenization_jieba.py` & `pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/tokenization_jieba.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/pcl_pangu.egg-info/SOURCES.txt` & `pcl_pangu-1.2.5.9/pcl_pangu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.8/setup.py` & `pcl_pangu-1.2.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
  'loguru>=0.3.0']
 
 extras_require = \
 {':python_version < "3.7"': ['dataclasses==0.6']}
 
 setup_kwargs = {
     'name': 'pcl_pangu',
-    'version': '1.2.5.8',
+    'version': '1.2.5.9',
     'description': 'pcl_pangu',
     'long_description': '# pcl_pangu ',
     'author': '2022 PCL',
     'author_email': 'pcl.openi@pcl.ac.cn',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://openi.pcl.ac.cn/PCL-Platform.Intelligence/pcl_pangu',
```

