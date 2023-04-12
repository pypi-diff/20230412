# Comparing `tmp/sherpa-onnx-1.4.0.tar.gz` & `tmp/sherpa-onnx-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.4.0.tar", last modified: Tue Apr  4 12:03:13 2023, max compression
+gzip compressed data, was "sherpa-onnx-1.4.1.tar", last modified: Wed Apr 12 11:33:58 2023, max compression
```

## Comparing `sherpa-onnx-1.4.0.tar` & `sherpa-onnx-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:03:13.189097 sherpa-onnx-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-04 11:54:13.000000 sherpa-onnx-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-04 12:03:13.189097 sherpa-onnx-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-04 11:54:13.000000 sherpa-onnx-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 12:03:13.189097 sherpa-onnx-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-04 11:54:13.000000 sherpa-onnx-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:03:13.189097 sherpa-onnx-1.4.0/sherpa-onnx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:03:13.189097 sherpa-onnx-1.4.0/sherpa-onnx/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:03:13.189097 sherpa-onnx-1.4.0/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-04 12:03:13.000000 sherpa-onnx-1.4.0/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-04 11:54:13.000000 sherpa-onnx-1.4.0/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-04 11:54:13.000000 sherpa-onnx-1.4.0/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:03:13.189097 sherpa-onnx-1.4.0/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-04 12:03:13.000000 sherpa-onnx-1.4.0/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-04 12:03:13.000000 sherpa-onnx-1.4.0/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:03:13.000000 sherpa-onnx-1.4.0/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:03:13.000000 sherpa-onnx-1.4.0/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 12:03:13.000000 sherpa-onnx-1.4.0/sherpa_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-04 12:03:13.000000 sherpa-onnx-1.4.0/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:33:58.851428 sherpa-onnx-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 11:22:47.000000 sherpa-onnx-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-12 11:33:58.851428 sherpa-onnx-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-12 11:22:47.000000 sherpa-onnx-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 11:33:58.851428 sherpa-onnx-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-12 11:22:47.000000 sherpa-onnx-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:33:58.847428 sherpa-onnx-1.4.1/sherpa-onnx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:33:58.847428 sherpa-onnx-1.4.1/sherpa-onnx/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:33:58.847428 sherpa-onnx-1.4.1/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-12 11:22:47.000000 sherpa-onnx-1.4.1/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-12 11:22:47.000000 sherpa-onnx-1.4.1/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:33:58.851428 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 11:33:58.000000 sherpa-onnx-1.4.1/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.4.0/LICENSE` & `sherpa-onnx-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.0/PKG-INFO` & `sherpa-onnx-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.4.0
+Version: 1.4.1
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.4.0/setup.py` & `sherpa-onnx-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.0/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.4.1/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Copyright (c)  2023 by manyeyes
 from pathlib import Path
 from typing import List
 
 from _sherpa_onnx import (
     OfflineFeatureExtractorConfig,
-    OfflineRecognizer as _Recognizer,
+    OfflineModelConfig,
+    OfflineNemoEncDecCtcModelConfig,
+    OfflineParaformerModelConfig,
+)
+from _sherpa_onnx import OfflineRecognizer as _Recognizer
+from _sherpa_onnx import (
     OfflineRecognizerConfig,
     OfflineStream,
-    OfflineModelConfig,
     OfflineTransducerModelConfig,
-    OfflineParaformerModelConfig,
 )
 
 
 def _assert_file_exists(f: str):
     assert Path(f).is_file(), f"{f} does not exist"
 
 
@@ -71,15 +74,14 @@
         self = cls.__new__(cls)
         model_config = OfflineModelConfig(
             transducer=OfflineTransducerModelConfig(
                 encoder_filename=encoder,
                 decoder_filename=decoder,
                 joiner_filename=joiner,
             ),
-            paraformer=OfflineParaformerModelConfig(model=""),
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
         )
 
         feat_config = OfflineFeatureExtractorConfig(
             sampling_rate=sample_rate,
@@ -115,39 +117,94 @@
           tokens:
             Path to ``tokens.txt``. Each line in ``tokens.txt`` contains two
             columns::
 
                 symbol integer_id
 
           paraformer:
-            Path to ``paraformer.onnx``.
+            Path to ``model.onnx``.
           num_threads:
             Number of threads for neural network computation.
           sample_rate:
             Sample rate of the training data used to train the model.
           feature_dim:
             Dimension of the feature used to train the model.
           decoding_method:
             Valid values are greedy_search, modified_beam_search.
           debug:
             True to show debug messages.
         """
         self = cls.__new__(cls)
         model_config = OfflineModelConfig(
-            transducer=OfflineTransducerModelConfig(
-                encoder_filename="", decoder_filename="", joiner_filename=""
-            ),
             paraformer=OfflineParaformerModelConfig(model=paraformer),
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
         )
 
         feat_config = OfflineFeatureExtractorConfig(
             sampling_rate=sample_rate,
+            feature_dim=feature_dim,
+        )
+
+        recognizer_config = OfflineRecognizerConfig(
+            feat_config=feat_config,
+            model_config=model_config,
+            decoding_method=decoding_method,
+        )
+        self.recognizer = _Recognizer(recognizer_config)
+        return self
+
+    @classmethod
+    def from_nemo_ctc(
+        cls,
+        model: str,
+        tokens: str,
+        num_threads: int,
+        sample_rate: int = 16000,
+        feature_dim: int = 80,
+        decoding_method: str = "greedy_search",
+        debug: bool = False,
+    ):
+        """
+        Please refer to
+        `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/index.html>`_
+        to download pre-trained models for different languages, e.g., Chinese,
+        English, etc.
+
+        Args:
+          tokens:
+            Path to ``tokens.txt``. Each line in ``tokens.txt`` contains two
+            columns::
+
+                symbol integer_id
+
+          model:
+            Path to ``model.onnx``.
+          num_threads:
+            Number of threads for neural network computation.
+          sample_rate:
+            Sample rate of the training data used to train the model.
+          feature_dim:
+            Dimension of the feature used to train the model.
+          decoding_method:
+            Valid values are greedy_search, modified_beam_search.
+          debug:
+            True to show debug messages.
+        """
+        self = cls.__new__(cls)
+        model_config = OfflineModelConfig(
+            nemo_ctc=OfflineNemoEncDecCtcModelConfig(model=model),
+            tokens=tokens,
+            num_threads=num_threads,
+            debug=debug,
+        )
+
+        feat_config = OfflineFeatureExtractorConfig(
+            sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
 
         recognizer_config = OfflineRecognizerConfig(
             feat_config=feat_config,
             model_config=model_config,
             decoding_method=decoding_method,
```

### Comparing `sherpa-onnx-1.4.0/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.4.1/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.0/sherpa_onnx.egg-info/PKG-INFO` & `sherpa-onnx-1.4.1/sherpa_onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.4.0
+Version: 1.4.1
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

