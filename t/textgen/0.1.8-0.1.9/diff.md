# Comparing `tmp/textgen-0.1.8.tar.gz` & `tmp/textgen-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textgen-0.1.8.tar", last modified: Fri Apr  7 09:20:39 2023, max compression
+gzip compressed data, was "textgen-0.1.9.tar", last modified: Wed Apr 12 09:55:05 2023, max compression
```

## Comparing `textgen-0.1.8.tar` & `textgen-0.1.9.tar`

### file list

```diff
@@ -1,64 +1,68 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-07 09:20:39.889828 textgen-0.1.8/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:06.000000 textgen-0.1.8/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)    26585 2023-04-07 09:20:39.890673 textgen-0.1.8/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    22208 2023-03-26 02:30:43.000000 textgen-0.1.8/README.md
--rw-r--r--   0 xuming     (501) staff       (20)      309 2023-04-07 09:20:39.893100 textgen-0.1.8/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1395 2023-04-07 02:35:13.000000 textgen-0.1.8/setup.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-07 09:20:39.829813 textgen-0.1.8/textgen/
--rw-r--r--   0 xuming     (501) staff       (20)     1288 2023-04-07 02:35:13.000000 textgen-0.1.8/textgen/__init__.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-07 09:20:39.839844 textgen-0.1.8/textgen/augment/
--rw-r--r--   0 xuming     (501) staff       (20)      133 2022-06-30 07:59:18.000000 textgen-0.1.8/textgen/augment/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1493 2022-05-09 11:34:10.000000 textgen-0.1.8/textgen/augment/sentence_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     3384 2022-09-26 07:08:57.000000 textgen-0.1.8/textgen/augment/text_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     2256 2022-07-04 08:00:34.000000 textgen-0.1.8/textgen/augment/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)     1971 2021-08-05 02:59:06.000000 textgen-0.1.8/textgen/augment/translate_api.py
--rw-r--r--   0 xuming     (501) staff       (20)    13027 2022-09-26 07:39:41.000000 textgen-0.1.8/textgen/augment/word_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     1240 2022-05-09 11:34:10.000000 textgen-0.1.8/textgen/augment/word_vocab.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-07 09:20:39.843073 textgen-0.1.8/textgen/chatglm/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-03-26 02:30:43.000000 textgen-0.1.8/textgen/chatglm/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    26069 2023-04-07 08:08:24.000000 textgen-0.1.8/textgen/chatglm/chatglm_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     5884 2023-04-07 06:57:13.000000 textgen-0.1.8/textgen/chatglm/chatglm_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-07 09:20:39.845533 textgen-0.1.8/textgen/config/
--rw-r--r--   0 xuming     (501) staff       (20)      140 2021-08-05 02:59:06.000000 textgen-0.1.8/textgen/config/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1845 2022-06-30 03:18:51.000000 textgen-0.1.8/textgen/config/global_args.py
--rw-r--r--   0 xuming     (501) staff       (20)    12292 2023-04-07 08:08:24.000000 textgen-0.1.8/textgen/config/model_args.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-07 09:20:39.847246 textgen-0.1.8/textgen/custom_models/
--rwxr-xr-x   0 xuming     (501) staff       (20)        0 2021-08-05 02:59:06.000000 textgen-0.1.8/textgen/custom_models/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2022-08-24 03:27:39.000000 textgen-0.1.8/textgen/custom_models/models.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-07 09:20:39.850267 textgen-0.1.8/textgen/data/
--rwxr-xr-x   0 xuming     (501) staff       (20)    48098 2019-08-25 14:57:21.000000 textgen-0.1.8/textgen/data/HowNetPOSWord.txt
--rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 textgen-0.1.8/textgen/data/stopwords.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-07 09:20:39.854199 textgen-0.1.8/textgen/language_generation/
--rwxr-xr-x   0 xuming     (501) staff       (20)      292 2021-08-05 02:59:06.000000 textgen-0.1.8/textgen/language_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    10056 2022-07-05 07:48:33.000000 textgen-0.1.8/textgen/language_generation/language_generation_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     2829 2022-06-14 12:08:00.000000 textgen-0.1.8/textgen/language_generation/language_generation_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-07 09:20:39.862985 textgen-0.1.8/textgen/language_modeling/
--rwxr-xr-x   0 xuming     (501) staff       (20)      407 2022-09-10 06:38:25.000000 textgen-0.1.8/textgen/language_modeling/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    56833 2022-09-09 11:41:34.000000 textgen-0.1.8/textgen/language_modeling/language_modeling_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     8938 2022-06-14 12:08:00.000000 textgen-0.1.8/textgen/language_modeling/language_modeling_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    65595 2022-11-27 05:36:55.000000 textgen-0.1.8/textgen/language_modeling/songnet_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    17103 2022-12-05 07:28:16.000000 textgen-0.1.8/textgen/language_modeling/songnet_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-07 09:20:39.873459 textgen-0.1.8/textgen/seq2seq/
--rwxr-xr-x   0 xuming     (501) staff       (20)      313 2022-08-07 03:00:11.000000 textgen-0.1.8/textgen/seq2seq/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    73298 2022-09-09 11:41:34.000000 textgen-0.1.8/textgen/seq2seq/bart_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    18559 2022-06-19 09:29:30.000000 textgen-0.1.8/textgen/seq2seq/bart_seq2seq_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    23456 2022-08-25 03:06:56.000000 textgen-0.1.8/textgen/seq2seq/conv_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     4345 2022-05-10 10:48:02.000000 textgen-0.1.8/textgen/seq2seq/data_reader.py
--rw-r--r--   0 xuming     (501) staff       (20)    19319 2022-08-25 03:06:56.000000 textgen-0.1.8/textgen/seq2seq/seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    10741 2022-06-15 12:49:21.000000 textgen-0.1.8/textgen/seq2seq/seq2seq_trainer.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-07 09:20:39.881625 textgen-0.1.8/textgen/t5/
--rwxr-xr-x   0 xuming     (501) staff       (20)      272 2022-08-23 06:18:39.000000 textgen-0.1.8/textgen/t5/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    50493 2022-11-16 12:03:51.000000 textgen-0.1.8/textgen/t5/copyt5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6917 2022-11-16 13:02:34.000000 textgen-0.1.8/textgen/t5/copyt5_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    50541 2023-02-16 08:10:32.000000 textgen-0.1.8/textgen/t5/t5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     7146 2022-11-17 02:54:45.000000 textgen-0.1.8/textgen/t5/t5_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-07 09:20:39.888068 textgen-0.1.8/textgen/unsup_generation/
--rw-r--r--   0 xuming     (501) staff       (20)      246 2022-09-06 02:24:58.000000 textgen-0.1.8/textgen/unsup_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3456 2022-09-26 07:01:36.000000 textgen-0.1.8/textgen/unsup_generation/tgls_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    27678 2022-09-06 02:29:56.000000 textgen-0.1.8/textgen/unsup_generation/tgls_util.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-07 09:20:39.833383 textgen-0.1.8/textgen.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    26585 2023-04-07 09:20:39.000000 textgen-0.1.8/textgen.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)     1608 2023-04-07 09:20:39.000000 textgen-0.1.8/textgen.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-07 09:20:39.000000 textgen-0.1.8/textgen.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)      145 2023-04-07 09:20:39.000000 textgen-0.1.8/textgen.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)        8 2023-04-07 09:20:39.000000 textgen-0.1.8/textgen.egg-info/top_level.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.809881 textgen-0.1.9/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:06.000000 textgen-0.1.9/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)    30674 2023-04-12 09:55:05.810717 textgen-0.1.9/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    25881 2023-04-11 07:50:53.000000 textgen-0.1.9/README.md
+-rw-r--r--   0 xuming     (501) staff       (20)      309 2023-04-12 09:55:05.812715 textgen-0.1.9/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1395 2023-04-12 09:49:33.000000 textgen-0.1.9/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.737362 textgen-0.1.9/textgen/
+-rw-r--r--   0 xuming     (501) staff       (20)     1386 2023-04-12 09:49:33.000000 textgen-0.1.9/textgen/__init__.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.750356 textgen-0.1.9/textgen/augment/
+-rw-r--r--   0 xuming     (501) staff       (20)      133 2022-06-30 07:59:18.000000 textgen-0.1.9/textgen/augment/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1493 2022-05-09 11:34:10.000000 textgen-0.1.9/textgen/augment/sentence_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-04-12 09:49:33.000000 textgen-0.1.9/textgen/augment/text_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2256 2022-07-04 08:00:34.000000 textgen-0.1.9/textgen/augment/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1971 2021-08-05 02:59:06.000000 textgen-0.1.9/textgen/augment/translate_api.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13027 2022-09-26 07:39:41.000000 textgen-0.1.9/textgen/augment/word_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1240 2022-05-09 11:34:10.000000 textgen-0.1.9/textgen/augment/word_vocab.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.754473 textgen-0.1.9/textgen/chatglm/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-03-26 02:30:43.000000 textgen-0.1.9/textgen/chatglm/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    31686 2023-04-11 15:12:32.000000 textgen-0.1.9/textgen/chatglm/chatglm_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6228 2023-04-12 09:49:33.000000 textgen-0.1.9/textgen/chatglm/chatglm_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.756991 textgen-0.1.9/textgen/config/
+-rw-r--r--   0 xuming     (501) staff       (20)      140 2021-08-05 02:59:06.000000 textgen-0.1.9/textgen/config/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1845 2022-06-30 03:18:51.000000 textgen-0.1.9/textgen/config/global_args.py
+-rw-r--r--   0 xuming     (501) staff       (20)    14188 2023-04-12 06:51:22.000000 textgen-0.1.9/textgen/config/model_args.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.759489 textgen-0.1.9/textgen/custom_models/
+-rwxr-xr-x   0 xuming     (501) staff       (20)        0 2021-08-05 02:59:06.000000 textgen-0.1.9/textgen/custom_models/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2022-08-24 03:27:39.000000 textgen-0.1.9/textgen/custom_models/models.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.762844 textgen-0.1.9/textgen/data/
+-rwxr-xr-x   0 xuming     (501) staff       (20)    48098 2019-08-25 14:57:21.000000 textgen-0.1.9/textgen/data/HowNetPOSWord.txt
+-rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 textgen-0.1.9/textgen/data/stopwords.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.767938 textgen-0.1.9/textgen/language_generation/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      292 2021-08-05 02:59:06.000000 textgen-0.1.9/textgen/language_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10056 2022-07-05 07:48:33.000000 textgen-0.1.9/textgen/language_generation/language_generation_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2829 2022-06-14 12:08:00.000000 textgen-0.1.9/textgen/language_generation/language_generation_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.774012 textgen-0.1.9/textgen/language_modeling/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      407 2022-09-10 06:38:25.000000 textgen-0.1.9/textgen/language_modeling/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    56833 2022-09-09 11:41:34.000000 textgen-0.1.9/textgen/language_modeling/language_modeling_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8938 2022-06-14 12:08:00.000000 textgen-0.1.9/textgen/language_modeling/language_modeling_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    65595 2022-11-27 05:36:55.000000 textgen-0.1.9/textgen/language_modeling/songnet_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17103 2022-12-05 07:28:16.000000 textgen-0.1.9/textgen/language_modeling/songnet_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.777513 textgen-0.1.9/textgen/llama/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-10 03:44:03.000000 textgen-0.1.9/textgen/llama/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    23061 2023-04-11 14:20:32.000000 textgen-0.1.9/textgen/llama/llama_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4853 2023-04-12 05:35:51.000000 textgen-0.1.9/textgen/llama/llama_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.788862 textgen-0.1.9/textgen/seq2seq/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      313 2022-08-07 03:00:11.000000 textgen-0.1.9/textgen/seq2seq/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    73298 2022-09-09 11:41:34.000000 textgen-0.1.9/textgen/seq2seq/bart_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    18559 2022-06-19 09:29:30.000000 textgen-0.1.9/textgen/seq2seq/bart_seq2seq_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    23456 2022-08-25 03:06:56.000000 textgen-0.1.9/textgen/seq2seq/conv_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4345 2022-05-10 10:48:02.000000 textgen-0.1.9/textgen/seq2seq/data_reader.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19319 2022-08-25 03:06:56.000000 textgen-0.1.9/textgen/seq2seq/seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10741 2022-06-15 12:49:21.000000 textgen-0.1.9/textgen/seq2seq/seq2seq_trainer.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.798950 textgen-0.1.9/textgen/t5/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      272 2022-08-23 06:18:39.000000 textgen-0.1.9/textgen/t5/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50493 2022-11-16 12:03:51.000000 textgen-0.1.9/textgen/t5/copyt5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6917 2022-11-16 13:02:34.000000 textgen-0.1.9/textgen/t5/copyt5_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50541 2023-02-16 08:10:32.000000 textgen-0.1.9/textgen/t5/t5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7146 2022-11-17 02:54:45.000000 textgen-0.1.9/textgen/t5/t5_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.805866 textgen-0.1.9/textgen/unsup_generation/
+-rw-r--r--   0 xuming     (501) staff       (20)      246 2022-09-06 02:24:58.000000 textgen-0.1.9/textgen/unsup_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3456 2022-09-26 07:01:36.000000 textgen-0.1.9/textgen/unsup_generation/tgls_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    27678 2022-09-06 02:29:56.000000 textgen-0.1.9/textgen/unsup_generation/tgls_util.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-12 09:55:05.741739 textgen-0.1.9/textgen.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    30674 2023-04-12 09:55:05.000000 textgen-0.1.9/textgen.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)     1692 2023-04-12 09:55:05.000000 textgen-0.1.9/textgen.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-12 09:55:05.000000 textgen-0.1.9/textgen.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      145 2023-04-12 09:55:05.000000 textgen-0.1.9/textgen.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        8 2023-04-12 09:55:05.000000 textgen-0.1.9/textgen.egg-info/top_level.txt
```

### Comparing `textgen-0.1.8/LICENSE` & `textgen-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/PKG-INFO` & `textgen-0.1.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.1.8
+Version: 0.1.9
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/textgen)
         [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/project/textgen)
