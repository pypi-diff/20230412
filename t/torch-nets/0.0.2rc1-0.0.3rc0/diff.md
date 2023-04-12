# Comparing `tmp/torch-nets-0.0.2rc1.tar.gz` & `tmp/torch-nets-0.0.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-nets-0.0.2rc1.tar", last modified: Thu Jan  5 16:07:47 2023, max compression
+gzip compressed data, was "torch-nets-0.0.3rc0.tar", last modified: Wed Apr 12 16:53:35 2023, max compression
```

## Comparing `torch-nets-0.0.2rc1.tar` & `torch-nets-0.0.3rc0.tar`

### file list

```diff
@@ -1,22 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:07:47.734094 torch-nets-0.0.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-01-05 16:07:36.000000 torch-nets-0.0.2rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-01-05 16:07:47.734094 torch-nets-0.0.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-01-05 16:07:36.000000 torch-nets-0.0.2rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 16:07:47.734094 torch-nets-0.0.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-01-05 16:07:36.000000 torch-nets-0.0.2rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:07:47.730094 torch-nets-0.0.2rc1/torch_nets/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-01-05 16:07:36.000000 torch-nets-0.0.2rc1/torch_nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-01-05 16:07:36.000000 torch-nets-0.0.2rc1/torch_nets/_augmented_torch_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-01-05 16:07:36.000000 torch-nets-0.0.2rc1/torch_nets/_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-01-05 16:07:36.000000 torch-nets-0.0.2rc1/torch_nets/_torch_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:07:47.730094 torch-nets-0.0.2rc1/torch_nets/core/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-05 16:07:36.000000 torch-nets-0.0.2rc1/torch_nets/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-01-05 16:07:36.000000 torch-nets-0.0.2rc1/torch_nets/core/_base_torch_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-01-05 16:07:36.000000 torch-nets-0.0.2rc1/torch_nets/core/_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-01-05 16:07:36.000000 torch-nets-0.0.2rc1/torch_nets/core/_support_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:07:47.730094 torch-nets-0.0.2rc1/torch_nets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-01-05 16:07:47.000000 torch-nets-0.0.2rc1/torch_nets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-01-05 16:07:47.000000 torch-nets-0.0.2rc1/torch_nets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 16:07:47.000000 torch-nets-0.0.2rc1/torch_nets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-05 16:07:47.000000 torch-nets-0.0.2rc1/torch_nets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-05 16:07:47.000000 torch-nets-0.0.2rc1/torch_nets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:53:35.622441 torch-nets-0.0.3rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-12 16:53:35.622441 torch-nets-0.0.3rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:53:35.622441 torch-nets-0.0.3rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:53:35.618441 torch-nets-0.0.3rc0/torch_nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/_augmented_torch_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/_torch_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:53:35.622441 torch-nets-0.0.3rc0/torch_nets/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/core/_layer_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/core/_power_space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:53:35.622441 torch-nets-0.0.3rc0/torch_nets/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/core/config/_activation_function_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/core/config/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/core/config/_layer_wise_attributes_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/core/config/_network_structure_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:53:35.622441 torch-nets-0.0.3rc0/torch_nets/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/plotting/_plot_weights_and_biases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:53:35.622441 torch-nets-0.0.3rc0/torch_nets/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-12 16:53:23.000000 torch-nets-0.0.3rc0/torch_nets/tools/_infer_network_architecture_from_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:53:35.618441 torch-nets-0.0.3rc0/torch_nets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-12 16:53:35.000000 torch-nets-0.0.3rc0/torch_nets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 16:53:35.000000 torch-nets-0.0.3rc0/torch_nets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:53:35.000000 torch-nets-0.0.3rc0/torch_nets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 16:53:35.000000 torch-nets-0.0.3rc0/torch_nets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 16:53:35.000000 torch-nets-0.0.3rc0/torch_nets.egg-info/top_level.txt
```

### Comparing `torch-nets-0.0.2rc1/LICENSE` & `torch-nets-0.0.3rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.2rc1/PKG-INFO` & `torch-nets-0.0.3rc0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-nets
-Version: 0.0.2rc1
+Version: 0.0.3rc0
 Summary: API to compose PyTorch neural networks on the fly.
 Author: Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
