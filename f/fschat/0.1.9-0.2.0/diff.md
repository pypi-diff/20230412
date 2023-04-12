# Comparing `tmp/fschat-0.1.9.tar.gz` & `tmp/fschat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fschat-0.1.9.tar", last modified: Sat Apr  8 15:48:39 2023, max compression
+gzip compressed data, was "fschat-0.2.0.tar", last modified: Wed Apr 12 19:33:55 2023, max compression
```

## Comparing `fschat-0.1.9.tar` & `fschat-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,59 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.062306 fschat-0.1.9/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.1.9/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11862 2023-04-08 15:48:39.062306 fschat-0.1.9/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11388 2023-04-08 15:47:09.000000 fschat-0.1.9/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.058306 fschat-0.1.9/fastchat/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       88 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6432 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.058306 fschat-0.1.9/fastchat/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1819 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/data/alpaca-converter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4465 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/data/clean_sharegpt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      615 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/data/inspect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2684 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/data/optional_clean.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/data/pretty_json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3403 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/data/split_long_conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.058306 fschat-0.1.9/fastchat/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5042 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/eval/eval_gpt_review.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3661 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/eval/generate_webpage_data_from_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3054 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/eval/get_model_answer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2345 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/eval/qa_baseline_gpt35.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.062306 fschat-0.1.9/fastchat/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2036 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/model/apply_delta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2303 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/model/make_delta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.062306 fschat-0.1.9/fastchat/serve/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/serve/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6691 2023-04-08 15:47:09.000000 fschat-0.1.9/fastchat/serve/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2023-04-08 15:47:09.000000 fschat-0.1.9/fastchat/serve/compression.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9942 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/serve/controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2717 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/serve/gradio_css.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/serve/gradio_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16383 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/serve/gradio_web_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6775 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/serve/model_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3997 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/serve/monkey_patch_non_inplace.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/serve/register_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/serve/serve_chatglm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2028 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/serve/test_message.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.062306 fschat-0.1.9/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3982 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/train/llama_flash_attn_monkey_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12308 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/train/train.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3657 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/train/train_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      420 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/train/train_mem.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4186 2023-04-08 15:47:09.000000 fschat-0.1.9/fastchat/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.062306 fschat-0.1.9/fschat.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11862 2023-04-08 15:48:39.000000 fschat-0.1.9/fschat.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1228 2023-04-08 15:48:39.000000 fschat-0.1.9/fschat.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-08 15:48:39.000000 fschat-0.1.9/fschat.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2023-04-08 15:48:39.000000 fschat-0.1.9/fschat.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-04-08 15:48:39.000000 fschat-0.1.9/fschat.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      938 2023-04-08 15:48:30.000000 fschat-0.1.9/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-08 15:48:39.062306 fschat-0.1.9/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 19:33:55.071399 fschat-0.2.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11731 2023-04-12 19:33:55.071399 fschat-0.2.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11257 2023-04-12 19:30:04.000000 fschat-0.2.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 19:33:55.067399 fschat-0.2.0/fastchat/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.2.0/fastchat/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5440 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 19:33:55.067399 fschat-0.2.0/fastchat/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.2.0/fastchat/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1819 2023-04-03 18:06:47.000000 fschat-0.2.0/fastchat/data/alpaca-converter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5543 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/data/clean_sharegpt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5976 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/data/hardcoded_questions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      615 2023-04-03 18:06:47.000000 fschat-0.2.0/fastchat/data/inspect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/data/merge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2684 2023-04-08 06:26:44.000000 fschat-0.2.0/fastchat/data/optional_clean.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-03 18:06:47.000000 fschat-0.2.0/fastchat/data/pretty_json.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/data/sample.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3188 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/data/split_long_conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 19:33:55.067399 fschat-0.2.0/fastchat/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5042 2023-04-08 06:26:44.000000 fschat-0.2.0/fastchat/eval/eval_gpt_review.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3661 2023-04-03 18:06:47.000000 fschat-0.2.0/fastchat/eval/generate_webpage_data_from_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2986 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/eval/get_model_answer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2345 2023-04-03 18:06:47.000000 fschat-0.2.0/fastchat/eval/qa_baseline_gpt35.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 19:33:55.067399 fschat-0.2.0/fastchat/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.2.0/fastchat/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1576 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/model/apply_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      840 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/model/convert_fp16.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1669 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/model/make_delta.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 19:33:55.071399 fschat-0.2.0/fastchat/serve/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.2.0/fastchat/serve/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11255 2023-04-10 08:26:53.000000 fschat-0.2.0/fastchat/serve/cacheflow_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4206 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/serve/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2023-04-09 00:28:23.000000 fschat-0.2.0/fastchat/serve/compression.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9943 2023-04-11 03:55:38.000000 fschat-0.2.0/fastchat/serve/controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2717 2023-04-03 18:06:47.000000 fschat-0.2.0/fastchat/serve/gradio_css.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-04-03 18:06:47.000000 fschat-0.2.0/fastchat/serve/gradio_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16276 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/serve/gradio_web_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6539 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/serve/inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7053 2023-04-11 17:38:03.000000 fschat-0.2.0/fastchat/serve/model_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3997 2023-04-08 06:26:44.000000 fschat-0.2.0/fastchat/serve/monkey_patch_non_inplace.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-03 18:06:47.000000 fschat-0.2.0/fastchat/serve/register_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-09 00:28:23.000000 fschat-0.2.0/fastchat/serve/serve_chatglm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2359 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/serve/test_message.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3867 2023-04-11 03:55:38.000000 fschat-0.2.0/fastchat/serve/test_throughput.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 19:33:55.071399 fschat-0.2.0/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3982 2023-04-08 06:26:44.000000 fschat-0.2.0/fastchat/train/llama_flash_attn_monkey_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8450 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/train/train.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3657 2023-04-08 06:26:44.000000 fschat-0.2.0/fastchat/train/train_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      345 2023-04-12 19:30:04.000000 fschat-0.2.0/fastchat/train/train_mem.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4186 2023-04-09 00:28:23.000000 fschat-0.2.0/fastchat/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 19:33:55.071399 fschat-0.2.0/fschat.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11731 2023-04-12 19:33:55.000000 fschat-0.2.0/fschat.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1440 2023-04-12 19:33:55.000000 fschat-0.2.0/fschat.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-12 19:33:55.000000 fschat-0.2.0/fschat.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-04-12 19:33:55.000000 fschat-0.2.0/fschat.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-04-12 19:33:55.000000 fschat-0.2.0/fschat.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      979 2023-04-12 19:33:46.000000 fschat-0.2.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-12 19:33:55.071399 fschat-0.2.0/setup.cfg
```

### Comparing `fschat-0.1.9/LICENSE` & `fschat-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/PKG-INFO` & `fschat-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.1.9
+Version: 0.2.0
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -51,15 +51,15 @@
 ```bash
 git clone https://github.com/lm-sys/FastChat.git
 cd FastChat
 ```
 
 If you are running on Mac:
 ```bash
-brew install rust
+brew install rust cmake
 ```
 
 2. Install Package
 ```bash
 pip3 install --upgrade pip  # enable PEP 660 support
 pip3 install -e .
 ```
@@ -71,84 +71,85 @@
 1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
 2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
 Our released weights are only compatible with the latest main branch of huggingface/transformers.
 We install the correct version of transformers when fastchat is installed.
 
-### Vicuna-13B
-This conversion command needs around 60 GB of CPU RAM.
+### Vicuna-7B
+This conversion command needs around 30 GB of CPU RAM.
 If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
-    --base /path/to/llama-13b \
-    --target /output/path/to/vicuna-13b \
-    --delta lmsys/vicuna-13b-delta-v0
+    --base /path/to/llama-7b \
+    --target /output/path/to/vicuna-7b \
+    --delta lmsys/vicuna-7b-delta-v1.1
 ```
 
-### Vicuna-7B
-This conversion command needs around 30 GB of CPU RAM.
+### Vicuna-13B
+This conversion command needs around 60 GB of CPU RAM.
 If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
-    --base /path/to/llama-7b \
-    --target /output/path/to/vicuna-7b \
-    --delta lmsys/vicuna-7b-delta-v0
+    --base /path/to/llama-13b \
+    --target /output/path/to/vicuna-13b \
+    --delta lmsys/vicuna-13b-delta-v1.1
 ```
 
+### Old weights
+See [docs/weights_version.md](docs/weights_version.md) for all versions of weights and their differences.
+
 ## Inference with Command Line Interface
 
+(Experimental Feature: You can specify `--style rich` to enable rich text output and better text streaming quality for some non-ASCII content. This may not work properly on certain terminals.)
+
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
+See the "No Enough Memory" section below if you do not have enough memory.
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
 ```
 
 #### Multiple GPUs
-If you do not have enough GPU memory, you can use model parallelism to aggregate memory from multiple GPUs on the same machine.
+You can use model parallelism to aggregate GPU memory from multiple GPUs on the same machine.
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --num-gpus 2
 ```
 
 #### CPU Only
 This runs on the CPU only and does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device cpu
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu
 ```
 
 #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs)
-Use `--device mps` to enable GPU acceleration on Mac computers and use `--load-8bit` to turn on 8-bit compression.
+Use `--device mps` to enable GPU acceleration on Mac computers (requires torch >= 2.0).
+Use `--load-8bit` to turn on 8-bit compression.
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device mps --load-8bit
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device mps --load-8bit
 ```
 Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second.
 
 #### No Enough Memory or Other Platforms
 If you do not have enough memory, you can enable 8-bit compression by adding `--load-8bit` to commands above.
-This can reduce the memory usage by around half with slightly degraded model quality.
+This can reduce memory usage by around half with slightly degraded model quality.
 It is compatible with the CPU, GPU, and Metal backend.
-Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4090/V100(16GB) GPU.
+Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4080/V100(16GB) GPU.
 
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --load-8bit
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --load-8bit
 ```
 
 Besides, we are actively exploring more methods to make the model easier to run on more platforms.
 Contributions and pull requests are welcome.
 
 ## Serving with Web GUI
 
 To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. Here are the commands to follow in your terminal:
 
-**Note for Windows users:** Windows users will need Python 3.7 and above and to set the following environmental variable prior to launching the worker.
-
-```
-PYTHONUTF8=1
-```
-
 #### Launch the controller
 ```bash
 python3 -m fastchat.serve.controller
 ```
 
 This controller manages the distributed workers.
 
@@ -171,40 +172,80 @@
 This is the user interface that users will interact with.
 
 By following these steps, you will be able to serve your models using the web UI. You can open your browser and chat with a model now.
 
 
 ## Evaluation
 
-Our AI-enhanced [evaluation](fastchat/eval) pipeline is based on GPT-4. Here are some high-level instructions for using the pipeline:
+Our AI-enhanced evaluation pipeline is based on GPT-4. This section provides a high-level summary of the pipeline. For detailed instructions, please refer to the [evaluation](fastchat/eval) documentation.
+
+### Pipeline Steps
+
+1. Generate answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for Vicuna and other models.
+
+2. Generate reviews with GPT-4: Use GPT-4 to generate reviews automatically. This step can also be performed manually if the GPT-4 API is not available to you.
+
+3. Generate visualization data: Run `generate_webpage_data_from_table.py` to generate data for a static website, which allows you to visualize the evaluation data.
 
-First, generate answers from different models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint and run `model_qa.py` for Vicuna and other models.
+4. Visualize the data: Serve a static website under the `webpage` directory. You can use `python3 -m http.server` to serve the website locally.
 
-Then, use GPT-4 to generate reviews automatically, which can be done manually if the GPT-4 API is not available to you. Once you have your evaluation data, visualize the results by running `generate_webpage_data_from_table.py`, which generates data for a static website.
+### Data Format and Contribution
 
-Finally, serve a static website under the `webpage` directory. You can simply use `python3 -m http.server` to serve the website locally.
+We use a data format encoded with JSON Lines for evaluation. The format includes information on models, prompts, reviewers, questions, answers, and reviews.
 
-Besides the evaluation workflow, we also document the data format used for evaluation, which is encoded with JSON Lines and includes information on models, prompts, reviewers, questions, answers, and reviews. You can customize the evaluation process or contribute to our project by accessing relevant [data](fastchat/eval/table/).
+You can customize the evaluation process or contribute to our project by accessing the relevant [data](fastchat/eval/table/).
 
-Check [evaluation](fastchat/eval) for detailed instructions.
+For detailed instructions, please refer to the [evaluation](fastchat/eval) documentation.
 
 ## Fine-tuning
 ### Data
 
 Vicuna is created by fine-tuning a LLaMA base model using approximately 70K user-shared conversations gathered from ShareGPT.com with public APIs. To ensure data quality, we convert the HTML back to markdown and filter out some inappropriate or low-quality samples. Additionally, we divide lengthy conversations into smaller segments that fit the model's maximum context length. For detailed instructions to clean the ShareGPT data, check out [here](docs/commands/data_cleaning.md).
 
-Due to some concerns, we may not release the data at the moment. If you would like to try the fine-tuning code, you can try to run it with our [preprocessed alpaca dataset](playground/data/alpaca-data-conversation.json) (originally from [here](https://github.com/tatsu-lab/stanford_alpaca)).
+Due to some concerns, we may not release the ShareGPT dataset at the moment. If you would like to try the fine-tuning code, you can run it with some dummy questions in [dummy.json](playground/data/dummy.json). You can follow the same format and plug in your own data.
 
 ### Code and Hyperparameters
-We fine-tune the model using the code from [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca), with some modifications to support gradient checkpointing and [Flash Attention](https://github.com/HazyResearch/flash-attention). We use similar hyperparameters as the Stanford Alpaca.
+Our code is based on [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) with additional support for multi-round conversations.
+We use similar hyperparameters as the Stanford Alpaca.
 
 | Hyperparameter | Global Batch Size | Learning rate | Epochs | Max length | Weight decay |
 | --- | ---: | ---: | ---: | ---: | ---: |
 | Vicuna-13B | 128 | 2e-5 | 3 | 2048 | 0 |
 
+### Fine-tuning Vicuna-7B with Local GPUs
+You can use the following command to train Vicuna-7B with 4 x A100 (40GB).
+```bash
+torchrun --nproc_per_node=4 --master_port=20001 fastchat/train/train_mem.py \
+    --model_name_or_path ~/model_weights/llama-7b  \
+    --data_path playground/data/dummy.json \
+    --bf16 True \
+    --output_dir output \
+    --num_train_epochs 3 \
+    --per_device_train_batch_size 2 \
+    --per_device_eval_batch_size 2 \
+    --gradient_accumulation_steps 16 \
+    --evaluation_strategy "no" \
+    --save_strategy "steps" \
+    --save_steps 1200 \
+    --save_total_limit 10 \
+    --learning_rate 2e-5 \
+    --weight_decay 0. \
+    --warmup_ratio 0.03 \
+    --lr_scheduler_type "cosine" \
+    --logging_steps 1 \
+    --fsdp "full_shard auto_wrap" \
+    --fsdp_transformer_layer_cls_to_wrap 'LlamaDecoderLayer' \
+    --tf32 True \
+    --model_max_length 2048 \
+    --gradient_checkpointing True \
+    --lazy_preprocess True
+```
+
+If you meet out-of-memory during model saving, see solutions [here](https://github.com/pytorch/pytorch/issues/98823).
+
 ### Fine-tuning on Any Cloud with SkyPilot
 [SkyPilot](https://github.com/skypilot-org/skypilot) is a framework built by UC Berkeley for easily and cost effectively running ML workloads on any cloud (AWS, GCP, Azure, Lambda, etc.). 
 To use SkyPilot, install it with the following command and setup the cloud credentials locally following the instructions [here](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html).
 ```bash
 # Install skypilot from the master branch
 pip install git+https://github.com/skypilot-org/skypilot.git
 ```
@@ -218,43 +259,7 @@
 # Launch it on managed spot to save 3x cost (train Vicuna-13B with around $300)
 sky spot launch -n vicuna scripts/train-vicuna.yaml --env WANDB_API_KEY
 
 # Train a 7B model
 sky launch -c vicuna -s scripts/train-vicuna.yaml --env WANDB_API_KEY --env MODEL_SIZE=7
 ```
 Note: Please make sure the `WANDB_API_KEY` has been setup on your local machine. You can find the API key on your [wandb profile page](https://wandb.ai/authorize). If you would like to train the model without using wandb, you can replace the `--env WANDB_API_KEY` flag with `--env WANDB_MODE=offline`.
-
-#### Alpaca
-Launch the training job with the following line (will be launched on a single node with 4 A100-80GB GPUs)
-```
-sky launch -c alpaca -s scripts/train-alpaca.yaml --env WANDB_API_KEY
-```
-
-### Fine-tuning with Local GPUs
-Vicuna can also be trained on 8 A100 GPUs with 80GB memory with the following code. To train on fewer GPUs, you can reduce the `per_device_train_batch_size` and increase the `gradient_accumulation_steps` accordingly to keep the global batch size the same. To setup the environment, please see the setup section in [scripts/train-vicuna.yaml](scripts/train-vicuna.yaml).
-```bash
-torchrun --nnodes=1 --nproc_per_node=8 --master_port=<your_random_port> \
-    fastchat/train/train_mem.py \
-    --model_name_or_path <path-to-llama-model-weight> \
-    --data_path <path-to-data> \
-    --bf16 True \
-    --output_dir ./checkpoints \
-    --num_train_epochs 3 \
-    --per_device_train_batch_size 4 \
-    --per_device_eval_batch_size 4 \
-    --gradient_accumulation_steps 1 \
-    --evaluation_strategy "no" \
-    --save_strategy "steps" \
-    --save_steps 1200 \
-    --save_total_limit 100 \
-    --learning_rate 2e-5 \
-    --weight_decay 0. \
-    --warmup_ratio 0.03 \
-    --lr_scheduler_type "cosine" \
-    --logging_steps 1 \
-    --fsdp "full_shard auto_wrap" \
-    --fsdp_transformer_layer_cls_to_wrap 'LlamaDecoderLayer' \
-    --tf32 True \
-    --model_max_length 2048 \
-    --gradient_checkpointing True \
-    --lazy_preprocess True
-```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.1.9 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.2.0 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE # FastChat An open platform for training, serving, and evaluating large
 language model based chatbots. ## Release
@@ -16,138 +16,137 @@
 Interface](#inference-with-command-line-interface) - [Serving with Web GUI]
 (#serving-with-web-gui) - [Evaluation](#evaluation) - [Fine-tuning](#fine-
 tuning) ## Install ### Method 1: With pip ```bash # Install FastChat pip3
 install fschat # Install the latest main branch of huggingface/transformers
 pip3 install git+https://github.com/huggingface/transformers ``` ### Method 2:
 From source 1. Clone this repository and navigate to the FastChat folder
 ```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ``` If you
-are running on Mac: ```bash brew install rust ``` 2. Install Package ```bash
-pip3 install --upgrade pip # enable PEP 660 support pip3 install -e . ``` ##
-Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as delta
-weights to comply with the LLaMA model license. You can add our delta to the
-original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get the
-original LLaMA weights in the huggingface format by following the instructions
-[here](https://huggingface.co/docs/transformers/main/model_doc/llama). 2. Use
-the following scripts to get Vicuna weights by applying our delta. They will
-automatically download delta weights from our Hugging Face [account](https://
-huggingface.co/lmsys). **NOTE**: Our released weights are only compatible with
-the latest main branch of huggingface/transformers. We install the correct
-version of transformers when fastchat is installed. ### Vicuna-13B This
+are running on Mac: ```bash brew install rust cmake ``` 2. Install Package
+```bash pip3 install --upgrade pip # enable PEP 660 support pip3 install -e .
+``` ## Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as
+delta weights to comply with the LLaMA model license. You can add our delta to
+the original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get
+the original LLaMA weights in the huggingface format by following the
+instructions [here](https://huggingface.co/docs/transformers/main/model_doc/
+llama). 2. Use the following scripts to get Vicuna weights by applying our
+delta. They will automatically download delta weights from our Hugging Face
+[account](https://huggingface.co/lmsys). **NOTE**: Our released weights are
+only compatible with the latest main branch of huggingface/transformers. We
+install the correct version of transformers when fastchat is installed. ###
+Vicuna-7B This conversion command needs around 30 GB of CPU RAM. If you do not
+have enough memory, you can create a large swap file that allows the operating
+system to automatically utilize the disk as virtual memory. ```bash python3 -
+m fastchat.model.apply_delta \ --base /path/to/llama-7b \ --target /output/
+path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-v1.1 ``` ### Vicuna-13B This
 conversion command needs around 60 GB of CPU RAM. If you do not have enough
 memory, you can create a large swap file that allows the operating system to
 automatically utilize the disk as virtual memory. ```bash python3 -
 m fastchat.model.apply_delta \ --base /path/to/llama-13b \ --target /output/
-path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v0 ``` ### Vicuna-7B This
-conversion command needs around 30 GB of CPU RAM. If you do not have enough
-memory, you can create a large swap file that allows the operating system to
-automatically utilize the disk as virtual memory. ```bash python3 -
-m fastchat.model.apply_delta \ --base /path/to/llama-7b \ --target /output/
-path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-v0 ``` ## Inference with
-Command Line Interface #### Single GPU The command below requires around 28GB
-of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. ``` python3
--m fastchat.serve.cli --model-name /path/to/vicuna/weights ``` #### Multiple
-GPUs If you do not have enough GPU memory, you can use model parallelism to
-aggregate memory from multiple GPUs on the same machine. ``` python3 -
-m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2 ``` ####
-CPU Only This runs on the CPU only and does not require GPU. It requires around
-60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
-``` python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device
-cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
-`--device mps` to enable GPU acceleration on Mac computers and use `--load-
-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-
-name /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can run on
-a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or Other
-Platforms If you do not have enough memory, you can enable 8-bit compression by
-adding `--load-8bit` to commands above. This can reduce the memory usage by
-around half with slightly degraded model quality. It is compatible with the
-CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run on a
-single NVIDIA 3090/4090/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --
-model-name /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
+path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v1.1 ``` ### Old weights
+See [docs/weights_version.md](docs/weights_version.md) for all versions of
+weights and their differences. ## Inference with Command Line Interface
+(Experimental Feature: You can specify `--style rich` to enable rich text
+output and better text streaming quality for some non-ASCII content. This may
+not work properly on certain terminals.) #### Single GPU The command below
+requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for
+Vicuna-7B. See the "No Enough Memory" section below if you do not have enough
+memory. ``` python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
+``` #### Multiple GPUs You can use model parallelism to aggregate GPU memory
+from multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on
+the CPU only and does not require GPU. It requires around 60GB of CPU memory
+for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu ``` ####
+Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
+to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
+load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can
+run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or
+Other Platforms If you do not have enough memory, you can enable 8-bit
+compression by adding `--load-8bit` to commands above. This can reduce memory
+usage by around half with slightly degraded model quality. It is compatible
+with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
+on a single NVIDIA 3090/4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli
+--model-path /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
 exploring more methods to make the model easier to run on more platforms.
 Contributions and pull requests are welcome. ## Serving with Web GUI To serve
 using the web UI, you need three main components: web servers that interface
 with users, model workers that host one or more models, and a controller to
 coordinate the webserver and model workers. Here are the commands to follow in
-your terminal: **Note for Windows users:** Windows users will need Python 3.7
-and above and to set the following environmental variable prior to launching
-the worker. ``` PYTHONUTF8=1 ``` #### Launch the controller ```bash python3 -
+your terminal: #### Launch the controller ```bash python3 -
 m fastchat.serve.controller ``` This controller manages the distributed
 workers. #### Launch the model worker ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". You can launch multiple model workers to serve multiple models
 concurrently. The model worker will connect to the controller automatically. To
 ensure that your model worker is connected to your controller properly, send a
 test message using the following command: ```bash python3 -
 m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
 Gradio web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This
 is the user interface that users will interact with. By following these steps,
 you will be able to serve your models using the web UI. You can open your
-browser and chat with a model now. ## Evaluation Our AI-enhanced [evaluation]
-(fastchat/eval) pipeline is based on GPT-4. Here are some high-level
-instructions for using the pipeline: First, generate answers from different
-models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint
-and run `model_qa.py` for Vicuna and other models. Then, use GPT-4 to generate
-reviews automatically, which can be done manually if the GPT-4 API is not
-available to you. Once you have your evaluation data, visualize the results by
-running `generate_webpage_data_from_table.py`, which generates data for a
-static website. Finally, serve a static website under the `webpage` directory.
-You can simply use `python3 -m http.server` to serve the website locally.
-Besides the evaluation workflow, we also document the data format used for
-evaluation, which is encoded with JSON Lines and includes information on
-models, prompts, reviewers, questions, answers, and reviews. You can customize
-the evaluation process or contribute to our project by accessing relevant
-[data](fastchat/eval/table/). Check [evaluation](fastchat/eval) for detailed
-instructions. ## Fine-tuning ### Data Vicuna is created by fine-tuning a LLaMA
+browser and chat with a model now. ## Evaluation Our AI-enhanced evaluation
+pipeline is based on GPT-4. This section provides a high-level summary of the
+pipeline. For detailed instructions, please refer to the [evaluation](fastchat/
+eval) documentation. ### Pipeline Steps 1. Generate answers from different
+models: Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint
+and run `get_model_answer.py` for Vicuna and other models. 2. Generate reviews
+with GPT-4: Use GPT-4 to generate reviews automatically. This step can also be
+performed manually if the GPT-4 API is not available to you. 3. Generate
+visualization data: Run `generate_webpage_data_from_table.py` to generate data
+for a static website, which allows you to visualize the evaluation data. 4.
+Visualize the data: Serve a static website under the `webpage` directory. You
+can use `python3 -m http.server` to serve the website locally. ### Data Format
+and Contribution We use a data format encoded with JSON Lines for evaluation.
+The format includes information on models, prompts, reviewers, questions,
+answers, and reviews. You can customize the evaluation process or contribute to
+our project by accessing the relevant [data](fastchat/eval/table/). For
+detailed instructions, please refer to the [evaluation](fastchat/eval)
+documentation. ## Fine-tuning ### Data Vicuna is created by fine-tuning a LLaMA
 base model using approximately 70K user-shared conversations gathered from
 ShareGPT.com with public APIs. To ensure data quality, we convert the HTML back
 to markdown and filter out some inappropriate or low-quality samples.
 Additionally, we divide lengthy conversations into smaller segments that fit
 the model's maximum context length. For detailed instructions to clean the
 ShareGPT data, check out [here](docs/commands/data_cleaning.md). Due to some
-concerns, we may not release the data at the moment. If you would like to try
-the fine-tuning code, you can try to run it with our [preprocessed alpaca
-dataset](playground/data/alpaca-data-conversation.json) (originally from [here]
-(https://github.com/tatsu-lab/stanford_alpaca)). ### Code and Hyperparameters
-We fine-tune the model using the code from [Stanford Alpaca](https://
-github.com/tatsu-lab/stanford_alpaca), with some modifications to support
-gradient checkpointing and [Flash Attention](https://github.com/HazyResearch/
-flash-attention). We use similar hyperparameters as the Stanford Alpaca. |
-Hyperparameter | Global Batch Size | Learning rate | Epochs | Max length |
-Weight decay | | --- | ---: | ---: | ---: | ---: | ---: | | Vicuna-13B | 128 |
-2e-5 | 3 | 2048 | 0 | ### Fine-tuning on Any Cloud with SkyPilot [SkyPilot]
-(https://github.com/skypilot-org/skypilot) is a framework built by UC Berkeley
-for easily and cost effectively running ML workloads on any cloud (AWS, GCP,
-Azure, Lambda, etc.). To use SkyPilot, install it with the following command
-and setup the cloud credentials locally following the instructions [here]
-(https://skypilot.readthedocs.io/en/latest/getting-started/installation.html).
-```bash # Install skypilot from the master branch pip install git+https://
-github.com/skypilot-org/skypilot.git ``` #### Vicuna Vicuna can be trained on 8
-A100 GPUs with 80GB memory. The following command will automatically launch a
-node satisfying the requirement, setup and run the training job on it. ```bash
-sky launch -c vicuna -s scripts/train-vicuna.yaml --env WANDB_API_KEY ``` Other
-options are also valid: ```bash # Launch it on managed spot to save 3x cost
-(train Vicuna-13B with around $300) sky spot launch -n vicuna scripts/train-
-vicuna.yaml --env WANDB_API_KEY # Train a 7B model sky launch -c vicuna -
-s scripts/train-vicuna.yaml --env WANDB_API_KEY --env MODEL_SIZE=7 ``` Note:
-Please make sure the `WANDB_API_KEY` has been setup on your local machine. You
-can find the API key on your [wandb profile page](https://wandb.ai/authorize).
-If you would like to train the model without using wandb, you can replace the
-`--env WANDB_API_KEY` flag with `--env WANDB_MODE=offline`. #### Alpaca Launch
-the training job with the following line (will be launched on a single node
-with 4 A100-80GB GPUs) ``` sky launch -c alpaca -s scripts/train-alpaca.yaml --
-env WANDB_API_KEY ``` ### Fine-tuning with Local GPUs Vicuna can also be
-trained on 8 A100 GPUs with 80GB memory with the following code. To train on
-fewer GPUs, you can reduce the `per_device_train_batch_size` and increase the
-`gradient_accumulation_steps` accordingly to keep the global batch size the
-same. To setup the environment, please see the setup section in [scripts/train-
-vicuna.yaml](scripts/train-vicuna.yaml). ```bash torchrun --nnodes=1 --
-nproc_per_node=8 --master_port= \ fastchat/train/train_mem.py \ --
-model_name_or_path  \ --data_path  \ --bf16 True \ --output_dir ./checkpoints \
---num_train_epochs 3 \ --per_device_train_batch_size 4 \ --
-per_device_eval_batch_size 4 \ --gradient_accumulation_steps 1 \ --
+concerns, we may not release the ShareGPT dataset at the moment. If you would
+like to try the fine-tuning code, you can run it with some dummy questions in
+[dummy.json](playground/data/dummy.json). You can follow the same format and
+plug in your own data. ### Code and Hyperparameters Our code is based on
+[Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) with additional
+support for multi-round conversations. We use similar hyperparameters as the
+Stanford Alpaca. | Hyperparameter | Global Batch Size | Learning rate | Epochs
+| Max length | Weight decay | | --- | ---: | ---: | ---: | ---: | ---: | |
+Vicuna-13B | 128 | 2e-5 | 3 | 2048 | 0 | ### Fine-tuning Vicuna-7B with Local
+GPUs You can use the following command to train Vicuna-7B with 4 x A100 (40GB).
+```bash torchrun --nproc_per_node=4 --master_port=20001 fastchat/train/
+train_mem.py \ --model_name_or_path ~/model_weights/llama-7b \ --data_path
+playground/data/dummy.json \ --bf16 True \ --output_dir output \ --
+num_train_epochs 3 \ --per_device_train_batch_size 2 \ --
+per_device_eval_batch_size 2 \ --gradient_accumulation_steps 16 \ --
 evaluation_strategy "no" \ --save_strategy "steps" \ --save_steps 1200 \ --
-save_total_limit 100 \ --learning_rate 2e-5 \ --weight_decay 0. \ --
-warmup_ratio 0.03 \ --lr_scheduler_type "cosine" \ --logging_steps 1 \ --fsdp
-"full_shard auto_wrap" \ --fsdp_transformer_layer_cls_to_wrap
-'LlamaDecoderLayer' \ --tf32 True \ --model_max_length 2048 \ --
-gradient_checkpointing True \ --lazy_preprocess True ```
+save_total_limit 10 \ --learning_rate 2e-5 \ --weight_decay 0. \ --warmup_ratio
+0.03 \ --lr_scheduler_type "cosine" \ --logging_steps 1 \ --fsdp "full_shard
+auto_wrap" \ --fsdp_transformer_layer_cls_to_wrap 'LlamaDecoderLayer' \ --tf32
+True \ --model_max_length 2048 \ --gradient_checkpointing True \ --
+lazy_preprocess True ``` If you meet out-of-memory during model saving, see
+solutions [here](https://github.com/pytorch/pytorch/issues/98823). ### Fine-
+tuning on Any Cloud with SkyPilot [SkyPilot](https://github.com/skypilot-org/
+skypilot) is a framework built by UC Berkeley for easily and cost effectively
+running ML workloads on any cloud (AWS, GCP, Azure, Lambda, etc.). To use
+SkyPilot, install it with the following command and setup the cloud credentials
+locally following the instructions [here](https://skypilot.readthedocs.io/en/
+latest/getting-started/installation.html). ```bash # Install skypilot from the
+master branch pip install git+https://github.com/skypilot-org/skypilot.git ```
+#### Vicuna Vicuna can be trained on 8 A100 GPUs with 80GB memory. The
+following command will automatically launch a node satisfying the requirement,
+setup and run the training job on it. ```bash sky launch -c vicuna -s scripts/
+train-vicuna.yaml --env WANDB_API_KEY ``` Other options are also valid: ```bash
+# Launch it on managed spot to save 3x cost (train Vicuna-13B with around $300)
+sky spot launch -n vicuna scripts/train-vicuna.yaml --env WANDB_API_KEY # Train
+a 7B model sky launch -c vicuna -s scripts/train-vicuna.yaml --env
+WANDB_API_KEY --env MODEL_SIZE=7 ``` Note: Please make sure the `WANDB_API_KEY`
+has been setup on your local machine. You can find the API key on your [wandb
+profile page](https://wandb.ai/authorize). If you would like to train the model
+without using wandb, you can replace the `--env WANDB_API_KEY` flag with `--env
+WANDB_MODE=offline`.
```

### Comparing `fschat-0.1.9/README.md` & `fschat-0.2.0/fschat.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: fschat
+Version: 0.2.0
+Summary: An open platform for training, serving, and evaluating large language model based chatbots.
+Project-URL: Homepage, https://github.com/lm-sys/fastchat
+Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # FastChat
 An open platform for training, serving, and evaluating large language model based chatbots.
 
 ## Release
 
 <p align="center">
 <a href="https://vicuna.lmsys.org"><img src="assets/vicuna-logo.jpeg" width="20%"></a>
@@ -39,15 +51,15 @@
 ```bash
 git clone https://github.com/lm-sys/FastChat.git
 cd FastChat
 ```
 
 If you are running on Mac:
 ```bash
-brew install rust
+brew install rust cmake
 ```
 
 2. Install Package
 ```bash
 pip3 install --upgrade pip  # enable PEP 660 support
 pip3 install -e .
 ```
@@ -59,84 +71,85 @@
 1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
 2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
 Our released weights are only compatible with the latest main branch of huggingface/transformers.
 We install the correct version of transformers when fastchat is installed.
 
-### Vicuna-13B
-This conversion command needs around 60 GB of CPU RAM.
+### Vicuna-7B
+This conversion command needs around 30 GB of CPU RAM.
 If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
-    --base /path/to/llama-13b \
-    --target /output/path/to/vicuna-13b \
-    --delta lmsys/vicuna-13b-delta-v0
+    --base /path/to/llama-7b \
+    --target /output/path/to/vicuna-7b \
+    --delta lmsys/vicuna-7b-delta-v1.1
 ```
 
-### Vicuna-7B
-This conversion command needs around 30 GB of CPU RAM.
+### Vicuna-13B
+This conversion command needs around 60 GB of CPU RAM.
 If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
-    --base /path/to/llama-7b \
-    --target /output/path/to/vicuna-7b \
-    --delta lmsys/vicuna-7b-delta-v0
+    --base /path/to/llama-13b \
+    --target /output/path/to/vicuna-13b \
+    --delta lmsys/vicuna-13b-delta-v1.1
 ```
 
+### Old weights
+See [docs/weights_version.md](docs/weights_version.md) for all versions of weights and their differences.
+
 ## Inference with Command Line Interface
 
+(Experimental Feature: You can specify `--style rich` to enable rich text output and better text streaming quality for some non-ASCII content. This may not work properly on certain terminals.)
+
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
+See the "No Enough Memory" section below if you do not have enough memory.
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
 ```
 
 #### Multiple GPUs
-If you do not have enough GPU memory, you can use model parallelism to aggregate memory from multiple GPUs on the same machine.
+You can use model parallelism to aggregate GPU memory from multiple GPUs on the same machine.
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --num-gpus 2
 ```
 
 #### CPU Only
 This runs on the CPU only and does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device cpu
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu
 ```
 
 #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs)
-Use `--device mps` to enable GPU acceleration on Mac computers and use `--load-8bit` to turn on 8-bit compression.
+Use `--device mps` to enable GPU acceleration on Mac computers (requires torch >= 2.0).
+Use `--load-8bit` to turn on 8-bit compression.
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device mps --load-8bit
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device mps --load-8bit
 ```
 Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second.
 
 #### No Enough Memory or Other Platforms
 If you do not have enough memory, you can enable 8-bit compression by adding `--load-8bit` to commands above.
-This can reduce the memory usage by around half with slightly degraded model quality.
+This can reduce memory usage by around half with slightly degraded model quality.
 It is compatible with the CPU, GPU, and Metal backend.
-Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4090/V100(16GB) GPU.
+Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4080/V100(16GB) GPU.
 
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --load-8bit
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --load-8bit
 ```
 
 Besides, we are actively exploring more methods to make the model easier to run on more platforms.
 Contributions and pull requests are welcome.
 
 ## Serving with Web GUI
 
 To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. Here are the commands to follow in your terminal:
 
-**Note for Windows users:** Windows users will need Python 3.7 and above and to set the following environmental variable prior to launching the worker.
-
-```
-PYTHONUTF8=1
-```
-
 #### Launch the controller
 ```bash
 python3 -m fastchat.serve.controller
 ```
 
 This controller manages the distributed workers.
 
@@ -159,40 +172,80 @@
 This is the user interface that users will interact with.
 
 By following these steps, you will be able to serve your models using the web UI. You can open your browser and chat with a model now.
 
 
 ## Evaluation
 
-Our AI-enhanced [evaluation](fastchat/eval) pipeline is based on GPT-4. Here are some high-level instructions for using the pipeline:
+Our AI-enhanced evaluation pipeline is based on GPT-4. This section provides a high-level summary of the pipeline. For detailed instructions, please refer to the [evaluation](fastchat/eval) documentation.
+
+### Pipeline Steps
+
+1. Generate answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for Vicuna and other models.
+
+2. Generate reviews with GPT-4: Use GPT-4 to generate reviews automatically. This step can also be performed manually if the GPT-4 API is not available to you.
+
+3. Generate visualization data: Run `generate_webpage_data_from_table.py` to generate data for a static website, which allows you to visualize the evaluation data.
 
-First, generate answers from different models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint and run `model_qa.py` for Vicuna and other models.
+4. Visualize the data: Serve a static website under the `webpage` directory. You can use `python3 -m http.server` to serve the website locally.
 
-Then, use GPT-4 to generate reviews automatically, which can be done manually if the GPT-4 API is not available to you. Once you have your evaluation data, visualize the results by running `generate_webpage_data_from_table.py`, which generates data for a static website.
+### Data Format and Contribution
 
-Finally, serve a static website under the `webpage` directory. You can simply use `python3 -m http.server` to serve the website locally.
+We use a data format encoded with JSON Lines for evaluation. The format includes information on models, prompts, reviewers, questions, answers, and reviews.
 
-Besides the evaluation workflow, we also document the data format used for evaluation, which is encoded with JSON Lines and includes information on models, prompts, reviewers, questions, answers, and reviews. You can customize the evaluation process or contribute to our project by accessing relevant [data](fastchat/eval/table/).
+You can customize the evaluation process or contribute to our project by accessing the relevant [data](fastchat/eval/table/).
 
-Check [evaluation](fastchat/eval) for detailed instructions.
+For detailed instructions, please refer to the [evaluation](fastchat/eval) documentation.
 
 ## Fine-tuning
 ### Data
 
 Vicuna is created by fine-tuning a LLaMA base model using approximately 70K user-shared conversations gathered from ShareGPT.com with public APIs. To ensure data quality, we convert the HTML back to markdown and filter out some inappropriate or low-quality samples. Additionally, we divide lengthy conversations into smaller segments that fit the model's maximum context length. For detailed instructions to clean the ShareGPT data, check out [here](docs/commands/data_cleaning.md).
 
-Due to some concerns, we may not release the data at the moment. If you would like to try the fine-tuning code, you can try to run it with our [preprocessed alpaca dataset](playground/data/alpaca-data-conversation.json) (originally from [here](https://github.com/tatsu-lab/stanford_alpaca)).
+Due to some concerns, we may not release the ShareGPT dataset at the moment. If you would like to try the fine-tuning code, you can run it with some dummy questions in [dummy.json](playground/data/dummy.json). You can follow the same format and plug in your own data.
 
 ### Code and Hyperparameters
-We fine-tune the model using the code from [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca), with some modifications to support gradient checkpointing and [Flash Attention](https://github.com/HazyResearch/flash-attention). We use similar hyperparameters as the Stanford Alpaca.
+Our code is based on [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) with additional support for multi-round conversations.
+We use similar hyperparameters as the Stanford Alpaca.
 
 | Hyperparameter | Global Batch Size | Learning rate | Epochs | Max length | Weight decay |
 | --- | ---: | ---: | ---: | ---: | ---: |
 | Vicuna-13B | 128 | 2e-5 | 3 | 2048 | 0 |
 
+### Fine-tuning Vicuna-7B with Local GPUs
+You can use the following command to train Vicuna-7B with 4 x A100 (40GB).
+```bash
+torchrun --nproc_per_node=4 --master_port=20001 fastchat/train/train_mem.py \
+    --model_name_or_path ~/model_weights/llama-7b  \
+    --data_path playground/data/dummy.json \
+    --bf16 True \
+    --output_dir output \
+    --num_train_epochs 3 \
+    --per_device_train_batch_size 2 \
+    --per_device_eval_batch_size 2 \
+    --gradient_accumulation_steps 16 \
+    --evaluation_strategy "no" \
+    --save_strategy "steps" \
+    --save_steps 1200 \
+    --save_total_limit 10 \
+    --learning_rate 2e-5 \
+    --weight_decay 0. \
+    --warmup_ratio 0.03 \
+    --lr_scheduler_type "cosine" \
+    --logging_steps 1 \
+    --fsdp "full_shard auto_wrap" \
+    --fsdp_transformer_layer_cls_to_wrap 'LlamaDecoderLayer' \
+    --tf32 True \
+    --model_max_length 2048 \
+    --gradient_checkpointing True \
+    --lazy_preprocess True
+```
+
+If you meet out-of-memory during model saving, see solutions [here](https://github.com/pytorch/pytorch/issues/98823).
+
 ### Fine-tuning on Any Cloud with SkyPilot
 [SkyPilot](https://github.com/skypilot-org/skypilot) is a framework built by UC Berkeley for easily and cost effectively running ML workloads on any cloud (AWS, GCP, Azure, Lambda, etc.). 
 To use SkyPilot, install it with the following command and setup the cloud credentials locally following the instructions [here](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html).
 ```bash
 # Install skypilot from the master branch
 pip install git+https://github.com/skypilot-org/skypilot.git
 ```
@@ -206,43 +259,7 @@
 # Launch it on managed spot to save 3x cost (train Vicuna-13B with around $300)
 sky spot launch -n vicuna scripts/train-vicuna.yaml --env WANDB_API_KEY
 
 # Train a 7B model
 sky launch -c vicuna -s scripts/train-vicuna.yaml --env WANDB_API_KEY --env MODEL_SIZE=7
 ```
 Note: Please make sure the `WANDB_API_KEY` has been setup on your local machine. You can find the API key on your [wandb profile page](https://wandb.ai/authorize). If you would like to train the model without using wandb, you can replace the `--env WANDB_API_KEY` flag with `--env WANDB_MODE=offline`.
-
-#### Alpaca
-Launch the training job with the following line (will be launched on a single node with 4 A100-80GB GPUs)
-```
-sky launch -c alpaca -s scripts/train-alpaca.yaml --env WANDB_API_KEY
-```
-
-### Fine-tuning with Local GPUs
-Vicuna can also be trained on 8 A100 GPUs with 80GB memory with the following code. To train on fewer GPUs, you can reduce the `per_device_train_batch_size` and increase the `gradient_accumulation_steps` accordingly to keep the global batch size the same. To setup the environment, please see the setup section in [scripts/train-vicuna.yaml](scripts/train-vicuna.yaml).
-```bash
-torchrun --nnodes=1 --nproc_per_node=8 --master_port=<your_random_port> \
-    fastchat/train/train_mem.py \
-    --model_name_or_path <path-to-llama-model-weight> \
-    --data_path <path-to-data> \
-    --bf16 True \
-    --output_dir ./checkpoints \
-    --num_train_epochs 3 \
-    --per_device_train_batch_size 4 \
-    --per_device_eval_batch_size 4 \
-    --gradient_accumulation_steps 1 \
-    --evaluation_strategy "no" \
-    --save_strategy "steps" \
-    --save_steps 1200 \
-    --save_total_limit 100 \
-    --learning_rate 2e-5 \
-    --weight_decay 0. \
-    --warmup_ratio 0.03 \
-    --lr_scheduler_type "cosine" \
-    --logging_steps 1 \
-    --fsdp "full_shard auto_wrap" \
-    --fsdp_transformer_layer_cls_to_wrap 'LlamaDecoderLayer' \
-    --tf32 True \
-    --model_max_length 2048 \
-    --gradient_checkpointing True \
-    --lazy_preprocess True
-```
```

#### html2text {}

```diff
@@ -1,8 +1,14 @@
-# FastChat An open platform for training, serving, and evaluating large
+Metadata-Version: 2.1 Name: fschat Version: 0.2.0 Summary: An open platform for
+training, serving, and evaluating large language model based chatbots. Project-
+URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
+https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE # FastChat An open platform for training, serving, and evaluating large
 language model based chatbots. ## Release
                            [assets/vicuna-logo.jpeg]
 - ð¥ We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90%
 ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and
 [demo](https://chat.lmsys.org/). [assets/demo-narrow.gif] Join our [Discord]
 (https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://
 twitter.com/lmsysorg) to get the latest updates. ## Contents - [Install]
@@ -10,138 +16,137 @@
 Interface](#inference-with-command-line-interface) - [Serving with Web GUI]
 (#serving-with-web-gui) - [Evaluation](#evaluation) - [Fine-tuning](#fine-
 tuning) ## Install ### Method 1: With pip ```bash # Install FastChat pip3
 install fschat # Install the latest main branch of huggingface/transformers
 pip3 install git+https://github.com/huggingface/transformers ``` ### Method 2:
 From source 1. Clone this repository and navigate to the FastChat folder
 ```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ``` If you
-are running on Mac: ```bash brew install rust ``` 2. Install Package ```bash
-pip3 install --upgrade pip # enable PEP 660 support pip3 install -e . ``` ##
-Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as delta
-weights to comply with the LLaMA model license. You can add our delta to the
-original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get the
-original LLaMA weights in the huggingface format by following the instructions
-[here](https://huggingface.co/docs/transformers/main/model_doc/llama). 2. Use
-the following scripts to get Vicuna weights by applying our delta. They will
-automatically download delta weights from our Hugging Face [account](https://
-huggingface.co/lmsys). **NOTE**: Our released weights are only compatible with
-the latest main branch of huggingface/transformers. We install the correct
-version of transformers when fastchat is installed. ### Vicuna-13B This
+are running on Mac: ```bash brew install rust cmake ``` 2. Install Package
+```bash pip3 install --upgrade pip # enable PEP 660 support pip3 install -e .
+``` ## Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as
+delta weights to comply with the LLaMA model license. You can add our delta to
+the original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get
+the original LLaMA weights in the huggingface format by following the
+instructions [here](https://huggingface.co/docs/transformers/main/model_doc/
+llama). 2. Use the following scripts to get Vicuna weights by applying our
+delta. They will automatically download delta weights from our Hugging Face
+[account](https://huggingface.co/lmsys). **NOTE**: Our released weights are
+only compatible with the latest main branch of huggingface/transformers. We
+install the correct version of transformers when fastchat is installed. ###
+Vicuna-7B This conversion command needs around 30 GB of CPU RAM. If you do not
+have enough memory, you can create a large swap file that allows the operating
+system to automatically utilize the disk as virtual memory. ```bash python3 -
+m fastchat.model.apply_delta \ --base /path/to/llama-7b \ --target /output/
+path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-v1.1 ``` ### Vicuna-13B This
 conversion command needs around 60 GB of CPU RAM. If you do not have enough
 memory, you can create a large swap file that allows the operating system to
 automatically utilize the disk as virtual memory. ```bash python3 -
 m fastchat.model.apply_delta \ --base /path/to/llama-13b \ --target /output/
-path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v0 ``` ### Vicuna-7B This
-conversion command needs around 30 GB of CPU RAM. If you do not have enough
-memory, you can create a large swap file that allows the operating system to
-automatically utilize the disk as virtual memory. ```bash python3 -
-m fastchat.model.apply_delta \ --base /path/to/llama-7b \ --target /output/
-path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-v0 ``` ## Inference with
-Command Line Interface #### Single GPU The command below requires around 28GB
-of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. ``` python3
--m fastchat.serve.cli --model-name /path/to/vicuna/weights ``` #### Multiple
-GPUs If you do not have enough GPU memory, you can use model parallelism to
-aggregate memory from multiple GPUs on the same machine. ``` python3 -
-m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2 ``` ####
-CPU Only This runs on the CPU only and does not require GPU. It requires around
-60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
-``` python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device
-cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
-`--device mps` to enable GPU acceleration on Mac computers and use `--load-
-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-
-name /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can run on
-a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or Other
-Platforms If you do not have enough memory, you can enable 8-bit compression by
-adding `--load-8bit` to commands above. This can reduce the memory usage by
-around half with slightly degraded model quality. It is compatible with the
-CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run on a
-single NVIDIA 3090/4090/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --
-model-name /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
+path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v1.1 ``` ### Old weights
+See [docs/weights_version.md](docs/weights_version.md) for all versions of
+weights and their differences. ## Inference with Command Line Interface
+(Experimental Feature: You can specify `--style rich` to enable rich text
+output and better text streaming quality for some non-ASCII content. This may
+not work properly on certain terminals.) #### Single GPU The command below
+requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for
+Vicuna-7B. See the "No Enough Memory" section below if you do not have enough
+memory. ``` python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
+``` #### Multiple GPUs You can use model parallelism to aggregate GPU memory
+from multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on
+the CPU only and does not require GPU. It requires around 60GB of CPU memory
+for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu ``` ####
+Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
+to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
+load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can
+run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or
+Other Platforms If you do not have enough memory, you can enable 8-bit
+compression by adding `--load-8bit` to commands above. This can reduce memory
+usage by around half with slightly degraded model quality. It is compatible
+with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
+on a single NVIDIA 3090/4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli
+--model-path /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
 exploring more methods to make the model easier to run on more platforms.
 Contributions and pull requests are welcome. ## Serving with Web GUI To serve
 using the web UI, you need three main components: web servers that interface
 with users, model workers that host one or more models, and a controller to
 coordinate the webserver and model workers. Here are the commands to follow in
-your terminal: **Note for Windows users:** Windows users will need Python 3.7
-and above and to set the following environmental variable prior to launching
-the worker. ``` PYTHONUTF8=1 ``` #### Launch the controller ```bash python3 -
+your terminal: #### Launch the controller ```bash python3 -
 m fastchat.serve.controller ``` This controller manages the distributed
 workers. #### Launch the model worker ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". You can launch multiple model workers to serve multiple models
 concurrently. The model worker will connect to the controller automatically. To
 ensure that your model worker is connected to your controller properly, send a
 test message using the following command: ```bash python3 -
 m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
 Gradio web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This
 is the user interface that users will interact with. By following these steps,
 you will be able to serve your models using the web UI. You can open your
-browser and chat with a model now. ## Evaluation Our AI-enhanced [evaluation]
-(fastchat/eval) pipeline is based on GPT-4. Here are some high-level
-instructions for using the pipeline: First, generate answers from different
-models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint
-and run `model_qa.py` for Vicuna and other models. Then, use GPT-4 to generate
-reviews automatically, which can be done manually if the GPT-4 API is not
-available to you. Once you have your evaluation data, visualize the results by
-running `generate_webpage_data_from_table.py`, which generates data for a
-static website. Finally, serve a static website under the `webpage` directory.
-You can simply use `python3 -m http.server` to serve the website locally.
-Besides the evaluation workflow, we also document the data format used for
-evaluation, which is encoded with JSON Lines and includes information on
-models, prompts, reviewers, questions, answers, and reviews. You can customize
-the evaluation process or contribute to our project by accessing relevant
-[data](fastchat/eval/table/). Check [evaluation](fastchat/eval) for detailed
-instructions. ## Fine-tuning ### Data Vicuna is created by fine-tuning a LLaMA
+browser and chat with a model now. ## Evaluation Our AI-enhanced evaluation
+pipeline is based on GPT-4. This section provides a high-level summary of the
+pipeline. For detailed instructions, please refer to the [evaluation](fastchat/
+eval) documentation. ### Pipeline Steps 1. Generate answers from different
+models: Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint
+and run `get_model_answer.py` for Vicuna and other models. 2. Generate reviews
+with GPT-4: Use GPT-4 to generate reviews automatically. This step can also be
+performed manually if the GPT-4 API is not available to you. 3. Generate
+visualization data: Run `generate_webpage_data_from_table.py` to generate data
+for a static website, which allows you to visualize the evaluation data. 4.
+Visualize the data: Serve a static website under the `webpage` directory. You
+can use `python3 -m http.server` to serve the website locally. ### Data Format
+and Contribution We use a data format encoded with JSON Lines for evaluation.
+The format includes information on models, prompts, reviewers, questions,
+answers, and reviews. You can customize the evaluation process or contribute to
+our project by accessing the relevant [data](fastchat/eval/table/). For
+detailed instructions, please refer to the [evaluation](fastchat/eval)
+documentation. ## Fine-tuning ### Data Vicuna is created by fine-tuning a LLaMA
 base model using approximately 70K user-shared conversations gathered from
 ShareGPT.com with public APIs. To ensure data quality, we convert the HTML back
 to markdown and filter out some inappropriate or low-quality samples.
 Additionally, we divide lengthy conversations into smaller segments that fit
 the model's maximum context length. For detailed instructions to clean the
 ShareGPT data, check out [here](docs/commands/data_cleaning.md). Due to some
-concerns, we may not release the data at the moment. If you would like to try
-the fine-tuning code, you can try to run it with our [preprocessed alpaca
-dataset](playground/data/alpaca-data-conversation.json) (originally from [here]
-(https://github.com/tatsu-lab/stanford_alpaca)). ### Code and Hyperparameters
-We fine-tune the model using the code from [Stanford Alpaca](https://
-github.com/tatsu-lab/stanford_alpaca), with some modifications to support
-gradient checkpointing and [Flash Attention](https://github.com/HazyResearch/
-flash-attention). We use similar hyperparameters as the Stanford Alpaca. |
-Hyperparameter | Global Batch Size | Learning rate | Epochs | Max length |
-Weight decay | | --- | ---: | ---: | ---: | ---: | ---: | | Vicuna-13B | 128 |
-2e-5 | 3 | 2048 | 0 | ### Fine-tuning on Any Cloud with SkyPilot [SkyPilot]
-(https://github.com/skypilot-org/skypilot) is a framework built by UC Berkeley
-for easily and cost effectively running ML workloads on any cloud (AWS, GCP,
-Azure, Lambda, etc.). To use SkyPilot, install it with the following command
-and setup the cloud credentials locally following the instructions [here]
-(https://skypilot.readthedocs.io/en/latest/getting-started/installation.html).
-```bash # Install skypilot from the master branch pip install git+https://
-github.com/skypilot-org/skypilot.git ``` #### Vicuna Vicuna can be trained on 8
-A100 GPUs with 80GB memory. The following command will automatically launch a
-node satisfying the requirement, setup and run the training job on it. ```bash
-sky launch -c vicuna -s scripts/train-vicuna.yaml --env WANDB_API_KEY ``` Other
-options are also valid: ```bash # Launch it on managed spot to save 3x cost
-(train Vicuna-13B with around $300) sky spot launch -n vicuna scripts/train-
-vicuna.yaml --env WANDB_API_KEY # Train a 7B model sky launch -c vicuna -
-s scripts/train-vicuna.yaml --env WANDB_API_KEY --env MODEL_SIZE=7 ``` Note:
-Please make sure the `WANDB_API_KEY` has been setup on your local machine. You
-can find the API key on your [wandb profile page](https://wandb.ai/authorize).
-If you would like to train the model without using wandb, you can replace the
-`--env WANDB_API_KEY` flag with `--env WANDB_MODE=offline`. #### Alpaca Launch
-the training job with the following line (will be launched on a single node
-with 4 A100-80GB GPUs) ``` sky launch -c alpaca -s scripts/train-alpaca.yaml --
-env WANDB_API_KEY ``` ### Fine-tuning with Local GPUs Vicuna can also be
-trained on 8 A100 GPUs with 80GB memory with the following code. To train on
-fewer GPUs, you can reduce the `per_device_train_batch_size` and increase the
-`gradient_accumulation_steps` accordingly to keep the global batch size the
-same. To setup the environment, please see the setup section in [scripts/train-
-vicuna.yaml](scripts/train-vicuna.yaml). ```bash torchrun --nnodes=1 --
-nproc_per_node=8 --master_port= \ fastchat/train/train_mem.py \ --
-model_name_or_path  \ --data_path  \ --bf16 True \ --output_dir ./checkpoints \
---num_train_epochs 3 \ --per_device_train_batch_size 4 \ --
-per_device_eval_batch_size 4 \ --gradient_accumulation_steps 1 \ --
+concerns, we may not release the ShareGPT dataset at the moment. If you would
+like to try the fine-tuning code, you can run it with some dummy questions in
+[dummy.json](playground/data/dummy.json). You can follow the same format and
+plug in your own data. ### Code and Hyperparameters Our code is based on
+[Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) with additional
+support for multi-round conversations. We use similar hyperparameters as the
+Stanford Alpaca. | Hyperparameter | Global Batch Size | Learning rate | Epochs
+| Max length | Weight decay | | --- | ---: | ---: | ---: | ---: | ---: | |
+Vicuna-13B | 128 | 2e-5 | 3 | 2048 | 0 | ### Fine-tuning Vicuna-7B with Local
+GPUs You can use the following command to train Vicuna-7B with 4 x A100 (40GB).
+```bash torchrun --nproc_per_node=4 --master_port=20001 fastchat/train/
+train_mem.py \ --model_name_or_path ~/model_weights/llama-7b \ --data_path
+playground/data/dummy.json \ --bf16 True \ --output_dir output \ --
+num_train_epochs 3 \ --per_device_train_batch_size 2 \ --
+per_device_eval_batch_size 2 \ --gradient_accumulation_steps 16 \ --
 evaluation_strategy "no" \ --save_strategy "steps" \ --save_steps 1200 \ --
-save_total_limit 100 \ --learning_rate 2e-5 \ --weight_decay 0. \ --
-warmup_ratio 0.03 \ --lr_scheduler_type "cosine" \ --logging_steps 1 \ --fsdp
-"full_shard auto_wrap" \ --fsdp_transformer_layer_cls_to_wrap
-'LlamaDecoderLayer' \ --tf32 True \ --model_max_length 2048 \ --
-gradient_checkpointing True \ --lazy_preprocess True ```
+save_total_limit 10 \ --learning_rate 2e-5 \ --weight_decay 0. \ --warmup_ratio
+0.03 \ --lr_scheduler_type "cosine" \ --logging_steps 1 \ --fsdp "full_shard
+auto_wrap" \ --fsdp_transformer_layer_cls_to_wrap 'LlamaDecoderLayer' \ --tf32
+True \ --model_max_length 2048 \ --gradient_checkpointing True \ --
+lazy_preprocess True ``` If you meet out-of-memory during model saving, see
+solutions [here](https://github.com/pytorch/pytorch/issues/98823). ### Fine-
+tuning on Any Cloud with SkyPilot [SkyPilot](https://github.com/skypilot-org/
+skypilot) is a framework built by UC Berkeley for easily and cost effectively
+running ML workloads on any cloud (AWS, GCP, Azure, Lambda, etc.). To use
+SkyPilot, install it with the following command and setup the cloud credentials
+locally following the instructions [here](https://skypilot.readthedocs.io/en/
+latest/getting-started/installation.html). ```bash # Install skypilot from the
+master branch pip install git+https://github.com/skypilot-org/skypilot.git ```
+#### Vicuna Vicuna can be trained on 8 A100 GPUs with 80GB memory. The
+following command will automatically launch a node satisfying the requirement,
+setup and run the training job on it. ```bash sky launch -c vicuna -s scripts/
+train-vicuna.yaml --env WANDB_API_KEY ``` Other options are also valid: ```bash
+# Launch it on managed spot to save 3x cost (train Vicuna-13B with around $300)
+sky spot launch -n vicuna scripts/train-vicuna.yaml --env WANDB_API_KEY # Train
+a 7B model sky launch -c vicuna -s scripts/train-vicuna.yaml --env
+WANDB_API_KEY --env MODEL_SIZE=7 ``` Note: Please make sure the `WANDB_API_KEY`
+has been setup on your local machine. You can find the API key on your [wandb
+profile page](https://wandb.ai/authorize). If you would like to train the model
+without using wandb, you can replace the `--env WANDB_API_KEY` flag with `--env
+WANDB_MODE=offline`.
```

### Comparing `fschat-0.1.9/fastchat/conversation.py` & `fschat-0.2.0/fastchat/conversation.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,25 +16,26 @@
     roles: List[str]
     messages: List[List[str]]
     offset: int
     sep_style: SeparatorStyle = SeparatorStyle.SINGLE
     sep: str = "###"
     sep2: str = None
 
+    # Used for gradio server
     skip_next: bool = False
     conv_id: Any = None
 
     def get_prompt(self):
         if self.sep_style == SeparatorStyle.SINGLE:
-            ret = self.system + self.sep
+            ret = self.system
             for role, message in self.messages:
                 if message:
-                    ret += role + ": " + message + self.sep
+                    ret += self.sep + " " + role + ": " + message
                 else:
-                    ret += role + ":"
+                    ret += self.sep + " " + role + ":"
             return ret
         elif self.sep_style == SeparatorStyle.TWO:
             seps = [self.sep, self.sep2]
             ret = self.system + seps[0]
             for i, (role, message) in enumerate(self.messages):
                 if message:
                     ret += role + ": " + message + seps[i % 2]
@@ -75,42 +76,15 @@
             "offset": self.offset,
             "sep": self.sep,
             "sep2": self.sep2,
             "conv_id": self.conv_id,
         }
 
 
-conv_v1 = Conversation(
-    system="A chat between a curious human and an artificial intelligence assistant. "
-           "The assistant gives helpful, detailed, and polite answers to the human's questions.",
-    roles=("Human", "Assistant"),
-    messages=(
-        ("Human", "Give three tips for staying healthy."),
-        ("Assistant",
-            "Sure, here are three tips for staying healthy:\n"
-            "1. Exercise regularly: Regular physical activity can help improve your overall health and wellbeing. "
-            "It can also help reduce your risk of chronic conditions such as obesity, diabetes, heart disease, "
-            "and certain cancers. Aim for at least 150 minutes of moderate-intensity aerobic exercise or "
-            "75 minutes of vigorous-intensity aerobic exercise per week, along with muscle-strengthening "
-            "activities at least two days per week.\n"
-            "2. Eat a balanced diet: Eating a balanced diet that is rich in fruits, "
-            "vegetables, whole grains, lean proteins, and healthy fats can help support "
-            "your overall health. Try to limit your intake of processed and high-sugar foods, "
-            "and aim to drink plenty of water throughout the day.\n"
-            "3. Get enough sleep: Getting enough quality sleep is essential for your physical "
-            "and mental health. Adults should aim for seven to nine hours of sleep per night. "
-            "Establish a regular sleep schedule and try to create a relaxing bedtime routine to "
-            "help improve the quality of your sleep.")
-    ),
-    offset=2,
-    sep_style=SeparatorStyle.SINGLE,
-    sep="###",
-)
-
-conv_v1_2 = Conversation(
+conv_one_shot = Conversation(
     system="A chat between a curious human and an artificial intelligence assistant. "
            "The assistant gives helpful, detailed, and polite answers to the human's questions.",
     roles=("Human", "Assistant"),
     messages=(
         ("Human", "What are the key differences between renewable and non-renewable energy sources?"),
         ("Assistant",
             "Renewable energy sources are those that can be replenished naturally in a relatively "
@@ -126,34 +100,56 @@
             "3. Cost: Renewable energy sources can be more expensive to initially set up, but they typically "
             "have lower operational costs than non-renewable sources.\n"
             "4. Reliability: Renewable energy sources are often more reliable and can be used in more remote "
             "locations than non-renewable sources.\n"
             "5. Flexibility: Renewable energy sources are often more flexible and can be adapted to different "
             "situations and needs, while non-renewable sources are more rigid and inflexible.\n"
             "6. Sustainability: Renewable energy sources are more sustainable over the long term, while "
-            "non-renewable sources are not, and their depletion can lead to economic and social instability.\n")
+            "non-renewable sources are not, and their depletion can lead to economic and social instability.")
     ),
     offset=2,
     sep_style=SeparatorStyle.SINGLE,
     sep="###",
 )
 
-conv_bair_v1 = Conversation(
+
+conv_vicuna_v1_1 = Conversation(
+    system="A chat between a curious user and an artificial intelligence assistant. "
+           "The assistant gives helpful, detailed, and polite answers to the user's questions.",
+    roles=("USER", "ASSISTANT"),
+    messages=(),
+    offset=0,
+    sep_style=SeparatorStyle.TWO,
+    sep=" ",
+    sep2="</s>",
+)
+
+
+conv_koala_v1 = Conversation(
     system="BEGINNING OF CONVERSATION:",
     roles=("USER", "GPT"),
     messages=(),
     offset=0,
     sep_style=SeparatorStyle.TWO,
     sep=" ",
     sep2="</s>",
 )
 
 
-default_conversation = conv_v1_2
 conv_templates = {
-    "v1": conv_v1_2,
-    "bair_v1": conv_bair_v1,
+    "conv_one_shot": conv_one_shot,
+    "vicuna_v1.1": conv_vicuna_v1_1,
+    "koala_v1": conv_koala_v1,
 }
 
 
+def get_default_conv_template(model_name):
+    model_name = model_name.lower()
+    if "vicuna" in model_name or "output" in model_name:
+        return conv_vicuna_v1_1
+    elif "koala" in model_name:
+        return conv_koala_v1
+    return conv_one_shot
+
+
 if __name__ == "__main__":
     print(default_conversation.get_prompt())
```

### Comparing `fschat-0.1.9/fastchat/data/alpaca-converter.py` & `fschat-0.2.0/fastchat/data/alpaca-converter.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/data/clean_sharegpt.py` & `fschat-0.2.0/fastchat/data/clean_sharegpt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Convert html to markdown with basic data cleaning.
+- Convert html to markdown with basic data cleaning.
+- Deduplication.
 
 Usage:
 python3 -m fastchat.data.clean_sharegpt --in sharegpt_html.json --out sharegpt_clean.json
 """
 import argparse
 import json
 import logging
@@ -19,14 +20,15 @@
 span_pattern = re.compile("<span.*?>")
 code_lang_pattern = re.compile("```\s*" + "(.*?)" + "(?:Copy code)+" + "(.+?)" + "\s*?```", re.DOTALL)
 code_lang_format = "```\g<1>\n\g<2>\n```"
 regenerate_pattern = re.compile("\d+ / \d+")
 copy_chars_pattern = re.compile("Copy\d+ chars / \d+ words")
 copy_code_pattern = re.compile("```(.*?)Copy code\s*```")
 
+
 def reformat_code(val: str) -> str:
     # Input code format is:
     # ```
     # $<language>Copy code$<exact_code_here>
     #
     # ```
     # This function convert it into the correct markdown format
@@ -58,73 +60,98 @@
     if args.debug:
         print(val)
         exit()
 
     return val
 
 
-def should_skip(val: str) -> bool:
+def should_filter(val: str) -> bool:
     black_list = ["openai", "chatgpt"]
     for w in black_list:
         if w in val.lower():
             return True
     return False
 
 
 def clean_html_source(content, begin, end, check_tag, check_num):
     """
-    clean the input json content.
+    Clean the input json content.
+
     Args:
         content: json file loaded in memory.
         check_tag: a debug purpose arg. If a conversation contains the tag, log
           it before and after cleaning.
         check_num: number of matched conversations logged.
     """
     BARRIER = "\n" + "=" * 20 + "\n"
-    skip_cnt = 0
-    tag_cnt = 0
+    cnt_skip = 0
+    cnt_too_short = 0
+    cnt_id_duplication = 0
+    cnt_value_duplication = 0
+    cnt_filter = 0
+    cnt_tag = 0
+    visited = {}
 
     content = content[begin:end]
     new_content = []
 
     for sample in tqdm.tqdm(content):
         skipped = False
+        cid = sample["id"]
 
         if len(sample["conversations"]) <= 1:
-            # The conversation is too short
+            print(f"id {cid} is too short")
+            cnt_too_short += 1
+            skipped = True
+        elif cid in visited:
+            print(f"id {cid} is an id duplication of {visited[cid]}")
+            cnt_id_duplication += 1
+            skipped = True
+        elif (sample["conversations"][1]["value"], len(sample["conversations"])) in visited:
+            key = (sample["conversations"][1]["value"], len(sample["conversations"]))
+            print(f"id {cid} is a value duplication of {visited[key]}")
+            cnt_value_duplication += 1
             skipped = True
         else:
+            key = (sample["conversations"][1]["value"], len(sample["conversations"]))
+            visited[cid] = visited[key] = cid
+
             for c in sample["conversations"]:
-                if should_skip(c["value"]):
+                if should_filter(c["value"]):
+                    print(f"id {cid} is filtered out")
+                    cnt_filter += 1
                     skipped = True
                     break
 
                 try:
                     new_val = html_to_markdown(c["value"])
                 except (bs4.builder.ParserRejectedMarkup, AssertionError):
                     skipped = True
                     break
 
                 c["value"] = new_val
 
                 # Debug
                 if (check_tag is not None and check_tag in c["value"]
-                        and tag_cnt < check_num):
+                        and cnt_tag < check_num):
                     logging.debug(BARRIER + c["value"] + "\n" + BARRIER + new_val +
                                   "\n" + BARRIER + "\n")
-                    tag_cnt += 1
-                    if tag_cnt == check_num:
+                    cnt_tag += 1
+                    if cnt_tag == check_num:
                         break
 
         if not skipped:
             new_content.append(sample)
         else:
-            skip_cnt += 1
+            cnt_skip += 1
+
+    print(f"total: {len(content)}, skip: {cnt_skip}, new: {len(new_content)}, "
+          f"cnt_too_short: {cnt_too_short}, cnt_id_duplication: {cnt_id_duplication}, "
+          f"cnt_value_duplication: {cnt_value_duplication}, cnt_filter: {cnt_filter}")
 
-    print(f"total: {len(content)}, skip: {skip_cnt}, new: {len(new_content)}")
     return new_content
 
 
 def main(args):
     content = json.load(open(args['in_file'], "r"))
     content = clean_html_source(
         content, args['begin'], args['end'],
```

### Comparing `fschat-0.1.9/fastchat/data/inspect.py` & `fschat-0.2.0/fastchat/data/inspect.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/data/optional_clean.py` & `fschat-0.2.0/fastchat/data/optional_clean.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/eval/eval_gpt_review.py` & `fschat-0.2.0/fastchat/eval/eval_gpt_review.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/eval/generate_webpage_data_from_table.py` & `fschat-0.2.0/fastchat/eval/generate_webpage_data_from_table.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/eval/get_model_answer.py` & `fschat-0.2.0/fastchat/eval/get_model_answer.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch
 import os
 import json
 from tqdm import tqdm
 import shortuuid
 import ray
 
-from fastchat.conversation import default_conversation
+from fastchat.conversation import get_default_conv_template
 from fastchat.utils import disable_torch_init
 
 
 def run_eval(model_path, model_id, question_file, answer_file, num_gpus):
     # split question file into num_gpus files
     ques_jsons = []
     with open(os.path.expanduser(question_file), "r") as ques_file:
@@ -33,40 +33,37 @@
 
 
 @ray.remote(num_gpus=1)
 @torch.inference_mode()
 def get_model_answers(model_path, model_id, question_jsons):
     disable_torch_init()
     model_path = os.path.expanduser(model_path)
-    tokenizer = AutoTokenizer.from_pretrained(model_path)
+    tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
     model = AutoModelForCausalLM.from_pretrained(model_path,
         torch_dtype=torch.float16).cuda()
 
     ans_jsons = []
     for i, line in enumerate(tqdm(question_jsons)):
         ques_json = json.loads(line)
         idx = ques_json["question_id"]
         qs = ques_json["text"]
-        conv = default_conversation.copy()
+        conv = get_default_conv_template(model_id).copy()
         conv.append_message(conv.roles[0], qs)
+        conv.append_message(conv.roles[1], None)
         prompt = conv.get_prompt()
         inputs = tokenizer([prompt])
         output_ids = model.generate(
             torch.as_tensor(inputs.input_ids).cuda(),
             do_sample=True,
             temperature=0.7,
             max_new_tokens=1024)
         outputs = tokenizer.batch_decode(output_ids, skip_special_tokens=True)[0]
-        try:
-            index = outputs.index(conv.sep, len(prompt))
-        except ValueError:
-            outputs += conv.sep
-            index = outputs.index(conv.sep, len(prompt))
+        skip_echo_len = len(prompt.replace("</s>", " ")) + 1
 
-        outputs = outputs[len(prompt) + len(conv.roles[1]) + 2:index].strip()
+        outputs = outputs[skip_echo_len:].strip()
         ans_id = shortuuid.uuid()
         ans_jsons.append({"question_id": idx,
                           "text": outputs,
                           "answer_id": ans_id,
                           "model_id": model_id,
                           "metadata": {}})
     return ans_jsons
```

### Comparing `fschat-0.1.9/fastchat/eval/qa_baseline_gpt35.py` & `fschat-0.2.0/fastchat/eval/qa_baseline_gpt35.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/model/apply_delta.py` & `fschat-0.2.0/fastchat/model/make_delta.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,43 @@
 """
-Apply the delta weights on top of a base model.
+Make the delta weights by subtracting base weights.
 
 Usage:
-python3 -m fastchat.model.apply_delta --base ~/model_weights/llama-13b --target ~/model_weights/vicuna-13b --delta lmsys/vicuna-13b-delta
+python3 -m fastchat.model.make_delta --base ~/model_weights/llama-13b --target ~/model_weights/vicuna-13b --delta ~/model_weights/vicuna-13b-delta --hub-repo-id lmsys/vicuna-13b-delta-v1.1
 """
 import argparse
 
 import torch
 from tqdm import tqdm
 from transformers import AutoTokenizer, AutoModelForCausalLM
 
 
-def apply_delta(base_model_path, target_model_path, delta_path):
+def make_delta(base_model_path, target_model_path, delta_path):
     print(f"Loading the base model from {base_model_path}")
     base = AutoModelForCausalLM.from_pretrained(
         base_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True)
 
-    print(f"Loading the delta from {delta_path}")
-    delta = AutoModelForCausalLM.from_pretrained(delta_path, torch_dtype=torch.float16, low_cpu_mem_usage=True)
-    delta_tokenizer = AutoTokenizer.from_pretrained(delta_path, use_fast=False)
-
-    DEFAULT_PAD_TOKEN = "[PAD]"
-    base_tokenizer = AutoTokenizer.from_pretrained(base_model_path, use_fast=False)
-    num_new_tokens = base_tokenizer.add_special_tokens(dict(pad_token=DEFAULT_PAD_TOKEN))
-
-    base.resize_token_embeddings(len(base_tokenizer))
-    input_embeddings = base.get_input_embeddings().weight.data
-    output_embeddings = base.get_output_embeddings().weight.data
-    input_embeddings[-num_new_tokens:] = 0
-    output_embeddings[-num_new_tokens:] = 0
-
-    print("Applying the delta")
-    for name, param in tqdm(base.state_dict().items(), desc="Applying delta"):
-        assert name in delta.state_dict()
-        param.data += delta.state_dict()[name]
-
-    print(f"Saving the target model to {target_model_path}")
-    base.save_pretrained(target_model_path)
-    delta_tokenizer.save_pretrained(target_model_path)
+    print(f"Loading the target model from {target_model_path}")
+    target = AutoModelForCausalLM.from_pretrained(target_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True)
+
+    print("Calculating the delta")
+    for name, param in tqdm(target.state_dict().items(), desc="Calculating delta"):
+        assert name in base.state_dict()
+        param.data -= base.state_dict()[name]
+
+    print(f"Saving the delta to {delta_path}")
+    if args.hub_repo_id:
+        kwargs = {"push_to_hub": True, "repo_id": args.hub_repo_id}
+    else:
+        kwargs = {}
+    target.save_pretrained(delta_path, **kwargs)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--base-model-path", type=str, required=True)
     parser.add_argument("--target-model-path", type=str, required=True)
     parser.add_argument("--delta-path", type=str, required=True)
-
+    parser.add_argument("--hub-repo-id", type=str)
     args = parser.parse_args()
 
-    apply_delta(args.base_model_path, args.target_model_path, args.delta_path)
+    make_delta(args.base_model_path, args.target_model_path, args.delta_path)
```

### Comparing `fschat-0.1.9/fastchat/serve/compression.py` & `fschat-0.2.0/fastchat/serve/compression.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/serve/controller.py` & `fschat-0.2.0/fastchat/serve/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
                 "text": server_error_msg,
                 "error_code": 2,
             }
             yield json.dumps(ret).encode() + b"\0"
 
         try:
             response = requests.post(worker_addr + "/worker_generate_stream",
-                json=params, stream=True, timeout=5)
+                json=params, stream=True, timeout=15)
             for chunk in response.iter_lines(decode_unicode=False, delimiter=b"\0"):
                 if chunk:
                     yield chunk + b"\0"
         except requests.exceptions.RequestException as e:
             logger.info(f"worker timeout: {worker_addr}")
             ret = {
                 "text": server_error_msg,
```

### Comparing `fschat-0.1.9/fastchat/serve/gradio_css.py` & `fschat-0.2.0/fastchat/serve/gradio_css.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/serve/gradio_patch.py` & `fschat-0.2.0/fastchat/serve/gradio_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/serve/gradio_web_server.py` & `fschat-0.2.0/fastchat/serve/gradio_web_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import time
 import uuid
 
 import gradio as gr
 import requests
 
-from fastchat.conversation import (default_conversation, conv_templates,
+from fastchat.conversation import (get_default_conv_template,
                                    SeparatorStyle)
 from fastchat.constants import LOGDIR
 from fastchat.utils import (build_logger, server_error_msg,
     violates_moderation, moderation_msg)
 from fastchat.serve.gradio_patch import Chatbot as grChatbot
 from fastchat.serve.gradio_css import code_highlight_css
 
@@ -25,14 +25,15 @@
 no_change_btn = gr.Button.update()
 enable_btn = gr.Button.update(interactive=True)
 disable_btn = gr.Button.update(interactive=False)
 
 priority = {
     "vicuna-13b": "aaaaaaa",
     "koala-13b": "aaaaaab",
+    "chatglm-6b": "aaaaaac",
 }
 
 
 def get_conv_log_filename():
     t = datetime.datetime.now()
     name = os.path.join(LOGDIR, f"{t.year}-{t.month:02d}-{t.day:02d}-conv.json")
     return name
@@ -64,28 +65,28 @@
     dropdown_update = gr.Dropdown.update(visible=True)
     if "model" in url_params:
         model = url_params["model"]
         if model in models:
             dropdown_update = gr.Dropdown.update(
                 value=model, visible=True)
 
-    state = default_conversation.copy()
+    state = None
     return (state,
             dropdown_update,
             gr.Chatbot.update(visible=True),
             gr.Textbox.update(visible=True),
             gr.Button.update(visible=True),
             gr.Row.update(visible=True),
             gr.Accordion.update(visible=True))
 
 
 def load_demo_refresh_model_list(request: gr.Request):
     logger.info(f"load_demo. ip: {request.client.host}")
     models = get_model_list()
-    state = default_conversation.copy()
+    state = None
     return (state, gr.Dropdown.update(
                choices=models,
                value=models[0] if len(models) > 0 else ""),
             gr.Chatbot.update(visible=True),
             gr.Textbox.update(visible=True),
             gr.Button.update(visible=True),
             gr.Row.update(visible=True),
@@ -127,30 +128,33 @@
     state.messages[-1][-1] = None
     state.skip_next = False
     return (state, state.to_gradio_chatbot(), "") + (disable_btn,) * 5
 
 
 def clear_history(request: gr.Request):
     logger.info(f"clear_history. ip: {request.client.host}")
-    state = default_conversation.copy()
-    return (state, state.to_gradio_chatbot(), "") + (disable_btn,) * 5
+    state = None
+    return (state, [], "") + (disable_btn,) * 5
 
 
 def add_text(state, text, request: gr.Request):
     logger.info(f"add_text. ip: {request.client.host}. len: {len(text)}")
     if len(text) <= 0:
         state.skip_next = True
         return (state, state.to_gradio_chatbot(), "") + (no_change_btn,) * 5
     if args.moderate:
         flagged = violates_moderation(text)
         if flagged:
             state.skip_next = True
             return (state, state.to_gradio_chatbot(), moderation_msg) + (
                 no_change_btn,) * 5
 
+    if state is None:
+        state = get_default_conv_template("vicuna").copy()
+
     text = text[:1536]  # Hard cut-off
     state.append_message(state.roles[0], text)
     state.append_message(state.roles[1], None)
     state.skip_next = False
     return (state, state.to_gradio_chatbot(), "") + (disable_btn,) * 5
 
 
@@ -173,19 +177,15 @@
     if state.skip_next:
         # This generate call is skipped due to invalid inputs
         yield (state, state.to_gradio_chatbot()) + (no_change_btn,) * 5
         return
 
     if len(state.messages) == state.offset + 2:
         # First round of conversation
-        if "koala" in model_name: # Hardcode the condition
-            template_name = "bair_v1"
-        else:
-            template_name = "v1"
-        new_state = conv_templates[template_name].copy()
+        new_state = get_default_conv_template(model_name).copy()
         new_state.conv_id = uuid.uuid4().hex
         new_state.append_message(new_state.roles[0], state.messages[-2][1])
         new_state.append_message(new_state.roles[1], None)
         state = new_state
 
     # Query worker address
     controller_url = args.controller_url
@@ -202,15 +202,15 @@
 
     # Construct prompt
     if "chatglm" in model_name:
         prompt = state.messages[state.offset:]
         skip_echo_len = len(state.messages[-2][1]) + 1
     else:
         prompt = state.get_prompt()
-        skip_echo_len = len(prompt) + 1
+        skip_echo_len = len(prompt.replace("</s>", " ")) + 1
 
     # Make requests
     pload = {
         "model": model_name,
         "prompt": prompt,
         "temperature": float(temperature),
         "max_new_tokens": int(max_new_tokens),
@@ -220,15 +220,15 @@
 
     state.messages[-1][-1] = "▌"
     yield (state, state.to_gradio_chatbot()) + (disable_btn,) * 5
 
     try:
         # Stream output
         response = requests.post(worker_addr + "/worker_generate_stream",
-            headers=headers, json=pload, stream=True, timeout=10)
+            headers=headers, json=pload, stream=True, timeout=20)
         for chunk in response.iter_lines(decode_unicode=False, delimiter=b"\0"):
             if chunk:
                 data = json.loads(chunk.decode())
                 if data["error_code"] == 0:
                     output = data["text"][skip_echo_len:].strip()
                     output = post_process_code(output)
                     state.messages[-1][-1] = output + "▌"
@@ -271,15 +271,15 @@
 
 ### Terms of use
 By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. The service may collect user dialogue data for future research.
 
 ### Choose a model to chat with
 - [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations. This one is expected to perform best according to our evaluation.
 - [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a chatbot fine-tuned from LLaMA on user-shared conversations and open-source datasets. This one performs similarly to Vicuna.
-- [ChatGLM](https://chatglm.cn/blog): An Open Bilingual Dialogue Language Model | 开源双语对话语言模型
+- [ChatGLM](https://chatglm.cn/blog): an open bilingual dialogue language model | 开源双语对话语言模型
 - [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on 52K instruction-following demonstrations.
 - [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models
 
 Note: If you are waiting in the queue, check out more benchmark results from GPT-4 on a static website [here](https://vicuna.lmsys.org/eval).
 """)
```

### Comparing `fschat-0.1.9/fastchat/serve/model_worker.py` & `fschat-0.2.0/fastchat/serve/model_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 from typing import List, Union
 import threading
 import uuid
 
 from fastapi import FastAPI, Request, BackgroundTasks
 from fastapi.responses import StreamingResponse
 import requests
-from transformers import AutoTokenizer, AutoModelForCausalLM, LlamaTokenizer
+try:
+    from transformers import AutoTokenizer, AutoModelForCausalLM, LlamaTokenizer, AutoModel
+except ImportError:
+    from transformers import AutoTokenizer, AutoModelForCausalLM, LLaMATokenizer, AutoModel
 import torch
 import uvicorn
 
 from fastchat.constants import WORKER_HEART_BEAT_INTERVAL
-from fastchat.serve.cli import load_model, generate_stream
+from fastchat.serve.inference import load_model, generate_stream
 from fastchat.serve.serve_chatglm import chatglm_generate_stream
 from fastchat.utils import (build_logger, server_error_msg,
     pretty_print_semaphore)
 
 GB = 1 << 30
 
 worker_id = str(uuid.uuid4())[:6]
@@ -105,15 +108,15 @@
                 logger.error(f"heart beat error: {e}")
             time.sleep(5)
 
         if not exist:
             self.register_to_controller()
 
     def get_queue_length(self):
-        if model_semaphore is None:
+        if model_semaphore is None or model_semaphore._value is None or model_semaphore._waiters is None:
             return 0
         else:
             return args.limit_model_concurrency - model_semaphore._value + len(
                 model_semaphore._waiters)
 
     def get_status(self):
         return {
@@ -170,16 +173,18 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--port", type=int, default=21002)
     parser.add_argument("--worker-address", type=str,
         default="http://localhost:21002")
     parser.add_argument("--controller-address", type=str,
         default="http://localhost:21001")
-    parser.add_argument("--model-path", type=str, default="facebook/opt-350m")
-    parser.add_argument("--model-name", type=str)
+    parser.add_argument("--model-path", type=str, default="facebook/opt-350m",
+        help="The path to the weights")
+    parser.add_argument("--model-name", type=str,
+        help="Optional name")
     parser.add_argument("--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda")
     parser.add_argument("--num-gpus", type=int, default=1)
     parser.add_argument("--load-8bit", action="store_true")
     parser.add_argument("--limit-model-concurrency", type=int, default=5)
     parser.add_argument("--stream-interval", type=int, default=2)
     parser.add_argument("--no-register", action="store_true")
     args = parser.parse_args()
```

### Comparing `fschat-0.1.9/fastchat/serve/monkey_patch_non_inplace.py` & `fschat-0.2.0/fastchat/serve/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/serve/register_worker.py` & `fschat-0.2.0/fastchat/serve/register_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/serve/serve_chatglm.py` & `fschat-0.2.0/fastchat/serve/serve_chatglm.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/serve/test_message.py` & `fschat-0.2.0/fastchat/serve/test_message.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 import argparse
 import json
 
 import requests
 
-from fastchat.conversation import default_conversation
+from fastchat.conversation import get_default_conv_template, SeparatorStyle
 
 
 def main():
+    model_name = args.model_name
+
     if args.worker_address:
         worker_addr = args.worker_address
     else:
         controller_addr = args.controller_address
         ret = requests.post(controller_addr + "/refresh_all_workers")
         ret = requests.post(controller_addr + "/list_models")
         models = ret.json()["models"]
         models.sort()
         print(f"Models: {models}")
 
         ret = requests.post(controller_addr + "/get_worker_address",
-            json={"model": args.model_name})
+            json={"model": model_name})
         worker_addr = ret.json()["address"]
         print(f"worker_addr: {worker_addr}")
 
     if worker_addr == "":
         return
 
-    conv = default_conversation.copy()
+    conv = get_default_conv_template(model_name).copy()
     conv.append_message(conv.roles[0], args.message)
+    conv.append_message(conv.roles[1], None)
     prompt = conv.get_prompt()
 
     headers = {"User-Agent": "fastchat Client"}
     pload = {
-        "model": args.model_name,
+        "model": model_name,
         "prompt": prompt,
         "max_new_tokens": args.max_new_tokens,
-        "temperature": 0.7,
-        "stop": conv.sep,
+        "temperature": args.temperature,
+        "stop": conv.sep if conv.sep_style == SeparatorStyle.SINGLE else conv.sep2,
     }
     response = requests.post(worker_addr + "/worker_generate_stream", headers=headers,
             json=pload, stream=True)
 
-    print(prompt.replace(conv.sep, "\n"), end="")
+    print(f"{conv.roles[0]}: {args.message}")
     for chunk in response.iter_lines(chunk_size=8192, decode_unicode=False, delimiter=b"\0"):
         if chunk:
             data = json.loads(chunk.decode("utf-8"))
-            output = data["text"].split(conv.sep)[-1]
-            print(output, end="\r")
+            skip_echo_len = len(prompt.replace("</s>", " ")) + 1
+            output = data["text"][skip_echo_len:].strip()
+            print(f"{conv.roles[1]}: {output}", end="\r")
     print("")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--controller-address", type=str, default="http://localhost:21001")
     parser.add_argument("--worker-address", type=str)
     parser.add_argument("--model-name", type=str, default="facebook/opt-350m")
+    parser.add_argument("--temperature", type=float, default=0.0)
     parser.add_argument("--max-new-tokens", type=int, default=32)
     parser.add_argument("--message", type=str, default=
         "Tell me a story with more than 1000 words.")
     args = parser.parse_args()
 
     main()
```

### Comparing `fschat-0.1.9/fastchat/train/llama_flash_attn_monkey_patch.py` & `fschat-0.2.0/fastchat/train/llama_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/train/train_lora.py` & `fschat-0.2.0/fastchat/train/train_lora.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fastchat/utils.py` & `fschat-0.2.0/fastchat/utils.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.9/fschat.egg-info/PKG-INFO` & `fschat-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: fschat
-Version: 0.1.9
-Summary: An open platform for training, serving, and evaluating large language model based chatbots.
-Project-URL: Homepage, https://github.com/lm-sys/fastchat
-Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # FastChat
 An open platform for training, serving, and evaluating large language model based chatbots.
 
 ## Release
 
 <p align="center">
 <a href="https://vicuna.lmsys.org"><img src="assets/vicuna-logo.jpeg" width="20%"></a>
@@ -51,15 +39,15 @@
 ```bash
 git clone https://github.com/lm-sys/FastChat.git
 cd FastChat
 ```
 
 If you are running on Mac:
 ```bash
-brew install rust
+brew install rust cmake
 ```
 
 2. Install Package
 ```bash
 pip3 install --upgrade pip  # enable PEP 660 support
 pip3 install -e .
 ```
@@ -71,84 +59,85 @@
 1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
 2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
 Our released weights are only compatible with the latest main branch of huggingface/transformers.
 We install the correct version of transformers when fastchat is installed.
 
-### Vicuna-13B
-This conversion command needs around 60 GB of CPU RAM.
+### Vicuna-7B
+This conversion command needs around 30 GB of CPU RAM.
 If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
-    --base /path/to/llama-13b \
-    --target /output/path/to/vicuna-13b \
-    --delta lmsys/vicuna-13b-delta-v0
+    --base /path/to/llama-7b \
+    --target /output/path/to/vicuna-7b \
+    --delta lmsys/vicuna-7b-delta-v1.1
 ```
 
-### Vicuna-7B
-This conversion command needs around 30 GB of CPU RAM.
+### Vicuna-13B
+This conversion command needs around 60 GB of CPU RAM.
 If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
-    --base /path/to/llama-7b \
-    --target /output/path/to/vicuna-7b \
-    --delta lmsys/vicuna-7b-delta-v0
+    --base /path/to/llama-13b \
+    --target /output/path/to/vicuna-13b \
+    --delta lmsys/vicuna-13b-delta-v1.1
 ```
 
+### Old weights
+See [docs/weights_version.md](docs/weights_version.md) for all versions of weights and their differences.
+
 ## Inference with Command Line Interface
 
+(Experimental Feature: You can specify `--style rich` to enable rich text output and better text streaming quality for some non-ASCII content. This may not work properly on certain terminals.)
+
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
+See the "No Enough Memory" section below if you do not have enough memory.
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
 ```
 
 #### Multiple GPUs
-If you do not have enough GPU memory, you can use model parallelism to aggregate memory from multiple GPUs on the same machine.
+You can use model parallelism to aggregate GPU memory from multiple GPUs on the same machine.
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --num-gpus 2
 ```
 
 #### CPU Only
 This runs on the CPU only and does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device cpu
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu
 ```
 
 #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs)
-Use `--device mps` to enable GPU acceleration on Mac computers and use `--load-8bit` to turn on 8-bit compression.
+Use `--device mps` to enable GPU acceleration on Mac computers (requires torch >= 2.0).
+Use `--load-8bit` to turn on 8-bit compression.
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device mps --load-8bit
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --device mps --load-8bit
 ```
 Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second.
 
 #### No Enough Memory or Other Platforms
 If you do not have enough memory, you can enable 8-bit compression by adding `--load-8bit` to commands above.
-This can reduce the memory usage by around half with slightly degraded model quality.
+This can reduce memory usage by around half with slightly degraded model quality.
 It is compatible with the CPU, GPU, and Metal backend.
-Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4090/V100(16GB) GPU.
+Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4080/V100(16GB) GPU.
 
 ```
-python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --load-8bit
+python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights --load-8bit
 ```
 
 Besides, we are actively exploring more methods to make the model easier to run on more platforms.
 Contributions and pull requests are welcome.
 
 ## Serving with Web GUI
 
 To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. Here are the commands to follow in your terminal:
 
-**Note for Windows users:** Windows users will need Python 3.7 and above and to set the following environmental variable prior to launching the worker.
-
-```
-PYTHONUTF8=1
-```
-
 #### Launch the controller
 ```bash
 python3 -m fastchat.serve.controller
 ```
 
 This controller manages the distributed workers.
 
@@ -171,40 +160,80 @@
 This is the user interface that users will interact with.
 
 By following these steps, you will be able to serve your models using the web UI. You can open your browser and chat with a model now.
 
 
 ## Evaluation
 
-Our AI-enhanced [evaluation](fastchat/eval) pipeline is based on GPT-4. Here are some high-level instructions for using the pipeline:
+Our AI-enhanced evaluation pipeline is based on GPT-4. This section provides a high-level summary of the pipeline. For detailed instructions, please refer to the [evaluation](fastchat/eval) documentation.
+
+### Pipeline Steps
+
+1. Generate answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for Vicuna and other models.
+
+2. Generate reviews with GPT-4: Use GPT-4 to generate reviews automatically. This step can also be performed manually if the GPT-4 API is not available to you.
+
+3. Generate visualization data: Run `generate_webpage_data_from_table.py` to generate data for a static website, which allows you to visualize the evaluation data.
 
-First, generate answers from different models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint and run `model_qa.py` for Vicuna and other models.
+4. Visualize the data: Serve a static website under the `webpage` directory. You can use `python3 -m http.server` to serve the website locally.
 
-Then, use GPT-4 to generate reviews automatically, which can be done manually if the GPT-4 API is not available to you. Once you have your evaluation data, visualize the results by running `generate_webpage_data_from_table.py`, which generates data for a static website.
+### Data Format and Contribution
 
-Finally, serve a static website under the `webpage` directory. You can simply use `python3 -m http.server` to serve the website locally.
+We use a data format encoded with JSON Lines for evaluation. The format includes information on models, prompts, reviewers, questions, answers, and reviews.
 
-Besides the evaluation workflow, we also document the data format used for evaluation, which is encoded with JSON Lines and includes information on models, prompts, reviewers, questions, answers, and reviews. You can customize the evaluation process or contribute to our project by accessing relevant [data](fastchat/eval/table/).
+You can customize the evaluation process or contribute to our project by accessing the relevant [data](fastchat/eval/table/).
 
-Check [evaluation](fastchat/eval) for detailed instructions.
+For detailed instructions, please refer to the [evaluation](fastchat/eval) documentation.
 
 ## Fine-tuning
 ### Data
 
 Vicuna is created by fine-tuning a LLaMA base model using approximately 70K user-shared conversations gathered from ShareGPT.com with public APIs. To ensure data quality, we convert the HTML back to markdown and filter out some inappropriate or low-quality samples. Additionally, we divide lengthy conversations into smaller segments that fit the model's maximum context length. For detailed instructions to clean the ShareGPT data, check out [here](docs/commands/data_cleaning.md).
 
-Due to some concerns, we may not release the data at the moment. If you would like to try the fine-tuning code, you can try to run it with our [preprocessed alpaca dataset](playground/data/alpaca-data-conversation.json) (originally from [here](https://github.com/tatsu-lab/stanford_alpaca)).
+Due to some concerns, we may not release the ShareGPT dataset at the moment. If you would like to try the fine-tuning code, you can run it with some dummy questions in [dummy.json](playground/data/dummy.json). You can follow the same format and plug in your own data.
 
 ### Code and Hyperparameters
-We fine-tune the model using the code from [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca), with some modifications to support gradient checkpointing and [Flash Attention](https://github.com/HazyResearch/flash-attention). We use similar hyperparameters as the Stanford Alpaca.
+Our code is based on [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) with additional support for multi-round conversations.
+We use similar hyperparameters as the Stanford Alpaca.
 
 | Hyperparameter | Global Batch Size | Learning rate | Epochs | Max length | Weight decay |
 | --- | ---: | ---: | ---: | ---: | ---: |
 | Vicuna-13B | 128 | 2e-5 | 3 | 2048 | 0 |
 
+### Fine-tuning Vicuna-7B with Local GPUs
+You can use the following command to train Vicuna-7B with 4 x A100 (40GB).
+```bash
+torchrun --nproc_per_node=4 --master_port=20001 fastchat/train/train_mem.py \
+    --model_name_or_path ~/model_weights/llama-7b  \
+    --data_path playground/data/dummy.json \
+    --bf16 True \
+    --output_dir output \
+    --num_train_epochs 3 \
+    --per_device_train_batch_size 2 \
+    --per_device_eval_batch_size 2 \
+    --gradient_accumulation_steps 16 \
+    --evaluation_strategy "no" \
+    --save_strategy "steps" \
+    --save_steps 1200 \
+    --save_total_limit 10 \
+    --learning_rate 2e-5 \
+    --weight_decay 0. \
+    --warmup_ratio 0.03 \
+    --lr_scheduler_type "cosine" \
+    --logging_steps 1 \
+    --fsdp "full_shard auto_wrap" \
+    --fsdp_transformer_layer_cls_to_wrap 'LlamaDecoderLayer' \
+    --tf32 True \
+    --model_max_length 2048 \
+    --gradient_checkpointing True \
+    --lazy_preprocess True
+```
+
+If you meet out-of-memory during model saving, see solutions [here](https://github.com/pytorch/pytorch/issues/98823).
+
 ### Fine-tuning on Any Cloud with SkyPilot
 [SkyPilot](https://github.com/skypilot-org/skypilot) is a framework built by UC Berkeley for easily and cost effectively running ML workloads on any cloud (AWS, GCP, Azure, Lambda, etc.). 
 To use SkyPilot, install it with the following command and setup the cloud credentials locally following the instructions [here](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html).
 ```bash
 # Install skypilot from the master branch
 pip install git+https://github.com/skypilot-org/skypilot.git
 ```
@@ -218,43 +247,7 @@
 # Launch it on managed spot to save 3x cost (train Vicuna-13B with around $300)
 sky spot launch -n vicuna scripts/train-vicuna.yaml --env WANDB_API_KEY
 
 # Train a 7B model
 sky launch -c vicuna -s scripts/train-vicuna.yaml --env WANDB_API_KEY --env MODEL_SIZE=7
 ```
 Note: Please make sure the `WANDB_API_KEY` has been setup on your local machine. You can find the API key on your [wandb profile page](https://wandb.ai/authorize). If you would like to train the model without using wandb, you can replace the `--env WANDB_API_KEY` flag with `--env WANDB_MODE=offline`.
-
-#### Alpaca
-Launch the training job with the following line (will be launched on a single node with 4 A100-80GB GPUs)
-```
-sky launch -c alpaca -s scripts/train-alpaca.yaml --env WANDB_API_KEY
-```
-
-### Fine-tuning with Local GPUs
-Vicuna can also be trained on 8 A100 GPUs with 80GB memory with the following code. To train on fewer GPUs, you can reduce the `per_device_train_batch_size` and increase the `gradient_accumulation_steps` accordingly to keep the global batch size the same. To setup the environment, please see the setup section in [scripts/train-vicuna.yaml](scripts/train-vicuna.yaml).
-```bash
-torchrun --nnodes=1 --nproc_per_node=8 --master_port=<your_random_port> \
-    fastchat/train/train_mem.py \
-    --model_name_or_path <path-to-llama-model-weight> \
-    --data_path <path-to-data> \
-    --bf16 True \
-    --output_dir ./checkpoints \
-    --num_train_epochs 3 \
-    --per_device_train_batch_size 4 \
-    --per_device_eval_batch_size 4 \
-    --gradient_accumulation_steps 1 \
-    --evaluation_strategy "no" \
-    --save_strategy "steps" \
-    --save_steps 1200 \
-    --save_total_limit 100 \
-    --learning_rate 2e-5 \
-    --weight_decay 0. \
-    --warmup_ratio 0.03 \
-    --lr_scheduler_type "cosine" \
-    --logging_steps 1 \
-    --fsdp "full_shard auto_wrap" \
-    --fsdp_transformer_layer_cls_to_wrap 'LlamaDecoderLayer' \
-    --tf32 True \
-    --model_max_length 2048 \
-    --gradient_checkpointing True \
-    --lazy_preprocess True
-```
```

#### html2text {}

```diff
@@ -1,14 +1,8 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.1.9 Summary: An open platform for
-training, serving, and evaluating large language model based chatbots. Project-
-URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
-https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE # FastChat An open platform for training, serving, and evaluating large
+# FastChat An open platform for training, serving, and evaluating large
 language model based chatbots. ## Release
                            [assets/vicuna-logo.jpeg]
 - ð¥ We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90%
 ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and
 [demo](https://chat.lmsys.org/). [assets/demo-narrow.gif] Join our [Discord]
 (https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://
 twitter.com/lmsysorg) to get the latest updates. ## Contents - [Install]
@@ -16,138 +10,137 @@
 Interface](#inference-with-command-line-interface) - [Serving with Web GUI]
 (#serving-with-web-gui) - [Evaluation](#evaluation) - [Fine-tuning](#fine-
 tuning) ## Install ### Method 1: With pip ```bash # Install FastChat pip3
 install fschat # Install the latest main branch of huggingface/transformers
 pip3 install git+https://github.com/huggingface/transformers ``` ### Method 2:
 From source 1. Clone this repository and navigate to the FastChat folder
 ```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ``` If you
-are running on Mac: ```bash brew install rust ``` 2. Install Package ```bash
-pip3 install --upgrade pip # enable PEP 660 support pip3 install -e . ``` ##
-Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as delta
-weights to comply with the LLaMA model license. You can add our delta to the
-original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get the
-original LLaMA weights in the huggingface format by following the instructions
-[here](https://huggingface.co/docs/transformers/main/model_doc/llama). 2. Use
-the following scripts to get Vicuna weights by applying our delta. They will
-automatically download delta weights from our Hugging Face [account](https://
-huggingface.co/lmsys). **NOTE**: Our released weights are only compatible with
-the latest main branch of huggingface/transformers. We install the correct
-version of transformers when fastchat is installed. ### Vicuna-13B This
+are running on Mac: ```bash brew install rust cmake ``` 2. Install Package
+```bash pip3 install --upgrade pip # enable PEP 660 support pip3 install -e .
+``` ## Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as
+delta weights to comply with the LLaMA model license. You can add our delta to
+the original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get
+the original LLaMA weights in the huggingface format by following the
+instructions [here](https://huggingface.co/docs/transformers/main/model_doc/
+llama). 2. Use the following scripts to get Vicuna weights by applying our
+delta. They will automatically download delta weights from our Hugging Face
+[account](https://huggingface.co/lmsys). **NOTE**: Our released weights are
+only compatible with the latest main branch of huggingface/transformers. We
+install the correct version of transformers when fastchat is installed. ###
+Vicuna-7B This conversion command needs around 30 GB of CPU RAM. If you do not
+have enough memory, you can create a large swap file that allows the operating
+system to automatically utilize the disk as virtual memory. ```bash python3 -
+m fastchat.model.apply_delta \ --base /path/to/llama-7b \ --target /output/
+path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-v1.1 ``` ### Vicuna-13B This
 conversion command needs around 60 GB of CPU RAM. If you do not have enough
 memory, you can create a large swap file that allows the operating system to
 automatically utilize the disk as virtual memory. ```bash python3 -
 m fastchat.model.apply_delta \ --base /path/to/llama-13b \ --target /output/
-path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v0 ``` ### Vicuna-7B This
-conversion command needs around 30 GB of CPU RAM. If you do not have enough
-memory, you can create a large swap file that allows the operating system to
-automatically utilize the disk as virtual memory. ```bash python3 -
-m fastchat.model.apply_delta \ --base /path/to/llama-7b \ --target /output/
-path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-v0 ``` ## Inference with
-Command Line Interface #### Single GPU The command below requires around 28GB
-of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. ``` python3
--m fastchat.serve.cli --model-name /path/to/vicuna/weights ``` #### Multiple
-GPUs If you do not have enough GPU memory, you can use model parallelism to
-aggregate memory from multiple GPUs on the same machine. ``` python3 -
-m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2 ``` ####
-CPU Only This runs on the CPU only and does not require GPU. It requires around
-60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
-``` python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device
-cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
-`--device mps` to enable GPU acceleration on Mac computers and use `--load-
-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-
-name /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can run on
-a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or Other
-Platforms If you do not have enough memory, you can enable 8-bit compression by
-adding `--load-8bit` to commands above. This can reduce the memory usage by
-around half with slightly degraded model quality. It is compatible with the
-CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run on a
-single NVIDIA 3090/4090/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --
-model-name /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
+path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v1.1 ``` ### Old weights
+See [docs/weights_version.md](docs/weights_version.md) for all versions of
+weights and their differences. ## Inference with Command Line Interface
+(Experimental Feature: You can specify `--style rich` to enable rich text
+output and better text streaming quality for some non-ASCII content. This may
+not work properly on certain terminals.) #### Single GPU The command below
+requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for
+Vicuna-7B. See the "No Enough Memory" section below if you do not have enough
+memory. ``` python3 -m fastchat.serve.cli --model-path /path/to/vicuna/weights
+``` #### Multiple GPUs You can use model parallelism to aggregate GPU memory
+from multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --num-gpus 2 ``` #### CPU Only This runs on
+the CPU only and does not require GPU. It requires around 60GB of CPU memory
+for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/vicuna/weights --device cpu ``` ####
+Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
+to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
+load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can
+run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or
+Other Platforms If you do not have enough memory, you can enable 8-bit
+compression by adding `--load-8bit` to commands above. This can reduce memory
+usage by around half with slightly degraded model quality. It is compatible
+with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
+on a single NVIDIA 3090/4080/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli
+--model-path /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
 exploring more methods to make the model easier to run on more platforms.
 Contributions and pull requests are welcome. ## Serving with Web GUI To serve
 using the web UI, you need three main components: web servers that interface
 with users, model workers that host one or more models, and a controller to
 coordinate the webserver and model workers. Here are the commands to follow in
-your terminal: **Note for Windows users:** Windows users will need Python 3.7
-and above and to set the following environmental variable prior to launching
-the worker. ``` PYTHONUTF8=1 ``` #### Launch the controller ```bash python3 -
+your terminal: #### Launch the controller ```bash python3 -
 m fastchat.serve.controller ``` This controller manages the distributed
 workers. #### Launch the model worker ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". You can launch multiple model workers to serve multiple models
 concurrently. The model worker will connect to the controller automatically. To
 ensure that your model worker is connected to your controller properly, send a
 test message using the following command: ```bash python3 -
 m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
 Gradio web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This
 is the user interface that users will interact with. By following these steps,
 you will be able to serve your models using the web UI. You can open your
-browser and chat with a model now. ## Evaluation Our AI-enhanced [evaluation]
-(fastchat/eval) pipeline is based on GPT-4. Here are some high-level
-instructions for using the pipeline: First, generate answers from different
-models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint
-and run `model_qa.py` for Vicuna and other models. Then, use GPT-4 to generate
-reviews automatically, which can be done manually if the GPT-4 API is not
-available to you. Once you have your evaluation data, visualize the results by
-running `generate_webpage_data_from_table.py`, which generates data for a
-static website. Finally, serve a static website under the `webpage` directory.
-You can simply use `python3 -m http.server` to serve the website locally.
-Besides the evaluation workflow, we also document the data format used for
-evaluation, which is encoded with JSON Lines and includes information on
-models, prompts, reviewers, questions, answers, and reviews. You can customize
-the evaluation process or contribute to our project by accessing relevant
-[data](fastchat/eval/table/). Check [evaluation](fastchat/eval) for detailed
-instructions. ## Fine-tuning ### Data Vicuna is created by fine-tuning a LLaMA
+browser and chat with a model now. ## Evaluation Our AI-enhanced evaluation
+pipeline is based on GPT-4. This section provides a high-level summary of the
+pipeline. For detailed instructions, please refer to the [evaluation](fastchat/
+eval) documentation. ### Pipeline Steps 1. Generate answers from different
+models: Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint
+and run `get_model_answer.py` for Vicuna and other models. 2. Generate reviews
+with GPT-4: Use GPT-4 to generate reviews automatically. This step can also be
+performed manually if the GPT-4 API is not available to you. 3. Generate
+visualization data: Run `generate_webpage_data_from_table.py` to generate data
+for a static website, which allows you to visualize the evaluation data. 4.
+Visualize the data: Serve a static website under the `webpage` directory. You
+can use `python3 -m http.server` to serve the website locally. ### Data Format
+and Contribution We use a data format encoded with JSON Lines for evaluation.
+The format includes information on models, prompts, reviewers, questions,
+answers, and reviews. You can customize the evaluation process or contribute to
+our project by accessing the relevant [data](fastchat/eval/table/). For
+detailed instructions, please refer to the [evaluation](fastchat/eval)
+documentation. ## Fine-tuning ### Data Vicuna is created by fine-tuning a LLaMA
 base model using approximately 70K user-shared conversations gathered from
 ShareGPT.com with public APIs. To ensure data quality, we convert the HTML back
 to markdown and filter out some inappropriate or low-quality samples.
 Additionally, we divide lengthy conversations into smaller segments that fit
 the model's maximum context length. For detailed instructions to clean the
 ShareGPT data, check out [here](docs/commands/data_cleaning.md). Due to some
-concerns, we may not release the data at the moment. If you would like to try
-the fine-tuning code, you can try to run it with our [preprocessed alpaca
-dataset](playground/data/alpaca-data-conversation.json) (originally from [here]
-(https://github.com/tatsu-lab/stanford_alpaca)). ### Code and Hyperparameters
-We fine-tune the model using the code from [Stanford Alpaca](https://
-github.com/tatsu-lab/stanford_alpaca), with some modifications to support
-gradient checkpointing and [Flash Attention](https://github.com/HazyResearch/
-flash-attention). We use similar hyperparameters as the Stanford Alpaca. |
-Hyperparameter | Global Batch Size | Learning rate | Epochs | Max length |
-Weight decay | | --- | ---: | ---: | ---: | ---: | ---: | | Vicuna-13B | 128 |
-2e-5 | 3 | 2048 | 0 | ### Fine-tuning on Any Cloud with SkyPilot [SkyPilot]
-(https://github.com/skypilot-org/skypilot) is a framework built by UC Berkeley
-for easily and cost effectively running ML workloads on any cloud (AWS, GCP,
-Azure, Lambda, etc.). To use SkyPilot, install it with the following command
-and setup the cloud credentials locally following the instructions [here]
-(https://skypilot.readthedocs.io/en/latest/getting-started/installation.html).
-```bash # Install skypilot from the master branch pip install git+https://
-github.com/skypilot-org/skypilot.git ``` #### Vicuna Vicuna can be trained on 8
-A100 GPUs with 80GB memory. The following command will automatically launch a
-node satisfying the requirement, setup and run the training job on it. ```bash
-sky launch -c vicuna -s scripts/train-vicuna.yaml --env WANDB_API_KEY ``` Other
-options are also valid: ```bash # Launch it on managed spot to save 3x cost
-(train Vicuna-13B with around $300) sky spot launch -n vicuna scripts/train-
-vicuna.yaml --env WANDB_API_KEY # Train a 7B model sky launch -c vicuna -
-s scripts/train-vicuna.yaml --env WANDB_API_KEY --env MODEL_SIZE=7 ``` Note:
-Please make sure the `WANDB_API_KEY` has been setup on your local machine. You
-can find the API key on your [wandb profile page](https://wandb.ai/authorize).
-If you would like to train the model without using wandb, you can replace the
-`--env WANDB_API_KEY` flag with `--env WANDB_MODE=offline`. #### Alpaca Launch
-the training job with the following line (will be launched on a single node
-with 4 A100-80GB GPUs) ``` sky launch -c alpaca -s scripts/train-alpaca.yaml --
-env WANDB_API_KEY ``` ### Fine-tuning with Local GPUs Vicuna can also be
-trained on 8 A100 GPUs with 80GB memory with the following code. To train on
-fewer GPUs, you can reduce the `per_device_train_batch_size` and increase the
-`gradient_accumulation_steps` accordingly to keep the global batch size the
-same. To setup the environment, please see the setup section in [scripts/train-
-vicuna.yaml](scripts/train-vicuna.yaml). ```bash torchrun --nnodes=1 --
-nproc_per_node=8 --master_port= \ fastchat/train/train_mem.py \ --
-model_name_or_path  \ --data_path  \ --bf16 True \ --output_dir ./checkpoints \
---num_train_epochs 3 \ --per_device_train_batch_size 4 \ --
-per_device_eval_batch_size 4 \ --gradient_accumulation_steps 1 \ --
+concerns, we may not release the ShareGPT dataset at the moment. If you would
+like to try the fine-tuning code, you can run it with some dummy questions in
+[dummy.json](playground/data/dummy.json). You can follow the same format and
+plug in your own data. ### Code and Hyperparameters Our code is based on
+[Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) with additional
+support for multi-round conversations. We use similar hyperparameters as the
+Stanford Alpaca. | Hyperparameter | Global Batch Size | Learning rate | Epochs
+| Max length | Weight decay | | --- | ---: | ---: | ---: | ---: | ---: | |
+Vicuna-13B | 128 | 2e-5 | 3 | 2048 | 0 | ### Fine-tuning Vicuna-7B with Local
+GPUs You can use the following command to train Vicuna-7B with 4 x A100 (40GB).
+```bash torchrun --nproc_per_node=4 --master_port=20001 fastchat/train/
+train_mem.py \ --model_name_or_path ~/model_weights/llama-7b \ --data_path
+playground/data/dummy.json \ --bf16 True \ --output_dir output \ --
+num_train_epochs 3 \ --per_device_train_batch_size 2 \ --
+per_device_eval_batch_size 2 \ --gradient_accumulation_steps 16 \ --
 evaluation_strategy "no" \ --save_strategy "steps" \ --save_steps 1200 \ --
-save_total_limit 100 \ --learning_rate 2e-5 \ --weight_decay 0. \ --
-warmup_ratio 0.03 \ --lr_scheduler_type "cosine" \ --logging_steps 1 \ --fsdp
-"full_shard auto_wrap" \ --fsdp_transformer_layer_cls_to_wrap
-'LlamaDecoderLayer' \ --tf32 True \ --model_max_length 2048 \ --
-gradient_checkpointing True \ --lazy_preprocess True ```
+save_total_limit 10 \ --learning_rate 2e-5 \ --weight_decay 0. \ --warmup_ratio
+0.03 \ --lr_scheduler_type "cosine" \ --logging_steps 1 \ --fsdp "full_shard
+auto_wrap" \ --fsdp_transformer_layer_cls_to_wrap 'LlamaDecoderLayer' \ --tf32
+True \ --model_max_length 2048 \ --gradient_checkpointing True \ --
+lazy_preprocess True ``` If you meet out-of-memory during model saving, see
+solutions [here](https://github.com/pytorch/pytorch/issues/98823). ### Fine-
+tuning on Any Cloud with SkyPilot [SkyPilot](https://github.com/skypilot-org/
+skypilot) is a framework built by UC Berkeley for easily and cost effectively
+running ML workloads on any cloud (AWS, GCP, Azure, Lambda, etc.). To use
+SkyPilot, install it with the following command and setup the cloud credentials
+locally following the instructions [here](https://skypilot.readthedocs.io/en/
+latest/getting-started/installation.html). ```bash # Install skypilot from the
+master branch pip install git+https://github.com/skypilot-org/skypilot.git ```
+#### Vicuna Vicuna can be trained on 8 A100 GPUs with 80GB memory. The
+following command will automatically launch a node satisfying the requirement,
+setup and run the training job on it. ```bash sky launch -c vicuna -s scripts/
+train-vicuna.yaml --env WANDB_API_KEY ``` Other options are also valid: ```bash
+# Launch it on managed spot to save 3x cost (train Vicuna-13B with around $300)
+sky spot launch -n vicuna scripts/train-vicuna.yaml --env WANDB_API_KEY # Train
+a 7B model sky launch -c vicuna -s scripts/train-vicuna.yaml --env
+WANDB_API_KEY --env MODEL_SIZE=7 ``` Note: Please make sure the `WANDB_API_KEY`
+has been setup on your local machine. You can find the API key on your [wandb
+profile page](https://wandb.ai/authorize). If you would like to train the model
+without using wandb, you can replace the `--env WANDB_API_KEY` flag with `--env
+WANDB_MODE=offline`.
```

### Comparing `fschat-0.1.9/fschat.egg-info/SOURCES.txt` & `fschat-0.2.0/fschat.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,37 +4,44 @@
 fastchat/__init__.py
 fastchat/constants.py
 fastchat/conversation.py
 fastchat/utils.py
 fastchat/data/__init__.py
 fastchat/data/alpaca-converter.py
 fastchat/data/clean_sharegpt.py
+fastchat/data/hardcoded_questions.py
 fastchat/data/inspect.py
+fastchat/data/merge.py
 fastchat/data/optional_clean.py
 fastchat/data/pretty_json.py
+fastchat/data/sample.py
 fastchat/data/split_long_conversation.py
 fastchat/eval/eval_gpt_review.py
 fastchat/eval/generate_webpage_data_from_table.py
 fastchat/eval/get_model_answer.py
 fastchat/eval/qa_baseline_gpt35.py
 fastchat/model/__init__.py
 fastchat/model/apply_delta.py
+fastchat/model/convert_fp16.py
 fastchat/model/make_delta.py
 fastchat/serve/__init__.py
+fastchat/serve/cacheflow_worker.py
 fastchat/serve/cli.py
 fastchat/serve/compression.py
 fastchat/serve/controller.py
 fastchat/serve/gradio_css.py
 fastchat/serve/gradio_patch.py
 fastchat/serve/gradio_web_server.py
+fastchat/serve/inference.py
 fastchat/serve/model_worker.py
 fastchat/serve/monkey_patch_non_inplace.py
 fastchat/serve/register_worker.py
 fastchat/serve/serve_chatglm.py
 fastchat/serve/test_message.py
+fastchat/serve/test_throughput.py
 fastchat/train/llama_flash_attn_monkey_patch.py
 fastchat/train/train.py
 fastchat/train/train_lora.py
 fastchat/train/train_mem.py
 fschat.egg-info/PKG-INFO
 fschat.egg-info/SOURCES.txt
 fschat.egg-info/dependency_links.txt
```

### Comparing `fschat-0.1.9/pyproject.toml` & `fschat-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fschat"
-version = "0.1.9"
+version = "0.2.0"
 description = "An open platform for training, serving, and evaluating large language model based chatbots."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
     "accelerate", "fastapi", "gradio==3.23", "markdown2[all]", "numpy",
     "requests", "sentencepiece", "tokenizers>=0.12.1",
-    "torch", "uvicorn", "wandb",
+    "torch", "uvicorn", "wandb", "prompt_toolkit>=3.0.0", "rich>=10.0.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/lm-sys/fastchat"
 "Bug Tracker" = "https://github.com/lm-sys/fastchat/issues"
 
 [tool.setuptools.packages.find]
```

