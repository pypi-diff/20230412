# Comparing `tmp/SwissArmyTransformer-0.2.9.tar.gz` & `tmp/SwissArmyTransformer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SwissArmyTransformer-0.2.9.tar", last modified: Sat Jul 16 16:39:48 2022, max compression
+gzip compressed data, was "/home/mingding/SwissArmyTransformer/dist/.tmp-z934vhzp/SwissArmyTransformer-0.3.1.tar", last modified: Wed Apr 12 06:44:49 2023, max compression
```

## Comparing `SwissArmyTransformer-0.2.9.tar` & `SwissArmyTransformer-0.3.1.tar`

### file list

```diff
@@ -1,126 +1,137 @@
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:48.014370 SwissArmyTransformer-0.2.9/
--rw-rw-r--   0 dingming  (1015) dingming  (1015)    11338 2022-06-01 10:13:56.000000 SwissArmyTransformer-0.2.9/LICENSE
--rw-rw-r--   0 dingming  (1015) dingming  (1015)      142 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/MANIFEST.in
--rw-rw-r--   0 dingming  (1015) dingming  (1015)     9484 2022-07-16 16:39:48.014370 SwissArmyTransformer-0.2.9/PKG-INFO
--rw-rw-r--   0 dingming  (1015) dingming  (1015)     9112 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/README.md
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.986369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)      179 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/__init__.py
--rwxr-xr-x   0 dingming  (1015) dingming  (1015)    20596 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/arguments.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.986369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/data_utils/
--rwxrwxrwx   0 dingming  (1015) dingming  (1015)      288 2022-06-01 10:13:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/data_utils/__init__.py
--rwxr-xr-x   0 dingming  (1015) dingming  (1015)    13317 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/data_utils/configure_data.py
--rwxrwxrwx   0 dingming  (1015) dingming  (1015)     2459 2022-06-09 18:53:16.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/data_utils/datasets.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     1852 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/data_utils/hf_dataset.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     7028 2022-06-09 19:04:59.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/data_utils/samplers.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.986369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/
--rwxrwxrwx   0 dingming  (1015) dingming  (1015)        0 2022-06-01 10:13:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/__init__.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     5606 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/autoregressive_sampling.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     3218 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/cuda2d_sampling.py
--rwxrwxrwx   0 dingming  (1015) dingming  (1015)     1709 2022-06-01 10:13:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/magnify.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.990369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/sampling_strategies/
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)      161 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/sampling_strategies/__init__.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     2899 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/sampling_strategies/base_strategy.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     4990 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/sampling_strategies/beam_search_strategy.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     2270 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/sampling_strategies/iterative_entfilter_strategy.py
--rwxr-xr-x   0 dingming  (1015) dingming  (1015)     2819 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/utils.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.990369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)      201 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/__init__.py
--rwxr-xr-x   0 dingming  (1015) dingming  (1015)     7356 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/base_model.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     1770 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/cached_autoregressive_model.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     5560 2022-06-18 08:06:02.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/encoder_decoder_model.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.990369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/finetune/
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)      187 2022-06-17 13:32:48.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/finetune/__init__.py
--rw-rw-r--   0 dingming  (1015) dingming  (1015)     2676 2022-06-17 13:32:48.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/finetune/adapter.py
--rw-rw-r--   0 dingming  (1015) dingming  (1015)     2036 2022-06-17 13:32:48.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/finetune/ffadd.py
--rw-rw-r--   0 dingming  (1015) dingming  (1015)     3930 2022-06-17 13:32:48.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/finetune/lora.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     1127 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/finetune/mlp_head.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     1638 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/finetune/prompt_tuning.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)      367 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/mixins.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.994369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/
--rwxr-xr-x   0 dingming  (1015) dingming  (1015)      307 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/__init__.py
--rw-rw-r--   0 dingming  (1015) dingming  (1015)     1883 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/bert_model.py
--rw-rw-r--   0 dingming  (1015) dingming  (1015)    10594 2022-06-18 08:06:02.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/cait_model.py
--rw-rw-r--   0 dingming  (1015) dingming  (1015)     7466 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/clip_model.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     9782 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/cuda2d_model.py
--rw-rw-r--   0 dingming  (1015) dingming  (1015)      779 2022-06-22 05:56:10.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/distill_model.py
--rw-r--r--   0 dingming  (1015) dingming  (1015)    13981 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/glm130B_model.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     3803 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/glm_model.py
--rw-rw-r--   0 dingming  (1015) dingming  (1015)     8455 2022-06-17 15:49:40.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/mae_model.py
--rw-rw-r--   0 dingming  (1015) dingming  (1015)      279 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/roberta_model.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)    14851 2022-06-18 08:06:02.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/t5_model.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     8876 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/vit_model.py
--rw-rw-r--   0 dingming  (1015) dingming  (1015)     3020 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/yolos_model.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.994369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/position_embedding/
--rw-r--r--   0 dingming  (1015) dingming  (1015)      296 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/position_embedding/__init__.py
--rw-r--r--   0 dingming  (1015) dingming  (1015)     5303 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/position_embedding/rotary_embeddings.py
--rw-rw-r--   0 dingming  (1015) dingming  (1015)     4078 2022-06-17 15:49:40.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/position_embedding/sincos2d.py
--rwxr-xr-x   0 dingming  (1015) dingming  (1015)    26407 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/transformer.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.994369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     1776 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/__init__.py
--rwxrwxrwx   0 dingming  (1015) dingming  (1015)     4716 2022-06-01 10:13:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/cross_entropy.py
--rwxrwxrwx   0 dingming  (1015) dingming  (1015)     4018 2022-06-01 10:13:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/data.py
--rwxrwxrwx   0 dingming  (1015) dingming  (1015)     4884 2022-06-01 10:13:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/initialize.py
--rwxr-xr-x   0 dingming  (1015) dingming  (1015)    14251 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/layers.py
--rwxrwxrwx   0 dingming  (1015) dingming  (1015)     4136 2022-06-01 10:13:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/mappings.py
--rwxrwxrwx   0 dingming  (1015) dingming  (1015)     3483 2022-06-07 12:48:02.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/utils.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.994369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/ops/
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)      264 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/ops/__init__.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)      582 2022-06-16 06:33:26.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/ops/layernorm.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     2067 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/ops/local_attention_function.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.994369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/resources/
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)       33 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/resources/__init__.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     1956 2022-06-18 08:06:02.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/resources/download.py
--rw-r--r--   0 dingming  (1015) dingming  (1015)     2029 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/resources/urls.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.994369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/
--rwxr-xr-x   0 dingming  (1015) dingming  (1015)     3621 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/__init__.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.994369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)      303 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/__init__.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     5092 2022-06-12 07:33:18.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/sp_tokenizer.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     1767 2022-06-12 07:33:18.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/templates.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     7095 2022-06-12 07:33:18.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/unified_tokenizer.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.998370 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/vqvae/
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)      167 2022-06-12 07:33:18.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/vqvae/__init__.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     7691 2022-06-12 07:33:18.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/vqvae/api.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)    30392 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/vqvae/vqvae_diffusion.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)    12917 2022-06-12 07:33:18.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/vqvae/vqvae_zc.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     2453 2022-06-12 07:33:18.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/vqvae_tokenizer.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.986369 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.998370 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/chinese_sentencepiece/
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)  1021864 2022-06-12 07:33:18.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)   723078 2022-06-12 07:33:18.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:48.010370 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/english_tokenizer/
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)   231508 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)   231508 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)   456318 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)  1042301 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)   456318 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)   898823 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:48.010370 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/glm/
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)       63 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/glm/__init__.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     3272 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/glm/sp_tokenizer.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)    18774 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/glm/tokenization.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)    13843 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/glm/tokenization_gpt2.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     3206 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/hf_tokenizer.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:48.010370 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/icetk_glm_130B/
--rw-r--r--   0 dingming  (1015) dingming  (1015)       40 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/icetk_glm_130B/__init__.py
--rw-r--r--   0 dingming  (1015) dingming  (1015)     2805 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/icetk_glm_130B/ice_tokenizer.py
--rw-r--r--   0 dingming  (1015) dingming  (1015)     2295 2022-07-16 16:30:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/icetk_glm_130B/tokenizer.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:48.014370 SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)      109 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/__init__.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)    23362 2022-06-20 09:07:27.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/deepspeed_training.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)      355 2022-06-27 04:08:10.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/deepspeed_zero0.json
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)      970 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/deepspeed_zero1.json
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     1029 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/deepspeed_zero2.json
--rwxrwxrwx   0 dingming  (1015) dingming  (1015)     3432 2022-06-01 10:13:56.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/learning_rates.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     8267 2022-06-22 05:56:10.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/model_io.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     4384 2022-06-09 19:03:57.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/utils.py
--rwxrwxr-x   0 dingming  (1015) dingming  (1015)     7581 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer/transformer_defaults.py
-drwxrwxr-x   0 dingming  (1015) dingming  (1015)        0 2022-07-16 16:39:47.986369 SwissArmyTransformer-0.2.9/SwissArmyTransformer.egg-info/
--rw-rw-r--   0 dingming  (1015) dingming  (1015)     9484 2022-07-16 16:39:47.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer.egg-info/PKG-INFO
--rw-rw-r--   0 dingming  (1015) dingming  (1015)     5151 2022-07-16 16:39:47.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 dingming  (1015) dingming  (1015)        1 2022-07-16 16:39:47.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 dingming  (1015) dingming  (1015)       65 2022-07-16 16:39:47.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer.egg-info/requires.txt
--rw-rw-r--   0 dingming  (1015) dingming  (1015)       21 2022-07-16 16:39:47.000000 SwissArmyTransformer-0.2.9/SwissArmyTransformer.egg-info/top_level.txt
--rw-rw-r--   0 dingming  (1015) dingming  (1015)       64 2022-06-15 15:10:07.000000 SwissArmyTransformer-0.2.9/requirements.txt
--rw-rw-r--   0 dingming  (1015) dingming  (1015)       38 2022-07-16 16:39:48.014370 SwissArmyTransformer-0.2.9/setup.cfg
--rw-r--r--   0 dingming  (1015) dingming  (1015)      880 2022-07-16 16:38:39.000000 SwissArmyTransformer-0.2.9/setup.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.3.1/LICENSE
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      125 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/MANIFEST.in
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9446 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9074 2023-04-12 06:44:14.000000 SwissArmyTransformer-0.3.1/README.md
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.200191 SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9446 2023-04-12 06:44:49.000000 SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3924 2023-04-12 06:44:49.000000 SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-04-12 06:44:49.000000 SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       65 2023-04-12 06:44:49.000000 SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/requires.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-04-12 06:44:49.000000 SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/top_level.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       64 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/requirements.txt
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.200191 SwissArmyTransformer-0.3.1/sat/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      179 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23055 2023-04-12 06:10:30.000000 SwissArmyTransformer-0.3.1/sat/arguments.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.200191 SwissArmyTransformer-0.3.1/sat/data_utils/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/data_utils/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15216 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/data_utils/configure_data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3720 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/data_utils/datasets.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1852 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/data_utils/hf_dataset.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/data_utils/samplers.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.200191 SwissArmyTransformer-0.3.1/sat/generation/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5653 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/autoregressive_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/cuda2d_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/magnify.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.200191 SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2899 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/base_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4990 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/beam_search_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3183 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/generation/utils.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3484 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/helpers.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.200191 SwissArmyTransformer-0.3.1/sat/model/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      201 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    11487 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/base_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1753 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/cached_autoregressive_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5492 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/encoder_decoder_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.204191 SwissArmyTransformer-0.3.1/sat/model/finetune/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/finetune/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/finetune/adapter.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/finetune/ffadd.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/finetune/lora.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/finetune/mlp_head.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1604 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/finetune/prompt_tuning.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      367 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/mixins.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.204191 SwissArmyTransformer-0.3.1/sat/model/official/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      598 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/official/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1882 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/bert_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/cait_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    11755 2023-04-11 14:19:47.000000 SwissArmyTransformer-0.3.1/sat/model/official/chatglm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7337 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/clip_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9680 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/cuda2d_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-11 14:26:12.000000 SwissArmyTransformer-0.3.1/sat/model/official/distill_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/dpr_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7364 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/eva2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    14109 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/glm130B_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3786 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/glm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3488 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/gpt2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/gptneo_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/mae_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/roberta_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/t5_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     8842 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/vit_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/yolos_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.204191 SwissArmyTransformer-0.3.1/sat/model/position_embedding/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/position_embedding/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5441 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/position_embedding/rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/position_embedding/sincos2d.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/position_embedding/vision_rotary_embeddings.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    26381 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/transformer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.204191 SwissArmyTransformer-0.3.1/sat/mpu/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1776 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/cross_entropy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4884 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/initialize.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14251 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/layers.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/mappings.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3483 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/utils.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.204191 SwissArmyTransformer-0.3.1/sat/ops/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      264 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/ops/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      582 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/ops/layernorm.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/ops/local_attention_function.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.208191 SwissArmyTransformer-0.3.1/sat/resources/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/resources/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1956 2023-04-11 13:31:52.000000 SwissArmyTransformer-0.3.1/sat/resources/download.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2881 2023-04-11 13:31:52.000000 SwissArmyTransformer-0.3.1/sat/resources/urls.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.208191 SwissArmyTransformer-0.3.1/sat/tokenization/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3822 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/tokenization/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.208191 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/templates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/unified_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.208191 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/api.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/vqvae_zc.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.196191 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.208191 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/chinese_sentencepiece/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.212191 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/sat/tokenization/glm/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/glm/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/glm/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/glm/tokenization.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/glm/tokenization_gpt2.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/glm/tokenization_wordpiece.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/hf_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/sat/tokenization/icetk_glm_130B/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/icetk_glm_130B/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/icetk_glm_130B/tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/sat/training/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      109 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/training/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23474 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/training/deepspeed_training.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      354 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/training/deepspeed_zero0.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      970 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/training/deepspeed_zero1.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1029 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/training/deepspeed_zero2.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3432 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/training/learning_rates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9271 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/training/model_io.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4431 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/training/utils.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7479 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/transformer_defaults.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/setup.cfg
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-04-12 06:38:10.000000 SwissArmyTransformer-0.3.1/setup.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/tests/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-11 14:34:16.000000 SwissArmyTransformer-0.3.1/tests/test_base_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/tests/test_list_info.py
```

### Comparing `SwissArmyTransformer-0.2.9/LICENSE` & `SwissArmyTransformer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/PKG-INFO` & `SwissArmyTransformer-0.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.2.9
+Version: 0.3.1
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Introduction
-`SwissArmyTransformer` is a flexible and powerful library to develop your own Transformer variants.
+`sat`(`SwissArmyTransformer`) is a flexible and powerful library to develop your own Transformer variants.
 
-`SwissArmyTransformer` is named after "swiss army knife", meaning that all the models (e.g. BERT, GPT, T5, GLM, CogView, ViT...) **share the same backone code** and cater for versatile usages with some extra light-weight mixins. 
+`sat` is named after "swiss army knife", meaning that all the models (e.g. BERT, GPT, T5, GLM, CogView, ViT...) **share the same backone code** and cater for versatile usages with some extra light-weight mixins. 
+
+`sat` is powered by `deepspeed-ZeRO` and model parallelism, aiming to provide the best practice for pretraining and finetuning large models (100M\~20B parameters). 
+
+# Migrate from SwissArmyTransformer 0.2.x to 0.3.x
+1. delete all `--sandwich-ln` in you script, use `layernorm-order='sandwich'`.
+2. change order `from_pretrained(args, name) => from_pretrained(name, args)`.
 
-`SwissArmyTransformer` is powered by `deepspeed-ZeRO` and model parallelism, aiming to provide the best practice for pretraining and finetuning large models (100M\~20B parameters). 
 ## Install
 ```
     pip install SwissArmyTransformer
 ```
 # Features
 
 * **Add model-agnostic components**, e.g. prefix-tuning, in just *ONE* line! 
