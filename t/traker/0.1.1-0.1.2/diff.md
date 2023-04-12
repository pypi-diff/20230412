# Comparing `tmp/traker-0.1.1.tar.gz` & `tmp/traker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traker-0.1.1.tar", last modified: Thu Mar 23 05:08:56 2023, max compression
+gzip compressed data, was "traker-0.1.2.tar", last modified: Wed Apr 12 17:51:30 2023, max compression
```

## Comparing `traker-0.1.1.tar` & `traker-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-03-23 05:08:56.391636 traker-0.1.1/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-03-23 05:08:56.383636 traker-0.1.1/PKG-INFO
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     2600 2023-03-23 05:07:57.000000 traker-0.1.1/README.md
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       38 2023-03-23 05:08:56.395636 traker-0.1.1/setup.cfg
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      756 2023-03-23 05:07:59.000000 traker-0.1.1/setup.py
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-03-23 05:08:56.027630 traker-0.1.1/tests/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     2989 2023-03-23 05:07:59.000000 traker-0.1.1/tests/test_cifar_accuracy.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3810 2023-03-19 02:36:41.000000 traker-0.1.1/tests/test_class.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4571 2023-03-19 02:36:41.000000 traker-0.1.1/tests/test_integration_cifar.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1545 2023-03-23 05:07:59.000000 traker-0.1.1/tests/test_integration_clip.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    10812 2023-03-19 02:36:41.000000 traker-0.1.1/tests/test_jl.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4065 2023-03-23 05:07:59.000000 traker-0.1.1/tests/test_parallel.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1601 2023-03-19 02:36:41.000000 traker-0.1.1/tests/test_rademacher.py
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-03-23 05:08:56.227634 traker-0.1.1/trak/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       72 2023-03-23 05:07:59.000000 traker-0.1.1/trak/__init__.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     7952 2023-03-19 02:36:47.000000 traker-0.1.1/trak/gradient_computers.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    19273 2023-03-23 05:07:59.000000 traker-0.1.1/trak/modelout_functions.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     9315 2023-03-19 02:36:41.000000 traker-0.1.1/trak/projectors.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    12301 2023-03-23 05:07:59.000000 traker-0.1.1/trak/savers.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3499 2023-03-19 02:36:41.000000 traker-0.1.1/trak/score_computers.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    16391 2023-03-23 05:07:59.000000 traker-0.1.1/trak/traker.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1461 2023-03-19 02:36:41.000000 traker-0.1.1/trak/utils.py
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-03-23 05:08:56.359635 traker-0.1.1/traker.egg-info/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-03-23 05:08:54.000000 traker-0.1.1/traker.egg-info/PKG-INFO
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      502 2023-03-23 05:08:55.000000 traker-0.1.1/traker.egg-info/SOURCES.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        1 2023-03-23 05:08:54.000000 traker-0.1.1/traker.egg-info/dependency_links.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       96 2023-03-23 05:08:54.000000 traker-0.1.1/traker.egg-info/requires.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        5 2023-03-23 05:08:54.000000 traker-0.1.1/traker.egg-info/top_level.txt
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-12 17:51:30.688856 traker-0.1.2/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-04-12 17:51:30.676856 traker-0.1.2/PKG-INFO
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3311 2023-04-10 13:58:42.000000 traker-0.1.2/README.md
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       38 2023-04-12 17:51:30.692856 traker-0.1.2/setup.cfg
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      756 2023-04-12 17:48:19.000000 traker-0.1.2/setup.py
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-12 17:51:30.240849 traker-0.1.2/tests/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     5575 2023-04-12 13:40:47.000000 traker-0.1.2/tests/test_accuracy.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     2989 2023-04-11 13:28:04.000000 traker-0.1.2/tests/test_cifar_accuracy.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4143 2023-04-10 13:58:43.000000 traker-0.1.2/tests/test_class.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4571 2023-03-27 15:11:24.000000 traker-0.1.2/tests/test_integration_cifar.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1545 2023-03-27 15:11:24.000000 traker-0.1.2/tests/test_integration_clip.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    10812 2023-03-27 15:11:24.000000 traker-0.1.2/tests/test_jl.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4065 2023-03-27 15:11:24.000000 traker-0.1.2/tests/test_parallel.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3116 2023-04-12 17:48:19.000000 traker-0.1.2/tests/test_rademacher.py
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-12 17:51:30.468853 traker-0.1.2/trak/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       72 2023-04-12 17:48:19.000000 traker-0.1.2/trak/__init__.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     8766 2023-03-28 20:01:05.000000 traker-0.1.2/trak/gradient_computers.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    20281 2023-04-12 17:48:19.000000 traker-0.1.2/trak/modelout_functions.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    11180 2023-04-12 17:48:19.000000 traker-0.1.2/trak/projectors.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    12660 2023-03-27 15:11:24.000000 traker-0.1.2/trak/savers.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3499 2023-03-27 15:11:24.000000 traker-0.1.2/trak/score_computers.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    16926 2023-04-12 17:48:19.000000 traker-0.1.2/trak/traker.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1527 2023-03-27 15:11:24.000000 traker-0.1.2/trak/utils.py
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-12 17:51:30.640855 traker-0.1.2/traker.egg-info/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-04-12 17:51:28.000000 traker-0.1.2/traker.egg-info/PKG-INFO
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      525 2023-04-12 17:51:28.000000 traker-0.1.2/traker.egg-info/SOURCES.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        1 2023-04-12 17:51:28.000000 traker-0.1.2/traker.egg-info/dependency_links.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       96 2023-04-12 17:51:28.000000 traker-0.1.2/traker.egg-info/requires.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        5 2023-04-12 17:51:28.000000 traker-0.1.2/traker.egg-info/top_level.txt
```

### Comparing `traker-0.1.1/README.md` & `traker-0.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,101 @@
-[![Python package](https://github.com/MadryLab/trak/actions/workflows/python-package.yml/badge.svg)](https://github.com/MadryLab/trak/actions/workflows/python-package.yml)
-<!-- [![arXiv](https://img.shields.io/badge/arXiv-1234.56789-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/1234.56789) -->
+[![PyPI version](https://badge.fury.io/py/traker.svg)](https://badge.fury.io/py/traker)
+[![arXiv](https://img.shields.io/badge/arXiv-2303.14186-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2303.14186)
 
-[[docs & tutorials]](https://trak.csail.mit.edu/html/index.html)
-[[paper]](https://gradientscience.org/trak.pdf)
+[[docs & tutorials]](https://trak.readthedocs.io/en/latest/)
+[[paper]](https://arxiv.org/abs/2303.14186)
 [[blog post]](https://gradientscience.org/trak/)
 [[website]](https://trak.csail.mit.edu)
-[[PyPI]](https://pypi.org/project/traker/)
 
 # TRAK: Attributing Model Behavior at Scale
 
-In our recent [paper](TODO:link), we introduce `TRAK` (Tracing with the
-Randomly-Projected After Kernel). In short, `TRAK` scores can make accurate
+In our [paper](https://arxiv.org/abs/2303.14186), we introduce a new data attribution method called `TRAK` (Tracing with the
+Randomly-Projected After Kernel). Using `TRAK`, you can make  accurate
 counterfactual predictions (e.g., answers to questions of the form “what would
-happen to this prediction if these images were removed from the training set").
-Furthermore, these scores come at a small fraction of the cost of prior methods
-that are comparably effective (e.g., TRAK is 2-3 orders of magnitude cheaper
-than comparable methods, on CIFAR-10 and QNLI):
+happen to this prediction if these examples are removed from the training set?").
+Computing  data attribution with  TRAK is 2-3 orders of magnitude cheaper than
+comparably effective methods, e.g., see our evaluation on:
 
 ![Main figure](/docs/assets/main_figure.png)
 
+## Citation
+If you use this code in your work, please cite using the following BibTeX entry:
+```
+@inproceedings{park2023trak,
+  title = {TRAK: Attributing Model Behavior at Scale},
+  author = {Sung Min Park and Kristian Georgiev and Andrew Ilyas and Guillaume Leclerc and Aleksander Madry},
+  booktitle = {Arxiv preprint arXiv:2303.14186},
+  year = {2023}
+}
+```
+
 ## Usage
 
-Check [our docs](https://trak.csail.mit.edu/html) for more detailed examples and
-tutorials on how to use `TRAK`.  Below, we provide a brief blueprint of the
-steps needed to get `TRAK` attribution scores with our API.
 
-### Setting up the `TRAK` scorer
+[[Quickstart]](https://trak.readthedocs.io/en/latest/quickstart.html)
+
+Check [our docs](https://trak.readthedocs.io/en/latest/) for more detailed examples and
+tutorials on how to use `TRAK`.  Below, we provide a brief blueprint of using `TRAK`'s API to compute attribution scores.
+
+### Make a `TRAKer` instance
 
 ```python
 from trak import TRAKer
 
 model, checkpoints = ...
 train_loader = ...
 
 traker = TRAKer(model=model, task='image_classification', train_set_size=...)
 ```
 
-### Getting `TRAK` features for the train data
+### Compute `TRAK` features on training data
 
 ```python
 for model_id, checkpoint in enumerate(checkpoints):
   traker.load_checkpoint(ckeckpoint, model_id=model_id)
   for batch in loader_train:
+      # batch should be a tuple of inputs and labels
       traker.featurize(batch=batch, ...)
 traker.finalize_features()
 ```
 
-### Getting `TRAK` scores
+### Compute `TRAK` scores for target examples
 
 ```python
 targets_loader = ...
 
 for model_id, checkpoint in enumerate(checkpoints):
   traker.start_scoring_checkpoint(ckeckpoint, model_id=model_id, num_targets=...)
   for batch in targets_loader:
     traker.score(batch=batch, ...)
 
 scores = traker.finalize_scores()
 ```
 
+## Examples
+You can find several end-to-end examples in the `examples/` directory.
+
 ## Installation
 
 To install the version of our package which contains a fast, custom `CUDA`
 kernel for the JL projection step, use
 ```bash
 pip install traker[fast]
 ```
 You will need compatible versions of `gcc` and `CUDA toolkit` to install it. See
-the [installation FAQs](https://trak.csail.mit.edu/html/install.html) for tips
+the [installation FAQs](https://trak.readthedocs.io/en/latest/install.html) for tips
 regarding this. To install the basic version of our package that requires no
 compilation, use
 ```bash
 pip install traker
 ```
+
+## Questions?
+
+Please send an email to trak@mit.edu
+
+## Maintainers:
+
+[Kristian Georgiev](https://twitter.com/kris_georgiev1)<br>
+[Andrew Ilyas](https://twitter.com/andrew_ilyas)<br>
+[Guillaume Leclerc](https://twitter.com/gpoleclerc)<br>
+[Sung Min Park](https://twitter.com/smsampark)
```

### Comparing `traker-0.1.1/setup.py` & `traker-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(name="traker",
-      version="0.1.1",
+      version="0.1.2",
       description="TRAK: Attributing Model Behavior at Scale",
       long_description="Check https://trak.csail.mit.edu/ to learn more about TRAK",
       author="MadryLab",
       author_email='trak@mit.edu',
       license_files=('LICENSE.txt', ),
       packages=['trak'],
       install_requires=[
```

### Comparing `traker-0.1.1/tests/test_cifar_accuracy.py` & `traker-0.1.2/tests/test_cifar_accuracy.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.1/tests/test_class.py` & `traker-0.1.2/tests/test_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from trak import TRAKer
 from torchvision.models import resnet18
 import pytest
 import torch as ch
 from trak.projectors import BasicProjector
+from trak.modelout_functions import ImageClassificationModelOutput
 
 
 @pytest.fixture
 def cpu_proj():
     projector = BasicProjector(grad_dim=11689512,
                                proj_dim=20,
                                seed=0,
@@ -113,7 +114,17 @@
     traker.load_checkpoint(ckpt, model_id=0)
     traker.featurize(batch, num_samples=N)
     traker.finalize_features()
 
     traker.start_scoring_checkpoint(ckpt, 0, num_targets=N)
     traker.score(batch, num_samples=N)
     traker.finalize_scores()
+
+
+def test_custom_model_output(tmp_path, cpu_proj):
+    model = resnet18()
+    TRAKer(model=model,
+           task=ImageClassificationModelOutput,
+           save_dir=tmp_path,
+           projector=cpu_proj,
+           train_set_size=20,
+           device='cuda:0')
```

### Comparing `traker-0.1.1/tests/test_integration_cifar.py` & `traker-0.1.2/tests/test_integration_cifar.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.1/tests/test_integration_clip.py` & `traker-0.1.2/tests/test_integration_clip.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.1/tests/test_jl.py` & `traker-0.1.2/tests/test_jl.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.1/tests/test_parallel.py` & `traker-0.1.2/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.1/trak/gradient_computers.py` & `traker-0.1.2/trak/gradient_computers.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,45 +8,50 @@
 try:
     from functorch import grad, vmap, make_functional_with_buffers
 except ImportError:
     print('Cannot import `functorch`. Functional mode cannot be used.')
 
 
 class AbstractGradientComputer(ABC):
-    """
-    Implementations of the GradientComputer class should allow for per-sample
-    gradients.
-    This is behavior is enabled with three methods:
-    - the `load_model_params` method, well, loads model parameters. It can be as
-      simple as a self.model.load_state_dict(..)
-    - the `compute_per_sample_grad` method computes per-sample gradients of the
-      chosen model output function with respect to the model's parameters.
-    - the `compute_loss_grad` method computes the gradients of the loss function
-       with respect to the model output (which should be a scalar) for every
-       sample.
-
-    The class attribute `is_functional` is used to determine what implementation
-    of ModelOutput to use, i.e. whether it should use `functorch`'s functional
-    models.
+    """ Implementations of the GradientComputer class should allow for
+    per-sample gradients.  This is behavior is enabled with three methods:
+
+    - the :meth:`.load_model_params` method, well, loads model parameters. It can
+      be as simple as a :code:`self.model.load_state_dict(..)`
+
+    - the :meth:`.compute_per_sample_grad` method computes per-sample gradients
+      of the chosen model output function with respect to the model's parameters.
+
+    - the :meth:`.compute_loss_grad` method computes the gradients of the loss
+      function with respect to the model output (which should be a scalar) for
+      every sample.
+
+    The class attribute :code:`is_functional` is used to determine what
+    implementation of ModelOutput to use, i.e. whether it should use
+    :code:`functorch`'s functional models.
     """
     is_functional = True
 
     @abstractmethod
     def __init__(self,
                  model: torch.nn.Module,
                  modelout_fn: AbstractModelOutput,
                  grad_dim: Optional[int] = None,
                  ) -> None:
         """ Initializes attributes, nothing too interesting happening.
 
         Args:
-            model (torch.nn.Module): model
-            modelout_fn (AbstractModelOutput): model output function
-            grad_dim (int, optional): Size of the gradients (number of model
-                parameters). Defaults to None.
+            model (torch.nn.Module):
+                model
+            modelout_fn (AbstractModelOutput):
+                model output function
+            grad_dim (int, optional):
+                Size of the gradients (number of model parameters). Defaults to
+                None.
+
         """
         self.model = model
         self.modelout_fn = modelout_fn()
         self.grad_dim = grad_dim
 
     @abstractmethod
     def load_model_params(self, model) -> None:
@@ -72,61 +77,77 @@
     def load_model_params(self, model) -> None:
         """ Given a a torch.nn.Module model, inits/updates the func_model, along
         with its weights and buffers. See
         https://pytorch.org/functorch/stable/generated/functorch.make_functional_with_buffers.html#functorch-make-functional-with-buffers
         for more details on `functorch`'s functional models.
 
         Args:
-            model (torch.nn.Module): model to load
+            model (torch.nn.Module):
+                model to load
+
         """
         self.func_model, self.func_weights, self.func_buffers = make_functional_with_buffers(model)
         self.params_dict = get_params_dict(model)
 
     def compute_per_sample_grad(self,
                                 batch: Iterable[Tensor],
                                 batch_size: Optional[int] = None,
                                 ) -> Tensor:
-        """ Uses functorch's vmap (see
+        """ Uses functorch's :code:`vmap` (see
         https://pytorch.org/functorch/stable/generated/functorch.vmap.html#functorch.vmap
         for more details) to vectorize the computations of per-sample gradients.
 
-        Doesn't use `batch_size`; only added to follow the abstract method signature.
+        Doesn't use :code:`batch_size`; only added to follow the abstract method
+        signature.
 
         Args:
-            batch (Iterable[Tensor]): batch of data
-            batch_size (int, optional): Defaults to None.
+            batch (Iterable[Tensor]):
+                batch of data
+            batch_size (int, optional):
+                Defaults to None.
 
         Returns:
-            Tensor: gradients of the model output function of each sample in the batch
-                with respect to the model's parameters.
+            Tensor:
+                gradients of the model output function of each sample in the
+                batch with respect to the model's parameters.
+
         """
         # taking the gradient wrt weights (second argument of get_output, hence argnums=1)
         grads_loss = grad(self.modelout_fn.get_output, has_aux=False, argnums=1)
         # map over batch dimensions (hence 0 for each batch dimension, and None for model params)
         grads = vmap(grads_loss,
                      in_dims=(None, None, None, *([0] * len(batch))),
                      randomness='different')(self.func_model, self.func_weights,
                                              self.func_buffers, *batch)
         return vectorize_and_ignore_buffers(grads, self.params_dict)
 
     def compute_loss_grad(self, batch: Iterable[Tensor]) -> Tensor:
         """Computes the gradient of the loss with respect to the model output
+
         .. math::
-            \\partial \\ell / \\partial \\text{model output}
+
+            \\partial \\ell / \\partial \\text{(model output)}
 
         Note: For all applications we considered, we analytically derived the
         out-to-loss gradient, thus avoiding the need to do any backward passes
         (let alone per-sample grads). If for your application this is not feasible,
         you'll need to subclass this and modify this method to have a structure
-        similar to the one of `self.get_output`, i.e. something like:
-        ```
-        grad_out_to_loss = grad(self.model_out_to_loss_grad, ...)
-        grads = vmap(grad_out_to_loss, ...)
-        ...
-        ```
+        similar to the one of :meth:`FunctionalGradientComputer:.get_output`,
+        i.e. something like:
+
+        .. code-block:: python
+
+            grad_out_to_loss = grad(self.model_out_to_loss_grad, ...)
+            grads = vmap(grad_out_to_loss, ...)
+            ...
+
+        Args:
+            batch (Iterable[Tensor]):
+                batch of data
+
         """
         return self.modelout_fn.get_out_to_loss_grad(self.func_model,
                                                      self.func_weights,
                                                      self.func_buffers,
                                                      batch)
 
 
@@ -146,40 +167,59 @@
 
     def compute_per_sample_grad(self,
                                 batch: Iterable[Tensor],
                                 batch_size: int,
                                 ) -> Tensor:
         """ Computes per-sample gradients of the model output function This
         method does not leverage vectorization (and is hence much slower than
-        its equivalent in `FunctionalGradientComputer`). We recommend that
-        you use this only if `functorch` is not available to you, e.g. you have
-        a (very) old version of pytorch.
+        its equivalent in :class:`.FunctionalGradientComputer`). We recommend
+        that you use this only if :code:`functorch` is not available to you,
+        e.g. you have a (very) old version of pytorch.
+
+        Args:
+            batch (Iterable[Tensor]):
+                batch of data
+            batch_size (int, optional):
+                Defaults to None.
+
+        Returns:
+            Tensor:
+                gradients of the model output function of each sample in the
+                batch with respect to the model's parameters.
+
         """
         grads = ch.zeros(batch_size, self.grad_dim).to(batch[0].device)
 
         margin = self.modelout_fn.get_output(self.model, *batch)
         for ind in range(batch_size):
             grads[ind] = parameters_to_vector(ch.autograd.grad(margin[ind],
                                                                self.model_params,
                                                                retain_graph=True))
         return grads
 
     def compute_loss_grad(self, batch: Iterable[Tensor]) -> Tensor:
         """Computes the gradient of the loss with respect to the model output
+
         .. math::
-            \\partial \\ell / \\partial \\text{model output}
+
+            \\partial \\ell / \\partial \\text{(model output)}
 
         Note: For all applications we considered, we analytically derived the
         out-to-loss gradient, thus avoiding the need to do any backward passes
         (let alone per-sample grads). If for your application this is not feasible,
         you'll need to subclass this and modify this method to have a structure
-        similar to the one of `self.get_output`, i.e. something like:
+        similar to the one of :meth:`.IterativeGradientComputer.get_output`,
+        i.e. something like:
 
-        ```
-        out_to_loss = self.model_out_to_loss(...)
-        for ind in range(batch_size):
-            grads[ind] = torch.autograd.grad(out_to_loss[ind], ...)
-        ...
-        ```
+        .. code-block:: python
+
+            out_to_loss = self.model_out_to_loss(...)
+            for ind in range(batch_size):
+                grads[ind] = torch.autograd.grad(out_to_loss[ind], ...)
+            ...
+
+        Args:
+            batch (Iterable[Tensor]):
+                batch of data
 
         """
         return self.modelout_fn.get_out_to_loss_grad(self.model, batch)
```

### Comparing `traker-0.1.1/trak/modelout_functions.py` & `traker-0.1.2/trak/modelout_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,87 +1,98 @@
 """
 Here we provide an abstract "model output" class AbstractModelOutput, together with a number
 of subclasses for particular applications (vision, language, etc):
-- :code:`ImageClassificationModelOutput`
-- :code:`IterImageClassificationModelOutput`
-- :code:`CLIPModelOutput`
+
+- :class:`.ImageClassificationModelOutput`
+- :class:`.IterImageClassificationModelOutput`
+- :class:`.CLIPModelOutput`
+- :class:`.TextClassificationModelOutput`
 
 These classes implement methods that transform input batches to the desired model output
 (e.g. logits, loss, etc).
-See Sections 2 & 3 of (TODO: link)[our paper] for more details on what model output functions are
-in the context of TRAK and how to use & design them.
-
-See [TODO: docs link] for examples on how to subclass AbstractModelOutput for a task of your choice.
+See Sections 2 & 3 of `our paper <https://arxiv.org/abs/2303.14186>`_ for more
+details on what model output functions are in the context of TRAK and how to use
+& design them.
+
+See, e.g. `this tutorial <https://trak.readthedocs.io/en/latest/clip.html>`_ for an
+example on how to subclass :code:`AbstractModelOutput` for a task of your
+choice.
 """
 from abc import ABC, abstractmethod
 from typing import Iterable
 from torch import Tensor
 from torch.nn import Module
 import torch as ch
 
 
 class AbstractModelOutput(ABC):
-    """ See [TODO: docs link] for examples on how to subclass
-    :code:`AbstractModelOutput` for a task of your choice.
+    """ See, e.g. `this tutorial <https://trak.readthedocs.io/en/latest/clip.html>`_
+    for an example on how to subclass :code:`AbstractModelOutput` for a task of
+    your choice.
 
     Subclasses must implement:
+
     - a :code:`get_output` method that takes in a batch of inputs and model
-    weights to produce outputs that TRAK will be trained to predict. In the
-    notation of the paper, :code:`get_output` should return :math:`f(z,\\theta)`
+      weights to produce outputs that TRAK will be trained to predict. In the
+      notation of the paper, :code:`get_output` should return :math:`f(z,\\theta)`
 
     - a :code:`get_out_to_loss_grad` method that takes in a batch of inputs and
-    model weights to produce the gradient of the function that transforms the
-    model outputs above into the loss with respect to the batch. In the notation
-    of the paper, :code:`get_out_to_loss_grad` returns (entries along the
-    diagonal of) :math:`Q`.
+      model weights to produce the gradient of the function that transforms the
+      model outputs above into the loss with respect to the batch. In the
+      notation of the paper, :code:`get_out_to_loss_grad` returns (entries along
+      the diagonal of) :math:`Q`.
 
     """
     @abstractmethod
     def __init__(self) -> None:
         pass
 
     @abstractmethod
     def get_output(self,
                    model,
                    batch: Iterable[Tensor]) -> Tensor:
-        """ See Sections 2 & 3 of (TODO: link)[our paper] for more details on
-        what model output functions are in the context of TRAK and how to use &
-        design them.
+        """ See Sections 2 & 3 of `our paper
+        <https://arxiv.org/abs/2303.14186>`_ for more details on what model
+        output functions are in the context of TRAK and how to use & design
+        them.
 
         Args:
-            model (torch.nn.Module): model
-            batch (Iterable[Tensor]): input batch
+            model (torch.nn.Module):
+                model
+            batch (Iterable[Tensor]):
+                input batch
 
         Returns:
-            Tensor: model output function
+            Tensor:
+                model output function
         """
         ...
 
     @abstractmethod
     def get_out_to_loss_grad(self,
                              model,
                              batch: Iterable[Tensor]) -> Tensor:
-        """ See Sections 2 & 3 of (TODO: link)[our paper] for more details on
-        what the out-to-loss functions (in the notation of the paper, :math:`Q`)
-        are in the context of TRAK and how to use & design them.
+        """ See Sections 2 & 3 of `our paper
+        <https://arxiv.org/abs/2303.14186>`_ for more details on what the
+        out-to-loss functions (in the notation of the paper, :math:`Q`) are in
+        the context of TRAK and how to use & design them.
 
         Args:
             model (torch.nn.Module): model
             batch (Iterable[Tensor]): input batch
 
         Returns:
             Tensor: gradient of the out-to-loss function
         """
         ...
 
 
 class ImageClassificationModelOutput(AbstractModelOutput):
-    """
-    Margin for (multiclass) image classification. See Section 3.3 of (TODO: link)[our paper]
-    for more details.
+    """ Margin for (multiclass) image classification. See Section 3.3 of `our
+    paper <https://arxiv.org/abs/2303.14186>`_ for more details.
     """
 
     def __init__(self, temperature: float = 1.) -> None:
         """
         Args:
             temperature (float, optional): Temperature to use inside the
             softmax for the out-to-loss function. Defaults to 1.
@@ -95,38 +106,46 @@
                    weights: Iterable[Tensor],
                    buffers: Iterable[Tensor],
                    image: Tensor,
                    label: Tensor) -> Tensor:
         """ For a given input :math:`z=(x, y)` and model parameters :math:`\\theta`,
         let :math:`p(z, \\theta)` be the softmax probability of the correct class.
         This method implements the model output function
+
         .. math::
+
             \\log(\\frac{p(z, \\theta)}{1 - p(z, \\theta)}).
 
         It uses functorch's functional models to make the per-sample gradient computations faster.
         For more details on what func_model, weights & buffers are, and how to use them, please
         refer to https://pytorch.org/functorch/stable/ and
         https://pytorch.org/functorch/stable/notebooks/per_sample_grads.html.
 
         Note: this method slightly breaks abstraction since it has a different
         signature from the abstract :code:`get_output`. It's only used
         internally by :func:`GradientComputer` so it shouldn't be a big problem.
         If you're reading this and feel strongly about it, feel free to make a
         PR with a fix.
 
         Args:
-            func_model (func): functorch functional model
-            weights (Iterable[Tensor]): functorch model weights
-            buffers (Iterable[Tensor]): functorch model buffers
-            image (Tensor): input image, should not have batch dimension
-            label (Tensor): input label, should not have batch dimension
+            func_model (func):
+                functorch functional model
+            weights (Iterable[Tensor]):
+                functorch model weights
+            buffers (Iterable[Tensor]):
+                functorch model buffers
+            image (Tensor):
+                input image, should not have batch dimension
+            label (Tensor):
+                input label, should not have batch dimension
 
         Returns:
-            Tensor: model output for the given image-label pair :math:`z` and
-            weights & buffers :math:`\\theta`.
+            Tensor:
+                model output for the given image-label pair :math:`z` and
+                weights & buffers :math:`\\theta`.
         """
         logits = func_model(weights, buffers, image.unsqueeze(0))
         bindex = ch.arange(logits.shape[0]).to(logits.device, non_blocking=False)
         logits_correct = logits[bindex, label.unsqueeze(0)]
 
         cloned_logits = logits.clone()
         # a hacky way to remove the logits of the correct labels from the sum
@@ -140,77 +159,92 @@
         """ Utility method to make forward passes compatible across different models,
         e.g. image classification models take in only the images in the batch,
         but CLIP takes in both the images and captions --- using this method,
         the TRAKer class does not need to be modified when we have a new model
         that uses different parts of the input batch.
 
         Args:
-            model (Module): model
-            batch (Iterable[Tensor]): input batch
+            model (Module):
+                model
+            batch (Iterable[Tensor]):
+                input batch
 
         Returns:
-            Tensor: model output (not to be confused with the model output function)
+            Tensor:
+                model output (not to be confused with the model output function)
         """
         images, _ = batch
         return model(images)
 
     def get_out_to_loss_grad(self, func_model, weights, buffers, batch: Iterable[Tensor]) -> Tensor:
         """ Computes the (reweighting term Q in the paper)
 
         Args:
-            func_model (func): functorch functional model
-            weights (Iterable[Tensor]): functorch model weights
-            buffers (Iterable[Tensor]): functorch model buffers
-            batch (Iterable[Tensor]): input batch
+            func_model (func):
+                functorch functional model
+            weights (Iterable[Tensor]):
+                functorch model weights
+            buffers (Iterable[Tensor]):
+                functorch model buffers
+            batch (Iterable[Tensor]):
+                input batch
 
         Returns:
-            Tensor: out-to-loss (reweighting term) for the input batch
+            Tensor:
+                out-to-loss (reweighting term) for the input batch
         """
         images, labels = batch
         logits = func_model(weights, buffers, images)
         # here we are directly implementing the gradient instead of relying on autodiff to do
         # that for us
         ps = self.softmax(logits / self.loss_temperature)[ch.arange(logits.size(0)), labels]
         return (1 - ps).clone().detach().unsqueeze(-1)
 
 
 class IterImageClassificationModelOutput(AbstractModelOutput):
     """
-    Margin for (multiclass) image classification. See Section 3.3 of (TODO: link)[our paper]
-    for more details.
+    Margin for (multiclass) image classification. See Section 3.3 of `our paper
+    <https://arxiv.org/abs/2303.14186>`_ for more details.
     """
 
     def __init__(self, temperature=1.) -> None:
         """
         Args:
-            temperature (float, optional): Temperature to use inside the
-            softmax for the out-to-loss function. Defaults to 1.
+            temperature (float, optional):
+                Temperature to use inside the softmax for the out-to-loss
+                function. Defaults to 1.
         """
         super().__init__()
         self.softmax = ch.nn.Softmax(-1)
         self.loss_temperature = temperature
 
     def get_output(self,
                    model: Module,
                    images: Tensor,
                    labels: Tensor) -> Tensor:
         """ For a given input :math:`z=(x, y)` and model parameters :math:`\\theta`,
         let :math:`p(z, \\theta)` be the softmax probability of the correct class.
         This method implements the model output function
+
         .. math::
+
             \\log(\\frac{p(z, \\theta)}{1 - p(z, \\theta)}).
 
         Args:
-            model (torch.nn.Module): model
-            image (Tensor): input images
-            label (Tensor): input labels
+            model (torch.nn.Module):
+                model
+            images (Tensor):
+                input images
+            labels (Tensor):
+                input labels
 
         Returns:
-            Tensor: model output for the given image-label pair :math:`z` and
-            model parameters :math:`\theta`.
+            Tensor:
+                model output for the given image-label pair :math:`z` and model
+                parameters :math:`\\theta`.
         """
         logits = model(images)
         bindex = ch.arange(logits.shape[0]).to(logits.device, non_blocking=False)
         logits_correct = logits[bindex, labels]
 
         cloned_logits = logits.clone()
         # a hacky way to remove the logits of the correct labels from the sum
@@ -220,51 +254,58 @@
         margins = logits_correct - cloned_logits.logsumexp(dim=-1)
         return margins
 
     def get_out_to_loss_grad(self, model: Module, batch: Iterable[Tensor]) -> Tensor:
         """ Computes the (reweighting term Q in the paper)
 
         Args:
-            model (torch.nn.Module): model
-            batch (Iterable[Tensor]): input batch
+            model (torch.nn.Module)
+                model
+            batch (Iterable[Tensor]):
+                input batch
 
         Returns:
-            Tensor: out-to-loss (reweighting term) for the input batch
+            Tensor:
+                out-to-loss (reweighting term) for the input batch
         """
         images, labels = batch
         logits = model(images)
         # here we are directly implementing the gradient instead of relying on autodiff to do
         # that for us
         ps = self.softmax(logits / self.loss_temperature)[ch.arange(logits.size(0)), labels]
         return (1 - ps).clone().detach().unsqueeze(-1)
 
 
 class CLIPModelOutput(AbstractModelOutput):
     """ Margin for multimodal contrastive learning (CLIP). See Section 5.1 of
-    (TODO: link)[our paper] for more details.
+    `our paper <https://arxiv.org/abs/2303.14186>`_ for more details.
 
     Raises:
         AssertionError: this model output function requires using additional
         CLIP embeddings, which are computed using the :func:`get_embeddings`
         method. This method should be invoked before featurizing.
     """
     num_computed_embeddings = 0
     sim_batch_size = 0
     image_embeddings = None
     text_embeddings = None
 
     def __init__(self, temperature: float = None, simulated_batch_size: int = 300) -> None:
         """
+
         Args:
-            temperature (float, optional): Temperature to use inside the
-                softmax for the out-to-loss function. If None, CLIP's
-                :code:`logit_scale` is used.  Defaults to None
-            simulated_batch_size (int, optional): Size of the "simulated" batch
-                size for the model output function. See Section 5.1 of the TRAK
-                paper for more details. Defaults to 300.
+            temperature (float, optional):
+                Temperature to use inside the softmax for the out-to-loss
+                function. If None, CLIP's :code:`logit_scale` is used.  Defaults
+                to None
+            simulated_batch_size (int, optional):
+                Size of the "simulated" batch size for the model output
+                function. See Section 5.1 of the TRAK paper for more details.
+                Defaults to 300.
+
         """
         super().__init__()
         self.softmax = ch.nn.Softmax(-1)
         self.temperature = temperature
 
         self.sim_batch_size = simulated_batch_size
         CLIPModelOutput.sim_batch_size = simulated_batch_size
@@ -277,23 +318,31 @@
                        embedding_dim: int = 1024,
                        preprocess_fn_img=None,
                        preprocess_fn_txt=None) -> None:
         """ Computes (image and text) embeddings and saves them in the class
         attributes :code:`image_embeddings` and :code:`text_embeddings`.
 
         Args:
-            model (torch.nn.Module): model
-            loader (): data loader
-            batch_size (int): input batch size
-            size (int, optional): Maximum number of embeddings to compute. Defaults to 50_000.
-            embedding_dim (int, optional): Dimension of CLIP embedding. Defaults to 1024.
-            preprocess_fn_img (func, optional): Transforms to apply to images
-            from the loader before forward pass. Defaults to None.
-            preprocess_fn_txt (func, optional): Transforms to apply to images
-            from the loader before forward pass. Defaults to None.
+            model (torch.nn.Module):
+                model
+            loader ():
+                data loader
+            batch_size (int):
+                input batch size
+            size (int, optional):
+                Maximum number of embeddings to compute. Defaults to 50_000.
+            embedding_dim (int, optional):
+                Dimension of CLIP embedding. Defaults to 1024.
+            preprocess_fn_img (func, optional):
+                Transforms to apply to images from the loader before forward
+                pass. Defaults to None.
+            preprocess_fn_txt (func, optional):
+                Transforms to apply to images from the loader before forward
+                pass. Defaults to None.
+
         """
         img_embs, txt_embs = ch.zeros(size, embedding_dim).cuda(),\
             ch.zeros(size, embedding_dim).cuda()
 
         cutoff = batch_size
         with ch.no_grad():
             for ind, (images, text) in enumerate(loader):
@@ -316,20 +365,22 @@
 
     @staticmethod
     def get_output(func_model,
                    weights: Iterable[Tensor],
                    buffers: Iterable[Tensor],
                    image: Tensor,
                    label: Tensor) -> Tensor:
-        """ For a given input :math:`z=(x, y)` and model parameters :math:`\\theta`,
-        let :math:`\\phi(x, \\theta)` be the CLIP image embedding and
-        :math:`\\psi(y, \\theta)` be the CLIP text embedding. Last, let
-        :math:`B` be a (simulated) batch. This method implements the model
-        output function
+        """ For a given input :math:`z=(x, y)` and model parameters
+        :math:`\\theta`, let :math:`\\phi(x, \\theta)` be the CLIP image
+        embedding and :math:`\\psi(y, \\theta)` be the CLIP text embedding.
+        Last, let :math:`B` be a (simulated) batch. This method implements the
+        model output function
+
         .. math::
+
             -\\log(\\frac{\\phi(x)\\cdot \\psi(y)}{\\sum_{(x', y')\\in B}
             \\phi(x)\\cdot \\psi(y')})
             -\\log(\\frac{\\phi(x)\\cdot \\psi(y)}{\\sum_{(x', y')\\in B}
             \\phi(x')\\cdot \\psi(y)})
 
         It uses functorch's functional models to make the per-sample gradient
         computations faster.  For more details on what func_model, weights &
@@ -340,23 +391,29 @@
         Note: this method slightly breaks abstraction since it has a different
         signature from the abstract :code:`get_output`. It's only used
         internally by :func:`GradientComputer` so it shouldn't be a big problem.
         If you're reading this and feel strongly about it, feel free to make a
         PR with a fix.
 
         Args:
-            func_model (func): functorch functional model
-            weights (Iterable[Tensor]): functorch model weights
-            buffers (Iterable[Tensor]): functorch model buffers
-            image (Tensor): input image, should not have batch dimension
-            label (Tensor): input label, should not have batch dimension
+            func_model (func):
+                functorch functional model
+            weights (Iterable[Tensor]):
+                functorch model weights
+            buffers (Iterable[Tensor]):
+                functorch model buffers
+            image (Tensor):
+                input image, should not have batch dimension
+            label (Tensor):
+                input label, should not have batch dimension
 
         Returns:
-            Tensor: model output for the given image-label pair :math:`z` and
-            weights & buffers :math:`\\theta`.
+            Tensor:
+                model output for the given image-label pair :math:`z` and
+                weights & buffers :math:`\\theta`.
         """
         all_im_embs = CLIPModelOutput.image_embeddings
         all_txt_embs = CLIPModelOutput.text_embeddings
         N = CLIPModelOutput.num_computed_embeddings
         sim_bs = CLIPModelOutput.sim_batch_size
 
         if all_im_embs is None:
@@ -375,39 +432,45 @@
                  -ch.logsumexp(-text_embeddings @ (image_embeddings - all_im_embs[ii]).T, dim=1)
         return result.sum()  # shape of result should be [1]
 
     def get_out_to_loss_grad(self, func_model, weights, buffers, batch: Iterable[Tensor]) -> Tensor:
         """ Computes the (reweighting term Q in the paper)
 
         Args:
-            func_model (func): functorch functional model
-            weights (Iterable[Tensor]): functorch model weights
-            buffers (Iterable[Tensor]): functorch model buffers
-            batch (Iterable[Tensor]): input batch
+            func_model (func):
+                functorch functional model
+            weights (Iterable[Tensor]):
+                functorch model weights
+            buffers (Iterable[Tensor]):
+                functorch model buffers
+            batch (Iterable[Tensor]):
+                input batch
 
         Returns:
-            Tensor: out-to-loss (reweighting term) for the input batch
+            Tensor:
+                out-to-loss (reweighting term) for the input batch
+
         """
         image_embeddings, text_embeddings, temp = func_model(weights, buffers, *batch)
         if self.temperature is None:
             self.temperature = temp
         res = self.temperature * image_embeddings @ text_embeddings.T
         ps = (self.softmax(res) + self.softmax(res.T)).diag() / 2.
         return (1 - ps).clone().detach()
 
 
 class TextClassificationModelOutput(AbstractModelOutput):
-    """
-    Margin for text classification models. This assumes that the model takes in
-    input_ids, token_type_ids, and attention_mask.
+    """ Margin for text classification models. This assumes that the model takes
+    in input_ids, token_type_ids, and attention_mask.
+
     .. math::
-        \text{logit}[\text{correct}] - \log\left(\sum_{i \neq \text{correct}}
-        \exp(\text{logit}[i])\right)
-    Version of margin proposed in 'Understanding Influence Functions
-    and Datamodels via Harmonic Analysis'
+
+        \\text{logit}[\\text{correct}] - \\log\\left(\\sum_{i \\neq
+        \\text{correct}} \\exp(\\text{logit}[i])\\right)
+
     """
 
     def __init__(self, temperature=1.) -> None:
         super().__init__()
         self.softmax = ch.nn.Softmax(-1)
         self.loss_temperature = temperature
 
@@ -417,30 +480,30 @@
                    buffers: Iterable[Tensor],
                    input_id: Tensor,
                    token_type_id: Tensor,
                    attention_mask: Tensor,
                    label: Tensor,
                    ) -> Tensor:
         logits = func_model(weights, buffers, input_id.unsqueeze(0),
-                                token_type_id.unsqueeze(0),
-                                attention_mask.unsqueeze(0))
+                            token_type_id.unsqueeze(0),
+                            attention_mask.unsqueeze(0))
         bindex = ch.arange(logits.shape[0]).to(logits.device, non_blocking=False)
         logits_correct = logits[bindex, label.unsqueeze(0)]
 
         cloned_logits = logits.clone()
         cloned_logits[bindex, label.unsqueeze(0)] = ch.tensor(-ch.inf).to(logits.device)
 
         margins = logits_correct - cloned_logits.logsumexp(dim=-1)
         return margins.sum()
 
     def forward(self, model: Module, batch: Iterable[Tensor]) -> Tensor:
         input_ids, token_type_ids, attention_mask, _ = batch
         return model(input_ids=input_ids,
-            token_type_ids=token_type_ids,
-            attention_mask=attention_mask)
+                     token_type_ids=token_type_ids,
+                     attention_mask=attention_mask)
 
     def get_out_to_loss_grad(self, func_model, weights, buffers, batch: Iterable[Tensor]) -> Tensor:
         input_ids, token_type_ids, attention_mask, labels = batch
         logits = func_model(weights, buffers, input_ids, token_type_ids, attention_mask)
         ps = self.softmax(logits / self.loss_temperature)[ch.arange(logits.size(0)), labels]
         return (1 - ps).clone().detach().unsqueeze(-1)
```

### Comparing `traker-0.1.1/trak/projectors.py` & `traker-0.1.2/trak/projectors.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,40 +9,45 @@
 
 class ProjectionType(str, Enum):
     normal: str = 'normal'
     rademacher: str = 'rademacher'
 
 
 class AbstractProjector(ABC):
-    """
-    Implementations of the Projector class must implement the `project` method,
-    which takes in model gradients and returns
+    """ Implementations of the Projector class must implement the
+    :meth:`AbstractProjector.project` method, which takes in model gradients and
+    returns
     """
     @abstractmethod
     def __init__(self,
                  grad_dim: int,
                  proj_dim: int,
                  seed: int,
                  proj_type: Union[str, ProjectionType],
                  device: Union[str, torch.device]) -> None:
         """ Initializes hyperparameters for the projection.
 
         Args:
-            grad_dim (int): number of parameters in the model (dimension of the
-                gradient vectors)
-            proj_dim (int): dimension after the projection
-            seed (int): random seed for the generation of the sketching
-                (projection) matrix
-            proj_type (Union[str, ProjectionType]): the random projection
-                (JL transform) guearantees that distances will be approximately
-                preserved for a variety of choices of the random matrix (see
-                e.g. https://arxiv.org/abs/1411.2404). Here, we provide an
-                implementation for matrices with iid Gaussian entries and iid
-                Rademacher entries.
-            device (Union[str, torch.device]): CUDA device to use
+            grad_dim (int):
+                number of parameters in the model (dimension of the gradient
+                vectors)
+            proj_dim (int):
+                dimension after the projection
+            seed (int):
+                random seed for the generation of the sketching (projection)
+                matrix
+            proj_type (Union[str, ProjectionType]):
+                the random projection (JL transform) guearantees that distances
+                will be approximately preserved for a variety of choices of the
+                random matrix (see e.g. https://arxiv.org/abs/1411.2404). Here,
+                we provide an implementation for matrices with iid Gaussian
+                entries and iid Rademacher entries.
+            device (Union[str, torch.device]):
+                CUDA device to use
+
         """
         self.grad_dim = grad_dim
         self.proj_dim = proj_dim
         self.seed = seed
         self.proj_type = proj_type
         self.device = device
 
@@ -101,15 +106,15 @@
             self.proj_matrix -= 1.
         else:
             raise KeyError(f'Projection type {self.proj_type} not recognized.')
 
     def project(self, grads: Tensor, model_id: int) -> Tensor:
         if model_id != self.model_id:
             self.model_id = model_id
-            self.generator = self.generator.manual_seed(self.seed + 10e4 * self.model_id)
+            self.generator = self.generator.manual_seed(self.seed + int(1e4) * self.model_id)
             self.generate_sketch_matrix()  # updates self.proj_matrix
 
         return grads @ self.proj_matrix
 
 
 class BasicProjector(AbstractProjector):
     """
@@ -189,16 +194,43 @@
 
 class CudaProjector(AbstractProjector):
     """
     A performant implementation of the projection for CUDA with compute
     capability >= 7.0.
     """
     def __init__(self, grad_dim: int, proj_dim: int, seed: int, proj_type:
-                 ProjectionType, device, *args, **kwargs) -> None:
+                 ProjectionType, device, max_batch_size: int = 32, *args, **kwargs) -> None:
+        """
+
+        Args:
+            grad_dim (int):
+                Number of parameters
+            proj_dim (int):
+                Dimension we project *to* during the projection step
+            seed (int):
+                Random seed
+            proj_type (ProjectionType):
+                Type of randomness to use for projection matrix (rademacher or normal)
+            device:
+                CUDA device
+            max_batch_size (int):
+                Explicitly constraints the batch size the CudaProjector is going
+                to use for projection. Set this if you get a 'The batch size of
+                the CudaProjector is too large for your GPU' error. Must be
+                either 8, 16, or 32.
+
+        Raises:
+            ValueError:
+                When attempting to use this on a non-CUDA device
+            ModuleNotFoundError:
+                When fast_jl is not installed
+
+        """
         super().__init__(grad_dim, proj_dim, seed, proj_type, device)
+        self.max_batch_size = max_batch_size
 
         if isinstance(device, str):
             device = ch.device(device)
 
         if device.type != 'cuda':
             err = "CudaProjector only works on a CUDA device; Either switch to a CUDA device, or use the BasicProjector"
             raise ValueError(err)
@@ -212,17 +244,30 @@
         except ImportError:
             err = "You should make sure to install the CUDA projector for traker (called fast_jl).\
                   See the installation FAQs for more details."
             raise ModuleNotFoundError(err)
 
     def project(self, grads: Tensor, model_id: int) -> Tensor:
         batch_size = grads.shape[0]
+
         effective_batch_size = 32
         if batch_size <= 8:
             effective_batch_size = 8
         elif batch_size <= 16:
             effective_batch_size = 16
 
+        effective_batch_size = min(self.max_batch_size, effective_batch_size)
+
         function_name = f"project_{self.proj_type.value}_{effective_batch_size}"
         import fast_jl
         fn = getattr(fast_jl, function_name)
-        return fn(grads, self.proj_dim, self.seed + int(1e4) * model_id, self.num_sms)
+
+        try:
+            result = fn(grads, self.proj_dim, self.seed + int(1e4) * model_id, self.num_sms)
+        except RuntimeError as e:
+            if str(e) == 'CUDA error: too many resources requested for launch\nCUDA kernel errors might be asynchronously reported at some other API call, so the stacktrace below might be incorrect.\nFor debugging consider passing CUDA_LAUNCH_BLOCKING=1.\nCompile with `TORCH_USE_CUDA_DSA` to enable device-side assertions.\n':
+                # provide a more helpful error message
+                raise RuntimeError(f'The batch size of the CudaProjector is too large for your GPU. Reduce it by using the max_batch_size argument of the CudaProjector.\nOriginal error: {str(e)}')
+            else:
+                raise e
+
+        return result
```

### Comparing `traker-0.1.1/trak/savers.py` & `traker-0.1.2/trak/savers.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 
 class AbstractSaver(ABC):
     """
     Implementations of Saver class must implement getters and setters for TRAK
     features and scores, as well as intermediate values like gradients and
     "out-to-loss-gradient".
-
+    
     The Saver class also handles the recording of metadata associated with each
     TRAK run. For example, hyperparameters like "JL dimension" -- the dimension
-    used for the dimensionality reduction step of TRAk (Johnson-Lindenstrauss
+    used for the dimensionality reduction step of TRAK (Johnson-Lindenstrauss
     projection).
     """
     @abstractmethod
     def __init__(self,
                  save_dir: Union[Path, str],
                  metadata: Iterable,
                  load_from_save_dir: bool) -> None:
@@ -95,69 +95,83 @@
         self.current_target_grads = None
 
     @abstractmethod
     def register_model_id(self, model_id: int) -> None:
         """ Create metadata for a new model ID (checkpoint).
 
         Args:
-            model_id (int): a unique ID for a checkpoint
+            model_id (int):
+                a unique ID for a checkpoint
+
         """
         ...
 
     @abstractmethod
     def serialize_model_id_metadata(self, model_id: int) -> None:
         """ Write to disk / commit any updates to the metadata associated
         to a given model ID
 
         Args:
-            model_id (int): a unique ID for a checkpoint
+            model_id (int):
+                a unique ID for a checkpoint
+
         """
         ...
 
     @abstractmethod
     def load_store(self, model_id: int) -> None:
         """ Populates the self.current_* attributes with data for the
         given model ID (checkpoint).
 
         Args:
-            model_id (int): a unique ID for a checkpoint
+            model_id (int):
+                a unique ID for a checkpoint
+
         """
         ...
 
     @abstractmethod
     def load_target_store(self,
                           model_id: int,
                           num_targets: int,
                           mode: Optional[str]) -> None:
         """ Loads/initializes metadata and store arrays for target results and
         features (gradients)
 
         Args:
-            model_id (int): a unique ID for a checkpoint
-            num_targets (int): number of target samples that will be scored
+            model_id (int):
+                a unique ID for a checkpoint
+            num_targets (int):
+                number of target samples that will be scored
+
         """
         ...
 
     @abstractmethod
     def del_grads(self, model_id: int, target: bool) -> None:
         """ Delete the intermediate values (gradients) for a given model id
 
         Args:
-            model_id (int): a unique ID for a checkpoint
-            target (bool): if True, delete the gradients of the target samples,
-                otherwise delete the train set gradients.
+            model_id (int):
+                a unique ID for a checkpoint
+            target (bool):
+                if True, delete the gradients of the target samples, otherwise
+                delete the train set gradients.
+
         """
         ...
 
     @abstractmethod
     def clear_target_grad_count(self, model_id: int) -> None:
         """ Reset the count for how many targets we are scoring
 
         Args:
-            model_id (int): a unique ID for a checkpoint
+            model_id (int):
+                a unique ID for a checkpoint
+
         """
         ...
 
 
 class ModelIDException(Exception):
     """ A minimal custom exception for errors related to model IDs """
     pass
@@ -181,19 +195,21 @@
                           _allow_featurizing_already_registered: bool) -> None:
         """ This method
         1) checks if the model ID already exists in the save dir
         2) if yes, it raises an error since model IDs must be unique
         3) if not, it creates a metadata file for it and initalizes store mmaps
 
         Args:
-            model_id (int): a unique ID for a checkpoint
+            model_id (int):
+                a unique ID for a checkpoint
 
         Raises:
-            ModelIDException: raised if the model ID to be registered already
-            exists
+            ModelIDException:
+                raised if the model ID to be registered already exists
+
         """
         self.current_model_id = model_id
 
         if self.current_model_id in self.model_ids.keys() and (not _allow_featurizing_already_registered):
             err_msg = f'model id {self.current_model_id} is already registered. Check {self.save_dir}'
             raise ModelIDException(err_msg)
         self.model_ids[self.current_model_id] = {'featurized': 0,
@@ -220,16 +236,19 @@
     def load_store(self,
                    model_id: int,
                    mode: Optional[str] = 'r+') -> None:
         """ This method uses numpy memmaps for serializing the TRAK results and
         intermediate values.
 
         Args:
-            model_id (int): a unique ID for a checkpoint
-            mode (str, optional): Defaults to 'r+'.
+            model_id (int):
+                a unique ID for a checkpoint
+            mode (str, optional):
+                Defaults to 'r+'.
+
         """
         self.current_model_id = model_id
         prefix = self.save_dir.joinpath(str(model_id))
 
         self.current_grads_path = prefix.joinpath('grads.mmap')
         self.current_grads = open_memmap(filename=self.current_grads_path,
                                          mode=mode,
@@ -249,19 +268,23 @@
                                             dtype=np.float32)
 
     def load_target_store(self,
                           model_id: int,
                           num_targets: int,
                           mode: Optional[str] = 'r+',
                           ) -> None:
-        """_summary_
+        """ This method uses numpy memmaps for serializing the TRAK intermediate
+        values for targets.
 
         Args:
-            model_id (int): _description_
-            num_targets (int): _description_
+            model_id (int):
+                a unique ID for a checkpoint
+            num_targets (int):
+                number of target samples that will be scored
+
         """
         self.num_targets = num_targets
         self.current_model_id = model_id
         self.model_ids[model_id]['targets_scored'] = self.num_targets
         self.serialize_model_id_metadata(model_id)
 
         prefix = self.save_dir.joinpath(str(model_id))
```

### Comparing `traker-0.1.1/trak/score_computers.py` & `traker-0.1.2/trak/score_computers.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.1/trak/traker.py` & `traker-0.1.2/trak/traker.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,74 +13,86 @@
 
 import numpy as np
 import torch
 ch = torch
 
 
 class TRAKer():
+    """ The main front-facing class for TRAK. See the `README
+    <https://github.com/MadryLab/trak>`_ and `docs
+    <https://trak.readthedocs.io/en/latest/>`_ for example usage.
+
+    """
     def __init__(self,
                  model: torch.nn.Module,
                  task: Union[AbstractModelOutput, str],
                  train_set_size: int,
                  save_dir: str = './trak_results',
                  load_from_save_dir: bool = True,
                  device: Union[str, torch.device] = 'cuda',
                  gradient_computer: AbstractGradientComputer = FunctionalGradientComputer,
                  projector: Optional[AbstractProjector] = None,
                  proj_dim: int = 2048,
                  ) -> None:
-        """ The main front-facing class for TRAK. See the README and docs for
-        example usage.
+        """
 
         Args:
-            model (torch.nn.Module): model to use for TRAK
-            task (Union[AbstractModelOutput, str]): Type of model that TRAK will
-                be ran on. Accepts either one of the following strings:
+            model (torch.nn.Module):
+                model to use for TRAK
+            task (Union[AbstractModelOutput, str]):
+                Type of model that TRAK will be ran on. Accepts either one of
+                the following strings:
                 - :code:`image_classification`
+                - :code:`text_classification`
                 - :code:`clip`
-                - :code:`bert_...` TODO: @Sam
-                or an implementation of :func:`AbstractModelOutput`.
-            train_set_size (int): Size of the train set that TRAK is featurizing
-            save_dir (str, optional): Directory to save final TRAK scores,
-                intermediate results, and metadata. Defaults to './trak_results'.
-            load_from_save_dir (bool, optional): If True, the TRAKer instance
-                will attempt to load existing metadata from save_dir. May lead
-                to I/O issues if multiple TRAKer instances ran in parallel have
-                this flag set to True. See the SLURM tutorial for more details.
-            device (Union[str, torch.device], optional): torch device on which
-                to do computations. Defaults to 'cuda'.
+                or an implementation of :class:`.AbstractModelOutput`.
+            train_set_size (int):
+                Size of the train set that TRAK is featurizing
+            save_dir (str, optional):
+                Directory to save final TRAK scores, intermediate results, and
+                metadata. Defaults to :code:'./trak_results'.
+            load_from_save_dir (bool, optional):
+                If True, the :class`.TRAKer` instance will attempt to load
+                existing metadata from save_dir. May lead to I/O issues if
+                multiple TRAKer instances ran in parallel have this flag set to
+                True. See the SLURM tutorial for more details.
+            device (Union[str, torch.device], optional):
+                torch device on which to do computations. Defaults to 'cuda'.
             gradient_computer (AbstractGradientComputer, optional):
                 Class to use to get per-example gradients. See
-                :func:`AbstractGradientComputer` for more details. Defaults to
-                FunctionalGradientComputer.
-            projector (Optional[AbstractProjector], optional): Either set
-                :code:`proj_dim` and a :func:`CudaProjector` Rademacher
-                projector will be used or give a custom :code:`Projector` class
-                and leave :code:`proj_dim` to None. Defaults to None.
-            proj_dim (int, optional): Dimension of the projected TRAK features.
-                See Section 4.3 of (TODO: link)[our paper] for more details.
-                Defaults to 2048.
+                :class:`.AbstractGradientComputer` for more details. Defaults to
+                :class:`.FunctionalGradientComputer`.
+            projector (Optional[AbstractProjector], optional):
+                Either set :code:`proj_dim` and a :class:`.CudaProjector`
+                Rademacher projector will be used or give a custom subclass of
+                :class:`.AbstractProjector` class and leave :code:`proj_dim` as
+                None. Defaults to None.
+            proj_dim (int, optional):
+                Dimension of the projected TRAK features. See Section 4.3 of
+                `our paper <https://arxiv.org/abs/2303.14186>`_ for more
+                details. Defaults to 2048.
+
         """
 
         self.model = model
         self.task = task
         self.train_set_size = train_set_size
         self.device = device
 
         self.num_params = get_num_params(self.model)
         self.init_projector(projector, proj_dim)  # inits self.projector
 
         self.save_dir = Path(save_dir).resolve()
         self.load_from_save_dir = load_from_save_dir
 
         if type(self.task) is str:
-            self.modelout_fn = TASK_TO_MODELOUT[(self.task, gradient_computer.is_functional)]
+            self.task = TASK_TO_MODELOUT[(self.task, gradient_computer.is_functional)]
 
         self.gradient_computer = gradient_computer(model=self.model,
-                                                   modelout_fn=self.modelout_fn,
+                                                   modelout_fn=self.task,
                                                    grad_dim=self.num_params)
 
         self.score_computer = BasicScoreComputer(device=self.device)
 
         metadata = {
             'JL dimension': self.projector.proj_dim,
             'JL matrix type': self.projector.proj_type,
@@ -91,15 +103,17 @@
                                proj_dim=self.proj_dim,
                                load_from_save_dir=self.load_from_save_dir)
 
     def init_projector(self, projector, proj_dim) -> None:
         """ Initialize the projector for a traker class
 
         Args:
-            projector (AbstractProjector): JL projector
+            projector (AbstractProjector):
+                JL projector
+
         """
 
         self.projector = projector
         if projector is not None:
             self.proj_dim = self.projector.proj_dim
         else:
             self.proj_dim = proj_dim
@@ -113,20 +127,23 @@
                         checkpoint: Iterable[Tensor],
                         model_id: int,
                         _allow_featurizing_already_registered=None) -> None:
         """ Loads state dictionary for the given checkpoint; initializes arrays
         to store TRAK features for that checkpoint, tied to the model ID.
 
         Args:
-            checkpoint (Iterable[Tensor]): state_dict to load
-            model_id (int): a unique ID for a checkpoint
-            _allow_featurizing_already_registered (bool, optional): Only use if
-                you want to override the default behaviour that
+            checkpoint (Iterable[Tensor]):
+                state_dict to load
+            model_id (int):
+                a unique ID for a checkpoint
+            _allow_featurizing_already_registered (bool, optional):
+                Only use if you want to override the default behaviour that
                 :code:`featurize` is forbidden on already registered model IDs.
                 Defaults to None.
+
         """
         if self.saver.model_ids.get(model_id) is None:
             self.saver.register_model_id(model_id,
                                          _allow_featurizing_already_registered)
         else:
             self.saver.load_store(model_id)
 
@@ -153,19 +170,21 @@
         3.4).
 
         Either :code:`inds` or :code:`num_samples` must be specified. Using
         :code:`num_samples` will write sequentially into the internal store of
         the :func:`TRAKer`.
 
         Args:
-            batch (Iterable[Tensor]): input batch
-            inds (Optional[Iterable[int]], optional): Indices of the batch
-            samples in the train set. Defaults to None.
-            num_samples (Optional[int], optional): Number of samples in the
-            batch. Defaults to None.
+            batch (Iterable[Tensor]):
+                input batch
+            inds (Optional[Iterable[int]], optional):
+                Indices of the batch samples in the train set. Defaults to None.
+            num_samples (Optional[int], optional):
+                Number of samples in the batch. Defaults to None.
+
         """
         assert (inds is None) or (num_samples is None),\
             "Exactly one of num_samples and inds should be specified"
         assert (inds is not None) or (num_samples is not None),\
             "Exactly one of num_samples and inds should be specified"
 
         if num_samples is not None:
@@ -197,16 +216,17 @@
         :math:`\\Phi_c (\\Phi_c^\\top\\Phi_c)^{-1}` for all :math:`c\\in C`
         and stores the results in the internal store of the :func:`TRAKer`
         class.
 
         Args:
             model_ids (Iterable[int], optional): A list of model IDs for which
                 features should be finalized. If None, features are finalized
-                for all model IDs in the :code:`save_dir` of the :func:`TRAKer`
+                for all model IDs in the :code:`save_dir` of the :class:`.TRAKer`
                 class. Defaults to None.
+
         """
         if model_ids is None:
             model_ids = list(self.saver.model_ids.keys())
 
         self._last_ind = 0
 
         for model_id in tqdm(model_ids, desc='Finalizing features for all model IDs..'):
@@ -229,48 +249,55 @@
             self.saver.serialize_model_id_metadata(self.saver.current_model_id)
 
     def start_scoring_checkpoint(self,
                                  checkpoint: Iterable[Tensor],
                                  model_id: int,
                                  num_targets: int,
                                  ) -> None:
-        """ This method prepares the internal store of the :func:`TRAKer` class
+        """ This method prepares the internal store of the :class:`.TRAKer` class
         to start computing scores for a set of targets.
 
         Args:
-            checkpoint (Iterable[Tensor]): model checkpoint (state dict)
-            model_id (int): a unique ID for a checkpoint
-            num_targets (int): number of targets to score
+            checkpoint (Iterable[Tensor]):
+                model checkpoint (state dict)
+            model_id (int):
+                a unique ID for a checkpoint
+            num_targets (int):
+                number of targets to score
+
         """
         self.saver.load_target_store(model_id, num_targets, mode='w+')
 
         self.model.load_state_dict(checkpoint)
         self.model.eval()
+        self.gradient_computer.load_model_params(self.model)
 
         self._last_ind_target = 0
 
     def score(self,
               batch: Iterable[Tensor],
               inds: Optional[Iterable[int]] = None,
               num_samples: Optional[int] = None,
               ) -> None:
         """ This method computes the (intermediate per-checkpoint) TRAK scores
         for a batch of targets and stores them in the internal store of the
-        :func:`TRAKer` class.
+        :class:`.TRAKer` class.
 
         Either :code:`inds` or :code:`num_samples` must be specified. Using
         :code:`num_samples` will write sequentially into the internal store of
-        the :func:`TRAKer`.
+        the :class:`.TRAKer`.
 
         Args:
-            batch (Iterable[Tensor]): input batch
-            inds (Optional[Iterable[int]], optional): Indices of the batch
-            samples in the train set. Defaults to None.
-            num_samples (Optional[int], optional): Number of samples in the
-            batch. Defaults to None.
+            batch (Iterable[Tensor]):
+                input batch
+            inds (Optional[Iterable[int]], optional):
+                Indices of the batch samples in the train set. Defaults to None.
+            num_samples (Optional[int], optional):
+                Number of samples in the batch. Defaults to None.
+
         """
         assert (inds is None) or (num_samples is None),\
             "Exactly one of num_samples and inds should be specified"
         assert (inds is not None) or (num_samples is not None),\
             "Exactly one of num_samples and inds should be specified"
 
         # TODO: currently this is breaking abstraction -- either define dict
@@ -290,34 +317,37 @@
 
         grads = self.projector.project(grads, model_id=self.saver.current_model_id)
 
         self.saver.current_target_grads[inds] = grads.cpu().clone().detach()
 
     def finalize_scores(self,
                         model_ids: Iterable[int] = None,
-                        del_grads: bool = True,
+                        del_grads: bool = False,
                         exp_name: str = None) -> Tensor:
         """ This method computes the final TRAK scores for the given targets,
         train samples, and model checkpoints (specified by model IDs).
 
         Args:
-            model_ids (Iterable[int], optional): A list of model IDs for which
+            model_ids (Iterable[int], optional):
+                A list of model IDs for which
                 scores should be finalized. If None, scores are computed
-                for all model IDs in the :code:`save_dir` of the :func:`TRAKer`
+                for all model IDs in the :code:`save_dir` of the :class:`.TRAKer`
                 class. Defaults to None.
-            del_grads (bool, optional): If True, the target gradients
-                (intermediate results) are deleted from the internal store of the
-                :func:`TRAKer` class.  Defaults to True.
-            exp_name (str, optional): Used to name the scores :code:`.npy`
-                array produced by this method in the :code:`save_dir` of the
-                :func:`TRAKer` class. If None, a random uuid is generated.
-                Defaults to None.
+            del_grads (bool, optional):
+                If True, the target gradients (intermediate results) are deleted
+                from the internal store of the :class:`.TRAKer` class.  Defaults
+                to True.
+            exp_name (str, optional):
+                Used to name the scores :code:`.npy` array produced by this
+                method in the :code:`save_dir` of the :class:`.TRAKer` class. If
+                None, a random uuid is generated.  Defaults to None.
 
         Returns:
             Tensor: TRAK scores
+
         """
         # reset counter for inds used for scoring
         self._last_ind_target = 0
 
         if model_ids is None:
             model_ids = self.saver.model_ids
```

### Comparing `traker-0.1.1/trak/utils.py` & `traker-0.1.2/trak/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import torch
 ch = torch
 
 
 def parameters_to_vector(parameters) -> Tensor:
     """
     Same as https://pytorch.org/docs/stable/generated/torch.nn.utils.parameters_to_vector.html
-    but with `reshape` instead of `view` to avoid a pesky error.
+    but with :code:`reshape` instead of :code:`view` to avoid a pesky error.
     """
     vec = []
     for param in parameters:
         vec.append(param.reshape(-1))
     return ch.cat(vec)
 
 
@@ -27,18 +27,18 @@
     if ('running_mean' in name) or ('running_var' in name) or ('num_batches_tracked' in name):
         return False
     return True
 
 
 def vectorize_and_ignore_buffers(g, params_dict=None) -> Tensor:
     """
-    gradients are given as a tuple (grad_w0, grad_w1, ... grad_wp)
-    where p is the number of weight matrices. each grad_wi has shape
-    [batch_size, ...]
-    this f-n flattens g to have shape [batch_size, num_params]
+    gradients are given as a tuple :code:`(grad_w0, grad_w1, ... grad_wp)` where
+    :code:`p` is the number of weight matrices. each :code:`grad_wi` has shape
+    :code:`[batch_size, ...]` this function flattens :code:`g` to have shape
+    :code:`[batch_size, num_params]`.
     """
     batch_size = len(g[0])
     out = []
     if params_dict is not None:
         for b in range(batch_size):
             out.append(ch.cat([x[b].flatten() for i, x in enumerate(g) if is_not_buffer(i, params_dict)]))
     else:
```

