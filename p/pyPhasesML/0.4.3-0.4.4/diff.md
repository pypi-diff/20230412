# Comparing `tmp/pyPhasesML-0.4.3.tar.gz` & `tmp/pyPhasesML-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.4.3.tar", last modified: Wed Apr 12 10:50:55 2023, max compression
+gzip compressed data, was "pyPhasesML-0.4.4.tar", last modified: Wed Apr 12 11:53:07 2023, max compression
```

## Comparing `pyPhasesML-0.4.3.tar` & `pyPhasesML-0.4.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 10:50:55.787641 pyPhasesML-0.4.3/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-12 10:50:55.786641 pyPhasesML-0.4.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 10:50:55.780640 pyPhasesML-0.4.3/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 10:50:55.783641 pyPhasesML-0.4.3/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)    17729 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/adapter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 10:50:55.784641 pyPhasesML-0.4.3/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 10:50:55.786641 pyPhasesML-0.4.3/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    22289 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 10:50:55.782641 pyPhasesML-0.4.3/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-12 10:50:55.000000 pyPhasesML-0.4.3/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      838 2023-04-12 10:50:55.000000 pyPhasesML-0.4.3/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 10:50:55.000000 pyPhasesML-0.4.3/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 10:50:55.000000 pyPhasesML-0.4.3/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-12 10:50:55.000000 pyPhasesML-0.4.3/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-12 10:50:27.000000 pyPhasesML-0.4.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 10:50:55.787641 pyPhasesML-0.4.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-04-12 10:50:29.000000 pyPhasesML-0.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:53:07.865352 pyPhasesML-0.4.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-12 11:53:07.865352 pyPhasesML-0.4.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:53:07.859351 pyPhasesML-0.4.4/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:53:07.862352 pyPhasesML-0.4.4/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    17734 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/adapter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:53:07.863352 pyPhasesML-0.4.4/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:53:07.864352 pyPhasesML-0.4.4/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    22289 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:53:07.861352 pyPhasesML-0.4.4/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-12 11:53:07.000000 pyPhasesML-0.4.4/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      838 2023-04-12 11:53:07.000000 pyPhasesML-0.4.4/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:53:07.000000 pyPhasesML-0.4.4/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 11:53:07.000000 pyPhasesML-0.4.4/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-12 11:53:07.000000 pyPhasesML-0.4.4/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:53:07.865352 pyPhasesML-0.4.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-04-12 11:52:41.000000 pyPhasesML-0.4.4/setup.py
```

### Comparing `pyPhasesML-0.4.3/LICENSE` & `pyPhasesML-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/PKG-INFO` & `pyPhasesML-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.4.3/README.md` & `pyPhasesML-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.4.4/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML/DataSet.py` & `pyPhasesML-0.4.4/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.4.4/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML/Model.py` & `pyPhasesML-0.4.4/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML/ModelManager.py` & `pyPhasesML-0.4.4/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML/Plugin.py` & `pyPhasesML-0.4.4/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.4.4/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.4.4/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.4.4/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.4.4/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                             return max(0, (1 - x)) * scaler(cycle)
 
                         return lr_lambda
                     # setup optimizer and scheduler
                     optimizer = torch.optim.Adam(model.parameters(), lr=1.)
                     step_size = 4*len(dataset.trainingData)
                     clr = cyclical_lr(step_size, min_lr=lr, max_lr=lrMax)
-                    self.scheduler = torch.optim.lr_scheduler.LambdaLR(optimizer, [clr])
+                    self.batchScheduler = torch.optim.lr_scheduler.LambdaLR(optimizer, [clr])
 
         if self.oneCyclicLR:
             lr = self.learningRate / self.cycleLRFactor
             lrMax = self.learningRate
             steps = self.maxEpochs * len(dataset.trainingData)
 
             self.batchScheduler = torch.optim.lr_scheduler.OneCycleLR(optimizer, max_lr=lrMax, total_steps=steps, cycle_momentum=False)
```

### Comparing `pyPhasesML-0.4.3/pyPhasesML/config.yaml` & `pyPhasesML-0.4.4/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.4.4/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.4.4/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.4.4/pyPhasesML/scorer/Scorer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.4.4/pyPhasesML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.4.3/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.4.4/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.3/setup.py` & `pyPhasesML-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.4.3"[1:],
+    version="v0.4.4"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

