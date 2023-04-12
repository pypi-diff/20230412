# Comparing `tmp/pyPhasesML-0.4.1.tar.gz` & `tmp/pyPhasesML-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.4.1.tar", last modified: Thu Mar 30 09:26:38 2023, max compression
+gzip compressed data, was "pyPhasesML-0.4.2.tar", last modified: Wed Apr 12 08:46:21 2023, max compression
```

## Comparing `pyPhasesML-0.4.1.tar` & `pyPhasesML-0.4.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:26:38.675868 pyPhasesML-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3691 2023-03-30 09:26:38.674868 pyPhasesML-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:26:38.668868 pyPhasesML-0.4.1/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)     7247 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     1491 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     4656 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)     4547 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4558 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:26:38.671868 pyPhasesML-0.4.1/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10212 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)    16304 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/adapter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:26:38.672868 pyPhasesML-0.4.1/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5358 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:26:38.674868 pyPhasesML-0.4.1/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    22302 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 09:26:38.670868 pyPhasesML-0.4.1/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3691 2023-03-30 09:26:38.000000 pyPhasesML-0.4.1/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      838 2023-03-30 09:26:38.000000 pyPhasesML-0.4.1/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 09:26:38.000000 pyPhasesML-0.4.1/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-03-30 09:26:38.000000 pyPhasesML-0.4.1/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-03-30 09:26:38.000000 pyPhasesML-0.4.1/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-03-30 09:26:09.000000 pyPhasesML-0.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 09:26:38.675868 pyPhasesML-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-03-30 09:26:11.000000 pyPhasesML-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:46:21.321825 pyPhasesML-0.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-12 08:46:21.320826 pyPhasesML-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:46:21.315831 pyPhasesML-0.4.2/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:46:21.318828 pyPhasesML-0.4.2/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    17693 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/adapter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:46:21.319827 pyPhasesML-0.4.2/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:46:21.320826 pyPhasesML-0.4.2/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    22289 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:46:21.317829 pyPhasesML-0.4.2/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-12 08:46:21.000000 pyPhasesML-0.4.2/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      838 2023-04-12 08:46:21.000000 pyPhasesML-0.4.2/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 08:46:21.000000 pyPhasesML-0.4.2/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 08:46:21.000000 pyPhasesML-0.4.2/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-12 08:46:21.000000 pyPhasesML-0.4.2/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-12 08:45:54.000000 pyPhasesML-0.4.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 08:46:21.321825 pyPhasesML-0.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-04-12 08:45:56.000000 pyPhasesML-0.4.2/setup.py
```

### Comparing `pyPhasesML-0.4.1/LICENSE` & `pyPhasesML-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.1/PKG-INFO` & `pyPhasesML-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.4.1/README.md` & `pyPhasesML-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.1/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.4.2/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.1/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.4.2/pyPhasesML/FeatureExtraction.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from pyPhases import classLogger
 from pyPhasesRecordloader import RecordSignal, Signal
 
 
 @classLogger
 class FeatureExtraction:
 
-    def step(self, stepname, recordSignal, **options):
+    def step(self, stepname: str, recordSignal: RecordSignal, **options) -> Signal:
         if hasattr(self, stepname):
             # call method
             return getattr(self, stepname)(recordSignal, **options)
         else:
             raise Exception(f"FeatureExtraction '{stepname}' not found")
 
-    def __call__(self, recordSignal, config=None):
+    def __call__(self, recordSignal: RecordSignal, config: dict = None):
         return self.extractChannelsByConfig(recordSignal, config)
 
-    def extractChannelsByConfig(self, recordSignal, config):
+    def extractChannelsByConfig(self, recordSignal: RecordSignal, config: dict):
 
         for c in config:
             self.extractChannelByConfig(recordSignal, c)
 
-    def addSingle(self, name, recordSignal: RecordSignal, signalOrArray):
+    def addSingle(self, name: str, recordSignal: RecordSignal, signalOrArray: Signal):
         if not isinstance(signalOrArray, Signal):
             signalOrArray = Signal(name, signalOrArray, frequency=recordSignal.targetFrequency)
         signalOrArray.name = name
         recordSignal.addSignal(signalOrArray, name)
 
-    def extractChannelByConfig(self, recordSignal, config):
+    def extractChannelByConfig(self, recordSignal: RecordSignal, config: dict):
         config = config.copy()
         name = config["name"]
         channels = config["channels"]
         del config["name"]
         del config["channels"]
 
         ret = self.step(name, recordSignal, **config)
