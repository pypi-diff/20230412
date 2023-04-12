# Comparing `tmp/ScandEval-6.2.4.tar.gz` & `tmp/ScandEval-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScandEval-6.2.4.tar", max compression
+gzip compressed data, was "ScandEval-6.3.0.tar", max compression
```

## Comparing `ScandEval-6.2.4.tar` & `ScandEval-6.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1077 2023-01-26 21:11:58.574218 ScandEval-6.2.4/LICENSE
--rw-r--r--   0        0        0     6950 2023-01-26 21:11:58.574889 ScandEval-6.2.4/README.md
--rw-r--r--   0        0        0     1747 2023-03-10 15:05:24.723127 ScandEval-6.2.4/pyproject.toml
--rw-r--r--   0        0        0      846 2022-11-05 19:28:53.198522 ScandEval-6.2.4/src/scandeval/__init__.py
--rw-r--r--   0        0        0     8645 2023-03-10 14:44:06.418626 ScandEval-6.2.4/src/scandeval/benchmark_config_factory.py
--rw-r--r--   0        0        0    26263 2023-03-10 14:57:58.339554 ScandEval-6.2.4/src/scandeval/benchmark_dataset.py
--rw-r--r--   0        0        0    17317 2023-03-10 14:45:16.272845 ScandEval-6.2.4/src/scandeval/benchmarker.py
--rw-r--r--   0        0        0     1382 2022-11-03 09:23:55.848473 ScandEval-6.2.4/src/scandeval/callbacks.py
--rw-r--r--   0        0        0     6298 2023-03-10 14:45:13.253631 ScandEval-6.2.4/src/scandeval/cli.py
--rw-r--r--   0        0        0     5805 2023-03-10 14:44:27.154206 ScandEval-6.2.4/src/scandeval/config.py
--rw-r--r--   0        0        0     4962 2022-12-29 15:49:44.942921 ScandEval-6.2.4/src/scandeval/dataset_configs.py
--rw-r--r--   0        0        0     1920 2022-11-03 09:23:55.849427 ScandEval-6.2.4/src/scandeval/dataset_factory.py
--rw-r--r--   0        0        0     3352 2022-12-29 15:49:44.943265 ScandEval-6.2.4/src/scandeval/dataset_tasks.py
--rw-r--r--   0        0        0      650 2022-07-22 11:05:37.491231 ScandEval-6.2.4/src/scandeval/exceptions.py
--rw-r--r--   0        0        0    12351 2023-02-22 12:37:31.608038 ScandEval-6.2.4/src/scandeval/hf_hub.py
--rw-r--r--   0        0        0     7946 2022-07-14 15:19:22.963227 ScandEval-6.2.4/src/scandeval/languages.py
--rw-r--r--   0        0        0    15916 2023-03-10 15:03:15.594793 ScandEval-6.2.4/src/scandeval/model_loading.py
--rw-r--r--   0        0        0    12365 2022-12-24 12:57:14.794100 ScandEval-6.2.4/src/scandeval/named_entity_recognition.py
--rw-r--r--   0        0        0    14150 2023-01-02 15:54:53.052640 ScandEval-6.2.4/src/scandeval/question_answering.py
--rw-r--r--   0        0        0    11733 2022-12-24 12:57:14.794624 ScandEval-6.2.4/src/scandeval/question_answering_trainer.py
--rw-r--r--   0        0        0     4692 2022-12-29 15:49:44.943541 ScandEval-6.2.4/src/scandeval/scores.py
--rw-r--r--   0        0        0     3899 2022-12-24 12:57:14.794885 ScandEval-6.2.4/src/scandeval/sequence_classification.py
--rw-r--r--   0        0        0     5752 2023-01-02 14:37:55.718835 ScandEval-6.2.4/src/scandeval/speed_benchmark.py
--rw-r--r--   0        0        0      163 2022-11-03 09:23:55.851896 ScandEval-6.2.4/src/scandeval/types.py
--rw-r--r--   0        0        0     9020 2023-03-10 14:56:19.791076 ScandEval-6.2.4/src/scandeval/utils.py
--rw-r--r--   0        0        0     8798 1970-01-01 00:00:00.000000 ScandEval-6.2.4/setup.py
--rw-r--r--   0        0        0     8395 1970-01-01 00:00:00.000000 ScandEval-6.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-01-26 21:11:58.574218 ScandEval-6.3.0/LICENSE
+-rw-r--r--   0        0        0     6950 2023-04-12 09:20:57.766641 ScandEval-6.3.0/README.md
+-rw-r--r--   0        0        0     1747 2023-04-12 09:23:21.661468 ScandEval-6.3.0/pyproject.toml
+-rw-r--r--   0        0        0      846 2022-11-05 19:28:53.198522 ScandEval-6.3.0/src/scandeval/__init__.py
+-rw-r--r--   0        0        0     8919 2023-04-12 09:02:17.736254 ScandEval-6.3.0/src/scandeval/benchmark_config_factory.py
+-rw-r--r--   0        0        0    28601 2023-04-12 09:02:17.736539 ScandEval-6.3.0/src/scandeval/benchmark_dataset.py
+-rw-r--r--   0        0        0    17639 2023-04-12 09:02:17.736765 ScandEval-6.3.0/src/scandeval/benchmarker.py
+-rw-r--r--   0        0        0     1382 2022-11-03 09:23:55.848473 ScandEval-6.3.0/src/scandeval/callbacks.py
+-rw-r--r--   0        0        0     6661 2023-04-12 09:02:17.736945 ScandEval-6.3.0/src/scandeval/cli.py
+-rw-r--r--   0        0        0     6035 2023-04-12 09:02:17.737107 ScandEval-6.3.0/src/scandeval/config.py
+-rw-r--r--   0        0        0     4962 2022-12-29 15:49:44.942921 ScandEval-6.3.0/src/scandeval/dataset_configs.py
+-rw-r--r--   0        0        0     1920 2022-11-03 09:23:55.849427 ScandEval-6.3.0/src/scandeval/dataset_factory.py
+-rw-r--r--   0        0        0     3352 2022-12-29 15:49:44.943265 ScandEval-6.3.0/src/scandeval/dataset_tasks.py
+-rw-r--r--   0        0        0      650 2022-07-22 11:05:37.491231 ScandEval-6.3.0/src/scandeval/exceptions.py
+-rw-r--r--   0        0        0    12351 2023-02-22 12:37:31.608038 ScandEval-6.3.0/src/scandeval/hf_hub.py
+-rw-r--r--   0        0        0     7946 2022-07-14 15:19:22.963227 ScandEval-6.3.0/src/scandeval/languages.py
+-rw-r--r--   0        0        0    16510 2023-04-12 09:02:17.737319 ScandEval-6.3.0/src/scandeval/model_loading.py
+-rw-r--r--   0        0        0    15045 2023-03-10 17:33:33.955970 ScandEval-6.3.0/src/scandeval/named_entity_recognition.py
+-rw-r--r--   0        0        0    14150 2023-04-12 09:02:17.737732 ScandEval-6.3.0/src/scandeval/question_answering.py
+-rw-r--r--   0        0        0    11733 2022-12-24 12:57:14.794624 ScandEval-6.3.0/src/scandeval/question_answering_trainer.py
+-rw-r--r--   0        0        0     4692 2022-12-29 15:49:44.943541 ScandEval-6.3.0/src/scandeval/scores.py
+-rw-r--r--   0        0        0     3899 2022-12-24 12:57:14.794885 ScandEval-6.3.0/src/scandeval/sequence_classification.py
+-rw-r--r--   0        0        0     5812 2023-04-12 09:02:17.737892 ScandEval-6.3.0/src/scandeval/speed_benchmark.py
+-rw-r--r--   0        0        0      163 2022-11-03 09:23:55.851896 ScandEval-6.3.0/src/scandeval/types.py
+-rw-r--r--   0        0        0     9020 2023-03-10 14:56:19.791076 ScandEval-6.3.0/src/scandeval/utils.py
+-rw-r--r--   0        0        0     8798 1970-01-01 00:00:00.000000 ScandEval-6.3.0/setup.py
+-rw-r--r--   0        0        0     8395 1970-01-01 00:00:00.000000 ScandEval-6.3.0/PKG-INFO
```

### Comparing `ScandEval-6.2.4/LICENSE` & `ScandEval-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/README.md` & `ScandEval-6.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ### Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.
 
 ______________________________________________________________________
 [![PyPI Status](https://badge.fury.io/py/scandeval.svg)](https://pypi.org/project/scandeval/)
 [![Documentation](https://img.shields.io/badge/docs-passing-green)](https://saattrupdan.github.io/ScandEval/scandeval.html)
 [![License](https://img.shields.io/github/license/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/blob/main/LICENSE)
 [![LastCommit](https://img.shields.io/github/last-commit/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/commits/main)
-[![Code Coverage](https://img.shields.io/badge/Coverage-74%25-yellow.svg)](https://github.com/saattrupdan/ScandEval/tree/main/tests)
+[![Code Coverage](https://img.shields.io/badge/Coverage-73%25-yellow.svg)](https://github.com/saattrupdan/ScandEval/tree/main/tests)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](https://github.com/saattrupdan/ScandEval/blob/main/CODE_OF_CONDUCT.md)
 
 
 ## Installation
 To install the package simply write the following command in your favorite terminal:
 ```
 $ pip install scandeval
```

### Comparing `ScandEval-6.2.4/pyproject.toml` & `ScandEval-6.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ScandEval"
-version = "6.2.4"
+version = "6.3.0"
 description = "Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks."
 authors = ["Dan Saattrup Nielsen <saattrupdan@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://scandeval.github.io"
 repository = "https://github.com/saattrupdan/ScandEval"
```

### Comparing `ScandEval-6.2.4/src/scandeval/__init__.py` & `ScandEval-6.3.0/src/scandeval/__init__.py`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/src/scandeval/benchmark_config_factory.py` & `ScandEval-6.3.0/src/scandeval/benchmark_config_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,25 +16,29 @@
     raise_errors: bool,
     cache_dir: str,
     evaluate_train: bool,
     use_auth_token: Union[bool, str],
     progress_bar: bool,
     save_results: bool,
     verbose: bool,
+    model_framework: Optional[str],
 ) -> BenchmarkConfig:
     """Create a benchmark configuration.
 
     Args:
         language (str or list of str, optional):
             The language codes of the languages to include, both for models and
             datasets. Here 'no' means both Bokmål (nb) and Nynorsk (nn). Set this
             to 'all' if all languages (also non-Scandinavian) should be considered.
         model_language (None, str or sequence of str, optional):
             The language codes of the languages to include for models. If specified
             then this overrides the `language` parameter for model languages.
+        model_framework (str, optional):
+            The model framework to use. Only relevant if `model-id` refers to a local
+            path. Otherwise, the framework will be set automatically.
         dataset_language (None, str or sequence of str, optional):
             The language codes of the languages to include for datasets. If
             specified then this overrides the `language` parameter for dataset
             languages.
         dataset_task (str or sequence of str, optional):
             The tasks to include for dataset. If "all" then datasets will not be
             filtered based on their task.
@@ -86,14 +90,15 @@
         raise_errors=raise_errors,
         cache_dir=cache_dir,
         evaluate_train=evaluate_train,
         use_auth_token=use_auth_token,
         progress_bar=progress_bar,
         save_results=save_results,
         verbose=verbose,
+        model_framework=model_framework,
     )
 
 
 def prepare_languages(language: Union[str, List[str]]) -> Sequence[str]:
     """Prepare language(s) for benchmarking.
 
     Args:
```

### Comparing `ScandEval-6.2.4/src/scandeval/benchmark_dataset.py` & `ScandEval-6.3.0/src/scandeval/benchmark_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Abstract benchmarking dataset class."""
 
 import logging
 import warnings
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from functools import partial
+from pathlib import Path
 from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 import evaluate
 import numpy as np
 import torch
 from datasets.arrow_dataset import Dataset
 from datasets.dataset_dict import DatasetDict
@@ -43,14 +44,73 @@
     handle_error,
 )
 
 # Set up logger
 logger = logging.getLogger(__name__)
 
 
+def get_local_model_config(
+    model_id: str, benchmark_config: BenchmarkConfig
+) -> ModelConfig:
+    """Builds the configuration for a local model.
+
+    Args:
+        model_id (str):
+            The path of the local model.
+        benchmark_config (BenchmarkConfig):
+            The configuration of the benchmark.
+
+    Returns:
+        ModelConfig:
+            The model configuration.
+
+    Raises:
+        RuntimeError:
+            If the --raise-errors option has been set to True and
+            the framework cannot be recognized automatically and
+            it has not explicitly been provided using --model-framework.
+    """
+    framework = benchmark_config.model_framework
+    if framework is None:
+        try:
+            exts = {f.suffix for f in Path(model_id).iterdir()}
+            if ".bin" in exts:
+                framework = "pytorch"
+            elif ".msgpack" in exts:
+                framework = "jax"
+            elif ".whl" in exts:
+                raise InvalidBenchmark("SpaCy models are not supported.")
+            elif ".h5" in exts:
+                raise InvalidBenchmark("TensorFlow/Keras models are not supported.")
+        except OSError as e:
+            logger.info(f"Cannot list files for local model `{model_id}`!")
+            if benchmark_config.raise_errors:
+                raise e
+    if framework is None:
+        if benchmark_config.raise_errors:
+            raise InvalidBenchmark(
+                "Cannot recognize framework automatically for local model "
+                f"`{model_id}`! Please use the --model-framework option."
+            )
+        logger.info(
+            f"Assuming 'pytorch' as the framework for local model `{model_id}`! "
+            "If this is in error, please use the --model-framework option to override."
+        )
+        framework = "pytorch"
+
+    model_config = ModelConfig(
+        model_id=model_id,
+        revision="main",
+        framework=framework,
+        task="fill-mask",
+        languages=list(),
+    )
+    return model_config
+
+
 class BenchmarkDataset(ABC):
     """Abstract benchmarking dataset class.
 
     Args:
         dataset_config (DatasetConfig):
             The configuration of the dataset.
         benchmark_config (BenchmarkConfig):
@@ -109,15 +169,19 @@
                 scores in the second.
 
         Raises:
             RuntimeError:
                 If the extracted framework is not recognized.
         """
         # Fetch the model config
-        model_config = get_model_config(
+        if Path(model_id).is_dir():
+            model_configurator = get_local_model_config
+        else:
+            model_configurator = get_model_config
+        model_config = model_configurator(
             model_id=model_id, benchmark_config=self.benchmark_config
         )
 
         # Set random seeds to enforce reproducibility of the randomly initialised
         # weights
         rng = enforce_reproducibility(framework=model_config.framework)
 
@@ -129,14 +193,15 @@
             language=self.dataset_config.languages[0].code,
             num_labels=self.dataset_config.num_labels,
             id2label=self.dataset_config.id2label,
             label2id=self.dataset_config.label2id,
             from_flax=model_config.framework == "jax",
             use_auth_token=self.benchmark_config.use_auth_token,
             cache_dir=self.benchmark_config.cache_dir,
+            raise_errors=self.benchmark_config.raise_errors,
         )
 
         # Get the metadata
         metadata_dict = self._get_metadata(model=model, tokenizer=tokenizer)
 
         # Set variable with number of iterations
         num_iter = 10 if not self.benchmark_config.testing else 5
@@ -474,14 +539,15 @@
                     language=self.dataset_config.languages[0].code,
                     num_labels=self.dataset_config.num_labels,
                     label2id=self.dataset_config.label2id,
                     id2label=self.dataset_config.id2label,
                     from_flax=model_config.framework == "jax",
                     use_auth_token=self.benchmark_config.use_auth_token,
                     cache_dir=self.benchmark_config.cache_dir,
+                    raise_errors=self.benchmark_config.raise_errors,
                 )
 
             # Initialise compute_metrics function
             compute_metrics = partial(
                 self._compute_metrics, id2label=model.config.id2label
             )
```

### Comparing `ScandEval-6.2.4/src/scandeval/benchmarker.py` & `ScandEval-6.3.0/src/scandeval/benchmarker.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,17 @@
             datasets. Here 'no' means both Bokmål (nb) and Nynorsk (nn). Set this to
             'all' if all languages (also non-Scandinavian) should be considered.
             Defaults to ['da', 'sv', 'no'].
         model_language (None, str or sequence of str, optional):
             The language codes of the languages to include for models. If specified
             then this overrides the `language` parameter for model languages. Defaults
             to None.
+        model_framework (None, str or sequence of str, optional):
+            The model framework to use. Only relevant if `model-id` refers to a local
+            path. Otherwise, the framework will be set automatically. Defaults to None.
         dataset_language (None, str or sequence of str, optional):
             The language codes of the languages to include for datasets. If specified
             then this overrides the `language` parameter for dataset languages.
             Defaults to None.
         dataset_task (str or sequence of str, optional):
             The tasks to include for dataset. If "all" then datasets will not be
             filtered based on their task. Defaults to "all".
@@ -86,14 +89,15 @@
         batch_size: int = 32,
         evaluate_train: bool = False,
         raise_errors: bool = False,
         cache_dir: str = ".scandeval_cache",
         use_auth_token: Union[bool, str] = False,
         ignore_duplicates: bool = True,
         verbose: bool = False,
+        model_framework: str = None,
     ) -> None:
         # Build benchmark configuration
         self.benchmark_config = build_benchmark_config(
             language=language,
             model_language=model_language,
             dataset_language=dataset_language,
             dataset_task=dataset_task,
@@ -101,14 +105,15 @@
             raise_errors=raise_errors,
             cache_dir=cache_dir,
             evaluate_train=evaluate_train,
             use_auth_token=use_auth_token,
             progress_bar=progress_bar,
             save_results=save_results,
             verbose=verbose,
+            model_framework=model_framework,
         )
 
         # Set attributes from arguments
         self.ignore_duplicates = ignore_duplicates
 
         # Initialise variable storing model lists, so we only have to fetch it once
         self._model_lists: Union[Dict[str, Sequence[str]], None] = None
```

### Comparing `ScandEval-6.2.4/src/scandeval/callbacks.py` & `ScandEval-6.3.0/src/scandeval/callbacks.py`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/src/scandeval/cli.py` & `ScandEval-6.3.0/src/scandeval/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,23 @@
     metavar="ISO 639-1 LANGUAGE CODE",
     type=click.Choice(["all"] + list(get_all_languages().keys())),
     help="""The model languages to benchmark. Only relevant if `model-id` has not been
     specified. If "all" then all models will be benchmarked. If not specified then this
     will use the `language` value.""",
 )
 @click.option(
+    "--model-framework",
+    "-mf",
+    default=None,
+    show_default=True,
+    type=click.Choice(["pytorch", "jax"]),
+    help="""The model framework to use. Only relevant if `model-id` refers to a local
+    path. Otherwise, the framework will be set automatically.""",
+)
+@click.option(
     "--dataset-language",
     "-dl",
     default=None,
     show_default=True,
     multiple=True,
     metavar="ISO 639-1 LANGUAGE CODE",
     type=click.Choice(["all"] + list(get_all_languages().keys())),
@@ -160,14 +169,15 @@
     progress_bar: bool,
     save_results: bool,
     cache_dir: str,
     use_auth_token: bool,
     auth_token: str,
     ignore_duplicates: bool,
     verbose: bool = False,
+    model_framework: str = None,
 ) -> None:
     """Benchmark pretrained language models on Scandinavian language tasks."""
 
     # Set up language variables
     model_ids = None if len(model_id) == 0 else list(model_id)
     datasets = None if len(dataset) == 0 else list(dataset)
     languages: List[str] = list(language)
@@ -188,11 +198,12 @@
         save_results=save_results,
         evaluate_train=evaluate_train,
         raise_errors=raise_errors,
         verbose=verbose,
         use_auth_token=auth,
         ignore_duplicates=ignore_duplicates,
         cache_dir=cache_dir,
+        model_framework=model_framework,
     )
 
     # Perform the benchmark evaluation
     benchmarker(model_id=model_ids, dataset=datasets)
```

### Comparing `ScandEval-6.2.4/src/scandeval/config.py` & `ScandEval-6.3.0/src/scandeval/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Configuration classes used throughout the project."""
 
 from dataclasses import dataclass, field
-from typing import Any, Callable, Dict, List, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 
 @dataclass
 class MetricConfig:
     """Configuration for a metric.
 
     Attributes:
@@ -77,14 +77,17 @@
 @dataclass
 class BenchmarkConfig:
     """General benchmarking configuration, across datasets and models.
 
     Attributes:
         model_languages (sequence of Language objects):
             The languages of the models to benchmark.
+        model_framework (str or None, optional):
+            The framework of the models to benchmark. If None then the framework will
+            be inferred. Defaults to None.
         dataset_languages (sequence of Language objects):
             The languages of the datasets in the benchmark.
         dataset_tasks (sequence of DatasetTask):
             The tasks to benchmark.
         batch_size (int):
             The batch size to use.
         raise_errors (bool):
@@ -117,14 +120,15 @@
     cache_dir: str
     evaluate_train: bool
     use_auth_token: Union[bool, str]
     progress_bar: bool
     save_results: bool
     verbose: bool
     testing: bool = False
+    model_framework: Optional[str] = None
 
 
 @dataclass
 class DatasetConfig:
     """Configuration for a dataset.
 
     Attributes:
```

### Comparing `ScandEval-6.2.4/src/scandeval/dataset_configs.py` & `ScandEval-6.3.0/src/scandeval/dataset_configs.py`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/src/scandeval/dataset_factory.py` & `ScandEval-6.3.0/src/scandeval/dataset_factory.py`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/src/scandeval/dataset_tasks.py` & `ScandEval-6.3.0/src/scandeval/dataset_tasks.py`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/src/scandeval/exceptions.py` & `ScandEval-6.3.0/src/scandeval/exceptions.py`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/src/scandeval/hf_hub.py` & `ScandEval-6.3.0/src/scandeval/hf_hub.py`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/src/scandeval/languages.py` & `ScandEval-6.3.0/src/scandeval/languages.py`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/src/scandeval/model_loading.py` & `ScandEval-6.3.0/src/scandeval/model_loading.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     language: str,
     num_labels: int,
     id2label: List[str],
     label2id: Dict[str, int],
     from_flax: bool,
     use_auth_token: Union[bool, str],
     cache_dir: str,
+    raise_errors: bool = False,
 ) -> Tuple[PreTrainedTokenizer, PreTrainedModel]:
     """Load a model.
 
     Args:
         model_id (str):
             The Hugging Face ID of the model.
         revision (str):
@@ -61,14 +62,16 @@
         use_auth_token (bool or str):
             Whether to use an authentication token to access the model. If a boolean
             value is specified then it is assumed that the user is logged in to the
             Hugging Face CLI, and if a string is specified then it is used as the
             token.
         cache_dir (str):
             The directory to cache the model in.
+        raise_errors (bool, optional):
+            Whether to raise errors instead of trying to fix them silently.
 
     Returns:
         pair of (tokenizer, model):
             The tokenizer and model.
 
     Raises:
         RuntimeError:
@@ -120,16 +123,17 @@
                     class_name=f"auto-model-for-{supertask}",
                     module_name="transformers",
                 )
 
                 # If the model class could not be found then raise an error
                 if not model_cls_or_none:
                     raise InvalidBenchmark(
-                        f"The supertask '{supertask}' does not correspond to a Hugging Face"
-                        " AutoModel type (such as `AutoModelForSequenceClassification`)."
+                        f"The supertask '{supertask}' does not correspond to a "
+                        "Hugging Face AutoModel type (such as "
+                        "`AutoModelForSequenceClassification`)."
                     )
 
                 # If the model is a DeBERTaV2 model then we ensure that
                 # `pooler_hidden_size` is the same size as `hidden_size`
                 if config.model_type == "deberta-v2":
                     config.pooler_hidden_size = config.hidden_size
 
@@ -211,15 +215,17 @@
                 use_fast=True,
                 verbose=False,
             )
         except (JSONDecodeError, OSError):
             raise InvalidBenchmark(f"Could not load tokenizer for model {model_id!r}.")
 
     # Align the model and the tokenizer
-    model, tokenizer = align_model_and_tokenizer(model=model, tokenizer=tokenizer)
+    model, tokenizer = align_model_and_tokenizer(
+        model=model, tokenizer=tokenizer, raise_errors=raise_errors
+    )
 
     return tokenizer, model
 
 
 def load_fresh_model_class(
     model_id: str, supertask: str
 ) -> Tuple[Type[PreTrainedModel], str]:
@@ -347,23 +353,25 @@
     # Set the model config to use the new type vocab size
     model.config.type_vocab_size = 2
 
     return model
 
 
 def align_model_and_tokenizer(
-    model: PreTrainedModel, tokenizer: PreTrainedTokenizer
+    model: PreTrainedModel, tokenizer: PreTrainedTokenizer, raise_errors: bool = False
 ) -> Tuple[PreTrainedModel, PreTrainedTokenizer]:
     """Aligns the model and the tokenizer.
 
     Args:
         model (PreTrainedModel):
             The model to fix.
         tokenizer (PreTrainedTokenizer):
             The tokenizer to fix.
+        raise_errors (bool, optional):
+            Whether to raise errors instead of trying to fix them silently.
 
     Returns:
         pair of (model, tokenizer):
             The fixed model and tokenizer.
     """
     # Get all possible maximal lengths
     all_max_lengths: List[int] = []
@@ -401,18 +409,21 @@
     else:
         tokenizer.model_max_length = 512
 
     # If there is a mismatch between the vocab size according to the tokenizer and
     # the vocab size according to the model, we raise an error
     if hasattr(model.config, "vocab_size") and hasattr(tokenizer, "vocab_size"):
         if model.config.vocab_size < tokenizer.vocab_size:
-            raise InvalidBenchmark(
-                "The vocab size of the tokenizer is larger than the vocab size of the "
-                "model. This is not supported."
-            )
+            if raise_errors:
+                raise InvalidBenchmark(
+                    "The vocab size of the tokenizer is larger than the vocab size of "
+                    "the model. As the --raise-errors option was specified, the "
+                    "embeddings of the model will not be automatically adjusted."
+                )
+            model.resize_token_embeddings(new_num_tokens=tokenizer.vocab_size + 1)
 
     # If the tokenizer does not have a padding token (e.g. GPT-2), we use find a
     # suitable padding token and set it
     if tokenizer.pad_token is None:
         if tokenizer.eos_token is not None:
             tokenizer.padding_side = "left"
             tokenizer.pad_token = tokenizer.eos_token
```

### Comparing `ScandEval-6.2.4/src/scandeval/named_entity_recognition.py` & `ScandEval-6.3.0/src/scandeval/named_entity_recognition.py`

 * *Files 12% similar despite different names*

```diff
@@ -173,23 +173,21 @@
         # Extract a mapping between all the tokens and their corresponding word. If the
         # tokenizer is of a "fast" variant then this can be accessed through the
         # `word_ids` method. Otherwise, we have to extract it manually.
         all_labels: List[List[int]] = list()
         labels: List[str]
         word_ids: List[Optional[int]]
         for i, labels in enumerate(examples["ner_tags"]):
-
             # Try to get the word IDs from the tokenizer
             try:
                 word_ids = tokenized_inputs.word_ids(batch_index=i)
 
             # If the tokenizer is not of a "fast" variant, we have to extract the word
             # IDs manually
             except ValueError:
-
                 # Get the list of words in the document
                 words: List[str] = examples["tokens"][i]
 
                 # Get the list of token IDs in the document
                 tok_ids: List[int] = tokenized_inputs.input_ids[i]
 
                 # Decode the token IDs
@@ -198,15 +196,21 @@
                 # Remove prefixes from the tokens
                 prefixes_to_remove = ["▁", "##"]
                 for tok_idx, tok in enumerate(tokens):
                     if tok:
                         for prefix in prefixes_to_remove:
                             if tok.startswith(prefix):
                                 tokens[tok_idx] = tok[len(prefix) :]
-                    tokens[tok_idx] = tok
+
+                # Replace UNK tokens with the correct word
+                tokens = self._handle_unk_tokens(
+                    tokenizer=tokenizer,
+                    tokens=tokens,
+                    words=words,
+                )
 
                 # Get list of special tokens. Some tokenizers do not record these
                 # properly, which is why we convert the values to their indices and
                 # then back to strings
                 sp_toks = [
                     tokenizer.convert_ids_to_tokens(
                         tokenizer.convert_tokens_to_ids(sp_tok)
@@ -251,15 +255,14 @@
                             if token_idx == tok_idx
                         ][0]
                         word_ids.append(word_idx)
 
             previous_word_idx: Optional[int] = None
             label_ids: List[int] = list()
             for word_id in word_ids:
-
                 # Special tokens have a word id that is None. We set the label to -100
                 # so they are automatically ignored in the loss function
                 if word_id is None:
                     label_ids.append(-100)
 
                 # We set the label for the first token of each word
                 elif word_id != previous_word_idx:
@@ -277,14 +280,75 @@
 
                 previous_word_idx = word_id
 
             all_labels.append(label_ids)
         tokenized_inputs["labels"] = all_labels
         return tokenized_inputs
 
+    def _handle_unk_tokens(
+        self, tokenizer: PreTrainedTokenizer, tokens: List[str], words: List[str]
+    ) -> List[str]:
+        """Replace unknown tokens in the tokens with the corresponding word.
+
+        Args:
+            tokenizer (PreTrainedTokenizer):
+                The tokenizer used to tokenize the words.
+            tokens (list of str):
+                The list of tokens.
+            words (list of str):
+                The list of words.
+
+        Returns:
+            list of str:
+                The list of tokens with unknown tokens replaced by the corresponding
+                word.
+        """
+        # Locate the token indices of the unknown tokens
+        token_unk_idxs = [
+            i for i, tok in enumerate(tokens) if tok == tokenizer.unk_token
+        ]
+
+        # Locate the word indices of the words which contain an unknown token
+        word_unk_idxs = [
+            i
+            for i, word in enumerate(words)
+            if tokenizer.unk_token
+            in tokenizer.convert_ids_to_tokens(
+                tokenizer.encode(word, add_special_tokens=False)
+            )
+        ]
+
+        # Iterate over the token index and word index pairs
+        for tok_idx, word_idx in zip(token_unk_idxs, word_unk_idxs):
+            # Fetch the word
+            word = words[word_idx]
+
+            # Tokenize the word, which is now a list containing at least one UNK token
+            tokens_with_unk = tokenizer.convert_ids_to_tokens(
+                tokenizer.encode(word, add_special_tokens=False)
+            )
+
+            # Iterate over the tokens in the word
+            for possible_unk_token in tokens_with_unk:
+                # If the token is not an UNK token then we remove the first occurence
+                # of the content of this token from the word. The result of the `word`
+                # variable will be the content of the UNK token.
+                # NOTE: This is a bit hacky and not bulletproof. For instance, if the
+                # word is "1925-1950" and the tokenizer splits it into ["[UNK]", "-",
+                # "19", "50"], then the result will be 2519 instead of 1925. This
+                # happens almost never, however, so we can live with it.
+                if possible_unk_token != tokenizer.unk_token:
+                    word = word.replace(possible_unk_token, "", 1)
+
+            # Replace the token with the word
+            tokens[tok_idx] = word
+
+        # Return the tokens
+        return tokens
+
     def _preprocess_data(self, dataset: Dataset, **kwargs) -> Dataset:
         """Preprocess a dataset by tokenizing and aligning the labels.
 
         Args:
             dataset (Hugging Face dataset):
                 The dataset to preprocess.
             kwargs:
```

### Comparing `ScandEval-6.2.4/src/scandeval/question_answering.py` & `ScandEval-6.3.0/src/scandeval/question_answering.py`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/src/scandeval/question_answering_trainer.py` & `ScandEval-6.3.0/src/scandeval/question_answering_trainer.py`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/src/scandeval/scores.py` & `ScandEval-6.3.0/src/scandeval/scores.py`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/src/scandeval/sequence_classification.py` & `ScandEval-6.3.0/src/scandeval/sequence_classification.py`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/src/scandeval/speed_benchmark.py` & `ScandEval-6.3.0/src/scandeval/speed_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
                 language=dataset_config.languages[0].code,
                 num_labels=dataset_config.num_labels,
                 label2id=dataset_config.label2id,
                 id2label=dataset_config.id2label,
                 from_flax=model_config.framework == "jax",
                 use_auth_token=benchmark_config.use_auth_token,
                 cache_dir=benchmark_config.cache_dir,
+                raise_errors=benchmark_config.raise_errors,
             )
 
         # Ensure that the model is on the CPU
         model.cpu()
 
         # Create a dummy document
         doc = "This is a dummy document. " * 100
```

### Comparing `ScandEval-6.2.4/src/scandeval/utils.py` & `ScandEval-6.3.0/src/scandeval/utils.py`

 * *Files identical despite different names*

### Comparing `ScandEval-6.2.4/setup.py` & `ScandEval-6.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
  'transformers>=4.20.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['scandeval = scandeval.cli:benchmark']}
 
 setup_kwargs = {
     'name': 'scandeval',
-    'version': '6.2.4',
+    'version': '6.3.0',
     'description': 'Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.',
-    'long_description': '<div align=\'center\'>\n<img src="https://raw.githubusercontent.com/saattrupdan/ScandEval/main/gfx/scandeval.png" width="517" height="217">\n</div>\n\n### Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.\n\n______________________________________________________________________\n[![PyPI Status](https://badge.fury.io/py/scandeval.svg)](https://pypi.org/project/scandeval/)\n[![Documentation](https://img.shields.io/badge/docs-passing-green)](https://saattrupdan.github.io/ScandEval/scandeval.html)\n[![License](https://img.shields.io/github/license/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/blob/main/LICENSE)\n[![LastCommit](https://img.shields.io/github/last-commit/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/commits/main)\n[![Code Coverage](https://img.shields.io/badge/Coverage-74%25-yellow.svg)](https://github.com/saattrupdan/ScandEval/tree/main/tests)\n[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](https://github.com/saattrupdan/ScandEval/blob/main/CODE_OF_CONDUCT.md)\n\n\n## Installation\nTo install the package simply write the following command in your favorite terminal:\n```\n$ pip install scandeval\n```\n\n## Quickstart\n### Benchmarking from the Command Line\nThe easiest way to benchmark pretrained models is via the command line interface. After\nhaving installed the package, you can benchmark your favorite model like so:\n```\n$ scandeval --model-id <model-id>\n```\n\nHere `model_id` is the HuggingFace model ID, which can be found on the [HuggingFace\nHub](https://huggingface.co/models). By default this will benchmark the model on all\nthe datasets eligible. If you want to benchmark on a specific dataset, this can be done\nvia the `--dataset` flag. This will for instance evaluate the model on the\n`AngryTweets` dataset:\n```\n$ scandeval --model-id <model-id> --dataset angry-tweets\n```\n\nWe can also separate by language. To benchmark all Danish models on all Danish\ndatasets, say, this can be done using the `language` tag, like so:\n```\n$ scandeval --language da\n```\n\nMultiple models, datasets and/or languages can be specified by just attaching multiple\narguments. Here is an example with two models:\n```\n$ scandeval --model-id <model-id1> --model-id <model-id2> --dataset angry-tweets\n```\n\nThe specific model version to use can also be added after the suffix \'@\':\n```\n$ scandeval --model-id <model-id>@<commit>\n```\n\nIt can be a branch name, a tag name, or a commit id. It defaults to \'main\' for latest.\n\nSee all the arguments and options available for the `scandeval` command by typing\n```\n$ scandeval --help\n```\n\n### Benchmarking from a Script\nIn a script, the syntax is similar to the command line interface. You simply initialise\nan object of the `Benchmarker` class, and call this benchmark object with your favorite\nmodels and/or datasets:\n```\n>>> from scandeval import Benchmarker\n>>> benchmark = Benchmarker()\n>>> benchmark(\'<model-id>\')\n```\n\nTo benchmark on a specific dataset, you simply specify the second argument, shown here\nwith the `AngryTweets` dataset again:\n```\n>>> benchmark(\'<model_id>\', \'angry-tweets\')\n```\n\nIf you want to benchmark a subset of all the models on the Hugging Face Hub, you can\nspecify several parameters in the `Benchmarker` initializer to narrow down the list of\nmodels to the ones you care about. As a simple example, the following would benchmark\nall the Nynorsk models on Nynorsk datasets:\n```\n>>> benchmark = Benchmarker(language=\'nn\')\n>>> benchmark()\n```\n\n\n## Documentation\n\nSee the full documentation [here](https://saattrupdan.github.io/ScandEval/scandeval.html).\n\n\n## Citing ScandEval\nIf you want to cite the framework then feel free to use this:\n```\n@article{nielsen2022scandeval,\n  title={ScandEval: Evaluation of language models on mono- or multilingual Scandinavian language tasks.},\n  author={Nielsen, Dan Saattrup},\n  journal={GitHub. Note: https://github.com/saattrupdan/ScandEval},\n  year={2022}\n}\n```\n\n## Remarks\nThe image used in the logo has been created by the amazing [Scandinavia and the\nWorld](https://satwcomic.com/) team. Go check them out!\n\n\n## Project structure\n```\n.\n├── .flake8\n├── .github\n│\xa0\xa0 └── workflows\n│\xa0\xa0     ├── ci.yaml\n│\xa0\xa0     └── docs.yaml\n├── .gitignore\n├── .pre-commit-config.yaml\n├── CHANGELOG.md\n├── LICENSE\n├── README.md\n├── gfx\n│\xa0\xa0 └── scandeval.png\n├── makefile\n├── notebooks\n├── poetry.toml\n├── pyproject.toml\n├── src\n│\xa0\xa0 ├── scandeval\n│\xa0\xa0 │\xa0\xa0 ├── __init__.py\n│\xa0\xa0 │\xa0\xa0 ├── benchmark_config_factory.py\n│\xa0\xa0 │\xa0\xa0 ├── benchmark_dataset.py\n│\xa0\xa0 │\xa0\xa0 ├── benchmarker.py\n│\xa0\xa0 │\xa0\xa0 ├── callbacks.py\n│\xa0\xa0 │\xa0\xa0 ├── cli.py\n│\xa0\xa0 │\xa0\xa0 ├── config.py\n│\xa0\xa0 │\xa0\xa0 ├── dataset_configs.py\n│\xa0\xa0 │\xa0\xa0 ├── dataset_factory.py\n│\xa0\xa0 │\xa0\xa0 ├── dataset_tasks.py\n│\xa0\xa0 │\xa0\xa0 ├── exceptions.py\n│\xa0\xa0 │\xa0\xa0 ├── hf_hub.py\n│\xa0\xa0 │\xa0\xa0 ├── languages.py\n│\xa0\xa0 │\xa0\xa0 ├── model_loading.py\n│\xa0\xa0 │\xa0\xa0 ├── named_entity_recognition.py\n│\xa0\xa0 │\xa0\xa0 ├── question_answering.py\n│\xa0\xa0 │\xa0\xa0 ├── question_answering_trainer.py\n│\xa0\xa0 │\xa0\xa0 ├── scores.py\n│\xa0\xa0 │\xa0\xa0 ├── sequence_classification.py\n│\xa0\xa0 │\xa0\xa0 ├── speed_benchmark.py\n│\xa0\xa0 │\xa0\xa0 ├── types.py\n│\xa0\xa0 │\xa0\xa0 └── utils.py\n│\xa0\xa0 └── scripts\n│\xa0\xa0     ├── create_angry_tweets.py\n│\xa0\xa0     ├── create_dane.py\n│\xa0\xa0     ├── create_mim_gold_ner.py\n│\xa0\xa0     ├── create_norec.py\n│\xa0\xa0     ├── create_norne.py\n│\xa0\xa0     ├── create_scala.py\n│\xa0\xa0     ├── create_scandiqa.py\n│\xa0\xa0     ├── create_suc3.py\n│\xa0\xa0     ├── create_swerec.py\n│\xa0\xa0     ├── create_wikiann_fo.py\n│\xa0\xa0     ├── fill_in_missing_model_metadata.py\n│\xa0\xa0     ├── fix_dot_env_file.py\n│\xa0\xa0     ├── load_ud_pos.py\n│\xa0\xa0     └── versioning.py\n└── tests\n    ├── __init__.py\n    ├── conftest.py\n    ├── test_benchmark_config_factory.py\n    ├── test_benchmark_dataset.py\n    ├── test_benchmarker.py\n    ├── test_callbacks.py\n    ├── test_cli.py\n    ├── test_config.py\n    ├── test_dataset_configs.py\n    ├── test_dataset_factory.py\n    ├── test_dataset_tasks.py\n    ├── test_exceptions.py\n    ├── test_hf_hub.py\n    ├── test_languages.py\n    ├── test_model_loading.py\n    ├── test_named_entity_recognition.py\n    ├── test_question_answering.py\n    ├── test_question_answering_trainer.py\n    ├── test_scores.py\n    ├── test_sequence_classification.py\n    ├── test_speed_benchmark.py\n    ├── test_types.py\n    └── test_utils.py\n```\n',
+    'long_description': '<div align=\'center\'>\n<img src="https://raw.githubusercontent.com/saattrupdan/ScandEval/main/gfx/scandeval.png" width="517" height="217">\n</div>\n\n### Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.\n\n______________________________________________________________________\n[![PyPI Status](https://badge.fury.io/py/scandeval.svg)](https://pypi.org/project/scandeval/)\n[![Documentation](https://img.shields.io/badge/docs-passing-green)](https://saattrupdan.github.io/ScandEval/scandeval.html)\n[![License](https://img.shields.io/github/license/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/blob/main/LICENSE)\n[![LastCommit](https://img.shields.io/github/last-commit/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/commits/main)\n[![Code Coverage](https://img.shields.io/badge/Coverage-73%25-yellow.svg)](https://github.com/saattrupdan/ScandEval/tree/main/tests)\n[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](https://github.com/saattrupdan/ScandEval/blob/main/CODE_OF_CONDUCT.md)\n\n\n## Installation\nTo install the package simply write the following command in your favorite terminal:\n```\n$ pip install scandeval\n```\n\n## Quickstart\n### Benchmarking from the Command Line\nThe easiest way to benchmark pretrained models is via the command line interface. After\nhaving installed the package, you can benchmark your favorite model like so:\n```\n$ scandeval --model-id <model-id>\n```\n\nHere `model_id` is the HuggingFace model ID, which can be found on the [HuggingFace\nHub](https://huggingface.co/models). By default this will benchmark the model on all\nthe datasets eligible. If you want to benchmark on a specific dataset, this can be done\nvia the `--dataset` flag. This will for instance evaluate the model on the\n`AngryTweets` dataset:\n```\n$ scandeval --model-id <model-id> --dataset angry-tweets\n```\n\nWe can also separate by language. To benchmark all Danish models on all Danish\ndatasets, say, this can be done using the `language` tag, like so:\n```\n$ scandeval --language da\n```\n\nMultiple models, datasets and/or languages can be specified by just attaching multiple\narguments. Here is an example with two models:\n```\n$ scandeval --model-id <model-id1> --model-id <model-id2> --dataset angry-tweets\n```\n\nThe specific model version to use can also be added after the suffix \'@\':\n```\n$ scandeval --model-id <model-id>@<commit>\n```\n\nIt can be a branch name, a tag name, or a commit id. It defaults to \'main\' for latest.\n\nSee all the arguments and options available for the `scandeval` command by typing\n```\n$ scandeval --help\n```\n\n### Benchmarking from a Script\nIn a script, the syntax is similar to the command line interface. You simply initialise\nan object of the `Benchmarker` class, and call this benchmark object with your favorite\nmodels and/or datasets:\n```\n>>> from scandeval import Benchmarker\n>>> benchmark = Benchmarker()\n>>> benchmark(\'<model-id>\')\n```\n\nTo benchmark on a specific dataset, you simply specify the second argument, shown here\nwith the `AngryTweets` dataset again:\n```\n>>> benchmark(\'<model_id>\', \'angry-tweets\')\n```\n\nIf you want to benchmark a subset of all the models on the Hugging Face Hub, you can\nspecify several parameters in the `Benchmarker` initializer to narrow down the list of\nmodels to the ones you care about. As a simple example, the following would benchmark\nall the Nynorsk models on Nynorsk datasets:\n```\n>>> benchmark = Benchmarker(language=\'nn\')\n>>> benchmark()\n```\n\n\n## Documentation\n\nSee the full documentation [here](https://saattrupdan.github.io/ScandEval/scandeval.html).\n\n\n## Citing ScandEval\nIf you want to cite the framework then feel free to use this:\n```\n@article{nielsen2022scandeval,\n  title={ScandEval: Evaluation of language models on mono- or multilingual Scandinavian language tasks.},\n  author={Nielsen, Dan Saattrup},\n  journal={GitHub. Note: https://github.com/saattrupdan/ScandEval},\n  year={2022}\n}\n```\n\n## Remarks\nThe image used in the logo has been created by the amazing [Scandinavia and the\nWorld](https://satwcomic.com/) team. Go check them out!\n\n\n## Project structure\n```\n.\n├── .flake8\n├── .github\n│\xa0\xa0 └── workflows\n│\xa0\xa0     ├── ci.yaml\n│\xa0\xa0     └── docs.yaml\n├── .gitignore\n├── .pre-commit-config.yaml\n├── CHANGELOG.md\n├── LICENSE\n├── README.md\n├── gfx\n│\xa0\xa0 └── scandeval.png\n├── makefile\n├── notebooks\n├── poetry.toml\n├── pyproject.toml\n├── src\n│\xa0\xa0 ├── scandeval\n│\xa0\xa0 │\xa0\xa0 ├── __init__.py\n│\xa0\xa0 │\xa0\xa0 ├── benchmark_config_factory.py\n│\xa0\xa0 │\xa0\xa0 ├── benchmark_dataset.py\n│\xa0\xa0 │\xa0\xa0 ├── benchmarker.py\n│\xa0\xa0 │\xa0\xa0 ├── callbacks.py\n│\xa0\xa0 │\xa0\xa0 ├── cli.py\n│\xa0\xa0 │\xa0\xa0 ├── config.py\n│\xa0\xa0 │\xa0\xa0 ├── dataset_configs.py\n│\xa0\xa0 │\xa0\xa0 ├── dataset_factory.py\n│\xa0\xa0 │\xa0\xa0 ├── dataset_tasks.py\n│\xa0\xa0 │\xa0\xa0 ├── exceptions.py\n│\xa0\xa0 │\xa0\xa0 ├── hf_hub.py\n│\xa0\xa0 │\xa0\xa0 ├── languages.py\n│\xa0\xa0 │\xa0\xa0 ├── model_loading.py\n│\xa0\xa0 │\xa0\xa0 ├── named_entity_recognition.py\n│\xa0\xa0 │\xa0\xa0 ├── question_answering.py\n│\xa0\xa0 │\xa0\xa0 ├── question_answering_trainer.py\n│\xa0\xa0 │\xa0\xa0 ├── scores.py\n│\xa0\xa0 │\xa0\xa0 ├── sequence_classification.py\n│\xa0\xa0 │\xa0\xa0 ├── speed_benchmark.py\n│\xa0\xa0 │\xa0\xa0 ├── types.py\n│\xa0\xa0 │\xa0\xa0 └── utils.py\n│\xa0\xa0 └── scripts\n│\xa0\xa0     ├── create_angry_tweets.py\n│\xa0\xa0     ├── create_dane.py\n│\xa0\xa0     ├── create_mim_gold_ner.py\n│\xa0\xa0     ├── create_norec.py\n│\xa0\xa0     ├── create_norne.py\n│\xa0\xa0     ├── create_scala.py\n│\xa0\xa0     ├── create_scandiqa.py\n│\xa0\xa0     ├── create_suc3.py\n│\xa0\xa0     ├── create_swerec.py\n│\xa0\xa0     ├── create_wikiann_fo.py\n│\xa0\xa0     ├── fill_in_missing_model_metadata.py\n│\xa0\xa0     ├── fix_dot_env_file.py\n│\xa0\xa0     ├── load_ud_pos.py\n│\xa0\xa0     └── versioning.py\n└── tests\n    ├── __init__.py\n    ├── conftest.py\n    ├── test_benchmark_config_factory.py\n    ├── test_benchmark_dataset.py\n    ├── test_benchmarker.py\n    ├── test_callbacks.py\n    ├── test_cli.py\n    ├── test_config.py\n    ├── test_dataset_configs.py\n    ├── test_dataset_factory.py\n    ├── test_dataset_tasks.py\n    ├── test_exceptions.py\n    ├── test_hf_hub.py\n    ├── test_languages.py\n    ├── test_model_loading.py\n    ├── test_named_entity_recognition.py\n    ├── test_question_answering.py\n    ├── test_question_answering_trainer.py\n    ├── test_scores.py\n    ├── test_sequence_classification.py\n    ├── test_speed_benchmark.py\n    ├── test_types.py\n    └── test_utils.py\n```\n',
     'author': 'Dan Saattrup Nielsen',
     'author_email': 'saattrupdan@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://scandeval.github.io',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `ScandEval-6.2.4/PKG-INFO` & `ScandEval-6.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scandeval
-Version: 6.2.4
+Version: 6.3.0
 Summary: Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.
 Home-page: https://scandeval.github.io
 License: MIT
 Author: Dan Saattrup Nielsen
 Author-email: saattrupdan@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -41,15 +41,15 @@
 ### Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.
 
 ______________________________________________________________________
 [![PyPI Status](https://badge.fury.io/py/scandeval.svg)](https://pypi.org/project/scandeval/)
 [![Documentation](https://img.shields.io/badge/docs-passing-green)](https://saattrupdan.github.io/ScandEval/scandeval.html)
 [![License](https://img.shields.io/github/license/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/blob/main/LICENSE)
 [![LastCommit](https://img.shields.io/github/last-commit/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/commits/main)
-[![Code Coverage](https://img.shields.io/badge/Coverage-74%25-yellow.svg)](https://github.com/saattrupdan/ScandEval/tree/main/tests)
+[![Code Coverage](https://img.shields.io/badge/Coverage-73%25-yellow.svg)](https://github.com/saattrupdan/ScandEval/tree/main/tests)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](https://github.com/saattrupdan/ScandEval/blob/main/CODE_OF_CONDUCT.md)
 
 
 ## Installation
 To install the package simply write the following command in your favorite terminal:
 ```
 $ pip install scandeval
```

