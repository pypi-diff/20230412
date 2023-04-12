# Comparing `tmp/pytorch-accelerated-0.1.8.tar.gz` & `tmp/pytorch-accelerated-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-accelerated-0.1.8.tar", last modified: Sat Dec 11 12:26:19 2021, max compression
+gzip compressed data, was "pytorch-accelerated-0.1.9.tar", last modified: Fri Dec 31 11:17:56 2021, max compression
```

## Comparing `pytorch-accelerated-0.1.8.tar` & `pytorch-accelerated-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 12:26:19.831570 pytorch-accelerated-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11113 2021-12-11 12:26:19.831570 pytorch-accelerated-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8862 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 12:26:19.831570 pytorch-accelerated-0.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2778 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/custom_callback_event.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 12:26:19.831570 pytorch-accelerated-0.1.8/examples/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3349 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/metrics/train_with_metrics_in_callback.py
--rw-r--r--   0 runner    (1001) docker     (121)     3043 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/metrics/train_with_metrics_in_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/train_mnist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 12:26:19.831570 pytorch-accelerated-0.1.8/examples/vision/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 12:26:19.831570 pytorch-accelerated-0.1.8/examples/vision/transfer_learning/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/vision/transfer_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7584 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/vision/transfer_learning/hf_pets_cv_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     5155 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/vision/transfer_learning/progressive_resizing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2653 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/vision/transfer_learning/pytorch_tutorial_finetune.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 12:26:19.831570 pytorch-accelerated-0.1.8/examples/vision/using_timm_components/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/vision/using_timm_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5902 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/vision/using_timm_components/basic_timm_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     9618 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/examples/vision/using_timm_components/train_imagenette_mixup_ema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 12:26:19.835570 pytorch-accelerated-0.1.8/pytorch_accelerated/
--rw-r--r--   0 runner    (1001) docker     (121)      441 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/pytorch_accelerated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2021-12-11 12:26:19.835570 pytorch-accelerated-0.1.8/pytorch_accelerated/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    16528 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/pytorch_accelerated/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2411 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/pytorch_accelerated/run_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/pytorch_accelerated/tracking.py
--rw-r--r--   0 runner    (1001) docker     (121)    31360 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/pytorch_accelerated/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 12:26:19.831570 pytorch-accelerated-0.1.8/pytorch_accelerated.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11113 2021-12-11 12:26:19.000000 pytorch-accelerated-0.1.8/pytorch_accelerated.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2021-12-11 12:26:19.000000 pytorch-accelerated-0.1.8/pytorch_accelerated.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-11 12:26:19.000000 pytorch-accelerated-0.1.8/pytorch_accelerated.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-12-11 12:26:19.000000 pytorch-accelerated-0.1.8/pytorch_accelerated.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-12-11 12:26:19.000000 pytorch-accelerated-0.1.8/pytorch_accelerated.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-12-11 12:26:19.831570 pytorch-accelerated-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2402 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    80049 2021-12-11 12:26:06.000000 pytorch-accelerated-0.1.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 11:17:56.931388 pytorch-accelerated-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    11113 2021-12-31 11:17:56.931388 pytorch-accelerated-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8862 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 11:17:56.923388 pytorch-accelerated-0.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2778 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/custom_callback_event.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 11:17:56.923388 pytorch-accelerated-0.1.9/examples/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3349 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/metrics/train_with_metrics_in_callback.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3043 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/metrics/train_with_metrics_in_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/train_mnist.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 11:17:56.923388 pytorch-accelerated-0.1.9/examples/vision/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 11:17:56.923388 pytorch-accelerated-0.1.9/examples/vision/transfer_learning/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/vision/transfer_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7532 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/vision/transfer_learning/hf_pets_cv_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8410 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/vision/transfer_learning/pets_finetune.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5155 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/vision/transfer_learning/progressive_resizing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2653 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/vision/transfer_learning/pytorch_tutorial_finetune.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 11:17:56.927388 pytorch-accelerated-0.1.9/examples/vision/using_timm_components/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/vision/using_timm_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5902 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/vision/using_timm_components/basic_timm_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9618 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/examples/vision/using_timm_components/train_imagenette_mixup_ema.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 11:17:56.931388 pytorch-accelerated-0.1.9/pytorch_accelerated/
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/pytorch_accelerated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2021-12-31 11:17:56.931388 pytorch-accelerated-0.1.9/pytorch_accelerated/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16528 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/pytorch_accelerated/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9018 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/pytorch_accelerated/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2411 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/pytorch_accelerated/run_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3602 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/pytorch_accelerated/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32152 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/pytorch_accelerated/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 11:17:56.931388 pytorch-accelerated-0.1.9/pytorch_accelerated.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    11113 2021-12-31 11:17:56.000000 pytorch-accelerated-0.1.9/pytorch_accelerated.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-12-31 11:17:56.000000 pytorch-accelerated-0.1.9/pytorch_accelerated.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-31 11:17:56.000000 pytorch-accelerated-0.1.9/pytorch_accelerated.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2021-12-31 11:17:56.000000 pytorch-accelerated-0.1.9/pytorch_accelerated.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-12-31 11:17:56.000000 pytorch-accelerated-0.1.9/pytorch_accelerated.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2021-12-31 11:17:56.931388 pytorch-accelerated-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2402 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    80049 2021-12-31 11:17:53.000000 pytorch-accelerated-0.1.9/versioneer.py
```

### Comparing `pytorch-accelerated-0.1.8/LICENSE.txt` & `pytorch-accelerated-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/PKG-INFO` & `pytorch-accelerated-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-accelerated
-Version: 0.1.8
+Version: 0.1.9
 Summary: A lightweight library designed to accelerate the process of training PyTorch models by providing a minimal, but extensible training loop which is flexible enough to handle the majority of use cases, and capable of utilizing different hardware options with no code changes required.
 Home-page: https://github.com/Chris-hughes10/pytorch-accelerated
 Author: Chris Hughes
 Author-email: 31883449+Chris-hughes10@users.noreply.github.com
 License: UNKNOWN
 Description: 
         # pytorch-accelerated
