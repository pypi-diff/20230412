# Comparing `tmp/ceruleo-2.0.3.tar.gz` & `tmp/ceruleo-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ceruleo-2.0.3.tar", last modified: Mon Sep  5 12:33:33 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ceruleo-2.0.3.tar` & `ceruleo-2.0.4.tar`

### file list

```diff
@@ -1,208 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.918427 ceruleo-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-05 12:33:22.000000 ceruleo-2.0.3/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-09-05 12:33:22.000000 ceruleo-2.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.886425 ceruleo-2.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.890426 ceruleo-2.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-09-05 12:33:22.000000 ceruleo-2.0.3/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-09-05 12:33:22.000000 ceruleo-2.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-09-05 12:33:22.000000 ceruleo-2.0.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-09-05 12:33:22.000000 ceruleo-2.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2955 2022-09-05 12:33:22.000000 ceruleo-2.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-09-05 12:33:22.000000 ceruleo-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-09-05 12:33:33.918427 ceruleo-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-09-05 12:33:22.000000 ceruleo-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-09-05 12:33:22.000000 ceruleo-2.0.3/RELEASING.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.894426 ceruleo-2.0.3/ceruleo/
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.894426 ceruleo-2.0.3/ceruleo/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.894426 ceruleo-2.0.3/ceruleo/dataset/analysis/
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/dataset/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/dataset/analysis/correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4145 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/dataset/analysis/distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     6126 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/dataset/analysis/numerical_features.py
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/dataset/analysis/sample_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.894426 ceruleo-2.0.3/ceruleo/dataset/catalog/
--rw-r--r--   0 runner    (1001) docker     (121)     6126 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/dataset/catalog/CMAPSS.py
--rw-r--r--   0 runner    (1001) docker     (121)     5887 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/dataset/catalog/CMAPSS2.py
--rw-r--r--   0 runner    (1001) docker     (121)     7760 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/dataset/catalog/PHMDataset2018.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/dataset/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3955 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/dataset/transformed.py
--rw-r--r--   0 runner    (1001) docker     (121)     8989 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/dataset/ts_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.898426 ceruleo-2.0.3/ceruleo/graphics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/graphics/analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/graphics/control_charts.py
--rw-r--r--   0 runner    (1001) docker     (121)     8791 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/graphics/duration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3237 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/graphics/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (121)    20799 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/graphics/results.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.898426 ceruleo-2.0.3/ceruleo/graphics/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/graphics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/graphics/utils/annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)    12718 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/graphics/utils/curly_brace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.898426 ceruleo-2.0.3/ceruleo/iterators/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/iterators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7460 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/iterators/batcher.py
--rw-r--r--   0 runner    (1001) docker     (121)    12822 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/iterators/iterators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/iterators/sample_weight.py
--rw-r--r--   0 runner    (1001) docker     (121)    15427 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/iterators/shufflers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/iterators/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.898426 ceruleo-2.0.3/ceruleo/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2746 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/baseline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.898426 ceruleo-2.0.3/ceruleo/models/inspection/
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/inspection/feature_importance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.902426 ceruleo-2.0.3/ceruleo/models/keras/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/activations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2567 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/attention.py
--rw-r--r--   0 runner    (1001) docker     (121)     2281 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.902426 ceruleo-2.0.3/ceruleo/models/keras/catalog/
--rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/catalog/CNLSTM.py
--rw-r--r--   0 runner    (1001) docker     (121)     3677 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/catalog/InceptionTime.py
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/catalog/MSWRLRCN.py
--rw-r--r--   0 runner    (1001) docker     (121)     2050 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/catalog/MVCNN.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/catalog/MultiScaleConvolutional.py
--rw-r--r--   0 runner    (1001) docker     (121)     3822 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/catalog/MultiTaskRUL.py
--rw-r--r--   0 runner    (1001) docker     (121)     3862 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/catalog/XCM.py
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/catalog/XiangQiangJianQiao.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     7286 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/extras.py
--rw-r--r--   0 runner    (1001) docker     (121)     6600 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4984 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/losses.py
--rw-r--r--   0 runner    (1001) docker     (121)     4618 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/keras/weibull.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (121)     5713 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     8792 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.902426 ceruleo-2.0.3/ceruleo/models/torch/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15678 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/torch/dsanet.py
--rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/models/torch/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.902426 ceruleo-2.0.3/ceruleo/results/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4679 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/results/picewise_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)    22989 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/results/results.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.902426 ceruleo-2.0.3/ceruleo/transformation/
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21467 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/augmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.906426 ceruleo-2.0.3/ceruleo/transformation/features/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/cast.py
--rw-r--r--   0 runner    (1001) docker     (121)     6703 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/denoising.py
--rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/entropy.py
--rw-r--r--   0 runner    (1001) docker     (121)    33300 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/extraction.py
--rw-r--r--   0 runner    (1001) docker     (121)     4151 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/extraction_frequency.py
--rw-r--r--   0 runner    (1001) docker     (121)     9101 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/hurst.py
--rw-r--r--   0 runner    (1001) docker     (121)     9898 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/imputers.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/operations.py
--rw-r--r--   0 runner    (1001) docker     (121)    10745 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/outliers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4216 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/resamplers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/rolling_windows.py
--rw-r--r--   0 runner    (1001) docker     (121)    12451 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/scalers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8107 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/slicing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3500 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/split.py
--rw-r--r--   0 runner    (1001) docker     (121)    10869 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/tdigest.py
--rw-r--r--   0 runner    (1001) docker     (121)    10802 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/features/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.906426 ceruleo-2.0.3/ceruleo/transformation/functional/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/functional/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/functional/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3553 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/functional/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/functional/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.906426 ceruleo-2.0.3/ceruleo/transformation/functional/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/functional/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2235 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/functional/pipeline/cache_store.py
--rw-r--r--   0 runner    (1001) docker     (121)     4076 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/functional/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     5015 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/functional/pipeline/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/functional/pipeline/traversal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/functional/pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8446 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/functional/transformers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/functional/transformerstep.py
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/target.py
--rw-r--r--   0 runner    (1001) docker     (121)     5909 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/transformation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.910426 ceruleo-2.0.3/ceruleo/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-09-05 12:33:22.000000 ceruleo-2.0.3/ceruleo/utils/lrucache.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.894426 ceruleo-2.0.3/ceruleo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-09-05 12:33:33.000000 ceruleo-2.0.3/ceruleo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5723 2022-09-05 12:33:33.000000 ceruleo-2.0.3/ceruleo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 12:33:33.000000 ceruleo-2.0.3/ceruleo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-09-05 12:33:33.000000 ceruleo-2.0.3/ceruleo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-05 12:33:33.000000 ceruleo-2.0.3/ceruleo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.910426 ceruleo-2.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.910426 ceruleo-2.0.3/docs/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)   185022 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/dataset/Example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.910426 ceruleo-2.0.3/docs/dataset/analysis/
--rw-r--r--   0 runner    (1001) docker     (121)   478504 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/dataset/analysis/Sensor Validation.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/dataset/analysis/correlation.md
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/dataset/analysis/distribution.md
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/dataset/analysis/sample_rate.md
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/dataset/analysis/sensor_validation.md
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/dataset/catalog.md
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/dataset/dataset.md
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/dataset/visualization.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.910426 ceruleo-2.0.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (121)    17517 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/images/cerulean.png
--rw-r--r--   0 runner    (1001) docker     (121)    67664 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/images/unipd_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.910426 ceruleo-2.0.3/docs/img/
--rw-r--r--   0 runner    (1001) docker     (121)    50083 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/img/duration_histogram.png
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.914426 ceruleo-2.0.3/docs/iterators/
--rw-r--r--   0 runner    (1001) docker     (121)     8463 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/iterators/Iterators.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/iterators/batcher.md
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/iterators/iterators.md
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/iterators/shufflers.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.914426 ceruleo-2.0.3/docs/models/
--rw-r--r--   0 runner    (1001) docker     (121)   190058 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/models/Models.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   304534 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/models/Models_sklearn.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/models/baseline.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.914426 ceruleo-2.0.3/docs/models/keras/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.914426 ceruleo-2.0.3/docs/models/keras/catalog/
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/models/keras/catalog/models.md
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/models/keras/index.md
--rw-r--r--   0 runner    (1001) docker     (121)   139463 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/models/models_tf.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/models/sklearn.md
--rw-r--r--   0 runner    (1001) docker     (121)    13289 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/refs.bib
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.914426 ceruleo-2.0.3/docs/results/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/results/results.md
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/results/visualization.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.914426 ceruleo-2.0.3/docs/transformation/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.914426 ceruleo-2.0.3/docs/transformation/features/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/transformation/features/cast.md
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/transformation/features/denoising.md
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/transformation/features/entropy.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/transformation/features/extraction.md
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/transformation/features/imputers.md
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/transformation/features/outliers.md
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/transformation/features/resamplers.md
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/transformation/features/selection.md
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/transformation/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-05 12:33:22.000000 ceruleo-2.0.3/docs/transformation/transformers.md
--rw-r--r--   0 runner    (1001) docker     (121)     3034 2022-09-05 12:33:22.000000 ceruleo-2.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-09-05 12:33:22.000000 ceruleo-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-09-05 12:33:22.000000 ceruleo-2.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-09-05 12:33:33.918427 ceruleo-2.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 12:33:33.918427 ceruleo-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/manual_features.py
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_batcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     7051 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     3264 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_denoising.py
--rw-r--r--   0 runner    (1001) docker     (121)     2416 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     2655 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_graphics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_imputers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_iterators.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_lrucache.py
--rw-r--r--   0 runner    (1001) docker     (121)    10230 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     9526 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_scalers.py
--rw-r--r--   0 runner    (1001) docker     (121)     7061 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_shufflers.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_transformation.py
--rw-r--r--   0 runner    (1001) docker     (121)    20826 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-09-05 12:33:22.000000 ceruleo-2.0.3/tests/test_utils.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.bumpversion.cfg
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.coveragerc
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 ceruleo-2.0.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 ceruleo-2.0.4/RELEASING.md
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 ceruleo-2.0.4/mkdocs.yml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 ceruleo-2.0.4/requirements.txt
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.github/workflows/joss.yml
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/__init__.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/transformed.py
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/ts_dataset.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/utils.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/analysis/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/analysis/correlation.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/analysis/distribution.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/analysis/numerical_features.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/analysis/sample_rate.py
+-rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/catalog/CMAPSS.py
+-rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/catalog/CMAPSS2.py
+-rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/catalog/PHMDataset2018.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/dataset/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/__init__.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/analysis.py
+-rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/duration.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/explanations.py
+-rw-r--r--   0        0        0    21072 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/results.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/utils/__init__.py
+-rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/graphics/utils/curly_brace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/iterators/__init__.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/iterators/batcher.py
+-rw-r--r--   0        0        0    12822 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/iterators/iterators.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/iterators/sample_weight.py
+-rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/iterators/shufflers.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/iterators/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/__init__.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/baseline.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/pytorch.py
+-rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/sklearn.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/inspection/feature_importance.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/__init__.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/callbacks.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/dataset.py
+-rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/layers.py
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/losses.py
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/weibull.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/CNLSTM.py
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/InceptionTime.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/MSWRLRCN.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/MVCNN.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/MultiScaleConvolutional.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/MultiTaskRUL.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/XCM.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/XiangQiangJianQiao.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/keras/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/torch/__init__.py
+-rw-r--r--   0        0        0    15678 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/torch/dsanet.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/models/torch/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/results/__init__.py
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/results/picewise_regression.py
+-rw-r--r--   0        0        0    22960 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/results/results.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/target.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/__init__.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/cast.py
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/denoising.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/entropy.py
+-rw-r--r--   0        0        0    33816 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/extraction.py
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/extraction_frequency.py
+-rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/hurst.py
+-rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/imputers.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/operations.py
+-rw-r--r--   0        0        0    10745 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/outliers.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/resamplers.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/rolling_windows.py
+-rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/scalers.py
+-rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/selection.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/slicing.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/split.py
+-rw-r--r--   0        0        0    10869 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/tdigest.py
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/features/transformation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/__init__.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/common.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/concatenate.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/graph_utils.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/mixin.py
+-rw-r--r--   0        0        0     8446 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/transformers.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/transformerstep.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/__init__.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/cache_store.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/pipeline.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/runner.py
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/traversal.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/utils/__init__.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/utils/download.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ceruleo-2.0.4/ceruleo/utils/lrucache.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/index.md
+-rw-r--r--   0        0        0    13289 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/refs.bib
+-rw-r--r--   0        0        0   185022 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/Example.ipynb
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/catalog.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/dataset.md
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/visualization.md
+-rw-r--r--   0        0        0   478504 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/analysis/Sensor Validation.ipynb
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/analysis/correlation.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/analysis/distribution.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/analysis/sample_rate.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/dataset/analysis/sensor_validation.md
+-rw-r--r--   0        0        0    17517 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/images/cerulean.png
+-rw-r--r--   0        0        0    67664 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/images/unipd_logo.png
+-rw-r--r--   0        0        0    50083 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/img/duration_histogram.png
+-rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/iterators/Iterators.ipynb
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/iterators/batcher.md
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/iterators/iterators.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/iterators/shufflers.md
+-rw-r--r--   0        0        0   631762 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/Models.ipynb
+-rw-r--r--   0        0        0   304534 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/Models_sklearn.ipynb
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/baseline.md
+-rw-r--r--   0        0        0   139463 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/models_tf.ipynb
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/sklearn.md
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/keras/index.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/models/keras/catalog/models.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/results/results.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/results/visualization.md
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/pipeline.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/transformers.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/cast.md
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/denoising.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/entropy.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/extraction.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/imputers.md
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/outliers.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/resamplers.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ceruleo-2.0.4/docs/transformation/features/selection.md
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 ceruleo-2.0.4/paper/paper.bib
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 ceruleo-2.0.4/paper/paper.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/manual_features.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_analysis.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_batcher.py
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_dataset.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_denoising.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_graph.py
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_graphics.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_imputers.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_iterators.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_lrucache.py
+-rw-r--r--   0        0        0    13157 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_models.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_operations.py
+-rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_pipeline.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_results.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_scalers.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_shufflers.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_transformation.py
+-rw-r--r--   0        0        0    20808 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_transformers.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_utils.py
+-rw-r--r--   0        0        0    48809 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_XCM_explanation-expected.png
+-rw-r--r--   0        0        0    14744 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_barplot_errors_wrt_RUL-expected.png
+-rw-r--r--   0        0        0    22355 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_boxplot_errors_wrt_RUL-expected.png
+-rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_correlation_plot-expected.png
+-rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_durations_boxplot-expected.png
+-rw-r--r--   0        0        0    23670 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_durations_histogram-expected.png
+-rw-r--r--   0        0        0    26658 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_plot_predictions_grid_1-expected.png
+-rw-r--r--   0        0        0    38027 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_plot_predictions_grid_2-expected.png
+-rw-r--r--   0        0        0    53987 2020-02-02 00:00:00.000000 ceruleo-2.0.4/tests/test_images/test_shadedline_plot_errors_wrt_RUL-expected.png
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 ceruleo-2.0.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ceruleo-2.0.4/LICENSE
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 ceruleo-2.0.4/README.md
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ceruleo-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 ceruleo-2.0.4/PKG-INFO
```