@@ -15,65 +15,71 @@
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
         # TextGen
         
         🌈 Implementation of Text Generation models.
         
-        **textgen**实现了多种文本生成模型，包括：UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
+        **textgen**实现了多种文本生成模型，包括：LLAMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
         
         **Guide**
         
         - [Feature](#Feature)
         - [Install](#install)
         - [Usage](#usage)
         - [Contact](#Contact)
         - [Reference](#reference)
         
         # Feature
+        
         ## 文本生成
         
         1. seq2seq: Seq2Seq、ConvSeq2Seq、BART
-        2. language_modeling: GPT2、SongNet
+        2. language_modeling: GPT2、SongNet、ChatGLM、LLAMA
         3. t5: T5、CopyT5
-        4. question_answering: BERT、XLNet
-        5. chatglm: ChatGLM
         
         ## 文本扩增
+        
         ### 词粒度扩增
+        
         1. UDA，非核心词替换
         2. EDA，简单数据增强技术：相似词、同义词替换，随机词插入、删除、替换
         
         ### 句粒度扩增
+        
         1. 回译（BT, Back Translate）：中文-英文-中文
         2. GPT2模型续写：短文本->长文本
         3. BART摘要模型：长文本->短文本
         4. TGLS：无监督相似文本生成模型
         
         ## 功能列表
+        - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
+        - [LLAMA](textgen/llama)：本项目基于PyTorch实现了LLAMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
         - [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
         - [BT(回译)](textgen/augment/sentence_level_augment.py)：本项目基于百度翻译API实现了回译功能，先把中文句子翻译为英文，再把英文翻译为新的中文
         - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
         - [T5](textgen/t5)：本项目基于PyTorch实现了T5和CopyT5模型训练和预测，可以用于文本翻译、对话生成、对联生成、文案撰写等文本生成任务
         - [GPT2](textgen/language_modeling)：本项目基于PyTorch实现了GTP2模型训练和预测，可以用于文章生成、对联生成等文本生成任务
         - [SongNet](textgen/language_modeling/songnet_model.py)：本项目基于PyTorch实现了SongNet模型训练和预测，可以用于规范格式的诗词、歌词等文本生成任务
         - [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
         
         
         ## Release Models
+        
         release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
         
-        |Model|Arch|Intro|Training|Inference|
+        |Model|Arch|Introduce|Training|Inference| 
         |:-- |:--- |:--- |:--- |:--- |
         |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)|T5|中文NLP多任务Prompt模型|[prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5_prompt_demo.py)|
         |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)|T5|fine-tuned中文对联后的模型|[对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5_couplet_demo.py)|
         |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)|SongNet|SongNet预训练模型|-|-|
         |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)|SongNet|fine-tuned宋词后的模型|[training script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet_songci_demo.py)|
         |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)|SongNet|fine-tuned对联后的模型|[training script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet_couplet_demo.py)|
-        
+        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)|ChatGLM-6B|在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重|[training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)|
+        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重|[training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|
         
         # Demo
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/chinese-couplet-generate
         
         ![](docs/hf.png)
         
@@ -84,33 +90,76 @@
         ```
         
         model trained by [examples/T5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/T5/T5_Finetune_Chinese_Couplet.ipynb)
         
         # Install
         
         ```shell
-        pip install torch # conda install pytorch
         pip install -U textgen
         ```
         
         or
         
         ```shell
         pip install torch # conda install pytorch
         git clone https://github.com/shibing624/textgen.git
         cd textgen
-        python3 setup.py install
+        python setup.py install
         ```
         
         # Usage
         
+        ## ChatGLM-6B LoRA 模型
+        
+        ### 使用ChatGLM-6B LoRA微调后的模型
+        example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
+        
+        ```python
+        import sys
+        
+        sys.path.append('../..')
+        from textgen import ChatGlmModel
+        
+        model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", lora_name="shibing624/chatglm-6b-csc-zh-lora")
+        r = model.predict(["对下面中文拼写纠错：\n少先队员因该为老人让坐。\n答："])
+        print(r)  # ['少先队员应该为老人让座。\n错误字：因，坐']
+        ```
+        
+        ### 训练ChatGLM-6B LoRA模型
+        
+        支持自定义数据集，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)。
+        
+        example: [examples/chatglm/training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_demo.py)
+        
+        ## LLAMA LoRA 模型
+        
+        ### 使用LLAMA LoRA微调后的模型
+        
+        example: [examples/llama/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/predict_demo.py)
+        
+        ```python
+        import sys
+        
+        sys.path.append('../..')
+        from textgen import LlamaModel
+        
+        model = LlamaModel("llama", "huggyllama/llama-7b", lora_name="qychen/luotuo-lora-7b-0.1")
+        r = model.predict(["失眠了怎么办？"])
+        print(r)
+        ```
+        
+        ### 训练LLAMA LoRA模型
+        
+        example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)
+        
         ## ConvSeq2Seq 模型
+        
         训练并预测ConvSeq2Seq模型：
         
-        example: [examples/seq2sesq/training_convseq2seq_model_demo.py](examples/seq2seq/training_convseq2seq_model_demo.py)
+        example: [examples/seq2sesq/training_convseq2seq_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_convseq2seq_model_demo.py)
         
         ```python
         import argparse
         from loguru import logger
         import sys
         
         sys.path.append('../..')
@@ -152,27 +201,26 @@
         
         ```bash
         inputs: ["什么是ai", "你是什么类型的计算机", "你知道热力学吗"]
         outputs: ['人工智能是工程和科学的分支,致力于构建思维的机器。', '我的程序运行在python,所以我在任何运脑上工作！', '我不能错热是一个疯狂的人工智能"200年。']
         ```
         
         ## BART 模型
-        训练并预测BART模型：
         
-        example: [examples/seq2sesq/training_bartseq2seq_zh_demo.py](examples/seq2seq/training_bartseq2seq_zh_demo.py)
+        训练并预测BART模型：
         
+        example: [examples/seq2sesq/training_bartseq2seq_zh_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_bartseq2seq_zh_demo.py)
         
         output:
         
         ```shell
         inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
         outputs: ['人工智能是工程和科学的分支,致力于构', '我的程序运行在python,所以我在任何电脑上', '什么是热力学吗？']
         ```
         
-        
         ## T5 模型
         
         example: [examples/T5/training_zh_t5_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/T5/training_zh_t5_model_demo.py)
         
         ```python
         import argparse
         from loguru import logger
@@ -260,22 +308,20 @@
         
         
         if __name__ == '__main__':
             main()
         ```
         
         output:
+        
         ```shell
         inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
         outputs: ['人工智能有两个广义的定义,任何拟人的机械,如在卡雷尔capeks', '我的程序运行在Python,所以我在任何电脑上工作!', '什么是热力学']
         ```
         
-        
-        
-        
         ## GPT2 模型
         
         ### 中文GPT2 - 文章生成
         
         使用中文数据集（段落格式，`\n`间隔），训练GPT2模型，可以用于诗歌生成、文章生成等任务。
         
         example: [examples/language_generation/training_zh_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_gpt2_demo.py)
@@ -283,14 +329,15 @@
         ### 中文GPT2 - 对联生成
         
         使用中文对联数据集（tsv格式，`\t`间隔），自定义数据集读取Dataset，训练GPT2模型，可以用于对联生成、对话生成等任务。
         
         example: [examples/language_generation/training_couplet_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_couplet_gpt2_demo.py)
         
         #### GPT2 vs T5：
+        
         1. 都是从Transformer改进来的，T5同时有编码器和解码器，GPT2只有解码器
         2. T5的模型优势是处理给定输入，产出对应输出的任务，如翻译、对话、问答等
         3. GPT2的模型优势是自由创作，如写一篇短文
         4. T5的对联生成效果好于GPT2、GPT2的诗词生成效果好于T5
         
         - [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)
         - [古诗生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%8F%A4%E8%AF%97%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)
@@ -298,16 +345,14 @@
         ## SongNet 模型
         
         格式控制的文本生成模型，paper见[SongNet: Rigid Formats Controlled Text Generation](https://arxiv.org/abs/2004.08022)，
         适用于强韵律格式要求的诗歌、对联、歌词生成等任务。
         
         example: [examples/language_generation/training_zh_songnet_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)
         
-        
-        
         ## Keyword Text Augmentation(EDA/UDA)
         
         example: [examples/text_augmentation_demo.py](examples/text_augmentation_demo.py)
         
         ```python
         import sys
         
@@ -414,24 +459,31 @@
         希望好用，面膜用过了很好用，皮肤水嫩光滑白皙，补水不错，价格也合适。
         就是精华液太少了，保湿效果不错。
         面膜的补水效果非常好，保湿效果确实很赞，这个面膜相对于胶原蛋白和美白的那两款的面膜纸要厚一些，看着价格合适。
         ```
         
         前10句是真实用户评论，后10句是生成的。
         
+        # Dataset
+        
+        1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
+        2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
+        3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
+        4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+        5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
+        
         # Contact
         
         - Issue(建议)
           ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我： 加我*微信号：xuming624, 备注：姓名-公司名-NLP* 进NLP交流群。
         
         <img src="docs/wechat.jpeg" width="200" />
         
-        
         # Citation
         
         如果你在研究中使用了textgen，请按如下格式引用：
         
         ```latex
         @misc{textgen,
           title={textgen: Text Generation Tool},
@@ -461,15 +513,15 @@
         - [minimaxir/gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
         - [asyml/texar](https://github.com/asyml/texar)
         - [yangjianxin1/GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat)
         - [williamSYSU/TextGAN-PyTorch](https://github.com/williamSYSU/TextGAN-PyTorch)
         - [RUCAIBox/TextBox](https://github.com/RUCAIBox/TextBox)
         - [Tiiiger/bert_score]()
         - [1YCxZ/Fake-review-generation](https://github.com/1YCxZ/Fake-review-generation)
-        
+        - [tloen/alpaca-lora](https://github.com/tloen/alpaca-lora/blob/main/finetune.py)
 Keywords: textgen,text-generation,Text Generation Tool,ernie-gen,chinese text generation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Linguistic
```

### Comparing `textgen-0.1.8/README.md` & `textgen-0.1.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -7,65 +7,71 @@
 [![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
 [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
 
 # TextGen
 
 🌈 Implementation of Text Generation models.
 
-**textgen**实现了多种文本生成模型，包括：UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
+**textgen**实现了多种文本生成模型，包括：LLAMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
 
 **Guide**
 
 - [Feature](#Feature)
 - [Install](#install)
 - [Usage](#usage)
 - [Contact](#Contact)
 - [Reference](#reference)
 
 # Feature
+
 ## 文本生成
 
 1. seq2seq: Seq2Seq、ConvSeq2Seq、BART
-2. language_modeling: GPT2、SongNet
+2. language_modeling: GPT2、SongNet、ChatGLM、LLAMA
 3. t5: T5、CopyT5
-4. question_answering: BERT、XLNet
-5. chatglm: ChatGLM
 
 ## 文本扩增
+
 ### 词粒度扩增
+
 1. UDA，非核心词替换
 2. EDA，简单数据增强技术：相似词、同义词替换，随机词插入、删除、替换
 
 ### 句粒度扩增
+
 1. 回译（BT, Back Translate）：中文-英文-中文
 2. GPT2模型续写：短文本->长文本
 3. BART摘要模型：长文本->短文本
 4. TGLS：无监督相似文本生成模型
 
 ## 功能列表
+- [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
+- [LLAMA](textgen/llama)：本项目基于PyTorch实现了LLAMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
 - [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
 - [BT(回译)](textgen/augment/sentence_level_augment.py)：本项目基于百度翻译API实现了回译功能，先把中文句子翻译为英文，再把英文翻译为新的中文
 - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
 - [T5](textgen/t5)：本项目基于PyTorch实现了T5和CopyT5模型训练和预测，可以用于文本翻译、对话生成、对联生成、文案撰写等文本生成任务
 - [GPT2](textgen/language_modeling)：本项目基于PyTorch实现了GTP2模型训练和预测，可以用于文章生成、对联生成等文本生成任务
 - [SongNet](textgen/language_modeling/songnet_model.py)：本项目基于PyTorch实现了SongNet模型训练和预测，可以用于规范格式的诗词、歌词等文本生成任务
 - [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
 
 
 ## Release Models
+
 release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
 
-|Model|Arch|Intro|Training|Inference|
+|Model|Arch|Introduce|Training|Inference| 
 |:-- |:--- |:--- |:--- |:--- |
 |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)|T5|中文NLP多任务Prompt模型|[prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5_prompt_demo.py)|
 |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)|T5|fine-tuned中文对联后的模型|[对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5_couplet_demo.py)|
 |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)|SongNet|SongNet预训练模型|-|-|
 |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)|SongNet|fine-tuned宋词后的模型|[training script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet_songci_demo.py)|
 |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)|SongNet|fine-tuned对联后的模型|[training script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet_couplet_demo.py)|
-
+|[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)|ChatGLM-6B|在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重|[training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)|
+|[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重|[training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|
 
 # Demo
 
 HuggingFace Demo: https://huggingface.co/spaces/shibing624/chinese-couplet-generate
 
 ![](docs/hf.png)
 
@@ -76,33 +82,76 @@
 ```
 
 model trained by [examples/T5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/T5/T5_Finetune_Chinese_Couplet.ipynb)
 
 # Install
 
 ```shell
-pip install torch # conda install pytorch
 pip install -U textgen
 ```
 
 or
 
 ```shell
 pip install torch # conda install pytorch
 git clone https://github.com/shibing624/textgen.git
 cd textgen
-python3 setup.py install
+python setup.py install
 ```
 
 # Usage
 
+## ChatGLM-6B LoRA 模型
+
+### 使用ChatGLM-6B LoRA微调后的模型
+example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
+
+```python
+import sys
+
+sys.path.append('../..')
+from textgen import ChatGlmModel
+
+model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", lora_name="shibing624/chatglm-6b-csc-zh-lora")
+r = model.predict(["对下面中文拼写纠错：\n少先队员因该为老人让坐。\n答："])
+print(r)  # ['少先队员应该为老人让座。\n错误字：因，坐']
+```
+
+### 训练ChatGLM-6B LoRA模型
+
+支持自定义数据集，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)。
+
+example: [examples/chatglm/training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_demo.py)
+
+## LLAMA LoRA 模型
+
+### 使用LLAMA LoRA微调后的模型
+
+example: [examples/llama/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/predict_demo.py)
+
+```python
+import sys
+
+sys.path.append('../..')
+from textgen import LlamaModel
+
+model = LlamaModel("llama", "huggyllama/llama-7b", lora_name="qychen/luotuo-lora-7b-0.1")
+r = model.predict(["失眠了怎么办？"])
+print(r)
+```
+
+### 训练LLAMA LoRA模型
+
+example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)
+
 ## ConvSeq2Seq 模型
+
 训练并预测ConvSeq2Seq模型：
 
-example: [examples/seq2sesq/training_convseq2seq_model_demo.py](examples/seq2seq/training_convseq2seq_model_demo.py)
+example: [examples/seq2sesq/training_convseq2seq_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_convseq2seq_model_demo.py)
 
 ```python
 import argparse
 from loguru import logger
 import sys
 
 sys.path.append('../..')
@@ -144,27 +193,26 @@
 
 ```bash
 inputs: ["什么是ai", "你是什么类型的计算机", "你知道热力学吗"]
 outputs: ['人工智能是工程和科学的分支,致力于构建思维的机器。', '我的程序运行在python,所以我在任何运脑上工作！', '我不能错热是一个疯狂的人工智能"200年。']
 ```
 
 ## BART 模型
-训练并预测BART模型：
 
-example: [examples/seq2sesq/training_bartseq2seq_zh_demo.py](examples/seq2seq/training_bartseq2seq_zh_demo.py)
+训练并预测BART模型：
 
+example: [examples/seq2sesq/training_bartseq2seq_zh_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_bartseq2seq_zh_demo.py)
 
 output:
 
 ```shell
 inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
 outputs: ['人工智能是工程和科学的分支,致力于构', '我的程序运行在python,所以我在任何电脑上', '什么是热力学吗？']
 ```
 
-
 ## T5 模型
 
 example: [examples/T5/training_zh_t5_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/T5/training_zh_t5_model_demo.py)
 
 ```python
 import argparse
 from loguru import logger
@@ -252,22 +300,20 @@
 
 
 if __name__ == '__main__':
     main()
 ```
 
 output:
+
 ```shell
 inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
 outputs: ['人工智能有两个广义的定义,任何拟人的机械,如在卡雷尔capeks', '我的程序运行在Python,所以我在任何电脑上工作!', '什么是热力学']
 ```
 
-
-
-
 ## GPT2 模型
 
 ### 中文GPT2 - 文章生成
 
 使用中文数据集（段落格式，`\n`间隔），训练GPT2模型，可以用于诗歌生成、文章生成等任务。
 
 example: [examples/language_generation/training_zh_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_gpt2_demo.py)
@@ -275,14 +321,15 @@
 ### 中文GPT2 - 对联生成
 
 使用中文对联数据集（tsv格式，`\t`间隔），自定义数据集读取Dataset，训练GPT2模型，可以用于对联生成、对话生成等任务。
 
 example: [examples/language_generation/training_couplet_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_couplet_gpt2_demo.py)
 
 #### GPT2 vs T5：
+
 1. 都是从Transformer改进来的，T5同时有编码器和解码器，GPT2只有解码器
 2. T5的模型优势是处理给定输入，产出对应输出的任务，如翻译、对话、问答等
 3. GPT2的模型优势是自由创作，如写一篇短文
 4. T5的对联生成效果好于GPT2、GPT2的诗词生成效果好于T5
 
 - [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)
 - [古诗生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%8F%A4%E8%AF%97%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)
@@ -290,16 +337,14 @@
 ## SongNet 模型
 
 格式控制的文本生成模型，paper见[SongNet: Rigid Formats Controlled Text Generation](https://arxiv.org/abs/2004.08022)，
 适用于强韵律格式要求的诗歌、对联、歌词生成等任务。
 
 example: [examples/language_generation/training_zh_songnet_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)
 
-
-
 ## Keyword Text Augmentation(EDA/UDA)
 
 example: [examples/text_augmentation_demo.py](examples/text_augmentation_demo.py)
 
 ```python
 import sys
 
@@ -406,24 +451,31 @@
 希望好用，面膜用过了很好用，皮肤水嫩光滑白皙，补水不错，价格也合适。
 就是精华液太少了，保湿效果不错。
 面膜的补水效果非常好，保湿效果确实很赞，这个面膜相对于胶原蛋白和美白的那两款的面膜纸要厚一些，看着价格合适。
 ```
 
 前10句是真实用户评论，后10句是生成的。
 
+# Dataset
+
+1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
+2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
+3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
+4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
+
 # Contact
 
 - Issue(建议)
   ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
 - 邮件我：xuming: xuming624@qq.com
 - 微信我： 加我*微信号：xuming624, 备注：姓名-公司名-NLP* 进NLP交流群。
 
 <img src="docs/wechat.jpeg" width="200" />
 
-
 # Citation
 
 如果你在研究中使用了textgen，请按如下格式引用：
 
 ```latex
 @misc{textgen,
   title={textgen: Text Generation Tool},
@@ -453,7 +505,8 @@
 - [minimaxir/gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
 - [asyml/texar](https://github.com/asyml/texar)
 - [yangjianxin1/GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat)
 - [williamSYSU/TextGAN-PyTorch](https://github.com/williamSYSU/TextGAN-PyTorch)
 - [RUCAIBox/TextBox](https://github.com/RUCAIBox/TextBox)
 - [Tiiiger/bert_score]()
 - [1YCxZ/Fake-review-generation](https://github.com/1YCxZ/Fake-review-generation)
+- [tloen/alpaca-lora](https://github.com/tloen/alpaca-lora/blob/main/finetune.py)
```

### Comparing `textgen-0.1.8/setup.py` & `textgen-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='textgen',
-    version='0.1.8',
+    version='0.1.9',
     description='Text Generation Model',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='XuMing',
     author_email='xuming624@qq.com',
     url='https://github.com/shibing624/textgen',
     license="Apache 2.0",
```

### Comparing `textgen-0.1.8/textgen/__init__.py` & `textgen-0.1.9/textgen/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 from textgen.augment.text_augment import TextAugment
 
 from textgen.config.model_args import LanguageGenerationArgs
 from textgen.language_generation.language_generation_model import LanguageGenerationModel
 
 from textgen.config.model_args import LanguageModelingArgs
@@ -30,7 +30,10 @@
 from textgen.t5.copyt5_model import CopyT5Model
 from textgen.t5.copyt5_utils import ZHTokenizer
 
 from textgen.unsup_generation.tgls_model import TglsModel
 
 from textgen.chatglm.chatglm_model import ChatGlmModel
 from textgen.config.model_args import ChatGlmArgs
+
+from textgen.llama.llama_model import LlamaModel
+from textgen.config.model_args import LlamaArgs
```

### Comparing `textgen-0.1.8/textgen/augment/sentence_level_augment.py` & `textgen-0.1.9/textgen/augment/sentence_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/augment/text_augment.py` & `textgen-0.1.9/textgen/augment/text_augment.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 from loguru import logger
 from jieba import analyse
 import jieba
-from text2vec import Word2Vec
 
 from textgen.augment.sentence_level_augment import back_translation
 from textgen.augment.word_level_augment import (
     get_data_idf,
     RandomReplace,
     DeleteReplace,
     InsertReplace,
@@ -28,14 +27,19 @@
 
     def __init__(self, sentence_list=None, tokenizer=None):
         """
         Init
         :param sentence_list: list, docs
         """
         self.tokenizer = tokenizer if tokenizer is not None else Tokenizer()
+        try:
+            from text2vec import Word2Vec
+        except ImportError:
+            logger.warning("text2vec not installed, please install text2vec with command: `pip install text2vec`")
+            raise ImportError
         vec = Word2Vec()
         self.w2v = vec.w2v
         if sentence_list is None:
             # Use jieba IDF and TF dict
             idf = analyse.TFIDF()
             word_idf = idf.idf_freq
             dt = jieba.Tokenizer()
```

### Comparing `textgen-0.1.8/textgen/augment/tokenizer.py` & `textgen-0.1.9/textgen/augment/tokenizer.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/augment/translate_api.py` & `textgen-0.1.9/textgen/augment/translate_api.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/augment/word_level_augment.py` & `textgen-0.1.9/textgen/augment/word_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/augment/word_vocab.py` & `textgen-0.1.9/textgen/augment/word_vocab.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/chatglm/chatglm_model.py` & `textgen-0.1.9/textgen/llama/llama_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,88 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description:
+
+modified from https://github.com/tloen/alpaca-lora/blob/main/finetune.py
 """
 import os
-import sys
-import re
 import random
-from typing import Tuple, List
+import sys
+from typing import List, Tuple
 
 import numpy as np
 import torch
-import torch.nn as nn
 from loguru import logger
 from peft import (
     get_peft_model,
     LoraConfig,
     TaskType,
     PeftModel,
     get_peft_model_state_dict,
     prepare_model_for_int8_training,
     set_peft_model_state_dict,
 )
 from tqdm.auto import tqdm
-from transformers import Trainer, TrainingArguments, AutoTokenizer, AutoModel, AutoConfig
+from transformers import GenerationConfig, DataCollatorForSeq2Seq
+from transformers import LlamaForCausalLM, LlamaTokenizer
+from transformers import Trainer, TrainingArguments, AutoConfig
 from transformers.trainer import TRAINING_ARGS_NAME
-from textgen.config.model_args import ChatGlmArgs
-from textgen.chatglm.chatglm_utils import load_hf_dataset, ChatGlmDataset
+
+from textgen.config.model_args import LlamaArgs
+from textgen.llama.llama_utils import load_hf_dataset, LlamaDataset
 
 try:
     import wandb
 
     wandb_available = True
 except ImportError:
     wandb_available = False
 
 has_cuda = torch.cuda.is_available()
 os.environ["TOKENIZERS_PARALLELISM"] = "FALSE"
 os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
 
 MODEL_CLASSES = {
-    "chatglm": (AutoConfig, AutoModel, AutoTokenizer),
+    "llama": (AutoConfig, LlamaForCausalLM, LlamaTokenizer),
 }
 
 
-class ChatGlmModel:
+class LlamaModel:
     def __init__(
             self,
             model_type,
             model_name,
             lora_name=None,
             args=None,
             use_cuda=has_cuda,
             cuda_device=-1,
             **kwargs,
     ):
 
         """
-        Initializes a ChatGLMModel model.
+        Initializes a LlamaModel model.
 
         Args:
-            model_type: The type of model (chatglm)
+            model_type: The type of model (llama)
             model_name: The exact architecture and trained weights to use. This may be a Hugging Face Transformers compatible pre-trained model, a community model, or the path to a directory containing model files.
             lora_name (optional): Lora name
             args (optional): Default args will be used if this parameter is not provided. If provided, it should be a dict containing the args that should be changed in the default args.
             use_cuda (optional): Use GPU if available. Setting to False will force model to use CPU only.
             cuda_device (optional): Specific GPU that should be used. Will use the first available GPU by default.
             **kwargs (optional): For providing proxies, force_download, resume_download, cache_dir and other options specific to the 'from_pretrained' implementation where this will be supplied.
         """  # noqa: ignore flake8"
         model_type = model_type.lower()
         self.args = self._load_model_args(model_name)
 
         if isinstance(args, dict):
             self.args.update_from_dict(args)
-        elif isinstance(args, ChatGlmArgs):
+        elif isinstance(args, LlamaArgs):
             self.args = args
 
-        self.is_sweeping = False
         if self.args.manual_seed:
             random.seed(self.args.manual_seed)
             np.random.seed(self.args.manual_seed)
             torch.manual_seed(self.args.manual_seed)
             if self.args.n_gpu > 0:
                 torch.cuda.manual_seed_all(self.args.manual_seed)
 
@@ -101,66 +103,53 @@
         if not use_cuda:
             self.args.fp16 = False
             self.args.int8 = False
 
         self.results = {}
         config_class, model_class, tokenizer_class = MODEL_CLASSES[model_type]
         if model_name is None:
-            model_name = "THUDM/chatglm-6b"
-        config = AutoConfig.from_pretrained(model_name, trust_remote_code=True, **kwargs)
-        if use_cuda and torch.cuda.is_available():
-            self.model = model_class.from_pretrained(
-                model_name, config=config, trust_remote_code=True, load_in_8bit=self.args.int8)
-            if self.args.quantization_bit:
-                logger.debug(f"Quantized to {self.args.quantization_bit} bit")
-                self.model = self.model.quantize(self.args.quantization_bit)
-            if self.args.fp16:
-                self.model = self.model.half().cuda()
-        else:
-            self.model = model_class.from_pretrained(
-                model_name, config=config, trust_remote_code=True).float()
+            model_name = self.args.model_name_or_path
+        config = AutoConfig.from_pretrained(model_name, **kwargs)
+        device_map = "auto"
+        world_size = int(os.environ.get("WORLD_SIZE", 1))
+        self.ddp = world_size != 1
+        if self.ddp:
+            device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
+
+        self.model = model_class.from_pretrained(
+            model_name,
+            config=config,
+            load_in_8bit=self.args.int8,
+            torch_dtype=torch.float16 if self.args.fp16 else torch.float32,
+            device_map=device_map,
+        )
 
         self.tokenizer_class = tokenizer_class
         if self.args.tokenizer_name:
-            self.tokenizer = tokenizer_class.from_pretrained(self.args.tokenizer_name, trust_remote_code=True)
+            self.tokenizer = tokenizer_class.from_pretrained(self.args.tokenizer_name)
         else:
-            self.tokenizer = tokenizer_class.from_pretrained(model_name, trust_remote_code=True)
+            self.tokenizer = tokenizer_class.from_pretrained(model_name)
             self.args.tokenizer_name = self.args.model_name
 
+        self.tokenizer.pad_token_id = (
+            0  # unk. we want this to be different from the eos token
+        )
+        self.model.config.pad_token_id = 0  # unk
+        self.model.config.bos_token_id = 1
+        self.model.config.eos_token_id = 2
+        self.tokenizer.padding_side = "left"  # Allow batched inference
         self.args.model_type = model_type
         if model_name is None:
-            self.args.model_name = "ChatGLM_from_scratch"
+            self.args.model_name = "Llama_from_scratch"
         else:
             self.args.model_name = model_name
 
         self.lora_name = lora_name
         self.lora_loaded = False
 
-    def data_collator(self, batch):
-        len_ids = [len(example) for example in batch]
-        longest = max(len_ids)
-        input_ids = []
-        labels_list = []
-        for ids_l, example in sorted(zip(len_ids, batch), key=lambda x: -x[0]):
-            ids = list(example)
-            seq_len = ids.index(self.tokenizer.bos_token_id) + 1  # is equal to `seq_len = seq.index(150004) + 1`
-            label_pad_token_id = -100
-            labels = (
-                    [label_pad_token_id] * (seq_len - 1)
-                    + ids[(seq_len - 1):]
-                    + [label_pad_token_id] * (longest - ids_l)
-            )
-            ids = ids + [self.tokenizer.pad_token_id] * (longest - ids_l)
-            _ids = torch.LongTensor(ids)
-            labels_list.append(torch.LongTensor(labels))
-            input_ids.append(_ids)
-        input_ids = torch.stack(input_ids)
-        labels = torch.stack(labels_list)
-        return {"input_ids": input_ids, "labels": labels}
-
     def train_model(
             self,
             train_data,
             output_dir=None,
             args=None,
             eval_data=None,
             verbose=True,
@@ -171,17 +160,17 @@
 
         Args:
             train_data: Pandas DataFrame containing the 3 columns - `instruction`, `input`, `output`.
                         - `instruction`: The instruction text. (E.g. `"correct the following:"`)
                         - `input`: The input text sequence. `instruction` is automatically prepended to form the full input. (<instruction> `\n` <input>)
                         - `output`: The target sequence
             output_dir: The directory where model files will be saved. If not given, self.args.output_dir will be used.
-            show_running_loss (optional): Set to False to prevent running loss from being printed to console. Defaults to True.
             args (optional): Optional changes to the args dict of the model. Any changes made will persist for the model.
             eval_data (optional): A DataFrame against which evaluation will be performed when evaluate_during_training is enabled. Is required if evaluate_during_training is enabled.
+            verbose (optional): If True, all of the warnings related to data processing will be printed. 
             **kwargs: Additional metrics that should be used. Pass in the metrics as keyword arguments (name of metric: function to use).
                         A metric function should take in two parameters. The first parameter will be the true labels, and the second parameter will be the predictions. Both inputs
                         will be lists of strings. Note that this will slow down training significantly as the predicted sequences need to be generated.
 
         Returns:
             global_step: Number of global steps trained
             training_details: Average training loss if evaluate_during_training is False or full training progress scores if evaluate_during_training is True
@@ -193,39 +182,39 @@
             raise ValueError(
                 "evaluate_during_training is enabled but eval_data is not specified."
                 " Pass eval_data to model.train_model() if using evaluate_during_training."
             )
 
         if not output_dir:
             output_dir = self.args.output_dir
-        logger.info("*** Train ***")
         if (
                 os.path.exists(output_dir)
                 and os.listdir(output_dir)
                 and not self.args.overwrite_output_dir
         ):
             raise ValueError(
                 "Output directory ({}) already exists and is not empty."
                 " Set args.overwrite_output_dir = True to overcome.".format(output_dir)
             )
         # update model train config
         self.model.gradient_checkpointing_enable()
         self.model.enable_input_require_grads()
-        self.model.is_parallelizable = True
-        self.model.model_parallel = True
-        self.model.lm_head = CastOutputToFloat(self.model.lm_head)
+        if not self.ddp and torch.cuda.device_count() > 1:
+            # keeps Trainer from trying its own DataParallelism when more than 1 gpu is available
+            self.model.is_parallelizable = True
+            self.model.model_parallel = True
         self.model.config.use_cache = False
         resume_from_checkpoint = self.args.resume_from_checkpoint
 
         # setup peft, add lora config
         if self.args.use_lora:
             peft_config = LoraConfig(
                 task_type=TaskType.CAUSAL_LM,
                 inference_mode=False,
-                r=self.args.lora_rank,
+                r=self.args.lora_r,
                 lora_alpha=self.args.lora_alpha,
                 lora_dropout=self.args.lora_dropout,
                 target_modules=self.args.lora_target_modules,
                 bias=self.args.lora_bias,
             )
             if self.args.int8:
                 self.model = prepare_model_for_int8_training(self.model)
@@ -242,150 +231,114 @@
                     )
                 # The two files above have a different name depending on how they were saved, but are actually the same.
                 if os.path.exists(checkpoint_name):
                     logger.info(f"Restarting from {checkpoint_name}")
                     adapters_weights = torch.load(checkpoint_name)
                     self.model = set_peft_model_state_dict(self.model, adapters_weights)
                 else:
-                    logger.info(f"Checkpoint {checkpoint_name} not found")
+                    logger.warning(f"Checkpoint {checkpoint_name} not found")
 
-            print_trainable_parameters(self.model)
+            self.model.print_trainable_parameters()  # Be more transparent about the % of trainable params.
             self.lora_loaded = True
         else:
-            logger.error("only impl lora finetune, set `use_lora=True` for train.")
+            logger.error("only impl lora fine-tune, set `use_lora=True` for train.")
             raise ValueError("set `use_lora=True` for train.")
-        self._move_model_to_device()
-        # load dataset
-        train_dataset = self.load_and_cache_examples(train_data, verbose=verbose)
         os.makedirs(output_dir, exist_ok=True)
-        logger.debug(f"dataset: {train_dataset} first row: {next(iter(train_dataset))}")
+
+        # load dataset
+        train_dataset = self.load_and_cache_examples(train_data)
+        if verbose:
+            logger.debug(f"train_dataset len: {len(train_dataset)}, train_dataset[0]: {train_dataset[0]}")
+        eval_dataset = None
+        if eval_data is not None:
+            eval_dataset = self.load_and_cache_examples(eval_data, evaluate=True)
+            if verbose:
+                logger.debug(f"eval_dataset len: {len(eval_dataset)}, eval_dataset[0]: {eval_dataset[0]}")
 
         # start train
         training_args = TrainingArguments(
             output_dir=self.args.output_dir,
-            auto_find_batch_size=True,
             learning_rate=self.args.learning_rate,
             num_train_epochs=self.args.num_train_epochs,
             logging_dir=f"{self.args.output_dir}/logs",
             logging_steps=self.args.logging_steps,
             max_steps=self.args.max_steps,
             per_device_train_batch_size=self.args.per_device_train_batch_size,
             per_device_eval_batch_size=self.args.per_device_train_batch_size,
             gradient_accumulation_steps=self.args.gradient_accumulation_steps,
+            warmup_steps=self.args.warmup_steps,
             save_steps=self.args.save_steps,
+            optim=self.args.optimizer,
+            save_strategy=self.args.save_strategy,
+            evaluation_strategy='steps' if eval_data is not None else 'no',
+            eval_steps=self.args.eval_steps if eval_data is not None else None,
+            load_best_model_at_end=True if eval_data is not None else False,
+            ddp_find_unused_parameters=False if self.ddp else None,
             save_total_limit=self.args.save_total_limit,
             fp16=self.args.fp16,
             remove_unused_columns=self.args.remove_unused_columns,
             overwrite_output_dir=self.args.overwrite_output_dir,
-            do_train=True,
             no_cuda=True if self.device == "cpu" else False,
             **kwargs
         )
-        logger.debug(f"training_args: {training_args}")
+        # Log on each process the small summary:
+        logger.warning(
+            f"Process rank: {training_args.local_rank}, device: {training_args.device}, n_gpu: {training_args.n_gpu}, "
+            + f"distributed training: {bool(training_args.local_rank != -1)}, 16-bits training: {training_args.fp16}"
+        )
+        logger.info(f"Training/evaluation parameters {training_args}")
+
+        data_collator = DataCollatorForSeq2Seq(
+            self.tokenizer, pad_to_multiple_of=self.args.pad_to_multiple_of,
+            return_tensors="pt", padding=True
+        )
         trainer = FinetuneTrainer(
             model=self.model,
             train_dataset=train_dataset,
+            eval_dataset=eval_dataset if eval_data is not None else None,
             args=training_args,
             tokenizer=self.tokenizer,
-            data_collator=self.data_collator,
+            data_collator=data_collator,
         )
+
         if self.args.only_lora_state_dict:
             old_state_dict = self.model.state_dict
             self.model.state_dict = (
                 lambda self, *_, **__: get_peft_model_state_dict(
                     self, old_state_dict()
                 )
             ).__get__(self.model, type(self.model))
+
         if torch.__version__ >= "2" and sys.platform != "win32":
             self.model = torch.compile(self.model)
+
+        logger.info("*** Train ***")
         (global_step, training_loss, metrics) = trainer.train(resume_from_checkpoint=resume_from_checkpoint)
         self.handle_metrics("train", metrics, self.args.output_dir)
         self.results.update(metrics)
         self.save_model(model=self.model)
 
+        if eval_data is not None:
+            logger.info("*** Evaluate ***")
+            if torch.cuda.is_available() and self.args.fp16:
+                self.model = self.model.half().cuda()
+            metrics = trainer.evaluate(metric_key_prefix="eval")
+            logger.debug(f"eval metrics: {metrics}")
+            self.handle_metrics("eval", metrics, self.args.output_dir)
+            self.results.update(metrics)
+
         if verbose:
+            logger.debug(f"metrics: {self.results}")
             logger.info(
                 " Training of {} model complete. Saved to {}.".format(
                     self.args.model_name, output_dir
                 )
             )
         return global_step, training_loss
 
-    def eval_model(
-            self, eval_data, output_dir=None, verbose=True, silent=False, **kwargs
-    ):
-        """
-        Evaluates the model on eval_data. Saves results to output_dir.
-
-        Args:
-            eval_data: Pandas DataFrame containing the 2 columns - `input_text`, `target_text`.
-                        - `input_text`: The input text sequence.
-                        - `target_text`: The target text sequence.
-                        If `use_hf_datasets` is True, then this may also be the path to a TSV file with the same columns.
-            output_dir: The directory where model files will be saved. If not given, self.args.output_dir will be used.
-            verbose: If verbose, results will be printed to the console on completion of evaluation.
-            silent: If silent, tqdm progress bars will be hidden.
-            **kwargs: Additional metrics that should be used. Pass in the metrics as keyword arguments (name of metric: function to use).
-                        A metric function should take in two parameters. The first parameter will be the true labels, and the second parameter will be the predictions. Both inputs
-                        will be lists of strings. Note that this will slow down evaluation significantly as the predicted sequences need to be generated.
-        Returns:
-            results: Dictionary containing evaluation results.
-        """  # noqa: ignore flake8"
-
-        if not output_dir:
-            output_dir = self.args.output_dir
-        logger.info("*** Evaluate ***")
-        self._move_model_to_device()
-
-        eval_dataset = self.load_and_cache_examples(
-            eval_data, evaluate=True, verbose=verbose, silent=silent
-        )
-        os.makedirs(output_dir, exist_ok=True)
-
-        training_args = TrainingArguments(
-            output_dir=self.args.output_dir,
-            auto_find_batch_size=True,
-            learning_rate=self.args.learning_rate,
-            num_train_epochs=self.args.num_train_epochs,
-            logging_dir=f"{self.args.output_dir}/logs",
-            logging_steps=self.args.logging_steps,
-            max_steps=self.args.max_steps,
-            per_device_train_batch_size=self.args.per_device_train_batch_size,
-            per_device_eval_batch_size=self.args.per_device_train_batch_size,
-            gradient_accumulation_steps=self.args.gradient_accumulation_steps,
-            save_steps=self.args.save_steps,
-            save_total_limit=self.args.save_total_limit,
-            fp16=self.args.fp16,
-            remove_unused_columns=self.args.remove_unused_columns,
-            overwrite_output_dir=self.args.overwrite_output_dir,
-            do_train=False,
-            do_eval=True,
-            no_cuda=True if self.device == "cpu" else False,
-            **kwargs
-        )
-        logger.debug(f"training_args: {training_args}")
-        trainer = FinetuneTrainer(
-            model=self.model,
-            train_dataset=eval_dataset,
-            args=training_args,
-            tokenizer=self.tokenizer,
-            data_collator=self.data_collator,
-        )
-        metrics = trainer.evaluate(metric_key_prefix='val')
-        metrics["val_loss"] = round(metrics["val_loss"], 4)
-
-        if trainer.is_world_process_zero():
-            self.handle_metrics("val", metrics, self.args.output_dir)
-            self.results.update(metrics)
-
-        if verbose:
-            logger.info(self.results)
-
-        return self.results
-
     @staticmethod
     def handle_metrics(split, metrics, output_dir):
         """
         Log and save metrics
 
         Args:
         - split: one of train, val, test
@@ -399,42 +352,43 @@
         output_file = os.path.join(output_dir, f"{split}_results.txt")
         with open(output_file, "w") as writer:
             for key in sorted(metrics.keys()):
                 writer.write("{} = {}\n".format(key, str(metrics[key])))
 
     def load_lora(self):
         if self.args.use_lora:
-            if self.lora_name and self.lora_name.startswith('shibing624'):
+            if self.lora_name:
+                if os.path.isdir(self.lora_name) and os.path.exists(
+                        os.path.join(self.lora_name, "tokenizer_config.json")):
+                    update_tokenizer = True
+                else:
+                    update_tokenizer = False
+                if "ziqingyang/chinese" in self.lora_name or update_tokenizer:
+                    self.tokenizer = LlamaTokenizer.from_pretrained(self.lora_name)
+                    self.model.resize_token_embeddings(len(self.tokenizer))
+                    assert self.model.get_input_embeddings().weight.size(0) == len(self.tokenizer)
+                    logger.debug(f"Tokenizer updated, vocabulary size: {len(self.tokenizer)}")
                 self.model = PeftModel.from_pretrained(self.model, self.lora_name)
                 logger.info(f"Loaded lora model from {self.lora_name}")
                 self.lora_loaded = True
             else:
                 lora_path = os.path.join(self.args.output_dir, self.args.lora_name)
                 if lora_path and os.path.exists(lora_path):
-                    # infer with trained lora model
                     self.model = PeftModel.from_pretrained(self.model, self.args.output_dir)
                     logger.info(f"Loaded lora model from {lora_path}")
                     self.lora_loaded = True
+
+            # unwind broken decapoda-research config
+            self.tokenizer.padding_side = "left"
+            self.model.config.pad_token_id = self.tokenizer.pad_token_id = 0  # unk
+            self.model.config.bos_token_id = 1
+            self.model.config.eos_token_id = 2
             if torch.__version__ >= "2" and sys.platform != "win32":
                 self.model = torch.compile(self.model)
 
-    def process_response(self, response):
-        response = response.strip().replace("[[训练时间]]", "2023年")
-        punkts = [
-            [",", "，"],
-            ["!", "！"],
-            [":", "："],
-            [";", "；"],
-            ["\?", "？"],
-        ]
-        for item in punkts:
-            response = re.sub(r"([\u4e00-\u9fff])%s" % item[0], r"\1%s" % item[1], response)
-            response = re.sub(r"%s([\u4e00-\u9fff])" % item[0], r"%s\1" % item[1], response)
-        return response
-
     @torch.no_grad()
     def predict(self, sentences, keep_prompt=False, max_length=None, **kwargs):
         """
         Performs predictions on a list of text.
 
         Args:
             sentences: A python list of text (str) to be sent to the model for prediction. 
@@ -443,46 +397,47 @@
 
         Returns:
             preds: A python list of the generated sequences.
         """  # noqa: ignore flake8"
 
         if not self.lora_loaded:
             self.load_lora()
-        if torch.cuda.is_available() and self.args.fp16:
-            self.model = self.model.half().cuda()
         self._move_model_to_device()
         self.model.eval()
 
         all_outputs = []
         # Batching
         for batch in tqdm(
                 [
                     sentences[i: i + self.args.eval_batch_size]
                     for i in range(0, len(sentences), self.args.eval_batch_size)
                 ],
                 desc="Generating outputs",
                 disable=self.args.silent,
         ):
             inputs = self.tokenizer(batch, padding=True, return_tensors='pt').to(self.device)
-            gen_kwargs = {
-                "max_length": max_length if max_length else self.args.max_length,
-                "num_beams": self.args.num_beams,
-                "do_sample": self.args.do_sample,
-                "top_p": self.args.top_p,
-                "temperature": self.args.temperature,
-                "eos_token_id": self.tokenizer.eos_token_id,
-                **kwargs
-            }
-            outputs = self.model.generate(**inputs, **gen_kwargs)
-            for idx, (prompt_text, generated_sequence) in enumerate(zip(batch, outputs)):
+            generation_config = GenerationConfig(
+                max_new_tokens=max_length if max_length else self.args.max_length,
+                temperature=self.args.temperature,
+                top_p=self.args.top_p,
+                top_k=self.args.top_k,
+                num_beams=self.args.num_beams,
+                eos_token_id=self.tokenizer.eos_token_id,
+                pad_token_id=self.tokenizer.pad_token_id,
+                num_return_sequences=self.args.num_return_sequences,
+                return_dict_in_generate=True,
+                output_scores=True,
+                **kwargs,
+            )
+            outputs = self.model.generate(**inputs, generation_config=generation_config)
+            for idx, (prompt_text, generated_sequence) in enumerate(zip(batch, outputs.sequences)):
                 # Decode text
                 text = self.tokenizer.decode(generated_sequence)
                 prompt_len = len(prompt_text)
                 gen_text = text[prompt_len:]
-                gen_text = self.process_response(gen_text)
                 if keep_prompt:
                     total_sequence = prompt_text + gen_text
                 else:
                     total_sequence = gen_text
                 all_outputs.append(total_sequence)
         return all_outputs
 
@@ -494,37 +449,35 @@
         :param query:
         :param history:
         :param keep_prompt:
         :param max_length:
         :param kwargs:
         :return: response, history
         """
-        self._move_model_to_device()
-        self.model.eval()
         if history is None:
             history = []
         if not history:
             prompt = query
         else:
             prompt = ""
             for i, (old_query, response) in enumerate(history):
                 prompt += "[Round {}]\n问：{}\n答：{}\n".format(i, old_query, response)
             prompt += "[Round {}]\n问：{}\n答：".format(len(history), query)
         response = self.predict([prompt], keep_prompt=keep_prompt, max_length=len(prompt) + max_length, **kwargs)[0]
         history = history + [(query, response)]
         return response, history
 
     def _move_model_to_device(self):
-        self.model.to(self.device)
+        self.model.to(self.device, dtype=torch.float16 if self.args.fp16 else torch.float32)
 
     def load_and_cache_examples(
             self, data, evaluate=False, no_cache=False, verbose=True, silent=False
     ):
         """
-        Creates a ChatGLMDataset from data.
+        Creates a LlamaDataset from data.
 
         Utility function for train() and eval() methods. Not intended to be used directly.
         """
 
         tokenizer = self.tokenizer
         args = self.args
 
@@ -539,15 +492,15 @@
         if self.args.use_hf_datasets:
             dataset = load_hf_dataset(data, tokenizer, self.args, mode)
             return dataset
         elif args.dataset_class:
             CustomDataset = args.dataset_class
             return CustomDataset(tokenizer, args, data, mode)
         else:
-            return ChatGlmDataset(
+            return LlamaDataset(
                 tokenizer,
                 self.args,
                 data,
                 mode,
             )
 
     def save_model(
@@ -574,49 +527,17 @@
             self.save_model_args(output_dir)
 
     def save_model_args(self, output_dir):
         os.makedirs(output_dir, exist_ok=True)
         self.args.save(output_dir)
 
     def _load_model_args(self, input_dir):
-        args = ChatGlmArgs()
+        args = LlamaArgs()
         args.load(input_dir)
         return args
 
-    def get_named_parameters(self):
-        return [n for n, p in self.model.named_parameters()]
-
 
 class FinetuneTrainer(Trainer):
-    def compute_loss(self, model, inputs, return_outputs=False):
-        return model(
-            input_ids=inputs["input_ids"],
-            labels=inputs["labels"],
-        ).loss
-
-    def save_model(self, output_dir=None, _internal_call=False, lora_name='adapter_model.bin'):
+    def save_model(self, output_dir=None, _internal_call=False):
         os.makedirs(output_dir, exist_ok=True)
         torch.save(self.args, os.path.join(output_dir, TRAINING_ARGS_NAME))
-        saved_params = {
-            k: v.to("cpu") for k, v in self.model.named_parameters() if v.requires_grad
-        }
-        torch.save(saved_params, os.path.join(output_dir, lora_name))
-
-
-class CastOutputToFloat(nn.Sequential):
-    def forward(self, x):
-        return super().forward(x).to(torch.float32)
-
-
-def print_trainable_parameters(model):
-    """
-    Prints the number of trainable parameters in the model.
-    """
-    trainable_params = 0
-    all_param = 0
-    for _, param in model.named_parameters():
-        all_param += param.numel()
-        if param.requires_grad:
-            trainable_params += param.numel()
-    logger.debug(
-        f"trainable params: {trainable_params} || all params: {all_param} || trainable%: {100 * trainable_params / all_param}"
-    )
+        self.model.save_pretrained(output_dir)
```

### Comparing `textgen-0.1.8/textgen/chatglm/chatglm_utils.py` & `textgen-0.1.9/textgen/chatglm/chatglm_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 @description: 
 """
 
 import os
 import pickle
 from multiprocessing import Pool
 
+import datasets
+import numpy as np
 from datasets import Dataset as HFDataset
 from datasets import load_dataset
 from loguru import logger
+from rouge import Rouge
 from torch.utils.data import Dataset
-import numpy as np
 from tqdm.auto import tqdm
-from nltk.translate.bleu_score import sentence_bleu, SmoothingFunction
-from rouge import Rouge
 
 
 def preprocess_data(data):
     instruction, input_text, target_text, tokenizer, args = data
 
     prompt = f"问：{instruction}\n"
     if input_text:
@@ -41,31 +41,35 @@
     return dataset
 
 
 def load_hf_dataset(data, tokenizer, args, mode):
     if isinstance(data, str):
         if data.endswith('.json') or data.endswith('.jsonl'):
             dataset = load_dataset("json", data_files=data)
+        elif os.path.isdir(data):
+            dataset = datasets.load_from_disk(data)
         else:
             dataset = load_dataset(
                 data,
                 download_mode="force_redownload"
                 if args.reprocess_input_data
                 else "reuse_dataset_if_exists",
             )
         # This is not necessarily a train dataset. The datasets library insists on calling it train.
-        split = 'validation' if mode == 'dev' else mode
-        dataset = dataset[split]
+        dataset = dataset['train']
+        if mode == 'dev' and args.max_eval_samples is not None:
+            max_eval_samples = min(len(dataset), args.max_eval_samples)
+            dataset = dataset.select(range(max_eval_samples))
     else:
         dataset = HFDataset.from_pandas(data)
 
     dataset = dataset.map(
         lambda x: preprocess_batch_for_hf_dataset(x, tokenizer=tokenizer, args=args),
         batched=False,
-    )
+    ).filter(lambda x: tokenizer.bos_token_id in list(x['input_ids']))  # must contain bos_token_id
 
     dataset.set_format(type="np", columns=["input_ids"])
 
     return dataset["input_ids"]
 
 
 class ChatGlmDataset(Dataset):
@@ -122,14 +126,15 @@
         return len(self.examples)
 
     def __getitem__(self, index):
         return self.examples[index]
 
 
 def compute_bleu(label, pred, weights=None):
+    from nltk.translate.bleu_score import sentence_bleu, SmoothingFunction
     weights = weights or (0.25, 0.25, 0.25, 0.25)
     return np.mean([sentence_bleu(references=[list(a)], hypothesis=list(b),
                                   smoothing_function=SmoothingFunction().method1, weights=weights)
                     for a, b in zip(label, pred)])
 
 
 def compute_rouge(label, pred, weights=None, mode='weighted'):
```

### Comparing `textgen-0.1.8/textgen/config/global_args.py` & `textgen-0.1.9/textgen/config/global_args.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/config/model_args.py` & `textgen-0.1.9/textgen/config/model_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     evaluate_during_training: bool = False
     evaluate_during_training_silent: bool = True
     evaluate_during_training_steps: int = 2000
     evaluate_during_training_verbose: bool = False
     evaluate_each_epoch: bool = True
     fp16: bool = False
     gradient_accumulation_steps: int = 1
-    learning_rate: float = 4e-5
+    learning_rate: float = 2e-5
     local_rank: int = -1
     logging_steps: int = 50
     manual_seed: int = None
     max_grad_norm: float = 1.0
     max_seq_length: int = 128
     model_name: str = None
     model_type: str = None
@@ -335,43 +335,103 @@
 class ChatGlmArgs(ModelArgs):
     """
     Model args for a ChatGLMModel
     """
 
     model_class: str = "ChatGlmArgs"
     dataset_class: Dataset = None
+    learning_rate: float = 2e-4
     fp16: bool = True
     int8: bool = False
-    quantization_bit:int = None  # if use quantization bit, set 4, else None
+    quantization_bit: int = None  # if use quantization bit, set 4, else None
     debug: bool = False
     max_seq_length: int = 256  # max length of input sequence
     max_length = 384  # max length of the sequence to be generated
     do_sample: bool = True
     early_stopping: bool = True
-    evaluate_generated_text: bool = False
+    evaluate_generated_text: bool = True
+    optimizer: str = "adamw_torch"
+    save_strategy: str = "steps"
+    evaluation_strategy: str = "no"
+    eval_steps: int = None
+    save_steps: int = 400
+    max_eval_samples: int = 20
     length_penalty: float = 2.0
     num_beams: int = 1
     num_return_sequences: int = 1
     repetition_penalty: float = 1.0
     temperature: float = 0.95
     special_tokens_list: list = field(default_factory=list)
     top_k: float = None
     top_p: float = 0.7
     model_name_or_path: Optional[str] = field(default="THUDM/chatglm-6b")
     dataset_name_or_path: Optional[str] = field(default="shibing624/alpaca-zh")
     use_lora: bool = True
     lora_name: str = field(default="adapter_model.bin")
-    lora_rank: int = field(default=8)
-    lora_alpha = 32
-    lora_dropout = 0.1
+    lora_r: int = 8
+    lora_alpha = 16
+    lora_dropout = 0.05
     lora_target_modules = ["query_key_value"]
     lora_bias = "none"
     only_lora_state_dict: bool = False
     num_train_epochs = 1
     max_steps = -1
     per_device_train_batch_size = 2
+    eval_batch_size: int = 2
     gradient_accumulation_steps = 1
-    save_total_limit = 2
+    save_total_limit = 3
     remove_unused_columns = False
     logging_steps = 50
-    resume_from_checkpoint:str = None
+    resume_from_checkpoint: str = None
+
+
+@dataclass
+class LlamaArgs(ModelArgs):
+    """
+    Model args for a LlamaModel
+    """
 
+    model_class: str = "LlamaArgs"
+    dataset_class: Dataset = None
+    learning_rate: float = 3e-4
+    fp16: bool = True
+    int8: bool = False
+    quantization_bit: int = None  # if use quantization bit, set 4, else None
+    debug: bool = False
+    max_seq_length: int = 256  # max length of input sequence
+    max_length = 384  # max length of the sequence to be generated
+    do_sample: bool = True
+    early_stopping: bool = True
+    evaluate_generated_text: bool = True
+    warmup_steps: int = 50
+    optimizer: str = "adamw_torch"
+    save_strategy: str = "steps"
+    eval_steps: int = 200
+    save_steps: int = 400
+    pad_to_multiple_of: int = 8
+    max_eval_samples: int = 20
+    length_penalty: float = 2.0
+    num_beams: int = 1
+    num_return_sequences: int = 1
+    repetition_penalty: float = 1.0
+    temperature: float = 0.95
+    special_tokens_list: list = field(default_factory=list)
+    top_k: float = 30
+    top_p: float = 0.7
+    model_name_or_path: Optional[str] = field(default="decapoda-research/llama-7b-hf")
+    use_lora: bool = True
+    lora_name: str = field(default="adapter_model.bin")
+    lora_r: int = 8
+    lora_alpha = 16
+    lora_dropout = 0.05
+    lora_target_modules = ["q_proj", "k_proj", "v_proj", "o_proj"]
+    lora_bias = "none"
+    only_lora_state_dict: bool = True
+    num_train_epochs = 3
+    max_steps = -1
+    per_device_train_batch_size = 2
+    eval_batch_size: int = 2
+    gradient_accumulation_steps = 1
+    save_total_limit = 3
+    remove_unused_columns = False
+    logging_steps = 50
+    resume_from_checkpoint: str = None
```

### Comparing `textgen-0.1.8/textgen/custom_models/models.py` & `textgen-0.1.9/textgen/custom_models/models.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/data/HowNetPOSWord.txt` & `textgen-0.1.9/textgen/data/HowNetPOSWord.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/data/stopwords.txt` & `textgen-0.1.9/textgen/data/stopwords.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/language_generation/language_generation_model.py` & `textgen-0.1.9/textgen/language_generation/language_generation_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/language_generation/language_generation_utils.py` & `textgen-0.1.9/textgen/language_generation/language_generation_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/language_modeling/language_modeling_model.py` & `textgen-0.1.9/textgen/language_modeling/language_modeling_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/language_modeling/language_modeling_utils.py` & `textgen-0.1.9/textgen/language_modeling/language_modeling_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/language_modeling/songnet_model.py` & `textgen-0.1.9/textgen/language_modeling/songnet_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/language_modeling/songnet_utils.py` & `textgen-0.1.9/textgen/language_modeling/songnet_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/seq2seq/bart_seq2seq_model.py` & `textgen-0.1.9/textgen/seq2seq/bart_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/seq2seq/bart_seq2seq_utils.py` & `textgen-0.1.9/textgen/seq2seq/bart_seq2seq_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/seq2seq/conv_seq2seq_model.py` & `textgen-0.1.9/textgen/seq2seq/conv_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/seq2seq/data_reader.py` & `textgen-0.1.9/textgen/seq2seq/data_reader.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/seq2seq/seq2seq_model.py` & `textgen-0.1.9/textgen/seq2seq/seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/seq2seq/seq2seq_trainer.py` & `textgen-0.1.9/textgen/seq2seq/seq2seq_trainer.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/t5/copyt5_model.py` & `textgen-0.1.9/textgen/t5/copyt5_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/t5/copyt5_utils.py` & `textgen-0.1.9/textgen/t5/copyt5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/t5/t5_model.py` & `textgen-0.1.9/textgen/t5/t5_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/t5/t5_utils.py` & `textgen-0.1.9/textgen/t5/t5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/unsup_generation/tgls_model.py` & `textgen-0.1.9/textgen/unsup_generation/tgls_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen/unsup_generation/tgls_util.py` & `textgen-0.1.9/textgen/unsup_generation/tgls_util.py`

 * *Files identical despite different names*

### Comparing `textgen-0.1.8/textgen.egg-info/PKG-INFO` & `textgen-0.1.9/textgen.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.1.8
+Version: 0.1.9
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/textgen)
         [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/project/textgen)
@@ -15,65 +15,71 @@
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
         # TextGen
         
         🌈 Implementation of Text Generation models.
         
-        **textgen**实现了多种文本生成模型，包括：UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
+        **textgen**实现了多种文本生成模型，包括：LLAMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
         
         **Guide**
         
         - [Feature](#Feature)
         - [Install](#install)
         - [Usage](#usage)
         - [Contact](#Contact)
         - [Reference](#reference)
         
         # Feature
+        
         ## 文本生成
         
         1. seq2seq: Seq2Seq、ConvSeq2Seq、BART
-        2. language_modeling: GPT2、SongNet
+        2. language_modeling: GPT2、SongNet、ChatGLM、LLAMA
         3. t5: T5、CopyT5
-        4. question_answering: BERT、XLNet
-        5. chatglm: ChatGLM
         
         ## 文本扩增
+        
         ### 词粒度扩增
+        
         1. UDA，非核心词替换
         2. EDA，简单数据增强技术：相似词、同义词替换，随机词插入、删除、替换
         
         ### 句粒度扩增
+        
         1. 回译（BT, Back Translate）：中文-英文-中文
         2. GPT2模型续写：短文本->长文本
         3. BART摘要模型：长文本->短文本
         4. TGLS：无监督相似文本生成模型
         
         ## 功能列表
+        - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
+        - [LLAMA](textgen/llama)：本项目基于PyTorch实现了LLAMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
         - [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
         - [BT(回译)](textgen/augment/sentence_level_augment.py)：本项目基于百度翻译API实现了回译功能，先把中文句子翻译为英文，再把英文翻译为新的中文
         - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
         - [T5](textgen/t5)：本项目基于PyTorch实现了T5和CopyT5模型训练和预测，可以用于文本翻译、对话生成、对联生成、文案撰写等文本生成任务
         - [GPT2](textgen/language_modeling)：本项目基于PyTorch实现了GTP2模型训练和预测，可以用于文章生成、对联生成等文本生成任务
         - [SongNet](textgen/language_modeling/songnet_model.py)：本项目基于PyTorch实现了SongNet模型训练和预测，可以用于规范格式的诗词、歌词等文本生成任务
         - [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
         
         
         ## Release Models
+        
         release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
         
-        |Model|Arch|Intro|Training|Inference|
+        |Model|Arch|Introduce|Training|Inference| 
         |:-- |:--- |:--- |:--- |:--- |
         |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)|T5|中文NLP多任务Prompt模型|[prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5_prompt_demo.py)|
         |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)|T5|fine-tuned中文对联后的模型|[对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/t5_couplet_demo.py)|
         |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)|SongNet|SongNet预训练模型|-|-|
         |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)|SongNet|fine-tuned宋词后的模型|[training script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet_songci_demo.py)|
         |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)|SongNet|fine-tuned对联后的模型|[training script](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet_couplet_demo.py)|
-        
+        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)|ChatGLM-6B|在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重|[training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)|
+        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)|ChatGLM-6B|在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重|[training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|[predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)|
         
         # Demo
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/chinese-couplet-generate
         
         ![](docs/hf.png)
         
@@ -84,33 +90,76 @@
         ```
         
         model trained by [examples/T5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/T5/T5_Finetune_Chinese_Couplet.ipynb)
         
         # Install
         
         ```shell
-        pip install torch # conda install pytorch
         pip install -U textgen
         ```
         
         or
         
         ```shell
         pip install torch # conda install pytorch
         git clone https://github.com/shibing624/textgen.git
         cd textgen
-        python3 setup.py install
+        python setup.py install
         ```
         
         # Usage
         
+        ## ChatGLM-6B LoRA 模型
+        
+        ### 使用ChatGLM-6B LoRA微调后的模型
+        example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
+        
+        ```python
+        import sys
+        
+        sys.path.append('../..')
+        from textgen import ChatGlmModel
+        
+        model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", lora_name="shibing624/chatglm-6b-csc-zh-lora")
+        r = model.predict(["对下面中文拼写纠错：\n少先队员因该为老人让坐。\n答："])
+        print(r)  # ['少先队员应该为老人让座。\n错误字：因，坐']
+        ```
+        
+        ### 训练ChatGLM-6B LoRA模型
+        
+        支持自定义数据集，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)。
+        
+        example: [examples/chatglm/training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_demo.py)
+        
+        ## LLAMA LoRA 模型
+        
+        ### 使用LLAMA LoRA微调后的模型
+        
+        example: [examples/llama/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/predict_demo.py)
+        
+        ```python
+        import sys
+        
+        sys.path.append('../..')
+        from textgen import LlamaModel
+        
+        model = LlamaModel("llama", "huggyllama/llama-7b", lora_name="qychen/luotuo-lora-7b-0.1")
+        r = model.predict(["失眠了怎么办？"])
+        print(r)
+        ```
+        
+        ### 训练LLAMA LoRA模型
+        
+        example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)
+        
         ## ConvSeq2Seq 模型
+        
         训练并预测ConvSeq2Seq模型：
         
-        example: [examples/seq2sesq/training_convseq2seq_model_demo.py](examples/seq2seq/training_convseq2seq_model_demo.py)
+        example: [examples/seq2sesq/training_convseq2seq_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_convseq2seq_model_demo.py)
         
         ```python
         import argparse
         from loguru import logger
         import sys
         
         sys.path.append('../..')
@@ -152,27 +201,26 @@
         
         ```bash
         inputs: ["什么是ai", "你是什么类型的计算机", "你知道热力学吗"]
         outputs: ['人工智能是工程和科学的分支,致力于构建思维的机器。', '我的程序运行在python,所以我在任何运脑上工作！', '我不能错热是一个疯狂的人工智能"200年。']
         ```
         
         ## BART 模型
-        训练并预测BART模型：
         
-        example: [examples/seq2sesq/training_bartseq2seq_zh_demo.py](examples/seq2seq/training_bartseq2seq_zh_demo.py)
+        训练并预测BART模型：
         
+        example: [examples/seq2sesq/training_bartseq2seq_zh_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_bartseq2seq_zh_demo.py)
         
         output:
         
         ```shell
         inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
         outputs: ['人工智能是工程和科学的分支,致力于构', '我的程序运行在python,所以我在任何电脑上', '什么是热力学吗？']
         ```
         
-        
         ## T5 模型
         
         example: [examples/T5/training_zh_t5_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/T5/training_zh_t5_model_demo.py)
         
         ```python
         import argparse
         from loguru import logger
@@ -260,22 +308,20 @@
         
         
         if __name__ == '__main__':
             main()
         ```
         
         output:
+        
         ```shell
         inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
         outputs: ['人工智能有两个广义的定义,任何拟人的机械,如在卡雷尔capeks', '我的程序运行在Python,所以我在任何电脑上工作!', '什么是热力学']
         ```
         
-        
-        
-        
         ## GPT2 模型
         
         ### 中文GPT2 - 文章生成
         
         使用中文数据集（段落格式，`\n`间隔），训练GPT2模型，可以用于诗歌生成、文章生成等任务。
         
         example: [examples/language_generation/training_zh_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_gpt2_demo.py)
@@ -283,14 +329,15 @@
         ### 中文GPT2 - 对联生成
         
         使用中文对联数据集（tsv格式，`\t`间隔），自定义数据集读取Dataset，训练GPT2模型，可以用于对联生成、对话生成等任务。
         
         example: [examples/language_generation/training_couplet_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_couplet_gpt2_demo.py)
         
         #### GPT2 vs T5：
+        
         1. 都是从Transformer改进来的，T5同时有编码器和解码器，GPT2只有解码器
         2. T5的模型优势是处理给定输入，产出对应输出的任务，如翻译、对话、问答等
         3. GPT2的模型优势是自由创作，如写一篇短文
         4. T5的对联生成效果好于GPT2、GPT2的诗词生成效果好于T5
         
         - [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)
         - [古诗生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%8F%A4%E8%AF%97%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md)
@@ -298,16 +345,14 @@
         ## SongNet 模型
         
         格式控制的文本生成模型，paper见[SongNet: Rigid Formats Controlled Text Generation](https://arxiv.org/abs/2004.08022)，
         适用于强韵律格式要求的诗歌、对联、歌词生成等任务。
         
         example: [examples/language_generation/training_zh_songnet_demo.py](https://github.com/shibing624/textgen/blob/main/examples/language_generation/training_zh_songnet_demo.py)
         
-        
-        
         ## Keyword Text Augmentation(EDA/UDA)
         
         example: [examples/text_augmentation_demo.py](examples/text_augmentation_demo.py)
         
         ```python
         import sys
         
@@ -414,24 +459,31 @@
         希望好用，面膜用过了很好用，皮肤水嫩光滑白皙，补水不错，价格也合适。
         就是精华液太少了，保湿效果不错。
         面膜的补水效果非常好，保湿效果确实很赞，这个面膜相对于胶原蛋白和美白的那两款的面膜纸要厚一些，看着价格合适。
         ```
         
         前10句是真实用户评论，后10句是生成的。
         
+        # Dataset
+        
+        1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
+        2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
+        3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
+        4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+        5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
+        
         # Contact
         
         - Issue(建议)
           ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我： 加我*微信号：xuming624, 备注：姓名-公司名-NLP* 进NLP交流群。
         
         <img src="docs/wechat.jpeg" width="200" />
         
-        
         # Citation
         
         如果你在研究中使用了textgen，请按如下格式引用：
         
         ```latex
         @misc{textgen,
           title={textgen: Text Generation Tool},
@@ -461,15 +513,15 @@
         - [minimaxir/gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
         - [asyml/texar](https://github.com/asyml/texar)
         - [yangjianxin1/GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat)
         - [williamSYSU/TextGAN-PyTorch](https://github.com/williamSYSU/TextGAN-PyTorch)
         - [RUCAIBox/TextBox](https://github.com/RUCAIBox/TextBox)
         - [Tiiiger/bert_score]()
         - [1YCxZ/Fake-review-generation](https://github.com/1YCxZ/Fake-review-generation)
-        
+        - [tloen/alpaca-lora](https://github.com/tloen/alpaca-lora/blob/main/finetune.py)
 Keywords: textgen,text-generation,Text Generation Tool,ernie-gen,chinese text generation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Linguistic
```

### Comparing `textgen-0.1.8/textgen.egg-info/SOURCES.txt` & `textgen-0.1.9/textgen.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 textgen/language_generation/language_generation_model.py
 textgen/language_generation/language_generation_utils.py
 textgen/language_modeling/__init__.py
 textgen/language_modeling/language_modeling_model.py
 textgen/language_modeling/language_modeling_utils.py
 textgen/language_modeling/songnet_model.py
 textgen/language_modeling/songnet_utils.py
+textgen/llama/__init__.py
+textgen/llama/llama_model.py
+textgen/llama/llama_utils.py
 textgen/seq2seq/__init__.py
 textgen/seq2seq/bart_seq2seq_model.py
 textgen/seq2seq/bart_seq2seq_utils.py
 textgen/seq2seq/conv_seq2seq_model.py
 textgen/seq2seq/data_reader.py
 textgen/seq2seq/seq2seq_model.py
 textgen/seq2seq/seq2seq_trainer.py
```