```

### Comparing `pyPhasesML-0.4.1/pyPhasesML/ModelManager.py` & `pyPhasesML-0.4.2/pyPhasesML/ModelManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
             if ModelManager.modelOptions is None:
                 raise Exception("ModelManager setModel was never called!")
             else:
                 ModelManager.loadModelFromOptions()
         return ModelManager.model
 
     def loadModelFromOptions() -> None:
-
         options = ModelManager.modelOptions
         modelClass = ModelManager.loadModelByModule(options["modelName"])
         model = modelClass(options["modelConfig"])
 
         for field in options["general"]:
             setattr(model, field, options["general"][field])
 
@@ -33,22 +32,16 @@
             ModelManager.beforeBuild(model)
 
         model.init()
         model.define()
         model.build()
         ModelManager.model = model
 
-    def checkValueInConfig(self, config, value):
-
-        if value not in config:
-            raise ConfigNotFoundException("The value '%s' is required in the config" % value)
-
     def validate(config):
         def checkValueInConfig(config, value, valuePath=None):
-
             checkDict = config if valuePath is None else config[valuePath]
 
             if value not in checkDict:
                 valuePath = value if valuePath is None else valuePath + "." + value
                 raise ConfigNotFoundException("The value '%s' is required in the config" % valuePath)
 
         checkValueInConfig(config, "modelName")
```

### Comparing `pyPhasesML-0.4.1/pyPhasesML/Plugin.py` & `pyPhasesML-0.4.2/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.1/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.4.2/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.1/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.4.2/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.1/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.4.2/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.1/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.4.2/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import gc
 import math
 import os
+import pickle
 import timeit
 
 import numpy as np
 import psutil
 import torch
 import torch.optim as optim
+from pyPhases import CSVLogger
 from tqdm import tqdm
 
-from ..DataSet import DataSet, TrainingSet
+from ..DataSet import DataSet, TrainingSetLoader
 from ..Model import Model
 from ..scorer.ScorerTorch import ScorerTorch
 
 
 class ModelTorchAdapter(Model):
     model: torch.nn.Module
     useGPU = torch.cuda.is_available()
     useTensorBoard = False
     saveOnlyWeights = True
     findLearningRate = False
     oneCyclicLR = False
     cycleLR = False
+    cycleLRCustom = False
     cycleLRFactor = 4
     cycleLRStepsideFactor = 2
     cycleLRMax = 2
     findLearningRatePlot = "data/learningRate.png"
 
     def _metrics(self, metric):
         return "val_" + metric["name"]
@@ -126,80 +129,106 @@
 
             if self.ignoreClassIndex is not None:
                 mask = targets != self.ignoreClassIndex
                 targets = targets[mask]
 
         return targets.float(), mask
 
-    def train(self, dataset: TrainingSet):
+    def train(self, dataset: TrainingSetLoader):
         if ModelTorchAdapter.useTensorBoard:
             from torch.utils.tensorboard import SummaryWriter
 
             self.summarywriter = SummaryWriter()
 
             for f, title in self.startFigures:
                 self.summarywriter.add_figure(title, f)
         else:
             self.summarywriter = None
-        self.cleanCsv()
+
+        self.logger = CSVLogger(self.getCsvPath())
 
         metrics = self.validationMetrics
         scorer = ScorerTorch(self.numClasses)
         metricDefinitions = {m: scorer.getMetricDefinition(m) for m in metrics}
 
         model = self.model
         globalBestMetric = self.validationMetrics[0]
         self.batchScheduler = None
 
         self.log("LR: %s" % self.learningRate)
         decay = 0 if self.learningRateDecay is None else self.learningRateDecay
         if self.optimizer == "adams":
-            self.optimizer = optim.Adam(model.parameters(), lr=self.learningRate, weight_decay=decay)
+            optimizer = optim.Adam(model.parameters(), lr=self.learningRate, weight_decay=decay)
         elif self.optimizer == "sgd":
-            self.optimizer = optim.SGD(model.parameters(), lr=self.learningRate, weight_decay=decay)
+            optimizer = optim.SGD(model.parameters(), lr=self.learningRate, weight_decay=decay)
         elif self.optimizer == "nesterov":