@@ -34,19 +39,19 @@
                 # Arm an arbitrary model with Prefix-tuning with this line!
                 self.add_mixin('prefix-tuning', PrefixTuningMixin(args.num_layers, args.hidden_size // args.num_attention_heads, args.num_attention_heads, args.prefix_len))
     ```
 
     - GPT and other auto-regressive models act differently during training and inference. During inference, text is generated token-by-token and we need to cache previous states for efficiency. With our lib, you only need to consider the behavior during training (teacher-forcing) and transform it to a cached auto-regressive model via adding a mixin:
 
     ```python
-        model, args = AutoModel.from_pretrained(args, 'glm-10b-chinese')
+        model, args = AutoModel.from_pretrained('glm-10b-chinese', args)
         model.add_mixin('auto-regressive', CachedAutoregressiveMixin())
         # Generate a sequence with beam search
-        from SwissArmyTransformer.generation.autoregressive_sampling import filling_sequence
-        from SwissArmyTransformer.generation.sampling_strategies import BeamSearchStrategy
+        from sat.generation.autoregressive_sampling import filling_sequence
+        from sat.generation.sampling_strategies import BeamSearchStrategy
         output, *mems = filling_sequence(model, input_seq,
                         batch_size=args.batch_size,
                         strategy=BeamSearchStrategy(args.batch_size))
     ```     
 
 
 * **Build your Transformer-based model with minimal codes**. We mentioned [GLM](https://arxiv.org/pdf/2103.10360.pdf), which only differs from standard transformer (called BaseModel) on position embedding (and training losses). We only need to focus on the related part when coding.
@@ -74,66 +79,66 @@
         def __init__(self, args, transformer=None, parallel_output=True):
             super().__init__(args, transformer=transformer, parallel_output=parallel_output)
             self.add_mixin('block_position_embedding', 
                 BlockPositionEmbeddingMixin(args.max_sequence_length, args.hidden_size)
             ) # Add the mixin for GLM
     ```
 
-*  **Comprehensive supports for training**. `SwissArmyTransformer` aims to provide the best practice for pretraining and finetuning, where you only need to finish `forward_step` and `create_dataset_function` but with hyperparameters to alter useful training configurations.
+*  **Comprehensive supports for training**. `sat` aims to provide the best practice for pretraining and finetuning, where you only need to finish `forward_step` and `create_dataset_function` but with hyperparameters to alter useful training configurations.
     - Extend the training to multiple GPUs or nodes by specifying `--num_nodes`, `--num_gpus` and a simple `hostfile`. 
     - DeepSpeed and Model parallelism.
     - Better integration of ZeRO-2 and activation checkpointing.
     - Automatic extending and shuffling training data and `memmap`. 
     - Successfully support the training of [CogView2](http://github.com/THUDM/CogView2) and [CogVideo](https://github.com/THUDM/cogvideo).
     - The only open-source codebase supporting finetuning [T5-10B](https://arxiv.org/abs/1910.10683) on GPUs currently.
 
 </p></details>
 
 
 # Quick Tour
 
-The most typical python file to use `Bert` in SwissArmyTransformer (for inference) is as follows:
+The most typical python file to use `Bert` in sat (for inference) is as follows:
 ```python
 # @File: inference_bert.py
-from SwissArmyTransformer import get_args, get_tokenizer, AutoModel
+from sat import get_args, get_tokenizer, AutoModel
 # Parse args, initialize the environment. This is necessary.
 args = get_args() 
 # Automatically download and load model. Will also dump model-related hyperparameters to args.
-model, args = AutoModel.from_pretrained(args, 'bert-base-uncased') 
+model, args = AutoModel.from_pretrained('bert-base-uncased', args) 
 # Get the BertTokenizer according to args.tokenizer_type (automatically set).
 tokenizer = get_tokenizer(args) 
 # Here to use bert as you want!
 # ...
 ```
 Then we can run the code via
 ```bash
     SAT_HOME=/path/to/download python inference_bert.py --mode inference
 ```
-All officially supported model names are in [urls.py](SwissArmyTransformer/resources/urls.py).
+All officially supported model names are in [urls.py](sat/resources/urls.py).
 
 To finetune or pretrain a transformer is also extremely easy!
 ```python
 # @File: finetune_bert.py
-from SwissArmyTransformer import get_args, get_tokenizer, AutoModel
-from SwissArmyTransformer.model.mixins import MLPHeadMixin
+from sat import get_args, get_tokenizer, AutoModel
+from sat.model.mixins import MLPHeadMixin
 
 def create_dataset_function(path, args):
     # Here to load the dataset
     # ...
     assert isinstance(dataset, torch.utils.data.Dataset)
     return dataset
 
 def forward_step(data_iterator, model, args, timers):
     inputs = next(data_iterator) # from the dataset of create_dataset_function.
     loss, *others = model(inputs)
     return loss
     
 # Parse args, initialize the environment. This is necessary.
 args = get_args() 
-model, args = AutoModel.from_pretrained(args, 'bert-base-uncased') 
+model, args = AutoModel.from_pretrained('bert-base-uncased', args) 
 tokenizer = get_tokenizer(args) 
 # Here to use bert as you want!
 model.del_mixin('bert-final')
 model.add_mixin('classification_head', MLPHeadMixin(args.hidden_size, 2048, 1))
 # ONE LINE to train! 
 # args already includes hyperparams such as lr, train-iters, zero-stage ...
 training_main(args, 
@@ -150,34 +155,34 @@
     --train-data /path/to/train --valid-data /path/to/valid \
     --lr 0.00002 --batch-size 8 --zero-stage 1 --fp16
 ```
 Here we use data-parallel on GPUs 0,1. We can also launch the training on many inter-connected machines via `--hostfile /path/to/hostfile`. See the tutorial for more details.
 
 To write your own model, you only need to consider the difference between the standard Transformer. For example, if you have a idea to improve the attention operation:
 ```python
-from SwissArmyTransformer.model import BaseMixin
+from sat.model import BaseMixin
 class MyAttention(BaseMixin):
     def __init__(self, hidden_size):
         super(MyAttention, self).__init__()
         # MyAttention may needs some new params, e.g. a learnable alpha.
         self.learnable_alpha = torch.nn.Parameter(torch.ones(hidden_size))
     
     # This is a hook function, the name `attention_fn` is special.
     def attention_fn(q, k, v, mask, dropout=None, **kwargs):
         # Code for my attention.
         # ...
         return attention_results
 ```
-Here `attention_fn` is a hook function, replacing the default action by the new function. All available hooks are in [transformer_defaults.py](/SwissArmyTransformer/transformer_defaults.py). 
+Here `attention_fn` is a hook function, replacing the default action by the new function. All available hooks are in [transformer_defaults.py](/sat/transformer_defaults.py). 
 Now we can use `add_mixin` to apply our change to all the transformers, such as BERT, Vit and CogView. See the tutorial for more details. 
 
 ## Tutorials 
 TO BE RELEASED SOON...
 
 # Citation
 Currently we don't have a paper, so you don't need to formally cite us!~ 
 
-If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/SwissArmyTransformer}` to mention us and recommend `SwissArmyTransformer` to others.
+If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/sat}` to mention us and recommend `sat` to others.
 
-The tutorial for contributing SwissArmyTransformer is on the way!
+The tutorial for contributing sat is on the way!
 
 The project is based on (a user of) DeepSpeed, Megatron-LM and Huggingface transformers. Thanks for their awesome work.
```

### Comparing `SwissArmyTransformer-0.2.9/README.md` & `SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,30 @@
+Metadata-Version: 2.1
+Name: SwissArmyTransformer
+Version: 0.3.1
+Summary: A transformer-based framework with finetuning as the first class citizen.
+Home-page: https://github.com/THUDM/SwissArmyTransformer
+Author: Ming Ding, et al.
+Author-email: dm_thu@qq.com
+License: Apache 2.0 license
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Introduction
-`SwissArmyTransformer` is a flexible and powerful library to develop your own Transformer variants.
+`sat`(`SwissArmyTransformer`) is a flexible and powerful library to develop your own Transformer variants.
+
+`sat` is named after "swiss army knife", meaning that all the models (e.g. BERT, GPT, T5, GLM, CogView, ViT...) **share the same backone code** and cater for versatile usages with some extra light-weight mixins. 
+
+`sat` is powered by `deepspeed-ZeRO` and model parallelism, aiming to provide the best practice for pretraining and finetuning large models (100M\~20B parameters). 
 
-`SwissArmyTransformer` is named after "swiss army knife", meaning that all the models (e.g. BERT, GPT, T5, GLM, CogView, ViT...) **share the same backone code** and cater for versatile usages with some extra light-weight mixins. 
+# Migrate from SwissArmyTransformer 0.2.x to 0.3.x
+1. delete all `--sandwich-ln` in you script, use `layernorm-order='sandwich'`.
+2. change order `from_pretrained(args, name) => from_pretrained(name, args)`.
 
-`SwissArmyTransformer` is powered by `deepspeed-ZeRO` and model parallelism, aiming to provide the best practice for pretraining and finetuning large models (100M\~20B parameters). 
 ## Install
 ```
     pip install SwissArmyTransformer
 ```
 # Features
 
 * **Add model-agnostic components**, e.g. prefix-tuning, in just *ONE* line! 
@@ -22,19 +39,19 @@
                 # Arm an arbitrary model with Prefix-tuning with this line!
                 self.add_mixin('prefix-tuning', PrefixTuningMixin(args.num_layers, args.hidden_size // args.num_attention_heads, args.num_attention_heads, args.prefix_len))
     ```
 
     - GPT and other auto-regressive models act differently during training and inference. During inference, text is generated token-by-token and we need to cache previous states for efficiency. With our lib, you only need to consider the behavior during training (teacher-forcing) and transform it to a cached auto-regressive model via adding a mixin:
 
     ```python
-        model, args = AutoModel.from_pretrained(args, 'glm-10b-chinese')
+        model, args = AutoModel.from_pretrained('glm-10b-chinese', args)
         model.add_mixin('auto-regressive', CachedAutoregressiveMixin())
         # Generate a sequence with beam search
-        from SwissArmyTransformer.generation.autoregressive_sampling import filling_sequence
-        from SwissArmyTransformer.generation.sampling_strategies import BeamSearchStrategy
+        from sat.generation.autoregressive_sampling import filling_sequence
+        from sat.generation.sampling_strategies import BeamSearchStrategy
         output, *mems = filling_sequence(model, input_seq,
                         batch_size=args.batch_size,
                         strategy=BeamSearchStrategy(args.batch_size))
     ```     
 
 
 * **Build your Transformer-based model with minimal codes**. We mentioned [GLM](https://arxiv.org/pdf/2103.10360.pdf), which only differs from standard transformer (called BaseModel) on position embedding (and training losses). We only need to focus on the related part when coding.
@@ -62,66 +79,66 @@
         def __init__(self, args, transformer=None, parallel_output=True):
             super().__init__(args, transformer=transformer, parallel_output=parallel_output)
             self.add_mixin('block_position_embedding', 
                 BlockPositionEmbeddingMixin(args.max_sequence_length, args.hidden_size)
             ) # Add the mixin for GLM
     ```
 
-*  **Comprehensive supports for training**. `SwissArmyTransformer` aims to provide the best practice for pretraining and finetuning, where you only need to finish `forward_step` and `create_dataset_function` but with hyperparameters to alter useful training configurations.
+*  **Comprehensive supports for training**. `sat` aims to provide the best practice for pretraining and finetuning, where you only need to finish `forward_step` and `create_dataset_function` but with hyperparameters to alter useful training configurations.
     - Extend the training to multiple GPUs or nodes by specifying `--num_nodes`, `--num_gpus` and a simple `hostfile`. 
     - DeepSpeed and Model parallelism.
     - Better integration of ZeRO-2 and activation checkpointing.
     - Automatic extending and shuffling training data and `memmap`. 
     - Successfully support the training of [CogView2](http://github.com/THUDM/CogView2) and [CogVideo](https://github.com/THUDM/cogvideo).
     - The only open-source codebase supporting finetuning [T5-10B](https://arxiv.org/abs/1910.10683) on GPUs currently.
 
 </p></details>
 
 
 # Quick Tour
 
-The most typical python file to use `Bert` in SwissArmyTransformer (for inference) is as follows:
+The most typical python file to use `Bert` in sat (for inference) is as follows:
 ```python
 # @File: inference_bert.py
-from SwissArmyTransformer import get_args, get_tokenizer, AutoModel
+from sat import get_args, get_tokenizer, AutoModel
 # Parse args, initialize the environment. This is necessary.
 args = get_args() 
 # Automatically download and load model. Will also dump model-related hyperparameters to args.
-model, args = AutoModel.from_pretrained(args, 'bert-base-uncased') 
+model, args = AutoModel.from_pretrained('bert-base-uncased', args) 
 # Get the BertTokenizer according to args.tokenizer_type (automatically set).
 tokenizer = get_tokenizer(args) 
 # Here to use bert as you want!
 # ...
 ```
 Then we can run the code via
 ```bash
     SAT_HOME=/path/to/download python inference_bert.py --mode inference
 ```
-All officially supported model names are in [urls.py](SwissArmyTransformer/resources/urls.py).
+All officially supported model names are in [urls.py](sat/resources/urls.py).
 
 To finetune or pretrain a transformer is also extremely easy!
 ```python
 # @File: finetune_bert.py
-from SwissArmyTransformer import get_args, get_tokenizer, AutoModel
-from SwissArmyTransformer.model.mixins import MLPHeadMixin
+from sat import get_args, get_tokenizer, AutoModel
+from sat.model.mixins import MLPHeadMixin
 
 def create_dataset_function(path, args):
     # Here to load the dataset
     # ...
     assert isinstance(dataset, torch.utils.data.Dataset)
     return dataset
 
 def forward_step(data_iterator, model, args, timers):
     inputs = next(data_iterator) # from the dataset of create_dataset_function.
     loss, *others = model(inputs)
     return loss
     
 # Parse args, initialize the environment. This is necessary.
 args = get_args() 
-model, args = AutoModel.from_pretrained(args, 'bert-base-uncased') 
+model, args = AutoModel.from_pretrained('bert-base-uncased', args) 
 tokenizer = get_tokenizer(args) 
 # Here to use bert as you want!
 model.del_mixin('bert-final')
 model.add_mixin('classification_head', MLPHeadMixin(args.hidden_size, 2048, 1))
 # ONE LINE to train! 
 # args already includes hyperparams such as lr, train-iters, zero-stage ...
 training_main(args, 
@@ -138,34 +155,34 @@
     --train-data /path/to/train --valid-data /path/to/valid \
     --lr 0.00002 --batch-size 8 --zero-stage 1 --fp16
 ```
 Here we use data-parallel on GPUs 0,1. We can also launch the training on many inter-connected machines via `--hostfile /path/to/hostfile`. See the tutorial for more details.
 
 To write your own model, you only need to consider the difference between the standard Transformer. For example, if you have a idea to improve the attention operation:
 ```python
-from SwissArmyTransformer.model import BaseMixin
+from sat.model import BaseMixin
 class MyAttention(BaseMixin):
     def __init__(self, hidden_size):
         super(MyAttention, self).__init__()
         # MyAttention may needs some new params, e.g. a learnable alpha.
         self.learnable_alpha = torch.nn.Parameter(torch.ones(hidden_size))
     
     # This is a hook function, the name `attention_fn` is special.
     def attention_fn(q, k, v, mask, dropout=None, **kwargs):
         # Code for my attention.
         # ...
         return attention_results
 ```
-Here `attention_fn` is a hook function, replacing the default action by the new function. All available hooks are in [transformer_defaults.py](/SwissArmyTransformer/transformer_defaults.py). 
+Here `attention_fn` is a hook function, replacing the default action by the new function. All available hooks are in [transformer_defaults.py](/sat/transformer_defaults.py). 
 Now we can use `add_mixin` to apply our change to all the transformers, such as BERT, Vit and CogView. See the tutorial for more details. 
 
 ## Tutorials 
 TO BE RELEASED SOON...
 
 # Citation
 Currently we don't have a paper, so you don't need to formally cite us!~ 
 
-If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/SwissArmyTransformer}` to mention us and recommend `SwissArmyTransformer` to others.
+If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/sat}` to mention us and recommend `sat` to others.
 
-The tutorial for contributing SwissArmyTransformer is on the way!
+The tutorial for contributing sat is on the way!
 
 The project is based on (a user of) DeepSpeed, Megatron-LM and Huggingface transformers. Thanks for their awesome work.
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/arguments.py` & `SwissArmyTransformer-0.3.1/sat/arguments.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,49 +18,52 @@
 import argparse
 import os
 import torch
 import deepspeed
 import json
 import random
 import numpy as np
-from SwissArmyTransformer import mpu
+import warnings
+from sat import mpu
 
 
 def add_model_config_args(parser):
     """Model arguments"""
 
     group = parser.add_argument_group('model', 'model configuration')
 
     # --------------- Core hyper-parameters --------------- 
     group.add_argument('--num-layers', type=int, default=24,
-                       help='num decoder layers')
+                       help='num of layers')
     group.add_argument('--hidden-size', type=int, default=1024,
                        help='transformer hidden size')
     group.add_argument('--num-attention-heads', type=int, default=16,
                        help='num of transformer attention heads')
     group.add_argument('--vocab-size', type=int, default=0,
                        help='vocab size for tokenization. the size of word_embeddings.')
     group.add_argument('--max-sequence-length', type=int, default=512,
                        help='maximum number of position embeddings to use')
     
     # ---------------  Optional hyper-parameters --------------- 
 
     group.add_argument('--layernorm-order', type=str, default='pre',
+                       help='choose from "pre", "post", "sandwich".',
                        choices=['post', # In the original Transformer.
                                 'pre', # Used by most current frameworks.
                                 'sandwich' # More stable.
                                 ])
     # The inner-hidden-size in MLP, default "None" means 4*hidden-size
-    group.add_argument('--inner-hidden-size', type=int, default=None)
+    group.add_argument('--inner-hidden-size', type=int, default=None,
+                       help='inner hidden size for transformer FFN, None means 4*hidden-size')
     # The hidden-size-per-attention-head in Self and Cross Attention, 
     # default "None" means hidden-size/num-attention-heads.
     group.add_argument('--hidden-size-per-attention-head', type=int, default=None)
     # TODO: fully test it, support the generation.
     group.add_argument('--model-parallel-size', type=int, default=1,
-                       help='size of the model parallel.')
+                       help='size of the model parallel. only use if you are an expert.')
 
     group.add_argument('--skip-init', action='store_true',
                        help='skip model initialization')
     
     group.add_argument('--use-gpu-initialization', action='store_true', 
                        help='initialize model on gpu')
     
@@ -73,16 +76,16 @@
                        help='dropout probability for hidden state transformer')
     group.add_argument('--attention-dropout', type=float, default=0.1,
                        help='dropout probability for attention weights')
     group.add_argument('--make-vocab-size-divisible-by', type=int, default=128,
                        help='Pad the vocab size to be divisible by this value.'
                             'This is added for computational efficieny reasons.')
     # Deprecated. Please use `--layernorm-order sandwich`.
-    group.add_argument('--sandwich-ln', action='store_true',
-                        help='add sandwich ln in cogview.')
+    # group.add_argument('--sandwich-ln', action='store_true',
+    #                     help='add sandwich ln in cogview.')
     
     return parser
 
 
 
 def add_training_args(parser):
     """Training arguments."""
@@ -202,14 +205,15 @@
     # Training datasets.
     group.add_argument('--train-data', nargs='+', default=None,
                        help='Whitespace separated filenames or corpora names for training.'
                        'Use hf://path/to/dataset to load huggingface datasets.')
     group.add_argument('--train-data-weights', nargs='+', default=None, type=int,
                         help='scaling factors for different train-data, must the same number of'
                         '--train-data or None(==1).')
+    group.add_argument('--iterable-dataset', action='store_true', help='iterable')
 
     # Validation and Test dataset.
     group.add_argument('--valid-data', nargs='*', default=None,
                        help="""Filename for validation data.""")
     group.add_argument('--test-data', nargs='*', default=None,
                        help="""Filename for testing""")
     group.add_argument('--split', default='1000,1,1',
@@ -271,19 +275,39 @@
     while (after % multiple) != 0:
         after += 1
     if args.rank == 0:
         print('> padded vocab (size: {}) with {} dummy '
                  'tokens (new size: {})'.format(
         before, after - before, after))
 
+def _simple_init(model_parallel_size=1):
+    '''Necessary initialization for torch.distributed for model-only mode'''
+    args = argparse.Namespace(
+        distributed_backend='nccl',
+        model_parallel_size=model_parallel_size,
+    )
+    args.rank = int(os.getenv('RANK', '0'))
+    args.world_size = int(os.getenv("WORLD_SIZE", '1'))
+    args.local_rank = int(os.getenv("LOCAL_RANK", '0')) # torchrun
+    args.device = args.local_rank
+    args.deepspeed = False
+    if initialize_distributed(args): # first time init model parallel, print warning
+        warnings.warn(
+                  'You are using model-only mode.\n\
+                  For torch.distributed users or loading model parallel models, set environment variables RANK, WORLD_SIZE and LOCAL_RANK.'
+                  )
+        return True
+    return False
 
-def get_args(args_list=None):
+def get_args(args_list=None, parser=None):
     """Parse all the args."""
-
-    parser = argparse.ArgumentParser(description='SwissArmyTransformer')
+    if parser is None:
+        parser = argparse.ArgumentParser(description='sat')
+    else:
+        assert isinstance(parser, argparse.ArgumentParser)
     parser = add_model_config_args(parser)
     parser = add_training_args(parser)
     parser = add_evaluation_args(parser)
     parser = add_data_args(parser)
     parser = add_tokenization_args(parser)
     parser = add_text_generate_args(parser)
 
@@ -299,20 +323,28 @@
 
     args.cuda = torch.cuda.is_available()
 
     args.rank = int(os.getenv('RANK', '0'))
     args.world_size = int(os.getenv("WORLD_SIZE", '1'))
     if args.local_rank is None:
         args.local_rank = int(os.getenv("LOCAL_RANK", '0')) # torchrun
-    
+   
     if args.device == -1: # not set manually
         args.device = args.rank % torch.cuda.device_count()
         if args.local_rank is not None:
             args.device = args.local_rank
 
+    # local rank should be consistent with device in DeepSpeed
+    if args.local_rank != args.device and args.mode != 'inference':
+        raise ValueError(
+            'LOCAL_RANK (default 0) and args.device inconsistent. '
+            'This can only happens in inference mode. '
+            'Please use CUDA_VISIBLE_DEVICES=x for single-GPU training. '
+            )
+
     # args.model_parallel_size = min(args.model_parallel_size, args.world_size)
     if args.rank == 0:
         print('using world size: {} and model-parallel size: {} '.format(
             args.world_size, args.model_parallel_size))
     if args.vocab_size > 0:
         _adjust_vocab_size(args)
     
@@ -366,16 +398,17 @@
                 args.gradient_accumulation_steps = None
             if "optimizer" in deepspeed_config:
                 optimizer_params_config = deepspeed_config["optimizer"].get("params", {})
                 args.lr = optimizer_params_config.get("lr", args.lr)
                 args.weight_decay = optimizer_params_config.get("weight_decay", args.weight_decay)
         args.deepspeed_config = deepspeed_config
     
-    if args.sandwich_ln:
-        args.layernorm_order = 'sandwich'
+    # if args.sandwich_ln: # removed in v0.3
+    #     args.layernorm_order = 'sandwich'
+    
     # initialize distributed and random seed because it always seems to be necessary.
     initialize_distributed(args)
     set_random_seed(args.seed)
     return args
 
 
 def update_args_with_file(args, path):
@@ -396,15 +429,25 @@
     args = argparse.Namespace(**config, **args)
     return args
 
 
 def initialize_distributed(args):
     """Initialize torch.distributed."""
     if torch.distributed.is_initialized():
-        return 
+        if mpu.model_parallel_is_initialized():
+            if args.model_parallel_size != mpu.get_model_parallel_world_size():
+                raise ValueError('model_parallel_size is inconsistent with prior configuration.'
+                                 'We currently do not support changing model_parallel_size.')
+            return False
+        else:
+            if args.model_parallel_size > 1:
+                warnings.warn('model_parallel_size > 1 but torch.distributed is not initialized via SAT.'
+                            'Please carefully make sure the correctness on your own.')
+            mpu.initialize_model_parallel(args.model_parallel_size)
+        return True
     # the automatic assignment of devices has been moved to arguments.py 
     torch.cuda.set_device(args.device)
     # Call the init process
     init_method = 'tcp://'
     args.master_ip = os.getenv('MASTER_ADDR', 'localhost')
     args.master_port = os.getenv('MASTER_PORT', '6000')
     init_method += args.master_ip + ':' + args.master_port
@@ -414,24 +457,29 @@
         init_method=init_method)
 
     # Set the model-parallel / data-parallel communicators.
     mpu.initialize_model_parallel(args.model_parallel_size)
 
     # Optional DeepSpeed Activation Checkpointing Features
     if args.deepspeed: 
+        deepspeed.init_distributed(
+            dist_backend=args.distributed_backend,
+            world_size=args.world_size, rank=args.rank, init_method=init_method)
         # It seems that it has no negative influence to configure it even without using checkpointing.  
         deepspeed.checkpointing.configure(mpu, deepspeed_config=args.deepspeed_config, num_checkpoints=args.num_layers)
+    return True
 
 def set_random_seed(seed):
     """Set random seed for reproducability."""
-    if seed is not None and seed > 0:
+    if seed is not None:
+        assert seed > 0
         random.seed(seed)
         np.random.seed(seed)
         torch.manual_seed(seed)
         torch.cuda.manual_seed(seed)
         torch.cuda.manual_seed_all(seed)  # if you are using multi-GPU.
-        torch.backends.cudnn.benchmark = False
+        torch.backends.cudnn.benchmark = True
         torch.backends.cudnn.deterministic = True
-        torch.backends.cudnn.enabled = False
+        torch.backends.cudnn.enabled = True # False
         torch.backends.cuda.matmul.allow_tf32 = False # if set it to True will be much faster but not accurate
         if deepspeed.checkpointing.is_configured():
             mpu.model_parallel_cuda_manual_seed(seed)
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/data_utils/configure_data.py` & `SwissArmyTransformer-0.3.1/sat/data_utils/configure_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,24 +16,41 @@
 import numpy as np
 import torch
 from bisect import bisect_right
 from functools import partial
 
 from torch.utils import data
 from .samplers import DistributedBatchSampler
+from torch.utils.data import ChainDataset, IterableDataset
 
-from SwissArmyTransformer import mpu
+from sat import mpu
+    
+
+def make_data_loader(dataset, batch_size, args, split, collate_fn=None):
 
-# class ExDataLoader(torch.utils.data.DataLoader)
-def make_data_loader(dataset, batch_size, args, split):
     world_size = torch.distributed.get_world_size(
         group=mpu.get_data_parallel_group())
     rank = torch.distributed.get_rank(group=mpu.get_data_parallel_group())
     distributed = world_size > 1
 
+    # if IterableDataset, assume everything is properly configured. (pre-sharded) 
+    if isinstance(dataset, IterableDataset):
+        if split in ['val', 'test'] and args.strict_eval:
+            raise ValueError('IterableDataset cannot be used for validation or testing if `args.strict_eval=True`, because we cannot infer the length of the final batch before reading out them.')
+        args.val_last_shape = [1] * world_size # just fake it, not actually used
+        args.val_drop_number = 0
+        args.test_last_shape = [1] * world_size
+        args.test_drop_number = 0
+        return torch.utils.data.DataLoader(
+            dataset,
+            batch_size=batch_size//world_size,
+            num_workers=args.num_workers,
+            pin_memory=True
+            )
+
     sampler = torch.utils.data.SequentialSampler(dataset)
     # drop_last = distributed
     drop_last = False # TODO will always drop last to keep the consistency.
     # or, how to avg in eval last batch?
 
     # the GPUs in the same model parallel group receive the same data
     if distributed: # TODO reformat this, but it is not urgent
@@ -47,53 +64,71 @@
                                                 gradient_accumulation_steps=gradient_accumulation_steps)
     else:
         batch_sampler = torch.utils.data.BatchSampler(sampler,
                                                       batch_size,
                                                       drop_last)
     last_len = len(dataset) % batch_size
     batch_per_worker = batch_size // world_size
-    last_shape = [batch_per_worker] * (last_len//batch_per_worker)
-    if last_len != 0 :
+    last_shape = [batch_per_worker] * (last_len//batch_per_worker) # some processes get full batch
+    if last_len != 0:
         if last_len % batch_per_worker != 0:
-            last_shape.append(last_len % batch_per_worker)
+            last_shape.append(last_len % batch_per_worker) # one process get the rest (<1 batch)
         drop_number = world_size - ((last_len-1)//batch_per_worker + 1)
-        for j in range(drop_number):
+        # other processes get nothing, but append 1 for running. will drop later according to drop_number.
+        for j in range(drop_number): 
             last_shape.append(1)
     else:
         drop_number = 0
     if split=='val':
         args.val_last_shape = last_shape
         args.val_drop_number = drop_number
     elif split=='test':
         args.test_last_shape = last_shape
         args.test_drop_number = drop_number
     data_loader = torch.utils.data.DataLoader(dataset,
                                               batch_sampler=batch_sampler,
                                               num_workers=args.num_workers,
-                                              pin_memory=True)
+                                              pin_memory=True,
+                                              collate_fn=collate_fn)
     return data_loader
 
 
 def make_dataset_full(path, split, args, create_dataset_function, 
         dataset_weights=None, random_mapping=True, is_train_data=False, **kwargs):
     """function to create datasets+tokenizers for common options"""
     print('make dataset ...', path)
-    if split is None:
-        split = [1.]
-
     assert isinstance(path, list)
-    
+
+    if args.iterable_dataset: # cannot indexed
+        # the random mapping is flexible and efficient, but sometimes we have pratical issue
+        # For instance, someone just gives you a iterable dataset, e.g. webdataset
+        from .datasets import ConfiguredResampledShards, DataPipeline
+        valid_types = (ConfiguredResampledShards, DataPipeline)
+        
+        assert split[0] == 1, 'Iterable dataset cannot auto split.'
+        assert dataset_weights is None
+        for p in path:
+            ds = []
+            for p in path:
+                d = create_dataset_function(p, args)
+                assert isinstance(d, valid_types)
+                ds.append(d)
+            ds = ChainDataset(ds)
+        return ds
+
+    if split is None:
+        split = [1.] 
     if not should_split(split):
         ds = []
         for p in path:
             d = create_dataset_function(p, args)
             ds.append(d)
         ds = ConcatDataset(ds, weights=dataset_weights)
         if random_mapping:
-            if args.epochs is not None:
+            if args.epochs is not None: # not auto-scale, but use a given number of epoches.
                 ds = RandomDataset(ds, scale=args.epochs, seed=args.seed)
             else:
                 world_size = torch.distributed.get_world_size(
                     group=mpu.get_data_parallel_group())
                 if is_train_data:
                 # only train-dataset will set this to True,
                 # so we enlarge it to make sure that the data is sufficient.
@@ -121,15 +156,15 @@
                 group=mpu.get_data_parallel_group())
             scale = max(200, 1 + (args.train_iters * args.batch_size * world_size) // len(train_ds))
             train_ds = RandomMappingDataset(train_ds, scale=scale)
             valid_ds = RandomMappingDataset(valid_ds) # TODO precise scale 
             test_ds = RandomMappingDataset(test_ds)
         return train_ds, valid_ds, test_ds
 
-def make_loaders(args, create_dataset_function):
+def make_loaders(args, create_dataset_function, collate_fn=None):
     """makes training/val/test
     Args:
         args.train_data, args.valid_data, args.test_data: str. Paths to the dataset.
         args.split: str. format: "8,1,1". how to split train_data.
         args.dataset_type: use to create the right datasets. 
     """
     make_dataset = partial(make_dataset_full, 
@@ -168,26 +203,26 @@
         valid = make_dataset(**eval_set_args, args=args, random_mapping=not args.strict_eval)
     if test is None and args.test_data is not None:
         eval_set_args['path'] = args.test_data
         test = make_dataset(**eval_set_args, args=args, random_mapping=not args.strict_eval)
 
     # wrap datasets with data loader
     if train is not None and args.batch_size > 0:
-        train = make_data_loader(train, batch_size, args, split='train')
+        train = make_data_loader(train, batch_size, args, split='train', collate_fn=collate_fn)
         args.do_train = True
     else:
         args.do_train = False
     eval_batch_size = eval_batch_size if eval_batch_size != 0 else batch_size
     if valid is not None:
-        valid = make_data_loader(valid, eval_batch_size, args, split='val')
+        valid = make_data_loader(valid, eval_batch_size, args, split='val', collate_fn=collate_fn)
         args.do_valid = True
     else:
         args.do_valid = False
     if test is not None:
-        test = make_data_loader(test, eval_batch_size, args, split='test')
+        test = make_data_loader(test, eval_batch_size, args, split='test', collate_fn=collate_fn)
         args.do_test = True
     else:
         args.do_test = False
 
     return train, valid, test
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/data_utils/hf_dataset.py` & `SwissArmyTransformer-0.3.1/sat/data_utils/hf_dataset.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/data_utils/samplers.py` & `SwissArmyTransformer-0.3.1/sat/data_utils/samplers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/autoregressive_sampling.py` & `SwissArmyTransformer-0.3.1/sat/generation/autoregressive_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,16 @@
     # building the initial tokens, attention_mask, and position_ids
     context_length = 0
     while seq[context_length] >= 0:
         context_length += 1 # [0, context_length-1] are given
     assert context_length > 0
     tokens, attention_mask, position_ids = get_masks_and_position_ids(seq)
     tokens = tokens[..., :context_length]
-    attention_mask = attention_mask.type_as(next(model.parameters())) # if fp16
+    if attention_mask.dtype != torch.bool:
+        attention_mask = attention_mask.type_as(next(model.parameters())) # if fp16
     # initialize generation
     counter = context_length - 1 # Last fixed index is ``counter'' 
     index = 0 if mems is None else mems.shape[2] # Next forward starting index, also the length of cache.
     # step-by-step generation
     while counter < len(seq) - 1:
         # Now, we want to generate seq[counter + 1],
         # token[:, index: counter+1] needs forwarding.
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/cuda2d_sampling.py` & `SwissArmyTransformer-0.3.1/sat/generation/cuda2d_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/magnify.py` & `SwissArmyTransformer-0.3.1/sat/generation/magnify.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/sampling_strategies/base_strategy.py` & `SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/base_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/sampling_strategies/beam_search_strategy.py` & `SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/beam_search_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/sampling_strategies/iterative_entfilter_strategy.py` & `SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/iterative_entfilter_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/generation/utils.py` & `SwissArmyTransformer-0.3.1/sat/generation/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import random
 import torch
 import time
 import stat
 from datetime import datetime
 from torchvision.utils import save_image
 import torch.distributed as dist
-from SwissArmyTransformer.mpu import get_data_parallel_world_size, get_data_parallel_rank
+from sat.mpu import get_data_parallel_world_size, get_data_parallel_rank, get_model_parallel_rank
 
 
 def timed_name(prefix, suffix=None, path=None):
     return os.path.join(
         path, 
         f"{prefix}-{datetime.now().strftime('%m-%d-%H-%M-%S')}{suffix}"
     )
@@ -39,42 +39,47 @@
             os.chmod(os.path.join(path,f'{i}.jpg'), stat.S_IRWXO+stat.S_IRWXG+stat.S_IRWXU)
         save_image(torch.cat(imgs, dim=0), os.path.join(path,f'concat.jpg'), normalize=True)
         os.chmod(os.path.join(path,f'concat.jpg'), stat.S_IRWXO+stat.S_IRWXG+stat.S_IRWXU)
 
 def generate_continually(func, input_source='interactive'):
     if input_source == 'interactive':
         while True:
-            raw_text = input("\nPlease Input Query (stop to exit) >>> ") 
-            raw_text = raw_text.strip()
-            if not raw_text:
-                print('Query should not be empty!')
-                continue
-            if raw_text == "stop":
-                return 
+            raw_text, is_stop = "", False
+            if torch.distributed.get_rank() == 0:
+                raw_text = input("\nPlease Input Query (stop to exit) >>> ")
+                raw_text = raw_text.strip()
+                if not raw_text:
+                    print('Query should not be empty!')
+                    continue
+                if raw_text == "stop":
+                    is_stop = True
+                torch.distributed.broadcast_object_list([raw_text, is_stop])
+            else:
+                info = [raw_text, is_stop]
+                torch.distributed.broadcast_object_list(info)
+                raw_text, is_stop = info
+            if is_stop:
+                return
             try:
                 start_time = time.time()
                 func(raw_text)
-                print("\nTaken time {:.2f}\n".format(time.time() - start_time), flush=True)
+                if torch.distributed.get_rank() == 0:
+                    print("\nTaken time {:.2f}\n".format(time.time() - start_time), flush=True)
             except (ValueError, FileNotFoundError) as e:
                 print(e)
                 continue
     else:
         with open(input_source, 'r') as fin:
             inputs = fin.readlines()
-        err_linenos = []
         for line_no, raw_text in enumerate(inputs):
             if line_no % get_data_parallel_world_size() != get_data_parallel_rank():
                 continue
             rk = dist.get_rank()
-            print(f'Working on No. {line_no} on {rk}... ')
+            if get_model_parallel_rank() == 0:
+                print(f'Working on No. {line_no} on model group {rk}... ')
             raw_text = raw_text.strip()
             if len(raw_text) == 0:
                 continue
-            # try:
             start_time = time.time()
             func(raw_text)
-            print("\nTaken time {:.2f}\n".format(time.time() - start_time), flush=True)
-            # except (ValueError, FileNotFoundError) as e:
-            #     err_linenos.append(line_no)
-            #     print(e)
-            #     continue
-        print(err_linenos)
+            if get_model_parallel_rank() == 0:
+                print("\nTaken time {:.2f}\n".format(time.time() - start_time), flush=True)
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/cached_autoregressive_model.py` & `SwissArmyTransformer-0.3.1/sat/model/cached_autoregressive_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 import sys
 import math
 import random
 import torch
 
 from .base_model import BaseModel, BaseMixin, non_conflict
-from SwissArmyTransformer.model.transformer import standard_attention, split_tensor_along_last_dim
+from sat.model.transformer import standard_attention, split_tensor_along_last_dim
 
 class CachedAutoregressiveMixin(BaseMixin):
     def __init__(self):
         super().__init__()     
            
     @non_conflict
     def attention_fn(self, q, k, v, mask, dropout_fn, mems=None, cross_attention=False, old_impl=standard_attention,
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/encoder_decoder_model.py` & `SwissArmyTransformer-0.3.1/sat/model/encoder_decoder_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 import os
 import sys
 import math
 import random
 import torch
 import argparse
 from .base_model import BaseModel, BaseMixin
-from SwissArmyTransformer.mpu.mappings import copy_to_model_parallel_region
-from SwissArmyTransformer import update_args_with_file
-from SwissArmyTransformer.training.deepspeed_training import load_checkpoint, get_model
-from SwissArmyTransformer.resources import auto_create
+from sat.mpu.mappings import copy_to_model_parallel_region
+from sat import update_args_with_file
+from sat.training.deepspeed_training import load_checkpoint, get_model
+from sat.resources import auto_create
 
 class EncoderFinalMixin(BaseMixin):
     def final_forward(self, logits, **kwargs):
         logits = copy_to_model_parallel_region(logits)
         return logits
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/finetune/adapter.py` & `SwissArmyTransformer-0.3.1/sat/model/finetune/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- encoding: utf-8 -*-
 # @File    :   adapter.py
 # @Time    :   2022/6/16
 # @Author  :   Zhuoyi Yang
 # @Contact :   yangzhuo18@mails.tsinghua.edu.cn
-from SwissArmyTransformer.model.base_model import BaseModel, BaseMixin, non_conflict
+from sat.model.base_model import BaseModel, BaseMixin, non_conflict
 import torch.nn as nn
 class AdapterMixin(BaseMixin):
     def __init__(self, num_layers, hidden_size, adapter_hidden):
         super().__init__()
         self.ff1 = nn.ModuleList([
             nn.Linear(hidden_size, adapter_hidden) for _ in range(num_layers)
         ])
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/finetune/ffadd.py` & `SwissArmyTransformer-0.3.1/sat/model/finetune/ffadd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- encoding: utf-8 -*-
 # @File    :   ffadd.py
 # @Time    :   2022/6/16
 # @Author  :   Zhuoyi Yang
 # @Contact :   yangzhuo18@mails.tsinghua.edu.cn
-from SwissArmyTransformer.model.base_model import BaseMixin, non_conflict
+from sat.model.base_model import BaseMixin, non_conflict
 import torch
 class FFADDMixin(BaseMixin):
     def __init__(
             self,
             hidden_size: int,
             layer_num: int = 24,
             r: int = 0,
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/finetune/lora.py` & `SwissArmyTransformer-0.3.1/sat/model/finetune/lora.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 # here put the import lib
 import os
 import sys
 import math
 import random
 import torch
 import torch.nn as nn
-from SwissArmyTransformer.model.transformer import standard_attention
-from SwissArmyTransformer.model.base_model import BaseModel, BaseMixin, non_conflict
-from SwissArmyTransformer.mpu.utils import split_tensor_along_last_dim
+from sat.model.transformer import standard_attention
+from sat.model.base_model import BaseModel, BaseMixin, non_conflict
+from sat.mpu.utils import split_tensor_along_last_dim
 import torch.nn.functional as F
 
 class LoRAMixin(BaseMixin):
     def __init__(
             self,
             hidden_size: int,
             layer_num: int = 24,
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/finetune/mlp_head.py` & `SwissArmyTransformer-0.3.1/sat/model/finetune/mlp_head.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # here put the import lib
 import os
 import sys
 import math
 import random
 
 import torch
-from SwissArmyTransformer.model.base_model import BaseModel, BaseMixin, non_conflict
+from sat.model.base_model import BaseModel, BaseMixin, non_conflict
 
 class MLPHeadMixin(BaseMixin):
     def __init__(self, hidden_size, *output_sizes, bias=True, activation_func=torch.nn.functional.relu, init_mean=0, init_std=0.005):
         super().__init__()
         self.activation_func = activation_func
         last_size = hidden_size
         self.layers = torch.nn.ModuleList()
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/finetune/prompt_tuning.py` & `SwissArmyTransformer-0.3.1/sat/model/finetune/prompt_tuning.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # here put the import lib
 import os
 import sys
 import math
 import random
 import torch
 
-from SwissArmyTransformer.model.transformer import standard_attention
-from SwissArmyTransformer.model.base_model import BaseModel, BaseMixin, non_conflict
+from sat.model.transformer import standard_attention
+from sat.model.base_model import BaseModel, BaseMixin, non_conflict
 
 
 class PrefixTuningMixin(BaseMixin):
     def __init__(self, num_layers, hidden_size_per_attention_head, num_attention_heads, prefix_len):
         super().__init__()
         self.prefix = torch.nn.ParameterList([
             torch.nn.Parameter(torch.randn(2, num_attention_heads, prefix_len, hidden_size_per_attention_head)*0.01)
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/bert_model.py` & `SwissArmyTransformer-0.3.1/sat/model/official/bert_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
-from SwissArmyTransformer.model.transformer import LayerNorm
-from SwissArmyTransformer.model.base_model import BaseMixin, BaseModel
+from sat.model.transformer import LayerNorm
+from sat.model.base_model import BaseMixin, BaseModel
 
 gelu = nn.functional.gelu
 
 class lm_head(torch.nn.Module):
     def __init__(self, vocab_size, hidden_size, layernorm_epsilon=1.0e-5):
         super().__init__()
         self.dense = nn.Linear(hidden_size, hidden_size)
@@ -42,8 +42,8 @@
         self.add_mixin("bert-type", BertTypeMixin(args.num_types, args.hidden_size))
         
 
     @classmethod
     def add_model_specific_args(cls, parser):
         group = parser.add_argument_group('BERT', 'BERT Configurations')
         group.add_argument('--num-types', type=int)
-        return parser
+        return super().add_model_specific_args(parser)
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/cait_model.py` & `SwissArmyTransformer-0.3.1/sat/model/official/cait_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from SwissArmyTransformer.model.base_model import BaseMixin, BaseModel, non_conflict
-from SwissArmyTransformer.model.official.vit_model import ViTModel, ClsMixin
-from SwissArmyTransformer.model.mixins import BaseMixin
-from SwissArmyTransformer import mpu
+from sat.model.base_model import BaseMixin, BaseModel, non_conflict
+from sat.model.official.vit_model import ViTModel, ClsMixin
+from sat.model.mixins import BaseMixin
+from sat import mpu
 
 class AttnMixin(BaseMixin):
     def __init__(self, num_heads, num_layers):
         super().__init__()
         self.num_layers = num_layers
         self.proj_l = nn.ModuleList([nn.Linear(num_heads, num_heads) for i in range(num_layers)])
         self.proj_w = nn.ModuleList([nn.Linear(num_heads, num_heads) for i in range(num_layers)])
 
     def attention_fn(self, query_layer, key_layer, value_layer, attention_mask,
                        attention_dropout=None, log_attention_weights=None, scaling_attention_score=True, **kwargs):
-        # adapted from https://github.com/THUDM/SwissArmyTransformer/blob/main/SwissArmyTransformer/mpu/transformer.py#L47
+        # adapted from https://github.com/THUDM/sat/blob/main/sat/mpu/transformer.py#L47
         if scaling_attention_score:
             query_layer = query_layer * (query_layer.shape[-1]**-0.5) # / math.sqrt(query_layer.shape[-1])
         attention_scores = torch.matmul(query_layer, key_layer.transpose(-1, -2))
         if log_attention_weights is not None:
             attention_scores += log_attention_weights
         
         attention_scores = self.proj_l[kwargs['layer_id']](attention_scores.permute(0, 2, 3, 1)).permute(0, 3, 1, 2)
@@ -72,16 +72,16 @@
         mlp_output = layer.mlp(layernorm_output, **kw_args)
 
         # Second residual connection.
         output = layernorm_input + self.gamma_2[kw_args['layer_id']] * mlp_output
 
         return output
 
-from SwissArmyTransformer.model.transformer import standard_attention
-from SwissArmyTransformer.mpu.utils import split_tensor_along_last_dim
+from sat.model.transformer import standard_attention
+from sat.mpu.utils import split_tensor_along_last_dim
 
 class DecForward(BaseMixin):
     def __init__(self, dim, num_layers, init_values=1e-4):
         super().__init__()
         self.gamma_1 = nn.ParameterList([nn.Parameter(init_values * torch.ones((dim)), requires_grad=True) for i in range(num_layers)])
         self.gamma_2 = nn.ParameterList([nn.Parameter(init_values * torch.ones((dim)), requires_grad=True) for i in range(num_layers)])
     
@@ -112,15 +112,15 @@
 
         # Second residual connection.
         output = layernorm_input + self.gamma_2[kw_args['layer_id']] * mlp_output
 
         return output
 
     def cross_attention_forward(self, hidden_states, cross_attention_mask, encoder_outputs, **kw_args):
-        # adapted from https://github.com/THUDM/SwissArmyTransformer/blob/d8c9d1e0a9bb2af1e1d26a68b35f16d84aafcc2f/SwissArmyTransformer/mpu/transformer.py#L216
+        # adapted from https://github.com/THUDM/sat/blob/d8c9d1e0a9bb2af1e1d26a68b35f16d84aafcc2f/sat/mpu/transformer.py#L216
         # if you want to use a customized attention_fn, just inherit the attention mixin for this mixin and use self.attention_fn instead of self.hooks['attention_fn']
         layer = self.transformer.layers[kw_args['layer_id']].cross_attention
         
         attention_fn = standard_attention
         
         mixed_query_layer = layer.query(hidden_states[:, :1])
         mixed_x_layer = layer.key_value(hidden_states)
@@ -164,23 +164,23 @@
         super().__init__(args, is_decoder=True, transformer=transformer, parallel_output=parallel_output, layernorm_epsilon=layernorm_epsilon)
         self.add_mixin('cls', ClsMixin(args.hidden_size, args.num_classes))
         self.add_mixin('dec_forward', DecForward(args.hidden_size, args.num_layers, init_values=args.init_scale))
     @classmethod
     def add_model_specific_args(cls, parser):
         return super().add_model_specific_args(parser)
 
-from SwissArmyTransformer.model import EncoderDecoderModel
+from sat.model import EncoderDecoderModel
 import argparse
 
 class CaiT(EncoderDecoderModel):
     def __init__(self, args, transformer=None, parallel_output=True, layernorm_epsilon=1e-6):
         encoder = CaiTEncoder(args, transformer=transformer, parallel_output=parallel_output, layernorm_epsilon=layernorm_epsilon)
         dec_args = argparse.Namespace(**vars(args))
         # dec_args.enc_hidden_size = dec_args.hidden_size  # used for cross attn
-        override_attrs = ['num_layers', 'hidden_size', 'num_attention_heads', 'layernorm_order'
+        override_attrs = ['num_layers', 'hidden_size', 'num_attention_heads', 'layernorm_order',
                             'max_sequence_length', 'inner_hidden_size', 'hidden_size_per_attention_head']
         for name in override_attrs:
             dec_attr = getattr(dec_args, 'dec_' + name, None)
             if dec_attr is not None:  # else use encoder-config
                 setattr(dec_args, name, dec_attr)
         decoder = CaiTDecoder(dec_args, transformer=transformer, parallel_output=parallel_output, layernorm_epsilon=layernorm_epsilon)
         super().__init__(args, encoder=encoder, decoder=decoder)
@@ -189,8 +189,8 @@
         # Please use self.decoder for auto-regressive generation.
         if enc_attention_mask is None:
             enc_attention_mask = torch.ones(1, 1, dtype=self.encoder.transformer.word_embeddings.weight.dtype, device=input_ids.device)
         if cross_attention_mask is None:
             cross_attention_mask = enc_attention_mask
         encoder_outputs = self.encode(input_ids, enc_position_ids, enc_attention_mask, **kw_args)
         decoder_outputs, *mems = self.decode(input_ids, dec_position_ids, dec_attention_mask, encoder_outputs=encoder_outputs, cross_attention_mask=cross_attention_mask, **kw_args)
-        return (encoder_outputs, decoder_outputs, *mems)
+        return (encoder_outputs, decoder_outputs, *mems)
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/clip_model.py` & `SwissArmyTransformer-0.3.1/sat/model/official/clip_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import math
 from re import L
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from SwissArmyTransformer.model.base_model import BaseMixin, BaseModel, non_conflict
-from SwissArmyTransformer.model.official.vit_model import ViTModel, ImagePatchEmbeddingMixin
-from SwissArmyTransformer.model.mixins import BaseMixin
-from SwissArmyTransformer import mpu
-from SwissArmyTransformer.model.transformer import LayerNorm
-from SwissArmyTransformer import update_args_with_file
-from SwissArmyTransformer.training.deepspeed_training import load_checkpoint, get_model
-from SwissArmyTransformer.resources import auto_create
+from sat.model.base_model import BaseMixin, BaseModel, non_conflict
+from sat.model.official.vit_model import ViTModel, ImagePatchEmbeddingMixin
+from sat.model.mixins import BaseMixin
+from sat import mpu
+from sat.model.transformer import LayerNorm
+from sat import update_args_with_file
+from sat.training.deepspeed_training import load_checkpoint, get_model
+from sat.resources import auto_create
 
 """
 CLIP model follows Siamese architecture.
 For image encoder, it is a ViTModel with 32x32 patch.
 For text encoder, it is a BaseModel with causal mask.
 """
 
@@ -84,26 +84,26 @@
         return output
 
 class TextEncoder(BaseModel):
     def __init__(self, args, layernorm_epsilon=1e-5, activation_func=QuickGELUActivation()):
         super().__init__(args, layernorm_epsilon=layernorm_epsilon, activation_func=activation_func)
         self.add_mixin('text_enc', TextMixin(args.hidden_size, args.projection_dim))
 
-    @classmethod
-    def add_model_specific_args(cls, parser):
-        return super().add_model_specific_args(parser)
+    # @classmethod
+    # def add_model_specific_args(cls, parser):
+    #     return super().add_model_specific_args(parser)
 
 import argparse
 
 class CLIP(nn.Module):
     def __init__(self, args, layernorm_epsilon=1e-5):
         super().__init__()
         self.image_encoder = ImageEncoder(args, layernorm_epsilon=layernorm_epsilon)
         text_args = argparse.Namespace(**vars(args))
-        override_attrs = ['vocab_size', 'num_layers', 'hidden_size', 'num_attention_heads', 'layernorm_order'
+        override_attrs = ['vocab_size', 'num_layers', 'hidden_size', 'num_attention_heads', 'layernorm_order',
                             'max_sequence_length', 'inner_hidden_size', 'hidden_size_per_attention_head']
         for name in override_attrs:
             text_attr = getattr(text_args, 'text_' + name, None)
             if text_attr is not None:  # else use encoder-config
                 setattr(text_args, name, text_attr)
         self.text_encoder = TextEncoder(text_args, layernorm_epsilon=layernorm_epsilon)
         self.logit_scale = nn.Parameter(torch.ones([]) * args.logit_scale_init_value)
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/cuda2d_model.py` & `SwissArmyTransformer-0.3.1/sat/model/official/cuda2d_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 import sys
 import math
 import random
 import torch
 import torch.nn.functional as F
 
 
-from SwissArmyTransformer.model.base_model import BaseModel, BaseMixin
+from sat.model.base_model import BaseModel, BaseMixin
 
-from SwissArmyTransformer.model.transformer import split_tensor_along_last_dim
-from SwissArmyTransformer.mpu.utils import sqrt
+from sat.model.transformer import split_tensor_along_last_dim
+from sat.mpu.utils import sqrt
 from deepspeed.runtime.activation_checkpointing.checkpointing import get_cuda_rng_tracker
-from SwissArmyTransformer.mpu import ColumnParallelLinear, RowParallelLinear
-from SwissArmyTransformer.model.transformer import unscaled_init_method
+from sat.mpu import ColumnParallelLinear, RowParallelLinear
+from sat.model.transformer import unscaled_init_method
 
 class PositionEmbeddingMixin(BaseMixin):
     def __init__(self, additional_sequence_length, hidden_size,
                  init_method_std=0.02, reinit_slice=slice(-1024, None)
                  ):
         super(PositionEmbeddingMixin, self).__init__()
         self.reinit_slice = reinit_slice
@@ -152,15 +152,15 @@
 def sparse_attention_2d_light(q0, k0, v0, q1, k1, v1, attention_mask, n_head, text_len, kernel_size=9, kernel_size2=7, attention_dropout=None, log_attention_weights = None, **kwargs):
     '''
     q0, k0, v0: [batch_size, 1088, hidden_size]
     q1, k1, v1: [batch_size, 4096, h2]
     n_head: int
     attention_mask: [batch_size, 1088, 1088]
     '''
-    from SwissArmyTransformer.ops.local_attention_function import f_similar, f_weighting
+    from sat.ops.local_attention_function import f_similar, f_weighting
 
     b, s0, h0 = q0.shape
     b, s1, h1 = q1.shape
     h, l0, l1 = h0 // n_head, sqrt(s0-text_len), sqrt(s1)
 
     q0 = q0.reshape(b, s0, n_head, h).permute(0, 2, 1, 3)
     v0 = v0.reshape(b, s0, n_head, h).permute(0, 2, 1, 3)
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/distill_model.py` & `SwissArmyTransformer-0.3.1/sat/model/official/distill_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,8 +15,20 @@
         for n, p in self.teacher.named_parameters():
             p.requires_grad_(False)
 
     @classmethod
     def add_model_specific_args(cls, parser):
         group = parser.add_argument_group('BERT-distill', 'BERT distill Configurations')
         group.add_argument('--teacher', type=str)
-        return parser
+        group.add_argument('--tc-type', type=str)
+        group.add_argument('--st-type', type=str)
+        return parser
+    
+    @classmethod
+    def from_pretrained(cls, args, teacher_cls, student_name, student_cls):
+        student, args = student_cls.from_pretrained(student_name, args, prefix='student.')
+        if isinstance(teacher_cls, type):
+            teacher, t_args = teacher_cls.from_pretrained(args.teacher, args)
+        else:
+            teacher = teacher_cls
+        model = DistillModel(teacher, student)
+        return model, args
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/glm130B_model.py` & `SwissArmyTransformer-0.3.1/sat/model/official/glm130B_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,351 +1,371 @@
 import math
 import torch
-import torch.nn as nn
 from torch.nn import functional as F
 
-from SwissArmyTransformer.model.base_model import BaseModel, BaseMixin
-
-from SwissArmyTransformer.mpu.layers import ColumnParallelLinear
-
-from SwissArmyTransformer.model.position_embedding import RotaryEmbedding
-from SwissArmyTransformer.model.position_embedding import \
-apply_rotary_pos_emb_torch, apply_rotary_pos_emb, apply_rotary_pos_emb_fused, \
-    apply_rotary_pos_emb_index_torch, apply_rotary_pos_emb_index, apply_rotary_pos_emb_index_fused
-
-from SwissArmyTransformer.transformer_defaults import standard_attention
-from SwissArmyTransformer.mpu.utils import split_tensor_along_last_dim, divide
+from sat import mpu
+from sat.transformer_defaults import standard_attention
+from sat.mpu.utils import split_tensor_along_last_dim, divide
+from sat.mpu.layers import ColumnParallelLinear
+from sat.model.base_model import BaseModel, BaseMixin
+from sat.model.position_embedding import RotaryEmbedding
+from sat.model.position_embedding import apply_rotary_pos_emb_index
 
 # flags required to enable jit fusion kernels
 torch._C._jit_set_profiling_mode(False)
 torch._C._jit_set_profiling_executor(False)
 torch._C._jit_override_can_fuse_on_cpu(True)
 torch._C._jit_override_can_fuse_on_gpu(True)
 
+try:
+    from apex.transformer.functional import FusedScaleMaskSoftmax
+    from apex.transformer.enums import AttnMaskType
+except ModuleNotFoundError:
+    print(
+        "Please install apex to use FusedScaleMaskSoftmax, otherwise the inference efficiency will be greatly reduced"
+    )
+    FusedScaleMaskSoftmax = None
 
 
 class RotaryEmbeddingMixin(BaseMixin):
-    def __init__(self, fp16, apply_rotary_positional_embedding_kernel, bf16, hidden_size, num_attention_heads, model_parallel_size, learnable_rotary_embedding=False):
+    def __init__(
+        self,
+        fp16: bool,
+        hidden_size: int,
+        num_attention_heads: int,
+        model_parallel_size: int,
+        position_encoding_2d: bool
+    ):
         super().__init__()
         hidden_size_per_attention_head = divide(hidden_size, num_attention_heads)
         self.hidden_size_per_attention_head = hidden_size_per_attention_head
         self.num_attention_heads_per_partition = divide(num_attention_heads, model_parallel_size)
+        self.position_encoding_2d = position_encoding_2d
         self.rotary_emb = RotaryEmbedding(
-            hidden_size_per_attention_head,
+            hidden_size_per_attention_head // 2
+            if position_encoding_2d
+            else hidden_size_per_attention_head,
             base=10000,
             precision=torch.half if fp16 else torch.float,
             learnable=False,
-            device=torch.cuda.current_device())
-
-        self.apply_rotary_fn = (
-                apply_rotary_pos_emb_index_fused
-                if apply_rotary_positional_embedding_kernel
-                else apply_rotary_pos_emb_index_torch
-                if bf16
-                else apply_rotary_pos_emb_index
-            )
+            device=torch.cuda.current_device(),
+        )
 
-           
     def attention_forward(self, hidden_states, mask, **kw_args):
-        attn = self.transformer.layers[kw_args['layer_id']].attention
+        attn = self.transformer.layers[kw_args["layer_id"]].attention
         attention_fn = standard_attention
-        if 'attention_fn' in attn.hooks:
-            attention_fn = attn.hooks['attention_fn']
+        if "attention_fn" in attn.hooks:
+            attention_fn = attn.hooks["attention_fn"]
 
         # [seq, b, 3 * hn * np]
         mixed_raw_layer = attn.query_key_value(hidden_states)
 
         # [seq, b, (np * 3 * hn)] --> [seq, b, np, 3 * hn]
-        new_tensor_shape = mixed_raw_layer.size()[:-1] + \
-            (self.num_attention_heads_per_partition,
-                3 * self.hidden_size_per_attention_head)
+        new_tensor_shape = mixed_raw_layer.size()[:-1] + (
+            self.num_attention_heads_per_partition,
+            3 * self.hidden_size_per_attention_head,
+        )
         mixed_raw_layer = mixed_raw_layer.view(*new_tensor_shape)
-        
+
         # [sq, b, np, hn]
-        (query_layer,
-            key_layer,
-            value_layer) = split_tensor_along_last_dim(mixed_raw_layer, 3)
+        (query_layer, key_layer, value_layer) = split_tensor_along_last_dim(mixed_raw_layer, 3)
 
         dropout_fn = attn.attention_dropout if attn.training else None
 
-        kw_args['position_ids'] = kw_args['position_ids'].transpose(0, 1)
-
-        cos, sin = self.rotary_emb(value_layer, seq_len=kw_args['position_ids'].max() + 1)
-
-        query_layer, key_layer = self.apply_rotary_fn(query_layer, key_layer, cos, sin, kw_args['position_ids'])
+        position_ids = kw_args["position_ids"]
+        if self.position_encoding_2d:
+            q1, q2 = query_layer.chunk(2, dim=(query_layer.ndim - 1))
+            k1, k2 = key_layer.chunk(2, dim=(key_layer.ndim - 1))
+            cos, sin = self.rotary_emb(q1, seq_len=position_ids.max() + 1)
+            position_ids, block_position_ids = position_ids[:, 0, :].transpose(0, 1).contiguous(), \
+                                               position_ids[:, 1, :].transpose(0, 1).contiguous()
+            q1, k1 = apply_rotary_pos_emb_index(q1, k1, cos, sin, position_ids)
+            q2, k2 = apply_rotary_pos_emb_index(q2, k2, cos, sin, block_position_ids)
+            query_layer = torch.concat([q1, q2], dim=(q1.ndim - 1))
+            key_layer = torch.concat([k1, k2], dim=(k1.ndim - 1))
+        else:
+            position_ids = position_ids.transpose(0, 1)
+            cos, sin = self.rotary_emb(value_layer, seq_len=position_ids.max() + 1)
+            query_layer, key_layer = apply_rotary_pos_emb_index(query_layer, key_layer, cos, sin, position_ids)
 
         context_layer = attention_fn(query_layer, key_layer, value_layer, mask, dropout_fn, **kw_args)
 
         output = attn.dense(context_layer)
 
         if attn.training:
             output = attn.output_dropout(output)
 
-
         return output
 
 
-class _GLUBaseModule(torch.nn.Module):
-    def __init__(self, activation_fn):
+class GEGLU(torch.nn.Module):
+    def __init__(self):
         super().__init__()
-        self.activation_fn = activation_fn
+        self.activation_fn = F.gelu
 
     def forward(self, x):
         # dim=-1 breaks in jit for pt<1.10
         x1, x2 = x.chunk(2, dim=(x.ndim - 1))
         return x1 * self.activation_fn(x2)
 
-class GEGLU(_GLUBaseModule):
-    def __init__(self):
-        super().__init__(F.gelu)
-
 
 class DeepNormWithGLUMixin(BaseMixin):
     def __init__(self, num_layers, hidden_size, inner_hidden_size=None):
         super().__init__()
         self.num_layers = num_layers
         self.hidden_size = hidden_size
         if inner_hidden_size is None:
             inner_hidden_size = 4 * hidden_size * 2 // 3
         self.inner_hidden_size = inner_hidden_size
 
     def reinit(self):
-        del self.transformer.position_embeddings
         for layer in self.transformer.layers:
             del layer.mlp.dense_h_to_4h
             layer.mlp.dense_h_to_4h = ColumnParallelLinear(
                 self.hidden_size,
                 2 * self.inner_hidden_size,
                 gather_output=False,
                 bias=True,
                 params_dtype=torch.half,
                 module=self,
                 name="dense_h_to_4h",
                 skip_init=True,
-                device=torch.cuda.current_device()
             )
             del layer.mlp.activation_func
             layer.mlp.activation_func = GEGLU()
 
-           
     def layer_forward(self, hidden_states, mask, *args, **kw_args):
-        '''
-            hidden_states: [seq_len, batch, hidden_size]
-            mask: [(1, 1), seq_len, seq_len]
-        '''
-        layer = self.transformer.layers[kw_args['layer_id']]
+        """
+        hidden_states: [seq_len, batch, hidden_size]
+        mask: [(1, 1), seq_len, seq_len]
+        """
+        layer = self.transformer.layers[kw_args["layer_id"]]
         # Layer norm at the begining of the transformer layer.
 
         attention_input = layer.input_layernorm(hidden_states)
 
         # Self attention.
         attention_output = layer.attention(attention_input, mask, **kw_args)
 
         # Residual connection.
         alpha = (2 * self.num_layers) ** 0.5
         hidden_states = attention_input * alpha + attention_output
 
         mlp_input = layer.post_attention_layernorm(hidden_states)
 
-        if layer.is_decoder:
-            encoder_outputs = kw_args['encoder_outputs']
-            if encoder_outputs is not None:
-                assert 'cross_attention_mask' in kw_args
-                # Cross attention
-                attention_output = layer.cross_attention(mlp_input, **kw_args)
-                # Residual connection.
-                hidden_states = hidden_states + attention_output
-                # Layer norm post the cross attention
-                mlp_input = layer.post_cross_attention_layernorm(hidden_states)
-
         # MLP.
         mlp_output = layer.mlp(mlp_input, **kw_args)
 
         # Second residual connection.
         output = mlp_input * alpha + mlp_output
 
         return output
 
+
 class SelfAttentionWithFP32SoftmaxMixin(BaseMixin):
     def __init__(self, hidden_size, num_attention_heads, model_parallel_size):
-        super().__init__()  
+        super().__init__()
         self.hidden_size_per_attention_head = divide(hidden_size, num_attention_heads)
-        self.hidden_size_per_partition = divide(hidden_size, model_parallel_size) 
+        self.hidden_size_per_partition = divide(hidden_size, model_parallel_size)
+        self.scale_mask_softmax = None
+        if FusedScaleMaskSoftmax is not None:
+            self.scale_mask_softmax = FusedScaleMaskSoftmax(
+                input_in_fp16=True,
+                input_in_bf16=False,
+                attn_mask_type=AttnMaskType.padding,
+                scaled_masked_softmax_fusion=True,
+                mask_func=self.attention_mask_func,
+                softmax_in_fp32=True,
+                scale=1,
+            )
 
-    def attention_fn(self, query_layer, key_layer, value_layer, attention_mask, attention_dropout=None, log_attention_weights=None, scaling_attention_score=True, mems=None, **kwargs):
+    @staticmethod
+    def attention_mask_func(attention_scores, attention_mask):
+        attention_scores.masked_fill_(attention_mask, -10000.0)
+        return attention_scores
+
+    def attention_fn(
+        self,
+        query_layer,
+        key_layer,
+        value_layer,
+        attention_mask,
+        attention_dropout=None,
+        log_attention_weights=None,
+        scaling_attention_score=True,
+        mems=None,
+        **kwargs
+    ):
+
+        mem = mems[kwargs["layer_id"]] if mems is not None else None
 
-        mem = mems[kwargs['layer_id']] if mems is not None else None
-        
         # seqlen, batch, head, hidden_size
         seq_len, b, nh, hidden_size = key_layer.shape
 
         # b, seqlen, stack, head, hidden
-        cache_kv = torch.stack((key_layer, value_layer)).permute(2, 1, 0, 3, 4).detach().contiguous().view(b, seq_len, nh * hidden_size * 2)
-        kwargs['output_this_layer']['mem_kv'] = cache_kv
+        cache_kv = (
+            torch.stack((key_layer, value_layer))
+            .permute(2, 1, 0, 3, 4)
+            .detach()
+            .contiguous()
+            .view(b, seq_len, nh * hidden_size * 2)
+        )
+        kwargs["output_this_layer"]["mem_kv"] = cache_kv
 
-        if mem is not None: # the first time, mem is None
+        if mem is not None:  # the first time, mem is None
             # might change batch_size
             # b, seqlen, stack, head, hidden -> stack, seqlen, b, head, hidden
             mem = mem.expand(b, -1, -1).reshape(b, mem.shape[1], 2, nh, hidden_size).permute(2, 1, 0, 3, 4)
             memk, memv = mem[0], mem[1]
             key_layer = torch.cat((memk, key_layer), dim=0)
             value_layer = torch.cat((memv, value_layer), dim=0)
 
-        # We disable the PB-relax-Attention and only changes the order of computation, because it is enough for most of training. 
-        # The implementation in the paper can be done very easily, if you really need it to train very deep transformers. 
-        query_key_layer_scaling_coeff = float(kwargs['layer_id'] + 1)
+        query_key_layer_scaling_coeff = float(kwargs["layer_id"] + 1)
         if scaling_attention_score:
             query_layer = query_layer / (math.sqrt(self.hidden_size_per_attention_head) * query_key_layer_scaling_coeff)
 
         # ===================================
         # Raw attention scores. [b, np, s, s]
         # ===================================
 
         # [b, np, sq, sk]
-        output_size = (query_layer.size(1),
-                       query_layer.size(2),
-                       query_layer.size(0),
-                       key_layer.size(0))
+        output_size = (query_layer.size(1), query_layer.size(2), query_layer.size(0), key_layer.size(0))
 
         # [sq, b, np, hn] -> [sq, b * np, hn]
-        query_layer = query_layer.view(output_size[2],
-                                       output_size[0] * output_size[1], -1)
+        query_layer = query_layer.view(output_size[2], output_size[0] * output_size[1], -1)
         # [sk, b, np, hn] -> [sk, b * np, hn]
-        key_layer = key_layer.view(output_size[3],
-                                   output_size[0] * output_size[1], -1)
+        key_layer = key_layer.view(output_size[3], output_size[0] * output_size[1], -1)
 
         matmul_result = torch.empty(
-                output_size[0]*output_size[1],
-                output_size[2],
-                output_size[3],
-                dtype=query_layer.dtype,
-                device=torch.cuda.current_device())
-        
+            output_size[0] * output_size[1],
+            output_size[2],
+            output_size[3],
+            dtype=query_layer.dtype,
+            device=torch.cuda.current_device(),
+        )
+
         matmul_result = torch.baddbmm(
-                matmul_result,
-                query_layer.transpose(0, 1),   # [b * np, sq, hn]
-                key_layer.transpose(0, 1).transpose(1, 2),  # [b * np, hn, sk]
-                beta=0.0, alpha=1.0)
+            matmul_result,
+            query_layer.transpose(0, 1),  # [b * np, sq, hn]
+            key_layer.transpose(0, 1).transpose(1, 2),  # [b * np, hn, sk]
+            beta=0.0,
+            alpha=1.0,
+        )
 
         # change view to [b, np, sq, sk]
         attention_scores = matmul_result.view(*output_size)
 
-
         # if log_attention_weights is not None:
         #     attention_scores += log_attention_weights
 
-        if not (attention_mask.shape[-2] == 1 and (attention_mask > 0).all()):
-            # if auto-regressive, skip
-            attention_scores = torch.mul(attention_scores, attention_mask) - \
-                            10000.0 * (1.0 - attention_mask)
-
-    
-
-        attention_scores = attention_scores.float()
-        attention_scores = attention_scores * query_key_layer_scaling_coeff
+        if self.scale_mask_softmax:
+            self.scale_mask_softmax.scale = query_key_layer_scaling_coeff
+            attention_probs = self.scale_mask_softmax(attention_scores, attention_mask.contiguous())
+        else:
+            if not (attention_mask.shape[-2] == 1 and (attention_mask > 0).all()):
+                # if auto-regressive, skip
+                attention_scores.masked_fill_(attention_mask, -10000.0)
 
-        attention_probs = F.softmax(attention_scores, dim=-1)
+            attention_scores = attention_scores.float()
+            attention_scores = attention_scores * query_key_layer_scaling_coeff
 
-        attention_probs = attention_probs.half()
+            attention_probs = F.softmax(attention_scores, dim=-1)
 
+            attention_probs = attention_probs.half()
 
         if attention_dropout is not None:
             if mpu.get_cuda_rng_tracker is not None:
                 with mpu.get_cuda_rng_tracker().fork():
                     attention_probs = attention_dropout(attention_probs)
             else:
                 attention_probs = attention_dropout(attention_probs)
-                
+
         # =========================
         # Context layer. [sq, b, hp]
         # =========================
 
         # value_layer -> context layer.
         # [sk, b, np, hn] --> [b, np, sq, hn]
 
         # context layer shape: [b, np, sq, hn]
-        output_size = (value_layer.size(1),
-                       value_layer.size(2),
-                       query_layer.size(0),
-                       value_layer.size(3))
+        output_size = (value_layer.size(1), value_layer.size(2), query_layer.size(0), value_layer.size(3))
 
         # change view [sk, b * np, hn]
-        value_layer = value_layer.view(value_layer.size(0),
-                                       output_size[0] * output_size[1], -1)
+        value_layer = value_layer.view(value_layer.size(0), output_size[0] * output_size[1], -1)
 
         # change view [b * np, sq, sk]
-        attention_probs = attention_probs.view(output_size[0] * output_size[1],
-                                               output_size[2], -1)
+        attention_probs = attention_probs.view(output_size[0] * output_size[1], output_size[2], -1)
 
         # matmul: [b * np, sq, hn]
         context_layer = torch.bmm(attention_probs, value_layer.transpose(0, 1))
 
         # change view [b, np, sq, hn]
         context_layer = context_layer.view(*output_size)
 
         # [b, np, sq, hn] --> [sq, b, np, hn]
         context_layer = context_layer.permute(2, 0, 1, 3).contiguous()
 
         # [sq, b, np, hn] --> [sq, b, hp]
-        new_context_layer_shape = context_layer.size()[:-2] + \
-            (self.hidden_size_per_partition,)
+        new_context_layer_shape = context_layer.size()[:-2] + (self.hidden_size_per_partition,)
         context_layer = context_layer.view(*new_context_layer_shape)
-        
-        # context_layer = torch.matmul(attention_probs, value_layer)
-        
+
         return context_layer
 
+
 class FinalForwardMixin(BaseMixin):
     def __init__(self):
         super().__init__()
 
     def final_forward(self, logits, **kw_args):
         return F.linear(logits, self.transformer.word_embeddings.weight).transpose(0, 1).contiguous()
 
+
 class NonePositionEmbedding(BaseMixin):
     def __init__(self):
         super().__init__()
 
     def position_embedding_forward(self, position_ids, output_cross_layer, **kw_args):
         return None
 
+
 class WordEmbedding(BaseMixin):
     def __init__(self):
         super().__init__()
 
     def word_embedding_forward(self, input_ids, output_cross_layer, **kw_args):
         return self.transformer.word_embeddings(input_ids).transpose(0, 1)
 
 
 class GLM130B(BaseModel):
     def __init__(self, args, transformer=None, parallel_output=False):
-        super().__init__(args, params_dtype=torch.half if args.fp16 else torch.float, transformer=transformer, parallel_output=parallel_output)
-        self.add_mixin('glu-deepnorm',
-            DeepNormWithGLUMixin(args.num_layers, args.hidden_size, args.inner_hidden_size)
-        )
-        self.add_mixin('fp32-softmax', 
-            SelfAttentionWithFP32SoftmaxMixin(args.hidden_size, args.num_attention_heads, args.model_parallel_size)
-        )
-        self.add_mixin('final-forward', 
-            FinalForwardMixin()
+        super().__init__(
+            args,
+            params_dtype=torch.half if args.fp16 else torch.float,
+            transformer=transformer,
+            parallel_output=parallel_output,
         )
-        self.add_mixin('non-position-embedding', 
-            NonePositionEmbedding()
+        self.add_mixin("glu-deepnorm", DeepNormWithGLUMixin(args.num_layers, args.hidden_size, args.inner_hidden_size))
+        self.add_mixin(
+            "fp32-softmax",
+            SelfAttentionWithFP32SoftmaxMixin(args.hidden_size, args.num_attention_heads, args.model_parallel_size),
         )
-        self.add_mixin('word-embedding', 
-            WordEmbedding()
-        )
-        self.add_mixin('rotary-embedding', 
-            RotaryEmbeddingMixin(args.fp16, args.apply_rotary_positional_embedding_kernel, args.bf16, args.hidden_size, args.num_attention_heads, args.model_parallel_size)
+        self.add_mixin("final-forward", FinalForwardMixin())
+        self.add_mixin("non-position-embedding", NonePositionEmbedding())
+        del self.transformer.position_embeddings
+        self.add_mixin("word-embedding", WordEmbedding())
+        self.add_mixin(
+            "rotary-embedding",
+            RotaryEmbeddingMixin(
+                args.fp16,
+                args.hidden_size,
+                args.num_attention_heads,
+                args.model_parallel_size,
+                args.position_encoding_2d
+            ),
         )
-        self.get_mixin("glu-deepnorm").reinit()
+        if not args.no_glu:
+            self.get_mixin("glu-deepnorm").reinit()
 
     @classmethod
     def add_model_specific_args(cls, parser):
-        """Arguments for GLM"""
-        group = parser.add_argument_group('GLM', 'GLM Configurations')
-        
-        group.add_argument('--task-mask', action='store_true', help="Use different mask for generation and blank filling")
-
-        group.add_argument('--apply-rotary-positional-embedding-kernel', action='store_true', help="Apply rotary positional embedding kernel")
-
-        return parser
+        parser.add_argument('--position-encoding-2d', action='store_true', help='Use 2D rotary embedding.')
+        parser.add_argument('--no-glu', action='store_true', help='Disable GLU.')
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/glm_model.py` & `SwissArmyTransformer-0.3.1/sat/model/official/glm_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
 
-from SwissArmyTransformer.model.base_model import BaseModel, BaseMixin
+from sat.model.base_model import BaseModel, BaseMixin
 
 class BlockPositionEmbeddingMixin(BaseMixin):
     def __init__(self, max_sequence_length, hidden_size, init_method_std=0.02):
         super(BlockPositionEmbeddingMixin, self).__init__()
         self.max_sequence_length = max_sequence_length
         self.hidden_size = hidden_size
         self.block_position_embeddings = torch.nn.Embedding(max_sequence_length, hidden_size)
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/mae_model.py` & `SwissArmyTransformer-0.3.1/sat/model/official/mae_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from SwissArmyTransformer.model.base_model import BaseMixin, BaseModel, non_conflict
-from SwissArmyTransformer.model.official.vit_model import ViTModel
-from SwissArmyTransformer.model.mixins import BaseMixin
-from SwissArmyTransformer import mpu
+from sat.model.base_model import BaseMixin, BaseModel, non_conflict
+from sat.model.official.vit_model import ViTModel
+from sat.model.mixins import BaseMixin
+from sat import mpu
 
-from SwissArmyTransformer.model.position_embedding import get_2d_sincos_pos_embed
+from sat.model.position_embedding import get_2d_sincos_pos_embed
 
 """
 MAE model follows encoder-decoder architecture.
 For encoder, it is a normal ViTModel with customed position embeddings.
 For decoder, it is a normal BaseModel adding [MASK] token.
 """
 
-from SwissArmyTransformer.model.official.vit_model import InterpolatedPositionEmbeddingMixin
+from sat.model.official.vit_model import InterpolatedPositionEmbeddingMixin
 
 class PosMixin(InterpolatedPositionEmbeddingMixin):
     def __init__(self, hidden_size, old_property, property, init_method_std=0.02):
         super().__init__(hidden_size, old_property, property, init_method_std=init_method_std)
         self.hidden_size = hidden_size
 
     def reinit(self, parent_model=None):
@@ -125,15 +125,15 @@
     def __init__(self, args, transformer=None, parallel_output=True, layernorm_epsilon=1e-6):
         super().__init__(args, transformer=transformer, parallel_output=parallel_output, layernorm_epsilon=layernorm_epsilon)
         self.add_mixin('mask_forward', MaskMixin(args))
     @classmethod
     def add_model_specific_args(cls, parser):
         return super().add_model_specific_args(parser)
 
-from SwissArmyTransformer.model import EncoderDecoderModel
+from sat.model import EncoderDecoderModel
 import argparse
 
 class MAE(EncoderDecoderModel):
     def __init__(self, args, transformer=None, parallel_output=True, layernorm_epsilon=1e-6):
         encoder = MAEEncoder(args, transformer=transformer, parallel_output=parallel_output, layernorm_epsilon=layernorm_epsilon)
         dec_args = argparse.Namespace(**vars(args))
         # dec_args.enc_hidden_size = dec_args.hidden_size  # used for cross attn
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/t5_model.py` & `SwissArmyTransformer-0.3.1/sat/model/official/t5_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import math
 import torch
 import torch.nn.functional as F
-from SwissArmyTransformer.model.mixins import BaseMixin
-from SwissArmyTransformer.model.encoder_decoder_model import EncoderDecoderModel
-from SwissArmyTransformer.model.base_model import non_conflict
-from SwissArmyTransformer.mpu import get_model_parallel_world_size
-from SwissArmyTransformer.model.transformer import standard_attention, SelfAttention, CrossAttention, MLP
-from SwissArmyTransformer.mpu.mappings import copy_to_model_parallel_region
-from SwissArmyTransformer.mpu.utils import divide, split_tensor_along_last_dim, unscaled_init_method
-from SwissArmyTransformer.mpu.layers import ColumnParallelLinear, VocabParallelEmbedding
+from sat.model.mixins import BaseMixin
+from sat.model.encoder_decoder_model import EncoderDecoderModel
+from sat.model.base_model import non_conflict
+from sat.mpu import get_model_parallel_world_size
+from sat.model.transformer import standard_attention, SelfAttention, CrossAttention, MLP
+from sat.mpu.mappings import copy_to_model_parallel_region
+from sat.mpu.utils import divide, split_tensor_along_last_dim, unscaled_init_method
+from sat.mpu.layers import ColumnParallelLinear, VocabParallelEmbedding
 
 
 class T5PositionEmbeddingMixin(BaseMixin):
     def position_embedding_forward(self, position_ids, **kw_args):
         return None
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/vit_model.py` & `SwissArmyTransformer-0.3.1/sat/model/official/vit_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 # @Modified:   2022/04/08
 # @By      :   Qingsong Lv
 # @Contact :   lqs19@mails.tsinghua.edu.cn
 import argparse
 
 import torch
 
-from SwissArmyTransformer.model.base_model import BaseModel
-from SwissArmyTransformer.model.mixins import BaseMixin
+from sat.model.base_model import BaseModel
+from sat.model.mixins import BaseMixin
 import torch.nn as nn
 from collections.abc import Iterable
 import math
 import torch.nn.functional as F
 
 
 gelu = nn.functional.gelu
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/official/yolos_model.py` & `SwissArmyTransformer-0.3.1/sat/model/official/yolos_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from SwissArmyTransformer.model import ViTModel
-from SwissArmyTransformer.model.official.vit_model import ImagePatchEmbeddingMixin
-from SwissArmyTransformer.model.mixins import BaseMixin
+from sat.model import ViTModel
+from sat.model.official.vit_model import ImagePatchEmbeddingMixin
+from sat.model.mixins import BaseMixin
 
 
 class NewTokenMixin(ImagePatchEmbeddingMixin):
     def __init__(self, new_token_size, in_channels, hidden_size, property, init_method_std=0.02):
         super(NewTokenMixin, self).__init__(in_channels, hidden_size, property)
         self.new_token_size = new_token_size
         self.init_method_std = init_method_std
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/position_embedding/rotary_embeddings.py` & `SwissArmyTransformer-0.3.1/sat/model/position_embedding/rotary_embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,17 @@
         else:
             self.register_buffer('inv_freq', inv_freq)
             self.max_seq_len_cached = None
             self.cos_cached = None
             self.sin_cached = None
         self.precision = precision
 
+    def _load_from_state_dict(self, state_dict, prefix, local_metadata, strict, missing_keys, unexpected_keys, error_msgs):
+        pass
+
     def forward(self, x, seq_dim=1, seq_len=None):
         if seq_len is None:
             seq_len = x.shape[seq_dim]
         if self.max_seq_len_cached is None or (seq_len > self.max_seq_len_cached):
             self.max_seq_len_cached = None if self.learnable else seq_len
             t = torch.arange(seq_len, device=x.device, dtype=self.inv_freq.dtype)
             freqs = torch.einsum('i,j->ij', t, self.inv_freq)
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/position_embedding/sincos2d.py` & `SwissArmyTransformer-0.3.1/sat/model/position_embedding/sincos2d.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/model/transformer.py` & `SwissArmyTransformer-0.3.1/sat/model/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 """Transformer."""
 
 import math
 import copy
 import torch
 import torch.nn.functional as F
 
-from SwissArmyTransformer import mpu
-from SwissArmyTransformer.mpu.initialize import get_model_parallel_world_size
-from SwissArmyTransformer.mpu.layers import ColumnParallelLinear, RowParallelLinear, VocabParallelEmbedding
-from SwissArmyTransformer.mpu.mappings import gather_from_model_parallel_region, copy_to_model_parallel_region
+from sat import mpu
+from sat.mpu.initialize import get_model_parallel_world_size
+from sat.mpu.layers import ColumnParallelLinear, RowParallelLinear, VocabParallelEmbedding
+from sat.mpu.mappings import gather_from_model_parallel_region, copy_to_model_parallel_region
 
 from deepspeed.runtime.activation_checkpointing.checkpointing import checkpoint
 
-from SwissArmyTransformer.mpu.utils import divide, sqrt, scaled_init_method, unscaled_init_method, gelu
-from SwissArmyTransformer.mpu.utils import split_tensor_along_last_dim
-from SwissArmyTransformer.ops import LayerNorm
+from sat.mpu.utils import divide, sqrt, scaled_init_method, unscaled_init_method, gelu
+from sat.mpu.utils import split_tensor_along_last_dim
+from sat.ops import LayerNorm
 
-from SwissArmyTransformer.transformer_defaults import HOOKS_DEFAULT, standard_attention
+from sat.transformer_defaults import HOOKS_DEFAULT, standard_attention
 
 
 class SelfAttention(torch.nn.Module):
     def __init__(self, hidden_size, num_attention_heads,
                  attention_dropout_prob, output_dropout_prob,
                  init_method, layer_id, hidden_size_per_attention_head=None, output_layer_init_method=None, bias=True,
                  hooks={}, transformer_pointer=None, params_dtype=torch.float, skip_init=False, device=torch.device('cpu')):
@@ -107,15 +107,16 @@
             return HOOKS_DEFAULT['attention_forward'](self, hidden_states, mask, **kw_args)
 
 
 class CrossAttention(torch.nn.Module):
     """Parallel cross-attention layer for Transformer"""
 
     def __init__(self, hidden_size, num_attention_heads, attention_dropout_prob, output_dropout_prob, init_method,
-                 layer_id, hidden_size_per_attention_head=None, output_layer_init_method=None, bias=True, hooks={},transformer_pointer=None, params_dtype=torch.float, skip_init=False, device=torch.device('cpu')):
+                 layer_id, hidden_size_per_attention_head=None, output_layer_init_method=None, bias=True, hooks={},
+                 transformer_pointer=None, params_dtype=torch.float, skip_init=False, device=torch.device('cpu')):
         super().__init__()
         # Set output layer initialization if not provided.
         if output_layer_init_method is None:
             output_layer_init_method = init_method
         self.hooks = hooks
         self.layer_id = layer_id
         # Per attention head and per partition values.
@@ -419,16 +420,16 @@
         self.use_final_layernorm = use_final_layernorm
         if use_final_layernorm:
             self.final_layernorm = layernorm(hidden_size, eps=layernorm_epsilon)
 
     def forward(self, input_ids, position_ids, attention_mask, *,
                 output_hidden_states=False, **kw_args):
         # sanity check
-        assert len(input_ids.shape) == 2
-        batch_size, query_length = input_ids.shape
+        assert len(input_ids.shape) >= 2
+        batch_size, query_length = input_ids.shape[:2]
 
         if attention_mask is None:
             attention_mask = torch.ones(1, 1, device=input_ids.device).type_as(
                 next(self.parameters())
             )  # None means full attention
         assert len(attention_mask.shape) == 2 or \
                len(attention_mask.shape) == 4 and attention_mask.shape[1] == 1
@@ -442,15 +443,15 @@
         else:  # default
             hidden_states = HOOKS_DEFAULT['word_embedding_forward'](self, input_ids, output_cross_layer=output_cross_layer,**kw_args)
 
         if 'position_embedding_forward' in self.hooks:
             position_embeddings = self.hooks['position_embedding_forward'](position_ids, output_cross_layer=output_cross_layer, **kw_args)
         else:
             assert len(position_ids.shape) <= 2
-            assert position_ids.shape[-1] == query_length
+            assert position_ids.shape[-1] == hidden_states.shape[1], (position_ids.shape, hidden_states.shape)
             position_embeddings = HOOKS_DEFAULT['position_embedding_forward'](self, position_ids, output_cross_layer=output_cross_layer, **kw_args)
         if position_embeddings is not None:
             hidden_states = hidden_states + position_embeddings
         hidden_states = self.embedding_dropout(hidden_states)
 
         output_per_layers = []
         if self.checkpoint_activations:
@@ -471,15 +472,15 @@
 
                     output_per_layers_part = []
                     for i, layer in enumerate(layers_):
                         output_this_layer_obj, output_cross_layer_obj = {}, {}
                         if 'layer_forward' in self.hooks:
                             layer_ret = self.hooks['layer_forward'](
                                 x_, mask, layer_id=layer.layer_id,
-                                **kw_args, **output_cross_layer,
+                                **kw_args, position_ids=position_ids, **output_cross_layer,
                                 output_this_layer=output_this_layer_obj,
                                 output_cross_layer=output_cross_layer_obj
                             )
                         else:
                             layer_ret = layer(
                                 x_, mask, layer_id=layer.layer_id,
                                 **kw_args, **output_cross_layer,
@@ -579,9 +580,9 @@
             logits_parallel = HOOKS_DEFAULT['final_forward'](self, logits, **kw_args)
 
         if not self.parallel_output:
             logits_parallel = gather_from_model_parallel_region(logits_parallel)
 
         outputs = [logits_parallel]
         outputs.extend(output_per_layers)
-
+        
         return outputs
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/__init__.py` & `SwissArmyTransformer-0.3.1/sat/mpu/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/cross_entropy.py` & `SwissArmyTransformer-0.3.1/sat/mpu/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/data.py` & `SwissArmyTransformer-0.3.1/sat/mpu/data.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/initialize.py` & `SwissArmyTransformer-0.3.1/sat/mpu/initialize.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/layers.py` & `SwissArmyTransformer-0.3.1/sat/mpu/layers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/mappings.py` & `SwissArmyTransformer-0.3.1/sat/mpu/mappings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/mpu/utils.py` & `SwissArmyTransformer-0.3.1/sat/mpu/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/ops/layernorm.py` & `SwissArmyTransformer-0.3.1/sat/ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/ops/local_attention_function.py` & `SwissArmyTransformer-0.3.1/sat/ops/local_attention_function.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/resources/download.py` & `SwissArmyTransformer-0.3.1/sat/resources/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 import sys
 import math
 import random
 import requests
 from tqdm import tqdm
 from filelock import FileLock
-from .urls import MODEL_ULRS
+from .urls import MODEL_URLS
 
 def download_with_progress_bar(save_path, url):
     with requests.get(url, stream=True) as r:
         r.raise_for_status()
         os.makedirs(os.path.dirname(save_path), exist_ok=True)
         with open(save_path, 'wb') as f:
             pbar = tqdm(total=int(r.headers['Content-Length']), unit_scale=True)
@@ -36,15 +36,15 @@
     os.makedirs(os.path.dirname(file_path), exist_ok=True)
     lock = FileLock(file_path + '.lock')
     with lock:
         if os.path.exists(file_path) or os.path.isdir(model_path):
             pass
         else:
             if url is None:
-                url = MODEL_ULRS[name]
+                url = MODEL_URLS[name]
             print(f'Downloading models {url} into {file_path} ...')
             download_with_progress_bar(file_path, url)
         # unzip
         if not os.path.isdir(model_path):
             import zipfile
             print(f'Unzipping {file_path}...')
             f = zipfile.ZipFile(file_path, 'r')
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/resources/urls.py` & `SwissArmyTransformer-0.3.1/sat/resources/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,42 @@
-MODEL_ULRS = {
+MODEL_URLS = {
     'bert-base-uncased': 'https://cloud.tsinghua.edu.cn/f/f45fff1a308846cfa63a/?dl=1',
     'bert-large-uncased': 'https://cloud.tsinghua.edu.cn/f/6d4f38c96e8c4c16917e/?dl=1',
     'roberta-base': 'https://cloud.tsinghua.edu.cn/f/307fd141932440bc92da/?dl=1',
     'roberta-large': 'https://cloud.tsinghua.edu.cn/f/66c42c24ca304cecaf7e/?dl=1',
     'vit-base-patch16-224-in21k': 'https://cloud.tsinghua.edu.cn/f/fdf40233d9034b6a8bdc/?dl=1',
     'deit-tiny': 'https://cloud.tsinghua.edu.cn/f/b759657cb80e4bc69303/?dl=1',
     'deit-small': 'https://cloud.tsinghua.edu.cn/f/51498210e2c943dbbef1/?dl=1',
     'deit-base': 'https://cloud.tsinghua.edu.cn/f/9a26fd1aee7146e1a848/?dl=1',
     'cait-s24-224': 'https://cloud.tsinghua.edu.cn/f/bdfb12396000468b8bb9/?dl=1',
-    'clip': 'https://cloud.tsinghua.edu.cn/f/bd29f0537f9949e6a4fb/?dl=1',
+    'gpt2': 'https://cloud.tsinghua.edu.cn/f/4448cff2f1644bd88fa9/?dl=1',
+    'chatglm-6b': 'https://cloud.tsinghua.edu.cn/f/26587ca6dd6f45f1ae85/?dl=1',
+    'eva02_L_pt_m38m_p14': 'https://cloud.tsinghua.edu.cn/f/98feef10af4f4ff79764/?dl=1',
+    # CLIP
+    'clip': 'https://cloud.tsinghua.edu.cn/f/bd29f0537f9949e6a4fb/?dl=1', # vit-base-patch32
+    'clip-vit-base-patch16': 'https://lfs.aminer.cn/misc/clip/clip-vit-base-patch16.zip',
+    'clip-vit-large-patch14': 'https://lfs.aminer.cn/misc/clip/clip-vit-large-patch14.zip',
     'yolos-tiny': 'https://cloud.tsinghua.edu.cn/f/8ee048b6a1f1403d9253/?dl=1',
     'mae-vit-base': 'https://cloud.tsinghua.edu.cn/f/5ab3543f0e1d4507ad8c/?dl=1',
     'cogview-base': 'https://cloud.tsinghua.edu.cn/f/df21f6d4109b4285bfd9/?dl=1',
     'glm-large-zh': 'https://lfs.aminer.cn/misc/cogview/glm/glm-large-zh.zip',
     'glm-large-en-blank': 'https://lfs.aminer.cn/misc/cogview/glm/glm-large-en-blank.zip',
     'glm-10b-en': 'https://lfs.aminer.cn/misc/cogview/glm/glm-10b-en.zip',
     'glm-10b-zh': 'https://lfs.aminer.cn/misc/cogview/glm/glm-10b-zh.zip',
     # 'glm-large-zh': 'https://cloud.tsinghua.edu.cn/f/df21f6d4109b4285bfd9/?dl=1',
     # 'glm-large-en-blank': 'https://cloud.tsinghua.edu.cn/f/df21f6d4109b4285bfd9/?dl=1',
+    'gpt-neo-1.3b': 'https://cloud.tsinghua.edu.cn/f/22e87976b5b745ad90af/?dl=1',
 
     # CogView2
     'coglm': 'https://lfs.aminer.cn/misc/cogview/cogview2/coglm.zip',
     'cogview2-dsr': 'https://lfs.aminer.cn/misc/cogview/cogview2/cogview2-dsr.zip',
     'cogview2-itersr': 'https://lfs.aminer.cn/misc/cogview/cogview2/cogview2-itersr.zip',
     
     # CogVideo
     'cogvideo-stage1': 'https://lfs.aminer.cn/misc/cogvideo/cogvideo-stage1.zip', 
     'cogvideo-stage2': 'https://lfs.aminer.cn/misc/cogvideo/cogvideo-stage2.zip',
+    
+    # DPR
+    'dpr-ctx_encoder-single-nq-base': 'https://cloud.tsinghua.edu.cn/f/e5475f1211a948708baa/?dl=1',
+    'dpr-question_encoder-single-nq-base': 'https://cloud.tsinghua.edu.cn/f/5c4aae7d11fc4c45a5bd/?dl=1',
+    'dpr-reader-single-nq-base': 'https://cloud.tsinghua.edu.cn/f/e169889ab40d4615a34d/?dl=1',
 }
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/__init__.py` & `SwissArmyTransformer-0.3.1/sat/tokenization/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # here put the import lib
 import os
 import sys
 import math
 import random
 import torch
 
-from SwissArmyTransformer.training.utils import print_rank_0
+from sat.training.utils import print_rank_0
 
 
 def get_tokenizer(args=None, *, tokenizer_type=None, outer_tokenizer=None):
     '''
         If you're using outer_tokenizer, call `get_tokenizer(args, outer_tokenizer)`
         before `training_main`.
     '''
@@ -51,14 +51,17 @@
                     "add_decoder_mask": args.block_mask_prob > 0.0}
         if tokenizer_type == "glm_GPT2BPETokenizer":
             from .glm import GPT2BPETokenizer
             get_tokenizer.tokenizer = GPT2BPETokenizer(args.tokenizer_model_type, **kwargs)
         elif tokenizer_type == "glm_ChineseSPTokenizer":
             from .glm import ChineseSPTokenizer
             get_tokenizer.tokenizer = ChineseSPTokenizer(args.tokenizer_model_type, **kwargs)
+        elif tokenizer_type == "glm_BertWordPieceTokenizer":
+            from .glm import BertWordPieceTokenizer
+            get_tokenizer.tokenizer = BertWordPieceTokenizer(args.tokenizer_model_type, **kwargs)
     elif tokenizer_type == 'icetk':
         from icetk import icetk
         get_tokenizer.tokenizer = icetk
     elif tokenizer_type == 'icetk-glm-130B':
         from .icetk_glm_130B import _IceTokenizer
         get_tokenizer.tokenizer = _IceTokenizer()
     # elif tokenizer_type.startswith('hf'):
@@ -66,17 +69,17 @@
     #     if tokenizer_type == "hf_T5Tokenizer":
     #         get_tokenizer.tokenizer = HFT5Tokenizer(args.tokenizer_model_type, cache_dir=args.cache_dir)
     else:
         print_rank_0('Try to load tokenizer from Huggingface transformers...')
         os.environ['TOKENIZERS_PARALLELISM'] = 'true'
         from transformers import AutoTokenizer
         try:
-            get_tokenizer.tokenizer = AutoTokenizer.from_pretrained(tokenizer_type)
+            get_tokenizer.tokenizer = AutoTokenizer.from_pretrained(tokenizer_type, trust_remote_code=True)
         except OSError as e:
-            print_rank_0(f'Cannot find {tokenizer_type} from Huggingface or SwissArmyTransformer. Creating a fake tokenizer...')
+            print_rank_0(f'Cannot find {tokenizer_type} from Huggingface or sat. Creating a fake tokenizer...')
             assert args.vocab_size > 0
             get_tokenizer.tokenizer = FakeTokenizer(args.vocab_size)
             return get_tokenizer.tokenizer
     print_rank_0(f'> Set tokenizer as a {tokenizer_type} tokenizer! Now you can get_tokenizer() everywhere.')
     return get_tokenizer.tokenizer
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/sp_tokenizer.py` & `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/templates.py` & `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/templates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/unified_tokenizer.py` & `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/unified_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/vqvae/api.py` & `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/api.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/vqvae/vqvae_diffusion.py` & `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/vqvae_diffusion.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/vqvae/vqvae_zc.py` & `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/vqvae_zc.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/cogview/vqvae_tokenizer.py` & `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model` & `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab` & `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt` & `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt` & `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt` & `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json` & `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/english_tokenizer/roberta-merges.txt` & `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/embed_assets/english_tokenizer/roberta-vocab.json` & `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/glm/sp_tokenizer.py` & `SwissArmyTransformer-0.3.1/sat/tokenization/glm/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/glm/tokenization.py` & `SwissArmyTransformer-0.3.1/sat/tokenization/glm/tokenization.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import os
 import csv
 import torch
 import itertools
 
 
 from .tokenization_gpt2 import GPT2Tokenizer
+from .tokenization_wordpiece import BertTokenizer
 from .sp_tokenizer import SentencePieceTokenizer
 
 class Tokenization(object):
     """
     Tokenization object to hold tokenization, (processed text),and original
     text. Can hold tokenization as Ids or tokens.
 
@@ -150,15 +151,14 @@
     """
 
     def __init__(self, text_tokenizer, command_tokens=None):
         # set text tokenizer
         self.text_tokenizer = text_tokenizer
         if not hasattr(self, 'num_text_tokens'):
             self.num_text_tokens = len(self.text_tokenizer)
-        print(command_tokens)
         self._command_tokens = command_tokens
         self.command_name_map = {tok.name: tok for tok in self.command_tokens}
         self.command_token_map = {tok.token: tok for tok in self.command_tokens}
         self.command_id_map = {tok.Id: tok for tok in self.command_tokens}
 
         # parse tokens and vocabs from tokenizer
         max_token_id = max(len(self.text_tokenizer.tokens) - 1, max(self.command_id_map.keys()))
@@ -186,14 +186,20 @@
     def command_tokens(self):
         return self._command_tokens
 
     def __call__(self, text, process_fn=None):
         """run preprocessing and encode text as Ids"""
         return self.EncodeAsIds(text, process_fn=process_fn)
 
+    def tokenize(self, text):
+        return self.EncodeAsIds(text).tokenization
+
+    def detokenize(self, ids):
+        return self.DecodeIds(ids)
+
     def __len__(self):
         """total number of tokens"""
         return self.num_tokens
 
     def get_command(self, name):
         """get command token corresponding to `name`"""
         return self.command_name_map[name]
@@ -468,8 +474,111 @@
 
     def _encode(self, text):
         ids = self.text_tokenizer.encode(text)
         return ids
 
     def _decode(self, ids):
         text = self.text_tokenizer.decode(ids)
-        return text
+        return text
+
+
+class BertWordPieceTokenizer(Tokenizer):
+    """
+    Loads a pretrained WordPiece tokenizer from `cache_dir` for tokenization
+    in BERT training. Default to bert-large-uncased tokenizer.
+    """
+
+    def __init__(self, tokenizer_model_type=None, cache_dir=None, add_block_symbols=False, add_sentinel_token=0,
+                 add_task_mask=False, add_decoder_mask=False, added_command_tokens=None, **kwargs):
+        # default to bert-large-uncased tokenizer
+        do_lower_case = not ('-cased' in tokenizer_model_type or 'chinese' in tokenizer_model_type)
+        text_tokenizer = BertTokenizer.from_pretrained(tokenizer_model_type, do_lower_case=do_lower_case,
+                                                       cache_dir=cache_dir)
+        # disable max len warnings by increasing max len
+        text_tokenizer.max_len = int(1e12)
+        # set command tokens from wordpiece tokenizer values
+        num_tokens = len(text_tokenizer.vocab)
+
+        command_tokens = [
+            CommandToken('pad', '[PAD]', text_tokenizer.vocab['[PAD]']),
+            CommandToken('ENC', '[CLS]', text_tokenizer.vocab['[CLS]']),
+            CommandToken('MASK', '[MASK]', text_tokenizer.vocab['[MASK]']),
+            CommandToken('unk', '[UNK]', text_tokenizer.vocab['[UNK]']),
+            CommandToken('sep', '[SEP]', text_tokenizer.vocab['[SEP]']),
+            CommandToken('eos', '[PAD]', text_tokenizer.vocab['[PAD]']),
+        ]
+        if add_block_symbols:
+            command_tokens.extend([
+                CommandToken('sop', '<|startofpiece|>', num_tokens),
+                CommandToken('eop', '<|endofpiece|>', num_tokens + 1)
+            ])
+            num_tokens += 2
+            if add_task_mask:
+                command_tokens.extend([
+                    CommandToken('gMASK', '[gMASK]', num_tokens),
+                    CommandToken('sMASK', '[sMASK]', num_tokens + 1)
+                ])
+                num_tokens += 2
+            if add_decoder_mask:
+                command_tokens.extend([
+                    CommandToken('dBLOCK', '[dBLOCK]', num_tokens)
+                ])
+                num_tokens += 1
+        if add_sentinel_token > 0:
+            for i in range(1, add_sentinel_token):
+                command_tokens.extend([CommandToken(f'MASK{i}', f'[MASK{i}]', num_tokens),
+                                       CommandToken(f'sop{i}', f'<|startofpiece{i}|>', num_tokens + 1)])
+                num_tokens += 2
+
+        if added_command_tokens:
+            for name, token in added_command_tokens:
+                command_tokens.extend([
+                    CommandToken(name, token, num_tokens)
+                ])
+                num_tokens += 1
+        super().__init__(text_tokenizer, command_tokens=command_tokens)
+
+    def _encode(self, text):
+        tokens = self.text_tokenizer.tokenize(text)
+        ids = self.text_tokenizer.convert_tokens_to_ids(tokens)
+        return ids
+
+    @staticmethod
+    def clean_up_tokenization(out_string: str) -> str:
+        """
+        Clean up a list of simple English tokenization artifacts like spaces before punctuations and abbreviated forms.
+
+        Args:
+            out_string (:obj:`str`): The text to clean up.
+
+        Returns:
+            :obj:`str`: The cleaned-up string.
+        """
+        out_string = (
+            out_string.replace(" .", ".")
+                .replace(" ?", "?")
+                .replace(" !", "!")
+                .replace(" ,", ",")
+                .replace(" ' ", "'")
+                .replace(" n't", "n't")
+                .replace(" 'm", "'m")
+                .replace(" 's", "'s")
+                .replace(" 've", "'ve")
+                .replace(" 're", "'re")
+        )
+        return out_string
+
+    def _decode(self, ids):
+        Tokens = []
+        for Id in ids:
+            if Id in self.command_id_map:
+                Tokens.append(self.command_id_map[Id].token)
+            elif Id in self.text_tokenizer.tokens:
+                Tokens.append(self.text_tokenizer.tokens[Id])
+        new_tokens = []
+        for token in Tokens:
+            if token.startswith('##') and len(new_tokens) > 0:
+                new_tokens[-1] += token[2:]
+            else:
+                new_tokens.append(token)
+        output = ' '.join(new_tokens)
+        return output
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/glm/tokenization_gpt2.py` & `SwissArmyTransformer-0.3.1/sat/tokenization/glm/tokenization_gpt2.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     pairs = set()
     prev_char = word[0]
     for char in word[1:]:
         pairs.add((prev_char, char))
         prev_char = char
     return pairs
 
+
 class GPT2Tokenizer(object):
     """
     GPT-2 BPE tokenizer. Peculiarities:
         - Byte-level BPE
     """
     @classmethod
     def from_pretrained(cls, pretrained_model_name_or_path, cache_dir=None, *inputs, **kwargs):
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/hf_tokenizer.py` & `SwissArmyTransformer-0.3.1/sat/tokenization/hf_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,13 +68,14 @@
 
 class HFT5Tokenizer(HFTokenizer):
     def __init__(self, model_type_or_path=None, cache_dir=None):
         super().__init__(T5Tokenizer, model_type_or_path=model_type_or_path, cache_dir=cache_dir)
         command_tokens = [
             CommandToken('eos', '</s>', self.TokenToId("</s>")),
             CommandToken('pad', '<pad>', self.TokenToId("<pad>")),
-            CommandToken('sop', '<pad>', self.TokenToId("<pad>"))
+            CommandToken('sop', '<pad>', self.TokenToId("<pad>")),
+            CommandToken('eop', '</s>', self.TokenToId("</s>"))
         ]
         for i in range(100):
             command_tokens.append(CommandToken(f'MASK{i}', f'<extra_id_{i}>', self.TokenToId(f'<extra_id_{i}>')))
         self.command_tokens = command_tokens
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/tokenization/icetk_glm_130B/tokenizer.py` & `SwissArmyTransformer-0.3.1/sat/tokenization/icetk_glm_130B/tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/deepspeed_training.py` & `SwissArmyTransformer-0.3.1/sat/training/deepspeed_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,43 +31,44 @@
 
 from .utils import Timers
 from .utils import report_memory
 from .utils import print_args
 from .utils import print_rank_0
 from .utils import get_sample_writer
 
-from SwissArmyTransformer import mpu
-from SwissArmyTransformer.data_utils import make_loaders
-from SwissArmyTransformer.ops import LayerNorm
-from SwissArmyTransformer.arguments import set_random_seed, initialize_distributed
+from sat import mpu
+from sat.data_utils import make_loaders
+from sat.ops import LayerNorm
+from sat.arguments import set_random_seed, initialize_distributed
 
-def training_main(args, model_cls, forward_step_function, create_dataset_function, handle_metrics_function=None, init_function=None):
+def training_main(args, model_cls, forward_step_function, create_dataset_function, handle_metrics_function=None, init_function=None, collate_fn=None, forward_step_eval=None):
     """Main training program."""
     hooks = {
         'forward_step': forward_step_function,
         'init_function': init_function,
         'create_dataset_function': create_dataset_function,
         'handle_metrics': handle_metrics_function,
+        'forward_step_eval': forward_step_eval or forward_step_function
     }
 
     timers = Timers()  # Timer.
 
     # Experiment Name
     if args.load and args.mode == 'pretrain':  # continue training
         args.experiment_name = os.path.basename(os.path.normpath(args.load))
     else:
-        args.experiment_name = args.experiment_name + datetime.now().strftime("%m-%d-%H-%M")
+        args.experiment_name = args.experiment_name + '-' +datetime.now().strftime("%m-%d-%H-%M")
 
     # Pytorch distributed. must before seed. ALREADY MOVED TO arguments.py!
     # if isinstance(model_cls, type):
     #     initialize_distributed(args)
     #     set_random_seed(args.seed)  # Random seeds for reproducability.
 
     # Data stuff.
-    train_data, val_data, test_data = make_loaders(args, hooks['create_dataset_function'])
+    train_data, val_data, test_data = make_loaders(args, hooks['create_dataset_function'], collate_fn=collate_fn)
     if args.epochs:
         args.train_iters = len(train_data)
         if args.eval_interval is None:
             args.eval_interval = len(train_data)//args.epochs
         if args.save_interval is None:
             args.save_interval = len(train_data)//args.epochs
 
@@ -103,24 +104,25 @@
     if torch.distributed.get_rank() == 0:
         if args.mode == 'pretrain':
             print('Pretraining or Continuing training the Model...')
         elif args.mode == 'finetune':
             print('Finetuning Model...')
         print_args(args)
         summary_writer = get_sample_writer(base=args.summary_dir, name=args.experiment_name, iteration=args.iteration)
-        if hasattr(summary_writer, 'add_hparams'): # old version does not have this api
-            summary_writer.add_hparams(vars(args), {'_dump':0}, name=args.experiment_name, global_step=0)
 
     # Resume data loader if necessary.
     if args.resume_dataloader:
-        if train_data is not None:
-            train_data.batch_sampler.start_iter = args.iteration % len(train_data)
-        if val_data is not None:
-            start_iter_val = (args.train_iters // args.save_interval) * args.eval_interval
-            val_data.batch_sampler.start_iter = start_iter_val % len(val_data)
+        if not args.iterable_dataset:
+            if train_data is not None:
+                train_data.batch_sampler.start_iter = args.iteration % len(train_data)
+            if val_data is not None:
+                start_iter_val = (args.train_iters // args.save_interval) * args.eval_interval
+                val_data.batch_sampler.start_iter = start_iter_val % len(val_data)
+        else:
+            print('Warning: we cannot resume iterable dataloader. skipping...')
 
     # training 
     iteration = 0
     if args.train_iters > 0:
         if args.do_train:
             with ExitStack() as stack:
                 def save_on_exit(args_, model_, optimizer_, lr_scheduler_):
@@ -139,31 +141,31 @@
 
     # final testing
     if args.do_test and test_data is not None:
         prefix = 'the end of training for test data'
         test_loss = evaluate_and_print_results(prefix, iter(test_data),
             model, len(test_data) if args.strict_eval else args.eval_iters, args, timers, True, split='test', hooks=hooks)
 
-def get_model(args, model_cls):
+def get_model(args, model_cls, **kwargs):
     """Build the model."""
 
     print_rank_0(f'building {model_cls.__name__} model ...')
-    model = model_cls(args)
+    model = model_cls(args, **kwargs)
 
     if mpu.get_data_parallel_rank() == 0:
         print(' > number of parameters on model parallel rank {}: {}'.format(
             mpu.get_model_parallel_rank(),
             sum([p.nelement() for p in model.parameters()])), flush=True)
 
-    if args.fp16:
+    model.cuda(torch.cuda.current_device())
+    if hasattr(args, 'fp16') and args.fp16:
         model.half()
-    elif args.bf16:
+    elif hasattr(args, 'bf16') and args.bf16:
         model.bfloat16()
-    model.cuda(torch.cuda.current_device())
-
+    
     return model
 
 
 def setup_model_untrainable_params_and_optimizer(args, model, config_params=None):
     """Setup model and optimizer."""
 
     if hasattr(model, 'disable_untrainable_params'):
@@ -431,15 +433,15 @@
         # Reset the timer to avoid breaking timer logs below.
         timers('allreduce').reset()
 
     return
 
 def evaluate(data_iterator, model, eval_iters, args, timers, split, verbose=False, has_last=True, hooks={}):
     """Evaluation."""
-    forward_step = hooks['forward_step']
+    forward_step = hooks['forward_step_eval']
     # Turn on evaluation mode which disables dropout.
     model.eval()
     rank = torch.distributed.get_rank(group=mpu.get_data_parallel_group())
     total_lm_loss, metrics_total = 0, {}
     if split=='val':
         last_shape = args.val_last_shape
         drop_number = args.val_drop_number
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/deepspeed_zero1.json` & `SwissArmyTransformer-0.3.1/sat/training/deepspeed_zero1.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/deepspeed_zero2.json` & `SwissArmyTransformer-0.3.1/sat/training/deepspeed_zero2.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/learning_rates.py` & `SwissArmyTransformer-0.3.1/sat/training/learning_rates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/model_io.py` & `SwissArmyTransformer-0.3.1/sat/training/model_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import math
 import random
 import torch
 import numpy as np
 import json
 import argparse
 
-from SwissArmyTransformer import mpu
+from sat import mpu
 from .utils import print_rank_0
 
 def get_checkpoint_name(checkpoints_path, iteration, release=False, zero=False):
     if release:
         d = 'release'
     else:
         d = '{:d}'.format(iteration)
@@ -37,28 +37,34 @@
     parser = argparse.ArgumentParser()
     
     if hasattr(model, 'module'):
         model = model.module
     if isinstance(model, torch.nn.Module):
         for md in model.modules(): # search 
             if hasattr(md, 'add_model_specific_args'):
-                md.add_model_specific_args(parser)
+                try:
+                    md.add_model_specific_args(parser)
+                except argparse.ArgumentError as e:
+                    print(e)
     ret = {}
     for k in vars(parser.parse_args([])).keys():
         if hasattr(args, k):
             ret[k] = getattr(args, k)
     return ret
 
 def save_checkpoint(iteration, model, optimizer,
                     lr_scheduler, args):
     """Save a model checkpoint."""
     if args.deepspeed:
         if mpu.get_data_parallel_rank() == 0:
             print('Saving Model...')
             save_ds_checkpoint(iteration, model, lr_scheduler, args)
+    elif args.mode == 'inference':
+        os.makedirs(os.path.join(args.save, str(iteration)), exist_ok=True)
+        torch.save({'module': model.state_dict()}, os.path.join(args.save, str(iteration), 'mp_rank_00_model_states.pt'))
     else:
         raise ValueError("training without deepspeed is not supported.")
     # Wait so everyone is done (necessary)
     torch.distributed.barrier()
     # And update the latest iteration
     if torch.distributed.get_rank() == 0:
         tracker_filename = get_checkpoint_tracker_filename(args.save)
@@ -142,44 +148,61 @@
                 exit()
     assert iteration > 0 or release, 'error parsing metadata file {}'.format(
         tracker_filename)
 
     return iteration, release, True
 
 
-def load_checkpoint(model, args, load_path=None):
+def load_checkpoint(model, args, load_path=None, prefix=''):
     """Load a model checkpoint."""
     if load_path is None:
         load_path = args.load
 
+    # If model-only mode, set necessary args.
+    if not hasattr(args, 'mode'):
+        from copy import deepcopy
+        args = deepcopy(args)
+        args.mode = 'inference'
+
     iteration, release, success = get_checkpoint_iteration(load_path)
     if not success:
         return 0
     
     checkpoint_name = get_checkpoint_name(load_path, iteration, release)
     if mpu.get_data_parallel_rank() == 0:
             print('global rank {} is loading checkpoint {}'.format(
                 torch.distributed.get_rank(), checkpoint_name))
     sd = torch.load(checkpoint_name, map_location='cpu')
+    new_sd = {'module':{}}
+    for k in sd:
+        if k != 'module':
+            new_sd[k] = sd[k]
+    for k in sd['module']:
+        if k.startswith(prefix):
+            new_sd['module'][k[len(prefix):]] = sd['module'][k]
+    sd = new_sd
     
     if hasattr(model, 'module'):
         module = model.module
     else: # inference without deepspeed
         module = model
 
     # only load module, other hyperparameters are just for recording.
     missing_keys, unexpected_keys = module.load_state_dict(sd['module'], strict=False)
     if len(unexpected_keys) > 0:
         print_rank_0(
             f'Will continue but found unexpected_keys! Check whether you are loading correct checkpoints: {unexpected_keys}.')
     if len(missing_keys) > 0:
         if args.mode == 'inference':
-            raise ValueError(f'Missing keys for inference: {missing_keys}.')
+            if 'force_inference' in args and args.force_inference:
+                print(f'Warning: Missing keys for inference: {missing_keys}.')
+            else:
+                raise ValueError(f'Missing keys for inference: {missing_keys}.\nIf you still want to inference anyway, pass --force_inference to args.')
         else: # new params
-            assert all(name.find('mixins')>=0 for name in missing_keys)
+            assert all(name.find('mixins')>=0 for name in missing_keys), missing_keys
             assert args.mode == 'finetune'
             # list all mixin names
             mixin_names = []
             for key_name in missing_keys:
                 parts = key_name.split('.')
                 mixin_name = parts[parts.index('mixins')+1]
                 if mixin_name not in mixin_names:
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/training/utils.py` & `SwissArmyTransformer-0.3.1/sat/training/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 import time
 import numpy as np
 import torch
 
 from tensorboardX import SummaryWriter
 
 SUMMARY_WRITER_DIR_NAME = 'runs'
-ARGS_DIR_NAME = 'args'
 
 def get_sample_writer(name, base="..", iteration=0):
     """Returns a tensorboard summary writer
     """
     return SummaryWriter(
         log_dir=os.path.join(base, SUMMARY_WRITER_DIR_NAME, name), purge_step=iteration)
 
@@ -45,16 +44,16 @@
     """Print arguments."""
 
     print('arguments:', flush=True)
     for arg in vars(args):
         dots = '.' * (29 - len(arg))
         print('  {} {} {}'.format(arg, dots, getattr(args, arg)), flush=True)
     if args.save_args:
-        os.makedirs(ARGS_DIR_NAME, exist_ok=True)
-        with open(os.path.join(ARGS_DIR_NAME, args.experiment_name+'.txt'), "w") as f:
+        os.makedirs(os.path.join(args.summary_dir, SUMMARY_WRITER_DIR_NAME), exist_ok=True)
+        with open(os.path.join(args.summary_dir, SUMMARY_WRITER_DIR_NAME, args.experiment_name+'.txt'), "w") as f:
             for arg in vars(args):
                 dots = '.' * (29 - len(arg))
                 f.write('  {} {} {}\n'.format(arg, dots, getattr(args, arg)))
 
 
 class Timers:
     """Group of timers."""
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer/transformer_defaults.py` & `SwissArmyTransformer-0.3.1/sat/transformer_defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 '''
 
 import math
 import copy
 import torch
 import torch.nn.functional as F
 
-from SwissArmyTransformer import mpu
-from SwissArmyTransformer.mpu.initialize import get_model_parallel_world_size
-from SwissArmyTransformer.mpu.layers import ColumnParallelLinear, RowParallelLinear, VocabParallelEmbedding
-from SwissArmyTransformer.mpu.mappings import gather_from_model_parallel_region, copy_to_model_parallel_region
+from sat import mpu
+from sat.mpu.initialize import get_model_parallel_world_size
+from sat.mpu.layers import ColumnParallelLinear, RowParallelLinear, VocabParallelEmbedding
+from sat.mpu.mappings import gather_from_model_parallel_region, copy_to_model_parallel_region
 
 from deepspeed.runtime.activation_checkpointing.checkpointing import checkpoint
 
-from SwissArmyTransformer.mpu.utils import divide, sqrt, scaled_init_method, unscaled_init_method, gelu
-from SwissArmyTransformer.mpu.utils import split_tensor_along_last_dim
+from sat.mpu.utils import divide, sqrt, scaled_init_method, unscaled_init_method, gelu
+from sat.mpu.utils import split_tensor_along_last_dim
 
 def standard_attention(query_layer, key_layer, value_layer, attention_mask,
                        attention_dropout=None, log_attention_weights=None, scaling_attention_score=True, **kwargs):
     # We disable the PB-relax-Attention and only changes the order of computation, because it is enough for most of training. 
     # The implementation in the paper can be done very easily, if you really need it to train very deep transformers. 
 
     if scaling_attention_score:
```

### Comparing `SwissArmyTransformer-0.2.9/SwissArmyTransformer.egg-info/PKG-INFO` & `SwissArmyTransformer-0.3.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,18 @@
-Metadata-Version: 2.1
-Name: SwissArmyTransformer
-Version: 0.2.9
-Summary: A transformer-based framework with finetuning as the first class citizen.
-Home-page: https://github.com/THUDM/SwissArmyTransformer
-Author: Ming Ding, et al.
-Author-email: dm_thu@qq.com
-License: Apache 2.0 license
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Introduction
-`SwissArmyTransformer` is a flexible and powerful library to develop your own Transformer variants.
+`sat`(`SwissArmyTransformer`) is a flexible and powerful library to develop your own Transformer variants.
+
+`sat` is named after "swiss army knife", meaning that all the models (e.g. BERT, GPT, T5, GLM, CogView, ViT...) **share the same backone code** and cater for versatile usages with some extra light-weight mixins. 
+
+`sat` is powered by `deepspeed-ZeRO` and model parallelism, aiming to provide the best practice for pretraining and finetuning large models (100M\~20B parameters). 
 
-`SwissArmyTransformer` is named after "swiss army knife", meaning that all the models (e.g. BERT, GPT, T5, GLM, CogView, ViT...) **share the same backone code** and cater for versatile usages with some extra light-weight mixins. 
+# Migrate from SwissArmyTransformer 0.2.x to 0.3.x
+1. delete all `--sandwich-ln` in you script, use `layernorm-order='sandwich'`.
+2. change order `from_pretrained(args, name) => from_pretrained(name, args)`.
 
-`SwissArmyTransformer` is powered by `deepspeed-ZeRO` and model parallelism, aiming to provide the best practice for pretraining and finetuning large models (100M\~20B parameters). 
 ## Install
 ```
     pip install SwissArmyTransformer
 ```
 # Features
 
 * **Add model-agnostic components**, e.g. prefix-tuning, in just *ONE* line! 
@@ -34,19 +27,19 @@
                 # Arm an arbitrary model with Prefix-tuning with this line!
                 self.add_mixin('prefix-tuning', PrefixTuningMixin(args.num_layers, args.hidden_size // args.num_attention_heads, args.num_attention_heads, args.prefix_len))
     ```
 
     - GPT and other auto-regressive models act differently during training and inference. During inference, text is generated token-by-token and we need to cache previous states for efficiency. With our lib, you only need to consider the behavior during training (teacher-forcing) and transform it to a cached auto-regressive model via adding a mixin:
 
     ```python
-        model, args = AutoModel.from_pretrained(args, 'glm-10b-chinese')
+        model, args = AutoModel.from_pretrained('glm-10b-chinese', args)
         model.add_mixin('auto-regressive', CachedAutoregressiveMixin())
         # Generate a sequence with beam search
-        from SwissArmyTransformer.generation.autoregressive_sampling import filling_sequence
-        from SwissArmyTransformer.generation.sampling_strategies import BeamSearchStrategy
+        from sat.generation.autoregressive_sampling import filling_sequence
+        from sat.generation.sampling_strategies import BeamSearchStrategy
         output, *mems = filling_sequence(model, input_seq,
                         batch_size=args.batch_size,
                         strategy=BeamSearchStrategy(args.batch_size))
     ```     
 
 
 * **Build your Transformer-based model with minimal codes**. We mentioned [GLM](https://arxiv.org/pdf/2103.10360.pdf), which only differs from standard transformer (called BaseModel) on position embedding (and training losses). We only need to focus on the related part when coding.
@@ -74,66 +67,66 @@
         def __init__(self, args, transformer=None, parallel_output=True):
             super().__init__(args, transformer=transformer, parallel_output=parallel_output)
             self.add_mixin('block_position_embedding', 
                 BlockPositionEmbeddingMixin(args.max_sequence_length, args.hidden_size)
             ) # Add the mixin for GLM
     ```
 
-*  **Comprehensive supports for training**. `SwissArmyTransformer` aims to provide the best practice for pretraining and finetuning, where you only need to finish `forward_step` and `create_dataset_function` but with hyperparameters to alter useful training configurations.
+*  **Comprehensive supports for training**. `sat` aims to provide the best practice for pretraining and finetuning, where you only need to finish `forward_step` and `create_dataset_function` but with hyperparameters to alter useful training configurations.
     - Extend the training to multiple GPUs or nodes by specifying `--num_nodes`, `--num_gpus` and a simple `hostfile`. 
     - DeepSpeed and Model parallelism.
     - Better integration of ZeRO-2 and activation checkpointing.
     - Automatic extending and shuffling training data and `memmap`. 
     - Successfully support the training of [CogView2](http://github.com/THUDM/CogView2) and [CogVideo](https://github.com/THUDM/cogvideo).
     - The only open-source codebase supporting finetuning [T5-10B](https://arxiv.org/abs/1910.10683) on GPUs currently.
 
 </p></details>
 
 
 # Quick Tour
 
-The most typical python file to use `Bert` in SwissArmyTransformer (for inference) is as follows:
+The most typical python file to use `Bert` in sat (for inference) is as follows:
 ```python
 # @File: inference_bert.py
-from SwissArmyTransformer import get_args, get_tokenizer, AutoModel
+from sat import get_args, get_tokenizer, AutoModel
 # Parse args, initialize the environment. This is necessary.
 args = get_args() 
 # Automatically download and load model. Will also dump model-related hyperparameters to args.
-model, args = AutoModel.from_pretrained(args, 'bert-base-uncased') 
+model, args = AutoModel.from_pretrained('bert-base-uncased', args) 
 # Get the BertTokenizer according to args.tokenizer_type (automatically set).
 tokenizer = get_tokenizer(args) 
 # Here to use bert as you want!
 # ...
 ```
 Then we can run the code via
 ```bash
     SAT_HOME=/path/to/download python inference_bert.py --mode inference
 ```
-All officially supported model names are in [urls.py](SwissArmyTransformer/resources/urls.py).
+All officially supported model names are in [urls.py](sat/resources/urls.py).
 
 To finetune or pretrain a transformer is also extremely easy!
 ```python
 # @File: finetune_bert.py
-from SwissArmyTransformer import get_args, get_tokenizer, AutoModel
-from SwissArmyTransformer.model.mixins import MLPHeadMixin
+from sat import get_args, get_tokenizer, AutoModel
+from sat.model.mixins import MLPHeadMixin
 
 def create_dataset_function(path, args):
     # Here to load the dataset
     # ...
     assert isinstance(dataset, torch.utils.data.Dataset)
     return dataset
 
 def forward_step(data_iterator, model, args, timers):
     inputs = next(data_iterator) # from the dataset of create_dataset_function.
     loss, *others = model(inputs)
     return loss
     
 # Parse args, initialize the environment. This is necessary.
 args = get_args() 
-model, args = AutoModel.from_pretrained(args, 'bert-base-uncased') 
+model, args = AutoModel.from_pretrained('bert-base-uncased', args) 
 tokenizer = get_tokenizer(args) 
 # Here to use bert as you want!
 model.del_mixin('bert-final')
 model.add_mixin('classification_head', MLPHeadMixin(args.hidden_size, 2048, 1))
 # ONE LINE to train! 
 # args already includes hyperparams such as lr, train-iters, zero-stage ...
 training_main(args, 
@@ -150,34 +143,34 @@
     --train-data /path/to/train --valid-data /path/to/valid \
     --lr 0.00002 --batch-size 8 --zero-stage 1 --fp16
 ```
 Here we use data-parallel on GPUs 0,1. We can also launch the training on many inter-connected machines via `--hostfile /path/to/hostfile`. See the tutorial for more details.
 
 To write your own model, you only need to consider the difference between the standard Transformer. For example, if you have a idea to improve the attention operation:
 ```python
-from SwissArmyTransformer.model import BaseMixin
+from sat.model import BaseMixin
 class MyAttention(BaseMixin):
     def __init__(self, hidden_size):
         super(MyAttention, self).__init__()
         # MyAttention may needs some new params, e.g. a learnable alpha.
         self.learnable_alpha = torch.nn.Parameter(torch.ones(hidden_size))
     
     # This is a hook function, the name `attention_fn` is special.
     def attention_fn(q, k, v, mask, dropout=None, **kwargs):
         # Code for my attention.
         # ...
         return attention_results
 ```
-Here `attention_fn` is a hook function, replacing the default action by the new function. All available hooks are in [transformer_defaults.py](/SwissArmyTransformer/transformer_defaults.py). 
+Here `attention_fn` is a hook function, replacing the default action by the new function. All available hooks are in [transformer_defaults.py](/sat/transformer_defaults.py). 
 Now we can use `add_mixin` to apply our change to all the transformers, such as BERT, Vit and CogView. See the tutorial for more details. 
 
 ## Tutorials 
 TO BE RELEASED SOON...
 
 # Citation
 Currently we don't have a paper, so you don't need to formally cite us!~ 
 
-If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/SwissArmyTransformer}` to mention us and recommend `SwissArmyTransformer` to others.
+If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/sat}` to mention us and recommend `sat` to others.
 
-The tutorial for contributing SwissArmyTransformer is on the way!
+The tutorial for contributing sat is on the way!
 
 The project is based on (a user of) DeepSpeed, Megatron-LM and Huggingface transformers. Thanks for their awesome work.
```

### Comparing `SwissArmyTransformer-0.2.9/setup.py` & `SwissArmyTransformer-0.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def _requirements():
     return Path("requirements.txt").read_text()
 
 setup(
     name="SwissArmyTransformer",
-    version='0.2.9',
+    version='0.3.1',
     description="A transformer-based framework with finetuning as the first class citizen.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     install_requires=_requirements(),
     entry_points={},
     packages=find_packages(),
     url="https://github.com/THUDM/SwissArmyTransformer",
```