@@ -20,50 +20,54 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 <a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a>
 
 Compose PyTorch neural networks with ease.
 
-#### Installation
+### Installation
 
-From PYPI (current version: [`v0.0.1`](https://pypi.org/project/torch-nets/0.0.1/))
+From PYPI (current version: [`v0.0.3rc0`](https://pypi.org/project/torch-nets))
 ```python
 pip install torch-nets
 ```
 
 Alternatively, install the development version from GitHub:
 ```shell
 git clone https://github.com/mvinyard/torch-nets.git;
 cd torch-nets; pip install -e .
 ```
 
-### Example API use-case
+### Example API use-cases
 
 ```python
 from torch_nets import TorchNet
 ```
 
 #### Create a feed-forward neural network
 
+The only required arguments are `in_features` and `out_features`. The network can be made as simple or complex as you want through optional parameters.
+
 ```python
 net = TorchNet(
     in_features=50,
     out_features=50,
     hidden=[400, 400],
     activation="LeakyReLU",
     dropout=0.2,
-    n_augment=0,
     bias=True,
     output_bias=True,
 )
-net
 ```
+<details>
+<summary>See output</summary>
+<br>
+    
 ```
-Sequential(
+TorchNet(
   (hidden_1): Sequential(
     (linear): Linear(in_features=50, out_features=400, bias=True)
     (dropout): Dropout(p=0.2, inplace=False)
     (activation): LeakyReLU(negative_slope=0.01)
   )
   (hidden_2): Sequential(
     (linear): Linear(in_features=400, out_features=400, bias=True)
@@ -72,13 +76,23 @@
   )
   (output): Sequential(
     (linear): Linear(in_features=400, out_features=50, bias=True)
   )
 )
 ```
 
-The only required arguments are `in_features` and `out_features`. The network can be made as simple or complex as you want through optional parameters.
+</details>
+
+
+### Documentation
+
+For more information, including examples of additional use-cases please visit the [**documentation**]() (coming soon)! Additional use-cases include: `Encoder`, `Decoder`, `AugmentedTorchNet`.
+
+
+### Potential future plans
 
+- Flexible composition of `torch.optim` funcs.
+- Potential `pytorch_lightning` use-cases.
 
-#### Potential future plans
+---
 
-- Composition of `torch.optim` funcs.
+**Problem?** Open an [**issue**](https://github.com/mvinyard/torch-nets/issues/new) or get in touch via [**email**](mailto:vinyard@g.harvard.edu).
```

#### html2text {}

```diff
@@ -1,30 +1,36 @@
-Metadata-Version: 2.1 Name: torch-nets Version: 0.0.2rc1 Summary: API to
+Metadata-Version: 2.1 Name: torch-nets Version: 0.0.3rc0 Summary: API to
 compose PyTorch neural networks on the fly. Author: Michael E. Vinyard -
 Harvard University - Broad Institute of MIT and Harvard - Massachussetts
 General Hospital Author-email: mvinyard@broadinstitute.org License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Programming
 Language :: Python :: 3.7 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Requires-Python:
 >3.7.0 Description-Content-Type: text/markdown License-File: LICENSE # Torch-
 Nets [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-
 nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version](https://
 badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code
 style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
 (https://github.com/psf/black) [ol-reliable-spongebob] Compose PyTorch neural
-networks with ease. #### Installation From PYPI (current version: [`v0.0.1`]
-(https://pypi.org/project/torch-nets/0.0.1/)) ```python pip install torch-nets
-``` Alternatively, install the development version from GitHub: ```shell git
-clone https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -
-e . ``` ### Example API use-case ```python from torch_nets import TorchNet ```
-#### Create a feed-forward neural network ```python net = TorchNet
+networks with ease. ### Installation From PYPI (current version: [`v0.0.3rc0`]
+(https://pypi.org/project/torch-nets)) ```python pip install torch-nets ```
+Alternatively, install the development version from GitHub: ```shell git clone
+https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
+### Example API use-cases ```python from torch_nets import TorchNet ``` ####
+Create a feed-forward neural network The only required arguments are
+`in_features` and `out_features`. The network can be made as simple or complex
+as you want through optional parameters. ```python net = TorchNet
 ( in_features=50, out_features=50, hidden=[400, 400], activation="LeakyReLU",
-dropout=0.2, n_augment=0, bias=True, output_bias=True, ) net ``` ``` Sequential
-( (hidden_1): Sequential( (linear): Linear(in_features=50, out_features=400,
-bias=True) (dropout): Dropout(p=0.2, inplace=False) (activation): LeakyReLU
-(negative_slope=0.01) ) (hidden_2): Sequential( (linear): Linear
-(in_features=400, out_features=400, bias=True) (dropout): Dropout(p=0.2,
-inplace=False) (activation): LeakyReLU(negative_slope=0.01) ) (output):
-Sequential( (linear): Linear(in_features=400, out_features=50, bias=True) ) )
-``` The only required arguments are `in_features` and `out_features`. The
-network can be made as simple or complex as you want through optional
-parameters. #### Potential future plans - Composition of `torch.optim` funcs.
+dropout=0.2, bias=True, output_bias=True, ) ```  See output
+``` TorchNet( (hidden_1): Sequential( (linear): Linear(in_features=50,
+out_features=400, bias=True) (dropout): Dropout(p=0.2, inplace=False)
+(activation): LeakyReLU(negative_slope=0.01) ) (hidden_2): Sequential(
+(linear): Linear(in_features=400, out_features=400, bias=True) (dropout):
+Dropout(p=0.2, inplace=False) (activation): LeakyReLU(negative_slope=0.01) )
+(output): Sequential( (linear): Linear(in_features=400, out_features=50,
+bias=True) ) ) ```  ### Documentation For more information, including examples
+of additional use-cases please visit the [**documentation**]() (coming soon)!
+Additional use-cases include: `Encoder`, `Decoder`, `AugmentedTorchNet`. ###
+Potential future plans - Flexible composition of `torch.optim` funcs. -
+Potential `pytorch_lightning` use-cases. --- **Problem?** Open an [**issue**]
+(https://github.com/mvinyard/torch-nets/issues/new) or get in touch via
+[**email**](mailto:vinyard@g.harvard.edu).
```

### Comparing `torch-nets-0.0.2rc1/README.md` & `torch-nets-0.0.3rc0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,50 +5,54 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 <a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a>
 
 Compose PyTorch neural networks with ease.
 
-#### Installation
+### Installation
 
-From PYPI (current version: [`v0.0.1`](https://pypi.org/project/torch-nets/0.0.1/))
+From PYPI (current version: [`v0.0.3rc0`](https://pypi.org/project/torch-nets))
 ```python
 pip install torch-nets
 ```
 
 Alternatively, install the development version from GitHub:
 ```shell
 git clone https://github.com/mvinyard/torch-nets.git;
 cd torch-nets; pip install -e .
 ```
 
-### Example API use-case
+### Example API use-cases
 
 ```python
 from torch_nets import TorchNet
 ```
 
 #### Create a feed-forward neural network
 
+The only required arguments are `in_features` and `out_features`. The network can be made as simple or complex as you want through optional parameters.
+
 ```python
 net = TorchNet(
     in_features=50,
     out_features=50,
     hidden=[400, 400],
     activation="LeakyReLU",
     dropout=0.2,
-    n_augment=0,
     bias=True,
     output_bias=True,
 )
-net
 ```
+<details>
+<summary>See output</summary>
+<br>
+    
 ```
-Sequential(
+TorchNet(
   (hidden_1): Sequential(
     (linear): Linear(in_features=50, out_features=400, bias=True)
     (dropout): Dropout(p=0.2, inplace=False)
     (activation): LeakyReLU(negative_slope=0.01)
   )
   (hidden_2): Sequential(
     (linear): Linear(in_features=400, out_features=400, bias=True)
@@ -57,13 +61,23 @@
   )
   (output): Sequential(
     (linear): Linear(in_features=400, out_features=50, bias=True)
   )
 )
 ```
 
-The only required arguments are `in_features` and `out_features`. The network can be made as simple or complex as you want through optional parameters.
+</details>
+
+
+### Documentation
+
+For more information, including examples of additional use-cases please visit the [**documentation**]() (coming soon)! Additional use-cases include: `Encoder`, `Decoder`, `AugmentedTorchNet`.
+
+
+### Potential future plans
 
+- Flexible composition of `torch.optim` funcs.
+- Potential `pytorch_lightning` use-cases.
 
-#### Potential future plans
+---
 
-- Composition of `torch.optim` funcs.
+**Problem?** Open an [**issue**](https://github.com/mvinyard/torch-nets/issues/new) or get in touch via [**email**](mailto:vinyard@g.harvard.edu).
```

#### html2text {}

```diff
@@ -1,22 +1,28 @@
 # Torch-Nets [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-
 nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version](https://
 badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code
 style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
 (https://github.com/psf/black) [ol-reliable-spongebob] Compose PyTorch neural
-networks with ease. #### Installation From PYPI (current version: [`v0.0.1`]
-(https://pypi.org/project/torch-nets/0.0.1/)) ```python pip install torch-nets
-``` Alternatively, install the development version from GitHub: ```shell git
-clone https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -
-e . ``` ### Example API use-case ```python from torch_nets import TorchNet ```
-#### Create a feed-forward neural network ```python net = TorchNet
+networks with ease. ### Installation From PYPI (current version: [`v0.0.3rc0`]
+(https://pypi.org/project/torch-nets)) ```python pip install torch-nets ```
+Alternatively, install the development version from GitHub: ```shell git clone
+https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
+### Example API use-cases ```python from torch_nets import TorchNet ``` ####
+Create a feed-forward neural network The only required arguments are
+`in_features` and `out_features`. The network can be made as simple or complex
+as you want through optional parameters. ```python net = TorchNet
 ( in_features=50, out_features=50, hidden=[400, 400], activation="LeakyReLU",
-dropout=0.2, n_augment=0, bias=True, output_bias=True, ) net ``` ``` Sequential
-( (hidden_1): Sequential( (linear): Linear(in_features=50, out_features=400,
-bias=True) (dropout): Dropout(p=0.2, inplace=False) (activation): LeakyReLU
-(negative_slope=0.01) ) (hidden_2): Sequential( (linear): Linear
-(in_features=400, out_features=400, bias=True) (dropout): Dropout(p=0.2,
-inplace=False) (activation): LeakyReLU(negative_slope=0.01) ) (output):
-Sequential( (linear): Linear(in_features=400, out_features=50, bias=True) ) )
-``` The only required arguments are `in_features` and `out_features`. The
-network can be made as simple or complex as you want through optional
-parameters. #### Potential future plans - Composition of `torch.optim` funcs.
+dropout=0.2, bias=True, output_bias=True, ) ```  See output
+``` TorchNet( (hidden_1): Sequential( (linear): Linear(in_features=50,
+out_features=400, bias=True) (dropout): Dropout(p=0.2, inplace=False)
+(activation): LeakyReLU(negative_slope=0.01) ) (hidden_2): Sequential(
+(linear): Linear(in_features=400, out_features=400, bias=True) (dropout):
+Dropout(p=0.2, inplace=False) (activation): LeakyReLU(negative_slope=0.01) )
+(output): Sequential( (linear): Linear(in_features=400, out_features=50,
+bias=True) ) ) ```  ### Documentation For more information, including examples
+of additional use-cases please visit the [**documentation**]() (coming soon)!
+Additional use-cases include: `Encoder`, `Decoder`, `AugmentedTorchNet`. ###
+Potential future plans - Flexible composition of `torch.optim` funcs. -
+Potential `pytorch_lightning` use-cases. --- **Problem?** Open an [**issue**]
+(https://github.com/mvinyard/torch-nets/issues/new) or get in touch via
+[**email**](mailto:vinyard@g.harvard.edu).
```

### Comparing `torch-nets-0.0.2rc1/setup.py` & `torch-nets-0.0.3rc0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 import re
 import os
 import sys
 
 
 setuptools.setup(
     name="torch-nets",
-    version="0.0.2rc1",
+    version="0.0.3rc0",
     python_requires=">3.7.0",
     author="Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital",
     author_email="mvinyard@broadinstitute.org",
     url=None,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="API to compose PyTorch neural networks on the fly.",
     packages=setuptools.find_packages(),
     install_requires=[
         "torch>=1.12",
+        "ABCParse>=0.0.3",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python :: 3.7",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
```

### Comparing `torch-nets-0.0.2rc1/torch_nets/__init__.py` & `torch-nets-0.0.3rc0/torch_nets/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 
 __module_name__ = "__init__.py"
 __doc__ = """Main API __init__.py module."""
 __author__ = ", ".join(["Michael E. Vinyard"])
 __email__ = ", ".join(["vinyard@g.harvard.edu",])
-__version__ = "0.0.2"
+__version__ = "0.0.3rc0"
 
 
 # -- import network modules: -------------------------------------------------------------
-from ._torch_net import _torch_net as TorchNet
-from ._encoder_decoder import Encoder, Decoder
+from ._torch_net import TorchNet
+from ._encoder import Encoder
+from ._decoder import Decoder
 from ._augmented_torch_net import AugmentedTorchNet
 
 
 # -- import API core: --------------------------------------------------------------------
 from . import core
+from . import tools as tl
+from . import plotting as pl
```

### Comparing `torch-nets-0.0.2rc1/torch_nets.egg-info/PKG-INFO` & `torch-nets-0.0.3rc0/torch_nets.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-nets
-Version: 0.0.2rc1
+Version: 0.0.3rc0
 Summary: API to compose PyTorch neural networks on the fly.
 Author: Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
@@ -20,50 +20,54 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 <a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a>
 
 Compose PyTorch neural networks with ease.
 
-#### Installation
+### Installation
 
-From PYPI (current version: [`v0.0.1`](https://pypi.org/project/torch-nets/0.0.1/))
+From PYPI (current version: [`v0.0.3rc0`](https://pypi.org/project/torch-nets))
 ```python
 pip install torch-nets
 ```
 
 Alternatively, install the development version from GitHub:
 ```shell
 git clone https://github.com/mvinyard/torch-nets.git;
 cd torch-nets; pip install -e .
 ```
 
-### Example API use-case
+### Example API use-cases
 
 ```python
 from torch_nets import TorchNet
 ```
 
 #### Create a feed-forward neural network
 
+The only required arguments are `in_features` and `out_features`. The network can be made as simple or complex as you want through optional parameters.
+
 ```python
 net = TorchNet(
     in_features=50,
     out_features=50,
     hidden=[400, 400],
     activation="LeakyReLU",
     dropout=0.2,
-    n_augment=0,
     bias=True,
     output_bias=True,
 )
-net
 ```
+<details>
+<summary>See output</summary>
+<br>
+    
 ```
-Sequential(
+TorchNet(
   (hidden_1): Sequential(
     (linear): Linear(in_features=50, out_features=400, bias=True)
     (dropout): Dropout(p=0.2, inplace=False)
     (activation): LeakyReLU(negative_slope=0.01)
   )
   (hidden_2): Sequential(
     (linear): Linear(in_features=400, out_features=400, bias=True)
@@ -72,13 +76,23 @@
   )
   (output): Sequential(
     (linear): Linear(in_features=400, out_features=50, bias=True)
   )
 )
 ```
 
-The only required arguments are `in_features` and `out_features`. The network can be made as simple or complex as you want through optional parameters.
+</details>
+
+
+### Documentation
+
+For more information, including examples of additional use-cases please visit the [**documentation**]() (coming soon)! Additional use-cases include: `Encoder`, `Decoder`, `AugmentedTorchNet`.
+
+
+### Potential future plans
 
+- Flexible composition of `torch.optim` funcs.
+- Potential `pytorch_lightning` use-cases.
 
-#### Potential future plans
+---
 
-- Composition of `torch.optim` funcs.
+**Problem?** Open an [**issue**](https://github.com/mvinyard/torch-nets/issues/new) or get in touch via [**email**](mailto:vinyard@g.harvard.edu).
```

#### html2text {}

```diff
@@ -1,30 +1,36 @@
-Metadata-Version: 2.1 Name: torch-nets Version: 0.0.2rc1 Summary: API to
+Metadata-Version: 2.1 Name: torch-nets Version: 0.0.3rc0 Summary: API to
 compose PyTorch neural networks on the fly. Author: Michael E. Vinyard -
 Harvard University - Broad Institute of MIT and Harvard - Massachussetts
 General Hospital Author-email: mvinyard@broadinstitute.org License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Programming
 Language :: Python :: 3.7 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Requires-Python:
 >3.7.0 Description-Content-Type: text/markdown License-File: LICENSE # Torch-
 Nets [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-
 nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version](https://
 badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code
 style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
 (https://github.com/psf/black) [ol-reliable-spongebob] Compose PyTorch neural
-networks with ease. #### Installation From PYPI (current version: [`v0.0.1`]
-(https://pypi.org/project/torch-nets/0.0.1/)) ```python pip install torch-nets
-``` Alternatively, install the development version from GitHub: ```shell git
-clone https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -
-e . ``` ### Example API use-case ```python from torch_nets import TorchNet ```
-#### Create a feed-forward neural network ```python net = TorchNet
+networks with ease. ### Installation From PYPI (current version: [`v0.0.3rc0`]
+(https://pypi.org/project/torch-nets)) ```python pip install torch-nets ```
+Alternatively, install the development version from GitHub: ```shell git clone
+https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
+### Example API use-cases ```python from torch_nets import TorchNet ``` ####
+Create a feed-forward neural network The only required arguments are
+`in_features` and `out_features`. The network can be made as simple or complex
+as you want through optional parameters. ```python net = TorchNet
 ( in_features=50, out_features=50, hidden=[400, 400], activation="LeakyReLU",
-dropout=0.2, n_augment=0, bias=True, output_bias=True, ) net ``` ``` Sequential
-( (hidden_1): Sequential( (linear): Linear(in_features=50, out_features=400,
-bias=True) (dropout): Dropout(p=0.2, inplace=False) (activation): LeakyReLU
-(negative_slope=0.01) ) (hidden_2): Sequential( (linear): Linear
-(in_features=400, out_features=400, bias=True) (dropout): Dropout(p=0.2,
-inplace=False) (activation): LeakyReLU(negative_slope=0.01) ) (output):
-Sequential( (linear): Linear(in_features=400, out_features=50, bias=True) ) )
-``` The only required arguments are `in_features` and `out_features`. The
-network can be made as simple or complex as you want through optional
-parameters. #### Potential future plans - Composition of `torch.optim` funcs.
+dropout=0.2, bias=True, output_bias=True, ) ```  See output
+``` TorchNet( (hidden_1): Sequential( (linear): Linear(in_features=50,
+out_features=400, bias=True) (dropout): Dropout(p=0.2, inplace=False)
+(activation): LeakyReLU(negative_slope=0.01) ) (hidden_2): Sequential(
+(linear): Linear(in_features=400, out_features=400, bias=True) (dropout):
+Dropout(p=0.2, inplace=False) (activation): LeakyReLU(negative_slope=0.01) )
+(output): Sequential( (linear): Linear(in_features=400, out_features=50,
+bias=True) ) ) ```  ### Documentation For more information, including examples
+of additional use-cases please visit the [**documentation**]() (coming soon)!
+Additional use-cases include: `Encoder`, `Decoder`, `AugmentedTorchNet`. ###
+Potential future plans - Flexible composition of `torch.optim` funcs. -
+Potential `pytorch_lightning` use-cases. --- **Problem?** Open an [**issue**]
+(https://github.com/mvinyard/torch-nets/issues/new) or get in touch via
+[**email**](mailto:vinyard@g.harvard.edu).
```