```

### Comparing `pytorch-accelerated-0.1.8/README.md` & `pytorch-accelerated-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/examples/custom_callback_event.py` & `pytorch-accelerated-0.1.9/examples/custom_callback_event.py`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/examples/metrics/train_with_metrics_in_callback.py` & `pytorch-accelerated-0.1.9/examples/metrics/train_with_metrics_in_callback.py`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/examples/metrics/train_with_metrics_in_loop.py` & `pytorch-accelerated-0.1.9/examples/metrics/train_with_metrics_in_loop.py`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/examples/train_mnist.py` & `pytorch-accelerated-0.1.9/examples/train_mnist.py`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/examples/vision/transfer_learning/hf_pets_cv_example.py` & `pytorch-accelerated-0.1.9/examples/vision/transfer_learning/hf_pets_cv_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 
 
 class PetsTrainer(Trainer):
     def training_run_start(self):
         config = self._accelerator.unwrap_model(self.model).default_cfg
 
         self.mean = torch.tensor(config["mean"])[None, :, None, None].to(
-            self._accelerator.device
+            self.device
         )
         self.std = torch.tensor(config["std"])[None, :, None, None].to(
-            self._accelerator.device
+            self.device
         )
 
     def calculate_train_batch_loss(self, batch):
         inputs = (batch["image"] - self.mean) / self.std
 
         return super().calculate_train_batch_loss((inputs, batch["label"]))
 
@@ -67,17 +67,17 @@
     def calculate_eval_batch_loss(self, batch):
         inputs = (batch["image"] - self.mean) / self.std
 
         with torch.no_grad():
             outputs = self.model(inputs)
             loss = self.loss_func(outputs, batch["label"])
         predictions = outputs.argmax(dim=-1)