-            self.optimizer = optim.SGD(model.parameters(), lr=self.learningRate, weight_decay=decay, nesterov=True)
+            optimizer = optim.SGD(model.parameters(), lr=self.learningRate, weight_decay=decay, nesterov=True)
         elif self.optimizer == "nadams":
             torch.optim.NAdam(model.parameters(), lr=self.learningRate, momentum_decay=decay)
         elif type(self.optimizer) == str:
             raise Exception("optimizer %s is currently not supported for pytorch implementation" % self.optimizer)
+        else:
+            optimizer = self.optimizer
 
         if self.cycleLR:
-            lr = self.learningRate / self.cycleLRFactor
             lrMax = self.learningRate
-            stepSize = self.cycleLRStepsideFactor * len(dataset.trainingData)
+            lr = self.learningRate / self.cycleLRFactor
+            if not self.cycleLRCustom:
+                stepSize = self.cycleLRStepsideFactor * len(dataset.trainingData)
 
-            self.batchScheduler = torch.optim.lr_scheduler.CyclicLR(
-                self.optimizer, base_lr=self.learningRate / lr, max_lr=lrMax, step_size_up=stepSize
-            )
+                self.batchScheduler = torch.optim.lr_scheduler.CyclicLR(
+                    optimizer, base_lr=self.learningRate / lr, max_lr=lrMax, step_size_up=stepSize
+                )
+            else:
+                    
+                    def cyclical_lr(stepsize, min_lr=3e-4, max_lr=3e-3):
+
+                        # Scaler: we can adapt this if we do not want the triangular CLR
+                        scaler = lambda x: 1.
+
+                        # Lambda function to calculate the LR
+                        lr_lambda = lambda it: min_lr + (max_lr - min_lr) * relative(it, stepsize)
+
+                        # Additional function to see where on the cycle we are
+                        def relative(it, stepsize):
+                            cycle = math.floor(1 + it / (2 * stepsize))
+                            x = abs(it / stepsize - 2 * cycle + 1)
+                            return max(0, (1 - x)) * scaler(cycle)
+
+                        return lr_lambda
+                    # setup optimizer and scheduler
+                    optimizer = torch.optim.Adam(model.parameters(), lr=1.)
+                    step_size = 4*len(dataset.trainingData)
+                    clr = cyclical_lr(step_size, min_lr=lr, max_lr=lrMax)
+                    self.scheduler = torch.optim.lr_scheduler.LambdaLR(optimizer, [clr])
 
         if self.oneCyclicLR:
             lr = self.learningRate / self.cycleLRFactor
             lrMax = self.learningRate
             steps = self.maxEpochs * len(dataset.trainingData)
 
-            self.batchScheduler = torch.optim.lr_scheduler.OneCycleLR(self.optimizer, max_lr=lrMax, total_steps=steps)
+            self.batchScheduler = torch.optim.lr_scheduler.OneCycleLR(optimizer, max_lr=lrMax, total_steps=steps)
 
         if self.findLearningRate:
             start_lr = self.learningRate
             end_lr = self.cycleLRMax
             lr_lambda = lambda x: math.exp(x * math.log(end_lr / start_lr) / (self.maxEpochs * len(dataset.trainingData)))
-            self.batchScheduler = torch.optim.lr_scheduler.LambdaLR(self.optimizer, lr_lambda)
+            self.batchScheduler = torch.optim.lr_scheduler.LambdaLR(optimizer, lr_lambda)
             lr_find_loss = []
             lr_find_lr = []
             smoothing = 0.05
-
+        
         model = self.model
         lossCriterion = self.getLossFunction()
         i_epoch = self.startEpoch
         notImprovedSince = 0
         lastImprovdModel = None
 
         stopAfterNotImproving = 0 if self.stopAfterNotImproving is None else self.stopAfterNotImproving
-
+        
         while self.maxEpochs is None or i_epoch < self.maxEpochs:
             # Put in train mode
             trainingStartTime = timeit.default_timer()
 
             model.train(True)
             runningStats = {"loss": 0.0}
             batchesPerEpoch = len(dataset.trainingData)
@@ -208,15 +237,15 @@
             batchGenerator = iter(dataset.trainingData)
 
             for batchIndex in processList:
                 trainBatch = next(batchGenerator)
                 batchFeats, targs = self.prepareDataAdapter(trainBatch)
                 targs, mask = self.prepareTargetsForLoss(targs)
 
-                self.optimizer.zero_grad()
+                optimizer.zero_grad()
 
                 # check if there are any targets left
                 if len(targs) == 0:
                     continue
 
                 # for batchFeat in batchFeats:
                 output = model(batchFeats)