### Comparing `ceruleo-2.0.3/.github/workflows/documentation.yml` & `ceruleo-2.0.4/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/.github/workflows/publish.yml` & `ceruleo-2.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/.github/workflows/test.yml` & `ceruleo-2.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/.gitignore` & `ceruleo-2.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/CONTRIBUTING.md` & `ceruleo-2.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/LICENSE` & `ceruleo-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/PKG-INFO` & `ceruleo-2.0.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,22 @@
-Metadata-Version: 2.1
-Name: ceruleo
-Version: 2.0.3
-Summary: Remaining useful life estimation utilities
-Home-page: https://github.com/lucianolorenti/ceruleo
-License: MIT
-Keywords: predictive maintenance,remaining useful life
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: doc
-License-File: LICENSE
-
 <div align="center">
   <img src="https://github.com/lucianolorenti/ceruleo/blob/main/docs/images/cerulean.png?raw=true"><br>
 </div>
 
 # CeRULEo
 -----------------
 
 
 # CeRULEo: Comprehensive utilitiEs for Remaining Useful Life Estimation methOds
 
-[![Coverage Status](https://coveralls.io/repos/github/lucianolorenti/ceruleo/badge.svg?branch=main)](https://coveralls.io/github/lucianolorenti/ceruleo?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/lucianolorenti/ceruleo/badge.svg?branch=main&service=github)](https://coveralls.io/github/lucianolorenti/ceruleo?branch=main)
 [![Documentation](https://img.shields.io/badge/documentation-dev-brightgreen)](https://lucianolorenti.github.io/ceruleo/)
-
+![pypi](https://img.shields.io/pypi/v/ceruleo)
+![python-version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
+[![status](https://joss.theoj.org/papers/c879c234d7741885576ddc682416b41f/status.svg)](https://joss.theoj.org/papers/c879c234d7741885576ddc682416b41f)
 ## What is it?
 
 **CeRULeo** is a Python package that provides a flexible environment designed to make working with predictive maintenance task both easy and intuitive. 
 
 
 # Installation
 It is recommended to use pip  for installation. Please make sure the latest version is installed:
```

#### html2text {}

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 2.1 Name: ceruleo Version: 2.0.3 Summary: Remaining useful
-life estimation utilities Home-page: https://github.com/lucianolorenti/ceruleo
-License: MIT Keywords: predictive maintenance,remaining useful life Classifier:
-Programming Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering
-:: Artificial Intelligence Requires-Python: >=3.7 Description-Content-Type:
-text/markdown Provides-Extra: test Provides-Extra: doc License-File: LICENSE
        [https://github.com/lucianolorenti/ceruleo/blob/main/docs/images/
                             cerulean.png?raw=true]
 # CeRULEo ----------------- # CeRULEo: Comprehensive utilitiEs for Remaining
 Useful Life Estimation methOds [![Coverage Status](https://coveralls.io/repos/
-github/lucianolorenti/ceruleo/badge.svg?branch=main)](https://coveralls.io/
-github/lucianolorenti/ceruleo?branch=main) [![Documentation](https://
-img.shields.io/badge/documentation-dev-brightgreen)](https://
-lucianolorenti.github.io/ceruleo/) ## What is it? **CeRULeo** is a Python
+github/lucianolorenti/ceruleo/badge.svg?branch=main&service=github)](https://
+coveralls.io/github/lucianolorenti/ceruleo?branch=main) [![Documentation]
+(https://img.shields.io/badge/documentation-dev-brightgreen)](https://
+lucianolorenti.github.io/ceruleo/) ![pypi](https://img.shields.io/pypi/v/
+ceruleo) ![python-version](https://img.shields.io/badge/python-
+3.8%20%7C%203.9%20%7C%203.10-blue) [![status](https://joss.theoj.org/papers/
+c879c234d7741885576ddc682416b41f/status.svg)](https://joss.theoj.org/papers/
+c879c234d7741885576ddc682416b41f) ## What is it? **CeRULeo** is a Python
 package that provides a flexible environment designed to make working with
 predictive maintenance task both easy and intuitive. # Installation It is
 recommended to use pip for installation. Please make sure the latest version is
 installed: ```bash pip install ceruleo # normal install pip install --upgrade
 ceruleo # or update if needed ``` Alternatively, you could clone and install it
 from the sources: ```bash git clone https://github.com/lucianolorenti/
 ceruleo.git cd ceruleo pip install . ``` Made with <3 @ [University_of_Padova]
```

### Comparing `ceruleo-2.0.3/ceruleo/dataset/analysis/correlation.py` & `ceruleo-2.0.4/ceruleo/dataset/analysis/correlation.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,14 @@
     for ex in iterate_over_features(dataset):
         ex = ex[features]
         corr_m = ex.corr().fillna(0)
 
         correlated_features_for_execution = []
 
         for f1, f2 in combinations(features, 2):
-            if f1 == f2:
-                continue
-
             correlated_features_for_execution.append((f1, f2, corr_m.loc[f1, f2]))
 
         correlated_features.extend(correlated_features_for_execution)
 
     df = pd.DataFrame(correlated_features, columns=["Feature 1", "Feature 2", "Corr"])
     output = df.groupby(by=["Feature 1", "Feature 2"]).mean()
     output.rename(columns={"Corr": "Mean Correlation"}, inplace=True)
```

### Comparing `ceruleo-2.0.3/ceruleo/dataset/analysis/distribution.py` & `ceruleo-2.0.4/ceruleo/dataset/analysis/distribution.py`

 * *Files 25% similar despite different names*

```diff
@@ -94,47 +94,8 @@
         data = {}
         for ((i, h1), (j, h2)) in itertools.combinations(enumerate(histograms[feature]), 2):
             kl = (np.mean(kl_div(h1, h2)) + np.mean(kl_div(h2, h1))) / 2
             wd = wasserstein_distance(h1, h2)
             df_data.append((i, j, wd, kl, feature))
     df = pd.DataFrame(df_data, columns=["Life 1", "Life 2", "W", "KL", "feature"])
 
-    return df
-
-
-def wasserstein_between_lives(
-    life1: pd.DataFrame, life2: pd.DataFrame, columns: List[str], bins: int = 15
-) -> pd.DataFrame:
-    """Computer the Wasserstein distance between the features of two run-to-failure cycles
-
-    Parameters:
-
-        life1: Run-to-cycle failure
-        life2: Run-to-cycle failure
-        columns: List of features to consider
-        bins: Number of bins to make the distribution
-
-    Returns:
-
-        w: A dataframe with one column called Wasserstein
-
-    """
-
-    def dropna_values(x):
-        return x[~np.isnan(x)]
-
-    data = []
-    for c in columns:
-        v1 = dropna_values(life1[c].values)
-        v2 = dropna_values(life2[c].values)
-        n_points = min(len(v1), len(v2))
-        v1 = np.random.choice(v1, n_points)
-        v2 = np.random.choice(v2, n_points)
-        _, b = np.histogram(np.hstack((v1, v2)), bins=bins)
-
-        h1, _ = np.histogram(v1, bins=b)
-        h2, _ = np.histogram(v2, bins=b)
-
-        # h1 = h1 / (np.nansum(h1)+ 0.0001)
-        # h2 = h2 / (np.nansum(h2) + 0.0001)
-
-    return pd.DataFrame(data, columns=["Wasserstein"], index=columns)
+    return df
```

### Comparing `ceruleo-2.0.3/ceruleo/dataset/analysis/numerical_features.py` & `ceruleo-2.0.4/ceruleo/dataset/analysis/numerical_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from collections import defaultdict
 from typing import Dict, List, Optional, Union
 
 import antropy as ant
 import numpy as np
 import pandas as pd
-
-from pyparsing import col
 from scipy.stats import spearmanr
-from ceruleo.dataset.transformed import TransformedDataset
-from tqdm.auto import tqdm
 from sklearn.feature_selection import mutual_info_regression
+from tqdm.auto import tqdm
+from uncertainties import ufloat
+
+from ceruleo.dataset.transformed import TransformedDataset
 from ceruleo.dataset.ts_dataset import AbstractLivesDataset
 from ceruleo.dataset.utils import iterate_over_features_and_target
-from uncertainties import ufloat
 
 
 def entropy(s: np.ndarray)-> float:
     """Approximate entropy
 
     The approximate entropy quantifies the amount of regularity and the unpredictability of fluctuations over time-series data.
```

### Comparing `ceruleo-2.0.3/ceruleo/dataset/analysis/sample_rate.py` & `ceruleo-2.0.4/ceruleo/dataset/analysis/sample_rate.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import pandas as pd
 from ceruleo.dataset.ts_dataset import AbstractTimeSeriesDataset
 
 logger = logging.getLogger(__name__)
 
 
-def sample_rate(ds: AbstractTimeSeriesDataset, unit: Optional[str] = "s") -> np.ndarray:
+def sample_rate(ds: AbstractTimeSeriesDataset, unit: str = "s") -> np.ndarray:
     """Obtain an array of time difference between two consecutive samples
 
     If the index it's a timestamp, the time difference will be converted to the provided
     unit
 
     Parameters:
         ds: The dataset
@@ -23,16 +23,14 @@
         sample_rates: np.ndarray
 
     """
     time_diff = []
     for life in ds:
         diff = np.diff(life.index.values)
         if pd.api.types.is_timedelta64_ns_dtype(diff.dtype):
-            if unit is None:
-                unit = "s"
             diff = diff / np.timedelta64(1, unit)
         time_diff.extend(diff)
     return np.array(time_diff)
 
 
 def sample_rate_summary(
     ds: AbstractTimeSeriesDataset, unit: Optional[str] = "s"
```

### Comparing `ceruleo-2.0.3/ceruleo/dataset/catalog/CMAPSS.py` & `ceruleo-2.0.4/ceruleo/dataset/catalog/CMAPSS.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/dataset/catalog/CMAPSS2.py` & `ceruleo-2.0.4/ceruleo/dataset/catalog/CMAPSS2.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/dataset/catalog/PHMDataset2018.py` & `ceruleo-2.0.4/ceruleo/dataset/catalog/PHMDataset2018.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,34 @@
 
     path = path / "raw"
     path.mkdir(parents=True, exist_ok=True)
     if not (path / OUTPUT).resolve().is_file():
         download(path)
     logger.info("Decompressing  dataset...")
     with tarfile.open(path / OUTPUT, "r") as tarball:
-        tarball.extractall(path=path, members=track_progress(tarball))
+        def is_within_directory(directory, target):
+            
+            abs_directory = os.path.abspath(directory)
+            abs_target = os.path.abspath(target)
+        
+            prefix = os.path.commonprefix([abs_directory, abs_target])
+            
+            return prefix == abs_directory
+        
+        def safe_extract(tar, path=".", members=None, *, numeric_owner=False):
+        
+            for member in tar.getmembers():
+                member_path = os.path.join(path, member.name)
+                if not is_within_directory(path, member_path):
+                    raise Exception("Attempted Path Traversal in Tar File")
+        
+            tar.extractall(path, members, numeric_owner=numeric_owner) 
+            
+        
+        safe_extract(tarball, path=path, members=track_progress(tarball))
     shutil.move(str(path / "phm_data_challenge_2018" / "train"), str(path / "train"))
     shutil.move(str(path / "phm_data_challenge_2018" / "test"), str(path / "test"))
     shutil.rmtree(str(path / "phm_data_challenge_2018"))
     (path / OUTPUT).unlink()
 
 
 class FailureType(Enum):
```

### Comparing `ceruleo-2.0.3/ceruleo/dataset/transformed.py` & `ceruleo-2.0.4/ceruleo/dataset/transformed.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/dataset/ts_dataset.py` & `ceruleo-2.0.4/ceruleo/dataset/ts_dataset.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/dataset/utils.py` & `ceruleo-2.0.4/ceruleo/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/graphics/analysis.py` & `ceruleo-2.0.4/ceruleo/graphics/analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from typing import List, Optional
 
 import matplotlib
 import matplotlib.pyplot as plt
 from ceruleo.dataset.ts_dataset import AbstractTimeSeriesDataset
+from ceruleo.dataset.analysis.correlation import correlation_analysis
 
 
-def correlation_analysis(
+def plot_correlation_analysis(
     dataset: AbstractTimeSeriesDataset,
     corr_threshold: float = 0,
     features: Optional[List[str]] = None,
-    ax: matplotlib.axes.Axes = Optional[None],
+    ax: Optional[matplotlib.axes.Axes] = None,
     **kwargs,
 ):
     """Plot the correlated features in a dataset
 
     Parameters:
-    
+
         dataset: The dataset
         corr_threshold: Minimum threshold to consider that the correlation is high
         features: List of features
         ax: The axis where to draw
 
     Returns:
         ax: the axis
     """
 
-    df = correlation_analysis(
-        dataset, corr_threshold, features=list(set(features) - set(["relative_time"]))
-    )
+    if features is not None:
+        features = list(set(features) - set(["relative_time"]))
+
+    df = correlation_analysis(dataset, corr_threshold, features=features)
     df1 = df[(df["Abs mean correlation"] > corr_threshold)]
 
     df1.reset_index(inplace=True)
     df1.sort_values(by="Mean Correlation", ascending=True, inplace=True)
     if ax is None:
         fig, ax = plt.subplots(**kwargs)
     labels = []
```

### Comparing `ceruleo-2.0.3/ceruleo/graphics/duration.py` & `ceruleo-2.0.4/ceruleo/graphics/duration.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         fontweight="semibold",
     )
     txt.set_path_effects([PathEffects.withStroke(linewidth=2, foreground="w")])
 
 
 def durations_histogram(
     datasets: Union[AbstractTimeSeriesDataset, List[AbstractTimeSeriesDataset]],
-    xlabel: str,
-    label: Union[str, List[str]] = "",
+    xlabel: str = 'Cycle Duration',
+    label: Union[str, List[str]] = "1",
     bins: int = 15,
     units: str = "m",
     vlines: Tuple[float, str] = [],
     ax:matplotlib.axes.Axes=None,
     add_mean: bool = True,
     add_median: bool = True,
     transform: Callable[[float], float] = lambda x: x,
@@ -164,21 +164,21 @@
 
     colors = sns.color_palette("hls", len(vlines))
     for i, (v_x, l) in enumerate(vlines):
         label = f"{l}: {v_x:.2f} {units}"
         add_vertical_line(ax, v_x, label, colors[i], i, len(vlines))
     ax.legend()
 
-    return ax.figure, ax
+    return ax
 
 
 def durations_boxplot(
     datasets: Union[AbstractTimeSeriesDataset, List[AbstractTimeSeriesDataset]],
     xlabel: Union[str, List[str]],
-    ylabel: str,
+    ylabel: str = 'Cycle Duration',
     ax:Optional[matplotlib.axes.Axes]=None,
     hlines: List[Tuple[float, str]] = [],
     units: str = "m",
     transform: Callable[[float], float] = lambda x: x,
     maxy: Optional[float] = None,
     **kwargs,
 ) ->  matplotlib.axes.Axes:
```

### Comparing `ceruleo-2.0.3/ceruleo/graphics/results.py` & `ceruleo-2.0.4/ceruleo/graphics/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,41 +2,46 @@
 
 
 It is possible to visualize how it grows the unexploited lifetime grows as the conservative window size grows and how the unexpected breaks decrease as the conservative window size grows.
 
 
 """
 import math
-from typing import Dict, Iterable, List, Optional, Union
+from typing import Dict, Iterable, List, Optional, Tuple, Union
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
-
 import seaborn as sns
+
 from ceruleo.dataset.transformed import TransformedDataset
 from ceruleo.graphics.utils.curly_brace import curlyBrace
-from ceruleo.results.results import (FittedLife, PredictionResult,
-                                     models_cv_results, split_lives,
-                                     unexpected_breaks, unexploited_lifetime)
+from ceruleo.results.results import (
+    FittedLife,
+    PredictionResult,
+    models_cv_results,
+    split_lives,
+    unexpected_breaks,
+    unexploited_lifetime,
+)
 
 
 def plot_lives(ds: TransformedDataset):
     """
     Plot each life
 
     Parameters:
 
         ds: A transformed dataset
     """
     fig, ax = plt.subplots()
     it = ds
     for _, y in it:
         ax.plot(y)
-    return fig, ax
+    return ax
 
 
 def cv_plot_errors_wrt_RUL(bin_edges, error_histogram, **kwargs):
     """"""
     fig, ax = plt.subplots(**kwargs)
     labels = []
     heights = []
@@ -49,15 +54,15 @@
         yerr.append(np.std(error_histogram[i]))
         labels.append(f"[{bin_edges[i]:.1f}, {bin_edges[i+1]:.1f})")
 
     ax.bar(height=heights, x=xs, yerr=yerr, tick_label=labels)
     ax.set_xlabel("RUL")
     ax.set_ylabel("RMSE")
 
-    return fig, ax
+    return ax
 
 
 def _boxplot_errors_wrt_RUL_multiple_models(
     bin_edge: np.array,
     model_results: dict,
     ax=None,
     y_axis_label: Optional[str] = None,
@@ -112,15 +117,15 @@
         x = np.mean(
             [(model_number * 0.5) + (i * n_models) for model_number in range(n_models)]
         )
         ticks.append(x)
 
     max_x = np.max(ticks) + 1
     ax.set_xlabel("RUL" + ("" if x_axis_label is None else x_axis_label))
-    ax.set_ylabel("$y - \hat{y}$" + ("" if y_axis_label is None else y_axis_label))
+    ax.set_ylabel(r"$y - \hat{y}$" + ("" if y_axis_label is None else y_axis_label))
     ax.set_xticks(ticks)
     ax.set_xticklabels(labels)
     ax.legend()
     ax2 = ax.twinx()
     ax2.set_xlim(ax.get_xlim())
     ax2.set_ylim(ax.get_ylim())
     curlyBrace(
@@ -133,15 +138,15 @@
         ax2,
         (max_x, max_value),
         (max_x, 0),
         str_text="Under estim.",
         c="#000",
     )
 
-    return ax.figure, ax
+    return ax
 
 
 def boxplot_errors_wrt_RUL(
     results_dict: Dict[str, List[PredictionResult]],
     nbins: int,
     y_axis_label: Optional[str] = None,
     x_axis_label: Optional[str] = None,
@@ -259,20 +264,20 @@
     ticks = []
     dx = 0
     for i in range(nbins):
         ticks.append( dx + bar_group_width/2)
         dx += bar_group_width + group_separation
 
     ax.set_xlabel("RUL" + ("" if x_axis_label is None else x_axis_label))
-    ax.set_ylabel("$y - \hat{y}$" + ("" if y_axis_label is None else y_axis_label))
+    ax.set_ylabel(r"$y - \hat{y}$" + ("" if y_axis_label is None else y_axis_label))
     ax.set_xticks(ticks)
     ax.set_xticklabels(labels)
     ax.legend()
 
-    return fig, ax
+    return ax
 
 
 def barplot_errors_wrt_RUL(
     results_dict: Dict[str, List[PredictionResult]],
     nbins: int,
     y_axis_label=None,
     x_axis_label=None,
@@ -366,15 +371,15 @@
     for i in range(nbins):
         x = np.mean(
             [(model_number * 0.5) + (i * n_models) for model_number in range(n_models)]
         )
         ticks.append(x)
 
     ax.set_xlabel("RUL" + ("" if x_axis_label is None else x_axis_label))
-    ax.set_ylabel("$y - \hat{y}$" + ("" if y_axis_label is None else y_axis_label))
+    ax.set_ylabel(r"$y - \hat{y}$" + ("" if y_axis_label is None else y_axis_label))
     ax.set_xticks(ticks)
     ax.set_xticklabels(labels)
     ax.legend()
     max_x = np.max(ticks) + 1
     ax2 = ax.twinx()
     ax2.set_xlim(ax.get_xlim())
     ax2.set_ylim(ax.get_ylim())
@@ -681,43 +686,51 @@
 
     for a in ax.flatten():
         a.legend()
     return ax
 
 
 def plot_predictions(
-    result: PredictionResult,
+    result: Union[PredictionResult, Tuple[np.ndarray, np.ndarray]],
+    *,
     ax:Optional[matplotlib.axes.Axes]=None,
     units: str = "Hours [h]",
     markersize: float = 0.7,
+    marker: str = 'o',
     plot_fitted: bool  = True,
     model_name:str = '',
     **kwargs,
 ) -> matplotlib.axes.Axes:
     """Plots the predicted and the true remaining useful lives
 
     Parameters:
     
-        result: A PredictionResult object
+        result: A PredictionResult object or a tuple with (y_true, y_predicted)
         ax:  Axis to plot. If it is missing a new figure will be created
         units: Units of time to be used in the axis labels
-        cv: Number of the CV results
+        marker: Marker type
+        markersize: The size of the marker
+        plot_fitted: Wether to plot a LS line
+        model_name: Name of the model
+        
 
     Returns:
 
         ax: The axis on which the plot has been made
     """
     if ax is None:
         _, ax = plt.subplots(1, 1, **kwargs)
 
 
-
-    y_predicted = result.predicted_RUL
-    y_true = result.true_RUL
-    ax.plot(y_predicted, "o", label=f"Predicted {model_name}", markersize=markersize)
+    if isinstance(result, PredictionResult):
+        y_predicted = result.predicted_RUL
+        y_true = result.true_RUL
+    else:
+        y_true, y_predicted = result
+    ax.plot(y_predicted, marker, label=f"Predicted {model_name}", markersize=markersize)
     ax.plot(y_true, label="True")
     x = 0
 
 
     if plot_fitted:
         try:
             fitted = np.hstack([life.y_pred_fitted for life in split_lives(result)])
@@ -725,12 +738,12 @@
             
         except:
             
             pass
     ax.set_ylabel(units)
     ax.set_xlabel(units)
     legend = ax.legend()
-    for l in legend.legendHandles:
+    for l in legend.legend_handles:
         l.set_markersize(6)
 
 
     return ax
```

### Comparing `ceruleo-2.0.3/ceruleo/graphics/utils/curly_brace.py` & `ceruleo-2.0.4/ceruleo/graphics/utils/curly_brace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-'''
+"""
 Module Name : curlyBrace
 
 Author : 高斯羽 博士 (Dr. GAO, Siyu)
 
 Version : 1.0.2
 
 Last Modified : 2019-04-22
@@ -33,22 +32,22 @@
 
 List of functions
 ----------------------
 
 * getAxSize_
 * curlyBrace_
 
-'''
+"""
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 
 def getAxSize(fig, ax):
-    '''
+    """
     .. _getAxSize :
 
     Get the axes size in pixels.
 
     Parameters
     ----------
     fig : matplotlib figure object
@@ -64,45 +63,47 @@
 
     ax_height : float
         The axes height in pixels.
 
     Reference
     -----------
     https://stackoverflow.com/questions/19306510/determine-matplotlib-axis-size-in-pixels
-    '''
+    """
 
     bbox = ax.get_window_extent().transformed(fig.dpi_scale_trans.inverted())
     ax_width, ax_height = bbox.width, bbox.height
     ax_width *= fig.dpi
     ax_height *= fig.dpi
 
     return ax_width, ax_height
 
 
-def curlyBrace(fig,
-               ax,
-               p1,
-               p2,
-               k_r=0.1,
-               bool_auto=True,
-               str_text='',
-               int_line_num=2,
-               fontdict={},
-               **kwargs):
+def curlyBrace(
+    fig,
+    ax,
+    p1,
+    p2,
+    k_r=0.1,
+    bool_auto=True,
+    str_text="",
+    int_line_num=2,
+    fontdict={},
+    **kwargs
+):
     # def curlyBrace(fig, ax, p1, p2, k_r=0.1, bool_auto=True, str_text='', int_line_num=2, fontdict={}, **kwargs):
-    '''
+    """
     .. _curlyBrace :
 
     Plot an optionally annotated curly bracket on the given axes of the given figure.
 
     Note that the brackets are anti-clockwise by default. To reverse the text position, swap
     "p1" and "p2".
 
     Note that, when the axes aspect is not set to "equal", the axes coordinates need to be
-    transformed to screen coordinates, otherwise the arcs may not be seeable. 
+    transformed to screen coordinates, otherwise the arcs may not be seeable.
 
     Parameters
     ----------
     fig : matplotlib figure object
         The of the target axes.
 
     ax : matplotlib axes object
@@ -133,15 +134,15 @@
 
         Default = True
 
     str_text : string
         The annotation text of the bracket. It would displayed at the mid point
         of bracket with the same rotation as the bracket.
 
-        By default, it follows the anti-clockwise convention. To flip it, swap 
+        By default, it follows the anti-clockwise convention. To flip it, swap
         the end point and the starting point.
 
         The appearance of this string can be set by using "fontdict", which follows
         the same syntax as the normal matplotlib syntax for font dictionary.
 
         Default = empty string (no annotation)
 
@@ -183,26 +184,26 @@
 
     arc4 : list of lists
         arc4 positions.
 
     Reference
     ----------
     https://uk.mathworks.com/matlabcentral/fileexchange/38716-curly-brace-annotation
-    '''
+    """
 
     pt1 = [None, None]
     pt2 = [None, None]
 
     ax_width, ax_height = getAxSize(fig, ax)
 
     ax_xlim = list(ax.get_xlim())
     ax_ylim = list(ax.get_ylim())
 
     # log scale consideration
-    if 'log' in ax.get_xaxis().get_scale():
+    if "log" in ax.get_xaxis().get_scale():
 
         if p1[0] > 0.0:
 
             pt1[0] = np.log(p1[0])
 
         elif p1[0] < 0.0:
 
@@ -239,15 +240,15 @@
                 ax_xlim[i] = 0.0
 
     else:
 
         pt1[0] = p1[0]
         pt2[0] = p2[0]
 
-    if 'log' in ax.get_yaxis().get_scale():
+    if "log" in ax.get_yaxis().get_scale():
 
         if p1[1] > 0.0:
 
             pt1[1] = np.log(p1[1])
 
         elif p1[1] < 0.0:
 
@@ -359,15 +360,15 @@
 
     arc1y = arc1y / yscale + ax_ylim[0]
     arc2y = arc2y / yscale + ax_ylim[0]
     arc3y = arc3y / yscale + ax_ylim[0]
     arc4y = arc4y / yscale + ax_ylim[0]
 
     # log scale consideration
-    if 'log' in ax.get_xaxis().get_scale():
+    if "log" in ax.get_xaxis().get_scale():
 
         for i in range(0, len(arc1x)):
 
             if arc1x[i] > 0.0:
 
                 arc1x[i] = np.exp(arc1x[i])
 
@@ -421,15 +422,15 @@
 
                 arc4x[i] = 0.0
 
     else:
 
         pass
 
-    if 'log' in ax.get_yaxis().get_scale():
+    if "log" in ax.get_yaxis().get_scale():
 
         for i in range(0, len(arc1y)):
 
             if arc1y[i] > 0.0:
 
                 arc1y[i] = np.exp(arc1y[i])
 
@@ -490,28 +491,24 @@
     # plot arcs
     ax.plot(arc1x, arc1y, clip_on=False, **kwargs)
     ax.plot(arc2x, arc2y, clip_on=False, **kwargs)
     ax.plot(arc3x, arc3y, clip_on=False, **kwargs)
     ax.plot(arc4x, arc4y, clip_on=False, **kwargs)
 
     # plot lines
-    ax.plot([arc1x[-1], arc2x[1]], [arc1y[-1], arc2y[1]],
-            clip_on=False,
-            **kwargs)
-    ax.plot([arc3x[-1], arc4x[1]], [arc3y[-1], arc4y[1]],
-            clip_on=False,
-            **kwargs)
+    ax.plot([arc1x[-1], arc2x[1]], [arc1y[-1], arc2y[1]], clip_on=False, **kwargs)
+    ax.plot([arc3x[-1], arc4x[1]], [arc3y[-1], arc4y[1]], clip_on=False, **kwargs)
 
     summit = [arc2x[-1], arc2y[-1]]
 
     if str_text:
 
         int_line_num = int(int_line_num)
 
-        str_temp = '\n' * int_line_num
+        str_temp = "\n" * int_line_num
 
         # convert radians to degree and within 0 to 360
         ang = np.degrees(theta) % 360.0
 
         if (ang >= 0.0) and (ang <= 90.0):
 
             rotation = ang
@@ -530,26 +527,28 @@
 
             str_text = str_text + str_temp
 
         else:
 
             rotation = ang
 
-        ax.axes.text(arc2x[-1],
-                     arc2y[-1],
-                     str_text,
-                     ha='center',
-                     va='center',
-                     rotation=rotation,
-                     fontdict=fontdict,
-                     clip_on=False)
+        ax.axes.text(
+            arc2x[-1],
+            arc2y[-1],
+            str_text,
+            ha="center",
+            va="center",
+            rotation=rotation,
+            fontdict=fontdict,
+            clip_on=False,
+        )
 
     else:
 
         pass
 
     arc1 = [arc1x, arc1y]
     arc2 = [arc2x, arc2y]
     arc3 = [arc3x, arc3y]
     arc4 = [arc4x, arc4y]
 
-    return theta, summit, arc1, arc2, arc3, arc4
+    return theta, summit, arc1, arc2, arc3, arc4
```

### Comparing `ceruleo-2.0.3/ceruleo/iterators/batcher.py` & `ceruleo-2.0.4/ceruleo/iterators/batcher.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/iterators/iterators.py` & `ceruleo-2.0.4/ceruleo/iterators/iterators.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/iterators/sample_weight.py` & `ceruleo-2.0.4/ceruleo/iterators/sample_weight.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/iterators/shufflers.py` & `ceruleo-2.0.4/ceruleo/iterators/shufflers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/iterators/utils.py` & `ceruleo-2.0.4/ceruleo/iterators/utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/baseline.py` & `ceruleo-2.0.4/ceruleo/models/baseline.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/inspection/feature_importance.py` & `ceruleo-2.0.4/ceruleo/models/inspection/feature_importance.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/keras/catalog/CNLSTM.py` & `ceruleo-2.0.4/ceruleo/models/keras/catalog/CNLSTM.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 def CNLSTM(
     input_shape: Tuple[int, int],
     *,
     n_conv_layers: int,
     initial_convolutional_size: int,
     layers_recurrent: List[int],
     hidden_size: Tuple[int, int],
-    dropout: float,
+    dense_layer_size: int = 50,
+    dropout: float = 0.1,
 ):
     """
     The network contains stacked layers of 1-dimensional convolutional layers
     followed by max poolings
 
     * Temporal Convolutional Memory Networks forRemaining Useful Life Estimation of Industrial Machinery
     * Lahiru Jayasinghe, Tharaka Samarasinghe, Chau Yuen, Jenny Chen Ni Low, Shuzhi Sam Ge
@@ -32,14 +33,15 @@
             and a 1D-max-pooling   poolsize=2, strides=2, padding=same
         initial_convolutional_size: The number of filters of the first convolutional layers.
               Next ones will have the power of 2 of the previous one
         layers_recurrent: Number of current layers. Each recurrent layer is composed by an LSTM layer
         hidden_size: After the convolutional layers the signal is projected via a RELU layer and then
                      reshaped again as a time series of size (hidden_size[0], hidden_size[1])
         dropout: Droput factor
+        dense_layer_size: Size of the dense layer before the head
     """
 
     model = Sequential()
     model.add(Input(shape=input_shape))
 
     for n_filters in range(n_conv_layers):
         model.add(
@@ -66,11 +68,11 @@
                 n_filters, return_sequences=i < len(layers_recurrent) - 1
             )
         )
 
     model.add(Dropout(dropout))
 
     model.add(Flatten())
-    model.add(Dense(50, activation="relu"))
+    model.add(Dense(dense_layer_size, activation="relu"))
     model.add(Dropout(dropout))
     model.add(Dense(1, activation="relu"))
     return model
```

### Comparing `ceruleo-2.0.3/ceruleo/models/keras/catalog/InceptionTime.py` & `ceruleo-2.0.4/ceruleo/models/keras/catalog/InceptionTime.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/keras/catalog/MSWRLRCN.py` & `ceruleo-2.0.4/ceruleo/models/keras/catalog/MSWRLRCN.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/keras/catalog/MVCNN.py` & `ceruleo-2.0.4/ceruleo/models/keras/catalog/MVCNN.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/keras/catalog/MultiScaleConvolutional.py` & `ceruleo-2.0.4/ceruleo/models/keras/catalog/MultiScaleConvolutional.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/keras/catalog/MultiTaskRUL.py` & `ceruleo-2.0.4/ceruleo/models/keras/catalog/MultiTaskRUL.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/keras/catalog/XCM.py` & `ceruleo-2.0.4/ceruleo/models/keras/catalog/XCM.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/keras/catalog/XiangQiangJianQiao.py` & `ceruleo-2.0.4/ceruleo/models/keras/catalog/XiangQiangJianQiao.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/keras/dataset.py` & `ceruleo-2.0.4/ceruleo/models/keras/dataset.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/keras/layers.py` & `ceruleo-2.0.4/ceruleo/models/keras/layers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/keras/losses.py` & `ceruleo-2.0.4/ceruleo/models/keras/losses.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,20 +33,20 @@
 
     [Reference](https://ieeexplore.ieee.org/document/9287246)
 
     Parameters:
 
         y_true: True RUL values
         y_pred: Predicted RUL values
-        theta_l: theta parameter for underpredicting
-        alpha_l: alpha parameters for underpredicting
-        gamma_l: gamma parameters for underpredicting
-        theta_r:
-        alpha_r:
-        gamma_r:
+        theta_l: Linear to exponential change point for overpredictions (Positive)
+        alpha_l: Quadratic term parameters for overpredictions
+        gamma_l: Exponential term parameters for overpredictions
+        theta_r: Linear to exponential change point for underpredictions
+        alpha_r: Quadratic term parameters for underpredictions
+        gamma_r: Exponential term parameters for underpredictions
         relative_weight: Wether to use weigthing relative to the RUL
 
     Returns:
 
         l: the loss computed
     """
 
@@ -91,21 +91,21 @@
     Customizable Asymmetric Loss Functions for Machine Learning-based Predictive Maintenance.
     In 2020 8th International Conference on Condition Monitoring and Diagnosis
     (CMD) (pp. 250-253). IEEE.
 
     [Reference](https://ieeexplore.ieee.org/document/9287246)
 
     Parameters:
-        theta_l: Linear component of the assymetric loss in the underprediction
-        alpha_l: alpha component of the assymetric loss in the underprediction
-        gamma_l: gamma component of the assymetric loss in the underprediction
-        theta_r: theta component of the assymetric loss in the overprediction
-        alpha_r: alpha component of the assymetric loss in the overprediction
-        gamma_r: gamma component of the assymetric loss in the overprediction
-        relative_weight:
+        theta_l: Linear to exponential change point for overpredictions
+        alpha_l: Quadratic term parameters for overpredictions
+        gamma_l: Exponential term parameters for overpredictions
+        theta_r: Linear to exponential change point for underpredictions
+        alpha_r: Quadratic term parameters for underpredictions
+        gamma_r: Exponential term parameters for underpredictions
+        relative_weight: Wether to use weigthing relative to the RUL
     """
 
     def __init__(
         self,
         *,
         theta_l: float,
         alpha_l: float,
```

### Comparing `ceruleo-2.0.3/ceruleo/models/keras/weibull.py` & `ceruleo-2.0.4/ceruleo/models/keras/weibull.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/pytorch.py` & `ceruleo-2.0.4/ceruleo/models/pytorch.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/sklearn.py` & `ceruleo-2.0.4/ceruleo/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/torch/dsanet.py` & `ceruleo-2.0.4/ceruleo/models/torch/dsanet.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/models/torch/model.py` & `ceruleo-2.0.4/ceruleo/models/torch/model.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/results/picewise_regression.py` & `ceruleo-2.0.4/ceruleo/results/picewise_regression.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/results/results.py` & `ceruleo-2.0.4/ceruleo/results/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,17 @@
 [1] Machine Learning for Predictive Maintenance: A Multiple Classifiers Approach
     Susto, G. A., Schirru, A., Pampuri, S., McLoone, S., & Beghi, A. (2015). 
 
 
 """
 import logging
 from dataclasses import dataclass
-from typing import Callable, Dict, List, Optional, Tuple, Union
+from typing import  Dict, List, Optional, Tuple, Union
 
 import numpy as np
-import pandas as pd
 from ceruleo.results.picewise_regression import (PiecewesieLinearFunction,
                                                 PiecewiseLinearRegression)
 from sklearn.metrics import mean_absolute_error as mae
 from sklearn.metrics import mean_absolute_percentage_error as mape
 from sklearn.metrics import mean_squared_error as mse
 from uncertainties import ufloat
```

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/cast.py` & `ceruleo-2.0.4/ceruleo/transformation/features/cast.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/denoising.py` & `ceruleo-2.0.4/ceruleo/transformation/features/denoising.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,21 @@
 from sklearn.cluster import MiniBatchKMeans
 from ceruleo.transformation import TransformerStep
 
 
 class SavitzkyGolayTransformer(TransformerStep):
     """Filter each feature using LOESS
 
-    Parameters:    
+    Parameters:
         window: window size of the filter
         order:  Order of the filter, by default 2
         name: Step name
     """
 
     def __init__(self, window: int, order: int = 2, name: Optional[str] = None):
-
         super().__init__(name=name)
         self.window = window
         self.order = order
 
     def transform(self, X: pd.DataFrame, y=None) -> pd.DataFrame:
         """Return a new dataframe with the features filtered
 
@@ -62,24 +61,25 @@
     def __init__(
         self,
         window: int,
         center=True,
         min_periods: int = 15,
         name: Optional[str] = None,
     ):
-
         super().__init__(name=name)
         self.window = window
         self.min_periods = min_periods
         self.center = center
 
     def transform(self, X: pd.DataFrame, y=None) -> pd.DataFrame:
         return X.rolling(
-            self.window, min_periods=self.min_periods, center=self.center
-        ).mean(skip_na=True)
+            self.window,
+            min_periods=self.min_periods,
+            center=self.center,
+        ).mean(numeric_only=True)
 
 
 class MedianFilter(TransformerStep):
     """Filter each feature using a rolling median filter
 
     Parameters
     ----------
@@ -93,15 +93,17 @@
 
     def __init__(self, window: int, min_periods: int = 15, name: Optional[str] = None):
         super().__init__(name=name)
         self.window = window
         self.min_periods = min_periods
 
     def transform(self, X: pd.DataFrame, y=None) -> pd.DataFrame:
-        return X.rolling(self.window, min_periods=self.min_periods).median(skip_na=True)
+        return X.rolling(self.window, min_periods=self.min_periods).median(
+            numeric_only=True
+        )
 
 
 class OneDimensionalKMeans(TransformerStep):
     """Clusterize each feature into a number of clusters
 
     Parameters
     ----------
@@ -113,15 +115,17 @@
         super().__init__(name=name)
         self.clusters = {}
         self.n_clusters = n_clusters
 
     def partial_fit(self, X):
         if len(self.clusters) == 0:
             for c in X.columns:
-                self.clusters[c] = MiniBatchKMeans(n_clusters=self.n_clusters)
+                self.clusters[c] = MiniBatchKMeans(
+                    n_clusters=self.n_clusters, n_init="auto"
+                )
 
         for c in X.columns:
             self.clusters[c].partial_fit(np.atleast_2d(X[c]).T)
         return self
 
     def transform(self, X: pd.DataFrame, y=None) -> pd.DataFrame:
         """Transform the input dataframe
@@ -156,15 +160,15 @@
     name : Optional[str], optional
         Name of the step, by default None
     """
 
     def __init__(self, n_clusters: int = 5, name: Optional[str] = None):
         super().__init__(name=name)
         self.n_clusters = n_clusters
-        self.clusters = MiniBatchKMeans(n_clusters=self.n_clusters)
+        self.clusters = MiniBatchKMeans(n_clusters=self.n_clusters, n_init="auto")
 
     def partial_fit(self, X):
         self.clusters.partial_fit(X)
         return self
 
     def transform(self, X: pd.DataFrame, y=None) -> pd.DataFrame:
         """Transform the input life with the centroid information
@@ -199,15 +203,15 @@
     """
 
     def __init__(self, span: float, name: Optional[str] = None):
         super().__init__(name=name)
         self.span = span
 
     def transform(self, X: pd.DataFrame, y=None) -> pd.DataFrame:
-        return X.ewm(span=self.span).mean(skip_na=True)
+        return X.ewm(span=self.span, ignore_na=True).mean()
 
 
 class GaussianFilter(TransformerStep):
     """Apply a gaussian filter
 
     Parameters
     ----------
@@ -224,15 +228,15 @@
     def __init__(
         self,
         window_size: int,
         std: float,
         min_points: int = 1,
         center: bool = False,
         *args,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(**kwargs)
         self.window_size = window_size
         self.std = std
         self.center = center
         self.min_points = min_points
```

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/entropy.py` & `ceruleo-2.0.4/ceruleo/transformation/features/entropy.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/extraction.py` & `ceruleo-2.0.4/ceruleo/transformation/features/extraction.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 #    from temporis.transformation.features.hurst import hurst_exponent
 # except:
 #    pass
 from ceruleo.transformation import TransformerStep
 from ceruleo.transformation.features.rolling_windows import apply_rolling_data
 from ceruleo.transformation.functional.transformers import Transformer
 from ceruleo.transformation.utils import SKLearnTransformerWrapper
+from pandas.core.window.rolling import Rolling
+
 
 logger = logging.getLogger(__name__)
 
 
 class TimeToPreviousBinaryValue(TransformerStep):
     """Return a column with increasing number"""
 
@@ -240,18 +242,16 @@
             with 1 column
         """
         categories = sorted(list([c for c in self.categories if c is not None]))
         d = pd.Categorical(X[self.feature], categories=categories)
         return pd.DataFrame({"encoding": d.codes}, index=X.index)
 
 
-
-
 def rolling_kurtosis(s: pd.Series, window, min_periods):
-    return s.rolling(window, min_periods=min_periods).kurt(skipna=True)
+    return s.rolling(window, min_periods=min_periods).kurt(numeric_only=True)
 
 
 class LifeStatistics(TransformerStep):
     """Compute diverse number of features for each life.
 
     Returns a 1 row with the statistics computed for every feature
 
@@ -281,17 +281,16 @@
         'clearance', 'rms', 'shape', 'crest', 'hurst'
     name : Optional[str], optional
         Name of the step, by default None
 
     """
 
     def __init__(
-        self, *,to_compute: Optional[List[str]] = None, name: Optional[str] = None
+        self, *, to_compute: Optional[List[str]] = None, name: Optional[str] = None
     ):
-
         super().__init__(name=name)
         valid_stats = [
             "kurtosis",
             "skewness",
             "max",
             "min",
             "std",
@@ -455,15 +454,15 @@
             "std_atan",
             "std_acosh",
             "std_asinh",
             "energy",
         ]
 
         if to_compute is not None and specific is not None:
-            raise ValueError('Only one of to_compute or specific should be used')
+            raise ValueError("Only one of to_compute or specific should be used")
         self.specific = specific
         self.to_compute = to_compute
         if to_compute is None:
             if specific is None:
                 self.to_compute = valid_stats
             else:
                 self.specific = specific
@@ -479,104 +478,110 @@
         return self
 
     def fit(self, X, y=None):
         return self
 
     def _std_asinh(self, X, rolling, abs_rolling):
         return (
-            X.apply(np.arcsinh).rolling(self.window, self.min_points).std(skipna=True)
+            X.apply(np.arcsinh).rolling(self.window, self.min_points).std(numeric_only=True)
         )
 
     def _std_acosh(self, X, rolling, abs_rolling):
         return (
-            X.apply(np.arccosh).rolling(self.window, self.min_points).std(skipna=True)
+            X.apply(np.arccosh).rolling(self.window, self.min_points).std(numeric_only=True)
         )
 
     def _energy(self, X, rolling, abs_rolling):
         return X.pow(2).rolling(self.window, self.min_points).sum()
 
     def _std_atan(self, X, rolling, abs_rolling):
-        return X.apply(np.arctan).rolling(self.window, self.min_points).std(skipna=True)
+        return (
+            X.apply(np.arctan)
+            .rolling(self.window, self.min_points)
+            .std(numeric_only=True)
+        )
 
-    def _mean(self, X, rolling, abs_rolling):
-        return rolling.mean(skipna=True)
+    def _mean(self, X, rolling: Rolling, abs_rolling: Rolling):
+        return rolling.mean(numeric_only=True)
 
-    def _kurtosis(self, X, rolling, abs_rolling):
-        return rolling.kurt(skipna=True)
+    def _kurtosis(self, X, rolling: Rolling, abs_rolling: Rolling):
+        return rolling.kurt(numeric_only=True)
 
-    def _skewness(self, X, rolling, abs_rolling):
-        return rolling.skew(skipna=True)
+    def _skewness(self, X, rolling: Rolling, abs_rolling: Rolling):
+        return rolling.skew(numeric_only=True)
 
-    def _max(self, X, rolling, abs_rolling):
-        return rolling.max(skipna=True)
+    def _max(self, X, rolling: Rolling, abs_rolling: Rolling):
+        return rolling.max(numeric_only=True)
 
-    def _min(self, X, rolling, abs_rolling):
-        return rolling.min(skipna=True)
+    def _min(self, X, rolling: Rolling, abs_rolling: Rolling):
+        return rolling.min(numeric_only=True)
 
-    def _std(self, X, rolling, abs_rolling):
-        return rolling.std(skipna=True)
+    def _std(self, X, rolling: Rolling, abs_rolling: Rolling):
+        return rolling.std(numeric_only=True)
 
-    def _peak(self, X, rolling, abs_rolling):
-        return rolling.max(skipna=True) - rolling.min(skipna=True)
+    def _peak(self, X, rolling: Rolling, abs_rolling: Rolling):
+        return rolling.max(numeric_only=True) - rolling.min(numeric_only=True)
 
-    def _impulse(self, X, rolling, abs_rolling):
+    def _impulse(self, X, rolling: Rolling, abs_rolling: Rolling):
         return self._peak(X, rolling, abs_rolling) / abs_rolling.mean()
 
-    def _deviance(self, X, rolling, abs_rolling):
+    def _deviance(self, X, rolling: Rolling, abs_rolling: Rolling):
         return (X - rolling.mean()) / rolling.std()
 
-    def _clearance(self, X, rolling, abs_rolling):
+    def _clearance(self, X, rolling: Rolling, abs_rolling: Rolling):
         return self._peak(X, rolling, abs_rolling) / X.abs().pow(1.0 / 2).rolling(
             self.window, self.min_points
         ).mean().pow(2)
 
-    def _rms(self, X, rolling, abs_rolling):
+    def _rms(self, X, rolling: Rolling, abs_rolling: Rolling):
         return (
             X.pow(2)
             .rolling(self.window, self.min_points)
-            .mean(skipna=True)
+            .mean(numeric_only=True)
             .pow(1 / 2.0)
         )
 
-    def _shape(self, X, rolling, abs_rolling):
-        return self._rms(X, rolling, abs_rolling) / abs_rolling.mean(skipna=True)
+    def _shape(self, X, rolling: Rolling, abs_rolling: Rolling):
+        return self._rms(X, rolling, abs_rolling) / abs_rolling.mean(numeric_only=True)
 
     def _crest(self, X, rolling, abs_rolling):
         return self._peak(X, rolling, abs_rolling) / self._rms(X, rolling, abs_rolling)
 
-    def _compute_column_names(self, X:pd.DataFrame):
+    def _compute_column_names(self, X: pd.DataFrame):
         columns = []
         if self.to_compute is not None:
             for stats in self.to_compute:
                 for c in X.columns:
                     columns.append(f"{c}_{stats}")
         else:
             for c in self.specific.keys():
                 for stats in self.specific[c]:
                     columns.append(f"{c}_{stats}")
-        return columns 
-
-    def _transform_all_features(self, X:pd.DataFrame, X_new:pd.DataFrame, rolling, abs_rolling):
+        return columns
 
+    def _transform_all_features(
+        self, X: pd.DataFrame, X_new: pd.DataFrame, rolling, abs_rolling
+    ):
         for stats in self.to_compute:
             columns_to_assign = [f"{c}_{stats}" for c in X.columns]
             out = getattr(self, f"_{stats}")(X, rolling, abs_rolling)
             X_new.loc[:, columns_to_assign] = out.values
 
-
-    def _transform_specific(self,  X:pd.DataFrame, X_new:pd.DataFrame, rolling, abs_rolling):
+    def _transform_specific(
+        self, X: pd.DataFrame, X_new: pd.DataFrame, rolling, abs_rolling
+    ):
         for c in self.specific.keys():
-            for stats in self.specific[c]: 
+            for stats in self.specific[c]:
                 feature = f"{c}_{stats}"
                 out = getattr(self, f"_{stats}")(X[c], rolling[c], abs_rolling[c])
                 X_new.loc[:, feature] = out.values
 
-    def transform(self, X:pd.DataFrame):
+    def transform(self, X: pd.DataFrame):
         columns = self._compute_column_names(X)
-        
+
         X_new = pd.DataFrame(index=X.index, columns=columns)
         rolling = X.rolling(self.window, self.min_points)
         abs_rolling = X.abs().rolling(self.window, self.min_points)
         if self.to_compute is not None:
             self._transform_all_features(X, X_new, rolling, abs_rolling)
         else:
             self._transform_specific(X, X_new, rolling, abs_rolling)
@@ -615,15 +620,20 @@
         'clearance', 'rms', 'shape', 'crest', 'hurst'
     name : Optional[str], optional
         Name of the step, by default None
 
     """
 
     def __init__(
-        self, *, min_points=2, to_compute: List[str] = None, specific: Optional[Dict[str, List[str]]] = None, name: Optional[str] = None
+        self,
+        *,
+        min_points=2,
+        to_compute: List[str] = None,
+        specific: Optional[Dict[str, List[str]]] = None,
+        name: Optional[str] = None,
     ):
         super().__init__(name=name)
         self.min_points = min_points
         valid_stats = [
             "kurtosis",
             "skewness",
             "max",
@@ -638,20 +648,17 @@
             "mean",
             "deviance",
             "std_atan",
             "energy",
             "std_acosh",
             "std_asinh",
         ]
-        not_default = [
-            'energy',
-            'deviance'
-        ]
+        not_default = ["energy", "deviance"]
         if to_compute is not None and specific is not None:
-            raise ValueError('Only one of to_compute or specific should be used')
+            raise ValueError("Only one of to_compute or specific should be used")
         self.specific = specific
         self.to_compute = to_compute
         if to_compute is None:
             if specific is None:
                 self.to_compute = list(set(valid_stats) - set(not_default))
             else:
                 self.specific = specific
@@ -673,105 +680,105 @@
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return x.apply(np.arcsinh).expanding(self.min_points).std(skipna=True)
+        return x.apply(np.arcsinh).expanding(self.min_points).std(numeric_only=True)
 
     def _std_acosh(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return x.apply(np.arccosh).expanding(self.min_points).std(skipna=True)
+        return x.apply(np.arccosh).expanding(self.min_points).std(numeric_only=True)
 
     def _energy(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return x.pow(2).expanding(self.min_points).sum(skipna=True)
+        return x.pow(2).expanding(self.min_points).sum(numeric_only=True)
 
     def _std_atan(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return x.apply(np.arctan).expanding(self.min_points).std(skipna=True)
+        return x.apply(np.arctan).expanding(self.min_points).std(numeric_only=True)
 
     def _kurtosis(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return s.kurt(skipna=True)
+        return s.kurt(numeric_only=True)
 
     def _skewness(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return s.skew(skipna=True)
+        return s.skew(numeric_only=True)
 
     def _max(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return s.max(skipna=True)
+        return s.max(numeric_only=True)
 
     def _min(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return s.min(skipna=True)
+        return s.min(numeric_only=True)
 
     def _std(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return s.std(skipna=True)
+        return s.std(numeric_only=True)
 
     def _peak(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return s.max(skipna=True) - s.min(skipna=True)
+        return s.max(numeric_only=True) - s.min(numeric_only=True)
 
     def _impulse(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
@@ -783,15 +790,15 @@
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return (x - s.mean(skipna=True)) / (s.std(skipna=True) + 0.00000000001)
+        return (x - s.mean(numeric_only=True)) / (s.std(numeric_only=True) + 0.00000000001)
 
     def _clearance(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
@@ -813,83 +820,82 @@
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return s_sq.mean(skipna=True).pow(1 / 2.0)
+        return s_sq.mean(numeric_only=True).pow(1 / 2.0)
 
     def _mean(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return s.mean(skipna=True)
+        return s.mean(numeric_only=True)
 
     def _shape(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
-        return self._rms(x, s, s_abs, s_abs_sqrt, s_sq) / s_abs.mean(skipna=True)
+        return self._rms(x, s, s_abs, s_abs_sqrt, s_sq) / s_abs.mean(numeric_only=True)
 
     def _crest(
         self,
         x: pd.Series,
         s: Expanding,
         s_abs: Expanding,
         s_abs_sqrt: Expanding,
         s_sq: Expanding,
     ):
         return self._peak(x, s, s_abs, s_abs_sqrt, s_sq) / self._rms(
             x, s, s_abs, s_abs_sqrt, s_sq
         )
 
-
-    def _compute_column_names(self, X:pd.DataFrame):
+    def _compute_column_names(self, X: pd.DataFrame):
         columns = []
         if self.to_compute is not None:
             for stats in self.to_compute:
                 for c in X.columns:
                     columns.append(f"{c}_{stats}")
         else:
             for c in self.specific.keys():
                 for stats in self.specific[c]:
                     columns.append(f"{c}_{stats}")
-        return columns 
-
-    def _transform_all_features(self, X:pd.DataFrame, X_new:pd.DataFrame, expanding, s_abs, s_abs_sqrt, s_sq):
+        return columns
 
+    def _transform_all_features(
+        self, X: pd.DataFrame, X_new: pd.DataFrame, expanding, s_abs, s_abs_sqrt, s_sq
+    ):
         for stats in self.to_compute:
             columns_to_assign = [f"{c}_{stats}" for c in X.columns]
-            out = getattr(self, f"_{stats}")(
-                    X, expanding, s_abs, s_abs_sqrt, s_sq
-                )
+            out = getattr(self, f"_{stats}")(X, expanding, s_abs, s_abs_sqrt, s_sq)
             X_new.loc[:, columns_to_assign] = out.values
 
-
-    def _transform_specific(self,  X:pd.DataFrame, X_new:pd.DataFrame, expanding, s_abs, s_abs_sqrt, s_sq):
+    def _transform_specific(
+        self, X: pd.DataFrame, X_new: pd.DataFrame, expanding, s_abs, s_abs_sqrt, s_sq
+    ):
         for c in self.specific.keys():
-            for stats in self.specific[c]: 
+            for stats in self.specific[c]:
                 feature = f"{c}_{stats}"
                 out = getattr(self, f"_{stats}")(
                     X[c], expanding[c], s_abs[c], s_abs_sqrt[c], s_sq[c]
                 )
                 X_new.loc[:, feature] = out.values
 
-    def transform(self, X:pd.DataFrame):
+    def transform(self, X: pd.DataFrame):
         columns = self._compute_column_names(X)
-        
+
         X_new = pd.DataFrame(index=X.index, columns=columns)
         expanding = X.expanding(self.min_points)
         s_abs = X.abs().expanding(self.min_points)
         s_abs_sqrt = X.abs().pow(1.0 / 2).expanding(self.min_points)
         s_sq = X.pow(2).expanding(self.min_points)
         if self.to_compute is not None:
             self._transform_all_features(X, X_new, expanding, s_abs, s_abs_sqrt, s_sq)
@@ -902,15 +908,15 @@
     """Compute the difference between two set of features
 
     Example:
 
         X[features1] - X[features2]
 
     Parameters
-    
+
         feature_set1: Feature list of the first group to substract
         feature_set2:Feature list of the second group to substract
         name: Name of the step, by default None
 
     """
 
     def __init__(
@@ -1010,27 +1016,29 @@
 
     Parameters
     ----------
     n: int
        Number of
     """
 
-    def __init__(self, *, n: int, min_imf:int, max_imf:int, name: Optional[str] = "EMD"):
+    def __init__(
+        self, *, n: int, min_imf: int, max_imf: int, name: Optional[str] = "EMD"
+    ):
         super().__init__(name=name)
         self.n = n
         self.min_imf = min_imf
         self.max_imf = max_imf
 
     def transform(self, X):
         new_X = pd.DataFrame(index=X.index)
 
         for c in X.columns:
             try:
                 imf = emd.sift.sift(X[c].values, max_imfs=self.n)
-                new_X[c] = np.sum(imf[:, self.min_imf:self.max_imf], axis=1)
+                new_X[c] = np.sum(imf[:, self.min_imf : self.max_imf], axis=1)
             except Exception as e:
                 new_X[c] = X[c]
 
         return new_X
 
 
 class ChangesDetector(TransformerStep):
```

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/extraction_frequency.py` & `ceruleo-2.0.4/ceruleo/transformation/features/extraction_frequency.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/hurst.py` & `ceruleo-2.0.4/ceruleo/transformation/features/hurst.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/imputers.py` & `ceruleo-2.0.4/ceruleo/transformation/features/imputers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/outliers.py` & `ceruleo-2.0.4/ceruleo/transformation/features/outliers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/resamplers.py` & `ceruleo-2.0.4/ceruleo/transformation/features/resamplers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/rolling_windows.py` & `ceruleo-2.0.4/ceruleo/transformation/features/rolling_windows.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/scalers.py` & `ceruleo-2.0.4/ceruleo/transformation/features/scalers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/selection.py` & `ceruleo-2.0.4/ceruleo/transformation/features/selection.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/slicing.py` & `ceruleo-2.0.4/ceruleo/transformation/features/slicing.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/split.py` & `ceruleo-2.0.4/ceruleo/transformation/features/split.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/tdigest.py` & `ceruleo-2.0.4/ceruleo/transformation/features/tdigest.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/features/transformation.py` & `ceruleo-2.0.4/ceruleo/transformation/features/transformation.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/functional/concatenate.py` & `ceruleo-2.0.4/ceruleo/transformation/functional/concatenate.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/functional/graph_utils.py` & `ceruleo-2.0.4/ceruleo/transformation/functional/graph_utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/functional/mixin.py` & `ceruleo-2.0.4/ceruleo/transformation/functional/mixin.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/functional/pipeline/cache_store.py` & `ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/cache_store.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/functional/pipeline/pipeline.py` & `ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/functional/pipeline/runner.py` & `ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/runner.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/functional/pipeline/traversal.py` & `ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/traversal.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/functional/pipeline/utils.py` & `ceruleo-2.0.4/ceruleo/transformation/functional/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/functional/transformers.py` & `ceruleo-2.0.4/ceruleo/transformation/functional/transformers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/functional/transformerstep.py` & `ceruleo-2.0.4/ceruleo/transformation/functional/transformerstep.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/transformation/target.py` & `ceruleo-2.0.4/ceruleo/transformation/target.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,127 +1,79 @@
-from typing import Optional
+from functools import partial
+from typing import List, Optional
 
 import numpy as np
 import pandas as pd
 from ceruleo.transformation import TransformerStep
+from pandas.api.types import is_timedelta64_dtype
+from scipy.stats import norm
 
 
 class TargetToClasses(TransformerStep):
-    def __init__(self, bins):
+    """Transform the RUL values into a discrete set of classes
+
+    Parameters
+        bins: Bins limits
+    """
+
+    def __init__(self, bins: List[float]):
         super().__init__()
         self.bins = bins
 
     def transform(self, X):
         X_new = pd.DataFrame(index=X.index)
         X_new["RUL_class"] = np.digitize(X.iloc[:, 0].values, self.bins, right=False)
         return X_new
 
 
-class HealthPercentage(TransformerStep):
-    def transform(self, X):
-        return (X / X.iloc[0, 0]) * 100
-
-
 class PicewiseRUL(TransformerStep):
     """Transform the RUL clipping the maximum value
 
     Parameters
-    ----------
-    max_life : float, optional
-        Maximum threshold for clipping the RUL values, by default np.inf
-    name : Optional[str], optional
-        Name of the step, by default None    """
+
+        max_life:  Maximum threshold for clipping the RUL values
+        name:  Name of the step, by default None
+    """
+
     def __init__(self, *, max_life: float = np.inf, name: Optional[str] = None):
         super().__init__(name=name)
         self.max_life = max_life
 
-    def transform(self, X):
-        """Clip the maximum value of the true RUL
-
-        Parameters
-        ----------
-        X : np.array
-            Vector with the true labels
-
-        Returns
-        -------
-        np.array
-            Cliiped RUL values
-        """
-        return np.clip(X, 0, self.max_life)
+    def transform(self, X: pd.DataFrame):
+        return X.clip(0, self.max_life)
 
 
 class PicewiseRULQuantile(PicewiseRUL):
-    """Transform the RUL clipping the maximum value using a quantile value as threshold
+    """Clip the RUL  values using a quantile value as threshold
 
     Parameters
-    ----------
-    quantile : float, optional
-        Value between 0 and 1 to compute the RUL threshold
-    name : Optional[str], optional
-        Name of the step, by default None    """
-    def __init__(self, quantile:float, name: Optional[str] = None):
+
+        quantile: Value between 0 and 1 to compute the RUL threshold
+        name: Name of the step
+    """
+
+    def __init__(self, quantile: float, name: Optional[str] = None):
         super().__init__(name)
         self.quantile = quantile
 
     def fit(self, X, y=None):
-        """Clip the maximum value of the true RUL
-
-        Parameters
-        ----------
-        X : np.array
-            Vector with the true labels
-
-        Returns
-        -------
-        np.array
-            Cliiped RUL values
-        """
         self.max_life = np.quantile(X, self.quantile)
         return self
 
 
 class RULBinarizer(TransformerStep):
-    def __init__(self, t:float, **kwargs):
-        super().__init__(**kwargs)
-        self.t = t       
-    
-
-    def transform(self, X):
-        return (X < self.t).astype('int')
+    """Convert the RUL target into a binary vector
 
+    Useful for determining point of failures.
 
 
-
-class RemoveGaps(TransformerStep):
-    """Gaps larger than a treshold are removed
-
     Parameters
-    ----------
-    max_life : float, optional
-        Maximum threshold for clipping the RUL values, by default np.inf
-    name : Optional[str], optional
-        Name of the step, by default None    """
-    def __init__(self, *, threshold: float, name: Optional[str] = None):
-        super().__init__(name=name)
-        self.threshold = threshold
+        t: Starting point of failure
+        Every sample with a RUL greater than t will be 1 and the rest 0
+    """
 
-    def transform(self, x:pd.DataFrame):
-        """Remove gaps in the RUL target
+    def __init__(self, t: float, **kwargs):
+        super().__init__(**kwargs)
+        self.t = t
 
-        Parameters
-        ----------
-        X : np.array
-            Vector with the true labels
-
-        Returns
-        -------
-        np.array
-            Cliiped RUL values
-        """
-
-        y = np.abs(np.diff(np.squeeze(x)))
-        y[y  <= self.threshold] = 0        
-        new_x  = np.squeeze(x.values) + np.hstack((0, np.cumsum(y)))
-        
-        return pd.DataFrame(new_x - np.min(new_x), index=x.index, columns=x.columns)
-        
+    def transform(self, X):
+        return (X > self.t).astype("int")
```

### Comparing `ceruleo-2.0.3/ceruleo/transformation/utils.py` & `ceruleo-2.0.4/ceruleo/transformation/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,37 +5,28 @@
 import pandas as pd
 from ceruleo.transformation import TransformerStep
 from ceruleo.transformation.features.tdigest import TDigest
 from sklearn.pipeline import FeatureUnion, _transform_one
 
 
 class PandasToNumpy(TransformerStep):
-    def fit(self, X, y=None):
-        return self
-
-    def partial_fit(self, X, y=None):
-        return self
-
     def transform(self, X):
         return X.values
 
 
 class TransformerLambda(TransformerStep):
     def __init__(self, f, name: Optional[str] = None):
         super().__init__(name)
         self.f = f
 
     def transform(self, X, y=None):
         return self.f(X)
 
 
 class IdentityTransformerStep(TransformerStep):
-    def fit(self, input_array, y=None):
-        return self
-
     def transform(self, input_array, y=None):
         if isinstance(input_array, pd.DataFrame):
             return input_array.copy()
         else:
             return input_array * 1
```

### Comparing `ceruleo-2.0.3/ceruleo/utils/download.py` & `ceruleo-2.0.4/ceruleo/utils/download.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/ceruleo/utils/lrucache.py` & `ceruleo-2.0.4/ceruleo/utils/lrucache.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/docs/dataset/Example.ipynb` & `ceruleo-2.0.4/docs/dataset/Example.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/docs/dataset/analysis/Sensor Validation.ipynb` & `ceruleo-2.0.4/docs/dataset/analysis/Sensor Validation.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/docs/dataset/analysis/sensor_validation.md` & `ceruleo-2.0.4/docs/dataset/analysis/sensor_validation.md`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/docs/dataset/catalog.md` & `ceruleo-2.0.4/docs/dataset/catalog.md`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/docs/images/cerulean.png` & `ceruleo-2.0.4/docs/images/cerulean.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/docs/images/unipd_logo.png` & `ceruleo-2.0.4/docs/images/unipd_logo.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/docs/img/duration_histogram.png` & `ceruleo-2.0.4/docs/img/duration_histogram.png`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/docs/index.md` & `ceruleo-2.0.4/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # CeRULEo
 
 ## Welcome tu CeRULEo
 
-Cool utilitiEs for Remaining Useful Life Estimation methOds
+CeRULEo: Comprehensive utilitiEs for Remaining Useful Life Estimation methOds
+
 
 ### Predictive Maintenance
 
 Efficient management of maintenance in modern industrial environments is having a major impact on decreasing costs associated with defective products and equipment inactivity. Therefore, it is critical for companies to develop an efficient and well-implemented maintenance strategy to prevent unexpected outages, improve overall reliability, and reduce operating costs  [@8748978].
 
 
 The evolution of information systems has transformed traditional manufacturing into factories equipped with intelligent sensors that allow better knowledge about what happens during industrial processes.  All the information collected can be used to optimize decision-making processes. The use of this information in maintenance processes has caused a transition from Preventive Maintenance (PM) techniques to Predictive Maintenance (PdM) methods [@damant2021exploring]. PM  is carried out regularly while the asset is still in a  working condition to prevent sudden breakdowns. In contrast, PdM can statistically assess the health status of a piece of equipment, allowing early detection of pending failures, and enabling timely pre-failure interventions, thanks to prediction models based on historical data. The data-driven methods use condition monitoring data acquired from sensors to provide effective solutions in these areas [@susto2014machine].
```

### Comparing `ceruleo-2.0.3/docs/iterators/Iterators.ipynb` & `ceruleo-2.0.4/docs/iterators/Iterators.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/docs/iterators/iterators.md` & `ceruleo-2.0.4/docs/iterators/iterators.md`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/docs/models/Models_sklearn.ipynb` & `ceruleo-2.0.4/docs/models/Models_sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/docs/models/models_tf.ipynb` & `ceruleo-2.0.4/docs/models/models_tf.ipynb`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/docs/refs.bib` & `ceruleo-2.0.4/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/mkdocs.yml` & `ceruleo-2.0.4/mkdocs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -63,17 +63,14 @@
         - Imputers: transformation/features/imputers.md
         - Resamplers: transformation/features/resamplers.md
         - Resamplers: transformation/features/selection.md
         - Outliers: transformation/features/outliers.md
     - Results:
       - Results: results/results.md
       - Visualization: results/visualization.md
-    - Guides:
-      - Complete: guides/guide.ipynb
-      
     
 
 
 plugins:
 - search
 - mkdocstrings:
     handlers:
```

### Comparing `ceruleo-2.0.3/pyproject.toml` & `ceruleo-2.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,60 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "ceruleo"
 description = "Remaining useful life estimation utilities"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["predictive maintenance", "remaining useful life"]
 license = {text = "MIT"}
+dynamic = ["version"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
 dependencies = [
-        "pandas",
-        "numpy",
-        "tqdm",
-        "scikit-learn",
-        "gwpy",
-        "emd",
-        "dill",
-        "mmh3",
-        "pyarrow",
-        "fastparquet",
-        "sphinxcontrib.bibtex",
-        "gdown",
-        "uncertainties",
-        "pyinform",
-        "pyts",
-        "PyWavelets",
-        "seaborn",
-        "antropy"
-
+        "pandas >= 1.5",
+        "numpy >= 1.22",
+        "tqdm >= 4.56",
+        "scikit-learn >= 0.24",
+        "emd >= 0.4",
+        "mmh3   >= 2.0",
+        "pyarrow >= 4",
+        "gdown >= 4.2",
+        "pyinform >= 0.2",
+        "pyts >= 0.12",
+        "seaborn >= 0.11",
+        "antropy >= 0.1",
+        "uncertainties >= 3.1",
+        "PyWavelets >= 1.3",
 ]
-dynamic = ["version"]
 
-[project.optional-dependencies]
-doc = ["mkdocs"]
+
+[tool.hatch.version]
+path = "ceruleo/__init__.py"
 
 
+[project.urls]
+Homepage = "https://github.com/lucianolorenti/ceruleo"
+Documentation = "https://lucianolorenti.github.io/ceruleo/"
+
+[project.optional-dependencies]
+tensorflow = ["tensorflow >= 2.5"]
+
+test = [
+    "pytest",
+    "coverage",
+    "xgboost >= 1.5"
+]
+doc = [
+    "mkdocs", 
+    "mkdocstrings[python]",
+    "mkdocs-material",
+    "mkdocs-jupyter",
+    "jupyter_contrib_nbextensions",
+    "mkdocstrings",
+    "mkdocs-bibtex",
+    "sphinxcontrib.bibtex"
+]
```

### Comparing `ceruleo-2.0.3/tests/manual_features.py` & `ceruleo-2.0.4/tests/manual_features.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/tests/test_analysis.py` & `ceruleo-2.0.4/tests/test_analysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,14 +34,42 @@
         return "RUL"
 
     @property
     def n_time_series(self):
         return len(self.lives)
 
 
+class MockDatasetTimeDeltaIndex(AbstractTimeSeriesDataset):
+    def __init__(self, nlives: int):
+        super().__init__()
+        self.lives = [
+            pd.DataFrame(
+                {
+                    "feature1": np.linspace(0, 100, 50),
+                    "feature2": np.random.randint(2, size=(50,)),
+                    "RUL": np.linspace(100, 0, 50),
+                },
+                index=pd.timedelta_range(start='0 day', periods=50, freq='s')
+            )
+            for i in range(nlives)
+        ]
+
+    def get_time_series(self, i: int):
+        return self.lives[i]
+
+    @property
+    def rul_column(self):
+        return "RUL"
+
+    @property
+    def n_time_series(self):
+        return len(self.lives)
+
+
+
 class TestAnalysis:
     def test_correlation(self):
         ds = MockDataset(5)
         assert isinstance(correlation_analysis(ds), pd.DataFrame)
 
         transformer = Transformer(
             pipelineX=ByNameFeatureSelector(features=['feature1', 'feature2']), 
@@ -54,14 +82,22 @@
     def test_samplerate(self):
         dataset = MockDataset(5)
         sample_rates = sample_rate(dataset)
         assert isinstance(sample_rates, np.ndarray)
 
         assert isinstance(sample_rate_summary(dataset), pd.DataFrame)
 
+        dataset = MockDatasetTimeDeltaIndex(5)
+
+        sample_rates = sample_rate(dataset)
+        assert isinstance(sample_rates, np.ndarray)
+
+        assert isinstance(sample_rate_summary(dataset), pd.DataFrame)
+
+
     def test_distribution(self):
         dataset = MockDataset(5)
         assert isinstance(features_divergeces(dataset), pd.DataFrame)
 
     def test_analysis(self):
         dataset = MockDataset(5)
         df = analysis(dataset)
```

### Comparing `ceruleo-2.0.3/tests/test_batcher.py` & `ceruleo-2.0.4/tests/test_batcher.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/tests/test_dataset.py` & `ceruleo-2.0.4/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/tests/test_denoising.py` & `ceruleo-2.0.4/tests/test_denoising.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/tests/test_graph.py` & `ceruleo-2.0.4/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/tests/test_imputers.py` & `ceruleo-2.0.4/tests/test_imputers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/tests/test_iterators.py` & `ceruleo-2.0.4/tests/test_iterators.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/tests/test_lrucache.py` & `ceruleo-2.0.4/tests/test_lrucache.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/tests/test_models.py` & `ceruleo-2.0.4/tests/test_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,49 @@
+from pathlib import Path
+
 import numpy as np
 import pandas as pd
 import tensorflow as tf
 from ceruleo.dataset.ts_dataset import AbstractTimeSeriesDataset
 from ceruleo.iterators.iterators import WindowedDatasetIterator
 from ceruleo.iterators.shufflers import AllShuffled
 from ceruleo.iterators.utils import true_values
 from ceruleo.models.baseline import BaselineModel, FixedValueBaselineModel
+from ceruleo.models.keras.callbacks import PredictionCallback
 from ceruleo.models.keras.catalog.CNLSTM import CNLSTM
 from ceruleo.models.keras.catalog.InceptionTime import InceptionTime
 from ceruleo.models.keras.catalog.MSWRLRCN import MSWRLRCN
-from ceruleo.models.keras.catalog.MultiScaleConvolutional import \
-    MultiScaleConvolutionalModel
+from ceruleo.models.keras.catalog.MultiScaleConvolutional import (
+    MultiScaleConvolutionalModel,
+)
 from ceruleo.models.keras.catalog.XCM import XCM, explain
-from ceruleo.models.keras.catalog.XiangQiangJianQiao import \
-    XiangQiangJianQiaoModel
+from ceruleo.models.keras.catalog.XiangQiangJianQiao import XiangQiangJianQiaoModel
 from ceruleo.models.keras.dataset import tf_regression_dataset
-from ceruleo.models.sklearn import (CeruleoRegressor, EstimatorWrapper,
-                                    TimeSeriesWindowTransformer, predict,
-                                    train_model)
+from ceruleo.models.keras.losses import (
+    AsymmetricLossPM,
+    asymmetric_loss_pm,
+    relative_mae,
+    relative_mse,
+    root_mean_squared_error,
+)
+from ceruleo.models.sklearn import (
+    CeruleoRegressor,
+    EstimatorWrapper,
+    TimeSeriesWindowTransformer,
+    predict,
+    train_model,
+)
 from ceruleo.transformation import Transformer
 from ceruleo.transformation.features.scalers import MinMaxScaler
 from ceruleo.transformation.features.selection import ByNameFeatureSelector
 from numpy.random import seed
 from sklearn.linear_model import LinearRegression
 from sklearn.pipeline import make_pipeline
 from tensorflow.keras import Input, Model
-from tensorflow.keras.layers import Dense, Dropout, Flatten
+from tensorflow.keras.layers import Dense, Flatten
 from xgboost import XGBRegressor
 
 seed(1)
 
 
 tf.random.set_seed(2)
 
@@ -88,14 +102,21 @@
         return "RUL"
 
     @property
     def n_time_series(self):
         return len(self.lives)
 
 
+def _test_model_basic(model, ds_iterator, loss="mae"):
+    model.compile(loss=loss, optimizer=tf.keras.optimizers.SGD(0.0001))
+    model.fit(tf_regression_dataset(ds_iterator).batch(15), verbose=False)
+    y_pred = model.predict(tf_regression_dataset(ds_iterator).batch(15)).ravel()
+    assert isinstance(y_pred, np.ndarray)
+
+
 class TestModels:
     def test_models(self):
         features = ["feature1", "feature2"]
         x = ByNameFeatureSelector(features=features)
         x = MinMaxScaler(range=(-1, 1))(x)
 
         y = ByNameFeatureSelector(features=["RUL"])
@@ -224,93 +245,163 @@
         ds = MockDataset(5)
         transformer.fit(ds)
         transformed_ds = ds.map(transformer)
         ds_iterator = WindowedDatasetIterator(
             transformed_ds, window_size=5, step=2, shuffler=AllShuffled()
         )
 
-        def test_model_basic(model):
-            model.compile(loss="mae", optimizer=tf.keras.optimizers.SGD(0.0001))
-            model.fit(tf_regression_dataset(ds_iterator).batch(15), verbose=False)
-            y_pred = model.predict(tf_regression_dataset(ds_iterator).batch(15)).ravel()
-            assert isinstance(y_pred, np.ndarray)
-
         model = CNLSTM(
             ds_iterator.shape,
             n_conv_layers=2,
             initial_convolutional_size=5,
             layers_recurrent=[5, 5],
             hidden_size=(15, 5),
             dropout=0.3,
         )
-        test_model_basic(model)
+        _test_model_basic(model, ds_iterator)
 
         model = InceptionTime(
             ds_iterator.shape,
             nb_filters=3,
         )
-        test_model_basic(model)
+        _test_model_basic(model, ds_iterator)
 
         model = MSWRLRCN(ds_iterator.shape)
-        test_model_basic(model)
+        _test_model_basic(model, ds_iterator)
 
         model = MultiScaleConvolutionalModel(
             ds_iterator.shape, n_msblocks=1, scales=[2, 3], n_hidden=5
         )
-        test_model_basic(model)
+        _test_model_basic(model, ds_iterator)
 
         model = XiangQiangJianQiaoModel(ds_iterator.shape)
-        test_model_basic(model)
+        _test_model_basic(model, ds_iterator)
 
         model, model_extras = XCM(ds_iterator.shape)
-        test_model_basic(model)
+        _test_model_basic(model, ds_iterator)
         X, y, sw = next(iter(ds_iterator))
         (mmap, v) = explain(model_extras, X)
         print(type(mmap))
         assert isinstance(mmap, np.ndarray)
-    
+
     def test_baseline(self):
         ds = MockDataset(5)
         features = ["feature1", "feature2"]
 
         x = ByNameFeatureSelector(features=features)
         x = MinMaxScaler(range=(-1, 1))(x)
 
         y = ByNameFeatureSelector(features=["RUL"])
         transformer = Transformer(x, y)
 
         transformer.fit(ds)
         transformed_ds = ds.map(transformer)
 
-
-        model_mean = BaselineModel(mode='mean')
+        model_mean = BaselineModel(mode="mean")
         model_mean.fit(ds)
         y_pred = model_mean.predict(ds)
         assert isinstance(y_pred, np.ndarray)
 
-        model_median = BaselineModel(mode='median')
+        model_median = BaselineModel(mode="median")
         model_median.fit(ds)
         y_pred = model_mean.predict(ds)
         assert isinstance(y_pred, np.ndarray)
 
-
         model_fixed = FixedValueBaselineModel(value=100)
         model_fixed.fit(ds)
         y_pred = model_mean.predict(ds)
         assert isinstance(y_pred, np.ndarray)
 
-        model_mean = BaselineModel(mode='mean')
+        model_mean = BaselineModel(mode="mean")
         model_mean.fit(transformed_ds)
         y_pred = model_mean.predict(transformed_ds)
         assert isinstance(y_pred, np.ndarray)
 
-        model_median = BaselineModel(mode='median')
+        model_median = BaselineModel(mode="median")
         model_median.fit(transformed_ds)
         y_pred = model_mean.predict(transformed_ds)
         assert isinstance(y_pred, np.ndarray)
 
-
         model_fixed = FixedValueBaselineModel(value=100)
         model_fixed.fit(transformed_ds)
         y_pred = model_mean.predict(transformed_ds)
         assert isinstance(y_pred, np.ndarray)
 
+    def test_callbacks(self):
+        features = ["feature1", "feature2"]
+
+        x = ByNameFeatureSelector(features=features)
+        x = MinMaxScaler(range=(-1, 1))(x)
+
+        y = ByNameFeatureSelector(features=["RUL"])
+        transformer = Transformer(x, y)
+
+        ds = MockDataset(5)
+        transformer.fit(ds)
+        transformed_ds = ds.map(transformer)
+        ds_iterator = WindowedDatasetIterator(
+            transformed_ds, window_size=5, step=2, shuffler=AllShuffled()
+        )
+        model = MultiScaleConvolutionalModel(
+            ds_iterator.shape, n_msblocks=1, scales=[2, 3], n_hidden=5
+        )
+        model.compile(loss="mae", optimizer=tf.keras.optimizers.SGD(0.0001))
+
+        tf_dataset = tf_regression_dataset(ds_iterator).batch(15)
+        output_path = Path(".").resolve() / "output.png"
+        model.fit(
+            tf_dataset,
+            callbacks=[PredictionCallback(output_path, tf_dataset)],
+            verbose=False,
+        )
+
+        assert output_path.is_file()
+
+    def test_losses(self):
+        features = ["feature1", "feature2"]
+
+        x = ByNameFeatureSelector(features=features)
+        x = MinMaxScaler(range=(-1, 1))(x)
+
+        y = ByNameFeatureSelector(features=["RUL"])
+        transformer = Transformer(x, y)
+
+        ds = MockDataset(5)
+        transformer.fit(ds)
+        transformed_ds = ds.map(transformer)
+        ds_iterator = WindowedDatasetIterator(
+            transformed_ds, window_size=5, step=2, shuffler=AllShuffled()
+        )
+        model = MultiScaleConvolutionalModel(
+            ds_iterator.shape, n_msblocks=1, scales=[2, 3], n_hidden=5
+        )
+        _test_model_basic(
+            model,
+            ds_iterator,
+            loss=AsymmetricLossPM(
+                theta_l=1, alpha_l=1, gamma_l=1, theta_r=1, alpha_r=1, gamma_r=1
+            ),
+        )
+
+        _test_model_basic(model, ds_iterator, loss=root_mean_squared_error)
+
+        _test_model_basic(model, ds_iterator, loss=relative_mae(C=0.5))
+
+        _test_model_basic(model, ds_iterator, loss=relative_mse(C=0.5))
+
+        print(type(root_mean_squared_error(tf.random.uniform((50,)), tf.random.uniform((50,))).numpy()))
+        assert isinstance(
+            root_mean_squared_error(tf.random.uniform((50,)), tf.random.uniform((50,))).numpy(), np.float32
+        )
+        assert isinstance(
+            asymmetric_loss_pm(
+                tf.random.uniform((50,)),
+                tf.random.uniform((50,)),
+                theta_l=1,
+                alpha_l=1,
+                gamma_l=1,
+                theta_r=1,
+                alpha_r=1,
+                gamma_r=1,
+            ).numpy(),
+            np.float32,
+        )
```

### Comparing `ceruleo-2.0.3/tests/test_operations.py` & `ceruleo-2.0.4/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/tests/test_pipeline.py` & `ceruleo-2.0.4/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/tests/test_results.py` & `ceruleo-2.0.4/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/tests/test_scalers.py` & `ceruleo-2.0.4/tests/test_scalers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/tests/test_shufflers.py` & `ceruleo-2.0.4/tests/test_shufflers.py`

 * *Files identical despite different names*

### Comparing `ceruleo-2.0.3/tests/test_transformers.py` & `ceruleo-2.0.4/tests/test_transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from curses import window
 from typing import List, Optional
 
 import numpy as np
 import pandas as pd
 import pytest
 import scipy.stats
+
 from ceruleo.dataset.ts_dataset import AbstractTimeSeriesDataset
 from ceruleo.transformation.features.entropy import LocalEntropyMeasures
 from ceruleo.transformation.features.extraction import (
     EMD,
     ChangesDetector,
     Difference,
     ExpandingStatistics,
@@ -16,16 +16,16 @@
     RollingStatistics,
     SimpleEncodingCategorical,
     SlidingNonOverlappingEMD,
 )
 from ceruleo.transformation.features.outliers import (
     EWMAOutOfRange,
     IQROutlierRemover,
-    ZScoreOutlierRemover,
     IsolationForestOutlierRemover,
+    ZScoreOutlierRemover,
 )
 from ceruleo.transformation.features.resamplers import IntegerIndexResamplerTransformer
 from ceruleo.transformation.features.selection import (
     ByNameFeatureSelector,
     NullProportionSelector,
 )
 from ceruleo.transformation.features.transformation import Accumulate
@@ -354,15 +354,15 @@
             }
         )
         df_gt = pd.DataFrame(
             {"feature1": [1, 0, 0, 1, 0, 1, 0, 1], "feature2": [1, 0, 1, 0, 1, 0, 0, 0]}
         )
         t = ChangesDetector()
         df1 = t.fit_transform(df).astype("int")
-        assert df1.equals(df_gt)
+        assert df1.compare(df_gt).empty
 
     def test_Accumulate(self):
         df = pd.DataFrame(
             {"a": [1, 2, 3, 4], "b": [2, 4, 6, 8], "c": [2, 2, 2, 2], "d": [1, 0, 1, 0]}
         )
         transformer = Accumulate()
         df_new = transformer.fit_transform(df)
```

### Comparing `ceruleo-2.0.3/tests/test_utils.py` & `ceruleo-2.0.4/tests/test_utils.py`

 * *Files identical despite different names*