-        accurate_preds = self._accelerator.gather(
+        accurate_preds = self.gather(
             predictions
-        ) == self._accelerator.gather(batch["label"])
+        ) == self.gather(batch["label"])
         self.num_elems += accurate_preds.shape[0]
         self.accurate += accurate_preds.long().sum()
 
         return {
             "loss": loss,
             "model_outputs": outputs,
             "batch_size": inputs.size(0),
```

### Comparing `pytorch-accelerated-0.1.8/examples/vision/transfer_learning/progressive_resizing.py` & `pytorch-accelerated-0.1.9/examples/vision/transfer_learning/progressive_resizing.py`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/examples/vision/transfer_learning/pytorch_tutorial_finetune.py` & `pytorch-accelerated-0.1.9/examples/vision/transfer_learning/pytorch_tutorial_finetune.py`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/examples/vision/using_timm_components/basic_timm_example.py` & `pytorch-accelerated-0.1.9/examples/vision/using_timm_components/basic_timm_example.py`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/examples/vision/using_timm_components/train_imagenette_mixup_ema.py` & `pytorch-accelerated-0.1.9/examples/vision/using_timm_components/train_imagenette_mixup_ema.py`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/pytorch_accelerated/callbacks.py` & `pytorch-accelerated-0.1.9/pytorch_accelerated/callbacks.py`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/pytorch_accelerated/run_config.py` & `pytorch-accelerated-0.1.9/pytorch_accelerated/run_config.py`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/pytorch_accelerated/tracking.py` & `pytorch-accelerated-0.1.9/pytorch_accelerated/tracking.py`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/pytorch_accelerated/trainer.py` & `pytorch-accelerated-0.1.9/pytorch_accelerated/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -490,19 +490,21 @@
         """
         return self._accelerator.device
 
     def _prepare_model_optimizer_and_dataloaders(self):
         """
         Uses the trainer's instance of :class:`accelerate.Accelerator` to wrap the model, optimizer and dataloaders in any wrappers necessary for training.
         (e.g. :class:`torch.nn.parallel.DistributedDataParallel`) and ensures the parameters are placed on the appropriate device.
-         By default, this will convert each dataloader to an instance of :class:`accelerate.data_loader.DataLoaderShard`.
+        By default, this will convert each dataloader to an instance of :class:`accelerate.data_loader.DataLoaderShard`.
 
-         .. Note:: This may change the length of the dataloaders, so this should be called *before* the number of update steps per epoch is calculated, i.e. to initialise a learning rate scheduler
+        .. Note:: This may change the length of the dataloaders, so this should be called *before* the number of update steps per epoch is calculated, i.e. to initialise a learning rate scheduler
         """
         self._accelerator.free_memory()
+        self._accelerator = self._create_accelerator()
+
         components = [self.model, self.optimizer]
 
         if self._train_dataloader is not None:
             components.append(self._train_dataloader)
 
         if self._eval_dataloader is not None:
             components.append(self._eval_dataloader)
@@ -658,15 +660,15 @@
         for step, batch in enumerate(train_dl):
             self.callback_handler.call_event(
                 "on_train_step_start",
                 self,
             )
             batch_output = self.calculate_train_batch_loss(batch)
             self._loss_tracker.update(
-                self._accelerator.gather(batch_output["loss"]).detach().mean().item(),
+                self.gather(batch_output["loss"]).detach().mean().item(),
                 batch_output["batch_size"],
             )
             if self.run_config.gradient_accumulation_steps > 1:
                 batch_output["loss"] /= self.run_config.gradient_accumulation_steps
 
             self.callback_handler.call_event(
                 "on_train_step_end", self, batch_output=batch_output, batch=batch
@@ -721,28 +723,40 @@
         for batch in valid_dl:
             self.callback_handler.call_event(
                 "on_eval_step_start",
                 self,
             )
             batch_output = self.calculate_eval_batch_loss(batch)
             self._loss_tracker.update(
-                self._accelerator.gather(batch_output["loss"]).detach().mean().item(),
+                self.gather(batch_output["loss"]).detach().mean().item(),
                 batch_output["batch_size"],
             )
             self.callback_handler.call_event(
                 "on_eval_step_end", self, batch_output=batch_output, batch=batch
             )
         self.eval_epoch_end()
         metric_name = "eval_loss_epoch" if is_training else "evaluation_loss"
         self.run_history.update_metric(metric_name, self._loss_tracker.average)
         self.callback_handler.call_event(
             "on_eval_epoch_end",
             self,
         )
 
+    def gather(self, tensor):
+        """
+        Gather the values in `tensor` across all processes and concatenate them on the first dimension. This can be
+        useful to regroup the predictions from all processes when doing evaluation.
+
+        .. Note:: This gather happens in all processes.
+
+        :param tensor: (:obj:`torch.Tensor`, or a nested tuple/list/dictionary of :obj:`torch.Tensor`) The tensors to gather across all processes.
+        :return: The gathered tensor(s) (:obj:`torch.Tensor`, or a nested tuple/list/dictionary of :obj:`torch.Tensor`). The first dimension of the result is `num_processes` multiplied by the first dimension of the input tensors.
+        """
+        return self._accelerator.gather(tensor)
+
     def print(self, *args, **kwargs):
         """
         Use in replacement of ``print()`` to only print once per node.
         """
         if self._accelerator is not None:
             self._accelerator.print(*args, **kwargs)
         else:
@@ -753,15 +767,15 @@
     ):
         """
         Save the model, optimizer and specified args as a checkpoint file.
 
         :param save_path: the path where to save the checkpoint, this should end in '.pt'
         :param checkpoint_kwargs: additional objects to include in the checkpoint
         :param save_optimizer: flag to indicate whether to include the optimizer in the checkpoint
-        :param save_per_node: flag to indicate whether to save the checkpoint once per machine, if False, the checkpoint will only be saved from the world process zero
+        :param save_per_node: flag to indicate whether to save the checkpoint once per machine, if False, the checkpoint will only be saved from the world process zero. This is True by default.
         """
         # TODO: add save method for run history?
 
         checkpoint = {
             "model_state_dict": self._accelerator.unwrap_model(self.model).state_dict(),
         }
```

### Comparing `pytorch-accelerated-0.1.8/pytorch_accelerated.egg-info/PKG-INFO` & `pytorch-accelerated-0.1.9/pytorch_accelerated.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-accelerated
-Version: 0.1.8
+Version: 0.1.9
 Summary: A lightweight library designed to accelerate the process of training PyTorch models by providing a minimal, but extensible training loop which is flexible enough to handle the majority of use cases, and capable of utilizing different hardware options with no code changes required.
 Home-page: https://github.com/Chris-hughes10/pytorch-accelerated
 Author: Chris Hughes
 Author-email: 31883449+Chris-hughes10@users.noreply.github.com
 License: UNKNOWN
 Description: 
         # pytorch-accelerated
```

### Comparing `pytorch-accelerated-0.1.8/pytorch_accelerated.egg-info/SOURCES.txt` & `pytorch-accelerated-0.1.9/pytorch_accelerated.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 examples/train_mnist.py
 examples/metrics/__init__.py
 examples/metrics/train_with_metrics_in_callback.py
 examples/metrics/train_with_metrics_in_loop.py
 examples/vision/__init__.py
 examples/vision/transfer_learning/__init__.py
 examples/vision/transfer_learning/hf_pets_cv_example.py
+examples/vision/transfer_learning/pets_finetune.py
 examples/vision/transfer_learning/progressive_resizing.py
 examples/vision/transfer_learning/pytorch_tutorial_finetune.py
 examples/vision/using_timm_components/__init__.py
 examples/vision/using_timm_components/basic_timm_example.py
 examples/vision/using_timm_components/train_imagenette_mixup_ema.py
 pytorch_accelerated/__init__.py
 pytorch_accelerated/_version.py
 pytorch_accelerated/callbacks.py
+pytorch_accelerated/finetuning.py
 pytorch_accelerated/run_config.py
 pytorch_accelerated/tracking.py
 pytorch_accelerated/trainer.py
 pytorch_accelerated.egg-info/PKG-INFO
 pytorch_accelerated.egg-info/SOURCES.txt
 pytorch_accelerated.egg-info/dependency_links.txt
 pytorch_accelerated.egg-info/requires.txt
```

### Comparing `pytorch-accelerated-0.1.8/setup.py` & `pytorch-accelerated-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `pytorch-accelerated-0.1.8/versioneer.py` & `pytorch-accelerated-0.1.9/versioneer.py`

 * *Files identical despite different names*

