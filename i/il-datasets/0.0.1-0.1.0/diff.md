# Comparing `tmp/il-datasets-0.0.1.tar.gz` & `tmp/il-datasets-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "il-datasets-0.0.1.tar", last modified: Tue Oct 25 13:02:01 2022, max compression
+gzip compressed data, was "/home/nathan/Documents/git/IL-Datasets/dist/.tmp-6a75dv6h/il-datasets-0.1.0.tar", last modified: Wed Apr 12 10:13:30 2023, max compression
```

## Comparing `il-datasets-0.0.1.tar` & `il-datasets-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-10-25 13:02:01.420716 il-datasets-0.0.1/
--rw-rw-rw-   0        0        0     1101 2022-10-09 16:05:22.000000 il-datasets-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4085 2022-10-25 13:02:01.420716 il-datasets-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3618 2022-10-25 12:53:32.000000 il-datasets-0.0.1/README.md
--rw-rw-rw-   0        0        0      447 2022-10-25 12:59:12.000000 il-datasets-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      782 2022-10-25 13:02:01.423716 il-datasets-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       71 2022-10-09 16:25:41.000000 il-datasets-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-25 13:02:01.340827 il-datasets-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2022-10-25 13:02:01.404833 il-datasets-0.0.1/src/il_datasets.egg-info/
--rw-rw-rw-   0        0        0     4085 2022-10-25 13:02:01.000000 il-datasets-0.0.1/src/il_datasets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2022-10-25 13:02:01.000000 il-datasets-0.0.1/src/il_datasets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-25 13:02:01.000000 il-datasets-0.0.1/src/il_datasets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2022-10-25 13:02:01.000000 il-datasets-0.0.1/src/il_datasets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2022-10-25 13:02:01.000000 il-datasets-0.0.1/src/il_datasets.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-10-25 13:02:01.412716 il-datasets-0.0.1/src/imitation_datasets/
--rw-rw-rw-   0        0        0      191 2022-10-19 17:44:02.000000 il-datasets-0.0.1/src/imitation_datasets/__init__.py
--rw-rw-rw-   0        0        0      780 2022-10-08 12:07:17.000000 il-datasets-0.0.1/src/imitation_datasets/args.py
--rw-rw-rw-   0        0        0     3305 2022-10-25 12:50:05.000000 il-datasets-0.0.1/src/imitation_datasets/controller.py
--rw-rw-rw-   0        0        0     1962 2022-10-19 18:29:55.000000 il-datasets-0.0.1/src/imitation_datasets/experts.py
-drwxrwxrwx   0        0        0        0 2022-10-25 13:02:01.418717 il-datasets-0.0.1/src/imitation_datasets/register/
--rw-rw-rw-   0        0        0       82 2022-10-19 18:29:33.000000 il-datasets-0.0.1/src/imitation_datasets/register/__init__.py
--rw-rw-rw-   0        0        0     2179 2022-10-07 20:56:38.000000 il-datasets-0.0.1/src/imitation_datasets/register/atari.py
--rw-rw-rw-   0        0        0      245 2022-10-19 18:31:29.000000 il-datasets-0.0.1/src/imitation_datasets/register/classic.py
--rw-rw-rw-   0        0        0     1411 2022-10-07 20:54:54.000000 il-datasets-0.0.1/src/imitation_datasets/register/mujoco.py
--rw-rw-rw-   0        0        0     3033 2022-10-25 00:38:04.000000 il-datasets-0.0.1/src/imitation_datasets/utils.py
+drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-04-12 10:13:30.000000 il-datasets-0.1.0/
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     1081 2023-01-09 12:54:57.000000 il-datasets-0.1.0/LICENSE
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     3987 2023-04-12 10:13:30.000000 il-datasets-0.1.0/PKG-INFO
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     3534 2023-01-09 12:54:57.000000 il-datasets-0.1.0/README.md
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)      432 2023-01-09 12:54:57.000000 il-datasets-0.1.0/pyproject.toml
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)      746 2023-04-12 10:13:30.000000 il-datasets-0.1.0/setup.cfg
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)       68 2023-01-09 12:54:57.000000 il-datasets-0.1.0/setup.py
+drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-04-12 10:13:30.000000 il-datasets-0.1.0/src/
+drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-04-12 10:13:30.000000 il-datasets-0.1.0/src/il_datasets.egg-info/
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     3987 2023-04-12 10:13:30.000000 il-datasets-0.1.0/src/il_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)      584 2023-04-12 10:13:30.000000 il-datasets-0.1.0/src/il_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)        1 2023-04-12 10:13:30.000000 il-datasets-0.1.0/src/il_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)       64 2023-04-12 10:13:30.000000 il-datasets-0.1.0/src/il_datasets.egg-info/requires.txt
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)       19 2023-04-12 10:13:30.000000 il-datasets-0.1.0/src/il_datasets.egg-info/top_level.txt
+drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-04-12 10:13:30.000000 il-datasets-0.1.0/src/imitation_datasets/
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)      187 2023-01-09 12:54:57.000000 il-datasets-0.1.0/src/imitation_datasets/__init__.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)      758 2023-01-09 12:54:57.000000 il-datasets-0.1.0/src/imitation_datasets/args.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     3461 2023-04-12 10:04:01.000000 il-datasets-0.1.0/src/imitation_datasets/controller.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     1894 2023-01-09 12:54:57.000000 il-datasets-0.1.0/src/imitation_datasets/experts.py
+drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-04-12 10:13:30.000000 il-datasets-0.1.0/src/imitation_datasets/register/
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)       80 2023-01-09 12:54:57.000000 il-datasets-0.1.0/src/imitation_datasets/register/__init__.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     2112 2023-01-09 12:54:57.000000 il-datasets-0.1.0/src/imitation_datasets/register/atari.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)      436 2023-04-12 09:47:37.000000 il-datasets-0.1.0/src/imitation_datasets/register/classic.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     1357 2023-01-12 10:29:09.000000 il-datasets-0.1.0/src/imitation_datasets/register/mujoco.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     2938 2023-04-12 09:57:05.000000 il-datasets-0.1.0/src/imitation_datasets/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `il-datasets-0.0.1/LICENSE` & `il-datasets-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Nathan Schneider Gavenski
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2022 Nathan Schneider Gavenski
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `il-datasets-0.0.1/PKG-INFO` & `il-datasets-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-Metadata-Version: 2.1
-Name: il-datasets
-Version: 0.0.1
-Summary: A package for creating IL datasets
-Home-page: https://github.com/NathanGavenski/IL-Datasets
-Author: Nathan Gavenski
-Author-email: nathangavenski@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# IL Datasets
-
-Hi, welcome to the Imitation Learning (IL) Datasets.
-Something that always bothered me a lot was how difficult it was to find good weights for an expert, or trying to create a dataset for different state-of-the-art methods.
-For this reason I've created this repository in an effort to make it more accessible for researches to create datasets using experts from the [Hugging Face](https://huggingface.co/models?pipeline_tag=reinforcement-learning).
-
---- 
-## How does it work?
-
-This project also works with multithreading, which should accelerate the dataset creation.
-It consists of one ``Controller`` class, which requires two different functions to work: (i) a ``enjoy`` function (for the agent to play and record an episode); and a (ii) ``collate`` function (for putting all episodes together).
-
----
-
-The ``enjoy`` function will receive 3 parameters and return 1:
-
-* path: str - where the episode is going to be recorded
-* experiment: Context - A class for recording all information (if you don't want to use `print` - keeping the console clear)
-* expert: Policy - A model based on the [StableBaselines3](https://stable-baselines3.readthedocs.io/en/master/) `BaseAlgorithm`.
-
-* returns: bool - Whether it was successfull or not
-
-Obs: To use the model you can call ``predict``, the policy class already has the correct form of using it (a.k.a., how the StableBaselines3 uses).
-
----
-
-The ``collate`` function will receive 2 parameters and return 1:
-
-* path: str - where it should save the final dataset
-* episodes: list\[str\] - A list of paths for each file
-
-* returns: bool - Whether it was successfull or not
-
-
----
-## Requirements
-
-I did use Python=3.9 during development. \
-All other requirements are listed in [requirements.txt](./requirements.txt).
-
----
-## Registering new experts
-
-If you would like to add new experts locally, you can call the [Experts](./utils/experts.py) class. It uses the following structure:
-
-* identifier: str - A name for calling the expert.
-* policy: Policy - A dataclass with:
-    * name: str - Gym Environment name
-    * repo_id: str - Hugging Face repo indentification
-    * filename: str - Weights file name
-    * threshold: float - How much reward should the episode accumulate to be considered good
-    * algo: BaseAlgorithm - The class from StableBaselines3
-
-Obs: If not using StableBaselines, the expert has to have a `predict` function that receives:
-
-* obs: Tensor - Current environment state
-* state: Tensor - Model's internal state
-* deterministic: bool - If it should explore or not
-
----
-## This repository is not complete
-
-Here is a list of the upcoming releases:
-
-- [x] Collate function support
-- [X] Support for installing as a dependency
-- [ ] Module for downloading trajectories from a Hugging Face dataset 
-- [ ] Create actual documentation
-- [X] Create some examples
-- [ ] Create tests
- 
----
-
-## If you like this repository be sure to check my other projects:
-
-### Development
-- [An easy to use Wrapper for Tensorboard](https://github.com/NathanGavenski/Tensorboard-Wrapper)
-- [A watcher for python to facilitate development of small projects](https://github.com/NathanGavenski/python-watcher)
-
-### Academic
-- [Imitating Unknown Policies via Exploration (BMVC)](https://arxiv.org/pdf/2008.05660.pdf)
-- [Augmented behavioral cloning from observation (IJCNN)](https://arxiv.org/pdf/2004.13529.pdf)
-- [Self-supervised imitation learning from observation (MSc dissertation)](https://repositorio.pucrs.br/dspace/bitstream/10923/17536/1/000500266-Texto%2Bcompleto-0.pdf)
-
+Metadata-Version: 2.1
+Name: il-datasets
+Version: 0.1.0
+Summary: A package for creating IL datasets
+Home-page: https://github.com/NathanGavenski/IL-Datasets
+Author: Nathan Gavenski
+Author-email: nathangavenski@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# IL Datasets
+
+Hi, welcome to the Imitation Learning (IL) Datasets.
+Something that always bothered me a lot was how difficult it was to find good weights for an expert, or trying to create a dataset for different state-of-the-art methods.
+For this reason I've created this repository in an effort to make it more accessible for researches to create datasets using experts from the [Hugging Face](https://huggingface.co/models?pipeline_tag=reinforcement-learning).
+
+--- 
+## How does it work?
+
+This project also works with multithreading, which should accelerate the dataset creation.
+It consists of one ``Controller`` class, which requires two different functions to work: (i) a ``enjoy`` function (for the agent to play and record an episode); and a (ii) ``collate`` function (for putting all episodes together).
+
+---
+
+The ``enjoy`` function will receive 3 parameters and return 1:
+
+* path: str - where the episode is going to be recorded
+* experiment: Context - A class for recording all information (if you don't want to use `print` - keeping the console clear)
+* expert: Policy - A model based on the [StableBaselines3](https://stable-baselines3.readthedocs.io/en/master/) `BaseAlgorithm`.
+
+* returns: bool - Whether it was successfull or not
+
+Obs: To use the model you can call ``predict``, the policy class already has the correct form of using it (a.k.a., how the StableBaselines3 uses).
+
+---
+
+The ``collate`` function will receive 2 parameters and return 1:
+
+* path: str - where it should save the final dataset
+* episodes: list\[str\] - A list of paths for each file
+
+* returns: bool - Whether it was successfull or not
+
+
+---
+## Requirements
+
+I did use Python=3.9 during development. \
+All other requirements are listed in [requirements.txt](./requirements.txt).
+
+---
+## Registering new experts
+
+If you would like to add new experts locally, you can call the [Experts](./utils/experts.py) class. It uses the following structure:
+
+* identifier: str - A name for calling the expert.
+* policy: Policy - A dataclass with:
+    * name: str - Gym Environment name
+    * repo_id: str - Hugging Face repo indentification
+    * filename: str - Weights file name
+    * threshold: float - How much reward should the episode accumulate to be considered good
+    * algo: BaseAlgorithm - The class from StableBaselines3
+
+Obs: If not using StableBaselines, the expert has to have a `predict` function that receives:
+
+* obs: Tensor - Current environment state
+* state: Tensor - Model's internal state
+* deterministic: bool - If it should explore or not
+
+---
+## This repository is not complete
+
+Here is a list of the upcoming releases:
+
+- [x] Collate function support
+- [X] Support for installing as a dependency
+- [ ] Module for downloading trajectories from a Hugging Face dataset 
+- [ ] Create actual documentation
+- [X] Create some examples
+- [ ] Create tests
+ 
+---
+
+## If you like this repository be sure to check my other projects:
+
+### Development
+- [An easy to use Wrapper for Tensorboard](https://github.com/NathanGavenski/Tensorboard-Wrapper)
+- [A watcher for python to facilitate development of small projects](https://github.com/NathanGavenski/python-watcher)
+
+### Academic
+- [Imitating Unknown Policies via Exploration (BMVC)](https://arxiv.org/pdf/2008.05660.pdf)
+- [Augmented behavioral cloning from observation (IJCNN)](https://arxiv.org/pdf/2004.13529.pdf)
+- [Self-supervised imitation learning from observation (MSc dissertation)](https://repositorio.pucrs.br/dspace/bitstream/10923/17536/1/000500266-Texto%2Bcompleto-0.pdf)
+
```

### Comparing `il-datasets-0.0.1/setup.cfg` & `il-datasets-0.1.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,47 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2069 6c2d 6461 7461 7365 7473 0d0a   = il-datasets..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 310d  version = 0.0.1.
-00000030: 0a61 7574 686f 7220 3d20 4e61 7468 616e  .author = Nathan
-00000040: 2047 6176 656e 736b 690d 0a61 7574 686f   Gavenski..autho
-00000050: 725f 656d 6169 6c20 3d20 6e61 7468 616e  r_email = nathan
-00000060: 6761 7665 6e73 6b69 4067 6d61 696c 2e63  gavenski@gmail.c
-00000070: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
-00000080: 3d20 4120 7061 636b 6167 6520 666f 7220  = A package for 
-00000090: 6372 6561 7469 6e67 2049 4c20 6461 7461  creating IL data
-000000a0: 7365 7473 0d0a 6c6f 6e67 5f64 6573 6372  sets..long_descr
-000000b0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
-000000c0: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
-000000d0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
-000000e0: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
-000000f0: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
-00000100: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000110: 6d2f 4e61 7468 616e 4761 7665 6e73 6b69  m/NathanGavenski
-00000120: 2f49 4c2d 4461 7461 7365 7473 0d0a 7072  /IL-Datasets..pr
-00000130: 6f6a 6563 745f 7572 6c73 203d 200d 0a42  oject_urls = ..B
-00000140: 7567 2054 7261 636b 6572 203d 2068 7474  ug Tracker = htt
-00000150: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000160: 4e61 7468 616e 4761 7665 6e73 6b69 2f49  NathanGavenski/I
-00000170: 4c2d 4461 7461 7365 7473 2f69 7373 7565  L-Datasets/issue
-00000180: 730d 0a63 6c61 7373 6966 6965 7273 203d  s..classifiers =
-00000190: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
-000001a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000001b0: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
-000001c0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-000001d0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-000001e0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-000001f0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-00000200: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
-00000210: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
-00000220: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
-00000230: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
-00000240: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000250: 3e3d 332e 382e 350d 0a69 6e73 7461 6c6c  >=3.8.5..install
-00000260: 5f72 6571 7569 7265 7320 3d20 0d0a 0968  _requires = ...h
-00000270: 7567 6769 6e67 6661 6365 5f73 6233 0d0a  uggingface_sb3..
-00000280: 0973 7461 626c 655f 6261 7365 6c69 6e65  .stable_baseline
-00000290: 7333 0d0a 0973 6233 5f63 6f6e 7472 6962  s3...sb3_contrib
-000002a0: 0d0a 0974 7164 6d0d 0a09 746f 7263 680d  ...tqdm...torch.
-000002b0: 0a09 7073 7574 696c 0d0a 0d0a 5b6f 7074  ..psutil....[opt
-000002c0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-000002d0: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
-000002e0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000002f0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000300: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 696c 2d64 6174 6173 6574 730a 7665  = il-datasets.ve
+00000020: 7273 696f 6e20 3d20 302e 312e 300a 6175  rsion = 0.1.0.au
+00000030: 7468 6f72 203d 204e 6174 6861 6e20 4761  thor = Nathan Ga
+00000040: 7665 6e73 6b69 0a61 7574 686f 725f 656d  venski.author_em
+00000050: 6169 6c20 3d20 6e61 7468 616e 6761 7665  ail = nathangave
+00000060: 6e73 6b69 4067 6d61 696c 2e63 6f6d 0a64  nski@gmail.com.d
+00000070: 6573 6372 6970 7469 6f6e 203d 2041 2070  escription = A p
+00000080: 6163 6b61 6765 2066 6f72 2063 7265 6174  ackage for creat
+00000090: 696e 6720 494c 2064 6174 6173 6574 730a  ing IL datasets.
+000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000b0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+000000c0: 6d64 0a6c 6f6e 675f 6465 7363 7269 7074  md.long_descript
+000000d0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+000000e0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+000000f0: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
+00000100: 6974 6875 622e 636f 6d2f 4e61 7468 616e  ithub.com/Nathan
+00000110: 4761 7665 6e73 6b69 2f49 4c2d 4461 7461  Gavenski/IL-Data
+00000120: 7365 7473 0a70 726f 6a65 6374 5f75 726c  sets.project_url
+00000130: 7320 3d20 0a42 7567 2054 7261 636b 6572  s = .Bug Tracker
+00000140: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+00000150: 622e 636f 6d2f 4e61 7468 616e 4761 7665  b.com/NathanGave
+00000160: 6e73 6b69 2f49 4c2d 4461 7461 7365 7473  nski/IL-Datasets
+00000170: 2f69 7373 7565 730a 636c 6173 7369 6669  /issues.classifi
+00000180: 6572 7320 3d20 0a09 5072 6f67 7261 6d6d  ers = ..Programm
+00000190: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001a0: 5079 7468 6f6e 203a 3a20 330a 094c 6963  Python :: 3..Lic
+000001b0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+000001c0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+000001d0: 6e73 650a 094f 7065 7261 7469 6e67 2053  nse..Operating S
+000001e0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+000001f0: 7065 6e64 656e 740a 0a5b 6f70 7469 6f6e  pendent..[option
+00000200: 735d 0a70 6163 6b61 6765 5f64 6972 203d  s].package_dir =
+00000210: 200a 093d 2073 7263 0a70 6163 6b61 6765   ..= src.package
+00000220: 7320 3d20 6669 6e64 3a0a 7079 7468 6f6e  s = find:.python
+00000230: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+00000240: 382e 350a 696e 7374 616c 6c5f 7265 7175  8.5.install_requ
+00000250: 6972 6573 203d 200a 0968 7567 6769 6e67  ires = ..hugging
+00000260: 6661 6365 5f73 6233 0a09 7374 6162 6c65  face_sb3..stable
+00000270: 5f62 6173 656c 696e 6573 330a 0973 6233  _baselines3..sb3
+00000280: 5f63 6f6e 7472 6962 0a09 7471 646d 0a09  _contrib..tqdm..
+00000290: 746f 7263 680a 0970 7375 7469 6c0a 0a5b  torch..psutil..[
+000002a0: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+000002b0: 2e66 696e 645d 0a77 6865 7265 203d 2073  .find].where = s
+000002c0: 7263 0a0a 5b65 6767 5f69 6e66 6f5d 0a74  rc..[egg_info].t
+000002d0: 6167 5f62 7569 6c64 203d 200a 7461 675f  ag_build = .tag_
+000002e0: 6461 7465 203d 2030 0a0a                 date = 0..
```

### Comparing `il-datasets-0.0.1/src/il_datasets.egg-info/PKG-INFO` & `il-datasets-0.1.0/src/il_datasets.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-Metadata-Version: 2.1
-Name: il-datasets
-Version: 0.0.1
-Summary: A package for creating IL datasets
-Home-page: https://github.com/NathanGavenski/IL-Datasets
-Author: Nathan Gavenski
-Author-email: nathangavenski@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# IL Datasets
-
-Hi, welcome to the Imitation Learning (IL) Datasets.
-Something that always bothered me a lot was how difficult it was to find good weights for an expert, or trying to create a dataset for different state-of-the-art methods.
-For this reason I've created this repository in an effort to make it more accessible for researches to create datasets using experts from the [Hugging Face](https://huggingface.co/models?pipeline_tag=reinforcement-learning).
-
---- 
-## How does it work?
-
-This project also works with multithreading, which should accelerate the dataset creation.
-It consists of one ``Controller`` class, which requires two different functions to work: (i) a ``enjoy`` function (for the agent to play and record an episode); and a (ii) ``collate`` function (for putting all episodes together).
-
----
-
-The ``enjoy`` function will receive 3 parameters and return 1:
-
-* path: str - where the episode is going to be recorded
-* experiment: Context - A class for recording all information (if you don't want to use `print` - keeping the console clear)
-* expert: Policy - A model based on the [StableBaselines3](https://stable-baselines3.readthedocs.io/en/master/) `BaseAlgorithm`.
-
-* returns: bool - Whether it was successfull or not
-
-Obs: To use the model you can call ``predict``, the policy class already has the correct form of using it (a.k.a., how the StableBaselines3 uses).
-
----
-
-The ``collate`` function will receive 2 parameters and return 1:
-
-* path: str - where it should save the final dataset
-* episodes: list\[str\] - A list of paths for each file
-
-* returns: bool - Whether it was successfull or not
-
-
----
-## Requirements
-
-I did use Python=3.9 during development. \
-All other requirements are listed in [requirements.txt](./requirements.txt).
-
----
-## Registering new experts
-
-If you would like to add new experts locally, you can call the [Experts](./utils/experts.py) class. It uses the following structure:
-
-* identifier: str - A name for calling the expert.
-* policy: Policy - A dataclass with:
-    * name: str - Gym Environment name
-    * repo_id: str - Hugging Face repo indentification
-    * filename: str - Weights file name
-    * threshold: float - How much reward should the episode accumulate to be considered good
-    * algo: BaseAlgorithm - The class from StableBaselines3
-
-Obs: If not using StableBaselines, the expert has to have a `predict` function that receives:
-
-* obs: Tensor - Current environment state
-* state: Tensor - Model's internal state
-* deterministic: bool - If it should explore or not
-
----
-## This repository is not complete
-
-Here is a list of the upcoming releases:
-
-- [x] Collate function support
-- [X] Support for installing as a dependency
-- [ ] Module for downloading trajectories from a Hugging Face dataset 
-- [ ] Create actual documentation
-- [X] Create some examples
-- [ ] Create tests
- 
----
-
-## If you like this repository be sure to check my other projects:
-
-### Development
-- [An easy to use Wrapper for Tensorboard](https://github.com/NathanGavenski/Tensorboard-Wrapper)
-- [A watcher for python to facilitate development of small projects](https://github.com/NathanGavenski/python-watcher)
-
-### Academic
-- [Imitating Unknown Policies via Exploration (BMVC)](https://arxiv.org/pdf/2008.05660.pdf)
-- [Augmented behavioral cloning from observation (IJCNN)](https://arxiv.org/pdf/2004.13529.pdf)
-- [Self-supervised imitation learning from observation (MSc dissertation)](https://repositorio.pucrs.br/dspace/bitstream/10923/17536/1/000500266-Texto%2Bcompleto-0.pdf)
-
+Metadata-Version: 2.1
+Name: il-datasets
+Version: 0.1.0
+Summary: A package for creating IL datasets
+Home-page: https://github.com/NathanGavenski/IL-Datasets
+Author: Nathan Gavenski
+Author-email: nathangavenski@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# IL Datasets
+
+Hi, welcome to the Imitation Learning (IL) Datasets.
+Something that always bothered me a lot was how difficult it was to find good weights for an expert, or trying to create a dataset for different state-of-the-art methods.
+For this reason I've created this repository in an effort to make it more accessible for researches to create datasets using experts from the [Hugging Face](https://huggingface.co/models?pipeline_tag=reinforcement-learning).
+
+--- 
+## How does it work?
+
+This project also works with multithreading, which should accelerate the dataset creation.
+It consists of one ``Controller`` class, which requires two different functions to work: (i) a ``enjoy`` function (for the agent to play and record an episode); and a (ii) ``collate`` function (for putting all episodes together).
+
+---
+
+The ``enjoy`` function will receive 3 parameters and return 1:
+
+* path: str - where the episode is going to be recorded
+* experiment: Context - A class for recording all information (if you don't want to use `print` - keeping the console clear)
+* expert: Policy - A model based on the [StableBaselines3](https://stable-baselines3.readthedocs.io/en/master/) `BaseAlgorithm`.
+
+* returns: bool - Whether it was successfull or not
+
+Obs: To use the model you can call ``predict``, the policy class already has the correct form of using it (a.k.a., how the StableBaselines3 uses).
+
+---
+
+The ``collate`` function will receive 2 parameters and return 1:
+
+* path: str - where it should save the final dataset
+* episodes: list\[str\] - A list of paths for each file
+
+* returns: bool - Whether it was successfull or not
+
+
+---
+## Requirements
+
+I did use Python=3.9 during development. \
+All other requirements are listed in [requirements.txt](./requirements.txt).
+
+---
+## Registering new experts
+
+If you would like to add new experts locally, you can call the [Experts](./utils/experts.py) class. It uses the following structure:
+
+* identifier: str - A name for calling the expert.
+* policy: Policy - A dataclass with:
+    * name: str - Gym Environment name
+    * repo_id: str - Hugging Face repo indentification
+    * filename: str - Weights file name
+    * threshold: float - How much reward should the episode accumulate to be considered good
+    * algo: BaseAlgorithm - The class from StableBaselines3
+
+Obs: If not using StableBaselines, the expert has to have a `predict` function that receives:
+
+* obs: Tensor - Current environment state
+* state: Tensor - Model's internal state
+* deterministic: bool - If it should explore or not
+
+---
+## This repository is not complete
+
+Here is a list of the upcoming releases:
+
+- [x] Collate function support
+- [X] Support for installing as a dependency
+- [ ] Module for downloading trajectories from a Hugging Face dataset 
+- [ ] Create actual documentation
+- [X] Create some examples
+- [ ] Create tests
+ 
+---
+
+## If you like this repository be sure to check my other projects:
+
+### Development
+- [An easy to use Wrapper for Tensorboard](https://github.com/NathanGavenski/Tensorboard-Wrapper)
+- [A watcher for python to facilitate development of small projects](https://github.com/NathanGavenski/python-watcher)
+
+### Academic
+- [Imitating Unknown Policies via Exploration (BMVC)](https://arxiv.org/pdf/2008.05660.pdf)
+- [Augmented behavioral cloning from observation (IJCNN)](https://arxiv.org/pdf/2004.13529.pdf)
+- [Self-supervised imitation learning from observation (MSc dissertation)](https://repositorio.pucrs.br/dspace/bitstream/10923/17536/1/000500266-Texto%2Bcompleto-0.pdf)
+
```

### Comparing `il-datasets-0.0.1/src/il_datasets.egg-info/SOURCES.txt` & `il-datasets-0.1.0/src/il_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `il-datasets-0.0.1/src/imitation_datasets/args.py` & `il-datasets-0.1.0/src/imitation_datasets/args.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from argparse import ArgumentParser, Namespace
-
-def get_args() -> Namespace:
-    parser = ArgumentParser()
-    
-    parser.add_argument(
-        "-g", "--game", type=str, help="env name", required=True,
-    )
-    parser.add_argument(
-        "-e", "--episodes", default=10, type=int, help="number of episodes"
-    )
-    parser.add_argument(
-        "-t", "--threads", default=1, type=int, help="how many workers should the process execute",
-    )
-    parser.add_argument(
-        "--threshold", type=float, default=None, help="reward threshold for each execution",
-    )
-    parser.add_argument(
-        "--mode", default="play", choices=['all', 'play', 'collate'], type=str, help="reward threshold for each execution",
-    )
-
-    return parser.parse_args()
+from argparse import ArgumentParser, Namespace
+
+def get_args() -> Namespace:
+    parser = ArgumentParser()
+    
+    parser.add_argument(
+        "-g", "--game", type=str, help="env name", required=True,
+    )
+    parser.add_argument(
+        "-e", "--episodes", default=10, type=int, help="number of episodes"
+    )
+    parser.add_argument(
+        "-t", "--threads", default=1, type=int, help="how many workers should the process execute",
+    )
+    parser.add_argument(
+        "--threshold", type=float, default=None, help="reward threshold for each execution",
+    )
+    parser.add_argument(
+        "--mode", default="play", choices=['all', 'play', 'collate'], type=str, help="reward threshold for each execution",
+    )
+
+    return parser.parse_args()
```

### Comparing `il-datasets-0.0.1/src/imitation_datasets/experts.py` & `il-datasets-0.1.0/src/imitation_datasets/experts.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from dataclasses import dataclass, field
-from typing import Any, List, Tuple
-
-from huggingface_sb3 import load_from_hub
-from stable_baselines3.common.base_class import BaseAlgorithm
-
-from .register import atari, classic, mujoco
-
-
-@dataclass
-class Policy:
-    name: str
-    repo_id: str
-    filename: str
-    threshold: float
-    algo: BaseAlgorithm
-    policy: BaseAlgorithm = field(init=False, default=None)
-    internal_state: Any = field(init=False, default=None)
-
-    def load(self) -> None:
-        checkpoint = load_from_hub(
-            repo_id=self.repo_id,
-            filename=self.filename,
-        )
-
-        custom_objects = {
-            "learning_rate": 0.0,
-            "lr_schedule": lambda _: 0.0,
-            "clip_range": lambda _: 0.0
-        }
-        
-        self.policy = self.algo.load(
-            checkpoint, 
-            custom_objects=custom_objects
-        )
-        return self.policy
-
-    def predict(self, obs, deterministic: bool = True) -> Tuple[Any, Any]:
-            action, internal_states = self.policy.predict(
-                obs,
-                state=self.internal_state,
-                deterministic=deterministic,
-            )
-            self.internal_state = internal_states
-            return action, internal_states
-
-    def get_environment(self) -> str:
-        return self.name
-
-
-class Experts:
-
-    experts: List[Policy] = {key: Policy(**value) for env in [atari, classic, mujoco] for key, value in env.items()}
-
-    @classmethod
-    def register(cls, identifier: str, policy: Policy) -> None:
-        if not isinstance(policy.threshold, float):
-            policy.threshold = float(policy.threshold)
-        
-        cls.experts[identifier] = policy
-
-    @classmethod
-    def get_expert(cls, identifier: str) -> Policy:
-        return cls.experts[identifier]
-
-    @classmethod
-    def get_register(cls) -> str:
-        print(cls.experts)
+from dataclasses import dataclass, field
+from typing import Any, List, Tuple
+
+from huggingface_sb3 import load_from_hub
+from stable_baselines3.common.base_class import BaseAlgorithm
+
+from .register import atari, classic, mujoco
+
+
+@dataclass
+class Policy:
+    name: str
+    repo_id: str
+    filename: str
+    threshold: float
+    algo: BaseAlgorithm
+    policy: BaseAlgorithm = field(init=False, default=None)
+    internal_state: Any = field(init=False, default=None)
+
+    def load(self) -> None:
+        checkpoint = load_from_hub(
+            repo_id=self.repo_id,
+            filename=self.filename,
+        )
+
+        custom_objects = {
+            "learning_rate": 0.0,
+            "lr_schedule": lambda _: 0.0,
+            "clip_range": lambda _: 0.0
+        }
+        
+        self.policy = self.algo.load(
+            checkpoint, 
+            custom_objects=custom_objects
+        )
+        return self.policy
+
+    def predict(self, obs, deterministic: bool = True) -> Tuple[Any, Any]:
+            action, internal_states = self.policy.predict(
+                obs,
+                state=self.internal_state,
+                deterministic=deterministic,
+            )
+            self.internal_state = internal_states
+            return action, internal_states
+
+    def get_environment(self) -> str:
+        return self.name
+
+
+class Experts:
+
+    experts: List[Policy] = {key: Policy(**value) for env in [atari, classic, mujoco] for key, value in env.items()}
+
+    @classmethod
+    def register(cls, identifier: str, policy: Policy) -> None:
+        if not isinstance(policy.threshold, float):
+            policy.threshold = float(policy.threshold)
+        
+        cls.experts[identifier] = policy
+
+    @classmethod
+    def get_expert(cls, identifier: str) -> Policy:
+        return cls.experts[identifier]
+
+    @classmethod
+    def get_register(cls) -> str:
+        print(cls.experts)
```

### Comparing `il-datasets-0.0.1/src/imitation_datasets/register/atari.py` & `il-datasets-0.1.0/src/imitation_datasets/register/atari.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from stable_baselines3 import PPO
-from sb3_contrib import QRDQN
-
-atari = {
-    'asteroids': {
-        'name': 'AsteroidsNoFrameskip-v4',
-        'repo_id': "sb3/ppo-AsteroidsNoFrameskip-v4",
-        'filename': "ppo-AsteroidsNoFrameskip-v4.zip",
-        'threshold': 2439.,
-        'algo': PPO
-    },
-    'spaceinvaders': {
-        'name': 'SpaceInvadersNoFrameskip-v4',
-        'repo_id': 'meln1k/qrdqn-SpaceInvadersNoFrameskip-v4',
-        'filename': 'qrdqn-SpaceInvadersNoFrameskip-v4.zip',
-        'threshold': 2581.,
-        'algo': QRDQN
-    },
-    'breakout': {
-        'name': 'BreakoutNoFrameskip-v4',
-        'repo_id': 'sb3/ppo-BreakoutNoFrameskip-v4',
-        'filename': 'ppo-BreakoutNoFrameskip-v4.zip',
-        'threshold': 398.,
-        'algo': PPO
-    },
-    'qbert': {
-        'name': 'QbertNoFrameskip-v4',
-        'repo_id': 'Corianas/ppo-QbertNoFrameskip-v4_4',
-        'filename': 'ppo-QbertNoFrameskip-v4.zip',
-        'threshold': 19340.,
-        'algo': PPO
-    },
-    'beamrider': {
-        'name': 'BeamriderNoFrameskip-v4',
-        'repo_id': 'sb3/qrdqn-BeamRiderNoFrameskip-v4',
-        'filename': 'qrdqn-BeamRiderNoFrameskip-v4.zip',
-        'threshold': 15785.,
-        'algo': QRDQN
-    },
-    'pong': {
-        'name': 'PongNoFrameskip-v4',
-        'repo_id': 'sb3/ppo-PongNoFrameskip-v4',
-        'filename': 'ppo-PongNoFrameskip-v4.zip',
-        'threshold': 21.,
-        'algo': PPO
-    },
-    'enduro': {
-        'name': 'EnduroNoFrameskip-v4',
-        'repo_id': 'sb3/qrdqn-EnduroNoFrameskip-v4',
-        'filename': 'qrdqn-EnduroNoFrameskip-v4.zip',
-        'threshold': 2827.7,
-        'algo': QRDQN
-    },
-    'roadrunner': {
-        'name': 'RoadRunnerNoFrameskip-v4',
-        'repo_id': 'sb3/ppo-RoadRunnerNoFrameskip-v4',
-        'filename': 'ppo-RoadRunnerNoFrameskip-v4.zip',
-        'threshold': 970.,
-        'algo': PPO
-    },
-    'seaquest': {
-        'name': 'qrdqn-SeaquestNoFrameskip-v4',
-        'repo_id': 'sb3/qrdqn-SeaquestNoFrameskip-v4',
-        'filename': 'qrdqn-SeaquestNoFrameskip-v4.zip',
-        'threshold': 2562.,
-        'algo': QRDQN
-    }
+from stable_baselines3 import PPO
+from sb3_contrib import QRDQN
+
+atari = {
+    'asteroids': {
+        'name': 'AsteroidsNoFrameskip-v4',
+        'repo_id': "sb3/ppo-AsteroidsNoFrameskip-v4",
+        'filename': "ppo-AsteroidsNoFrameskip-v4.zip",
+        'threshold': 2439.,
+        'algo': PPO
+    },
+    'spaceinvaders': {
+        'name': 'SpaceInvadersNoFrameskip-v4',
+        'repo_id': 'meln1k/qrdqn-SpaceInvadersNoFrameskip-v4',
+        'filename': 'qrdqn-SpaceInvadersNoFrameskip-v4.zip',
+        'threshold': 2581.,
+        'algo': QRDQN
+    },
+    'breakout': {
+        'name': 'BreakoutNoFrameskip-v4',
+        'repo_id': 'sb3/ppo-BreakoutNoFrameskip-v4',
+        'filename': 'ppo-BreakoutNoFrameskip-v4.zip',
+        'threshold': 398.,
+        'algo': PPO
+    },
+    'qbert': {
+        'name': 'QbertNoFrameskip-v4',
+        'repo_id': 'Corianas/ppo-QbertNoFrameskip-v4_4',
+        'filename': 'ppo-QbertNoFrameskip-v4.zip',
+        'threshold': 19340.,
+        'algo': PPO
+    },
+    'beamrider': {
+        'name': 'BeamriderNoFrameskip-v4',
+        'repo_id': 'sb3/qrdqn-BeamRiderNoFrameskip-v4',
+        'filename': 'qrdqn-BeamRiderNoFrameskip-v4.zip',
+        'threshold': 15785.,
+        'algo': QRDQN
+    },
+    'pong': {
+        'name': 'PongNoFrameskip-v4',
+        'repo_id': 'sb3/ppo-PongNoFrameskip-v4',
+        'filename': 'ppo-PongNoFrameskip-v4.zip',
+        'threshold': 21.,
+        'algo': PPO
+    },
+    'enduro': {
+        'name': 'EnduroNoFrameskip-v4',
+        'repo_id': 'sb3/qrdqn-EnduroNoFrameskip-v4',
+        'filename': 'qrdqn-EnduroNoFrameskip-v4.zip',
+        'threshold': 2827.7,
+        'algo': QRDQN
+    },
+    'roadrunner': {
+        'name': 'RoadRunnerNoFrameskip-v4',
+        'repo_id': 'sb3/ppo-RoadRunnerNoFrameskip-v4',
+        'filename': 'ppo-RoadRunnerNoFrameskip-v4.zip',
+        'threshold': 970.,
+        'algo': PPO
+    },
+    'seaquest': {
+        'name': 'qrdqn-SeaquestNoFrameskip-v4',
+        'repo_id': 'sb3/qrdqn-SeaquestNoFrameskip-v4',
+        'filename': 'qrdqn-SeaquestNoFrameskip-v4.zip',
+        'threshold': 2562.,
+        'algo': QRDQN
+    }
 }
```

### Comparing `il-datasets-0.0.1/src/imitation_datasets/utils.py` & `il-datasets-0.1.0/src/imitation_datasets/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-import asyncio
-from collections import defaultdict
-from dataclasses import dataclass, field
-import multiprocessing
-import os
-from typing import Any, Callable, DefaultDict, Tuple, Union
-
-from .experts import Policy
-
-
-@dataclass
-class Experiment:
-    amount: int
-    path: str = './logs.txt'
-    waiting: int = field(init=False, default_factory=int)
-    logs: DefaultDict[int, list] = field(init=False, default_factory=lambda: defaultdict(list))
-    experiment_semaphore: asyncio.Lock = field(init=False, default=asyncio.BoundedSemaphore(value=1))
-
-    def __post_init__(self) -> None:
-        if not os.path.exists(self.path):
-            with open(self.path, 'w') as f:
-                f.write('#### Starting dataset creation ####\n')
-        else:
-            os.remove(self.path)
-
-    def is_done(self) -> bool:
-        return self.amount == 0
-
-    async def start(self, amount: int = 1) -> Union[bool, int]:
-        await self.experiment_semaphore.acquire()
-        if self.amount > 0:
-            self.waiting += amount
-            self.amount -= amount
-            self.experiment_semaphore.release()
-            return True, self.amount
-        else:
-            self.experiment_semaphore.release()
-            return False, -1
-
-    async def stop(self, status: bool, amount: int = 1) -> None:
-        await self.experiment_semaphore.acquire()
-        self.amount += -amount if status else amount
-        self.waiting -= amount
-        self.experiment_semaphore.release()
-
-    def add_log(self, experiment: int, log: str) -> None:
-        self.logs[experiment].append(log)
-
-    def write_log(self) -> None:
-        with open('./logs.txt', 'a') as f:
-            for idx, logs in self.logs.items():
-                for log in logs:
-                    f.write(f'\nExperiment {idx}: {log}')
-                f.write('\n')
-
-
-@dataclass
-class Context:
-    experiments: Experiment
-    index: int
-
-    def add_log(self, log: str) -> None:
-        self.experiments.add_log(self.index, log)
-
-
-@dataclass
-class CPUS:
-    available_cpus: int = field(default_factory=multiprocessing.cpu_count())
-    cpus: DefaultDict[int, bool] = field(init=False, default_factory=lambda: defaultdict(bool))
-    cpu_semaphore: asyncio.Lock = field(init=False)
-
-    def __post_init__(self) -> None:
-        if self.available_cpus > multiprocessing.cpu_count():
-            self.available_cpus = multiprocessing.cpu_count()
-        self.cpu_semaphore = asyncio.BoundedSemaphore(value=self.available_cpus)
-
-    async def cpu_allock(self) -> int:
-        await self.cpu_semaphore.acquire()
-        for idx in range(self.available_cpus):
-            if not self.cpus[idx]:
-                self.cpus[idx] = True
-                return idx
-    
-    def cpu_release(self, cpu_idx: int) -> None:
-        self.cpus[cpu_idx] = False
-        self.cpu_semaphore.release()
-
-EnjoyFunction = Callable[[Policy, str, Context], bool]
-CollateFunction = Callable[[str, list[str]], None]
+import asyncio
+from collections import defaultdict
+from dataclasses import dataclass, field
+import multiprocessing
+import os
+from typing import Any, Callable, DefaultDict, Tuple, Union
+
+from .experts import Policy
+
+
+@dataclass
+class Experiment:
+    amount: int
+    path: str = './logs.txt'
+    waiting: int = field(init=False, default_factory=int)
+    logs: DefaultDict[int, list] = field(init=False, default_factory=lambda: defaultdict(list))
+    experiment_semaphore: asyncio.Lock = field(init=False, default=asyncio.BoundedSemaphore(value=1))
+
+    def __post_init__(self) -> None:
+        if not os.path.exists(self.path):
+            with open(self.path, 'w') as f:
+                f.write('#### Starting dataset creation ####\n')
+        else:
+            os.remove(self.path)
+
+    def is_done(self) -> bool:
+        return self.amount == 0
+
+    async def start(self, amount: int = 1) -> Union[bool, int]:
+        await self.experiment_semaphore.acquire()
+        if self.amount > 0:
+            self.waiting += amount
+            self.amount -= amount
+            self.experiment_semaphore.release()
+            return True, self.amount
+        else:
+            self.experiment_semaphore.release()
+            return False, -1
+
+    async def stop(self, status: bool, amount: int = 1) -> None:
+        await self.experiment_semaphore.acquire()
+        self.amount += 0 if status else amount
+        self.waiting -= amount
+        self.experiment_semaphore.release()
+
+    def add_log(self, experiment: int, log: str) -> None:
+        self.logs[experiment].append(log)
+
+    def write_log(self) -> None:
+        with open('./logs.txt', 'a') as f:
+            for idx, logs in self.logs.items():
+                for log in logs:
+                    f.write(f'\nExperiment {idx}: {log}')
+                f.write('\n')
+
+
+@dataclass
+class Context:
+    experiments: Experiment
+    index: int
+
+    def add_log(self, log: str) -> None:
+        self.experiments.add_log(self.index, log)
+
+
+@dataclass
+class CPUS:
+    available_cpus: int = field(default_factory=multiprocessing.cpu_count())
+    cpus: DefaultDict[int, bool] = field(init=False, default_factory=lambda: defaultdict(bool))
+    cpu_semaphore: asyncio.Lock = field(init=False)
+
+    def __post_init__(self) -> None:
+        if self.available_cpus > multiprocessing.cpu_count():
+            self.available_cpus = multiprocessing.cpu_count()
+        self.cpu_semaphore = asyncio.BoundedSemaphore(value=self.available_cpus)
+
+    async def cpu_allock(self) -> int:
+        await self.cpu_semaphore.acquire()
+        for idx in range(self.available_cpus):
+            if not self.cpus[idx]:
+                self.cpus[idx] = True
+                return idx
+    
+    def cpu_release(self, cpu_idx: int) -> None:
+        self.cpus[cpu_idx] = False
+        self.cpu_semaphore.release()
+
+EnjoyFunction = Callable[[Policy, str, Context], bool]
+CollateFunction = Callable[[str, list[str]], None]
```