@@ -231,28 +260,28 @@
                             runningStats[stat] = value
                         else:
                             runningStats[stat] += value
 
                 # Backpropagation
                 loss.backward()
                 # torch.nn.utils.clip_grad()
-                self.optimizer.step()
+                optimizer.step()
 
                 # Perform one optimization step
                 currentBatchLoss = loss.data.cpu().numpy()
                 if np.isnan(currentBatchLoss):
                     model(batchFeats)
                     lossCriterion(output, targs)
                     raise Exception("batch loss should not be a number")
 
                 if self.batchScheduler is not None:
                     self.batchScheduler.step()
 
                 if self.findLearningRate:
-                    lr_step = self.optimizer.state_dict()["param_groups"][0]["lr"]
+                    lr_step = optimizer.state_dict()["param_groups"][0]["lr"]
                     lr_find_lr.append(lr_step)
 
                     # smooth the loss
                     if batchIndex == 0 and i_epoch == 0:
                         lr_find_loss.append(loss)
                     else:
                         loss = smoothing * loss + (1 - smoothing) * lr_find_loss[-1]
@@ -293,14 +322,16 @@
 
                 isBigger = metricVal > bestValue
 
                 if (biggerIsBetter and isBigger) or (not biggerIsBetter and not isBigger):
                     metricDefinitions[metricName][0] = metricVal
                     if useAsBest:
                         improved = True
+                        if metricName == globalBestMetric:
+                            self.bestMetric = max(self.bestMetric, metricsValues[globalBestMetric])
 
             validationEndTime = timeit.default_timer()
 
             self.log(
                 "Validation-Epoch Number: "
                 + str(i_epoch)
                 + "  Training Time: "
@@ -325,16 +356,15 @@
                 "epoch": i_epoch,
             }
             csvRow.update(runningStats)
 
             for metricName in metricsValues:
                 csvRow["val_%s" % metricName] = metricsValues[metricName]
 
-            self.addCsvRow(csvRow)
-            self.bestMetric = max(self.bestMetric, metricsValues[globalBestMetric])
+            self.logger.addCsvRow(csvRow)
 
             # If the validation accuracy improves, print out training and validation accuracy values and checkpoint the model
             if improved:
                 self.log("Model Improved: " + " ".join(metricDiffStrings))
                 f = open(
                     self.getModelPath() + "/" + modelId + "_".join(metricValuetrings) + ".pkl",
                     "wb",
@@ -361,15 +391,14 @@
             plt.savefig(self.findLearningRatePlotPath)
             minLr = lr_find_lr[np.argmin(lr_find_loss)]
             print("Lowest Loss LR: %f" % minLr)
             print("Suggested LR range max bound: %f" % minLr)
             self.lr_find_lr = lr_find_lr
             self.lr_find_loss = lr_find_loss
 
-        self.csvClose()
         self.fullEpochs = i_epoch
         return lastImprovdModel
 
     def getModelPath(self):
         return self.logPath
 
     def build(self):
```

### Comparing `pyPhasesML-0.4.1/pyPhasesML/config.yaml` & `pyPhasesML-0.4.2/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.1/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.4.2/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.1/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.4.2/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.1/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.4.2/pyPhasesML/scorer/Scorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
             self.results["all_values"] = np.histogram(classLikelyhood, bins=b, range=r)[0]
 
             pred_pos = classLikelyhood[truth > 0]
             self.results["pos_values"] = np.histogram(pred_pos, bins=b, range=r)[0]
 
             # Compute the histogram of probabilities within unscored regions
             pred_ign = classLikelyhood[truth < 0]
-            self.results["ign_values"] = ign_values = np.histogram(pred_ign, bins=b, range=r)[0]
+            self.results["ign_values"] = np.histogram(pred_ign, bins=b, range=r)[0]
 
             # Compute the histogram of probabilities in non-arousal regions,
             # given the above
             self.results["neg_values"] = self.results["all_values"] - self.results["pos_values"] - self.results["ign_values"]
             auroc, auprc, _, _, _ = self._auc(self.results["pos_values"], self.results["neg_values"])
             self.results["auprc"] = np.sum(auprc)
             self.results["auroc"] = np.sum(auroc)
```

### Comparing `pyPhasesML-0.4.1/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.4.2/pyPhasesML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.4.1/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.4.2/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.1/setup.py` & `pyPhasesML-0.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.4.1"[1:],
+    version="v0.4.2"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

