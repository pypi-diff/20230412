# Comparing `tmp/etna-1.9.0.tar.gz` & `tmp/etna-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etna-1.9.0.tar", max compression
+gzip compressed data, was "etna-2.0.0.tar", max compression
```

## Comparing `etna-1.9.0.tar` & `etna-2.0.0.tar`

### file list

```diff
@@ -1,124 +1,197 @@
--rw-r--r--   0        0        0    11244 2022-05-17 08:36:34.920591 etna-1.9.0/LICENSE
--rw-r--r--   0        0        0    11425 2022-05-17 08:36:34.920591 etna-1.9.0/README.md
--rw-r--r--   0        0        0       49 2022-05-17 08:36:34.924591 etna-1.9.0/etna/__init__.py
--rw-r--r--   0        0        0     2515 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/__init__.py
--rw-r--r--   0        0        0       72 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/change_points_trend/__init__.py
--rw-r--r--   0        0        0     2118 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/change_points_trend/search.py
--rw-r--r--   0        0        0    26338 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/eda_utils.py
--rw-r--r--   0        0        0      399 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/feature_relevance/__init__.py
--rw-r--r--   0        0        0     3114 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/feature_relevance/relevance.py
--rw-r--r--   0        0        0     3962 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/feature_relevance/relevance_table.py
--rw-r--r--   0        0        0      213 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/feature_selection/__init__.py
--rw-r--r--   0        0        0     3870 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/feature_selection/mrmr_selection.py
--rw-r--r--   0        0        0      393 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/outliers/__init__.py
--rw-r--r--   0        0        0     4879 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/outliers/density_outliers.py
--rw-r--r--   0        0        0    13173 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/outliers/hist_outliers.py
--rw-r--r--   0        0        0     1721 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/outliers/median_outliers.py
--rw-r--r--   0        0        0     3024 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/outliers/prediction_interval_outliers.py
--rw-r--r--   0        0        0    54088 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/plotters.py
--rw-r--r--   0        0        0      707 2022-05-17 08:36:34.924591 etna-1.9.0/etna/analysis/utils.py
--rw-r--r--   0        0        0      524 2022-05-17 08:36:34.924591 etna-1.9.0/etna/clustering/__init__.py
--rw-r--r--   0        0        0      686 2022-05-17 08:36:34.924591 etna-1.9.0/etna/clustering/base.py
--rw-r--r--   0        0        0      259 2022-05-17 08:36:34.924591 etna-1.9.0/etna/clustering/distances/__init__.py
--rw-r--r--   0        0        0     3758 2022-05-17 08:36:34.924591 etna-1.9.0/etna/clustering/distances/base.py
--rw-r--r--   0        0        0     4508 2022-05-17 08:36:34.924591 etna-1.9.0/etna/clustering/distances/distance_matrix.py
--rw-r--r--   0        0        0     5597 2022-05-17 08:36:34.924591 etna-1.9.0/etna/clustering/distances/dtw_distance.py
--rw-r--r--   0        0        0     1704 2022-05-17 08:36:34.924591 etna-1.9.0/etna/clustering/distances/euclidean_distance.py
--rw-r--r--   0        0        0      289 2022-05-17 08:36:34.924591 etna-1.9.0/etna/clustering/hierarchical/__init__.py
--rw-r--r--   0        0        0     6020 2022-05-17 08:36:34.924591 etna-1.9.0/etna/clustering/hierarchical/base.py
--rw-r--r--   0        0        0     1501 2022-05-17 08:36:34.924591 etna-1.9.0/etna/clustering/hierarchical/dtw_clustering.py
--rw-r--r--   0        0        0     1561 2022-05-17 08:36:34.924591 etna-1.9.0/etna/clustering/hierarchical/euclidean_clustering.py
--rw-r--r--   0        0        0      374 2022-05-17 08:36:34.924591 etna-1.9.0/etna/commands/__init__.py
--rw-r--r--   0        0        0      197 2022-05-17 08:36:34.924591 etna-1.9.0/etna/commands/__main__.py
--rw-r--r--   0        0        0     3074 2022-05-17 08:36:34.924591 etna-1.9.0/etna/commands/backtest_command.py
--rw-r--r--   0        0        0     3383 2022-05-17 08:36:34.924591 etna-1.9.0/etna/commands/forecast_command.py
--rw-r--r--   0        0        0      281 2022-05-17 08:36:34.924591 etna-1.9.0/etna/commands/resolvers.py
--rw-r--r--   0        0        0       87 2022-05-17 08:36:34.924591 etna-1.9.0/etna/core/__init__.py
--rw-r--r--   0        0        0     1343 2022-05-17 08:36:34.924591 etna-1.9.0/etna/core/mixins.py
--rw-r--r--   0        0        0      357 2022-05-17 08:36:34.924591 etna-1.9.0/etna/datasets/__init__.py
--rw-r--r--   0        0        0     5002 2022-05-17 08:36:34.924591 etna-1.9.0/etna/datasets/datasets_generation.py
--rw-r--r--   0        0        0    44785 2022-05-17 08:36:34.924591 etna-1.9.0/etna/datasets/tsdataset.py
--rw-r--r--   0        0        0     2903 2022-05-17 08:36:34.924591 etna-1.9.0/etna/datasets/utils.py
--rw-r--r--   0        0        0      166 2022-05-17 08:36:34.924591 etna-1.9.0/etna/ensembles/__init__.py
--rw-r--r--   0        0        0     1404 2022-05-17 08:36:34.924591 etna-1.9.0/etna/ensembles/base.py
--rw-r--r--   0        0        0     9766 2022-05-17 08:36:34.924591 etna-1.9.0/etna/ensembles/stacking_ensemble.py
--rw-r--r--   0        0        0     8333 2022-05-17 08:36:34.924591 etna-1.9.0/etna/ensembles/voting_ensemble.py
--rw-r--r--   0        0        0      341 2022-05-17 08:36:34.924591 etna-1.9.0/etna/libs/tsfresh/__init__.py
--rw-r--r--   0        0        0     1745 2022-05-17 08:36:34.924591 etna-1.9.0/etna/libs/tsfresh/defaults.py
--rw-r--r--   0        0        0     1831 2022-05-17 08:36:34.924591 etna-1.9.0/etna/libs/tsfresh/distribution.py
--rw-r--r--   0        0        0    16540 2022-05-17 08:36:34.924591 etna-1.9.0/etna/libs/tsfresh/relevance.py
--rw-r--r--   0        0        0     8431 2022-05-17 08:36:34.924591 etna-1.9.0/etna/libs/tsfresh/significance_tests.py
--rw-r--r--   0        0        0      804 2022-05-17 08:36:34.924591 etna-1.9.0/etna/loggers/__init__.py
--rw-r--r--   0        0        0     6383 2022-05-17 08:36:34.924591 etna-1.9.0/etna/loggers/base.py
--rw-r--r--   0        0        0     2643 2022-05-17 08:36:34.924591 etna-1.9.0/etna/loggers/console_logger.py
--rw-r--r--   0        0        0    15237 2022-05-17 08:36:34.924591 etna-1.9.0/etna/loggers/file_logger.py
--rw-r--r--   0        0        0     7067 2022-05-17 08:36:34.924591 etna-1.9.0/etna/loggers/wandb_logger.py
--rw-r--r--   0        0        0      865 2022-05-17 08:36:34.924591 etna-1.9.0/etna/metrics/__init__.py
--rw-r--r--   0        0        0     6581 2022-05-17 08:36:34.924591 etna-1.9.0/etna/metrics/base.py
--rw-r--r--   0        0        0     2546 2022-05-17 08:36:34.928591 etna-1.9.0/etna/metrics/functional_metrics.py
--rw-r--r--   0        0        0     5254 2022-05-17 08:36:34.928591 etna-1.9.0/etna/metrics/intervals_metrics.py
--rw-r--r--   0        0        0     5287 2022-05-17 08:36:34.928591 etna-1.9.0/etna/metrics/metrics.py
--rw-r--r--   0        0        0      780 2022-05-17 08:36:34.928591 etna-1.9.0/etna/metrics/utils.py
--rw-r--r--   0        0        0     1081 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/__init__.py
--rw-r--r--   0        0        0    13800 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/base.py
--rw-r--r--   0        0        0    11832 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/catboost.py
--rw-r--r--   0        0        0    23653 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/holt_winters.py
--rw-r--r--   0        0        0     4887 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/linear.py
--rw-r--r--   0        0        0      639 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/moving_average.py
--rw-r--r--   0        0        0      550 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/naive.py
--rw-r--r--   0        0        0      149 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/nn/__init__.py
--rw-r--r--   0        0        0     5688 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/nn/deepar.py
--rw-r--r--   0        0        0     6175 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/nn/tft.py
--rw-r--r--   0        0        0    14430 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/prophet.py
--rw-r--r--   0        0        0    22285 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/sarimax.py
--rw-r--r--   0        0        0     3832 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/seasonal_ma.py
--rw-r--r--   0        0        0     2757 2022-05-17 08:36:34.928591 etna-1.9.0/etna/models/sklearn.py
--rw-r--r--   0        0        0      157 2022-05-17 08:36:34.928591 etna-1.9.0/etna/pipeline/__init__.py
--rw-r--r--   0        0        0     5541 2022-05-17 08:36:34.928591 etna-1.9.0/etna/pipeline/autoregressive_pipeline.py
--rw-r--r--   0        0        0    21402 2022-05-17 08:36:34.928591 etna-1.9.0/etna/pipeline/base.py
--rw-r--r--   0        0        0     3101 2022-05-17 08:36:34.928591 etna-1.9.0/etna/pipeline/pipeline.py
--rw-r--r--   0        0        0     9389 2022-05-17 08:36:34.928591 etna-1.9.0/etna/settings.py
--rw-r--r--   0        0        0     2554 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/__init__.py
--rw-r--r--   0        0        0     3146 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/base.py
--rw-r--r--   0        0        0      425 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/decomposition/__init__.py
--rw-r--r--   0        0        0     2472 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/decomposition/binseg.py
--rw-r--r--   0        0        0     8139 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/decomposition/change_points_trend.py
--rw-r--r--   0        0        0     6921 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/decomposition/detrend.py
--rw-r--r--   0        0        0     7363 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/decomposition/stl.py
--rw-r--r--   0        0        0     6033 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/decomposition/trend.py
--rw-r--r--   0        0        0      306 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/encoders/__init__.py
--rw-r--r--   0        0        0     5495 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/encoders/categorical.py
--rw-r--r--   0        0        0     1566 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/encoders/mean_segment_encoder.py
--rw-r--r--   0        0        0     1640 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/encoders/segment_encoder.py
--rw-r--r--   0        0        0      444 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/feature_selection/__init__.py
--rw-r--r--   0        0        0     1640 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/feature_selection/base.py
--rw-r--r--   0        0        0     6973 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/feature_selection/feature_importance.py
--rw-r--r--   0        0        0     2495 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/feature_selection/filter.py
--rw-r--r--   0        0        0    14071 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/feature_selection/gale_shapley.py
--rw-r--r--   0        0        0     1137 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/math/__init__.py
--rw-r--r--   0        0        0     3801 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/math/add_constant.py
--rw-r--r--   0        0        0    13311 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/math/differencing.py
--rw-r--r--   0        0        0     2653 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/math/lags.py
--rw-r--r--   0        0        0     4156 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/math/log.py
--rw-r--r--   0        0        0     3330 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/math/power.py
--rw-r--r--   0        0        0     8460 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/math/scalers.py
--rw-r--r--   0        0        0     8462 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/math/sklearn.py
--rw-r--r--   0        0        0    16976 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/math/statistics.py
--rw-r--r--   0        0        0      233 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/missing_values/__init__.py
--rw-r--r--   0        0        0     8395 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/missing_values/imputation.py
--rw-r--r--   0        0        0     5795 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/missing_values/resample.py
--rw-r--r--   0        0        0       79 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/nn/__init__.py
--rw-r--r--   0        0        0     8572 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/nn/pytorch_forecasting.py
--rw-r--r--   0        0        0      301 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/outliers/__init__.py
--rw-r--r--   0        0        0     3941 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/outliers/base.py
--rw-r--r--   0        0        0     5684 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/outliers/point_outliers.py
--rw-r--r--   0        0        0      334 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/timestamp/__init__.py
--rw-r--r--   0        0        0    13532 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/timestamp/date_flags.py
--rw-r--r--   0        0        0     4775 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/timestamp/fourier.py
--rw-r--r--   0        0        0     2373 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/timestamp/holiday.py
--rw-r--r--   0        0        0     7712 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/timestamp/special_days.py
--rw-r--r--   0        0        0     7694 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/timestamp/time_flags.py
--rw-r--r--   0        0        0      261 2022-05-17 08:36:34.928591 etna-1.9.0/etna/transforms/utils.py
--rw-r--r--   0        0        0     5049 2022-05-17 08:36:35.000593 etna-1.9.0/pyproject.toml
--rw-r--r--   0        0        0    16109 2022-05-17 08:37:41.326591 etna-1.9.0/setup.py
--rw-r--r--   0        0        0    16002 2022-05-17 08:37:41.327574 etna-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11244 2023-04-12 06:09:53.967157 etna-2.0.0/LICENSE
+-rw-r--r--   0        0        0    13188 2023-04-12 06:09:53.971157 etna-2.0.0/README.md
+-rw-r--r--   0        0        0       49 2023-04-12 06:09:53.971157 etna-2.0.0/etna/__init__.py
+-rw-r--r--   0        0        0     2388 2023-04-12 06:09:53.971157 etna-2.0.0/etna/analysis/__init__.py
+-rw-r--r--   0        0        0      599 2023-04-12 06:09:53.971157 etna-2.0.0/etna/analysis/decomposition/__init__.py
+-rw-r--r--   0        0        0    16581 2023-04-12 06:09:53.971157 etna-2.0.0/etna/analysis/decomposition/plots.py
+-rw-r--r--   0        0        0     1189 2023-04-12 06:09:53.971157 etna-2.0.0/etna/analysis/decomposition/search.py
+-rw-r--r--   0        0        0     9835 2023-04-12 06:09:53.971157 etna-2.0.0/etna/analysis/decomposition/utils.py
+-rw-r--r--   0        0        0      475 2023-04-12 06:09:53.971157 etna-2.0.0/etna/analysis/eda/__init__.py
+-rw-r--r--   0        0        0    26025 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/eda/plots.py
+-rw-r--r--   0        0        0     4077 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/eda/utils.py
+-rw-r--r--   0        0        0      472 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_relevance/__init__.py
+-rw-r--r--   0        0        0     6004 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_relevance/plots.py
+-rw-r--r--   0        0        0     3114 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_relevance/relevance.py
+-rw-r--r--   0        0        0     3962 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_relevance/relevance_table.py
+-rw-r--r--   0        0        0      654 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_relevance/utils.py
+-rw-r--r--   0        0        0      213 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_selection/__init__.py
+-rw-r--r--   0        0        0     3870 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_selection/mrmr_selection.py
+-rw-r--r--   0        0        0      737 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/forecast/__init__.py
+-rw-r--r--   0        0        0    35388 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/forecast/plots.py
+-rw-r--r--   0        0        0     3855 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/forecast/utils.py
+-rw-r--r--   0        0        0      517 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/outliers/__init__.py
+-rw-r--r--   0        0        0     4879 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/outliers/density_outliers.py
+-rw-r--r--   0        0        0    13169 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/outliers/hist_outliers.py
+-rw-r--r--   0        0        0     1739 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/outliers/median_outliers.py
+-rw-r--r--   0        0        0     5343 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/outliers/plots.py
+-rw-r--r--   0        0        0     3131 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/outliers/prediction_interval_outliers.py
+-rw-r--r--   0        0        0     1471 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/utils.py
+-rw-r--r--   0        0        0       64 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/__init__.py
+-rw-r--r--   0        0        0    12482 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/auto.py
+-rw-r--r--   0        0        0      102 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/optuna/__init__.py
+-rw-r--r--   0        0        0     4680 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/optuna/config_sampler.py
+-rw-r--r--   0        0        0     2828 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/optuna/wrapper.py
+-rw-r--r--   0        0        0       93 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/pool/__init__.py
+-rw-r--r--   0        0        0     1533 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/pool/generator.py
+-rw-r--r--   0        0        0     5348 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/pool/templates.py
+-rw-r--r--   0        0        0      495 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/pool/utils.py
+-rw-r--r--   0        0        0      151 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/runner/__init__.py
+-rw-r--r--   0        0        0      451 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/runner/base.py
+-rw-r--r--   0        0        0     2114 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/runner/local.py
+-rw-r--r--   0        0        0      171 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/runner/utils.py
+-rw-r--r--   0        0        0      740 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/utils.py
+-rw-r--r--   0        0        0      524 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/__init__.py
+-rw-r--r--   0        0        0      686 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/base.py
+-rw-r--r--   0        0        0      259 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/distances/__init__.py
+-rw-r--r--   0        0        0     3756 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/distances/base.py
+-rw-r--r--   0        0        0     4508 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/distances/distance_matrix.py
+-rw-r--r--   0        0        0     5597 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/distances/dtw_distance.py
+-rw-r--r--   0        0        0     1705 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/distances/euclidean_distance.py
+-rw-r--r--   0        0        0      289 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/hierarchical/__init__.py
+-rw-r--r--   0        0        0     6020 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/hierarchical/base.py
+-rw-r--r--   0        0        0     1501 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/hierarchical/dtw_clustering.py
+-rw-r--r--   0        0        0     1561 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/hierarchical/euclidean_clustering.py
+-rw-r--r--   0        0        0      374 2023-04-12 06:09:53.975157 etna-2.0.0/etna/commands/__init__.py
+-rw-r--r--   0        0        0      197 2023-04-12 06:09:53.975157 etna-2.0.0/etna/commands/__main__.py
+-rw-r--r--   0        0        0     3549 2023-04-12 06:09:53.975157 etna-2.0.0/etna/commands/backtest_command.py
+-rw-r--r--   0        0        0     3858 2023-04-12 06:09:53.975157 etna-2.0.0/etna/commands/forecast_command.py
+-rw-r--r--   0        0        0      281 2023-04-12 06:09:53.975157 etna-2.0.0/etna/commands/resolvers.py
+-rw-r--r--   0        0        0      205 2023-04-12 06:09:53.975157 etna-2.0.0/etna/core/__init__.py
+-rw-r--r--   0        0        0     9194 2023-04-12 06:09:53.975157 etna-2.0.0/etna/core/mixins.py
+-rw-r--r--   0        0        0      617 2023-04-12 06:09:53.975157 etna-2.0.0/etna/core/saving.py
+-rw-r--r--   0        0        0     2248 2023-04-12 06:09:53.975157 etna-2.0.0/etna/core/utils.py
+-rw-r--r--   0        0        0      548 2023-04-12 06:09:53.975157 etna-2.0.0/etna/datasets/__init__.py
+-rw-r--r--   0        0        0     8274 2023-04-12 06:09:53.975157 etna-2.0.0/etna/datasets/datasets_generation.py
+-rw-r--r--   0        0        0     7778 2023-04-12 06:09:53.975157 etna-2.0.0/etna/datasets/hierarchical_structure.py
+-rw-r--r--   0        0        0    61946 2023-04-12 06:09:53.975157 etna-2.0.0/etna/datasets/tsdataset.py
+-rw-r--r--   0        0        0    10283 2023-04-12 06:09:53.975157 etna-2.0.0/etna/datasets/utils.py
+-rw-r--r--   0        0        0      226 2023-04-12 06:09:53.975157 etna-2.0.0/etna/ensembles/__init__.py
+-rw-r--r--   0        0        0     6197 2023-04-12 06:09:53.975157 etna-2.0.0/etna/ensembles/direct_ensemble.py
+-rw-r--r--   0        0        0     4671 2023-04-12 06:09:53.975157 etna-2.0.0/etna/ensembles/mixins.py
+-rw-r--r--   0        0        0    10931 2023-04-12 06:09:53.975157 etna-2.0.0/etna/ensembles/stacking_ensemble.py
+-rw-r--r--   0        0        0     9437 2023-04-12 06:09:53.975157 etna-2.0.0/etna/ensembles/voting_ensemble.py
+-rw-r--r--   0        0        0       94 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/change_points/__init__.py
+-rw-r--r--   0        0        0     5558 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/change_points/regularization_search.py
+-rw-r--r--   0        0        0      170 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/__init__.py
+-rw-r--r--   0        0        0      473 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/base.py
+-rw-r--r--   0        0        0     4926 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/classification.py
+-rw-r--r--   0        0        0      290 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/feature_extraction/__init__.py
+-rw-r--r--   0        0        0     1543 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/feature_extraction/base.py
+-rw-r--r--   0        0        0     2503 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/feature_extraction/tsfresh.py
+-rw-r--r--   0        0        0    14997 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/feature_extraction/weasel.py
+-rw-r--r--   0        0        0     3241 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/predictability.py
+-rw-r--r--   0        0        0      874 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/utils.py
+-rw-r--r--   0        0        0        0 2023-04-12 06:09:53.975157 etna-2.0.0/etna/libs/__init__.py
+-rw-r--r--   0        0        0       79 2023-04-12 06:09:53.975157 etna-2.0.0/etna/libs/pmdarima_utils/__init__.py
+-rw-r--r--   0        0        0     7455 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/pmdarima_utils/arima.py
+-rw-r--r--   0        0        0      415 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/pmdarima_utils/arima.pyi
+-rw-r--r--   0        0        0        0 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      472 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/pytorch_lightning/callbacks.py
+-rw-r--r--   0        0        0      341 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/__init__.py
+-rw-r--r--   0        0        0     1745 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/defaults.py
+-rw-r--r--   0        0        0     1831 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/distribution.py
+-rw-r--r--   0        0        0       69 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/distribution.pyi
+-rw-r--r--   0        0        0    16540 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/relevance.py
+-rw-r--r--   0        0        0      823 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/relevance.pyi
+-rw-r--r--   0        0        0     8431 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/significance_tests.py
+-rw-r--r--   0        0        0      344 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/significance_tests.pyi
+-rw-r--r--   0        0        0      804 2023-04-12 06:09:53.979157 etna-2.0.0/etna/loggers/__init__.py
+-rw-r--r--   0        0        0     4993 2023-04-12 06:09:53.979157 etna-2.0.0/etna/loggers/base.py
+-rw-r--r--   0        0        0     2643 2023-04-12 06:09:53.979157 etna-2.0.0/etna/loggers/console_logger.py
+-rw-r--r--   0        0        0    15306 2023-04-12 06:09:53.979157 etna-2.0.0/etna/loggers/file_logger.py
+-rw-r--r--   0        0        0     7105 2023-04-12 06:09:53.979157 etna-2.0.0/etna/loggers/wandb_logger.py
+-rw-r--r--   0        0        0     1230 2023-04-12 06:09:53.979157 etna-2.0.0/etna/metrics/__init__.py
+-rw-r--r--   0        0        0     7625 2023-04-12 06:09:53.979157 etna-2.0.0/etna/metrics/base.py
+-rw-r--r--   0        0        0     5151 2023-04-12 06:09:53.979157 etna-2.0.0/etna/metrics/functional_metrics.py
+-rw-r--r--   0        0        0     5513 2023-04-12 06:09:53.979157 etna-2.0.0/etna/metrics/intervals_metrics.py
+-rw-r--r--   0        0        0     9643 2023-04-12 06:09:53.979157 etna-2.0.0/etna/metrics/metrics.py
+-rw-r--r--   0        0        0     2539 2023-04-12 06:09:53.979157 etna-2.0.0/etna/metrics/utils.py
+-rw-r--r--   0        0        0     1729 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/__init__.py
+-rw-r--r--   0        0        0     2521 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/autoarima.py
+-rw-r--r--   0        0        0    22815 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/base.py
+-rw-r--r--   0        0        0    14654 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/catboost.py
+-rw-r--r--   0        0        0    13704 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/deadline_ma.py
+-rw-r--r--   0        0        0      557 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/decorators.py
+-rw-r--r--   0        0        0    30566 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/holt_winters.py
+-rw-r--r--   0        0        0     7136 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/linear.py
+-rw-r--r--   0        0        0    22799 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/mixins.py
+-rw-r--r--   0        0        0      828 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/moving_average.py
+-rw-r--r--   0        0        0      712 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/naive.py
+-rw-r--r--   0        0        0      307 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/nn/__init__.py
+-rw-r--r--   0        0        0     9210 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/nn/deepar.py
+-rw-r--r--   0        0        0     7988 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/nn/mlp.py
+-rw-r--r--   0        0        0    10502 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/nn/rnn.py
+-rw-r--r--   0        0        0    10658 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/nn/tft.py
+-rw-r--r--   0        0        0    11824 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/nn/utils.py
+-rw-r--r--   0        0        0    18870 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/prophet.py
+-rw-r--r--   0        0        0    31892 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/sarimax.py
+-rw-r--r--   0        0        0     8465 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/seasonal_ma.py
+-rw-r--r--   0        0        0     3555 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/sklearn.py
+-rw-r--r--   0        0        0    19716 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/tbats.py
+-rw-r--r--   0        0        0     3685 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/utils.py
+-rw-r--r--   0        0        0      292 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/__init__.py
+-rw-r--r--   0        0        0     5437 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/assembling_pipelines.py
+-rw-r--r--   0        0        0     7232 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/autoregressive_pipeline.py
+-rw-r--r--   0        0        0    36768 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/base.py
+-rw-r--r--   0        0        0    14014 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/hierarchical_pipeline.py
+-rw-r--r--   0        0        0     7388 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/mixins.py
+-rw-r--r--   0        0        0     5467 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/pipeline.py
+-rw-r--r--   0        0        0        0 2023-04-12 06:09:53.979157 etna-2.0.0/etna/py.typed
+-rw-r--r--   0        0        0      181 2023-04-12 06:09:53.979157 etna-2.0.0/etna/reconciliation/__init__.py
+-rw-r--r--   0        0        0     3473 2023-04-12 06:09:53.979157 etna-2.0.0/etna/reconciliation/base.py
+-rw-r--r--   0        0        0     1899 2023-04-12 06:09:53.979157 etna-2.0.0/etna/reconciliation/bottom_up.py
+-rw-r--r--   0        0        0     5742 2023-04-12 06:09:53.979157 etna-2.0.0/etna/reconciliation/top_down.py
+-rw-r--r--   0        0        0     9971 2023-04-12 06:09:53.979157 etna-2.0.0/etna/settings.py
+-rw-r--r--   0        0        0     3234 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/__init__.py
+-rw-r--r--   0        0        0    12526 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/base.py
+-rw-r--r--   0        0        0     1168 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/decomposition/__init__.py
+-rw-r--r--   0        0        0      949 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/decomposition/change_points_based/__init__.py
+-rw-r--r--   0        0        0     7980 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/decomposition/change_points_based/base.py
+-rw-r--r--   0        0        0      250 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/decomposition/change_points_based/change_points_models/__init__.py
+-rw-r--r--   0        0        0     1886 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/decomposition/change_points_based/change_points_models/base.py
+-rw-r--r--   0        0        0     2171 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/decomposition/change_points_based/change_points_models/ruptures_based.py
+-rw-r--r--   0        0        0     3600 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/detrend.py
+-rw-r--r--   0        0        0     3080 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/level.py
+-rw-r--r--   0        0        0      887 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/__init__.py
+-rw-r--r--   0        0        0      724 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/base.py
+-rw-r--r--   0        0        0     1311 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/constant.py
+-rw-r--r--   0        0        0     3397 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py
+-rw-r--r--   0        0        0     2496 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/statistics_based.py
+-rw-r--r--   0        0        0     3445 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/segmentation.py
+-rw-r--r--   0        0        0     3369 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/trend.py
+-rw-r--r--   0        0        0     7358 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/detrend.py
+-rw-r--r--   0        0        0     7670 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/stl.py
+-rw-r--r--   0        0        0      306 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/encoders/__init__.py
+-rw-r--r--   0        0        0     6985 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/encoders/categorical.py
+-rw-r--r--   0        0        0     2836 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/encoders/mean_segment_encoder.py
+-rw-r--r--   0        0        0     2525 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/encoders/segment_encoder.py
+-rw-r--r--   0        0        0      444 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/feature_selection/__init__.py
+-rw-r--r--   0        0        0     2469 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/feature_selection/base.py
+-rw-r--r--   0        0        0     7308 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/feature_selection/feature_importance.py
+-rw-r--r--   0        0        0     3434 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/feature_selection/filter.py
+-rw-r--r--   0        0        0    14261 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/feature_selection/gale_shapley.py
+-rw-r--r--   0        0        0     1326 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/__init__.py
+-rw-r--r--   0        0        0     4821 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/add_constant.py
+-rw-r--r--   0        0        0     5645 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/apply_lambda.py
+-rw-r--r--   0        0        0    16679 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/differencing.py
+-rw-r--r--   0        0        0     3346 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/lags.py
+-rw-r--r--   0        0        0     5002 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/log.py
+-rw-r--r--   0        0        0     3330 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/power.py
+-rw-r--r--   0        0        0     8464 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/scalers.py
+-rw-r--r--   0        0        0    11348 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/sklearn.py
+-rw-r--r--   0        0        0    21230 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/statistics.py
+-rw-r--r--   0        0        0      233 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/missing_values/__init__.py
+-rw-r--r--   0        0        0     9100 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/missing_values/imputation.py
+-rw-r--r--   0        0        0     6698 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/missing_values/resample.py
+-rw-r--r--   0        0        0      301 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/outliers/__init__.py
+-rw-r--r--   0        0        0     5106 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/outliers/base.py
+-rw-r--r--   0        0        0     5733 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/outliers/point_outliers.py
+-rw-r--r--   0        0        0      334 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/timestamp/__init__.py
+-rw-r--r--   0        0        0    14352 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/timestamp/date_flags.py
+-rw-r--r--   0        0        0     5135 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/timestamp/fourier.py
+-rw-r--r--   0        0        0     2848 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/timestamp/holiday.py
+-rw-r--r--   0        0        0     8370 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/timestamp/special_days.py
+-rw-r--r--   0        0        0     8347 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/timestamp/time_flags.py
+-rw-r--r--   0        0        0      734 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/utils.py
+-rw-r--r--   0        0        0    11759 2023-04-12 06:09:54.147159 etna-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    18682 1970-01-01 00:00:00.000000 etna-2.0.0/PKG-INFO
```

### Comparing `etna-1.9.0/LICENSE` & `etna-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/README.md` & `etna-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,21 @@
   <a href="https://pypi.org/project/etna/"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/etna.svg" /></a>
   <a href="https://pypi.org/project/etna/"><img alt="Python versions" src="https://img.shields.io/pypi/pyversions/etna.svg" /></a>
   <a href="https://pepy.tech/project/etna"><img alt="Downloads" src="https://static.pepy.tech/personalized-badge/etna?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" /></a>
 </p>
  
 <p align="center">
   <a href="https://codecov.io/gh/tinkoff-ai/etna"><img alt="Coverage" src="https://img.shields.io/codecov/c/github/tinkoff-ai/etna.svg" /></a>
-  <a href="https://github.com/tinkoff-ai/etna/actions/workflows/test.yml?query=branch%3Amaster++"><img alt="Test passing" src="https://img.shields.io/github/workflow/status/tinkoff-ai/etna/Test/master?label=tests" /></a>
-  <a href="https://github.com/tinkoff-ai/etna/actions/workflows/publish.yml"><img alt="Docs publish" src="https://img.shields.io/github/workflow/status/tinkoff-ai/etna/Publish?label=docs" /></a>
+  <a href="https://github.com/tinkoff-ai/etna/actions/workflows/test.yml?query=branch%3Amaster++"><img alt="Test passing" src="https://img.shields.io/github/actions/workflow/status/tinkoff-ai/etna/test.yml?branch=master&label=tests" /></a>
+  <a href="https://github.com/tinkoff-ai/etna/actions/workflows/publish.yml"><img alt="Docs publish" src="https://img.shields.io/github/actions/workflow/status/tinkoff-ai/etna/publish.yml?label=docs" /></a>
   <a href="https://github.com/tinkoff-ai/etna/blob/master/LICENSE"><img alt="License" src="https://img.shields.io/github/license/tinkoff-ai/etna.svg" /></a>
 </p>
 
 <p align="center">
   <a href="https://t.me/etna_support"><img alt="Telegram" src="https://img.shields.io/badge/channel-telegram-blue" /></a>
-  <a href="https://opendatascience.slack.com/archives/C02Q62NEPH8"><img alt="Slack" src="https://img.shields.io/badge/slack-ods.ai-orange" /></a>
   <a href="https://github.com/tinkoff-ai/etna/discussions"><img alt="GitHub Discussions" src="https://img.shields.io/github/discussions/tinkoff-ai/etna" /></a>
   <a href="https://github.com/tinkoff-ai/etna/graphs/contributors"><img alt="Contributors" src="https://img.shields.io/github/contributors/tinkoff-ai/etna.svg" /></a>
   <a href="https://github.com/tinkoff-ai/etna/stargazers"><img alt="Stars" src="https://img.shields.io/github/stars/tinkoff-ai/etna?style=social" /></a>
 </p>
 
 <p align="center">
   <a href="https://etna.tinkoff.ru">Homepage</a> | 
@@ -65,15 +64,15 @@
 
 # Make train/test split
 train_ts, test_ts = ts.train_test_split(test_size=HORIZON)
 ```
 
 Define transformations and model:
 ```python
-from etna.models import CatBoostModelMultiSegment
+from etna.models import CatBoostMultiSegmentModel
 from etna.transforms import DateFlagsTransform
 from etna.transforms import DensityOutliersTransform
 from etna.transforms import FourierTransform
 from etna.transforms import LagTransform
 from etna.transforms import LinearTrendTransform
 from etna.transforms import MeanTransform
 from etna.transforms import SegmentEncoderTransform
@@ -91,15 +90,15 @@
     FourierTransform(period=360.25, order=6, out_column="fourier"),
     SegmentEncoderTransform(),
     MeanTransform(in_column=f"target_lag_{HORIZON}", window=12, seasonality=7),
     MeanTransform(in_column=f"target_lag_{HORIZON}", window=7),
 ]
 
 # Prepare model
-model = CatBoostModelMultiSegment()
+model = CatBoostMultiSegmentModel()
 ```
 
 Fit `Pipeline` and make a prediction:
 ```python
 from etna.pipeline import Pipeline
 
 # Create and fit the pipeline
@@ -174,62 +173,80 @@
 | [Get started](https://github.com/tinkoff-ai/etna/tree/master/examples/get_started.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/get_started.ipynb) |
 | [Backtest](https://github.com/tinkoff-ai/etna/tree/master/examples/backtest.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/backtest.ipynb) |
 | [EDA](https://github.com/tinkoff-ai/etna/tree/master/examples/EDA.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/EDA.ipynb) |
 | [Outliers](https://github.com/tinkoff-ai/etna/tree/master/examples/outliers.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/outliers.ipynb) |
 | [Clustering](https://github.com/tinkoff-ai/etna/tree/master/examples/clustering.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/clustering.ipynb) |
 | [Deep learning models](https://github.com/tinkoff-ai/etna/tree/master/examples/NN_examples.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/NN_examples.ipynb) |
 | [Ensembles](https://github.com/tinkoff-ai/etna/tree/master/examples/ensembles.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/ensembles.ipynb) |
+| [Custom Transform and Model](https://github.com/tinkoff-ai/etna/tree/master/examples/custom_transform_and_model.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/custom_transform_and_model.ipynb) |
+| [Exogenous data](https://github.com/tinkoff-ai/etna/tree/master/examples/exogenous_data.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/exogenous_data.ipynb) |
+| [Forecasting strategies](https://github.com/tinkoff-ai/etna/blob/master/examples/forecasting_strategies.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/forecasting_strategies.ipynb) |
+| [Classification](https://github.com/tinkoff-ai/etna/blob/master/examples/classification.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/classification.ipynb) |
+| [Hierarchical time series](https://github.com/tinkoff-ai/etna/blob/master/examples/hierarchical_pipeline.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/hierarchical_pipeline.ipynb) |
 
 ## Documentation
 
 ETNA documentation is available [here](https://etna-docs.netlify.app/).
 
 ## Community
 
 To ask the questions or discuss the library you can join our [telegram chat](t.me/etna_support). 
 [Discussions section](https://github.com/tinkoff-ai/etna/discussions) on github is also open for this purpose.
 
 ## Resources
 
 - [Forecasting with ETNA: Fast and Furious](https://medium.com/its-tinkoff/forecasting-with-etna-fast-and-furious-1b58e1453809) on Medium
 
+- [ETNA Regressors](https://medium.com/its-tinkoff/etna-regressors-d2722923e88e) on Medium
+
+- [Time series forecasting with ETNA: first steps](https://medium.com/its-tinkoff/time-series-forecasting-with-etna-first-steps-dfaf90c5b919) on Medium
+
+- [ETNA: Time Series Analysis. What, why and how?](https://medium.com/its-tinkoff/etna-time-series-analysis-what-why-and-how-e45557af4f6c) on Medium
+
 - [Tabular Playground Series - Mar 2022 (7th place!)](https://www.kaggle.com/code/chikovalexander/tps-mar-2022-etna/notebook?scriptVersionId=91575908) on Kaggle
 
 - [Store sales prediction with etna library](https://www.kaggle.com/dmitrybunin/store-sales-prediction-with-etna-library?scriptVersionId=81104235) on Kaggle
 
 - [Tabular Playground Series - Jan 2022](https://www.kaggle.com/code/chikovalexander/tps-jan-2022-etna/notebook) on Kaggle
 
 - [EDA notebook for Ubiquant Market Prediction](https://www.kaggle.com/code/martins0n/ubiquant-eda-toy-predictions-etna) on Kaggle
 
 - [PyCon Russia September 2021 talk](https://youtu.be/VxWHLEFgXnE) on YouTube
 
-- ETNA Tutorial [Part 1 (Rus)](https://youtu.be/4iFVRfB2j30), [Part 2 (Rus)](https://youtu.be/Ct9dyUdHlmc),  [Part 3 (Rus)](https://youtu.be/Qof38dtigtE) on YouTube thanks to [RC Gewissta](https://github.com/Gewissta)
+- [ETNA Meetup Jun 2022](https://www.youtube.com/watch?v=N1Xy3EqY058&list=PLLrf_044z4JrSsjMd-3dF6VbBLPI_yOxG) on YouTube
 
+- [DUMP May 2022 talk](https://youtu.be/12uuxepdtks) on YouTube
+ 
 ## Acknowledgments
 
 ### ETNA.Team
 
 [Andrey Alekseev](https://github.com/iKintosh),
 [Nikita Barinov](https://github.com/diadorer),
 [Dmitriy Bunin](https://github.com/Mr-Geekman),
 [Aleksandr Chikov](https://github.com/alex-hse-repository),
 [Vladislav Denisov](https://github.com/v-v-denisov),
 [Martin Gabdushev](https://github.com/martins0n),
 [Sergey Kolesnikov](https://github.com/Scitator),
 [Artem Makhin](https://github.com/Ama16),
 [Ivan Mitskovets](https://github.com/imitskovets),
 [Albina Munirova](https://github.com/albinamunirova),
-[Nikolay Romantsov](https://github.com/WinstonDovlatov),
-[Julia Shenshina](https://github.com/julia-shenshina)
+[Julia Shenshina](https://github.com/julia-shenshina),
+[Yuriy Tarasyuk](https://github.com/DBcreator),
+[Konstantin Vedernikov](https://github.com/scanhex12)
 
 ### ETNA.Contributors
 
+[WinstonDovlatov](https://github.com/WinstonDovlatov),
+[mvakhmenin](https://github.com/mvakhmenin),
+[Carlosbogo](https://github.com/Carlosbogo),
+[Pacman1984](https://github.com/Pacman1984),
+[looopka](https://github.com/looopka),
 [Artem Levashov](https://github.com/soft1q),
-[Aleksey Podkidyshev](https://github.com/alekseyen),
-[Carlosbogo](https://github.com/Carlosbogo)
+[Aleksey Podkidyshev](https://github.com/alekseyen)
 
 ## License
 
 Feel free to use our library in your commercial and private applications.
 
 ETNA is covered by [Apache 2.0](/LICENSE). 
 Read more about this license [here](https://choosealicense.com/licenses/apache-2.0/)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
                                 [etna_logo.png]
               **** Predict your time series the easiest way ****
                  [PyPI_Version] [Python_versions] [Downloads]
               [Coverage] [Test_passing] [Docs_publish] [License]
-        [Telegram] [Slack] [GitHub_Discussions] [Contributors] [Stars]
+            [Telegram] [GitHub_Discussions] [Contributors] [Stars]
    Homepage | Documentation | Tutorials | Contribution_Guide | Release_Notes
 ETNA is an easy-to-use time series forecasting framework. It includes built in
 toolkits for time series preprocessing, feature generation, a variety of
 predictive models with unified interface - from classic machine learning to
 SOTA neural networks, models combination methods and smart backtesting. ETNA is
 designed to make working with time series simple, productive, and fun. ETNA is
 the first python open source framework of [Tinkoff.ru](https://www.tinkoff.ru/
@@ -16,30 +16,30 @@
 (https://github.com/tinkoff-ai/etna/blob/master/CONTRIBUTING.md). ## Get
 started Let's load and prepare the data. ```python import pandas as pd from
 etna.datasets import TSDataset # Read the data df = pd.read_csv("examples/data/
 example_dataset.csv") # Create a TSDataset df = TSDataset.to_dataset(df) ts =
 TSDataset(df, freq="D") # Choose a horizon HORIZON = 14 # Make train/test split
 train_ts, test_ts = ts.train_test_split(test_size=HORIZON) ``` Define
 transformations and model: ```python from etna.models import
-CatBoostModelMultiSegment from etna.transforms import DateFlagsTransform from
+CatBoostMultiSegmentModel from etna.transforms import DateFlagsTransform from
 etna.transforms import DensityOutliersTransform from etna.transforms import
 FourierTransform from etna.transforms import LagTransform from etna.transforms
 import LinearTrendTransform from etna.transforms import MeanTransform from
 etna.transforms import SegmentEncoderTransform from etna.transforms import
 TimeSeriesImputerTransform from etna.transforms import TrendTransform # Prepare
 transforms transforms = [ DensityOutliersTransform(in_column="target",
 distance_coef=3.0), TimeSeriesImputerTransform(in_column="target",
 strategy="forward_fill"), LinearTrendTransform(in_column="target"),
 TrendTransform(in_column="target", out_column="trend"), LagTransform
 (in_column="target", lags=list(range(HORIZON, 122)), out_column="target_lag"),
 DateFlagsTransform(week_number_in_month=True, out_column="date_flag"),
 FourierTransform(period=360.25, order=6, out_column="fourier"),
 SegmentEncoderTransform(), MeanTransform(in_column=f"target_lag_{HORIZON}",
 window=12, seasonality=7), MeanTransform(in_column=f"target_lag_{HORIZON}",
-window=7), ] # Prepare model model = CatBoostModelMultiSegment() ``` Fit
+window=7), ] # Prepare model model = CatBoostMultiSegmentModel() ``` Fit
 `Pipeline` and make a prediction: ```python from etna.pipeline import Pipeline
 # Create and fit the pipeline pipeline = Pipeline(model=model,
 transforms=transforms, horizon=HORIZON) pipeline.fit(train_ts) # Make a
 forecast forecast_ts = pipeline.forecast() ``` Let's plot the results:
 ```python from etna.analysis import plot_forecast plot_forecast
 (forecast_ts=forecast_ts, test_ts=test_ts, train_ts=train_ts,
 n_train_samples=50) ``` ![](examples/assets/readme/get_started.png) Print the
@@ -84,41 +84,67 @@
 mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
 master?filepath=examples/clustering.ipynb) | | [Deep learning models](https://
 github.com/tinkoff-ai/etna/tree/master/examples/NN_examples.ipynb) | [![Binder]
 (https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/
 etna/master?filepath=examples/NN_examples.ipynb) | | [Ensembles](https://
 github.com/tinkoff-ai/etna/tree/master/examples/ensembles.ipynb) | [![Binder]
 (https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/
-etna/master?filepath=examples/ensembles.ipynb) | ## Documentation ETNA
+etna/master?filepath=examples/ensembles.ipynb) | | [Custom Transform and Model]
+(https://github.com/tinkoff-ai/etna/tree/master/examples/
+custom_transform_and_model.ipynb) | [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
+master?filepath=examples/custom_transform_and_model.ipynb) | | [Exogenous data]
+(https://github.com/tinkoff-ai/etna/tree/master/examples/exogenous_data.ipynb)
+| [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/
+tinkoff-ai/etna/master?filepath=examples/exogenous_data.ipynb) | | [Forecasting
+strategies](https://github.com/tinkoff-ai/etna/blob/master/examples/
+forecasting_strategies.ipynb) | [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
+master?filepath=examples/forecasting_strategies.ipynb) | | [Classification]
+(https://github.com/tinkoff-ai/etna/blob/master/examples/classification.ipynb)
+| [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/
+tinkoff-ai/etna/master?filepath=examples/classification.ipynb) | |
+[Hierarchical time series](https://github.com/tinkoff-ai/etna/blob/master/
+examples/hierarchical_pipeline.ipynb) | [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
+master?filepath=examples/hierarchical_pipeline.ipynb) | ## Documentation ETNA
 documentation is available [here](https://etna-docs.netlify.app/). ## Community
 To ask the questions or discuss the library you can join our [telegram chat]
 (t.me/etna_support). [Discussions section](https://github.com/tinkoff-ai/etna/
 discussions) on github is also open for this purpose. ## Resources -
 [Forecasting with ETNA: Fast and Furious](https://medium.com/its-tinkoff/
-forecasting-with-etna-fast-and-furious-1b58e1453809) on Medium - [Tabular
-Playground Series - Mar 2022 (7th place!)](https://www.kaggle.com/code/
-chikovalexander/tps-mar-2022-etna/notebook?scriptVersionId=91575908) on Kaggle
-- [Store sales prediction with etna library](https://www.kaggle.com/
+forecasting-with-etna-fast-and-furious-1b58e1453809) on Medium - [ETNA
+Regressors](https://medium.com/its-tinkoff/etna-regressors-d2722923e88e) on
+Medium - [Time series forecasting with ETNA: first steps](https://medium.com/
+its-tinkoff/time-series-forecasting-with-etna-first-steps-dfaf90c5b919) on
+Medium - [ETNA: Time Series Analysis. What, why and how?](https://medium.com/
+its-tinkoff/etna-time-series-analysis-what-why-and-how-e45557af4f6c) on Medium
+- [Tabular Playground Series - Mar 2022 (7th place!)](https://www.kaggle.com/
+code/chikovalexander/tps-mar-2022-etna/notebook?scriptVersionId=91575908) on
+Kaggle - [Store sales prediction with etna library](https://www.kaggle.com/
 dmitrybunin/store-sales-prediction-with-etna-library?scriptVersionId=81104235)
 on Kaggle - [Tabular Playground Series - Jan 2022](https://www.kaggle.com/code/
 chikovalexander/tps-jan-2022-etna/notebook) on Kaggle - [EDA notebook for
 Ubiquant Market Prediction](https://www.kaggle.com/code/martins0n/ubiquant-eda-
 toy-predictions-etna) on Kaggle - [PyCon Russia September 2021 talk](https://
-youtu.be/VxWHLEFgXnE) on YouTube - ETNA Tutorial [Part 1 (Rus)](https://
-youtu.be/4iFVRfB2j30), [Part 2 (Rus)](https://youtu.be/Ct9dyUdHlmc), [Part 3
-(Rus)](https://youtu.be/Qof38dtigtE) on YouTube thanks to [RC Gewissta](https:/
-/github.com/Gewissta) ## Acknowledgments ### ETNA.Team [Andrey Alekseev](https:
-//github.com/iKintosh), [Nikita Barinov](https://github.com/diadorer), [Dmitriy
-Bunin](https://github.com/Mr-Geekman), [Aleksandr Chikov](https://github.com/
-alex-hse-repository), [Vladislav Denisov](https://github.com/v-v-denisov),
-[Martin Gabdushev](https://github.com/martins0n), [Sergey Kolesnikov](https://
+youtu.be/VxWHLEFgXnE) on YouTube - [ETNA Meetup Jun 2022](https://
+www.youtube.com/watch?v=N1Xy3EqY058&list=PLLrf_044z4JrSsjMd-3dF6VbBLPI_yOxG) on
+YouTube - [DUMP May 2022 talk](https://youtu.be/12uuxepdtks) on YouTube ##
+Acknowledgments ### ETNA.Team [Andrey Alekseev](https://github.com/iKintosh),
+[Nikita Barinov](https://github.com/diadorer), [Dmitriy Bunin](https://
+github.com/Mr-Geekman), [Aleksandr Chikov](https://github.com/alex-hse-
+repository), [Vladislav Denisov](https://github.com/v-v-denisov), [Martin
+Gabdushev](https://github.com/martins0n), [Sergey Kolesnikov](https://
 github.com/Scitator), [Artem Makhin](https://github.com/Ama16), [Ivan
 Mitskovets](https://github.com/imitskovets), [Albina Munirova](https://
-github.com/albinamunirova), [Nikolay Romantsov](https://github.com/
-WinstonDovlatov), [Julia Shenshina](https://github.com/julia-shenshina) ###
-ETNA.Contributors [Artem Levashov](https://github.com/soft1q), [Aleksey
-Podkidyshev](https://github.com/alekseyen), [Carlosbogo](https://github.com/
-Carlosbogo) ## License Feel free to use our library in your commercial and
-private applications. ETNA is covered by [Apache 2.0](/LICENSE). Read more
-about this license [here](https://choosealicense.com/licenses/apache-2.0/) >
-Please note that `etna[prophet]` is covered by [GPL 2.0](https://www.gnu.org/
-licenses/old-licenses/gpl-2.0.html) due to pystan package.
+github.com/albinamunirova), [Julia Shenshina](https://github.com/julia-
+shenshina), [Yuriy Tarasyuk](https://github.com/DBcreator), [Konstantin
+Vedernikov](https://github.com/scanhex12) ### ETNA.Contributors
+[WinstonDovlatov](https://github.com/WinstonDovlatov), [mvakhmenin](https://
+github.com/mvakhmenin), [Carlosbogo](https://github.com/Carlosbogo),
+[Pacman1984](https://github.com/Pacman1984), [looopka](https://github.com/
+looopka), [Artem Levashov](https://github.com/soft1q), [Aleksey Podkidyshev]
+(https://github.com/alekseyen) ## License Feel free to use our library in your
+commercial and private applications. ETNA is covered by [Apache 2.0](/LICENSE).
+Read more about this license [here](https://choosealicense.com/licenses/apache-
+2.0/) > Please note that `etna[prophet]` is covered by [GPL 2.0](https://
+www.gnu.org/licenses/old-licenses/gpl-2.0.html) due to pystan package.
```

### Comparing `etna-1.9.0/etna/analysis/__init__.py` & `etna-2.0.0/etna/analysis/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-from etna.analysis.change_points_trend import find_change_points
-from etna.analysis.eda_utils import SeasonalPlotAggregation
-from etna.analysis.eda_utils import SeasonalPlotAlignment
-from etna.analysis.eda_utils import SeasonalPlotCycle
-from etna.analysis.eda_utils import cross_corr_plot
-from etna.analysis.eda_utils import distribution_plot
-from etna.analysis.eda_utils import prediction_actual_scatter_plot
-from etna.analysis.eda_utils import qq_plot
-from etna.analysis.eda_utils import sample_acf_plot
-from etna.analysis.eda_utils import sample_pacf_plot
-from etna.analysis.eda_utils import seasonal_plot
-from etna.analysis.eda_utils import stl_plot
+from etna.analysis.decomposition import find_change_points
+from etna.analysis.decomposition import plot_change_points_interactive
+from etna.analysis.decomposition import plot_time_series_with_change_points
+from etna.analysis.decomposition import plot_trend
+from etna.analysis.decomposition import seasonal_plot
+from etna.analysis.decomposition import stl_plot
+from etna.analysis.eda import acf_plot
+from etna.analysis.eda import cross_corr_plot
+from etna.analysis.eda import distribution_plot
+from etna.analysis.eda import get_correlation_matrix
+from etna.analysis.eda import plot_clusters
+from etna.analysis.eda import plot_correlation_matrix
+from etna.analysis.eda import plot_holidays
+from etna.analysis.eda import plot_imputation
+from etna.analysis.eda import plot_periodogram
+from etna.analysis.feature_relevance import plot_feature_relevance
 from etna.analysis.feature_relevance.relevance import ModelRelevanceTable
 from etna.analysis.feature_relevance.relevance import RelevanceTable
 from etna.analysis.feature_relevance.relevance import StatisticsRelevanceTable
 from etna.analysis.feature_relevance.relevance_table import get_model_relevance_table
 from etna.analysis.feature_relevance.relevance_table import get_statistics_relevance_table
 from etna.analysis.feature_selection.mrmr_selection import AggregationMode
+from etna.analysis.forecast import get_residuals
+from etna.analysis.forecast import metric_per_segment_distribution_plot
+from etna.analysis.forecast import plot_backtest
+from etna.analysis.forecast import plot_backtest_interactive
+from etna.analysis.forecast import plot_forecast
+from etna.analysis.forecast import plot_forecast_decomposition
+from etna.analysis.forecast import plot_metric_per_segment
+from etna.analysis.forecast import plot_residuals
+from etna.analysis.forecast import prediction_actual_scatter_plot
+from etna.analysis.forecast import qq_plot
+from etna.analysis.outliers import plot_anomalies
+from etna.analysis.outliers import plot_anomalies_interactive
 from etna.analysis.outliers.density_outliers import absolute_difference_distance
 from etna.analysis.outliers.density_outliers import get_anomalies_density
 from etna.analysis.outliers.hist_outliers import get_anomalies_hist
 from etna.analysis.outliers.median_outliers import get_anomalies_median
 from etna.analysis.outliers.prediction_interval_outliers import get_anomalies_prediction_interval
-from etna.analysis.plotters import get_correlation_matrix
-from etna.analysis.plotters import get_residuals
-from etna.analysis.plotters import metric_per_segment_distribution_plot
-from etna.analysis.plotters import plot_anomalies
-from etna.analysis.plotters import plot_anomalies_interactive
-from etna.analysis.plotters import plot_backtest
-from etna.analysis.plotters import plot_backtest_interactive
-from etna.analysis.plotters import plot_clusters
-from etna.analysis.plotters import plot_correlation_matrix
-from etna.analysis.plotters import plot_feature_relevance
-from etna.analysis.plotters import plot_forecast
-from etna.analysis.plotters import plot_holidays
-from etna.analysis.plotters import plot_imputation
-from etna.analysis.plotters import plot_metric_per_segment
-from etna.analysis.plotters import plot_periodogram
-from etna.analysis.plotters import plot_residuals
-from etna.analysis.plotters import plot_time_series_with_change_points
-from etna.analysis.plotters import plot_trend
```

### Comparing `etna-1.9.0/etna/analysis/eda_utils.py` & `etna-2.0.0/etna/analysis/eda/plots.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,187 +1,591 @@
+import itertools
 import math
 import warnings
-from enum import Enum
+from copy import deepcopy
 from itertools import combinations
 from typing import TYPE_CHECKING
 from typing import Any
-from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 import statsmodels.api as sm
+from matplotlib.lines import Line2D
 from matplotlib.ticker import MaxNLocator
-from sklearn.linear_model import LinearRegression
-from sklearn.metrics import r2_score
-from statsmodels.graphics import utils
-from statsmodels.graphics.gofplots import qqplot
-from statsmodels.tsa.seasonal import STL
+from scipy.signal import periodogram
 from typing_extensions import Literal
 
-from etna.analysis.utils import prepare_axes
+from etna.analysis.eda.utils import _create_holidays_df
+from etna.analysis.eda.utils import get_correlation_matrix
+from etna.analysis.feature_selection import AGGREGATION_FN
+from etna.analysis.feature_selection import AggregationMode
+from etna.analysis.utils import _get_borders_ts
+from etna.analysis.utils import _prepare_axes
 
 if TYPE_CHECKING:
     from etna.datasets import TSDataset
+    from etna.transforms import TimeSeriesImputerTransform
 
 plot_acf = sm.graphics.tsa.plot_acf
 plot_pacf = sm.graphics.tsa.plot_pacf
 
 
+def plot_correlation_matrix(
+    ts: "TSDataset",
+    columns: Optional[List[str]] = None,
+    segments: Optional[List[str]] = None,
+    method: str = "pearson",
+    mode: str = "macro",
+    columns_num: int = 2,
+    figsize: Tuple[int, int] = (10, 10),
+    **heatmap_kwargs,
+):
+    """Plot pairwise correlation heatmap for selected segments.
+
+    Parameters
+    ----------
+    ts:
+        TSDataset with timeseries data
+    columns:
+        Columns to use, if None use all columns
+    segments:
+        Segments to use
+    method:
+        Method of correlation:
+
+        * pearson: standard correlation coefficient
+
+        * kendall: Kendall Tau correlation coefficient
+
+        * spearman: Spearman rank correlation
+
+    mode: 'macro' or 'per-segment'
+        Aggregation mode
+    columns_num:
+        Number of subplots columns
+    figsize:
+        size of the figure in inches
+    """
+    if segments is None:
+        segments = sorted(ts.segments)
+    if columns is None:
+        columns = list(set(ts.df.columns.get_level_values("feature")))
+    if "vmin" not in heatmap_kwargs:
+        heatmap_kwargs["vmin"] = -1
+    if "vmax" not in heatmap_kwargs:
+        heatmap_kwargs["vmax"] = 1
+
+    if mode not in ["macro", "per-segment"]:
+        raise ValueError(f"'{mode}' is not a valid method of mode.")
+
+    if mode == "macro":
+        fig, ax = plt.subplots(figsize=figsize)
+        correlation_matrix = get_correlation_matrix(ts, columns, segments, method)
+        labels = list(ts[:, segments, columns].columns.values)
+        ax = sns.heatmap(correlation_matrix, annot=True, fmt=".1g", square=True, ax=ax, **heatmap_kwargs)
+        ax.set_xticks(np.arange(len(labels)) + 0.5, labels=labels)
+        ax.set_yticks(np.arange(len(labels)) + 0.5, labels=labels)
+        plt.setp(ax.get_xticklabels(), rotation=45, ha="right", rotation_mode="anchor")
+        plt.setp(ax.get_yticklabels(), rotation=0, ha="right", rotation_mode="anchor")
+        ax.set_title("Correlation Heatmap")
+
+    if mode == "per-segment":
+        fig, ax = _prepare_axes(len(segments), columns_num=columns_num, figsize=figsize)
+
+        for i, segment in enumerate(segments):
+            correlation_matrix = get_correlation_matrix(ts, columns, [segment], method)
+            labels = list(ts[:, segment, columns].columns.values)
+            ax[i] = sns.heatmap(correlation_matrix, annot=True, fmt=".1g", square=True, ax=ax[i], **heatmap_kwargs)
+            ax[i].set_xticks(np.arange(len(labels)) + 0.5, labels=labels)
+            ax[i].set_yticks(np.arange(len(labels)) + 0.5, labels=labels)
+            plt.setp(ax[i].get_xticklabels(), rotation=45, ha="right", rotation_mode="anchor")
+            plt.setp(ax[i].get_yticklabels(), rotation=0, ha="right", rotation_mode="anchor")
+            ax[i].set_title("Correlation Heatmap" + " " + segment)
+
+
+def plot_clusters(
+    ts: "TSDataset",
+    segment2cluster: Dict[str, int],
+    centroids_df: Optional[pd.DataFrame] = None,
+    columns_num: int = 2,
+    figsize: Tuple[int, int] = (10, 5),
+):
+    """Plot clusters [with centroids].
+
+    Parameters
+    ----------
+    ts:
+        TSDataset with timeseries
+    segment2cluster:
+        mapping from segment to cluster in format {segment: cluster}
+    centroids_df:
+        dataframe with centroids
+    columns_num:
+        number of columns in subplots
+    figsize:
+        size of the figure per subplot with one segment in inches
+    """
+    unique_clusters = sorted(set(segment2cluster.values()))
+    _, ax = _prepare_axes(num_plots=len(unique_clusters), columns_num=columns_num, figsize=figsize)
+
+    default_colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
+    segment_color = default_colors[0]
+    for i, cluster in enumerate(unique_clusters):
+        segments = [segment for segment in segment2cluster if segment2cluster[segment] == cluster]
+        for segment in segments:
+            segment_slice = ts[:, segment, "target"]
+            ax[i].plot(
+                segment_slice.index.values,
+                segment_slice.values,
+                alpha=1 / math.sqrt(len(segments)),
+                c=segment_color,
+            )
+        ax[i].set_title(f"cluster={cluster}\n{len(segments)} segments in cluster")
+        if centroids_df is not None:
+            centroid = centroids_df[cluster, "target"]
+            ax[i].plot(centroid.index.values, centroid.values, c="red", label="centroid")
+        ax[i].legend()
+
+
+def plot_periodogram(
+    ts: "TSDataset",
+    period: float,
+    amplitude_aggregation_mode: Union[str, Literal["per-segment"]] = AggregationMode.mean,
+    periodogram_params: Optional[Dict[str, Any]] = None,
+    segments: Optional[List[str]] = None,
+    xticks: Optional[List[Any]] = None,
+    columns_num: int = 2,
+    figsize: Tuple[int, int] = (10, 5),
+):
+    """Plot the periodogram using :py:func:`scipy.signal.periodogram`.
+
+    It is useful to determine the optimal ``order`` parameter
+    for :py:class:`~etna.transforms.timestamp.fourier.FourierTransform`.
+
+    Parameters
+    ----------
+    ts:
+        TSDataset with timeseries data
+    period:
+        the period of the seasonality to capture in frequency units of time series, it should be >= 2;
+        it is translated to the ``fs`` parameter of :py:func:`scipy.signal.periodogram`
+    amplitude_aggregation_mode:
+        aggregation strategy for obtained per segment periodograms;
+        all the strategies can be examined
+        at :py:class:`~etna.analysis.feature_selection.mrmr_selection.AggregationMode`
+    periodogram_params:
+        additional keyword arguments for periodogram, :py:func:`scipy.signal.periodogram` is used
+    segments:
+        segments to use
+    xticks:
+        list of tick locations of the x-axis, useful to highlight specific reference periodicities
+    columns_num:
+        if ``amplitude_aggregation_mode="per-segment"`` number of columns in subplots, otherwise the value is ignored
+    figsize:
+        size of the figure per subplot with one segment in inches
+
+    Raises
+    ------
+    ValueError:
+        if period < 2
+    ValueError:
+        if periodogram can't be calculated on segment because of the NaNs inside it
+
+    Notes
+    -----
+    In non per-segment mode all segments are cut to be the same length, the last values are taken.
+    """
+    if period < 2:
+        raise ValueError("Period should be at least 2")
+    if periodogram_params is None:
+        periodogram_params = {}
+    if not segments:
+        segments = sorted(ts.segments)
+
+    df = ts.to_pandas()
+
+    # plot periodograms
+    if amplitude_aggregation_mode == "per-segment":
+        _, ax = _prepare_axes(num_plots=len(segments), columns_num=columns_num, figsize=figsize)
+        for i, segment in enumerate(segments):
+            segment_df = df.loc[:, pd.IndexSlice[segment, "target"]]
+            segment_df = segment_df[segment_df.first_valid_index() : segment_df.last_valid_index()]
+            if segment_df.isna().any():
+                raise ValueError(f"Periodogram can't be calculated on segment with NaNs inside: {segment}")
+            frequencies, spectrum = periodogram(x=segment_df, fs=period, **periodogram_params)
+            spectrum = spectrum[frequencies >= 1]
+            frequencies = frequencies[frequencies >= 1]
+            ax[i].step(frequencies, spectrum)
+            ax[i].set_xscale("log")
+            ax[i].set_xlabel("Frequency")
+            ax[i].set_ylabel("Power spectral density")
+            if xticks is not None:
+                ax[i].set_xticks(ticks=xticks, labels=xticks)
+            ax[i].set_title(f"Periodogram: {segment}")
+    else:
+        # find length of each segment
+        lengths_segments = []
+        for segment in segments:
+            segment_df = df.loc[:, pd.IndexSlice[segment, "target"]]
+            segment_df = segment_df[segment_df.first_valid_index() : segment_df.last_valid_index()]
+            if segment_df.isna().any():
+                raise ValueError(f"Periodogram can't be calculated on segment with NaNs inside: {segment}")
+            lengths_segments.append(len(segment_df))
+        cut_length = min(lengths_segments)
+
+        # cut each segment to `cut_length` last elements and find periodogram for each segment
+        frequencies_segments = []
+        spectrums_segments = []
+        for segment in segments:
+            segment_df = df.loc[:, pd.IndexSlice[segment, "target"]]
+            segment_df = segment_df[segment_df.first_valid_index() : segment_df.last_valid_index()][-cut_length:]
+            frequencies, spectrum = periodogram(x=segment_df, fs=period, **periodogram_params)
+            frequencies_segments.append(frequencies)
+            spectrums_segments.append(spectrum)
+
+        frequencies = frequencies_segments[0]
+        amplitude_aggregation_fn = AGGREGATION_FN[AggregationMode(amplitude_aggregation_mode)]
+        spectrum = amplitude_aggregation_fn(spectrums_segments, axis=0)  # type: ignore
+        spectrum = spectrum[frequencies >= 1]
+        frequencies = frequencies[frequencies >= 1]
+        _, ax = plt.subplots(figsize=figsize, constrained_layout=True)
+        ax.step(frequencies, spectrum)  # type: ignore
+        ax.set_xscale("log")  # type: ignore
+        ax.set_xlabel("Frequency")  # type: ignore
+        ax.set_ylabel("Power spectral density")  # type: ignore
+        if xticks is not None:
+            ax.set_xticks(ticks=xticks, labels=xticks)  # type: ignore
+        ax.set_title("Periodogram")  # type: ignore
+        ax.grid()  # type: ignore
+
+
+def plot_holidays(
+    ts: "TSDataset",
+    holidays: Union[str, pd.DataFrame],
+    segments: Optional[List[str]] = None,
+    columns_num: int = 2,
+    figsize: Tuple[int, int] = (10, 5),
+    start: Optional[str] = None,
+    end: Optional[str] = None,
+    as_is: bool = False,
+):
+    """Plot holidays for segments.
+
+    Sequence of timestamps with one holiday is drawn as a colored region.
+    Individual holiday is drawn like a colored point.
+
+    It is not possible to distinguish points plotted at one timestamp, but this case is considered rare.
+    This the problem isn't relevant for region drawing because they are partially transparent.
+
+    Parameters
+    ----------
+    ts:
+        TSDataset with timeseries data
+    holidays:
+        there are several options:
+
+        * if str, then this is code of the country in `holidays <https://pypi.org/project/holidays/>`_ library;
+
+        * if DataFrame, then dataframe is expected to be in prophet`s holiday format;
+
+    segments:
+        segments to use
+    columns_num:
+        number of columns in subplots
+    figsize:
+        size of the figure per subplot with one segment in inches
+    as_is:
+        * | Use this option if DataFrame is represented as a dataframe with a timestamp index and holiday names columns.
+          | In a holiday column values 0 represent absence of holiday in that timestamp, 1 represent the presence.
+    start:
+        start timestamp for plot
+    end:
+        end timestamp for plot
+
+    Raises
+    ------
+    ValueError:
+        * Holiday nor pd.DataFrame or String.
+        * Holiday is an empty pd.DataFrame.
+        * `as_is=True` while holiday is String.
+        * If upper_window is negative.
+        * If lower_window is positive.
+
+    """
+    start, end = _get_borders_ts(ts, start, end)
+
+    if segments is None:
+        segments = sorted(ts.segments)
+
+    holidays_df = _create_holidays_df(holidays, index=ts.index, as_is=as_is)
+
+    _, ax = _prepare_axes(num_plots=len(segments), columns_num=columns_num, figsize=figsize)
+
+    df = ts.to_pandas()
+
+    for i, segment in enumerate(segments):
+        segment_df = df.loc[start:end, pd.IndexSlice[segment, "target"]]  # type: ignore
+        segment_df = segment_df[segment_df.first_valid_index() : segment_df.last_valid_index()]
+
+        # plot target on segment
+        target_plot = ax[i].plot(segment_df.index, segment_df)
+        target_color = target_plot[0].get_color()
+
+        # plot holidays on segment
+        # remember color of each holiday to reuse it
+        default_colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
+        default_colors.remove(target_color)
+        color_cycle = itertools.cycle(default_colors)
+        holidays_colors = {holiday_name: next(color_cycle) for holiday_name in holidays_df.columns}
+
+        for holiday_name in holidays_df.columns:
+            holiday_df = holidays_df.loc[segment_df.index, holiday_name]
+            for _, holiday_group in itertools.groupby(enumerate(holiday_df.tolist()), key=lambda x: x[1]):
+                holiday_group_cached = list(holiday_group)
+                indices = [x[0] for x in holiday_group_cached]
+                values = [x[1] for x in holiday_group_cached]
+
+                # if we have group with zero value, then it is not a holidays, skip it
+                if values[0] == 0:
+                    continue
+
+                color = holidays_colors[holiday_name]
+                if len(indices) == 1:
+                    # plot individual holiday point
+                    ax[i].scatter(segment_df.index[indices[0]], segment_df.iloc[indices[0]], color=color, zorder=2)
+                else:
+                    # plot span with holiday borders
+                    x_min = segment_df.index[indices[0]]
+                    x_max = segment_df.index[indices[-1]]
+                    ax[i].axvline(x_min, color=color, linestyle="dashed")
+                    ax[i].axvline(x_max, color=color, linestyle="dashed")
+                    ax[i].axvspan(xmin=x_min, xmax=x_max, alpha=1 / 4, color=color)
+
+        ax[i].set_title(segment)
+        ax[i].tick_params("x", rotation=45)
+
+        legend_handles = [
+            Line2D([0], [0], marker="o", color=color, label=label) for label, color in holidays_colors.items()
+        ]
+        ax[i].legend(handles=legend_handles)
+
+
+def _cross_correlation(
+    a: np.ndarray, b: np.ndarray, maxlags: Optional[int] = None, normed: bool = True
+) -> Tuple[np.ndarray, np.ndarray]:
+    """Calculate cross correlation between arrays.
+
+    This implementation is slow: O(n^2), but can properly ignore NaNs.
+
+    Parameters
+    ----------
+    a:
+        first array, should be equal length with b
+    b:
+        second array, should be equal length with a
+    maxlags:
+        number of lags to compare, should be >=1 and < len(a)
+    normed:
+        should correlations be normed or not
+
+    Returns
+    -------
+    lags, result:
+
+        * lags: array of size ``maxlags * 2 + 1`` represents for which lags correlations are calculated in ``result``
+
+        * result: array of size ``maxlags * 2 + 1`` represents found correlations
+
+    Raises
+    ------
+    ValueError:
+        lengths of ``a`` and ``b`` are not the same
+    ValueError:
+        parameter ``maxlags`` doesn't satisfy constraints
+    """
+    if len(a) != len(b):
+        raise ValueError("Lengths of arrays should be equal")
+
+    length = len(a)
+
+    if maxlags is None:
+        maxlags = length - 1
+
+    if maxlags < 1 or maxlags >= length:
+        raise ValueError("Parameter maxlags should be >= 1 and < len(a)")
+
+    result = []
+    lags = np.arange(-maxlags, maxlags + 1)
+    for lag in lags:
+        if lag < 0:
+            cur_a = a[:lag]
+            cur_b = b[-lag:]
+        elif lag == 0:
+            cur_a = a
+            cur_b = b
+        else:
+            cur_a = a[lag:]
+            cur_b = b[:-lag]
+        dot_product = np.nansum(cur_a * cur_b)
+        if normed:
+            nan_mask_a = np.isnan(cur_a)
+            nan_mask_b = np.isnan(cur_b)
+            nan_mask = nan_mask_a | nan_mask_b
+            normed_dot_product = dot_product / np.sqrt(
+                np.sum(cur_a[~nan_mask] * cur_a[~nan_mask]) * np.sum(cur_b[~nan_mask] * cur_b[~nan_mask])
+            )
+            normed_dot_product = np.nan_to_num(normed_dot_product)
+            result.append(normed_dot_product)
+        else:
+            result.append(dot_product)
+    return lags, np.array(result)
+
+
 def cross_corr_plot(
     ts: "TSDataset",
     n_segments: int = 10,
     maxlags: int = 21,
     segments: Optional[List[str]] = None,
+    columns_num: int = 2,
     figsize: Tuple[int, int] = (10, 5),
 ):
     """
     Cross-correlation plot between multiple timeseries.
 
     Parameters
     ----------
     ts:
         TSDataset with timeseries data
     n_segments:
-        number of random segments to plot
+        number of random segments to plot, ignored if parameter ``segments`` is set
     maxlags:
-        number of timeseries shifts for cross-correlation
+        number of timeseries shifts for cross-correlation, should be >=1 and <= len(timeseries)
     segments:
         segments to plot
+    columns_num:
+        number of columns in subplots
     figsize:
         size of the figure per subplot with one segment in inches
+
+    Raises
+    ------
+    ValueError:
+        parameter ``maxlags`` doesn't satisfy constraints
     """
     if segments is None:
         exist_segments = list(ts.segments)
         chosen_segments = np.random.choice(exist_segments, size=min(len(exist_segments), n_segments), replace=False)
         segments = list(chosen_segments)
+
     segment_pairs = list(combinations(segments, r=2))
     if len(segment_pairs) == 0:
         raise ValueError("There are no pairs to plot! Try set n_segments > 1.")
-    columns_num = min(2, len(segment_pairs))
-    rows_num = math.ceil(len(segment_pairs) / columns_num)
 
-    figsize = (figsize[0] * columns_num, figsize[1] * rows_num)
-    fig, ax = plt.subplots(rows_num, columns_num, figsize=figsize, constrained_layout=True, squeeze=False)
-    ax = ax.ravel()
+    fig, ax = _prepare_axes(num_plots=len(segment_pairs), columns_num=columns_num, figsize=figsize)
     fig.suptitle("Cross-correlation", fontsize=16)
+
+    df = ts.to_pandas()
+
     for i, (segment_1, segment_2) in enumerate(segment_pairs):
-        df_segment_1 = ts[:, segment_1, :][segment_1]
-        df_segment_2 = ts[:, segment_2, :][segment_2]
-        fig, axx = utils.create_mpl_ax(ax[i])
-        target_1 = df_segment_1.target
-        target_2 = df_segment_2.target
+        target_1 = df.loc[:, pd.IndexSlice[segment_1, "target"]]
+        target_2 = df.loc[:, pd.IndexSlice[segment_2, "target"]]
+
         if target_1.dtype == int or target_2.dtype == int:
             warnings.warn(
                 "At least one target column has integer dtype, "
                 "it is converted to float in order to calculate correlation."
             )
             target_1 = target_1.astype(float)
             target_2 = target_2.astype(float)
-        lags, level, _, _ = axx.xcorr(x=target_1, y=target_2, maxlags=maxlags)
-        ax[i].plot(lags, level, "o", markersize=5)
+
+        lags, correlations = _cross_correlation(a=target_1.values, b=target_2.values, maxlags=maxlags, normed=True)
+        ax[i].plot(lags, correlations, "-o", markersize=5)
         ax[i].set_title(f"{segment_1} vs {segment_2}")
         ax[i].xaxis.set_major_locator(MaxNLocator(integer=True))
-    plt.show()
 
 
-def sample_acf_plot(
+def acf_plot(
     ts: "TSDataset",
     n_segments: int = 10,
     lags: int = 21,
+    partial: bool = False,
+    columns_num: int = 2,
     segments: Optional[List[str]] = None,
     figsize: Tuple[int, int] = (10, 5),
 ):
     """
-    Autocorrelation plot for multiple timeseries.
-
+    Autocorrelation and partial autocorrelation plot for multiple timeseries.
 
     Notes
     -----
     `Definition of autocorrelation <https://en.wikipedia.org/wiki/Autocorrelation>`_.
 
+    `Definition of partial autocorrelation <https://en.wikipedia.org/wiki/Partial_autocorrelation_function>`_.
+
+    * If ``partial=False`` function works with NaNs at any place of the time-series.
+
+    * if ``partial=True`` function works only with NaNs at the edges of the time-series and fails if there are NaNs inside it.
+
     Parameters
     ----------
     ts:
         TSDataset with timeseries data
     n_segments:
         number of random segments to plot
     lags:
         number of timeseries shifts for cross-correlation
+    partial:
+        plot autocorrelation or partial autocorrelation
+    columns_num:
+        number of columns in subplots
     segments:
         segments to plot
     figsize:
         size of the figure per subplot with one segment in inches
+
+    Raises
+    ------
+    ValueError:
+        If partial=True and there is a NaN in the middle of the time series
     """
     if segments is None:
-        segments = sorted(ts.segments)
-
-    k = min(n_segments, len(segments))
-    columns_num = min(2, k)
-    rows_num = math.ceil(k / columns_num)
+        exist_segments = sorted(ts.segments)
+        chosen_segments = np.random.choice(exist_segments, size=min(len(exist_segments), n_segments), replace=False)
+        segments = list(chosen_segments)
 
-    figsize = (figsize[0] * columns_num, figsize[1] * rows_num)
-    fig, ax = plt.subplots(rows_num, columns_num, figsize=figsize, constrained_layout=True, squeeze=False)
-    ax = ax.ravel()
-    fig.suptitle("Autocorrelation", fontsize=16)
-    for i, name in enumerate(sorted(np.random.choice(segments, size=k, replace=False))):
-        df_slice = ts[:, name, :][name]
-        plot_acf(x=df_slice["target"].values, ax=ax[i], lags=lags)
-        ax[i].set_title(name)
-    plt.show()
+    title = "Partial Autocorrelation" if partial else "Autocorrelation"
 
+    fig, ax = _prepare_axes(num_plots=len(segments), columns_num=columns_num, figsize=figsize)
+    fig.suptitle(title, fontsize=16)
 
-def sample_pacf_plot(
-    ts: "TSDataset",
-    n_segments: int = 10,
-    lags: int = 21,
-    segments: Optional[List[str]] = None,
-    figsize: Tuple[int, int] = (10, 5),
-):
-    """
-    Partial autocorrelation plot for multiple timeseries.
-
-    Notes
-    -----
-    `Definition of partial autocorrelation <https://en.wikipedia.org/wiki/Partial_autocorrelation_function>`_.
+    df = ts.to_pandas()
 
-    Parameters
-    ----------
-    ts:
-        TSDataset with timeseries data
-    n_segments:
-        number of random segments to plot
-    lags:
-        number of timeseries shifts for cross-correlation
-    segments:
-        segments to plot
-    figsize:
-        size of the figure per subplot with one segment in inches
-    """
-    if segments is None:
-        segments = sorted(ts.segments)
+    for i, name in enumerate(segments):
+        df_slice = df[name].reset_index()["target"]
+        if partial:
+            # for partial autocorrelation remove NaN from the beginning and end of the series
+            begin = df_slice.first_valid_index()
+            end = df_slice.last_valid_index()
+            x = df_slice.values[begin:end]
+            if np.isnan(x).any():
+                raise ValueError("There is a NaN in the middle of the time series!")
+            plot_pacf(x=x, ax=ax[i], lags=lags)
 
-    k = min(n_segments, len(segments))
-    columns_num = min(2, k)
-    rows_num = math.ceil(k / columns_num)
+        if not partial:
+            plot_acf(x=df_slice.values, ax=ax[i], lags=lags, missing="conservative")
 
-    figsize = (figsize[0] * columns_num, figsize[1] * rows_num)
-    fig, ax = plt.subplots(rows_num, columns_num, figsize=figsize, constrained_layout=True, squeeze=False)
-    ax = ax.ravel()
-    fig.suptitle("Partial Autocorrelation", fontsize=16)
-    for i, name in enumerate(sorted(np.random.choice(segments, size=k, replace=False))):
-        df_slice = ts[:, name, :][name]
-        plot_pacf(x=df_slice["target"].values, ax=ax[i], lags=lags)
         ax[i].set_title(name)
+
     plt.show()
 
 
 def distribution_plot(
     ts: "TSDataset",
     n_segments: int = 10,
     segments: Optional[List[str]] = None,
@@ -244,518 +648,69 @@
     ax = ax.ravel()
     i = 0
     for period, df_slice in grouped_data:
         if period not in groups:
             continue
         sns.boxplot(data=df_slice.sort_values(by="segment"), y="z", x="segment", ax=ax[i], fliersize=False)
         ax[i].set_title(f"{period}")
+        ax[i].grid()
         i += 1
 
 
-def stl_plot(
-    ts: "TSDataset",
-    period: int,
-    segments: Optional[List[str]] = None,
-    columns_num: int = 2,
-    figsize: Tuple[int, int] = (10, 10),
-    plot_kwargs: Optional[Dict[str, Any]] = None,
-    stl_kwargs: Optional[Dict[str, Any]] = None,
-):
-    """Plot STL decomposition for segments.
-
-    Parameters
-    ----------
-    ts:
-        dataset with timeseries data
-    period:
-        length of seasonality
-    segments:
-        segments to plot
-    columns_num:
-        number of columns in subplots
-    figsize:
-        size of the figure per subplot with one segment in inches
-    plot_kwargs:
-        dictionary with parameters for plotting, :py:meth:`matplotlib.axes.Axes.plot` is used
-    stl_kwargs:
-        dictionary with parameters for STL decomposition, :py:class:`statsmodels.tsa.seasonal.STL` is used
-    """
-    if plot_kwargs is None:
-        plot_kwargs = {}
-    if stl_kwargs is None:
-        stl_kwargs = {}
-    if segments is None:
-        segments = sorted(ts.segments)
-
-    in_column = "target"
-
-    segments_number = len(segments)
-    columns_num = min(columns_num, len(segments))
-    rows_num = math.ceil(segments_number / columns_num)
-
-    figsize = (figsize[0] * columns_num, figsize[1] * rows_num)
-    fig = plt.figure(figsize=figsize, constrained_layout=True)
-    subfigs = fig.subfigures(rows_num, columns_num, squeeze=False)
-
-    df = ts.to_pandas()
-    for i, segment in enumerate(segments):
-        segment_df = df.loc[:, pd.IndexSlice[segment, :]][segment]
-        segment_df = segment_df[segment_df.first_valid_index() : segment_df.last_valid_index()]
-        decompose_result = STL(endog=segment_df[in_column], period=period, **stl_kwargs).fit()
-
-        # start plotting
-        subfigs.flat[i].suptitle(segment)
-        axs = subfigs.flat[i].subplots(4, 1, sharex=True)
-
-        # plot observed
-        axs.flat[0].plot(segment_df.index, decompose_result.observed, **plot_kwargs)
-        axs.flat[0].set_ylabel("Observed")
-
-        # plot trend
-        axs.flat[1].plot(segment_df.index, decompose_result.trend, **plot_kwargs)
-        axs.flat[1].set_ylabel("Trend")
-
-        # plot seasonal
-        axs.flat[2].plot(segment_df.index, decompose_result.seasonal, **plot_kwargs)
-        axs.flat[2].set_ylabel("Seasonal")
-
-        # plot residuals
-        axs.flat[3].plot(segment_df.index, decompose_result.resid, **plot_kwargs)
-        axs.flat[3].set_ylabel("Residual")
-        axs.flat[3].tick_params("x", rotation=45)
-
-
-def qq_plot(
-    residuals_ts: "TSDataset",
-    qq_plot_params: Optional[Dict[str, Any]] = None,
-    segments: Optional[List[str]] = None,
-    columns_num: int = 2,
-    figsize: Tuple[int, int] = (10, 5),
-):
-    """Plot Q-Q plots for segments.
-
-    Parameters
-    ----------
-    residuals_ts:
-        dataset with the time series, expected to be the residuals of the model
-    qq_plot_params:
-        dictionary with parameters for qq plot, :py:func:`statsmodels.graphics.gofplots.qqplot` is used
-    segments:
-        segments to plot
-    columns_num:
-        number of columns in subplots
-    figsize:
-        size of the figure per subplot with one segment in inches
-    """
-    if qq_plot_params is None:
-        qq_plot_params = {}
-    if segments is None:
-        segments = sorted(residuals_ts.segments)
-
-    ax = prepare_axes(segments=segments, columns_num=columns_num, figsize=figsize)
-
-    residuals_df = residuals_ts.to_pandas()
-    for i, segment in enumerate(segments):
-        residuals_segment = residuals_df.loc[:, pd.IndexSlice[segment, "target"]]
-        qqplot(residuals_segment, ax=ax[i], **qq_plot_params)
-        ax[i].set_title(segment)
-
-
-def prediction_actual_scatter_plot(
-    forecast_df: pd.DataFrame,
-    ts: "TSDataset",
-    segments: Optional[List[str]] = None,
-    columns_num: int = 2,
-    figsize: Tuple[int, int] = (10, 5),
-):
-    """Plot scatter plot with forecasted/actual values for segments.
-
-    Parameters
-    ----------
-    forecast_df:
-        forecasted dataframe with timeseries data
-    ts:
-        dataframe of timeseries that was used for backtest
-    segments:
-        segments to plot
-    columns_num:
-        number of columns in subplots
-    figsize:
-        size of the figure per subplot with one segment in inches
-    """
-    if segments is None:
-        segments = sorted(ts.segments)
-
-    ax = prepare_axes(segments=segments, columns_num=columns_num, figsize=figsize)
-
-    df = ts.to_pandas()
-    for i, segment in enumerate(segments):
-        forecast_segment_df = forecast_df.loc[:, pd.IndexSlice[segment, "target"]]
-        segment_df = df.loc[forecast_segment_df.index, pd.IndexSlice[segment, "target"]]
-
-        # fit a linear model
-        x = forecast_segment_df.values
-        y = segment_df
-        model = LinearRegression()
-        model.fit(X=x[:, np.newaxis], y=y)
-        r2 = r2_score(y_true=y, y_pred=model.predict(x[:, np.newaxis]))
-
-        # prepare the limits of the plot, for the identity to be from corner to corner
-        x_min = min(x.min(), y.min())
-        x_max = max(x.max(), y.max())
-        # add some space at the borders of the plot
-        x_min -= 0.05 * (x_max - x_min)
-        x_max += 0.05 * (x_max - x_min)
-        xlim = (x_min, x_max)
-        ylim = xlim
-
-        # make plots
-        ax[i].scatter(x, y, label=f"R2: {r2:.3f}")
-        x_grid = np.linspace(*xlim, 100)
-        ax[i].plot(x_grid, x_grid, label="identity", linestyle="dotted", color="grey")
-        ax[i].plot(
-            x_grid,
-            model.predict(x_grid[:, np.newaxis]),
-            label=f"best fit: {model.coef_[0]:.3f} x + {model.intercept_:.3f}",
-            linestyle="dashed",
-            color="black",
-        )
-        ax[i].set_title(segment)
-        ax[i].set_xlabel("$\\widehat{y}$")
-        ax[i].set_ylabel("$y$")
-        ax[i].set_xlim(*xlim)
-        ax[i].set_ylim(*ylim)
-        ax[i].legend()
-
-
-class SeasonalPlotAlignment(str, Enum):
-    """Enum for types of alignment in a seasonal plot.
-
-    Attributes
-    ----------
-    first:
-        make first period full, allow last period to have NaNs in the ending
-    last:
-        make last period full, allow first period to have NaNs in the beginning
-    """
-
-    first = "first"
-    last = "last"
-
-    @classmethod
-    def _missing_(cls, value):
-        raise NotImplementedError(
-            f"{value} is not a valid {cls.__name__}. Only {', '.join([repr(m.value) for m in cls])} alignments are allowed"
-        )
-
-
-class SeasonalPlotAggregation(str, Enum):
-    """Enum for types of aggregation in a seasonal plot."""
-
-    mean = "mean"
-    sum = "sum"
-
-    @classmethod
-    def _missing_(cls, value):
-        raise NotImplementedError(
-            f"{value} is not a valid {cls.__name__}. Only {', '.join([repr(m.value) for m in cls])} aggregations are allowed"
-        )
-
-    @staticmethod
-    def _modified_nansum(series):
-        """Sum values with ignoring of NaNs.
-
-        * If there some nan: we skip them.
-
-        * If all values equal to nan we return nan.
-        """
-        if np.all(np.isnan(series)):
-            return np.NaN
-        else:
-            return np.nansum(series)
-
-    def get_function(self):
-        """Get aggregation function."""
-        if self.value == "mean":
-            return np.nanmean
-        elif self.value == "sum":
-            return self._modified_nansum
-
-
-class SeasonalPlotCycle(str, Enum):
-    """Enum for types of cycles in a seasonal plot."""
-
-    hour = "hour"
-    day = "day"
-    week = "week"
-    month = "month"
-    quarter = "quarter"
-    year = "year"
-
-    @classmethod
-    def _missing_(cls, value):
-        raise NotImplementedError(
-            f"{value} is not a valid {cls.__name__}. Only {', '.join([repr(m.value) for m in cls])} cycles are allowed"
-        )
-
-
-def _get_seasonal_cycle_name(
-    timestamp: pd.Series,
-    cycle: Union[
-        Literal["hour"], Literal["day"], Literal["week"], Literal["month"], Literal["quarter"], Literal["year"], int
-    ],
-) -> pd.Series:
-    """Get unique name for each cycle in a series with timestamps."""
-    cycle_functions: Dict[SeasonalPlotCycle, Callable[[pd.Series], pd.Series]] = {
-        SeasonalPlotCycle.hour: lambda x: x.dt.strftime("%Y-%m-%d %H"),
-        SeasonalPlotCycle.day: lambda x: x.dt.strftime("%Y-%m-%d"),
-        SeasonalPlotCycle.week: lambda x: x.dt.strftime("%Y-%W"),
-        SeasonalPlotCycle.month: lambda x: x.dt.strftime("%Y-%b"),
-        SeasonalPlotCycle.quarter: lambda x: x.apply(lambda x: f"{x.year}-{x.quarter}"),
-        SeasonalPlotCycle.year: lambda x: x.dt.strftime("%Y"),
-    }
-
-    if isinstance(cycle, int):
-        row_numbers = pd.Series(np.arange(len(timestamp)))
-        return (row_numbers // cycle + 1).astype(str)
-    else:
-        return cycle_functions[SeasonalPlotCycle(cycle)](timestamp)
-
-
-def _get_seasonal_in_cycle_num(
-    timestamp: pd.Series,
-    cycle_name: pd.Series,
-    cycle: Union[
-        Literal["hour"], Literal["day"], Literal["week"], Literal["month"], Literal["quarter"], Literal["year"], int
-    ],
-    freq: str,
-) -> pd.Series:
-    """Get number for each point within cycle in a series of timestamps."""
-    cycle_functions: Dict[Tuple[SeasonalPlotCycle, str], Callable[[pd.Series], pd.Series]] = {
-        (SeasonalPlotCycle.hour, "T"): lambda x: x.dt.minute,
-        (SeasonalPlotCycle.day, "H"): lambda x: x.dt.hour,
-        (SeasonalPlotCycle.week, "D"): lambda x: x.dt.weekday,
-        (SeasonalPlotCycle.month, "D"): lambda x: x.dt.day,
-        (SeasonalPlotCycle.quarter, "D"): lambda x: (x - pd.PeriodIndex(x, freq="Q").start_time).dt.days,
-        (SeasonalPlotCycle.year, "D"): lambda x: x.dt.dayofyear,
-        (SeasonalPlotCycle.year, "Q"): lambda x: x.dt.quarter,
-        (SeasonalPlotCycle.year, "QS"): lambda x: x.dt.quarter,
-        (SeasonalPlotCycle.year, "M"): lambda x: x.dt.month,
-        (SeasonalPlotCycle.year, "MS"): lambda x: x.dt.month,
-    }
-
-    if isinstance(cycle, int):
-        pass
-    else:
-        key = (SeasonalPlotCycle(cycle), freq)
-        if key in cycle_functions:
-            return cycle_functions[key](timestamp)
-
-    # in all other cases we can use numbers within each group
-    cycle_df = pd.DataFrame({"timestamp": timestamp.tolist(), "cycle_name": cycle_name.tolist()})
-    return cycle_df.sort_values("timestamp").groupby("cycle_name").cumcount()
-
-
-def _get_seasonal_in_cycle_name(
-    timestamp: pd.Series,
-    in_cycle_num: pd.Series,
-    cycle: Union[
-        Literal["hour"], Literal["day"], Literal["week"], Literal["month"], Literal["quarter"], Literal["year"], int
-    ],
-    freq: str,
-) -> pd.Series:
-    """Get unique name for each point within the cycle in a series of timestamps."""
-    if isinstance(cycle, int):
-        pass
-    elif SeasonalPlotCycle(cycle) == SeasonalPlotCycle.week:
-        if freq == "D":
-            return timestamp.dt.strftime("%a")
-    elif SeasonalPlotCycle(cycle) == SeasonalPlotCycle.year:
-        if freq == "M" or freq == "MS":
-            return timestamp.dt.strftime("%b")
-
-    # in all other cases we can use numbers from cycle_num
-    return in_cycle_num.astype(str)
-
-
-def _seasonal_split(
-    timestamp: pd.Series,
-    freq: str,
-    cycle: Union[
-        Literal["hour"], Literal["day"], Literal["week"], Literal["month"], Literal["quarter"], Literal["year"], int
-    ],
-) -> pd.DataFrame:
-    """Create a seasonal split into cycles of a given timestamp.
-
-    Parameters
-    ----------
-    timestamp:
-        series with timestamps
-    freq:
-        frequency of dataframe
-    cycle:
-        period of seasonality to capture (see :py:class:`~etna.analysis.eda_utils.SeasonalPlotCycle`)
-
-    Returns
-    -------
-    result: pd.DataFrame
-        dataframe with timestamps and corresponding cycle names and in cycle names
-    """
-    cycles_df = pd.DataFrame({"timestamp": timestamp.tolist()})
-    cycles_df["cycle_name"] = _get_seasonal_cycle_name(timestamp=cycles_df["timestamp"], cycle=cycle)
-    cycles_df["in_cycle_num"] = _get_seasonal_in_cycle_num(
-        timestamp=cycles_df["timestamp"], cycle_name=cycles_df["cycle_name"], cycle=cycle, freq=freq
-    )
-    cycles_df["in_cycle_name"] = _get_seasonal_in_cycle_name(
-        timestamp=cycles_df["timestamp"], in_cycle_num=cycles_df["in_cycle_num"], cycle=cycle, freq=freq
-    )
-    return cycles_df
-
-
-def _resample(df: pd.DataFrame, freq: str, aggregation: Union[Literal["sum"], Literal["mean"]]) -> pd.DataFrame:
-    from etna.datasets import TSDataset
-
-    agg_enum = SeasonalPlotAggregation(aggregation)
-    df_flat = TSDataset.to_flatten(df)
-    df_flat = (
-        df_flat.set_index("timestamp")
-        .groupby(["segment", pd.Grouper(freq=freq)])
-        .agg(agg_enum.get_function())
-        .reset_index()
-    )
-    df = TSDataset.to_dataset(df_flat)
-    return df
-
-
-def _prepare_seasonal_plot_df(
-    ts: "TSDataset",
-    freq: str,
-    cycle: Union[
-        Literal["hour"], Literal["day"], Literal["week"], Literal["month"], Literal["quarter"], Literal["year"], int
-    ],
-    alignment: Union[Literal["first"], Literal["last"]],
-    aggregation: Union[Literal["sum"], Literal["mean"]],
-    in_column: str,
-    segments: List[str],
-):
-    # for simplicity we will rename our column to target
-    df = ts.to_pandas().loc[:, pd.IndexSlice[segments, in_column]]
-    df.rename(columns={in_column: "target"}, inplace=True)
-
-    # remove timestamps with only nans, it is possible if in_column != "target"
-    df = df[(~df.isna()).sum(axis=1) > 0]
-
-    # make resampling if necessary
-    if ts.freq != freq:
-        df = _resample(df=df, freq=freq, aggregation=aggregation)
-
-    # process alignment
-    if isinstance(cycle, int):
-        timestamp = df.index
-        num_to_add = -len(timestamp) % cycle
-        # if we want align by the first value, then we should append NaNs to timestamp
-        to_add_index = None
-        if SeasonalPlotAlignment(alignment) == SeasonalPlotAlignment.first:
-            to_add_index = pd.date_range(start=timestamp.max(), periods=num_to_add + 1, closed="right", freq=freq)
-        # if we want to align by the last value, then we should prepend NaNs to timestamp
-        elif SeasonalPlotAlignment(alignment) == SeasonalPlotAlignment.last:
-            to_add_index = pd.date_range(end=timestamp.min(), periods=num_to_add + 1, closed="left", freq=freq)
-
-        df = df.append(pd.DataFrame(None, index=to_add_index)).sort_index()
-
-    return df
-
-
-def seasonal_plot(
+def plot_imputation(
     ts: "TSDataset",
-    freq: Optional[str] = None,
-    cycle: Union[
-        Literal["hour"], Literal["day"], Literal["week"], Literal["month"], Literal["quarter"], Literal["year"], int
-    ] = "year",
-    alignment: Union[Literal["first"], Literal["last"]] = "last",
-    aggregation: Union[Literal["sum"], Literal["mean"]] = "sum",
-    in_column: str = "target",
-    plot_params: Optional[Dict[str, Any]] = None,
-    cmap: str = "plasma",
+    imputer: "TimeSeriesImputerTransform",
     segments: Optional[List[str]] = None,
     columns_num: int = 2,
     figsize: Tuple[int, int] = (10, 5),
+    start: Optional[str] = None,
+    end: Optional[str] = None,
 ):
-    """Plot each season on one canvas for each segment.
+    """Plot the result of imputation by a given imputer.
 
     Parameters
     ----------
     ts:
-        dataset with timeseries data
-    freq:
-        frequency to analyze seasons:
-
-        * if isn't set, the frequency of ``ts`` will be used;
-
-        * if set, resampling will be made using ``aggregation`` parameter.
-          If given frequency is too low, then the frequency of ``ts`` will be used.
-
-    cycle:
-        period of seasonality to capture (see :class:`~etna.analysis.eda_utils.SeasonalPlotCycle`)
-    alignment:
-        how to align dataframe in case of integer cycle (see :py:class:`~etna.analysis.eda_utils.SeasonalPlotAlignment`)
-    aggregation:
-        how to aggregate values during resampling (see :py:class:`~etna.analysis.eda_utils.SeasonalPlotAggregation`)
-    in_column:
-        column to use
-    cmap:
-        name of colormap for plotting different cycles
-        (see `Choosing Colormaps in Matplotlib <https://matplotlib.org/3.5.1/tutorials/colors/colormaps.html>`_)
-    plot_params:
-        dictionary with parameters for plotting, :py:meth:`matplotlib.axes.Axes.plot` is used
+        TSDataset with timeseries data
+    imputer:
+        transform to make imputation of NaNs
     segments:
         segments to use
     columns_num:
         number of columns in subplots
     figsize:
         size of the figure per subplot with one segment in inches
+    start:
+        start timestamp for plot
+    end:
+        end timestamp for plot
     """
-    if plot_params is None:
-        plot_params = {}
-    if freq is None:
-        freq = ts.freq
+    start, end = _get_borders_ts(ts, start, end)
+
     if segments is None:
         segments = sorted(ts.segments)
 
-    df = _prepare_seasonal_plot_df(
-        ts=ts,
-        freq=freq,
-        cycle=cycle,
-        alignment=alignment,
-        aggregation=aggregation,
-        in_column=in_column,
-        segments=segments,
-    )
-    seasonal_df = _seasonal_split(timestamp=df.index.to_series(), freq=freq, cycle=cycle)
+    _, ax = _prepare_axes(num_plots=len(segments), columns_num=columns_num, figsize=figsize)
+
+    ts_after = deepcopy(ts)
+    imputer.fit_transform(ts_after)
+    feature_name = imputer.in_column
 
-    colors = plt.get_cmap(cmap)
-    ax = prepare_axes(segments=segments, columns_num=columns_num, figsize=figsize)
     for i, segment in enumerate(segments):
-        segment_df = df.loc[:, pd.IndexSlice[segment, "target"]]
-        cycle_names = seasonal_df["cycle_name"].unique()
-        for j, cycle_name in enumerate(cycle_names):
-            color = colors(j / len(cycle_names))
-            cycle_df = seasonal_df[seasonal_df["cycle_name"] == cycle_name]
-            segment_cycle_df = segment_df.loc[cycle_df["timestamp"]]
-            ax[i].plot(
-                cycle_df["in_cycle_num"],
-                segment_cycle_df[cycle_df["timestamp"]],
-                color=color,
-                label=cycle_name,
-                **plot_params,
-            )
+        # we want to capture nans at the beginning, so don't use `ts[:, segment, :]`
+        segment_before_df = ts.to_pandas().loc[start:end, pd.IndexSlice[segment, feature_name]]  # type: ignore
+        segment_after_df = ts_after.to_pandas().loc[start:end, pd.IndexSlice[segment, feature_name]]  # type: ignore
+
+        # plot result after imputation
+        ax[i].plot(segment_after_df.index, segment_after_df)
+
+        # highlight imputed points
+        imputed_index = ~segment_after_df.isna() & segment_before_df.isna()
+        ax[i].scatter(
+            segment_after_df.loc[imputed_index].index,
+            segment_after_df.loc[imputed_index],
+            c="red",
+            zorder=2,
+        )
 
-        # draw ticks if they are not digits
-        if not np.all(seasonal_df["in_cycle_name"].str.isnumeric()):
-            ticks_dict = {key: value for key, value in zip(seasonal_df["in_cycle_num"], seasonal_df["in_cycle_name"])}
-            ticks = np.array(list(ticks_dict.keys()))
-            ticks_labels = np.array(list(ticks_dict.values()))
-            idx_sort = np.argsort(ticks)
-            ax[i].set_xticks(ticks=ticks[idx_sort], labels=ticks_labels[idx_sort])
-        ax[i].set_xlabel(freq)
         ax[i].set_title(segment)
-        ax[i].legend(loc="upper center", bbox_to_anchor=(0.5, -0.12), ncol=6)
+        ax[i].tick_params("x", rotation=45)
```

### Comparing `etna-1.9.0/etna/analysis/feature_relevance/relevance.py` & `etna-2.0.0/etna/analysis/feature_relevance/relevance.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/analysis/feature_relevance/relevance_table.py` & `etna-2.0.0/etna/analysis/feature_relevance/relevance_table.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/analysis/feature_selection/mrmr_selection.py` & `etna-2.0.0/etna/analysis/feature_selection/mrmr_selection.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/analysis/outliers/density_outliers.py` & `etna-2.0.0/etna/analysis/outliers/density_outliers.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/analysis/outliers/hist_outliers.py` & `etna-2.0.0/etna/analysis/outliers/hist_outliers.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     Returns
     -------
     result: float
         approximation error
     """
     if left == 0:
         avg = p[right]
-        return pp[right] - avg ** 2 / (right - left + 1)
+        return pp[right] - avg**2 / (right - left + 1)
     avg = p[right] - p[left - 1]
-    return pp[right] - pp[left - 1] - avg ** 2 / (right - left + 1)
+    return pp[right] - pp[left - 1] - avg**2 / (right - left + 1)
 
 
 @numba.jit(nopython=True)
 def adjust_estimation(i: int, k: int, sse: np.ndarray, sse_one_bin: np.ndarray) -> float:
     """
     Count sse_one_bin[i][k] using binary search.
```

### Comparing `etna-1.9.0/etna/analysis/outliers/median_outliers.py` & `etna-2.0.0/etna/analysis/outliers/median_outliers.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     -------
     :
         dict of outliers in format {segment: [outliers_timestamps]}
     """
     outliers_per_segment = {}
     segments = ts.segments
     for seg in segments:
-        anomalies = []
+        anomalies: typing.List[int] = []
 
         segment_df = ts.df[seg].reset_index()
         values = segment_df[in_column].values
         timestamp = segment_df["timestamp"].values
 
         n_iter = math.ceil(len(values) / window_size)
         for i in range(n_iter):
```

### Comparing `etna-1.9.0/etna/analysis/outliers/prediction_interval_outliers.py` & `etna-2.0.0/etna/analysis/outliers/prediction_interval_outliers.py`

 * *Files 11% similar despite different names*

```diff
@@ -78,17 +78,18 @@
     else:
         ts_inner = create_ts_by_column(ts, in_column)
     outliers_per_segment = {}
     time_points = np.array(ts.index.values)
     model_instance = model(**model_params)
     model_instance.fit(ts_inner)
     lower_p, upper_p = [(1 - interval_width) / 2, (1 + interval_width) / 2]
-    prediction_interval = model_instance.forecast(
+    prediction_interval = model_instance.predict(
         deepcopy(ts_inner), prediction_interval=True, quantiles=[lower_p, upper_p]
     )
     for segment in ts_inner.segments:
-        segment_slice = prediction_interval[:, segment, :][segment]
-        anomalies_mask = (segment_slice["target"] > segment_slice[f"target_{upper_p:.4g}"]) | (
-            segment_slice["target"] < segment_slice[f"target_{lower_p:.4g}"]
+        predicted_segment_slice = prediction_interval[:, segment, :][segment]
+        actual_segment_slice = ts_inner[:, segment, :][segment]
+        anomalies_mask = (actual_segment_slice["target"] > predicted_segment_slice[f"target_{upper_p:.4g}"]) | (
+            actual_segment_slice["target"] < predicted_segment_slice[f"target_{lower_p:.4g}"]
         )
         outliers_per_segment[segment] = list(time_points[anomalies_mask])
     return outliers_per_segment
```

### Comparing `etna-1.9.0/etna/clustering/__init__.py` & `etna-2.0.0/etna/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/clustering/base.py` & `etna-2.0.0/etna/clustering/base.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/clustering/distances/base.py` & `etna-2.0.0/etna/clustering/distances/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 if TYPE_CHECKING:
     from etna.datasets import TSDataset
 
 
 class Distance(ABC, BaseMixin):
     """Base class for distances between series."""
 
-    def __init__(self, trim_series: bool = False, inf_value: float = sys.float_info.max // 10 ** 200):
+    def __init__(self, trim_series: bool = False, inf_value: float = sys.float_info.max // 10**200):
         """Init Distance.
 
         Parameters
         ----------
         trim_series:
 
             * if True, get common (according to timestamp index) part of series and compute distance with it;
```

### Comparing `etna-1.9.0/etna/clustering/distances/distance_matrix.py` & `etna-2.0.0/etna/clustering/distances/distance_matrix.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/clustering/distances/dtw_distance.py` & `etna-2.0.0/etna/clustering/distances/dtw_distance.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/clustering/distances/euclidean_distance.py` & `etna-2.0.0/etna/clustering/distances/euclidean_distance.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 from etna.clustering.distances.base import Distance
 
 if TYPE_CHECKING:
     from etna.datasets import TSDataset
 
 
 @numba.cfunc(numba.float64(numba.float64[:], numba.float64[:]))
-def euclidean_distance(x1: np.ndarray, x2: np.ndarray) -> float:
+def euclidean_distance(x1: np.ndarray, x2: np.ndarray) -> np.floating:
     """Get euclidean distance between two arrays.
 
     Parameters
     ----------
     x1:
         first array
     x2:
         second array
 
     Returns
     -------
-    float:
+    :
         distance between x1 and x2
     """
     return np.linalg.norm(x1 - x2)
 
 
 class EuclideanDistance(Distance):
     """Euclidean distance handler."""
```

### Comparing `etna-1.9.0/etna/clustering/hierarchical/base.py` & `etna-2.0.0/etna/clustering/hierarchical/base.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/clustering/hierarchical/dtw_clustering.py` & `etna-2.0.0/etna/clustering/hierarchical/dtw_clustering.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/clustering/hierarchical/euclidean_clustering.py` & `etna-2.0.0/etna/clustering/hierarchical/euclidean_clustering.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/commands/backtest_command.py` & `etna-2.0.0/etna/commands/backtest_command.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 from pathlib import Path
 from typing import Any
 from typing import Dict
+from typing import List
 from typing import Optional
+from typing import Sequence
+from typing import Union
 
 import hydra_slayer
 import pandas as pd
 import typer
 from omegaconf import OmegaConf
+from typing_extensions import Literal
 
 from etna.datasets import TSDataset
 from etna.pipeline import Pipeline
 
 
 def backtest(
     config_path: Path = typer.Argument(..., help="path to yaml config with desired pipeline"),
     backtest_config_path: Path = typer.Argument(..., help="path to backtest config file"),
     target_path: Path = typer.Argument(..., help="path to csv with data to forecast"),
     freq: str = typer.Argument(..., help="frequency of timestamp in files in pandas format"),
     output_path: Path = typer.Argument(..., help="where to save forecast"),
     exog_path: Optional[Path] = typer.Argument(default=None, help="path to csv with exog data"),
+    known_future: Optional[List[str]] = typer.Argument(
+        None,
+        help="list of all known_future columns (regressor "
+        "columns). If not specified then all exog_columns "
+        "considered known_future.",
+    ),
 ):
     """Command to run backtest with etna without coding.
 
     Expected format of csv with target timeseries:
 
     \b
     =============  ===========  ==========
@@ -56,19 +66,21 @@
     backtest_configs = OmegaConf.to_object(OmegaConf.load(backtest_config_path))
 
     df_timeseries = pd.read_csv(target_path, parse_dates=["timestamp"])
 
     df_timeseries = TSDataset.to_dataset(df_timeseries)
 
     df_exog = None
+    k_f: Union[Literal["all"], Sequence[Any]] = ()
     if exog_path:
         df_exog = pd.read_csv(exog_path, parse_dates=["timestamp"])
         df_exog = TSDataset.to_dataset(df_exog)
+        k_f = "all" if not known_future else known_future
 
-    tsdataset = TSDataset(df=df_timeseries, freq=freq, df_exog=df_exog)
+    tsdataset = TSDataset(df=df_timeseries, freq=freq, df_exog=df_exog, known_future=k_f)
 
     pipeline: Pipeline = hydra_slayer.get_from_params(**pipeline_configs)
     backtest_configs_hydra_slayer: Dict[str, Any] = hydra_slayer.get_from_params(**backtest_configs)
 
     metrics, forecast, info = pipeline.backtest(ts=tsdataset, **backtest_configs_hydra_slayer)
 
     (metrics.to_csv(output_path / "metrics.csv", index=False))
```

### Comparing `etna-1.9.0/etna/commands/forecast_command.py` & `etna-2.0.0/etna/commands/forecast_command.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 from pathlib import Path
 from typing import Any
 from typing import Dict
+from typing import List
 from typing import Optional
+from typing import Sequence
+from typing import Union
 
 import hydra_slayer
 import pandas as pd
 import typer
 from omegaconf import OmegaConf
+from typing_extensions import Literal
 
 from etna.datasets import TSDataset
 from etna.pipeline import Pipeline
 
 
 def forecast(
     config_path: Path = typer.Argument(..., help="path to yaml config with desired pipeline"),
     target_path: Path = typer.Argument(..., help="path to csv with data to forecast"),
     freq: str = typer.Argument(..., help="frequency of timestamp in files in pandas format"),
     output_path: Path = typer.Argument(..., help="where to save forecast"),
     exog_path: Optional[Path] = typer.Argument(None, help="path to csv with exog data"),
     forecast_config_path: Optional[Path] = typer.Argument(None, help="path to yaml config with forecast params"),
     raw_output: bool = typer.Argument(False, help="by default we return only forecast without features"),
+    known_future: Optional[List[str]] = typer.Argument(
+        None,
+        help="list of all known_future columns (regressor "
+        "columns). If not specified then all exog_columns "
+        "considered known_future.",
+    ),
 ):
     """Command to make forecast with etna without coding.
 
     Expected format of csv with target timeseries:
 
     \b
     =============  ===========  ==========
@@ -61,19 +71,21 @@
     forecast_params: Dict[str, Any] = hydra_slayer.get_from_params(**forecast_params_config)
 
     df_timeseries = pd.read_csv(target_path, parse_dates=["timestamp"])
 
     df_timeseries = TSDataset.to_dataset(df_timeseries)
 
     df_exog = None
+    k_f: Union[Literal["all"], Sequence[Any]] = ()
     if exog_path:
         df_exog = pd.read_csv(exog_path, parse_dates=["timestamp"])
         df_exog = TSDataset.to_dataset(df_exog)
+        k_f = "all" if not known_future else known_future
 
-    tsdataset = TSDataset(df=df_timeseries, freq=freq, df_exog=df_exog)
+    tsdataset = TSDataset(df=df_timeseries, freq=freq, df_exog=df_exog, known_future=k_f)
 
     pipeline: Pipeline = hydra_slayer.get_from_params(**pipeline_configs)
     pipeline.fit(tsdataset)
     forecast = pipeline.forecast(**forecast_params)
 
     flatten = forecast.to_pandas(flatten=True)
     if raw_output:
```

### Comparing `etna-1.9.0/etna/datasets/tsdataset.py` & `etna-2.0.0/etna/datasets/tsdataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 import math
 import warnings
 from copy import copy
+from copy import deepcopy
 from typing import TYPE_CHECKING
 from typing import Any
+from typing import Callable
 from typing import Dict
+from typing import Iterable
+from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Sequence
-from typing import Set
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 from typing_extensions import Literal
 
+from etna import SETTINGS
+from etna.datasets.hierarchical_structure import HierarchicalStructure
+from etna.datasets.utils import _TorchDataset
+from etna.datasets.utils import get_level_dataframe
+from etna.datasets.utils import inverse_transform_target_components
+from etna.datasets.utils import match_target_quantiles
 from etna.loggers import tslogger
 
 if TYPE_CHECKING:
     from etna.transforms.base import Transform
 
+if SETTINGS.torch_required:
+    from torch.utils.data import Dataset
+
 TTimestamp = Union[str, pd.Timestamp]
 
 
 class TSDataset:
     """TSDataset is the main class to handle your time series data.
     It prepares the series for exploration analyzing, implements feature generation with Transforms
     and generation of future points.
@@ -69,38 +81,56 @@
     feature    regressor_0 regressor_1 regressor_2 regressor_3 regressor_4 target
     timestamp
     2021-01-01        1.62       -0.02       -0.50       -0.56        0.52   1.62
     2021-01-02        1.01       -0.80       -0.81        0.38       -0.60   1.01
     2021-01-03        0.48        0.47       -0.81       -1.56       -1.37   0.48
     2021-01-04       -0.59        2.44       -2.21       -1.21       -0.69  -0.59
     2021-01-05        0.28        0.58       -3.07       -1.45        0.77   0.28
+
+    >>> from etna.datasets import generate_hierarchical_df
+    >>> pd.options.display.width = 0
+    >>> df = generate_hierarchical_df(periods=100, n_segments=[2, 4], start_time="2021-01-01",)
+    >>> df, hierarchical_structure = TSDataset.to_hierarchical_dataset(df=df, level_columns=["level_0", "level_1"])
+    >>> tsdataset = TSDataset(df=df, freq="D", hierarchical_structure=hierarchical_structure)
+    >>> tsdataset.df.head(5)
+    segment    l0s0_l1s3 l0s1_l1s0 l0s1_l1s1 l0s1_l1s2
+    feature       target    target    target    target
+    timestamp
+    2021-01-01      2.07      1.62     -0.45     -0.40
+    2021-01-02      0.59      1.01      0.78      0.42
+    2021-01-03     -0.24      0.48      1.18     -0.14
+    2021-01-04     -1.12     -0.59      1.77      1.82
+    2021-01-05     -1.40      0.28      0.68      0.48
     """
 
     idx = pd.IndexSlice
 
     def __init__(
         self,
         df: pd.DataFrame,
         freq: str,
         df_exog: Optional[pd.DataFrame] = None,
         known_future: Union[Literal["all"], Sequence] = (),
+        hierarchical_structure: Optional[HierarchicalStructure] = None,
     ):
         """Init TSDataset.
 
         Parameters
         ----------
         df:
             dataframe with timeseries
         freq:
             frequency of timestamp in df
         df_exog:
             dataframe with exogenous data;
         known_future:
             columns in ``df_exog[known_future]`` that are regressors,
             if "all" value is given, all columns are meant to be regressors
+        hierarchical_structure:
+            Structure of the levels in the hierarchy. If None, there is no hierarchical structure in the dataset.
         """
         self.raw_df = self._prepare_df(df)
         self.raw_df.index = pd.to_datetime(self.raw_df.index)
         self.freq = freq
         self.df_exog = None
 
         self.raw_df.index = pd.to_datetime(self.raw_df.index)
@@ -119,106 +149,69 @@
         self.raw_df = self.raw_df.asfreq(self.freq)
 
         self.df = self.raw_df.copy(deep=True)
 
         self.known_future = self._check_known_future(known_future, df_exog)
         self._regressors = copy(self.known_future)
 
+        self.hierarchical_structure = hierarchical_structure
+        self.current_df_level: Optional[str] = self._get_dataframe_level(df=self.df)
+        self.current_df_exog_level: Optional[str] = None
+
         if df_exog is not None:
             self.df_exog = df_exog.copy(deep=True)
             self.df_exog.index = pd.to_datetime(self.df_exog.index)
-            self.df = self._merge_exog(self.df)
+            self.current_df_exog_level = self._get_dataframe_level(df=self.df_exog)
+            if self.current_df_level == self.current_df_exog_level:
+                self.df = self._merge_exog(self.df)
+
+        self._target_components_names: Tuple[str, ...] = tuple()
+
+        self.df = self.df.sort_index(axis=1, level=("segment", "feature"))
+
+    def _get_dataframe_level(self, df: pd.DataFrame) -> Optional[str]:
+        """Return the level of the passed dataframe in hierarchical structure."""
+        if self.hierarchical_structure is None:
+            return None
+
+        df_segments = df.columns.get_level_values("segment").unique()
+        segment_levels = {self.hierarchical_structure.get_segment_level(segment=segment) for segment in df_segments}
+        if len(segment_levels) != 1:
+            raise ValueError("Segments in dataframe are from more than 1 hierarchical levels!")
+
+        df_level = segment_levels.pop()
+        level_segments = self.hierarchical_structure.get_level_segments(level_name=df_level)
+        if len(df_segments) != len(level_segments):
+            raise ValueError("Some segments of hierarchical level are missing in dataframe!")
 
-        self.transforms: Optional[Sequence["Transform"]] = None
+        return df_level
 
     def transform(self, transforms: Sequence["Transform"]):
         """Apply given transform to the data."""
         self._check_endings(warning=True)
-        self.transforms = transforms
-        for transform in self.transforms:
+        for transform in transforms:
             tslogger.log(f"Transform {repr(transform)} is applied to dataset")
-            columns_before = set(self.columns.get_level_values("feature"))
-            self.df = transform.transform(self.df)
-            columns_after = set(self.columns.get_level_values("feature"))
-            self._update_regressors(transform=transform, columns_before=columns_before, columns_after=columns_after)
+            transform.transform(self)
 
     def fit_transform(self, transforms: Sequence["Transform"]):
         """Fit and apply given transforms to the data."""
         self._check_endings(warning=True)
-        self.transforms = transforms
-        for transform in self.transforms:
+        for transform in transforms:
             tslogger.log(f"Transform {repr(transform)} is applied to dataset")
-            columns_before = set(self.columns.get_level_values("feature"))
-            self.df = transform.fit_transform(self.df)
-            columns_after = set(self.columns.get_level_values("feature"))
-            self._update_regressors(transform=transform, columns_before=columns_before, columns_after=columns_after)
+            transform.fit_transform(self)
 
     @staticmethod
     def _prepare_df(df: pd.DataFrame) -> pd.DataFrame:
         # cast segment to str type
         df_copy = df.copy(deep=True)
         columns_frame = df.columns.to_frame()
         columns_frame["segment"] = columns_frame["segment"].astype(str)
         df_copy.columns = pd.MultiIndex.from_frame(columns_frame)
         return df_copy
 
-    def _update_regressors(self, transform: "Transform", columns_before: Set[str], columns_after: Set[str]):
-        from etna.transforms import OneHotEncoderTransform
-        from etna.transforms.base import FutureMixin
-
-        # intersect list of regressors with columns after the transform
-        self._regressors = list(set(self._regressors).intersection(columns_after))
-
-        unseen_columns = list(columns_after - columns_before)
-
-        if len(unseen_columns) == 0:
-            return
-
-        new_regressors = []
-
-        if isinstance(transform, FutureMixin):
-            # Every column from FutureMixin is regressor
-            out_columns = list(columns_after - columns_before)
-            new_regressors = out_columns
-        elif isinstance(transform, OneHotEncoderTransform):
-            # Only the columns created with OneHotEncoderTransform from regressor are regressors
-            in_column = transform.in_column
-            out_columns = list(columns_after - columns_before)
-            if in_column in self.regressors:
-                new_regressors = out_columns
-        elif hasattr(transform, "in_column"):
-            # Only the columns created with the other transforms from regressors are regressors
-            in_columns = transform.in_column if isinstance(transform.in_column, list) else [transform.in_column]  # type: ignore
-            if hasattr(transform, "out_columns") and transform.out_columns is not None:  # type: ignore
-                # User defined out_columns in sklearn
-                # TODO: remove this case after fixing the out_column attribute in SklearnTransform
-                out_columns = transform.out_columns  # type: ignore
-                regressors_in_column_ids = [i for i, in_column in enumerate(in_columns) if in_column in self.regressors]
-                new_regressors = [out_columns[i] for i in regressors_in_column_ids]
-            elif hasattr(transform, "out_column") and transform.out_column is not None:  # type: ignore
-                # User defined out_columns
-                out_columns = transform.out_column if isinstance(transform.out_column, list) else [transform.out_column]  # type: ignore
-                regressors_in_column_ids = [i for i, in_column in enumerate(in_columns) if in_column in self.regressors]
-                new_regressors = [out_columns[i] for i in regressors_in_column_ids]
-            else:
-                # Default out_columns
-                out_columns = list(columns_after - columns_before)
-                regressors_in_column = [in_column for in_column in in_columns if in_column in self.regressors]
-                new_regressors = [
-                    out_column
-                    for out_column in out_columns
-                    if np.any([regressor in out_column for regressor in regressors_in_column])
-                ]
-
-        else:
-            raise ValueError("Transform is not FutureMixin and does not have in_column attribute!")
-
-        new_regressors = [regressor for regressor in new_regressors if regressor not in self.regressors]
-        self._regressors.extend(new_regressors)
-
     def __repr__(self):
         return self.df.__repr__()
 
     def _repr_html_(self):
         return self.df._repr_html_()
 
     def __getitem__(self, item):
@@ -230,21 +223,27 @@
             df = self.df.loc[self.idx[item[0]]]
         else:
             df = self.df.loc[self.idx[item[0]], self.idx[item[1], item[2]]]
         first_valid_idx = df.first_valid_index()
         df = df.loc[first_valid_idx:]
         return df
 
-    def make_future(self, future_steps: int) -> "TSDataset":
+    def make_future(
+        self, future_steps: int, transforms: Sequence["Transform"] = (), tail_steps: int = 0
+    ) -> "TSDataset":
         """Return new TSDataset with future steps.
 
         Parameters
         ----------
         future_steps:
             number of timestamp in the future to build features for.
+        transforms:
+            sequence of transforms to be applied.
+        tail_steps:
+            number of timestamp for context to build features for.
 
         Returns
         -------
         :
             dataset with features in the future.
 
         Examples
@@ -279,67 +278,93 @@
             start=max_date_in_dataset, periods=future_steps + 1, freq=self.freq, closed="right"
         )
 
         new_index = self.raw_df.index.append(future_dates)
         df = self.raw_df.reindex(new_index)
         df.index.name = "timestamp"
 
-        if self.df_exog is not None:
+        if self.df_exog is not None and self.current_df_level == self.current_df_exog_level:
             df = self._merge_exog(df)
 
             # check if we have enough values in regressors
             if self.regressors:
                 for segment in self.segments:
                     regressors_index = self.df_exog.loc[:, pd.IndexSlice[segment, self.regressors]].index
                     if not np.all(future_dates.isin(regressors_index)):
                         warnings.warn(
                             f"Some regressors don't have enough values in segment {segment}, "
                             f"NaN-s will be used for missing values"
                         )
 
-        if self.transforms is not None:
-            for transform in self.transforms:
-                tslogger.log(f"Transform {repr(transform)} is applied to dataset")
-                df = transform.transform(df)
+        # Here only df is required, other metadata is not necessary to build the dataset
+        ts = TSDataset(df=df, freq=self.freq)
+        for transform in transforms:
+            tslogger.log(f"Transform {repr(transform)} is applied to dataset")
+            transform.transform(ts)
+        df = ts.to_pandas()
+
+        future_dataset = df.tail(future_steps + tail_steps).copy(deep=True)
 
-        future_dataset = df.tail(future_steps).copy(deep=True)
         future_dataset = future_dataset.sort_index(axis=1, level=(0, 1))
         future_ts = TSDataset(df=future_dataset, freq=self.freq)
 
         # can't put known_future into constructor, _check_known_future fails with df_exog=None
-        future_ts.known_future = self.known_future
-        future_ts._regressors = self.regressors
-        future_ts.transforms = self.transforms
+        future_ts.known_future = deepcopy(self.known_future)
+        future_ts._regressors = deepcopy(self.regressors)
         future_ts.df_exog = self.df_exog
         return future_ts
 
+    def tsdataset_idx_slice(self, start_idx: Optional[int] = None, end_idx: Optional[int] = None) -> "TSDataset":
+        """Return new TSDataset with integer-location based indexing.
+
+        Parameters
+        ----------
+        start_idx:
+            starting index of the slice.
+        end_idx:
+            last index of the slice.
+
+        Returns
+        -------
+        :
+            TSDataset based on indexing slice.
+        """
+        df_slice = self.df.iloc[start_idx:end_idx].copy(deep=True)
+        tsdataset_slice = TSDataset(df=df_slice, freq=self.freq)
+        # can't put known_future into constructor, _check_known_future fails with df_exog=None
+        tsdataset_slice.known_future = deepcopy(self.known_future)
+        tsdataset_slice._regressors = deepcopy(self.regressors)
+        tsdataset_slice.df_exog = self.df_exog
+        tsdataset_slice._target_components_names = self._target_components_names
+        return tsdataset_slice
+
     @staticmethod
     def _check_known_future(
         known_future: Union[Literal["all"], Sequence], df_exog: Optional[pd.DataFrame]
     ) -> List[str]:
         """Check that ``known_future`` corresponds to ``df_exog`` and returns initial list of regressors."""
         if df_exog is None:
             exog_columns = set()
         else:
             exog_columns = set(df_exog.columns.get_level_values("feature"))
 
         if isinstance(known_future, str):
             if known_future == "all":
-                return sorted(list(exog_columns))
+                return sorted(exog_columns)
             else:
                 raise ValueError("The only possible literal is 'all'")
         else:
             known_future_unique = set(known_future)
             if not known_future_unique.issubset(exog_columns):
                 raise ValueError(
                     f"Some features in known_future are not present in df_exog: "
                     f"{known_future_unique.difference(exog_columns)}"
                 )
             else:
-                return sorted(list(known_future_unique))
+                return sorted(known_future_unique)
 
     @staticmethod
     def _check_regressors(df: pd.DataFrame, df_regressors: pd.DataFrame):
         """Check that regressors begin not later than in ``df`` and end later than in ``df``."""
         if df_regressors.shape[1] == 0:
             return
         # TODO: check performance
@@ -366,16 +391,15 @@
                     f"Series of segment {segment} have not enough history: "
                     f"{target_max} >= {exog_series_max}."
                 )
 
     def _merge_exog(self, df: pd.DataFrame) -> pd.DataFrame:
         if self.df_exog is None:
             raise ValueError("Something went wrong, Trying to merge df_exog which is None!")
-        segments = sorted(set(df.columns.get_level_values("segment")))
-        df_regressors = self.df_exog.loc[:, pd.IndexSlice[segments, self.known_future]]
+        df_regressors = self.df_exog.loc[:, pd.IndexSlice[:, self.known_future]]
         self._check_regressors(df=df, df_regressors=df_regressors)
         df = pd.concat((df, self.df_exog), axis=1).loc[df.index].sort_index(axis=1, level=(0, 1))
         return df
 
     def _check_endings(self, warning=False):
         """Check that all targets ends at the same timestamp."""
         max_index = self.df.index.max()
@@ -385,23 +409,48 @@
                     "Segments contains NaNs in the last timestamps."
                     "Some of the transforms might work incorrectly or even fail."
                     "Make sure that you use the imputer before making the forecast."
                 )
             else:
                 raise ValueError("All segments should end at the same timestamp")
 
-    def inverse_transform(self):
+    def _inverse_transform_target_components(self, target_components_df: pd.DataFrame, target_df: pd.DataFrame):
+        """Inverse transform target components in dataset with inverse transformed target."""
+        self.drop_target_components()
+        inverse_transformed_target_components_df = inverse_transform_target_components(
+            target_components_df=target_components_df,
+            target_df=target_df,
+            inverse_transformed_target_df=self.to_pandas(features=["target"]),
+        )
+        self.add_target_components(target_components_df=inverse_transformed_target_components_df)
+
+    def inverse_transform(self, transforms: Sequence["Transform"]):
         """Apply inverse transform method of transforms to the data.
 
         Applied in reversed order.
         """
-        if self.transforms is not None:
-            for transform in reversed(self.transforms):
+        # TODO: return regressors after inverse_transform
+        # Logic with target components is here for performance reasons.
+        # This way we avoid doing the inverse transformation for components several times.
+        target_components_present = len(self.target_components_names) > 0
+        target_df, target_components_df = None, None
+        if target_components_present:
+            target_df = self.to_pandas(features=["target"])
+            target_components_df = self.get_target_components()
+            self.drop_target_components()
+
+        try:
+            for transform in reversed(transforms):
                 tslogger.log(f"Inverse transform {repr(transform)} is applied to dataset")
-                self.df = transform.inverse_transform(self.df)
+                transform.inverse_transform(self)
+        finally:
+            if target_components_present:
+                self._inverse_transform_target_components(
+                    target_components_df=target_components_df, target_df=target_df
+                )
 
     @property
     def segments(self) -> List[str]:
         """Get list of all segments in dataset.
 
         Examples
         --------
@@ -442,14 +491,24 @@
         ...     df_ts_format, df_exog=df_exog_ts_format, freq="D", known_future="all"
         ... )
         >>> ts.regressors
         ['regressor_1']
         """
         return self._regressors
 
+    @property
+    def target_components_names(self) -> Tuple[str, ...]:
+        """Get tuple with target components names. Components sum up to target. Return the empty tuple in case of components absence."""
+        return self._target_components_names
+
+    @property
+    def target_quantiles_names(self) -> Tuple[str, ...]:
+        """Get tuple with target quantiles names. Return the empty tuple in case of quantile absence."""
+        return tuple(match_target_quantiles(features=set(self.columns.get_level_values("feature"))))
+
     def plot(
         self,
         n_segments: int = 10,
         column: str = "target",
         segments: Optional[Sequence[str]] = None,
         start: Optional[str] = None,
         end: Optional[str] = None,
@@ -489,26 +548,31 @@
         _, ax = plt.subplots(rows_num, columns_num, figsize=figsize, squeeze=False)
         ax = ax.ravel()
         rnd_state = np.random.RandomState(seed)
         for i, segment in enumerate(sorted(rnd_state.choice(segments, size=k, replace=False))):
             df_slice = self[start:end, segment, column]  # type: ignore
             ax[i].plot(df_slice.index, df_slice.values)
             ax[i].set_title(segment)
-
-        plt.show()
+            ax[i].grid()
 
     @staticmethod
-    def to_flatten(df: pd.DataFrame) -> pd.DataFrame:
+    def to_flatten(df: pd.DataFrame, features: Union[Literal["all"], Sequence[str]] = "all") -> pd.DataFrame:
         """Return pandas DataFrame with flatten index.
 
+        The order of columns is (timestamp, segment, target,
+        features in alphabetical order).
+
         Parameters
         ----------
         df:
             DataFrame in ETNA format.
-
+        features:
+            List of features to return.
+            If "all", return all the features in the dataset.
+            Always return columns with timestamp and segemnt.
         Returns
         -------
         pd.DataFrame:
             dataframe with TSDataset data
 
         Examples
         --------
@@ -522,48 +586,65 @@
         0  2021-06-01  segment_0    1.00
         1  2021-06-02  segment_0    1.00
         2  2021-06-03  segment_0    1.00
         3  2021-06-04  segment_0    1.00
         4  2021-06-05  segment_0    1.00
         >>> df_ts_format = TSDataset.to_dataset(df)
         >>> TSDataset.to_flatten(df_ts_format).head(5)
-           timestamp  target    segment
-        0 2021-06-01     1.0  segment_0
-        1 2021-06-02     1.0  segment_0
-        2 2021-06-03     1.0  segment_0
-        3 2021-06-04     1.0  segment_0
-        4 2021-06-05     1.0  segment_0
+           timestamp    segment  target
+        0 2021-06-01  segment_0    1.0
+        1 2021-06-02  segment_0    1.0
+        2 2021-06-03  segment_0    1.0
+        3 2021-06-04  segment_0    1.0
+        4 2021-06-05  segment_0    1.0
         """
-        # flatten dataframe
-        aggregator_list = []
-        segments = df.columns.get_level_values("segment").unique().tolist()
-        for segment in segments:
-            aggregator_list.append(df[segment].copy())
-            aggregator_list[-1]["segment"] = segment
-        df_flat = pd.concat(aggregator_list)
-        df_flat = df_flat.reset_index()
-        df_flat.columns.name = None
-
-        # mark category as category
+        segments = df.columns.get_level_values("segment").unique()
         dtypes = df.dtypes
         category_columns = dtypes[dtypes == "category"].index.get_level_values(1).unique()
-        df_flat[category_columns] = df_flat[category_columns].astype("category")
+        if isinstance(features, str):
+            if features != "all":
+                raise ValueError("The only possible literal is 'all'")
+        else:
+            df = df.loc[:, pd.IndexSlice[segments, features]].copy()
+        columns = df.columns.get_level_values("feature").unique()
+
+        # flatten dataframe
+        df_dict: Dict[str, Any] = {}
+        df_dict["timestamp"] = np.tile(df.index, len(segments))
+        df_dict["segment"] = np.repeat(segments, len(df.index))
+        if "target" in columns:
+            # set this value to lock position of key "target" in output dataframe columns
+            # None is a placeholder, actual column value will be assigned in the following cycle
+            df_dict["target"] = None
+        for column in columns:
+            df_cur = df.loc[:, pd.IndexSlice[:, column]]
+            if column in category_columns:
+                df_dict[column] = pd.api.types.union_categoricals([df_cur[col] for col in df_cur.columns])
+            else:
+                stacked = df_cur.values.T.ravel()
+                # creating series is necessary for dtypes like "Int64", "boolean", otherwise they will be objects
+                df_dict[column] = pd.Series(stacked, dtype=df_cur.dtypes[0])
+        df_flat = pd.DataFrame(df_dict)
 
         return df_flat
 
-    def to_pandas(self, flatten: bool = False) -> pd.DataFrame:
+    def to_pandas(self, flatten: bool = False, features: Union[Literal["all"], Sequence[str]] = "all") -> pd.DataFrame:
         """Return pandas DataFrame.
 
         Parameters
         ----------
         flatten:
             * If False, return pd.DataFrame with multiindex
 
-            * If True, return with flatten index
-
+            * If True, return with flatten index,
+            its order of columns is (timestamp, segment, target,
+            features in alphabetical order).
+        features:
+            List of features to return.
+            If "all", return all the features in the dataset.
         Returns
         -------
         pd.DataFrame
             dataframe with TSDataset data
 
         Examples
         --------
@@ -578,33 +659,38 @@
         1  2021-06-02  segment_0    1.00
         2  2021-06-03  segment_0    1.00
         3  2021-06-04  segment_0    1.00
         4  2021-06-05  segment_0    1.00
         >>> df_ts_format = TSDataset.to_dataset(df)
         >>> ts = TSDataset(df_ts_format, "D")
         >>> ts.to_pandas(True).head(5)
-           timestamp  target    segment
-        0 2021-06-01     1.0  segment_0
-        1 2021-06-02     1.0  segment_0
-        2 2021-06-03     1.0  segment_0
-        3 2021-06-04     1.0  segment_0
-        4 2021-06-05     1.0  segment_0
+            timestamp    segment  target
+        0  2021-06-01  segment_0    1.00
+        1  2021-06-02  segment_0    1.00
+        2  2021-06-03  segment_0    1.00
+        3  2021-06-04  segment_0    1.00
+        4  2021-06-05  segment_0    1.00
         >>> ts.to_pandas(False).head(5)
         segment    segment_0 segment_1
         feature       target    target
         timestamp
         2021-06-01      1.00      1.00
         2021-06-02      1.00      1.00
         2021-06-03      1.00      1.00
         2021-06-04      1.00      1.00
         2021-06-05      1.00      1.00
         """
         if not flatten:
-            return self.df.copy()
-        return self.to_flatten(self.df)
+            if isinstance(features, str):
+                if features == "all":
+                    return self.df.copy()
+                raise ValueError("The only possible literal is 'all'")
+            segments = self.columns.get_level_values("segment").unique().tolist()
+            return self.df.loc[:, self.idx[segments, features]].copy()
+        return self.to_flatten(self.df, features=features)
 
     @staticmethod
     def to_dataset(df: pd.DataFrame) -> pd.DataFrame:
         """Convert pandas dataframe to ETNA Dataset format.
 
         Columns "timestamp" and "segment" are required.
 
@@ -653,24 +739,97 @@
         timestamp
         2021-01-01           0           5
         2021-01-02           1           6
         2021-01-03           2           7
         2021-01-04           3           8
         2021-01-05           4           9
         """
-        df["timestamp"] = pd.to_datetime(df["timestamp"])
-        df["segment"] = df["segment"].astype(str)
-        feature_columns = df.columns.tolist()
+        df_copy = df.copy(deep=True)
+        df_copy["timestamp"] = pd.to_datetime(df_copy["timestamp"])
+        df_copy["segment"] = df_copy["segment"].astype(str)
+        feature_columns = df_copy.columns.tolist()
         feature_columns.remove("timestamp")
         feature_columns.remove("segment")
-        df = df.pivot(index="timestamp", columns="segment")
-        df = df.reorder_levels([1, 0], axis=1)
-        df.columns.names = ["segment", "feature"]
-        df = df.sort_index(axis=1, level=(0, 1))
-        return df
+        df_copy = df_copy.pivot(index="timestamp", columns="segment")
+        df_copy = df_copy.reorder_levels([1, 0], axis=1)
+        df_copy.columns.names = ["segment", "feature"]
+        df_copy = df_copy.sort_index(axis=1, level=(0, 1))
+        return df_copy
+
+    @staticmethod
+    def _hierarchical_structure_from_level_columns(
+        df: pd.DataFrame, level_columns: List[str], sep: str
+    ) -> HierarchicalStructure:
+        """Create hierarchical structure from dataframe columns."""
+        df_level_columns = df[level_columns].astype("string")
+
+        prev_level_name = level_columns[0]
+        for cur_level_name in level_columns[1:]:
+            df_level_columns[cur_level_name] = (
+                df_level_columns[prev_level_name] + sep + df_level_columns[cur_level_name]
+            )
+            prev_level_name = cur_level_name
+
+        level_structure = {"total": list(df_level_columns[level_columns[0]].unique())}
+        cur_level_name = level_columns[0]
+        for next_level_name in level_columns[1:]:
+            cur_level_to_next_level_edges = df_level_columns[[cur_level_name, next_level_name]].drop_duplicates()
+            cur_level_to_next_level_adjacency_list = cur_level_to_next_level_edges.groupby(cur_level_name).agg(list)
+            level_structure.update(cur_level_to_next_level_adjacency_list.to_records())
+            cur_level_name = next_level_name
+
+        hierarchical_structure = HierarchicalStructure(
+            level_structure=level_structure, level_names=["total"] + level_columns
+        )
+        return hierarchical_structure
+
+    @staticmethod
+    def to_hierarchical_dataset(
+        df: pd.DataFrame,
+        level_columns: List[str],
+        keep_level_columns: bool = False,
+        sep: str = "_",
+        return_hierarchy: bool = True,
+    ) -> Tuple[pd.DataFrame, Optional[HierarchicalStructure]]:
+        """Convert pandas dataframe from long hierarchical to ETNA Dataset format.
+
+        Parameters
+        ----------
+        df:
+            Dataframe in long hierarchical format with columns [timestamp, target] + [level_columns] + [other_columns]
+        level_columns:
+            Columns of dataframe defines the levels in the hierarchy in order
+            from top to bottom i.e [level_name_1, level_name_2, ...]. Names of the columns will be used as
+            names of the levels in hierarchy.
+        keep_level_columns:
+            If true, leave the level columns in the result dataframe.
+            By default level columns are concatenated into "segment" column and dropped
+        sep:
+            String to concatenated the level names with
+        return_hierarchy:
+            If true, returns the hierarchical structure
+
+        Returns
+        -------
+        :
+            Dataframe in wide format and optionally hierarchical structure
+        """
+        df_copy = df.copy(deep=True)
+        df_copy["segment"] = df_copy[level_columns].astype("string").agg(sep.join, axis=1)
+        if not keep_level_columns:
+            df_copy.drop(columns=level_columns, inplace=True)
+        df_copy = TSDataset.to_dataset(df_copy)
+
+        hierarchical_structure = None
+        if return_hierarchy:
+            hierarchical_structure = TSDataset._hierarchical_structure_from_level_columns(
+                df=df, level_columns=level_columns, sep=sep
+            )
+
+        return df_copy, hierarchical_structure
 
     def _find_all_borders(
         self,
         train_start: Optional[TTimestamp],
         train_end: Optional[TTimestamp],
         test_start: Optional[TTimestamp],
         test_end: Optional[TTimestamp],
@@ -804,37 +963,254 @@
         if pd.Timestamp(test_end_defined) > self.df.index.max():
             warnings.warn(f"Max timestamp in df is {self.df.index.max()}.")
         if pd.Timestamp(train_start_defined) < self.df.index.min():
             warnings.warn(f"Min timestamp in df is {self.df.index.min()}.")
 
         train_df = self.df[train_start_defined:train_end_defined][self.raw_df.columns]  # type: ignore
         train_raw_df = self.raw_df[train_start_defined:train_end_defined]  # type: ignore
-        train = TSDataset(df=train_df, df_exog=self.df_exog, freq=self.freq, known_future=self.known_future)
+        train = TSDataset(
+            df=train_df,
+            df_exog=self.df_exog,
+            freq=self.freq,
+            known_future=self.known_future,
+            hierarchical_structure=self.hierarchical_structure,
+        )
         train.raw_df = train_raw_df
         train._regressors = self.regressors
+        train._target_components_names = self.target_components_names
 
         test_df = self.df[test_start_defined:test_end_defined][self.raw_df.columns]  # type: ignore
         test_raw_df = self.raw_df[train_start_defined:test_end_defined]  # type: ignore
-        test = TSDataset(df=test_df, df_exog=self.df_exog, freq=self.freq, known_future=self.known_future)
+        test = TSDataset(
+            df=test_df,
+            df_exog=self.df_exog,
+            freq=self.freq,
+            known_future=self.known_future,
+            hierarchical_structure=self.hierarchical_structure,
+        )
         test.raw_df = test_raw_df
         test._regressors = self.regressors
-
+        test._target_components_names = self.target_components_names
         return train, test
 
+    def update_columns_from_pandas(self, df_update: pd.DataFrame):
+        """Update the existing columns in the dataset with the new values from pandas dataframe.
+
+        Before updating columns in df, columns of df_update will be cropped by the last timestamp in df.
+        Columns in df_exog are not updated. If you wish to update the df_exog, create the new
+        instance of TSDataset.
+
+        Parameters
+        ----------
+        df_update:
+            Dataframe with new values in wide ETNA format.
+        """
+        columns_to_update = sorted(set(df_update.columns.get_level_values("feature")))
+        self.df.loc[:, self.idx[self.segments, columns_to_update]] = df_update.loc[
+            : self.df.index.max(), self.idx[self.segments, columns_to_update]
+        ]
+
+    def add_columns_from_pandas(
+        self, df_update: pd.DataFrame, update_exog: bool = False, regressors: Optional[List[str]] = None
+    ):
+        """Update the dataset with the new columns from pandas dataframe.
+
+        Before updating columns in df, columns of df_update will be cropped by the last timestamp in df.
+
+        Parameters
+        ----------
+        df_update:
+            Dataframe with the new columns in wide ETNA format.
+        update_exog:
+             If True, update columns also in df_exog.
+             If you wish to add new regressors in the dataset it is recommended to turn on this flag.
+        regressors:
+            List of regressors in the passed dataframe.
+        """
+        self.df = pd.concat((self.df, df_update[: self.df.index.max()]), axis=1).sort_index(axis=1)
+        if update_exog:
+            if self.df_exog is None:
+                self.df_exog = df_update
+            else:
+                self.df_exog = pd.concat((self.df_exog, df_update), axis=1).sort_index(axis=1)
+        if regressors is not None:
+            self._regressors = list(set(self._regressors) | set(regressors))
+
+    def drop_features(self, features: List[str], drop_from_exog: bool = False):
+        """Drop columns with features from the dataset.
+
+        Parameters
+        ----------
+        features:
+            List of features to drop.
+        drop_from_exog:
+            * If False, drop features only from df. Features will appear again in df after make_future.
+            * If True, drop features from df and df_exog. Features won't appear in df after make_future.
+
+        Raises
+        ------
+        ValueError:
+            If ``features`` list contains target components
+        """
+        features_contain_target_components = len(set(features).intersection(self.target_components_names)) > 0
+        if features_contain_target_components:
+            raise ValueError(
+                "Target components can't be dropped from the dataset using this method! Use `drop_target_components` method!"
+            )
+
+        dfs = [("df", self.df)]
+        if drop_from_exog:
+            dfs.append(("df_exog", self.df_exog))
+
+        for name, df in dfs:
+            columns_in_df = df.columns.get_level_values("feature")
+            columns_to_remove = list(set(columns_in_df) & set(features))
+            unknown_columns = set(features) - set(columns_to_remove)
+            if len(unknown_columns) > 0:
+                warnings.warn(f"Features {unknown_columns} are not present in {name}!")
+            if len(columns_to_remove) > 0:
+                df.drop(columns=columns_to_remove, level="feature", inplace=True)
+        self._regressors = list(set(self._regressors) - set(features))
+
     @property
     def index(self) -> pd.core.indexes.datetimes.DatetimeIndex:
         """Return TSDataset timestamp index.
 
         Returns
         -------
         pd.core.indexes.datetimes.DatetimeIndex
             timestamp index of TSDataset
         """
         return self.df.index
 
+    def level_names(self) -> Optional[List[str]]:
+        """Return names of the levels in the hierarchical structure."""
+        if self.hierarchical_structure is None:
+            return None
+        return self.hierarchical_structure.level_names
+
+    def has_hierarchy(self) -> bool:
+        """Check whether dataset has hierarchical structure."""
+        return self.hierarchical_structure is not None
+
+    def get_level_dataset(self, target_level: str) -> "TSDataset":
+        """Generate new TSDataset on target level.
+
+        Parameters
+        ----------
+        target_level:
+            target level name
+
+        Returns
+        -------
+        TSDataset
+            generated dataset
+        """
+        if self.hierarchical_structure is None or self.current_df_level is None:
+            raise ValueError("Method could be applied only to instances with a hierarchy!")
+
+        current_level_segments = self.hierarchical_structure.get_level_segments(level_name=self.current_df_level)
+        target_level_segments = self.hierarchical_structure.get_level_segments(level_name=target_level)
+
+        current_level_index = self.hierarchical_structure.get_level_depth(self.current_df_level)
+        target_level_index = self.hierarchical_structure.get_level_depth(target_level)
+
+        if target_level_index > current_level_index:
+            raise ValueError("Target level should be higher in the hierarchy than the current level of dataframe!")
+
+        target_names = self.target_quantiles_names + self.target_components_names + ("target",)
+
+        if target_level_index < current_level_index:
+            summing_matrix = self.hierarchical_structure.get_summing_matrix(
+                target_level=target_level, source_level=self.current_df_level
+            )
+
+            target_level_df = get_level_dataframe(
+                df=self.to_pandas(features=target_names),
+                mapping_matrix=summing_matrix,
+                source_level_segments=current_level_segments,
+                target_level_segments=target_level_segments,
+            )
+
+        else:
+            target_level_df = self.to_pandas(features=target_names)
+
+        target_components_df = target_level_df.loc[:, pd.IndexSlice[:, self.target_components_names]]
+        if len(self.target_components_names) > 0:  # for pandas >=1.1, <1.2
+            target_level_df = target_level_df.drop(columns=list(self.target_components_names), level="feature")
+
+        ts = TSDataset(
+            df=target_level_df,
+            freq=self.freq,
+            df_exog=self.df_exog,
+            known_future=self.known_future,
+            hierarchical_structure=self.hierarchical_structure,
+        )
+
+        if len(self.target_components_names) > 0:
+            ts.add_target_components(target_components_df=target_components_df)
+        return ts
+
+    def add_target_components(self, target_components_df: pd.DataFrame):
+        """Add target components into dataset.
+
+        Parameters
+        ----------
+        target_components_df:
+            Dataframe in etna wide format with target components
+
+        Raises
+        ------
+        ValueError:
+            If dataset already contains target components
+        ValueError:
+            If target components names differs between segments
+        ValueError:
+            If components don't sum up to target
+        """
+        if len(self.target_components_names) > 0:
+            raise ValueError("Dataset already contains target components!")
+
+        components_names = sorted(target_components_df[self.segments[0]].columns.get_level_values("feature"))
+        for segment in self.segments:
+            components_names_segment = sorted(target_components_df[segment].columns.get_level_values("feature"))
+            if components_names != components_names_segment:
+                raise ValueError(
+                    f"Set of target components differs between segments '{self.segments[0]}' and '{segment}'!"
+                )
+
+        components_sum = target_components_df.sum(axis=1, level="segment")
+        if not np.allclose(components_sum.values, self[..., "target"].values):
+            raise ValueError("Components don't sum up to target!")
+
+        self._target_components_names = tuple(components_names)
+        self.df = (
+            pd.concat((self.df, target_components_df), axis=1)
+            .loc[self.df.index]
+            .sort_index(axis=1, level=("segment", "feature"))
+        )
+
+    def get_target_components(self) -> Optional[pd.DataFrame]:
+        """Get DataFrame with target components.
+
+        Returns
+        -------
+        :
+            Dataframe with target components
+        """
+        if len(self.target_components_names) == 0:
+            return None
+        return self.to_pandas(features=self.target_components_names)
+
+    def drop_target_components(self):
+        """Drop target components from dataset."""
+        if len(self.target_components_names) > 0:  # for pandas >=1.1, <1.2
+            self.df.drop(columns=list(self.target_components_names), level="feature", inplace=True)
+            self._target_components_names = ()
+
     @property
     def columns(self) -> pd.core.indexes.multi.MultiIndex:
         """Return columns of ``self.df``.
 
         Returns
         -------
         pd.core.indexes.multi.MultiIndex
@@ -1118,7 +1494,33 @@
 
         with pd.option_context("display.width", None):
             lines += segment_df.to_string().split("\n")
 
         # print the results
         result_string = "\n".join(lines)
         print(result_string)
+
+    def to_torch_dataset(
+        self, make_samples: Callable[[pd.DataFrame], Union[Iterator[dict], Iterable[dict]]], dropna: bool = True
+    ) -> "Dataset":
+        """Convert the TSDataset to a :py:class:`torch.Dataset`.
+
+        Parameters
+        ----------
+        make_samples:
+            function that takes per segment DataFrame and returns iterabale of samples
+        dropna:
+            if ``True``, missing rows are dropped
+
+        Returns
+        -------
+        :
+            :py:class:`torch.Dataset` with with train or test samples to infer on
+        """
+        df = self.to_pandas(flatten=True)
+        if dropna:
+            df = df.dropna()  # TODO: Fix this
+
+        ts_segments = [df_segment for _, df_segment in df.groupby("segment")]
+        ts_samples = [samples for df_segment in ts_segments for samples in make_samples(df_segment)]
+
+        return _TorchDataset(ts_samples=ts_samples)
```

### Comparing `etna-1.9.0/etna/ensembles/stacking_ensemble.py` & `etna-2.0.0/etna/ensembles/stacking_ensemble.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import warnings
 from copy import deepcopy
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Sequence
 from typing import Set
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from joblib import Parallel
 from joblib import delayed
 from sklearn.base import RegressorMixin
 from sklearn.linear_model import LinearRegression
 from typing_extensions import Literal
 
 from etna.datasets import TSDataset
-from etna.ensembles import EnsembleMixin
+from etna.ensembles.mixins import EnsembleMixin
+from etna.ensembles.mixins import SaveEnsembleMixin
 from etna.loggers import tslogger
 from etna.metrics import MAE
 from etna.pipeline.base import BasePipeline
 
 
-class StackingEnsemble(BasePipeline, EnsembleMixin):
+class StackingEnsemble(EnsembleMixin, SaveEnsembleMixin, BasePipeline):
     """StackingEnsemble is a pipeline that forecast future using the metamodel to combine the forecasts of the base models.
 
     Examples
     --------
     >>> from etna.datasets import generate_ar_df
     >>> from etna.datasets import TSDataset
     >>> from etna.ensembles import VotingEnsemble
@@ -153,30 +155,27 @@
         # Get forecasts from base models on backtest to fit the final model on
         forecasts = Parallel(n_jobs=self.n_jobs, **self.joblib_params)(
             delayed(self._backtest_pipeline)(pipeline=pipeline, ts=deepcopy(ts)) for pipeline in self.pipelines
         )
 
         # Fit the final model
         self.filtered_features_for_final_model = self._filter_features_to_use(forecasts)
-        x, y = self._make_features(forecasts=forecasts, train=True)
+        x, y = self._make_features(ts=self.ts, forecasts=forecasts, train=True)
         self.final_model.fit(x, y)
 
         # Fit the base models
         self.pipelines = Parallel(n_jobs=self.n_jobs, **self.joblib_params)(
             delayed(self._fit_pipeline)(pipeline=pipeline, ts=deepcopy(ts)) for pipeline in self.pipelines
         )
         return self
 
     def _make_features(
-        self, forecasts: List[TSDataset], train: bool = False
+        self, ts: TSDataset, forecasts: List[TSDataset], train: bool = False
     ) -> Tuple[pd.DataFrame, Optional[pd.Series]]:
         """Prepare features for the ``final_model``."""
-        if self.ts is None:
-            raise ValueError("StackingEnsemble is not fitted! Fit the StackingEnsemble before calling forecast method.")
-
         # Stack targets from the forecasts
         targets = [
             forecast[:, :, "target"].rename({"target": f"regressor_target_{i}"}, axis=1)
             for i, forecast in enumerate(forecasts)
         ]
         targets = pd.concat(targets, axis=1)
 
@@ -194,47 +193,73 @@
             features = pd.concat(
                 [forecast[:, :, features_in_forecasts[i]] for i, forecast in enumerate(forecasts)], axis=1
             )
             features = features.loc[:, ~features.columns.duplicated()]
         features_df = pd.concat([features, targets], axis=1)
 
         # Flatten the features to fit the sklearn interface
-        x = pd.concat([features_df.loc[:, segment] for segment in self.ts.segments], axis=0)
+        x = pd.concat([features_df.loc[:, segment] for segment in ts.segments], axis=0)
         if train:
             y = pd.concat(
-                [
-                    self.ts[forecasts[0].index.min() : forecasts[0].index.max(), segment, "target"]
-                    for segment in self.ts.segments
-                ],
+                [ts[forecasts[0].index.min() : forecasts[0].index.max(), segment, "target"] for segment in ts.segments],
                 axis=0,
             )
             return x, y
         else:
             return x, None
 
-    def _forecast(self) -> TSDataset:
-        """Make predictions.
-
-        Compute the combination of pipelines' forecasts using ``final_model``
-        """
-        if self.ts is None:
-            raise ValueError("Something went wrong, ts is None!")
-
-        # Get forecast
-        forecasts = Parallel(n_jobs=self.n_jobs, **self.joblib_params)(
-            delayed(self._forecast_pipeline)(pipeline=pipeline) for pipeline in self.pipelines
-        )
-        x, _ = self._make_features(forecasts=forecasts, train=False)
-        y = self.final_model.predict(x).reshape(-1, self.horizon).T
+    def _process_forecasts(self, ts: TSDataset, forecasts: List[TSDataset]) -> TSDataset:
+        x, _ = self._make_features(ts=ts, forecasts=forecasts, train=False)
+        y = self.final_model.predict(x)
+        num_segments = len(forecasts[0].segments)
+        y = y.reshape(num_segments, -1).T
+        num_timestamps = y.shape[0]
 
         # Format the forecast into TSDataset
-        segment_col = [segment for segment in self.ts.segments for _ in range(self.horizon)]
+        segment_col = [segment for segment in ts.segments for _ in range(num_timestamps)]
         x.loc[:, "segment"] = segment_col
         x.loc[:, "timestamp"] = x.index.values
         df_exog = TSDataset.to_dataset(x)
 
         df = forecasts[0][:, :, "target"].copy()
         df.loc[pd.IndexSlice[:], pd.IndexSlice[:, "target"]] = np.NAN
 
-        forecast = TSDataset(df=df, freq=self.ts.freq, df_exog=df_exog)
-        forecast.loc[pd.IndexSlice[:], pd.IndexSlice[:, "target"]] = y
+        result = TSDataset(df=df, freq=ts.freq, df_exog=df_exog)
+        result.loc[pd.IndexSlice[:], pd.IndexSlice[:, "target"]] = y
+        return result
+
+    def _forecast(self, ts: TSDataset, return_components: bool) -> TSDataset:
+        """Make predictions.
+
+        Compute the combination of pipelines' forecasts using ``final_model``
+        """
+        if return_components:
+            raise NotImplementedError("Adding target components is not currently implemented!")
+
+        forecasts = Parallel(n_jobs=self.n_jobs, **self.joblib_params)(
+            delayed(self._forecast_pipeline)(pipeline=pipeline, ts=ts) for pipeline in self.pipelines
+        )
+        forecast = self._process_forecasts(ts=ts, forecasts=forecasts)
         return forecast
+
+    def _predict(
+        self,
+        ts: TSDataset,
+        start_timestamp: pd.Timestamp,
+        end_timestamp: pd.Timestamp,
+        prediction_interval: bool,
+        quantiles: Sequence[float],
+        return_components: bool,
+    ) -> TSDataset:
+        if prediction_interval:
+            raise NotImplementedError(f"Ensemble {self.__class__.__name__} doesn't support prediction intervals!")
+        if return_components:
+            raise NotImplementedError("Adding target components is not currently implemented!")
+
+        predictions = Parallel(n_jobs=self.n_jobs, **self.joblib_params)(
+            delayed(self._predict_pipeline)(
+                ts=ts, pipeline=pipeline, start_timestamp=start_timestamp, end_timestamp=end_timestamp
+            )
+            for pipeline in self.pipelines
+        )
+        prediction = self._process_forecasts(ts=ts, forecasts=predictions)
+        return prediction
```

### Comparing `etna-1.9.0/etna/ensembles/voting_ensemble.py` & `etna-2.0.0/etna/ensembles/voting_ensemble.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from copy import deepcopy
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Sequence
 from typing import Union
 
 import pandas as pd
 from joblib import Parallel
 from joblib import delayed
 from sklearn.ensemble import RandomForestRegressor
 from typing_extensions import Literal
 
 from etna.analysis.feature_relevance.relevance_table import TreeBasedRegressor
 from etna.datasets import TSDataset
-from etna.ensembles import EnsembleMixin
+from etna.ensembles.mixins import EnsembleMixin
+from etna.ensembles.mixins import SaveEnsembleMixin
 from etna.loggers import tslogger
 from etna.metrics import MAE
 from etna.pipeline.base import BasePipeline
 
 
-class VotingEnsemble(BasePipeline, EnsembleMixin):
+class VotingEnsemble(EnsembleMixin, SaveEnsembleMixin, BasePipeline):
     """VotingEnsemble is a pipeline that forecast future values with weighted averaging of it's pipelines forecasts.
 
     Examples
     --------
     >>> from etna.datasets import generate_ar_df
     >>> from etna.datasets import TSDataset
     >>> from etna.ensembles import VotingEnsemble
@@ -192,20 +194,43 @@
 
         forecast_df = sum(
             [forecast[:, :, "target"] * weight for forecast, weight in zip(forecasts, self.processed_weights)]
         )
         forecast_dataset = TSDataset(df=forecast_df, freq=forecasts[0].freq)
         return forecast_dataset
 
-    def _forecast(self) -> TSDataset:
+    def _forecast(self, ts: TSDataset, return_components: bool) -> TSDataset:
         """Make predictions.
 
         Compute weighted average of pipelines' forecasts
         """
-        if self.ts is None:
-            raise ValueError("Something went wrong, ts is None!")
+        if return_components:
+            raise NotImplementedError("Adding target components is not currently implemented!")
 
         forecasts = Parallel(n_jobs=self.n_jobs, backend="multiprocessing", verbose=11)(
-            delayed(self._forecast_pipeline)(pipeline=pipeline) for pipeline in self.pipelines
+            delayed(self._forecast_pipeline)(pipeline=pipeline, ts=ts) for pipeline in self.pipelines
         )
         forecast = self._vote(forecasts=forecasts)
         return forecast
+
+    def _predict(
+        self,
+        ts: TSDataset,
+        start_timestamp: pd.Timestamp,
+        end_timestamp: pd.Timestamp,
+        prediction_interval: bool,
+        quantiles: Sequence[float],
+        return_components: bool,
+    ) -> TSDataset:
+        if prediction_interval:
+            raise NotImplementedError(f"Ensemble {self.__class__.__name__} doesn't support prediction intervals!")
+        if return_components:
+            raise NotImplementedError("Adding target components is not currently implemented!")
+
+        predictions = Parallel(n_jobs=self.n_jobs, backend="multiprocessing", verbose=11)(
+            delayed(self._predict_pipeline)(
+                ts=ts, pipeline=pipeline, start_timestamp=start_timestamp, end_timestamp=end_timestamp
+            )
+            for pipeline in self.pipelines
+        )
+        predictions = self._vote(forecasts=predictions)
+        return predictions
```

### Comparing `etna-1.9.0/etna/libs/tsfresh/defaults.py` & `etna-2.0.0/etna/libs/tsfresh/defaults.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/libs/tsfresh/distribution.py` & `etna-2.0.0/etna/libs/tsfresh/distribution.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/libs/tsfresh/relevance.py` & `etna-2.0.0/etna/libs/tsfresh/relevance.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/libs/tsfresh/significance_tests.py` & `etna-2.0.0/etna/libs/tsfresh/significance_tests.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/loggers/__init__.py` & `etna-2.0.0/etna/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/loggers/base.py` & `etna-2.0.0/etna/loggers/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from abc import abstractmethod
 from contextlib import contextmanager
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Dict
 from typing import Union
 
-import numpy as np
 import pandas as pd
 
 from etna.core.mixins import BaseMixin
 
 if TYPE_CHECKING:
     from etna.datasets import TSDataset
 
@@ -183,53 +182,7 @@
     @contextmanager
     def disable(self):
         """Context manager for local logging disabling."""
         temp_loggers = self.loggers
         self.loggers = []
         yield
         self.loggers = temp_loggers
-
-
-def percentile(n: int):
-    """Percentile for pandas agg."""
-
-    def percentile_(x):
-        return np.nanpercentile(a=x.values, q=n)
-
-    percentile_.__name__ = "percentile_%s" % n
-    return percentile_
-
-
-def aggregate_metrics_df(metrics_df: pd.DataFrame) -> Dict[str, float]:
-    """Aggregate metrics in :py:meth:`log_backtest_metrics` method.
-
-    Parameters
-    ----------
-    metrics_df:
-        Dataframe produced with :py:meth:`etna.pipeline.Pipeline._get_backtest_metrics`
-    """
-    # case for aggregate_metrics=False
-    if "fold_number" in metrics_df.columns:
-        metrics_dict = (
-            metrics_df.groupby("segment")
-            .mean()
-            .reset_index()
-            .drop(["segment", "fold_number"], axis=1)
-            .apply(["median", "mean", "std", percentile(5), percentile(25), percentile(75), percentile(95)])
-            .to_dict()
-        )
-
-    # case for aggregate_metrics=True
-    else:
-        metrics_dict = (
-            metrics_df.drop(["segment"], axis=1)
-            .apply(["median", "mean", "std", percentile(5), percentile(25), percentile(75), percentile(95)])
-            .to_dict()
-        )
-
-    metrics_dict_wide = {
-        f"{metrics_key}_{statistics_key}": value
-        for metrics_key, values in metrics_dict.items()
-        for statistics_key, value in values.items()
-    }
-
-    return metrics_dict_wide
```

### Comparing `etna-1.9.0/etna/loggers/console_logger.py` & `etna-2.0.0/etna/loggers/console_logger.py`

 * *Files identical despite different names*

### Comparing `etna-1.9.0/etna/loggers/file_logger.py` & `etna-2.0.0/etna/loggers/file_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from typing import Union
 
 import boto3
 import pandas as pd
 from botocore.exceptions import ClientError
 
 from etna.loggers.base import BaseLogger
-from etna.loggers.base import aggregate_metrics_df
 
 if TYPE_CHECKING:
     from etna.datasets import TSDataset
 
 DATETIME_FORMAT = "%Y-%m-%dT%H-%M-%S"
 
 
@@ -113,14 +112,15 @@
             Dataframe with ground truth
 
         Notes
         -----
         If some exception during saving is raised, then it becomes a warning.
         """
         from etna.datasets import TSDataset
+        from etna.metrics.utils import aggregate_metrics_df
 
         columns_name = list(metrics.columns)
         metrics = metrics.reset_index()
         metrics.columns = ["segment"] + columns_name
 
         try:
             self._save_table(metrics, "metrics")
@@ -154,14 +154,15 @@
             Fold information from backtest
 
         Notes
         -----
         If some exception during saving is raised, then it becomes a warning.
         """
         from etna.datasets import TSDataset
+        from etna.metrics.utils import aggregate_metrics_df
 
         try:
             self._save_table(metrics_df, "metrics")
             self._save_table(TSDataset.to_flatten(forecast_df), "forecast")
             self._save_table(fold_info_df, "fold_info")
         except Exception as e:
             warnings.warn(str(e), UserWarning)
```

### Comparing `etna-1.9.0/etna/loggers/wandb_logger.py` & `etna-2.0.0/etna/loggers/wandb_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Union
 from uuid import uuid4
 
 import pandas as pd
 
 from etna import SETTINGS
 from etna.loggers.base import BaseLogger
-from etna.loggers.base import aggregate_metrics_df
 
 if TYPE_CHECKING:
     from pytorch_lightning.loggers import WandbLogger as PLWandbLogger
 
     from etna.datasets import TSDataset
 
 if SETTINGS.wandb_required:
@@ -97,18 +96,18 @@
         msg:
             Message or dict to log
         kwargs:
             Parameters for changing additional info in log message
 
         Notes
         -----
-        We log nothing via current method in wandb case.
-        Currently you could call ``wandb.log`` by hand if you need this.
+        We log dictionary to wandb only.
         """
-        pass
+        if isinstance(msg, dict):
+            self.experiment.log(msg)
 
     def log_backtest_metrics(
         self, ts: "TSDataset", metrics_df: pd.DataFrame, forecast_df: pd.DataFrame, fold_info_df: pd.DataFrame
     ):
         """
         Write metrics to logger.
 
@@ -121,14 +120,15 @@
         forecast_df:
             Forecast from backtest
         fold_info_df:
             Fold information from backtest
         """
         from etna.analysis import plot_backtest_interactive
         from etna.datasets import TSDataset
+        from etna.metrics.utils import aggregate_metrics_df
 
         summary: Dict[str, Any] = dict()
         if self.table:
             summary["metrics"] = wandb.Table(data=metrics_df)
             summary["forecast"] = wandb.Table(data=TSDataset.to_flatten(forecast_df))
             summary["fold_info"] = wandb.Table(data=fold_info_df)
 
@@ -150,14 +150,15 @@
             Dataframe with metrics from backtest fold
         forecast:
             Dataframe with forecast
         test:
             Dataframe with ground truth
         """
         from etna.datasets import TSDataset
+        from etna.metrics.utils import aggregate_metrics_df
 
         columns_name = list(metrics.columns)
         metrics = metrics.reset_index()
         metrics.columns = ["segment"] + columns_name
         summary: Dict[str, Any] = dict()
         if self.table:
             summary["metrics"] = wandb.Table(data=metrics)
```

### Comparing `etna-1.9.0/etna/metrics/base.py` & `etna-2.0.0/etna/metrics/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from abc import ABC
+from abc import abstractmethod
 from enum import Enum
 from typing import Callable
 from typing import Dict
+from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
 
 from etna.core import BaseMixin
 from etna.datasets.tsdataset import TSDataset
@@ -20,15 +23,54 @@
     @classmethod
     def _missing_(cls, value):
         raise NotImplementedError(
             f"{value} is not a valid {cls.__name__}. Only {', '.join([repr(m.value) for m in cls])} aggregation allowed"
         )
 
 
-class Metric(BaseMixin):
+class AbstractMetric(ABC):
+    """Abstract class for metric."""
+
+    @abstractmethod
+    def __call__(self, y_true: TSDataset, y_pred: TSDataset) -> Union[float, Dict[str, float]]:
+        """
+        Compute metric's value with ``y_true`` and ``y_pred``.
+
+        Notes
+        -----
+        Note that if ``y_true`` and ``y_pred`` are not sorted Metric will sort it anyway
+
+        Parameters
+        ----------
+        y_true:
+            dataset with true time series values
+        y_pred:
+            dataset with predicted time series values
+
+        Returns
+        -------
+        :
+            metric's value aggregated over segments or not (depends on mode)
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def name(self) -> str:
+        """Metric name."""
+        pass
+
+    @property
+    @abstractmethod
+    def greater_is_better(self) -> Optional[bool]:
+        """Whether higher metric value is better."""
+        pass
+
+
+class Metric(AbstractMetric, BaseMixin):
     """
     Base class for all the multi-segment metrics.
 
     How it works: Metric computes ``metric_fn`` value for each segment in given forecast
     dataset and aggregates it according to mode.
     """
```

### Comparing `etna-1.9.0/etna/metrics/intervals_metrics.py` & `etna-2.0.0/etna/metrics/intervals_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,19 @@
             upper_quantile_flag = y_true[:, segment, "target"] <= y_pred[:, segment, f"target_{self.quantiles[1]:.4g}"]
             lower_quantile_flag = y_true[:, segment, "target"] >= y_pred[:, segment, f"target_{self.quantiles[0]:.4g}"]
 
             metrics_per_segment[segment] = np.mean(upper_quantile_flag * lower_quantile_flag)
         metrics = self._aggregate_metrics(metrics_per_segment)
         return metrics
 
+    @property
+    def greater_is_better(self) -> None:
+        """Whether higher metric value is better."""
+        return None
+
 
 class Width(Metric, _QuantileMetricMixin):
     """Mean width of prediction intervals.
 
     .. math::
         Width(y\_true, y\_pred) = \\frac{\\sum_{i=0}^{n-1}\\mid y\_pred_i^{upper\_quantile} - y\_pred_i^{lower\_quantile} \\mid}{n}
 
@@ -144,9 +149,14 @@
             lower_quantile = y_pred[:, segment, f"target_{self.quantiles[0]:.4g}"]
 
             metrics_per_segment[segment] = np.abs(lower_quantile - upper_quantile).mean()
 
         metrics = self._aggregate_metrics(metrics_per_segment)
         return metrics
 
+    @property
+    def greater_is_better(self) -> bool:
+        """Whether higher metric value is better."""
+        return False
+
 
 __all__ = ["Coverage", "Width"]
```

### Comparing `etna-1.9.0/etna/models/__init__.py` & `etna-2.0.0/etna/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 from etna import SETTINGS
+from etna.models.autoarima import AutoARIMAModel
 from etna.models.base import BaseAdapter
-from etna.models.base import BaseModel
-from etna.models.base import Model
-from etna.models.base import PerSegmentModel
-from etna.models.catboost import CatBoostModelMultiSegment
-from etna.models.catboost import CatBoostModelPerSegment
+from etna.models.base import ContextIgnorantModelType
+from etna.models.base import ContextRequiredModelType
+from etna.models.base import ModelType
+from etna.models.base import NonPredictionIntervalContextIgnorantAbstractModel
+from etna.models.base import NonPredictionIntervalContextRequiredAbstractModel
+from etna.models.base import NonPredictionIntervalModelType
+from etna.models.base import PredictionIntervalContextIgnorantAbstractModel
+from etna.models.base import PredictionIntervalContextRequiredAbstractModel
+from etna.models.base import PredictionIntervalModelType
+from etna.models.catboost import CatBoostMultiSegmentModel
+from etna.models.catboost import CatBoostPerSegmentModel
+from etna.models.deadline_ma import DeadlineMovingAverageModel
 from etna.models.holt_winters import HoltModel
 from etna.models.holt_winters import HoltWintersModel
 from etna.models.holt_winters import SimpleExpSmoothingModel
 from etna.models.linear import ElasticMultiSegmentModel
 from etna.models.linear import ElasticPerSegmentModel
 from etna.models.linear import LinearMultiSegmentModel
 from etna.models.linear import LinearPerSegmentModel
 from etna.models.moving_average import MovingAverageModel
 from etna.models.naive import NaiveModel
 from etna.models.sarimax import SARIMAXModel
 from etna.models.seasonal_ma import SeasonalMovingAverageModel
 from etna.models.sklearn import SklearnMultiSegmentModel
 from etna.models.sklearn import SklearnPerSegmentModel
+from etna.models.tbats import BATSModel
+from etna.models.tbats import TBATSModel
 
 if SETTINGS.prophet_required:
     from etna.models.prophet import ProphetModel
```

### Comparing `etna-1.9.0/etna/models/moving_average.py` & `etna-2.0.0/etna/models/moving_average.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 class MovingAverageModel(SeasonalMovingAverageModel):
     """MovingAverageModel averages previous series values to forecast future one.
 
     .. math::
         y_{t} = \\frac{\\sum_{i=1}^{n} y_{t-i} }{n},
 
     where :math:`n` is window size.
+
+    Notes
+    -----
+    This model supports in-sample and out-of-sample prediction decomposition.
+    Prediction components are corresponding target lags with weights of :math:`1/window`.
     """
 
     def __init__(self, window: int = 5):
         """
         Init MovingAverageModel.
 
         Parameters
```

### Comparing `etna-1.9.0/etna/models/sarimax.py` & `etna-2.0.0/etna/models/sarimax.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,393 @@
 import warnings
+from abc import abstractmethod
 from datetime import datetime
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 
+import numpy as np
 import pandas as pd
 from statsmodels.tools.sm_exceptions import ValueWarning
 from statsmodels.tsa.statespace.sarimax import SARIMAX
+from statsmodels.tsa.statespace.sarimax import SARIMAXResultsWrapper
+from statsmodels.tsa.statespace.simulation_smoother import SimulationSmoother
 
+from etna.libs.pmdarima_utils import seasonal_prediction_with_confidence
 from etna.models.base import BaseAdapter
-from etna.models.base import PerSegmentPredictionIntervalModel
+from etna.models.base import PredictionIntervalContextIgnorantAbstractModel
+from etna.models.mixins import PerSegmentModelMixin
+from etna.models.mixins import PredictionIntervalContextIgnorantModelMixin
+from etna.models.utils import determine_freq
+from etna.models.utils import determine_num_steps
+from etna.models.utils import select_observations
 
 warnings.filterwarnings(
     message="No frequency information was provided, so inferred frequency .* will be used",
     action="ignore",
     category=ValueWarning,
     module="statsmodels.tsa.base.tsa_model",
 )
 
 
-class _SARIMAXAdapter(BaseAdapter):
+class _SARIMAXBaseAdapter(BaseAdapter):
+    """Base class for adapters based on :py:class:`statsmodels.tsa.statespace.sarimax.SARIMAX`."""
+
+    def __init__(self):
+        self.regressor_columns = None
+        self._fit_results = None
+        self._freq = None
+        self._first_train_timestamp = None
+        self._last_train_timestamp = None
+
+    def fit(self, df: pd.DataFrame, regressors: List[str]) -> "_SARIMAXBaseAdapter":
+        """
+        Fits a SARIMAX model.
+
+        Parameters
+        ----------
+        df:
+            Features dataframe
+        regressors:
+            List of the columns with regressors
+
+        Returns
+        -------
+        :
+            Fitted model
+        """
+        self.regressor_columns = regressors
+
+        self._encode_categoricals(df)
+        self._check_df(df)
+
+        exog_train = self._select_regressors(df)
+        self._fit_results = self._get_fit_results(endog=df["target"], exog=exog_train)
+
+        self._freq = determine_freq(timestamps=df["timestamp"])
+        self._first_train_timestamp = df["timestamp"].min()
+        self._last_train_timestamp = df["timestamp"].max()
+
+        return self
+
+    def _make_prediction(
+        self, df: pd.DataFrame, prediction_interval: bool, quantiles: Sequence[float], dynamic: bool
+    ) -> pd.DataFrame:
+        """Make predictions taking into account ``dynamic`` parameter."""
+        if self._fit_results is None:
+            raise ValueError("Model is not fitted! Fit the model before calling predict method!")
+
+        horizon = len(df)
+        self._encode_categoricals(df)
+        self._check_df(df, horizon)
+
+        exog_future = self._select_regressors(df)
+        start_timestamp = df["timestamp"].min()
+        end_timestamp = df["timestamp"].max()
+        # determine index of start_timestamp if counting from first timestamp of train
+        start_idx = determine_num_steps(
+            start_timestamp=self._first_train_timestamp, end_timestamp=start_timestamp, freq=self._freq  # type: ignore
+        )
+        # determine index of end_timestamp if counting from first timestamp of train
+        end_idx = determine_num_steps(
+            start_timestamp=self._first_train_timestamp, end_timestamp=end_timestamp, freq=self._freq  # type: ignore
+        )
+
+        if prediction_interval:
+            forecast, _ = seasonal_prediction_with_confidence(
+                arima_res=self._fit_results, start=start_idx, end=end_idx, X=exog_future, alpha=0.05, dynamic=dynamic
+            )
+            y_pred = pd.DataFrame({"mean": forecast})
+            for quantile in quantiles:
+                # set alpha in the way to get a desirable quantile
+                alpha = min(quantile * 2, (1 - quantile) * 2)
+                _, borders = seasonal_prediction_with_confidence(
+                    arima_res=self._fit_results,
+                    start=start_idx,
+                    end=end_idx,
+                    X=exog_future,
+                    alpha=alpha,
+                    dynamic=dynamic,
+                )
+                if quantile < 1 / 2:
+                    series = borders[:, 0]
+                else:
+                    series = borders[:, 1]
+                y_pred[f"mean_{quantile:.4g}"] = series
+        else:
+            forecast, _ = seasonal_prediction_with_confidence(
+                arima_res=self._fit_results, start=start_idx, end=end_idx, X=exog_future, alpha=0.05, dynamic=dynamic
+            )
+            y_pred = pd.DataFrame({"mean": forecast})
+
+        rename_dict = {
+            column: column.replace("mean", "target") for column in y_pred.columns if column.startswith("mean")
+        }
+        y_pred = y_pred.rename(rename_dict, axis=1)
+        return y_pred
+
+    def forecast(self, df: pd.DataFrame, prediction_interval: bool, quantiles: Sequence[float]) -> pd.DataFrame:
+        """
+        Compute autoregressive predictions from a SARIMAX model.
+
+        Parameters
+        ----------
+        df:
+            Features dataframe
+        prediction_interval:
+             If True returns prediction interval for forecast
+        quantiles:
+            Levels of prediction distribution
+
+        Returns
+        -------
+        :
+            DataFrame with predictions
+        """
+        return self._make_prediction(df=df, prediction_interval=prediction_interval, quantiles=quantiles, dynamic=True)
+
+    def predict(self, df: pd.DataFrame, prediction_interval: bool, quantiles: Sequence[float]) -> pd.DataFrame:
+        """
+        Compute predictions from a SARIMAX model and use true in-sample data as lags if possible.
+
+        Parameters
+        ----------
+        df:
+            Features dataframe
+        prediction_interval:
+            If True returns prediction interval for forecast
+        quantiles:
+            Levels of prediction distribution
+
+        Returns
+        -------
+        :
+            DataFrame with predictions
+        """
+        return self._make_prediction(df=df, prediction_interval=prediction_interval, quantiles=quantiles, dynamic=False)
+
+    @abstractmethod
+    def _get_fit_results(self, endog: pd.Series, exog: pd.DataFrame) -> SARIMAXResultsWrapper:
+        pass
+
+    def _check_df(self, df: pd.DataFrame, horizon: Optional[int] = None):
+        if self.regressor_columns is None:
+            raise ValueError("Something went wrong, regressor_columns is None!")
+        column_to_drop = [col for col in df.columns if col not in ["target", "timestamp"] + self.regressor_columns]
+        if column_to_drop:
+            warnings.warn(
+                message=f"SARIMAX model does not work with exogenous features (features unknown in future).\n "
+                f"{column_to_drop} will be dropped"
+            )
+        if horizon:
+            short_regressors = [regressor for regressor in self.regressor_columns if df[regressor].count() < horizon]
+            if short_regressors:
+                raise ValueError(
+                    f"Regressors {short_regressors} are too short for chosen horizon value.\n "
+                    "Try lower horizon value, or drop this regressors."
+                )
+
+    def _select_regressors(self, df: pd.DataFrame) -> Optional[pd.DataFrame]:
+        if self.regressor_columns:
+            exog_future = df[self.regressor_columns]
+            exog_future.index = df["timestamp"]
+        else:
+            exog_future = None
+        return exog_future
+
+    def _encode_categoricals(self, df: pd.DataFrame) -> None:
+        categorical_cols = df.select_dtypes(include=["category"]).columns.tolist()
+        try:
+            df.loc[:, categorical_cols] = df[categorical_cols].astype(int)
+        except ValueError:
+            raise ValueError(
+                f"Categorical columns {categorical_cols} can not been converted to int.\n "
+                "Try to encode this columns manually."
+            )
+
+    def get_model(self) -> SARIMAXResultsWrapper:
+        """Get :py:class:`statsmodels.tsa.statespace.sarimax.SARIMAXResultsWrapper` that is used inside etna class.
+
+        Returns
+        -------
+        :
+           Internal model
+        """
+        return self._fit_results
+
+    @staticmethod
+    def _prepare_components_df(components: np.ndarray, model: SARIMAX) -> pd.DataFrame:
+        """Prepare `pd.DataFrame` with components."""
+        if model.exog_names is not None:
+            components_names = model.exog_names[:]
+        else:
+            components_names = []
+
+        if model.seasonal_periods == 0:
+            components_names.append("arima")
+        else:
+            components_names.append("sarima")
+
+        df = pd.DataFrame(data=components, columns=components_names)
+        return df.add_prefix("target_component_")
+
+    @staticmethod
+    def _prepare_design_matrix(ssm: SimulationSmoother) -> np.ndarray:
+        """Extract design matrix from state space model."""
+        design_mat = ssm["design"]
+        if len(design_mat.shape) == 2:
+            design_mat = design_mat[..., np.newaxis]
+
+        return design_mat
+
+    def _mle_regression_decomposition(self, state: np.ndarray, ssm: SimulationSmoother, exog: np.ndarray) -> np.ndarray:
+        """Estimate SARIMAX components for MLE regression case.
+
+        SARIMAX representation as SSM: https://www.statsmodels.org/dev/statespace.html
+        In MLE case exogenous data fitted separately from other components:
+        https://github.com/statsmodels/statsmodels/blob/main/statsmodels/tsa/statespace/sarimax.py#L1644
+        """
+        # get design matrix from SSM
+        design_mat = self._prepare_design_matrix(ssm)
+
+        # estimate SARIMA component
+        components = np.sum(design_mat * state, axis=1).T
+
+        if len(exog) > 0:
+            # restore parameters for exogenous variabales
+            exog_params = np.linalg.lstsq(a=exog, b=np.squeeze(ssm["obs_intercept"]))[0]
+
+            # estimate exogenous components and append to others
+            weighted_exog = exog * exog_params[np.newaxis]
+            components = np.concatenate([weighted_exog, components], axis=1)
+
+        return components
+
+    def _state_regression_decomposition(self, state: np.ndarray, ssm: SimulationSmoother, k_exog: int) -> np.ndarray:
+        """Estimate SARIMAX components for state regression case.
+
+        SARIMAX representation as SSM: https://www.statsmodels.org/dev/statespace.html
+        In state regression case parameters for exogenous variables estimated inside SSM.
+        """
+        # get design matrix from SSM
+        design_mat = self._prepare_design_matrix(ssm)
+
+        if k_exog > 0:
+            # estimate SARIMA component
+            sarima = np.sum(design_mat[:, :-k_exog] * state[:-k_exog], axis=1)
+
+            # obtain params from SSM and estimate exogenous components
+            weighted_exog = np.squeeze(design_mat[:, -k_exog:] * state[-k_exog:])
+            components = np.concatenate([weighted_exog, sarima], axis=0).T
+
+        else:
+            # in this case we can take whole matrix for SARIMA component
+            components = np.sum(design_mat * state, axis=1).T
+
+        return components
+
+    def predict_components(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Estimate prediction components.
+
+        Parameters
+        ----------
+        df:
+            features dataframe
+
+        Returns
+        -------
+        :
+            dataframe with prediction components
+        """
+        if df["timestamp"].min() < self._first_train_timestamp or df["timestamp"].max() > self._last_train_timestamp:
+            raise ValueError("To estimate out-of-sample prediction decomposition use `forecast` method.")
+
+        fit_results = self._fit_results
+        model = fit_results.model
+
+        if model.hamilton_representation:
+            raise ValueError("Prediction decomposition is not implemented for Hamilton representation of ARMA!")
+
+        state = fit_results.predicted_state[:, :-1]
+
+        if model.mle_regression:
+            components = self._mle_regression_decomposition(state=state, ssm=model.ssm, exog=model.exog)
+
+        else:
+            components = self._state_regression_decomposition(state=state, ssm=model.ssm, k_exog=model.k_exog)
+
+        components_df = self._prepare_components_df(components=components, model=model)
+
+        components_df = select_observations(
+            df=components_df,
+            timestamps=df["timestamp"],
+            start=self._first_train_timestamp,
+            end=self._last_train_timestamp,
+            freq=self._freq,
+        )
+
+        return components_df
+
+    def forecast_components(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Estimate forecast components.
+
+        Parameters
+        ----------
+        df:
+            features dataframe
+
+        Returns
+        -------
+        :
+            dataframe with forecast components
+        """
+        if df["timestamp"].min() <= self._last_train_timestamp:
+            raise ValueError("To estimate in-sample prediction decomposition use `predict` method.")
+
+        horizon = determine_num_steps(
+            start_timestamp=self._last_train_timestamp, end_timestamp=df["timestamp"].max(), freq=self._freq
+        )
+
+        fit_results = self._fit_results
+
+        model = fit_results.model
+        if model.hamilton_representation:
+            raise ValueError("Prediction decomposition is not implemented for Hamilton representation of ARMA!")
+
+        self._encode_categoricals(df)
+        self._check_df(df, horizon)
+
+        exog_future = self._select_regressors(df)
+
+        forecast_results = fit_results.get_forecast(horizon, exog=exog_future).prediction_results.results
+        state = forecast_results.predicted_state[:, :-1]
+
+        if model.mle_regression:
+            # If there are no exog variales `mle_regression` will be set to `False`
+            # even if user set to `True`.
+            components = self._mle_regression_decomposition(
+                state=state, ssm=forecast_results.model, exog=exog_future.values  # type: ignore
+            )
+
+        else:
+            components = self._state_regression_decomposition(
+                state=state, ssm=forecast_results.model, k_exog=model.k_exog
+            )
+
+        components_df = self._prepare_components_df(components=components, model=model)
+
+        components_df = select_observations(
+            df=components_df, timestamps=df["timestamp"], end=df["timestamp"].max(), periods=horizon, freq=self._freq
+        )
+
+        return components_df
+
+
+class _SARIMAXAdapter(_SARIMAXBaseAdapter):
     """
     Class for holding Sarimax model.
 
     Notes
     -----
     We use SARIMAX [1] model from statsmodels package. Statsmodels package uses `exog` attribute for
     `exogenous regressors` which should be known in future, however we use exogenous for
@@ -157,54 +520,22 @@
         self.trend_offset = trend_offset
         self.use_exact_diffuse = use_exact_diffuse
         self.dates = dates
         self.freq = freq
         self.missing = missing
         self.validate_specification = validate_specification
         self.kwargs = kwargs
-        self._model: Optional[SARIMAX] = None
-        self._result: Optional[SARIMAX] = None
-        self.regressor_columns: Optional[List[str]] = None
-
-    def fit(self, df: pd.DataFrame, regressors: List[str]) -> "_SARIMAXAdapter":
-        """
-        Fits a SARIMAX model.
-
-        Parameters
-        ----------
-        df:
-            Features dataframe
-        regressors:
-            List of the columns with regressors
-
-        Returns
-        -------
-        :
-            Fitted model
-        """
-        self.regressor_columns = regressors
-        categorical_cols = df.select_dtypes(include=["category"]).columns.tolist()
-        try:
-            df.loc[:, categorical_cols] = df[categorical_cols].astype(int)
-        except ValueError:
-            raise ValueError(
-                f"Categorical columns {categorical_cols} can not been converted to int.\n "
-                "Try to encode this columns manually."
-            )
+        super().__init__()
 
-        self._check_df(df)
-
-        targets = df["target"]
-        targets.index = df["timestamp"]
-
-        exog_train = self._select_regressors(df)
-
-        self._model = SARIMAX(
-            endog=targets,
-            exog=exog_train,
+    def _get_fit_results(self, endog: pd.Series, exog: pd.DataFrame):
+        # make it a numpy array for forgetting about indices, it is necessary for seasonal_prediction_with_confidence
+        endog_np = endog.values
+        model = SARIMAX(
+            endog=endog_np,
+            exog=exog,
             order=self.order,
             seasonal_order=self.seasonal_order,
             trend=self.trend,
             measurement_error=self.measurement_error,
             time_varying_regression=self.time_varying_regression,
             mle_regression=self.mle_regression,
             simple_differencing=self.simple_differencing,
@@ -216,126 +547,37 @@
             use_exact_diffuse=self.use_exact_diffuse,
             dates=self.dates,
             freq=self.freq,
             missing=self.missing,
             validate_specification=self.validate_specification,
             **self.kwargs,
         )
-        self._result = self._model.fit()
-        return self
+        result = model.fit()
+        return result
 
-    def predict(self, df: pd.DataFrame, prediction_interval: bool, quantiles: Sequence[float]) -> pd.DataFrame:
-        """
-        Compute predictions from a SARIMAX model.
 
-        Parameters
-        ----------
-        df:
-            Features dataframe
-        prediction_interval:
-             If True returns prediction interval for forecast
-        quantiles:
-            Levels of prediction distribution
-
-        Returns
-        -------
-        :
-            DataFrame with predictions
-        """
-        if self._result is None or self._model is None:
-            raise ValueError("SARIMAX model is not fitted! Fit the model before calling predict method!")
-        horizon = len(df)
-        self._check_df(df, horizon)
-
-        categorical_cols = df.select_dtypes(include=["category"]).columns.tolist()
-        try:
-            df.loc[:, categorical_cols] = df[categorical_cols].astype(int)
-        except ValueError:
-            raise ValueError(
-                f"Categorical columns {categorical_cols} can not been converted to int.\n "
-                "Try to encode this columns manually."
-            )
-
-        exog_future = self._select_regressors(df)
-        if prediction_interval:
-            forecast = self._result.get_prediction(
-                start=df["timestamp"].min(), end=df["timestamp"].max(), dynamic=False, exog=exog_future
-            )
-            y_pred = forecast.predicted_mean
-            y_pred.name = "mean"
-            y_pred = pd.DataFrame(y_pred)
-            for quantile in quantiles:
-                # set alpha in the way to get a desirable quantile
-                alpha = min(quantile * 2, (1 - quantile) * 2)
-                borders = forecast.conf_int(alpha=alpha)
-                if quantile < 1 / 2:
-                    series = borders["lower target"]
-                else:
-                    series = borders["upper target"]
-                y_pred[f"mean_{quantile:.4g}"] = series
-        else:
-            forecast = self._result.get_prediction(
-                start=df["timestamp"].min(), end=df["timestamp"].max(), dynamic=True, exog=exog_future
-            )
-            y_pred = forecast.predicted_mean
-            y_pred.name = "mean"
-            y_pred = pd.DataFrame(y_pred)
-        y_pred = y_pred.reset_index(drop=True, inplace=False)
-        rename_dict = {
-            column: column.replace("mean", "target") for column in y_pred.columns if column.startswith("mean")
-        }
-        y_pred = y_pred.rename(rename_dict, axis=1)
-        return y_pred
-
-    def _check_df(self, df: pd.DataFrame, horizon: Optional[int] = None):
-        if self.regressor_columns is None:
-            raise ValueError("Something went wrong, regressor_columns is None!")
-        column_to_drop = [col for col in df.columns if col not in ["target", "timestamp"] + self.regressor_columns]
-        if column_to_drop:
-            warnings.warn(
-                message=f"SARIMAX model does not work with exogenous features (features unknown in future).\n "
-                f"{column_to_drop} will be dropped"
-            )
-        if horizon:
-            short_regressors = [regressor for regressor in self.regressor_columns if df[regressor].count() < horizon]
-            if short_regressors:
-                raise ValueError(
-                    f"Regressors {short_regressors} are too short for chosen horizon value.\n "
-                    "Try lower horizon value, or drop this regressors."
-                )
-
-    def _select_regressors(self, df: pd.DataFrame) -> Optional[pd.DataFrame]:
-        if self.regressor_columns:
-            exog_future = df[self.regressor_columns]
-            exog_future.index = df["timestamp"]
-        else:
-            exog_future = None
-        return exog_future
-
-    def get_model(self) -> SARIMAX:
-        """Get internal statsmodels.tsa.statespace.sarimax.SARIMAX model that is used inside etna class.
-
-        Returns
-        -------
-        :
-           Internal model
-        """
-        return self._model
-
-
-class SARIMAXModel(PerSegmentPredictionIntervalModel):
+class SARIMAXModel(
+    PerSegmentModelMixin, PredictionIntervalContextIgnorantModelMixin, PredictionIntervalContextIgnorantAbstractModel
+):
     """
     Class for holding Sarimax model.
 
+    Method ``predict`` can use true target values only on train data on future data autoregression
+    forecasting will be made even if targets are known.
+
     Notes
     -----
     We use :py:class:`statsmodels.tsa.sarimax.SARIMAX`. Statsmodels package uses `exog` attribute for
     `exogenous regressors` which should be known in future, however we use exogenous for
     additional features what is not known in future, and regressors for features we do know in
     future.
+
+    This model supports in-sample and out-of-sample prediction decomposition.
+    Prediction components for SARIMAX model are: exogenous and SARIMA components.
+    Decomposition is obtained directly from fitted model parameters.
     """
 
     def __init__(
         self,
         order: Tuple[int, int, int] = (2, 1, 0),
         seasonal_order: Tuple[int, int, int, int] = (1, 1, 0, 12),
         trend: Optional[str] = "c",
```

### Comparing `etna-1.9.0/etna/models/sklearn.py` & `etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,113 @@
-from typing import List
 from typing import Optional
 
 import numpy as np
-import pandas as pd
 from sklearn.base import RegressorMixin
+from sklearn.base import TransformerMixin
+from sklearn.linear_model import LinearRegression
 
-from etna.models.base import BaseAdapter
-from etna.models.base import MultiSegmentModel
-from etna.models.base import PerSegmentModel
+from etna.transforms.decomposition.change_points_based.per_interval_models.base import PerIntervalModel
 
 
-class _SklearnAdapter(BaseAdapter):
-    def __init__(self, regressor: RegressorMixin):
-        self.model = regressor
-        self.regressor_columns: Optional[List[str]] = None
+class SklearnRegressionPerIntervalModel(PerIntervalModel):
+    """SklearnRegressionPerIntervalModel applies PerIntervalModel interface for sklearn-like regression models."""
 
-    def fit(self, df: pd.DataFrame, regressors: List[str]) -> "_SklearnAdapter":
+    def __init__(self, model: Optional[RegressorMixin] = None):
+        """Init SklearnPerIntervalModel.
+
+        Parameters
+        ----------
+        model:
+            model with sklearn interface to use for interval processing
         """
-        Fit Sklearn model.
+        self.model = model if model is not None else LinearRegression()
+
+    def fit(self, features: np.ndarray, target: np.ndarray, *args, **kwargs) -> "SklearnRegressionPerIntervalModel":
+        """Fit model with given features and targets.
 
         Parameters
         ----------
-        df:
-            Features dataframe
-        regressors:
-            List of the columns with regressors
+        features:
+            features to fit model with
+        target:
+            targets to fit model
 
         Returns
         -------
-        :
-            Fitted model
+        self:
+            fitted SklearnRegressionPerIntervalModel
         """
-        self.regressor_columns = regressors
-        try:
-            features = df[self.regressor_columns].apply(pd.to_numeric)
-        except ValueError:
-            raise ValueError("Only convertible to numeric features are accepted!")
-        target = df["target"]
-        self.model.fit(features, target)
+        self.model.fit(X=features, y=target)
         return self
 
-    def predict(self, df: pd.DataFrame) -> np.ndarray:
-        """
-        Compute predictions from a Sklearn model.
+    def predict(self, features: np.ndarray, *args, **kwargs) -> np.ndarray:
+        """Make prediction for given features.
 
         Parameters
         ----------
-        df:
-            Features dataframe
+        features:
+            features to make prediction for
 
         Returns
         -------
-        :
-            Array with predictions
+        prediction:
+            model's prediction for given features
         """
-        try:
-            features = df[self.regressor_columns].apply(pd.to_numeric)
-        except ValueError:
-            raise ValueError("Only convertible to numeric features are accepted!")
-        pred = self.model.predict(features)
-        return pred
+        return self.model.predict(X=features)
 
-    def get_model(self) -> RegressorMixin:
-        """Get internal sklearn model that is used inside etna class.
 
-        Returns
-        -------
-        :
-           Internal model
-        """
-        return self.model
+class SklearnPreprocessingPerIntervalModel(PerIntervalModel):
+    """SklearnPreprocessingPerIntervalModel applies PerIntervalModel interface for sklearn preprocessings."""
 
+    def __init__(self, preprocessing: TransformerMixin):
+        self.preprocessing = preprocessing
 
-class SklearnPerSegmentModel(PerSegmentModel):
-    """Class for holding per segment Sklearn model."""
-
-    def __init__(self, regressor: RegressorMixin):
-        """
-        Create instance of SklearnPerSegmentModel with given parameters.
+    def fit(self, features: np.ndarray, target: np.ndarray, *args, **kwargs) -> "SklearnPreprocessingPerIntervalModel":
+        """Fit preprocessing with given features and targets.
 
         Parameters
         ----------
-        regressor:
-            sklearn model for regression
+        features:
+            features to fit preprocessing with
+        target:
+            targets to apply preprocessing to
+
+        Returns
+        -------
+        self:
+            fitted SklearnPreprocessingPerIntervalModel
         """
-        super().__init__(base_model=_SklearnAdapter(regressor=regressor))
+        self.preprocessing.fit(X=features.reshape(-1, 1), y=target)
+        return self
 
+    def predict(self, features: np.ndarray, *args, **kwargs) -> np.ndarray:
+        """Apply preprocessing to given features.
 
-class SklearnMultiSegmentModel(MultiSegmentModel):
-    """Class for holding Sklearn model for all segments."""
+        Parameters
+        ----------
+        features:
+            features to make preprocessing for
 
-    def __init__(self, regressor: RegressorMixin):
+        Returns
+        -------
+        prediction:
+            preprocessing's prediction for given features
         """
-        Create instance of SklearnMultiSegmentModel with given parameters.
+        prediction = self.preprocessing.transform(X=features.reshape(-1, 1)).reshape(
+            -1,
+        )
+        return prediction
+
+    def inverse(self, features: np.ndarray) -> np.ndarray:
+        """Apply inverse transformation.
 
         Parameters
         ----------
-        regressor:
-            Sklearn model for regression
+        features:
+            features to apply inverse transformation
+
+        Returns
+        -------
+        inversed data:
+            features after inverse transformation
         """
-        super().__init__(base_model=_SklearnAdapter(regressor=regressor))
+        return self.preprocessing.inverse_transform(features.reshape(-1, 1)).reshape(-1, 1)
```

### Comparing `etna-1.9.0/etna/pipeline/autoregressive_pipeline.py` & `etna-2.0.0/etna/pipeline/pipeline.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,146 +1,144 @@
-import warnings
+from typing import Optional
 from typing import Sequence
+from typing import cast
 
-import pandas as pd
+from typing_extensions import get_args
 
 from etna.datasets import TSDataset
-from etna.models.base import BaseModel
+from etna.models.base import ContextIgnorantModelType
+from etna.models.base import ContextRequiredModelType
+from etna.models.base import ModelType
+from etna.models.base import PredictionIntervalContextIgnorantAbstractModel
+from etna.models.base import PredictionIntervalContextRequiredAbstractModel
 from etna.pipeline.base import BasePipeline
-from etna.transforms import Transform
+from etna.pipeline.mixins import ModelPipelinePredictMixin
+from etna.pipeline.mixins import SaveModelPipelineMixin
+from etna.transforms.base import Transform
 
 
-class AutoRegressivePipeline(BasePipeline):
-    """Pipeline that make regressive models autoregressive.
+class Pipeline(ModelPipelinePredictMixin, SaveModelPipelineMixin, BasePipeline):
+    """Pipeline of transforms with a final estimator."""
 
-    Examples
-    --------
-    >>> from etna.datasets import generate_periodic_df
-    >>> from etna.datasets import TSDataset
-    >>> from etna.models import LinearPerSegmentModel
-    >>> from etna.transforms import LagTransform
-    >>> classic_df = generate_periodic_df(
-    ...     periods=100,
-    ...     start_time="2020-01-01",
-    ...     n_segments=4,
-    ...     period=7,
-    ...     sigma=3
-    ... )
-    >>> df = TSDataset.to_dataset(df=classic_df)
-    >>> ts = TSDataset(df, freq="D")
-    >>> horizon = 7
-    >>> transforms = [
-    ...     LagTransform(in_column="target", lags=list(range(1, horizon+1)))
-    ... ]
-    >>> model = LinearPerSegmentModel()
-    >>> pipeline = AutoRegressivePipeline(model, horizon, transforms, step=1)
-    >>> _ = pipeline.fit(ts=ts)
-    >>> forecast = pipeline.forecast()
-    >>> pd.options.display.float_format = '{:,.2f}'.format
-    >>> forecast[:, :, "target"]
-    segment    segment_0 segment_1 segment_2 segment_3
-    feature       target    target    target    target
-    timestamp
-    2020-04-10      9.00      9.00      4.00      6.00
-    2020-04-11      5.00      2.00      7.00      9.00
-    2020-04-12      0.00      4.00      7.00      9.00
-    2020-04-13      0.00      5.00      9.00      7.00
-    2020-04-14      1.00      2.00      1.00      6.00
-    2020-04-15      5.00      7.00      4.00      7.00
-    2020-04-16      8.00      6.00      2.00      0.00
-    """
-
-    def __init__(self, model: BaseModel, horizon: int, transforms: Sequence[Transform] = (), step: int = 1):
+    def __init__(self, model: ModelType, transforms: Sequence[Transform] = (), horizon: int = 1):
         """
-        Create instance of AutoRegressivePipeline with given parameters.
+        Create instance of Pipeline with given parameters.
 
         Parameters
         ----------
         model:
             Instance of the etna Model
-        horizon:
-            Number of timestamps in the future for forecasting
         transforms:
             Sequence of the transforms
-        step:
-            Size of prediction for one step of forecasting
+        horizon:
+            Number of timestamps in the future for forecasting
         """
         self.model = model
         self.transforms = transforms
-        self.step = step
         super().__init__(horizon=horizon)
 
-    def fit(self, ts: TSDataset) -> "AutoRegressivePipeline":
-        """Fit the AutoRegressivePipeline.
+    def fit(self, ts: TSDataset) -> "Pipeline":
+        """Fit the Pipeline.
 
         Fit and apply given transforms to the data, then fit the model on the transformed data.
 
         Parameters
         ----------
         ts:
             Dataset with timeseries data
 
         Returns
         -------
         :
             Fitted Pipeline instance
         """
         self.ts = ts
-        ts.fit_transform(self.transforms)
-        self.model.fit(ts)
-        self.ts.inverse_transform()
+        self.ts.fit_transform(self.transforms)
+        self.model.fit(self.ts)
+        self.ts.inverse_transform(self.transforms)
         return self
 
-    def _create_predictions_template(self) -> pd.DataFrame:
-        """Create dataframe to fill with forecasts."""
-        if self.ts is None:
-            raise ValueError(
-                "AutoRegressivePipeline is not fitted! Fit the AutoRegressivePipeline before calling forecast method."
-            )
-        prediction_df = self.ts[:, :, "target"]
-        future_dates = pd.date_range(
-            start=prediction_df.index.max(), periods=self.horizon + 1, freq=self.ts.freq, closed="right"
-        )
-        prediction_df = prediction_df.reindex(prediction_df.index.append(future_dates))
-        prediction_df.index.name = "timestamp"
-        return prediction_df
-
-    def _forecast(self) -> TSDataset:
+    def _forecast(self, ts: TSDataset, return_components: bool) -> TSDataset:
         """Make predictions."""
-        if self.ts is None:
-            raise ValueError("Something went wrong, ts is None!")
-        prediction_df = self._create_predictions_template()
-
-        for idx_start in range(0, self.horizon, self.step):
-            current_step = min(self.step, self.horizon - idx_start)
-            current_idx_border = self.ts.index.shape[0] + idx_start
-            current_ts = TSDataset(
-                df=prediction_df.iloc[:current_idx_border],
-                freq=self.ts.freq,
-                df_exog=self.ts.df_exog,
-                known_future=self.ts.known_future,
-            )
-            # manually set transforms in current_ts, otherwise make_future won't know about them
-            current_ts.transforms = self.transforms
-            with warnings.catch_warnings():
-                warnings.filterwarnings(
-                    message="TSDataset freq can't be inferred",
-                    action="ignore",
-                )
-                warnings.filterwarnings(
-                    message="You probably set wrong freq.",
-                    action="ignore",
+        if isinstance(self.model, get_args(ContextRequiredModelType)):
+            self.model = cast(ContextRequiredModelType, self.model)
+            future = ts.make_future(
+                future_steps=self.horizon, transforms=self.transforms, tail_steps=self.model.context_size
+            )
+            predictions = self.model.forecast(
+                ts=future, prediction_size=self.horizon, return_components=return_components
+            )
+        else:
+            self.model = cast(ContextIgnorantModelType, self.model)
+            future = ts.make_future(future_steps=self.horizon, transforms=self.transforms)
+            predictions = self.model.forecast(ts=future, return_components=return_components)
+        return predictions
+
+    def forecast(
+        self,
+        ts: Optional[TSDataset] = None,
+        prediction_interval: bool = False,
+        quantiles: Sequence[float] = (0.025, 0.975),
+        n_folds: int = 3,
+        return_components: bool = False,
+    ) -> TSDataset:
+        """Make a forecast of the next points of a dataset.
+
+        The result of forecasting starts from the last point of ``ts``, not including it.
+
+        Parameters
+        ----------
+        ts:
+            Dataset to forecast. If not given, dataset given during :py:meth:``fit`` is used.
+        prediction_interval:
+            If True returns prediction interval for forecast
+        quantiles:
+            Levels of prediction distribution. By default 2.5% and 97.5% taken to form a 95% prediction interval
+        n_folds:
+            Number of folds to use in the backtest for prediction interval estimation
+        return_components:
+            If True additionally returns forecast components
+
+        Returns
+        -------
+        :
+            Dataset with predictions
+        """
+        if ts is None:
+            if self.ts is None:
+                raise ValueError(
+                    "There is no ts to forecast! Pass ts into forecast method or make sure that pipeline is loaded with ts."
                 )
-                current_ts_forecast = current_ts.make_future(current_step)
-            current_ts_future = self.model.forecast(current_ts_forecast)
-            prediction_df = prediction_df.combine_first(current_ts_future.to_pandas()[prediction_df.columns])
-
-        # construct dataset and add all features
-        prediction_ts = TSDataset(
-            df=prediction_df, freq=self.ts.freq, df_exog=self.ts.df_exog, known_future=self.ts.known_future
-        )
-        prediction_ts.transform(self.transforms)
-        prediction_ts.inverse_transform()
-        # cut only last timestamps from result dataset
-        prediction_ts.df = prediction_ts.df.tail(self.horizon)
-        prediction_ts.raw_df = prediction_ts.raw_df.tail(self.horizon)
-        return prediction_ts
+            ts = self.ts
+
+        self._validate_quantiles(quantiles=quantiles)
+        self._validate_backtest_n_folds(n_folds=n_folds)
+
+        if prediction_interval and isinstance(self.model, PredictionIntervalContextIgnorantAbstractModel):
+            future = ts.make_future(future_steps=self.horizon, transforms=self.transforms)
+            predictions = self.model.forecast(
+                ts=future,
+                prediction_interval=prediction_interval,
+                quantiles=quantiles,
+                return_components=return_components,
+            )
+        elif prediction_interval and isinstance(self.model, PredictionIntervalContextRequiredAbstractModel):
+            future = ts.make_future(
+                future_steps=self.horizon, transforms=self.transforms, tail_steps=self.model.context_size
+            )
+            predictions = self.model.forecast(
+                ts=future,
+                prediction_size=self.horizon,
+                prediction_interval=prediction_interval,
+                quantiles=quantiles,
+                return_components=return_components,
+            )
+        else:
+            predictions = super().forecast(
+                ts=ts,
+                prediction_interval=prediction_interval,
+                quantiles=quantiles,
+                n_folds=n_folds,
+                return_components=return_components,
+            )
+        predictions.inverse_transform(self.transforms)
+        return predictions
```

### Comparing `etna-1.9.0/etna/pipeline/base.py` & `etna-2.0.0/etna/pipeline/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from abc import ABC
+import math
 from abc import abstractmethod
 from copy import deepcopy
 from enum import Enum
 from typing import Any
 from typing import Dict
 from typing import Generator
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
-import scipy
 from joblib import Parallel
 from joblib import delayed
 from scipy.stats import norm
+from typing_extensions import TypedDict
+from typing_extensions import assert_never
 
+from etna.core import AbstractSaveable
 from etna.core import BaseMixin
 from etna.datasets import TSDataset
 from etna.loggers import tslogger
 from etna.metrics import MAE
 from etna.metrics import Metric
 from etna.metrics import MetricAggregationMode
 
@@ -30,14 +32,20 @@
 
 class CrossValidationMode(Enum):
     """Enum for different cross-validation modes."""
 
     expand = "expand"
     constant = "constant"
 
+    @classmethod
+    def _missing_(cls, value):
+        raise NotImplementedError(
+            f"{value} is not a valid {cls.__name__}. Only {', '.join([repr(m.value) for m in cls])} modes allowed"
+        )
+
 
 class FoldMask(BaseMixin):
     """Container to hold the description of the fold mask.
 
     Fold masks are expected to be used for backtest strategy customization.
     """
 
@@ -85,15 +93,15 @@
             Dataset to validate on
         horizon:
             Forecasting horizon
         """
         dataset_timestamps = list(ts.index)
         dataset_description = ts.describe()
 
-        min_first_timestamp = dataset_description["start_timestamp"].min()
+        min_first_timestamp = ts.index.min()
         if self.first_train_timestamp and self.first_train_timestamp < min_first_timestamp:
             raise ValueError(f"First train timestamp should be later than {min_first_timestamp}!")
 
         last_timestamp = dataset_description["end_timestamp"].min()
         if self.last_train_timestamp > last_timestamp:
             raise ValueError(f"Last train timestamp should be not later than {last_timestamp}!")
 
@@ -106,15 +114,15 @@
             dataset_timestamps.index(self.last_train_timestamp) + horizon
         ]
         mask_last_target_timestamp = self.target_timestamps[-1]
         if dataset_last_target_timestamp < mask_last_target_timestamp:
             raise ValueError(f"Last target timestamp should be not later than {dataset_last_target_timestamp}!")
 
 
-class AbstractPipeline(ABC):
+class AbstractPipeline(AbstractSaveable):
     """Interface for pipeline."""
 
     @abstractmethod
     def fit(self, ts: TSDataset) -> "AbstractPipeline":
         """Fit the Pipeline.
 
         Parameters
@@ -127,74 +135,158 @@
         :
             Fitted Pipeline instance
         """
         pass
 
     @abstractmethod
     def forecast(
-        self, prediction_interval: bool = False, quantiles: Sequence[float] = (0.025, 0.975), n_folds: int = 3
+        self,
+        ts: Optional[TSDataset] = None,
+        prediction_interval: bool = False,
+        quantiles: Sequence[float] = (0.025, 0.975),
+        n_folds: int = 3,
+        return_components: bool = False,
     ) -> TSDataset:
-        """Make predictions.
+        """Make a forecast of the next points of a dataset.
+
+        The result of forecasting starts from the last point of ``ts``, not including it.
 
         Parameters
         ----------
+        ts:
+            Dataset to forecast. If not given, dataset given during :py:meth:``fit`` is used.
         prediction_interval:
             If True returns prediction interval for forecast
         quantiles:
             Levels of prediction distribution. By default 2.5% and 97.5% taken to form a 95% prediction interval
         n_folds:
             Number of folds to use in the backtest for prediction interval estimation
+        return_components:
+            If True additionally returns forecast components
 
         Returns
         -------
         :
             Dataset with predictions
         """
         pass
 
     @abstractmethod
+    def predict(
+        self,
+        ts: TSDataset,
+        start_timestamp: Optional[pd.Timestamp] = None,
+        end_timestamp: Optional[pd.Timestamp] = None,
+        prediction_interval: bool = False,
+        quantiles: Sequence[float] = (0.025, 0.975),
+        return_components: bool = False,
+    ) -> TSDataset:
+        """Make in-sample predictions on dataset in a given range.
+
+        Currently, in situation when segments start with different timestamps
+        we only guarantee to work with ``start_timestamp`` >= beginning of all segments.
+
+        Parameters
+        ----------
+        ts:
+            Dataset to make predictions on.
+        start_timestamp:
+            First timestamp of prediction range to return, should be >= than first timestamp in ``ts``;
+            expected that beginning of each segment <= ``start_timestamp``;
+            if isn't set the first timestamp where each segment began is taken.
+        end_timestamp:
+            Last timestamp of prediction range to return; if isn't set the last timestamp of ``ts`` is taken.
+            Expected that value is less or equal to the last timestamp in ``ts``.
+        prediction_interval:
+            If True returns prediction interval for forecast.
+        quantiles:
+            Levels of prediction distribution. By default 2.5% and 97.5% taken to form a 95% prediction interval.
+        return_components:
+            If True additionally returns forecast components
+
+        Returns
+        -------
+        :
+            Dataset with predictions in ``[start_timestamp, end_timestamp]`` range.
+
+        Raises
+        ------
+        ValueError:
+            Value of ``end_timestamp`` is less than ``start_timestamp``.
+        ValueError:
+            Value of ``start_timestamp`` goes before point where each segment started.
+        ValueError:
+            Value of ``end_timestamp`` goes after the last timestamp.
+        """
+
+    @abstractmethod
     def backtest(
         self,
         ts: TSDataset,
         metrics: List[Metric],
         n_folds: Union[int, List[FoldMask]] = 5,
-        mode: str = "expand",
+        mode: Optional[str] = None,
         aggregate_metrics: bool = False,
         n_jobs: int = 1,
+        refit: Union[bool, int] = True,
+        stride: Optional[int] = None,
         joblib_params: Optional[Dict[str, Any]] = None,
         forecast_params: Optional[Dict[str, Any]] = None,
     ) -> Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]:
         """Run backtest with the pipeline.
 
+        If ``refit != True`` and some component of the pipeline doesn't support forecasting with gap, this component will raise an exception.
+
         Parameters
         ----------
         ts:
             Dataset to fit models in backtest
         metrics:
             List of metrics to compute for each fold
         n_folds:
             Number of folds or the list of fold masks
         mode:
-            One of 'expand', 'constant' -- train generation policy
+            Train generation policy: 'expand' or 'constant'. Works only if ``n_folds`` is integer.
+            By default, is set to 'expand'.
         aggregate_metrics:
             If True aggregate metrics above folds, return raw metrics otherwise
         n_jobs:
             Number of jobs to run in parallel
+        refit:
+            Determines how often pipeline should be retrained during iteration over folds.
+
+            * If ``True``: pipeline is retrained on each fold.
+
+            * If ``False``: pipeline is trained only on the first fold.
+
+            * If ``value: int``: pipeline is trained every ``value`` folds starting from the first.
+
+        stride:
+            Number of points between folds. Works only if ``n_folds`` is integer. By default, is set to ``horizon``.
         joblib_params:
             Additional parameters for :py:class:`joblib.Parallel`
         forecast_params:
             Additional parameters for :py:func:`~etna.pipeline.base.BasePipeline.forecast`
 
         Returns
         -------
         metrics_df, forecast_df, fold_info_df: Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]
             Metrics dataframe, forecast dataframe and dataframe with information about folds
         """
 
 
+class FoldParallelGroup(TypedDict):
+    """Group for parallel fold processing."""
+
+    train_fold_number: int
+    train_mask: FoldMask
+    forecast_fold_numbers: List[int]
+    forecast_masks: List[FoldMask]
+
+
 class BasePipeline(AbstractPipeline, BaseMixin):
     """Base class for pipeline."""
 
     def __init__(self, horizon: int):
         self._validate_horizon(horizon=horizon)
         self.horizon = horizon
         self.ts: Optional[TSDataset] = None
@@ -210,120 +302,264 @@
         """Check that given number of folds is grater than 1."""
         for quantile in quantiles:
             if not (0 < quantile < 1):
                 raise ValueError("Quantile should be a number from (0,1).")
         return quantiles
 
     @abstractmethod
-    def _forecast(self) -> TSDataset:
+    def _forecast(self, ts: TSDataset, return_components: bool) -> TSDataset:
         """Make predictions."""
         pass
 
     def _forecast_prediction_interval(
-        self, predictions: TSDataset, quantiles: Sequence[float], n_folds: int
+        self, ts: TSDataset, predictions: TSDataset, quantiles: Sequence[float], n_folds: int
     ) -> TSDataset:
         """Add prediction intervals to the forecasts."""
-        if self.ts is None:
-            raise ValueError("Pipeline is not fitted! Fit the Pipeline before calling forecast method.")
-        _, forecasts, _ = self.backtest(ts=self.ts, metrics=[MAE()], n_folds=n_folds)
-        forecasts = TSDataset(df=forecasts, freq=self.ts.freq)
+        with tslogger.disable():
+            _, forecasts, _ = self.backtest(ts=ts, metrics=[MAE()], n_folds=n_folds)
+
+        self._add_forecast_borders(ts=ts, backtest_forecasts=forecasts, quantiles=quantiles, predictions=predictions)
+
+        return predictions
+
+    def _add_forecast_borders(
+        self, ts: TSDataset, backtest_forecasts: pd.DataFrame, quantiles: Sequence[float], predictions: TSDataset
+    ) -> None:
+        """Estimate prediction intervals and add to the forecasts."""
+        backtest_forecasts = TSDataset(df=backtest_forecasts, freq=ts.freq)
         residuals = (
-            forecasts.loc[:, pd.IndexSlice[:, "target"]]
-            - self.ts[forecasts.index.min() : forecasts.index.max(), :, "target"]
+            backtest_forecasts.loc[:, pd.IndexSlice[:, "target"]]
+            - ts[backtest_forecasts.index.min() : backtest_forecasts.index.max(), :, "target"]
         )
 
-        se = scipy.stats.sem(residuals)
+        sigma = np.std(residuals.values, axis=0)
         borders = []
         for quantile in quantiles:
             z_q = norm.ppf(q=quantile)
-            border = predictions[:, :, "target"] + se * z_q
+            border = predictions[:, :, "target"] + sigma * z_q
             border.rename({"target": f"target_{quantile:.4g}"}, inplace=True, axis=1)
             borders.append(border)
 
         predictions.df = pd.concat([predictions.df] + borders, axis=1).sort_index(axis=1, level=(0, 1))
 
-        return predictions
-
     def forecast(
-        self, prediction_interval: bool = False, quantiles: Sequence[float] = (0.025, 0.975), n_folds: int = 3
+        self,
+        ts: Optional[TSDataset] = None,
+        prediction_interval: bool = False,
+        quantiles: Sequence[float] = (0.025, 0.975),
+        n_folds: int = 3,
+        return_components: bool = False,
     ) -> TSDataset:
-        """Make predictions.
+        """Make a forecast of the next points of a dataset.
+
+        The result of forecasting starts from the last point of ``ts``, not including it.
 
         Parameters
         ----------
+        ts:
+            Dataset to forecast. If not given, dataset given during :py:meth:``fit`` is used.
         prediction_interval:
             If True returns prediction interval for forecast
         quantiles:
             Levels of prediction distribution. By default 2.5% and 97.5% taken to form a 95% prediction interval
         n_folds:
             Number of folds to use in the backtest for prediction interval estimation
+        return_components:
+            If True additionally returns forecast components
 
         Returns
         -------
         :
             Dataset with predictions
+
+        Raises
+        ------
+        NotImplementedError:
+            Adding target components is not currently implemented
         """
-        if self.ts is None:
-            raise ValueError(
-                f"{self.__class__.__name__} is not fitted! Fit the {self.__class__.__name__} "
-                f"before calling forecast method."
-            )
+        if ts is None:
+            if self.ts is None:
+                raise ValueError(
+                    "There is no ts to forecast! Pass ts into forecast method or make sure that pipeline is loaded with ts."
+                )
+            ts = self.ts
+
         self._validate_quantiles(quantiles=quantiles)
         self._validate_backtest_n_folds(n_folds=n_folds)
 
-        predictions = self._forecast()
+        predictions = self._forecast(ts=ts, return_components=return_components)
         if prediction_interval:
             predictions = self._forecast_prediction_interval(
-                predictions=predictions, quantiles=quantiles, n_folds=n_folds
+                ts=ts, predictions=predictions, quantiles=quantiles, n_folds=n_folds
             )
         return predictions
 
+    @staticmethod
+    def _make_predict_timestamps(
+        ts: TSDataset,
+        start_timestamp: Optional[pd.Timestamp] = None,
+        end_timestamp: Optional[pd.Timestamp] = None,
+    ) -> Tuple[pd.Timestamp, pd.Timestamp]:
+        min_timestamp = ts.describe()["start_timestamp"].max()
+        max_timestamp = ts.index[-1]
+
+        if start_timestamp is None:
+            start_timestamp = min_timestamp
+        if end_timestamp is None:
+            end_timestamp = max_timestamp
+
+        if start_timestamp < min_timestamp:
+            raise ValueError("Value of start_timestamp is less than beginning of some segments!")
+        if end_timestamp > max_timestamp:
+            raise ValueError("Value of end_timestamp is more than ending of dataset!")
+
+        if start_timestamp > end_timestamp:
+            raise ValueError("Value of end_timestamp is less than start_timestamp!")
+
+        return start_timestamp, end_timestamp
+
+    @abstractmethod
+    def _predict(
+        self,
+        ts: TSDataset,
+        start_timestamp: Optional[pd.Timestamp],
+        end_timestamp: Optional[pd.Timestamp],
+        prediction_interval: bool,
+        quantiles: Sequence[float],
+        return_components: bool,
+    ) -> TSDataset:
+        pass
+
+    def predict(
+        self,
+        ts: TSDataset,
+        start_timestamp: Optional[pd.Timestamp] = None,
+        end_timestamp: Optional[pd.Timestamp] = None,
+        prediction_interval: bool = False,
+        quantiles: Sequence[float] = (0.025, 0.975),
+        return_components: bool = False,
+    ) -> TSDataset:
+        """Make in-sample predictions on dataset in a given range.
+
+        Currently, in situation when segments start with different timestamps
+        we only guarantee to work with ``start_timestamp`` >= beginning of all segments.
+
+        Parameters
+        ----------
+        ts:
+            Dataset to make predictions on.
+        start_timestamp:
+            First timestamp of prediction range to return, should be >= than first timestamp in ``ts``;
+            expected that beginning of each segment <= ``start_timestamp``;
+            if isn't set the first timestamp where each segment began is taken.
+        end_timestamp:
+            Last timestamp of prediction range to return; if isn't set the last timestamp of ``ts`` is taken.
+            Expected that value is less or equal to the last timestamp in ``ts``.
+        prediction_interval:
+            If True returns prediction interval for forecast.
+        quantiles:
+            Levels of prediction distribution. By default 2.5% and 97.5% taken to form a 95% prediction interval.
+        return_components:
+            If True additionally returns forecast components
+
+        Returns
+        -------
+        :
+            Dataset with predictions in ``[start_timestamp, end_timestamp]`` range.
+
+        Raises
+        ------
+        ValueError:
+            Value of ``end_timestamp`` is less than ``start_timestamp``.
+        ValueError:
+            Value of ``start_timestamp`` goes before point where each segment started.
+        ValueError:
+            Value of ``end_timestamp`` goes after the last timestamp.
+        NotImplementedError:
+            Adding target components is not currently implemented
+        """
+        start_timestamp, end_timestamp = self._make_predict_timestamps(
+            ts=ts, start_timestamp=start_timestamp, end_timestamp=end_timestamp
+        )
+        self._validate_quantiles(quantiles=quantiles)
+        result = self._predict(
+            ts=ts,
+            start_timestamp=start_timestamp,
+            end_timestamp=end_timestamp,
+            prediction_interval=prediction_interval,
+            quantiles=quantiles,
+            return_components=return_components,
+        )
+        return result
+
     def _init_backtest(self):
         self._folds: Optional[Dict[int, Any]] = None
         self._fold_column = "fold_number"
 
     @staticmethod
     def _validate_backtest_n_folds(n_folds: int):
-        """Check that given n_folds value is valid."""
+        """Check that given n_folds value is >= 1."""
         if n_folds < 1:
             raise ValueError(f"Folds number should be a positive number, {n_folds} given")
 
     @staticmethod
-    def _validate_backtest_dataset(ts: TSDataset, n_folds: int, horizon: int):
+    def _validate_backtest_mode(n_folds: Union[int, List[FoldMask]], mode: Optional[str]) -> CrossValidationMode:
+        if mode is None:
+            return CrossValidationMode.expand
+
+        if not isinstance(n_folds, int):
+            raise ValueError("Mode shouldn't be set if n_folds are fold masks!")
+
+        return CrossValidationMode(mode.lower())
+
+    @staticmethod
+    def _validate_backtest_stride(n_folds: Union[int, List[FoldMask]], horizon: int, stride: Optional[int]) -> int:
+        if stride is None:
+            return horizon
+
+        if not isinstance(n_folds, int):
+            raise ValueError("Stride shouldn't be set if n_folds are fold masks!")
+
+        if stride < 1:
+            raise ValueError(f"Stride should be a positive number, {stride} given!")
+
+        return stride
+
+    @staticmethod
+    def _validate_backtest_dataset(ts: TSDataset, n_folds: int, horizon: int, stride: int):
         """Check all segments have enough timestamps to validate forecaster with given number of splits."""
-        min_required_length = horizon * n_folds
+        min_required_length = horizon + (n_folds - 1) * stride
         segments = set(ts.df.columns.get_level_values("segment"))
         for segment in segments:
             segment_target = ts[:, segment, "target"]
             if len(segment_target) < min_required_length:
                 raise ValueError(
                     f"All the series from feature dataframe should contain at least "
-                    f"{horizon} * {n_folds} = {min_required_length} timestamps; "
+                    f"{horizon} + {n_folds-1} * {stride} = {min_required_length} timestamps; "
                     f"series {segment} does not."
                 )
 
     @staticmethod
-    def _generate_masks_from_n_folds(ts: TSDataset, n_folds: int, horizon: int, mode: str) -> List[FoldMask]:
+    def _generate_masks_from_n_folds(
+        ts: TSDataset, n_folds: int, horizon: int, mode: CrossValidationMode, stride: int
+    ) -> List[FoldMask]:
         """Generate fold masks from n_folds."""
-        mode_enum = CrossValidationMode(mode.lower())
-        if mode_enum == CrossValidationMode.expand:
+        if mode is CrossValidationMode.expand:
             constant_history_length = 0
-        elif mode_enum == CrossValidationMode.constant:
+        elif mode is CrossValidationMode.constant:
             constant_history_length = 1
         else:
-            raise NotImplementedError(
-                f"Only '{CrossValidationMode.expand}' and '{CrossValidationMode.constant}' modes allowed"
-            )
+            assert_never(mode)
 
         masks = []
         dataset_timestamps = list(ts.index)
         min_timestamp_idx, max_timestamp_idx = 0, len(dataset_timestamps)
         for offset in range(n_folds, 0, -1):
-            min_train_idx = min_timestamp_idx + (n_folds - offset) * horizon * constant_history_length
-            max_train_idx = max_timestamp_idx - horizon * offset - 1
+            min_train_idx = min_timestamp_idx + (n_folds - offset) * stride * constant_history_length
+            max_train_idx = max_timestamp_idx - stride * (offset - 1) - horizon - 1
             min_test_idx = max_train_idx + 1
             max_test_idx = max_train_idx + horizon
 
             min_train, max_train = dataset_timestamps[min_train_idx], dataset_timestamps[max_train_idx]
             min_test, max_test = dataset_timestamps[min_test_idx], dataset_timestamps[max_test_idx]
 
             mask = FoldMask(
@@ -363,84 +599,105 @@
             min_test, max_test = timestamps[min_test_idx], timestamps[max_test_idx]
 
             train, test = ts.train_test_split(
                 train_start=min_train, train_end=max_train, test_start=min_test, test_end=max_test
             )
             yield train, test
 
-    @staticmethod
-    def _compute_metrics(metrics: List[Metric], y_true: TSDataset, y_pred: TSDataset) -> Dict[str, Dict[str, float]]:
+    def _compute_metrics(
+        self, metrics: List[Metric], y_true: TSDataset, y_pred: TSDataset
+    ) -> Dict[str, Dict[str, float]]:
         """Compute metrics for given y_true, y_pred."""
         metrics_values: Dict[str, Dict[str, float]] = {}
         for metric in metrics:
             metrics_values[metric.name] = metric(y_true=y_true, y_pred=y_pred)  # type: ignore
         return metrics_values
 
-    def _run_fold(
+    def _fit_backtest_pipeline(
+        self,
+        ts: TSDataset,
+        fold_number: int,
+    ) -> "BasePipeline":
+        """Fit pipeline for a given data in backtest."""
+        tslogger.start_experiment(job_type="training", group=str(fold_number))
+        pipeline = deepcopy(self)
+        pipeline.fit(ts=ts)
+        tslogger.finish_experiment()
+        return pipeline
+
+    def _forecast_backtest_pipeline(
+        self, pipeline: "BasePipeline", ts: TSDataset, fold_number: int, forecast_params: Dict[str, Any]
+    ) -> TSDataset:
+        """Make a forecast with a given pipeline in backtest."""
+        tslogger.start_experiment(job_type="forecasting", group=str(fold_number))
+        forecast = pipeline.forecast(ts=ts, **forecast_params)
+        tslogger.finish_experiment()
+        return forecast
+
+    def _process_fold_forecast(
         self,
+        forecast: TSDataset,
         train: TSDataset,
         test: TSDataset,
+        pipeline: "BasePipeline",
         fold_number: int,
         mask: FoldMask,
         metrics: List[Metric],
-        forecast_params: Dict[str, Any],
     ) -> Dict[str, Any]:
-        """Run fit-forecast pipeline of model for one fold."""
+        """Process forecast made for a fold."""
         tslogger.start_experiment(job_type="crossval", group=str(fold_number))
 
-        pipeline = deepcopy(self)
-        pipeline.fit(ts=train)
-        forecast = pipeline.forecast(**forecast_params)
         fold: Dict[str, Any] = {}
         for stage_name, stage_df in zip(("train", "test"), (train, test)):
             fold[f"{stage_name}_timerange"] = {}
             fold[f"{stage_name}_timerange"]["start"] = stage_df.index.min()
             fold[f"{stage_name}_timerange"]["end"] = stage_df.index.max()
 
         forecast.df = forecast.df.loc[mask.target_timestamps]
         test.df = test.df.loc[mask.target_timestamps]
 
         fold["forecast"] = forecast
-        fold["metrics"] = deepcopy(self._compute_metrics(metrics=metrics, y_true=test, y_pred=forecast))
+        fold["metrics"] = deepcopy(pipeline._compute_metrics(metrics=metrics, y_true=test, y_pred=forecast))
 
         tslogger.log_backtest_run(pd.DataFrame(fold["metrics"]), forecast.to_pandas(), test.to_pandas())
         tslogger.finish_experiment()
 
         return fold
 
     def _get_backtest_metrics(self, aggregate_metrics: bool = False) -> pd.DataFrame:
         """Get dataframe with metrics."""
         if self._folds is None:
             raise ValueError("Something went wrong during backtest initialization!")
-        metrics_df = pd.DataFrame()
+        metrics_dfs = []
 
         for i, fold in self._folds.items():
             fold_metrics = pd.DataFrame(fold["metrics"]).reset_index().rename({"index": "segment"}, axis=1)
             fold_metrics[self._fold_column] = i
-            metrics_df = metrics_df.append(fold_metrics)
-
+            metrics_dfs.append(fold_metrics)
+        metrics_df = pd.concat(metrics_dfs)
         metrics_df.sort_values(["segment", self._fold_column], inplace=True)
 
         if aggregate_metrics:
             metrics_df = metrics_df.groupby("segment").mean().reset_index().drop(self._fold_column, axis=1)
 
         return metrics_df
 
     def _get_fold_info(self) -> pd.DataFrame:
         """Get information about folds."""
         if self._folds is None:
             raise ValueError("Something went wrong during backtest initialization!")
-        timerange_df = pd.DataFrame()
+        timerange_dfs = []
         for fold_number, fold_info in self._folds.items():
             tmp_df = pd.DataFrame()
             for stage_name in ("train", "test"):
                 for border in ("start", "end"):
                     tmp_df[f"{stage_name}_{border}_time"] = [fold_info[f"{stage_name}_timerange"][border]]
             tmp_df[self._fold_column] = fold_number
-            timerange_df = timerange_df.append(tmp_df)
+            timerange_dfs.append(tmp_df)
+        timerange_df = pd.concat(timerange_dfs, ignore_index=True)
         return timerange_df
 
     def _get_backtest_forecasts(self) -> pd.DataFrame:
         """Get forecasts from different folds."""
         if self._folds is None:
             raise ValueError("Something went wrong during backtest initialization!")
         forecasts_list = []
@@ -452,90 +709,218 @@
                 np.tile(fold_number, (forecast.index.shape[0], len(segments))),
                 columns=pd.MultiIndex.from_product([segments, [self._fold_column]], names=("segment", "feature")),
                 index=forecast.index,
             )
             forecast = forecast.join(fold_number_df)
             forecasts_list.append(forecast)
         forecasts = pd.concat(forecasts_list)
+        forecasts.sort_index(axis=1, inplace=True)
         return forecasts
 
-    def _prepare_fold_masks(self, ts: TSDataset, masks: Union[int, List[FoldMask]], mode: str) -> List[FoldMask]:
+    def _prepare_fold_masks(
+        self, ts: TSDataset, masks: Union[int, List[FoldMask]], mode: CrossValidationMode, stride: int
+    ) -> List[FoldMask]:
         """Prepare and validate fold masks."""
         if isinstance(masks, int):
             self._validate_backtest_n_folds(n_folds=masks)
-            self._validate_backtest_dataset(ts=ts, n_folds=masks, horizon=self.horizon)
-            masks = self._generate_masks_from_n_folds(ts=ts, n_folds=masks, horizon=self.horizon, mode=mode)
+            self._validate_backtest_dataset(ts=ts, n_folds=masks, horizon=self.horizon, stride=stride)
+            masks = self._generate_masks_from_n_folds(
+                ts=ts, n_folds=masks, horizon=self.horizon, mode=mode, stride=stride
+            )
         for i, mask in enumerate(masks):
             mask.first_train_timestamp = mask.first_train_timestamp if mask.first_train_timestamp else ts.index[0]
             masks[i] = mask
         for mask in masks:
             mask.validate_on_dataset(ts=ts, horizon=self.horizon)
         return masks
 
+    @staticmethod
+    def _make_backtest_fold_groups(masks: List[FoldMask], refit: Union[bool, int]) -> List[FoldParallelGroup]:
+        """Make groups of folds for backtest."""
+        if not refit:
+            refit = len(masks)
+
+        grouped_folds = []
+        num_groups = math.ceil(len(masks) / refit)
+        for group_id in range(num_groups):
+            train_fold_number = group_id * refit
+            forecast_fold_numbers = [train_fold_number + i for i in range(refit) if train_fold_number + i < len(masks)]
+            cur_group: FoldParallelGroup = {
+                "train_fold_number": train_fold_number,
+                "train_mask": masks[train_fold_number],
+                "forecast_fold_numbers": forecast_fold_numbers,
+                "forecast_masks": [masks[i] for i in forecast_fold_numbers],
+            }
+            grouped_folds.append(cur_group)
+
+        return grouped_folds
+
+    def _run_all_folds(
+        self,
+        masks: List[FoldMask],
+        ts: TSDataset,
+        metrics: List[Metric],
+        n_jobs: int,
+        refit: Union[bool, int],
+        joblib_params: Dict[str, Any],
+        forecast_params: Dict[str, Any],
+    ) -> Dict[int, Any]:
+        """Run pipeline on all folds."""
+        fold_groups = self._make_backtest_fold_groups(masks=masks, refit=refit)
+
+        with Parallel(n_jobs=n_jobs, **joblib_params) as parallel:
+            # fitting
+            fit_masks = [group["train_mask"] for group in fold_groups]
+            fit_datasets = (
+                train for train, _ in self._generate_folds_datasets(ts=ts, masks=fit_masks, horizon=self.horizon)
+            )
+            pipelines = parallel(
+                delayed(self._fit_backtest_pipeline)(ts=fit_ts, fold_number=fold_groups[group_idx]["train_fold_number"])
+                for group_idx, fit_ts in enumerate(fit_datasets)
+            )
+
+            # forecasting
+            forecast_masks = [group["forecast_masks"] for group in fold_groups]
+            forecast_datasets = (
+                (
+                    train
+                    for train, _ in self._generate_folds_datasets(
+                        ts=ts, masks=group_forecast_masks, horizon=self.horizon
+                    )
+                )
+                for group_forecast_masks in forecast_masks
+            )
+            forecasts_flat = parallel(
+                delayed(self._forecast_backtest_pipeline)(
+                    ts=forecast_ts,
+                    pipeline=pipelines[group_idx],
+                    fold_number=fold_groups[group_idx]["forecast_fold_numbers"][idx],
+                    forecast_params=forecast_params,
+                )
+                for group_idx, group_forecast_datasets in enumerate(forecast_datasets)
+                for idx, forecast_ts in enumerate(group_forecast_datasets)
+            )
+
+            # processing forecasts
+            fold_process_train_datasets = (
+                train for train, _ in self._generate_folds_datasets(ts=ts, masks=fit_masks, horizon=self.horizon)
+            )
+            fold_process_test_datasets = (
+                (
+                    test
+                    for _, test in self._generate_folds_datasets(
+                        ts=ts, masks=group_forecast_masks, horizon=self.horizon
+                    )
+                )
+                for group_forecast_masks in forecast_masks
+            )
+            fold_results_flat = parallel(
+                delayed(self._process_fold_forecast)(
+                    forecast=forecasts_flat[group_idx * refit + idx],
+                    train=train,
+                    test=test,
+                    pipeline=pipelines[group_idx],
+                    fold_number=fold_groups[group_idx]["forecast_fold_numbers"][idx],
+                    mask=fold_groups[group_idx]["forecast_masks"][idx],
+                    metrics=metrics,
+                )
+                for group_idx, (train, group_fold_process_test_datasets) in enumerate(
+                    zip(fold_process_train_datasets, fold_process_test_datasets)
+                )
+                for idx, test in enumerate(group_fold_process_test_datasets)
+            )
+
+        results = {
+            fold_number: fold_results_flat[group_idx * refit + idx]
+            for group_idx in range(len(fold_groups))
+            for idx, fold_number in enumerate(fold_groups[group_idx]["forecast_fold_numbers"])
+        }
+        return results
+
     def backtest(
         self,
         ts: TSDataset,
         metrics: List[Metric],
         n_folds: Union[int, List[FoldMask]] = 5,
-        mode: str = "expand",
+        mode: Optional[str] = None,
         aggregate_metrics: bool = False,
         n_jobs: int = 1,
+        refit: Union[bool, int] = True,
+        stride: Optional[int] = None,
         joblib_params: Optional[Dict[str, Any]] = None,
         forecast_params: Optional[Dict[str, Any]] = None,
     ) -> Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]:
         """Run backtest with the pipeline.
 
+        If ``refit != True`` and some component of the pipeline doesn't support forecasting with gap, this component will raise an exception.
+
         Parameters
         ----------
         ts:
             Dataset to fit models in backtest
         metrics:
             List of metrics to compute for each fold
         n_folds:
             Number of folds or the list of fold masks
         mode:
-            One of 'expand', 'constant' -- train generation policy, ignored if n_folds is a list of masks
+            Train generation policy: 'expand' or 'constant'. Works only if ``n_folds`` is integer.
+            By default, is set to 'expand'.
         aggregate_metrics:
             If True aggregate metrics above folds, return raw metrics otherwise
         n_jobs:
             Number of jobs to run in parallel
+        refit:
+            Determines how often pipeline should be retrained during iteration over folds.
+
+            * If ``True``: pipeline is retrained on each fold.
+
+            * If ``False``: pipeline is trained only on the first fold.
+
+            * If ``value: int``: pipeline is trained every ``value`` folds starting from the first.
+
+        stride:
+            Number of points between folds. Works only if ``n_folds`` is integer. By default, is set to ``horizon``.
         joblib_params:
             Additional parameters for :py:class:`joblib.Parallel`
         forecast_params:
             Additional parameters for :py:func:`~etna.pipeline.base.BasePipeline.forecast`
 
         Returns
         -------
         metrics_df, forecast_df, fold_info_df: Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]
             Metrics dataframe, forecast dataframe and dataframe with information about folds
+
+        Raises
+        ------
+        ValueError:
+            If ``mode`` is set when ``n_folds`` are ``List[FoldMask]``.
+        ValueError:
+            If ``stride`` is set when ``n_folds`` are ``List[FoldMask]``.
         """
+        mode_enum = self._validate_backtest_mode(n_folds=n_folds, mode=mode)
+        stride = self._validate_backtest_stride(n_folds=n_folds, horizon=self.horizon, stride=stride)
+
         if joblib_params is None:
             joblib_params = dict(verbose=11, backend="multiprocessing", mmap_mode="c")
 
         if forecast_params is None:
             forecast_params = dict()
 
         self._init_backtest()
         self._validate_backtest_metrics(metrics=metrics)
-        masks = self._prepare_fold_masks(ts=ts, masks=n_folds, mode=mode)
-
-        folds = Parallel(n_jobs=n_jobs, **joblib_params)(
-            delayed(self._run_fold)(
-                train=train,
-                test=test,
-                fold_number=fold_number,
-                mask=masks[fold_number],
-                metrics=metrics,
-                forecast_params=forecast_params,
-            )
-            for fold_number, (train, test) in enumerate(
-                self._generate_folds_datasets(ts=ts, masks=masks, horizon=self.horizon)
-            )
+        masks = self._prepare_fold_masks(ts=ts, masks=n_folds, mode=mode_enum, stride=stride)
+        self._folds = self._run_all_folds(
+            masks=masks,
+            ts=ts,
+            metrics=metrics,
+            n_jobs=n_jobs,
+            refit=refit,
+            joblib_params=joblib_params,
+            forecast_params=forecast_params,
         )
-        self._folds = {i: fold for i, fold in enumerate(folds)}
 
         metrics_df = self._get_backtest_metrics(aggregate_metrics=aggregate_metrics)
         forecast_df = self._get_backtest_forecasts()
         fold_info_df = self._get_fold_info()
 
         tslogger.start_experiment(job_type="crossval_results", group="all")
         tslogger.log_backtest_metrics(ts, metrics_df, forecast_df, fold_info_df)
```

### Comparing `etna-1.9.0/etna/settings.py` & `etna-2.0.0/etna/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,24 @@
     if _module_available("prophet"):
         return True
     else:
         warnings.warn("etna[prophet] is not available, to install it, run `pip install etna[prophet]`")
         return False
 
 
+def _is_tsfresh_available():
+    if _module_available("tsfresh"):
+        return True
+    else:
+        warnings.warn(
+            "`tsfresh` is not available, to install it, run `pip install tsfresh==0.19.0 && pip install protobuf==3.20.1`"
+        )
+        return False
+
+
 def _get_optional_value(is_required: Optional[bool], is_available_fn: Callable, assert_msg: str) -> bool:
     if is_required is None:
         return is_available_fn()
     elif is_required:
         if not is_available_fn():
             raise ImportError(assert_msg)
         return True
@@ -69,14 +79,15 @@
     """etna settings."""
 
     def __init__(  # noqa: D107
         self,
         torch_required: Optional[bool] = None,
         prophet_required: Optional[bool] = None,
         wandb_required: Optional[bool] = None,
+        tsfresh_required: Optional[bool] = None,
     ):
         # True – use the package
         # None – use the package if available
         # False - block the package
         self.torch_required: bool = _get_optional_value(
             torch_required,
             _is_torch_available,
@@ -86,14 +97,19 @@
             wandb_required, _is_wandb_available, "wandb is not available, to install it, " "run `pip install wandb`."
         )
         self.prophet_required: bool = _get_optional_value(
             prophet_required,
             _is_prophet_available,
             "etna[prophet] is not available, to install it, run `pip install etna[prophet]`.",
         )
+        self.tsfresh_required: bool = _get_optional_value(
+            tsfresh_required,
+            _is_tsfresh_available,
+            "`tsfresh` is not available, to install it, run `pip install tsfresh==0.19.0 && pip install protobuf==3.20.1`",
+        )
 
     @staticmethod
     def parse() -> "Settings":
         """Parse and return the settings.
 
         Returns
         -------
```

### Comparing `etna-1.9.0/etna/transforms/__init__.py` & `etna-2.0.0/etna/transforms/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+from etna.transforms.base import IrreversiblePerSegmentWrapper
+from etna.transforms.base import IrreversibleTransform
+from etna.transforms.base import OneSegmentTransform
 from etna.transforms.base import PerSegmentWrapper
+from etna.transforms.base import ReversiblePerSegmentWrapper
+from etna.transforms.base import ReversibleTransform
 from etna.transforms.base import Transform
-from etna.transforms.decomposition import BinsegTrendTransform
+from etna.transforms.decomposition import BaseChangePointsTransform
+from etna.transforms.decomposition import ChangePointsLevelTransform
+from etna.transforms.decomposition import ChangePointsSegmentationTransform
 from etna.transforms.decomposition import ChangePointsTrendTransform
+from etna.transforms.decomposition import IrreversibleChangePointsTransform
 from etna.transforms.decomposition import LinearTrendTransform
+from etna.transforms.decomposition import ReversibleChangePointsTransform
 from etna.transforms.decomposition import STLTransform
 from etna.transforms.decomposition import TheilSenTrendTransform
 from etna.transforms.decomposition import TrendTransform
 from etna.transforms.encoders import LabelEncoderTransform
 from etna.transforms.encoders import MeanSegmentEncoderTransform
 from etna.transforms.encoders import OneHotEncoderTransform
 from etna.transforms.encoders import SegmentEncoderTransform
@@ -14,30 +23,32 @@
 from etna.transforms.feature_selection import GaleShapleyFeatureSelectionTransform
 from etna.transforms.feature_selection import MRMRFeatureSelectionTransform
 from etna.transforms.feature_selection import TreeFeatureSelectionTransform
 from etna.transforms.math import AddConstTransform
 from etna.transforms.math import BoxCoxTransform
 from etna.transforms.math import DifferencingTransform
 from etna.transforms.math import LagTransform
+from etna.transforms.math import LambdaTransform
 from etna.transforms.math import LogTransform
 from etna.transforms.math import MADTransform
 from etna.transforms.math import MaxAbsScalerTransform
 from etna.transforms.math import MaxTransform
 from etna.transforms.math import MeanTransform
 from etna.transforms.math import MedianTransform
+from etna.transforms.math import MinMaxDifferenceTransform
 from etna.transforms.math import MinMaxScalerTransform
 from etna.transforms.math import MinTransform
 from etna.transforms.math import QuantileTransform
 from etna.transforms.math import RobustScalerTransform
 from etna.transforms.math import StandardScalerTransform
 from etna.transforms.math import StdTransform
+from etna.transforms.math import SumTransform
 from etna.transforms.math import YeoJohnsonTransform
 from etna.transforms.missing_values import ResampleWithDistributionTransform
 from etna.transforms.missing_values import TimeSeriesImputerTransform
-from etna.transforms.nn import PytorchForecastingTransform
 from etna.transforms.outliers import DensityOutliersTransform
 from etna.transforms.outliers import MedianOutliersTransform
 from etna.transforms.outliers import PredictionIntervalOutliersTransform
 from etna.transforms.timestamp import DateFlagsTransform
 from etna.transforms.timestamp import FourierTransform
 from etna.transforms.timestamp import HolidayTransform
 from etna.transforms.timestamp import SpecialDaysTransform
```

### Comparing `etna-1.9.0/etna/transforms/decomposition/change_points_trend.py` & `etna-2.0.0/etna/transforms/decomposition/change_points_based/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,150 +1,185 @@
+from abc import ABC
+from abc import abstractmethod
 from copy import deepcopy
+from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
-from typing import Type
 
 import numpy as np
 import pandas as pd
-from ruptures.base import BaseEstimator
-from sklearn.base import RegressorMixin
 
-from etna.analysis.change_points_trend.search import _find_change_points_segment
-from etna.transforms.base import PerSegmentWrapper
-from etna.transforms.base import Transform
-from etna.transforms.utils import match_target_quantiles
+from etna.transforms.base import FutureMixin
+from etna.transforms.base import IrreversiblePerSegmentWrapper
+from etna.transforms.base import OneSegmentTransform
+from etna.transforms.base import ReversiblePerSegmentWrapper
+from etna.transforms.decomposition.change_points_based.change_points_models import BaseChangePointsModelAdapter
+from etna.transforms.decomposition.change_points_based.per_interval_models import PerIntervalModel
 
-TTimestampInterval = Tuple[pd.Timestamp, pd.Timestamp]
-TDetrendModel = Type[RegressorMixin]
-
-
-class _OneSegmentChangePointsTrendTransform(Transform):
-    """_OneSegmentChangePointsTransform subtracts multiple linear trend from series."""
 
+class _OneSegmentChangePointsTransform(OneSegmentTransform, ABC):
     def __init__(
-        self,
-        in_column: str,
-        change_point_model: BaseEstimator,
-        detrend_model: TDetrendModel,
-        **change_point_model_predict_params,
+        self, in_column: str, change_points_model: BaseChangePointsModelAdapter, per_interval_model: PerIntervalModel
     ):
-        """Init _OneSegmentChangePointsTrendTransform.
+        """Init _OneSegmentChangePointsTransform.
 
         Parameters
         ----------
         in_column:
-            name of column to apply transform to
-        change_point_model:
-            model to get trend change points
-        detrend_model:
-            model to get trend in data
-        change_point_model_predict_params:
-            params for ``change_point_model.predict`` method
+            name of column to apple transform to
+        change_points_model:
+            model to get change points from data
+        per_interval_model:
+            model to process intervals between change points
         """
         self.in_column = in_column
-        self.out_columns = in_column
-        self.change_point_model = change_point_model
-        self.detrend_model = detrend_model
-        self.per_interval_models: Optional[Dict[TTimestampInterval, TDetrendModel]] = None
-        self.intervals: Optional[List[TTimestampInterval]] = None
-        self.change_point_model_predict_params = change_point_model_predict_params
+        self.change_points_model = change_points_model
+        self.per_interval_model = per_interval_model
+        self.per_interval_models: Optional[Dict[Any, PerIntervalModel]] = None
+        self.intervals: Optional[List[Tuple[Any, Any]]] = None
+
+    def _init_per_interval_models(self, intervals: List[Tuple[Any, Any]]) -> Dict[Tuple[Any, Any], PerIntervalModel]:
+        """Multiply per interval model for given intervals."""
+        per_interval_models = {interval: deepcopy(self.per_interval_model) for interval in intervals}
+        return per_interval_models
 
     @staticmethod
-    def _build_trend_intervals(change_points: List[pd.Timestamp]) -> List[TTimestampInterval]:
-        """Create list of stable trend intervals from list of change points."""
-        change_points = sorted(change_points)
-        left_border = pd.Timestamp.min
-        intervals = []
-        for point in change_points:
-            right_border = point
-            intervals.append((left_border, right_border))
-            left_border = right_border
-        intervals.append((left_border, pd.Timestamp.max))
-        return intervals
-
-    def _init_detrend_models(
-        self, intervals: List[TTimestampInterval]
-    ) -> Dict[Tuple[pd.Timestamp, pd.Timestamp], TDetrendModel]:
-        """Create copy of detrend model for each timestamp interval."""
-        per_interval_models = {interval: deepcopy(self.detrend_model) for interval in intervals}
-        return per_interval_models
+    def _get_features(series: pd.Series) -> np.ndarray:
+        """Prepare features to train per interval model.
+
+        Parameters
+        ----------
+        series:
+            series to get features from
 
-    def _get_timestamps(self, series: pd.Series) -> np.ndarray:
-        """Convert ETNA timestamp-index to a list of timestamps to fit regression models."""
-        timestamps = series.index
-        timestamps = np.array([[ts.timestamp()] for ts in timestamps])
-        return timestamps
+        Returns
+        -------
+        features:
+            array with prepared features
+        """
+        features = series.index.values.reshape((-1, 1))
+        return features
 
-    def _fit_per_interval_model(self, series: pd.Series):
+    @staticmethod
+    def _get_targets(series: pd.Series) -> np.ndarray:
+        """Get targets from given series to train per interval model.
+
+        Parameters
+        ----------
+        series:
+            series to get targets from
+
+        Returns
+        -------
+        targets:
+            array with targets
+        """
+        return series.values
+
+    def _fit_per_interval_models(self, series: pd.Series):
         """Fit per-interval models with corresponding data from series."""
         if self.intervals is None or self.per_interval_models is None:
             raise ValueError("Something went wrong on fit! Check the parameters of the transform.")
         for interval in self.intervals:
             tmp_series = series[interval[0] : interval[1]]
-            x = self._get_timestamps(series=tmp_series)
-            y = tmp_series.values
-            self.per_interval_models[interval].fit(x, y)
+            features = self._get_features(series=tmp_series)
+            targets = self._get_targets(series=tmp_series)
+            self.per_interval_models[interval].fit(features=features, target=targets)
+
+    def fit(self, df: pd.DataFrame) -> "_OneSegmentChangePointsTransform":
+        """Fit transform.
+        Get no-changepoints intervals with change_points_model and fit per_interval_model on the intervals.
+
+        Parameters
+        ----------
+        df:
+            dataframe to process
+
+        Returns
+        -------
+        self:
+            fitted _OneSegmentChangePointsTransform
+        """
+        self.intervals = self.change_points_model.get_change_points_intervals(df=df, in_column=self.in_column)
+        self.per_interval_models = self._init_per_interval_models(intervals=self.intervals)
+
+        series = df.loc[df[self.in_column].first_valid_index() : df[self.in_column].last_valid_index(), self.in_column]
+        self._fit_per_interval_models(series=series)
+        return self
 
     def _predict_per_interval_model(self, series: pd.Series) -> pd.Series:
         """Apply per-interval detrending to series."""
         if self.intervals is None or self.per_interval_models is None:
             raise ValueError("Transform is not fitted! Fit the Transform before calling transform method.")
-        trend_series = pd.Series(index=series.index)
+        prediction_series = pd.Series(index=series.index)
         for interval in self.intervals:
             tmp_series = series[interval[0] : interval[1]]
             if tmp_series.empty:
                 continue
-            x = self._get_timestamps(series=tmp_series)
-            trend = self.per_interval_models[interval].predict(x)
-            trend_series[tmp_series.index] = trend
-        return trend_series
+            features = self._get_features(series=tmp_series)
+            per_interval_prediction = self.per_interval_models[interval].predict(features=features)
+            prediction_series[tmp_series.index] = per_interval_prediction
+        return prediction_series
+
+    @abstractmethod
+    def _apply_transformation(self, df: pd.DataFrame, transformed_series: pd.Series) -> pd.DataFrame:
+        """Apply transformation given by per_interval_model.
+
+        Parameters
+        ----------
+        df:
+            original dataframe to apply transformation
+        transformed_series:
+            transformed series to be applied to df
 
-    def fit(self, df: pd.DataFrame) -> "_OneSegmentChangePointsTrendTransform":
-        """Fit OneSegmentChangePointsTransform: find trend change points in ``df``, fit detrend models with data from intervals of stable trend.
+        Returns
+        -------
+        transformed_df:
+            dataframe with applied transformation
+        """
+        pass
+
+    @abstractmethod
+    def _apply_inverse_transformation(self, df: pd.DataFrame, transformed_series: pd.Series) -> pd.DataFrame:
+        """Apply inverse transformation given by per_interval_model.
 
         Parameters
         ----------
         df:
-            one segment dataframe indexed with timestamp
+            transformed dataframe to apply inverse transformation
+        transformed_series:
+            transformed series to be applied to df
 
         Returns
         -------
-        :
+        transformed_df:
+            dataframe with inverse transformation
         """
-        series = df.loc[df[self.in_column].first_valid_index() : df[self.in_column].last_valid_index(), self.in_column]
-        if series.isnull().values.any():
-            raise ValueError("The input column contains NaNs in the middle of the series! Try to use the imputer.")
-        change_points = _find_change_points_segment(
-            series=series, change_point_model=self.change_point_model, **self.change_point_model_predict_params
-        )
-        self.intervals = self._build_trend_intervals(change_points=change_points)
-        self.per_interval_models = self._init_detrend_models(intervals=self.intervals)
-        self._fit_per_interval_model(series=series)
-        return self
+        pass
 
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
-        """Split df to intervals of stable trend and subtract trend from each one.
+        """Transform data from df.
 
         Parameters
         ----------
         df:
-            one segment dataframe to subtract trend
+            dataframe to apply transformation to
 
         Returns
         -------
-        detrended df: pd.DataFrame
-            df with detrended in_column series
+        transformed_df:
+            dataframe with applied transformation
         """
         df._is_copy = False
         series = df[self.in_column]
-        trend_series = self._predict_per_interval_model(series=series)
-        df.loc[:, self.in_column] -= trend_series
-        return df
+        transformed_series = self._predict_per_interval_model(series=series)
+        transformed_df = self._apply_transformation(df=df, transformed_series=transformed_series)
+        return transformed_df
 
     def inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """Split df to intervals of stable trend according to previous change point detection and add trend to each one.
 
         Parameters
         ----------
         df:
@@ -154,56 +189,33 @@
         -------
         df: pd.DataFrame
             df with restored trend in in_column
         """
         df._is_copy = False
         series = df[self.in_column]
         trend_series = self._predict_per_interval_model(series=series)
-        df.loc[:, self.in_column] += trend_series
-        if self.in_column == "target":
-            quantiles = match_target_quantiles(set(df.columns))
-            for quantile_column_nm in quantiles:
-                df.loc[:, quantile_column_nm] += trend_series
+        self._apply_inverse_transformation(df=df, transformed_series=trend_series)
         return df
 
 
-class ChangePointsTrendTransform(PerSegmentWrapper):
-    """ChangePointsTrendTransform subtracts multiple linear trend from series.
+class BaseChangePointsTransform:
+    """Base class for all the change points based transforms."""
 
-    Warning
-    -------
-    This transform can suffer from look-ahead bias. For transforming data at some timestamp
-    it uses information from the whole train part.
-    """
+    pass
 
-    def __init__(
-        self,
-        in_column: str,
-        change_point_model: BaseEstimator,
-        detrend_model: TDetrendModel,
-        **change_point_model_predict_params,
-    ):
-        """Init ChangePointsTrendTransform.
 
-        Parameters
-        ----------
-        in_column:
-            name of column to apply transform to
-        change_point_model:
-            model to get trend change points
-        detrend_model:
-            model to get trend in data
-        change_point_model_predict_params:
-            params for ``change_point_model.predict`` method
-        """
-        self.in_column = in_column
-        self.change_point_model = change_point_model
-        self.detrend_model = detrend_model
-        self.change_point_model_predict_params = change_point_model_predict_params
-        super().__init__(
-            transform=_OneSegmentChangePointsTrendTransform(
-                in_column=self.in_column,
-                change_point_model=self.change_point_model,
-                detrend_model=self.detrend_model,
-                **self.change_point_model_predict_params,
-            )
-        )
+class ReversibleChangePointsTransform(BaseChangePointsTransform, ReversiblePerSegmentWrapper):
+    """ReversibleChangePointsTransform class is a base class for all reversible transforms that work with change point."""
+
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        return []
+
+
+class IrreversibleChangePointsTransform(BaseChangePointsTransform, IrreversiblePerSegmentWrapper, FutureMixin):
+    """IrreversibleChangePointsTransform class is a base class for all irreversible transforms that work with change point."""
+
+    out_column: Optional[str] = None
+
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        return [self.out_column]  # type: ignore
```

### Comparing `etna-1.9.0/etna/transforms/decomposition/detrend.py` & `etna-2.0.0/etna/transforms/decomposition/detrend.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from typing import List
+
 import numpy as np
 import pandas as pd
 from sklearn.base import RegressorMixin
 from sklearn.linear_model import LinearRegression
 from sklearn.linear_model import TheilSenRegressor
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import PolynomialFeatures
 
-from etna.transforms.base import PerSegmentWrapper
-from etna.transforms.base import Transform
+from etna.transforms.base import OneSegmentTransform
+from etna.transforms.base import ReversiblePerSegmentWrapper
 from etna.transforms.utils import match_target_quantiles
 
 
-class _OneSegmentLinearTrendBaseTransform(Transform):
+class _OneSegmentLinearTrendBaseTransform(OneSegmentTransform):
     """LinearTrendBaseTransform is a base class that implements trend subtraction and reconstruction feature."""
 
     def __init__(self, in_column: str, regressor: RegressorMixin, poly_degree: int = 1):
         """
         Create instance of _OneSegmentLinearTrendBaseTransform.
 
         Parameters
@@ -77,15 +79,15 @@
             data to subtract trend from
 
         Returns
         -------
         pd.DataFrame
             residue after trend subtraction
         """
-        result = df.copy()
+        result = df
         x = self._get_x(df)
         x -= self._x_median
         y = df[self.in_column].values
         trend = self._pipeline.predict(x)
         no_trend_timeseries = y - trend
         result[self.in_column] = no_trend_timeseries
         return result
@@ -116,29 +118,29 @@
             data to transform
 
         Returns
         -------
         pd.DataFrame
             data with reconstructed trend
         """
-        result = df.copy()
+        result = df
         x = self._get_x(df)
         x -= self._x_median
         y = df[self.in_column].values
         trend = self._pipeline.predict(x)
         add_trend_timeseries = y + trend
         result[self.in_column] = add_trend_timeseries
         if self.in_column == "target":
             quantiles = match_target_quantiles(set(result.columns))
             for quantile_column_nm in quantiles:
                 result.loc[:, quantile_column_nm] += trend
         return result
 
 
-class LinearTrendTransform(PerSegmentWrapper):
+class LinearTrendTransform(ReversiblePerSegmentWrapper):
     """
     Transform that uses :py:class:`sklearn.linear_model.LinearRegression` to find linear or polynomial trend in data.
 
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
     it uses information from the whole train part.
@@ -160,19 +162,24 @@
         self.poly_degree = poly_degree
         self.regression_params = regression_params
         super().__init__(
             transform=_OneSegmentLinearTrendBaseTransform(
                 in_column=self.in_column,
                 regressor=LinearRegression(**self.regression_params),
                 poly_degree=self.poly_degree,
-            )
+            ),
+            required_features=[self.in_column],
         )
 
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        return []
+
 
-class TheilSenTrendTransform(PerSegmentWrapper):
+class TheilSenTrendTransform(ReversiblePerSegmentWrapper):
     """
     Transform that uses :py:class:`sklearn.linear_model.TheilSenRegressor` to find linear or polynomial trend in data.
 
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
     it uses information from the whole train part.
@@ -199,9 +206,14 @@
         self.poly_degree = poly_degree
         self.regression_params = regression_params
         super().__init__(
             transform=_OneSegmentLinearTrendBaseTransform(
                 in_column=self.in_column,
                 regressor=TheilSenRegressor(**self.regression_params),
                 poly_degree=self.poly_degree,
-            )
+            ),
+            required_features=[self.in_column],
         )
+
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        return []
```

### Comparing `etna-1.9.0/etna/transforms/decomposition/stl.py` & `etna-2.0.0/etna/transforms/decomposition/stl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import Any
 from typing import Dict
+from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 from statsmodels.tsa.arima.model import ARIMA
 from statsmodels.tsa.base.tsa_model import TimeSeriesModel
 from statsmodels.tsa.exponential_smoothing.ets import ETSModel
 from statsmodels.tsa.forecasting.stl import STLForecast
 from statsmodels.tsa.forecasting.stl import STLForecastResults
 
-from etna.transforms.base import PerSegmentWrapper
-from etna.transforms.base import Transform
+from etna.transforms.base import OneSegmentTransform
+from etna.transforms.base import ReversiblePerSegmentWrapper
 from etna.transforms.utils import match_target_quantiles
 
 
-class _OneSegmentSTLTransform(Transform):
+class _OneSegmentSTLTransform(OneSegmentTransform):
     def __init__(
         self,
         in_column: str,
         period: int,
         model: Union[str, TimeSeriesModel] = "arima",
         robust: bool = False,
         model_kwargs: Optional[Dict[str, Any]] = None,
@@ -117,15 +118,15 @@
             Features dataframe with time
 
         Returns
         -------
         result: pd.DataFrame
             Dataframe with extracted features
         """
-        result = df.copy()
+        result = df
         if self.fit_results is not None:
             season_trend = self.fit_results.get_prediction(
                 start=df[self.in_column].first_valid_index(), end=df[self.in_column].last_valid_index()
             ).predicted_mean
         else:
             raise ValueError("Transform is not fitted! Fit the Transform before calling transform method.")
         result[self.in_column] -= season_trend
@@ -141,27 +142,29 @@
             Features dataframe with time
 
         Returns
         -------
         result: pd.DataFrame
             Dataframe with extracted features
         """
-        result = df.copy()
+        result = df
         if self.fit_results is None:
             raise ValueError("Transform is not fitted! Fit the Transform before calling inverse_transform method.")
-        season_trend = self.fit_results.get_prediction(start=df.index.min(), end=df.index.max()).predicted_mean
+        season_trend = self.fit_results.get_prediction(
+            start=df[self.in_column].first_valid_index(), end=df[self.in_column].last_valid_index()
+        ).predicted_mean
         result[self.in_column] += season_trend
         if self.in_column == "target":
             quantiles = match_target_quantiles(set(result.columns))
             for quantile_column_nm in quantiles:
                 result.loc[:, quantile_column_nm] += season_trend
         return result
 
 
-class STLTransform(PerSegmentWrapper):
+class STLTransform(ReversiblePerSegmentWrapper):
     """Transform that uses :py:class:`statsmodels.tsa.seasonal.STL` to subtract season and trend from the data.
 
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
     it uses information from the whole train part.
     """
@@ -210,9 +213,14 @@
             transform=_OneSegmentSTLTransform(
                 in_column=self.in_column,
                 period=self.period,
                 model=self.model,
                 robust=self.robust,
                 model_kwargs=self.model_kwargs,
                 stl_kwargs=self.stl_kwargs,
-            )
+            ),
+            required_features=[self.in_column],
         )
+
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        return []
```

### Comparing `etna-1.9.0/etna/transforms/encoders/categorical.py` & `etna-2.0.0/etna/transforms/encoders/categorical.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 from enum import Enum
+from typing import List
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 from sklearn import preprocessing
 from sklearn.utils._encode import _check_unknown
 from sklearn.utils._encode import _encode
 
 from etna.datasets import TSDataset
-from etna.transforms.base import Transform
+from etna.transforms.base import IrreversibleTransform
 
 
 class ImputerMode(str, Enum):
     """Enum for different imputation strategy."""
 
     new_value = "new_value"
     mean = "mean"
     none = "none"
 
 
 class _LabelEncoder(preprocessing.LabelEncoder):
     def transform(self, y: pd.Series, strategy: str):
         diff = _check_unknown(y, known_values=self.classes_)
 
-        index = np.where(np.isin(y, diff))[0]
+        is_new_index = np.isin(y, diff)
 
-        encoded = _encode(y, uniques=self.classes_, check_unknown=False).astype(float)
+        encoded = np.zeros(y.shape[0], dtype=float)
+        encoded[~is_new_index] = _encode(y.iloc[~is_new_index], uniques=self.classes_, check_unknown=False).astype(
+            float
+        )
 
         if strategy == ImputerMode.none:
             filling_value = None
         elif strategy == ImputerMode.new_value:
             filling_value = -1
         elif strategy == ImputerMode.mean:
             filling_value = np.mean(encoded[~np.isin(y, diff)])
         else:
             raise ValueError(f"The strategy '{strategy}' doesn't exist")
 
-        encoded[index] = filling_value
+        encoded[is_new_index] = filling_value
         return encoded
 
 
-class LabelEncoderTransform(Transform):
+class LabelEncoderTransform(IrreversibleTransform):
     """Encode categorical feature with value between 0 and n_classes-1."""
 
     def __init__(self, in_column: str, out_column: Optional[str] = None, strategy: str = ImputerMode.mean):
         """
         Init LabelEncoderTransform.
 
         Parameters
@@ -59,20 +63,28 @@
             - If "new_value", then replace missing values with '-1'
 
             - If "mean", then replace missing values using the mean in encoded column
 
             - If "none", then replace missing values with None
 
         """
+        super().__init__(required_features=[in_column])
         self.in_column = in_column
         self.out_column = out_column
         self.strategy = strategy
         self.le = _LabelEncoder()
+        self.in_column_regressor: Optional[bool] = None
 
-    def fit(self, df: pd.DataFrame) -> "LabelEncoderTransform":
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        if self.in_column_regressor is None:
+            raise ValueError("Fit the transform to get the correct regressors info!")
+        return [self._get_column_name()] if self.in_column_regressor else []
+
+    def _fit(self, df: pd.DataFrame) -> "LabelEncoderTransform":
         """
         Fit Label encoder.
 
         Parameters
         ----------
         df:
             Dataframe with data to fit the transform
@@ -81,15 +93,21 @@
         :
             Fitted transform
         """
         y = TSDataset.to_flatten(df)[self.in_column]
         self.le.fit(y=y)
         return self
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def fit(self, ts: TSDataset) -> "LabelEncoderTransform":
+        """Fit the transform."""
+        self.in_column_regressor = self.in_column in ts.regressors
+        super().fit(ts)
+        return self
+
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Encode the ``in_column`` by fitted Label encoder.
 
         Parameters
         ----------
         df
             Dataframe with data to transform
@@ -109,15 +127,15 @@
     def _get_column_name(self) -> str:
         """Get the ``out_column`` depending on the transform's parameters."""
         if self.out_column:
             return self.out_column
         return self.__repr__()
 
 
-class OneHotEncoderTransform(Transform):
+class OneHotEncoderTransform(IrreversibleTransform):
     """Encode categorical feature as a one-hot numeric features.
 
     If unknown category is encountered during transform, the resulting one-hot
     encoded columns for this feature will be all zeros.
     """
 
     def __init__(self, in_column: str, out_column: Optional[str] = None):
@@ -127,56 +145,69 @@
         Parameters
         ----------
         in_column:
             Name of column to be encoded
         out_column:
             Prefix of names of added columns. If not given, use ``self.__repr__()``
         """
+        super().__init__(required_features=[in_column])
         self.in_column = in_column
         self.out_column = out_column
-        self.ohe = preprocessing.OneHotEncoder(handle_unknown="ignore", sparse=False)
+        self.ohe = preprocessing.OneHotEncoder(handle_unknown="ignore", sparse=False, dtype=int)
+        self.in_column_regressor: Optional[bool] = None
+
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        if self.in_column_regressor is None:
+            raise ValueError("Fit the transform to get the correct regressors info!")
+        return self._get_out_column_names() if self.in_column_regressor else []
 
-    def fit(self, df: pd.DataFrame) -> "OneHotEncoderTransform":
+    def _fit(self, df: pd.DataFrame) -> "OneHotEncoderTransform":
         """
         Fit One Hot encoder.
 
         Parameters
         ----------
         df:
             Dataframe with data to fit the transform
         Returns
         -------
         :
             Fitted transform
         """
-        x = TSDataset.to_flatten(df)[self.in_column].values.reshape(-1, 1)
+        x = TSDataset.to_flatten(df)[[self.in_column]]
         self.ohe.fit(X=x)
         return self
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def fit(self, ts: TSDataset) -> "OneHotEncoderTransform":
+        """Fit the transform."""
+        self.in_column_regressor = self.in_column in ts.regressors
+        super().fit(ts)
+        return self
+
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Encode the `in_column` by fitted One Hot encoder.
 
         Parameters
         ----------
         df
             Dataframe with data to transform
 
         Returns
         -------
         :
             Dataframe with column with encoded values
         """
-        out_column = self._get_column_name()
-        out_columns = [out_column + "_" + str(i) for i in range(len(self.ohe.categories_[0]))]
         result_df = TSDataset.to_flatten(df)
-        x = result_df[self.in_column].values.reshape(-1, 1)
+        x = result_df[[self.in_column]]
+        out_columns = self._get_out_column_names()
         result_df[out_columns] = self.ohe.transform(X=x)
         result_df[out_columns] = result_df[out_columns].astype("category")
         result_df = TSDataset.to_dataset(result_df)
         return result_df
 
-    def _get_column_name(self) -> str:
-        """Get the ``out_column`` depending on the transform's parameters."""
-        if self.out_column:
-            return self.out_column
-        return self.__repr__()
+    def _get_out_column_names(self) -> List[str]:
+        """Get the list of ``out_column`` depending on the transform's parameters."""
+        out_column = self.out_column if self.out_column is not None else self.__repr__()
+        out_columns = [out_column + "_" + str(i) for i in range(len(self.ohe.categories_[0]))]
+        return out_columns
```

### Comparing `etna-1.9.0/etna/transforms/feature_selection/base.py` & `etna-2.0.0/etna/transforms/feature_selection/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,69 @@
 import warnings
 from abc import ABC
 from typing import List
+from typing import Optional
 from typing import Union
 
 import pandas as pd
 from typing_extensions import Literal
 
-from etna.transforms import Transform
+from etna.transforms import ReversibleTransform
 
 
-class BaseFeatureSelectionTransform(Transform, ABC):
+class BaseFeatureSelectionTransform(ReversibleTransform, ABC):
     """Base class for feature selection transforms."""
 
-    def __init__(self, features_to_use: Union[List[str], Literal["all"]] = "all"):
+    def __init__(self, features_to_use: Union[List[str], Literal["all"]] = "all", return_features: bool = False):
+        super().__init__(required_features="all")
         self.features_to_use = features_to_use
         self.selected_features: List[str] = []
+        self.return_features = return_features
+        self._df_removed: Optional[pd.DataFrame] = None
+
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        return []
 
     def _get_features_to_use(self, df: pd.DataFrame) -> List[str]:
         """Get list of features from the dataframe to perform the selection on."""
-        features = set(df.columns.get_level_values("feature")) - set(["target"])
+        features = set(df.columns.get_level_values("feature")) - {"target"}
         if self.features_to_use != "all":
             features = features.intersection(self.features_to_use)
             if sorted(features) != sorted(self.features_to_use):
                 warnings.warn("Columns from feature_to_use which are out of dataframe columns will be dropped!")
         return sorted(features)
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """Select top_k features.
 
         Parameters
         ----------
         df:
             dataframe with all segments data
 
         Returns
         -------
         result: pd.DataFrame
             Dataframe with with only selected features
         """
-        result = df.copy()
         rest_columns = set(df.columns.get_level_values("feature")) - set(self._get_features_to_use(df))
         selected_columns = sorted(self.selected_features + list(rest_columns))
-        result = result.loc[:, pd.IndexSlice[:, selected_columns]]
+        result = df.loc[:, pd.IndexSlice[:, selected_columns]]
+        if self.return_features:
+            self._df_removed = df.drop(result.columns, axis=1)
         return result
+
+    def _inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Apply inverse transform to the data.
+
+        Parameters
+        ----------
+        df:
+            dataframe to apply inverse transformation
+
+        Returns
+        -------
+        result: pd.DataFrame
+            dataframe before transformation
+        """
+        return pd.concat([df, self._df_removed], axis=1)
```

### Comparing `etna-1.9.0/etna/transforms/feature_selection/feature_importance.py` & `etna-2.0.0/etna/transforms/feature_selection/feature_importance.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,32 +36,38 @@
     Notes
     -----
     Transform works with any type of features, however most of the models works only with regressors.
     Therefore, it is recommended to pass the regressors into the feature selection transforms.
     """
 
     def __init__(
-        self, model: TreeBasedRegressor, top_k: int, features_to_use: Union[List[str], Literal["all"]] = "all"
+        self,
+        model: TreeBasedRegressor,
+        top_k: int,
+        features_to_use: Union[List[str], Literal["all"]] = "all",
+        return_features: bool = False,
     ):
         """
         Init TreeFeatureSelectionTransform.
 
         Parameters
         ----------
         model:
             model to make selection, it should have ``feature_importances_`` property
             (e.g. all tree-based regressors in sklearn)
         top_k:
             num of features to select; if there are not enough features, then all will be selected
         features_to_use:
             columns of the dataset to select from; if "all" value is given, all columns are used
+        return_features:
+            indicates whether to return features or not.
         """
         if not isinstance(top_k, int) or top_k < 0:
             raise ValueError("Parameter top_k should be positive integer")
-        super().__init__(features_to_use=features_to_use)
+        super().__init__(features_to_use=features_to_use, return_features=return_features)
         self.model = model
         self.top_k = top_k
 
     def _get_train(self, df: pd.DataFrame) -> Tuple[pd.DataFrame, pd.DataFrame]:
         """Get train data for model."""
         features = self._get_features_to_use(df)
         df = TSDataset.to_flatten(df).dropna()
@@ -81,15 +87,15 @@
     def _select_top_k_features(weights: Dict[str, float], top_k: int) -> List[str]:
         keys = np.array(list(weights.keys()))
         values = np.array(list(weights.values()))
         idx_sort = np.argsort(values)[::-1]
         idx_selected = idx_sort[:top_k]
         return keys[idx_selected].tolist()
 
-    def fit(self, df: pd.DataFrame) -> "TreeFeatureSelectionTransform":
+    def _fit(self, df: pd.DataFrame) -> "TreeFeatureSelectionTransform":
         """
         Fit the model and remember features to select.
 
         Parameters
         ----------
         df:
             dataframe with all segments data
@@ -120,14 +126,15 @@
         self,
         relevance_table: RelevanceTable,
         top_k: int,
         features_to_use: Union[List[str], Literal["all"]] = "all",
         relevance_aggregation_mode: str = AggregationMode.mean,
         redundancy_aggregation_mode: str = AggregationMode.mean,
         atol: float = 1e-10,
+        return_features: bool = False,
         **relevance_params,
     ):
         """
         Init MRMRFeatureSelectionTransform.
 
         Parameters
         ----------
@@ -140,27 +147,29 @@
             if "all" value is given, all columns are used
         relevance_aggregation_mode:
             the method for relevance values per-segment aggregation
         redundancy_aggregation_mode:
             the method for redundancy values per-segment aggregation
         atol:
             the absolute tolerance to compare the float values
+        return_features:
+            indicates whether to return features or not.
         """
         if not isinstance(top_k, int) or top_k < 0:
             raise ValueError("Parameter top_k should be positive integer")
 
-        super().__init__(features_to_use=features_to_use)
+        super().__init__(features_to_use=features_to_use, return_features=return_features)
         self.relevance_table = relevance_table
         self.top_k = top_k
         self.relevance_aggregation_mode = relevance_aggregation_mode
         self.redundancy_aggregation_mode = redundancy_aggregation_mode
         self.atol = atol
         self.relevance_params = relevance_params
 
-    def fit(self, df: pd.DataFrame) -> "MRMRFeatureSelectionTransform":
+    def _fit(self, df: pd.DataFrame) -> "MRMRFeatureSelectionTransform":
         """
         Fit the method and remember features to select.
 
         Parameters
         ----------
         df:
             dataframe with all segments data
```

### Comparing `etna-1.9.0/etna/transforms/feature_selection/filter.py` & `etna-2.0.0/etna/transforms/feature_selection/filter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,74 +1,106 @@
+from typing import List
 from typing import Optional
 from typing import Sequence
 
 import pandas as pd
 
-from etna.transforms.base import Transform
+from etna.transforms.base import ReversibleTransform
 
 
-class FilterFeaturesTransform(Transform):
+class FilterFeaturesTransform(ReversibleTransform):
     """Filters features in each segment of the dataframe."""
 
-    def __init__(self, include: Optional[Sequence[str]] = None, exclude: Optional[Sequence[str]] = None):
+    def __init__(
+        self,
+        include: Optional[Sequence[str]] = None,
+        exclude: Optional[Sequence[str]] = None,
+        return_features: bool = False,
+    ):
         """Create instance of FilterFeaturesTransform.
 
         Parameters
         ----------
         include:
             list of columns to pass through filter
         exclude:
             list of columns to not pass through
-
+        return_features:
+            indicates whether to return features or not.
         Raises
         ------
         ValueError:
             if both options set or non of them
         """
+        super().__init__(required_features="all")
         self.include: Optional[Sequence[str]] = None
         self.exclude: Optional[Sequence[str]] = None
+        self.return_features: bool = return_features
+        self._df_removed: Optional[pd.DataFrame] = None
         if include is not None and exclude is None:
             self.include = list(set(include))
         elif exclude is not None and include is None:
             self.exclude = list(set(exclude))
         else:
             raise ValueError("There should be exactly one option set: include or exclude")
 
-    def fit(self, df: pd.DataFrame) -> "FilterFeaturesTransform":
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        return []
+
+    def _fit(self, df: pd.DataFrame) -> "FilterFeaturesTransform":
         """Fit method does nothing and is kept for compatibility.
 
         Parameters
         ----------
         df:
             dataframe with data.
 
         Returns
         -------
         result: FilterFeaturesTransform
         """
         return self
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """Filter features according to include/exclude parameters.
 
         Parameters
         ----------
         df:
             dataframe with data to transform.
 
         Returns
         -------
         result: pd.Dataframe
             transformed dataframe
         """
-        result = df.copy()
+        result = df
         features = df.columns.get_level_values("feature")
         if self.include is not None:
             if not set(self.include).issubset(features):
                 raise ValueError(f"Features {set(self.include) - set(features)} are not present in the dataset.")
-            segments = sorted(set(df.columns.get_level_values("segment")))
-            result = result.loc[:, pd.IndexSlice[segments, self.include]]
+            result = result.loc[:, pd.IndexSlice[:, self.include]]
         if self.exclude is not None and self.exclude:
             if not set(self.exclude).issubset(features):
                 raise ValueError(f"Features {set(self.exclude) - set(features)} are not present in the dataset.")
-            result = result.drop(columns=self.exclude, level="feature")
+            result = df.drop(columns=self.exclude, level="feature")
+        if self.return_features:
+            self._df_removed = df.drop(result.columns, axis=1)
+
+        result = result.sort_index(axis=1)
         return result
+
+    def _inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Apply inverse transform to the data.
+
+        Parameters
+        ----------
+        df:
+            dataframe to apply inverse transformation
+
+        Returns
+        -------
+        result: pd.DataFrame
+            dataframe before transformation
+        """
+        return pd.concat([df, self._df_removed], axis=1)
```

### Comparing `etna-1.9.0/etna/transforms/feature_selection/gale_shapley.py` & `etna-2.0.0/etna/transforms/feature_selection/gale_shapley.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,14 +232,15 @@
 
     def __init__(
         self,
         relevance_table: RelevanceTable,
         top_k: int,
         features_to_use: Union[List[str], Literal["all"]] = "all",
         use_rank: bool = False,
+        return_features: bool = False,
         **relevance_params,
     ):
         """Init GaleShapleyFeatureSelectionTransform.
 
         Parameters
         ----------
         relevance_table:
@@ -247,16 +248,18 @@
         top_k:
             number of features that should be selected from all the given ones
         features_to_use:
             columns of the dataset to select from
             if "all" value is given, all columns are used
         use_rank:
             if True, use rank in relevance table computation
+        return_features:
+            indicates whether to return features or not.
         """
-        super().__init__(features_to_use=features_to_use)
+        super().__init__(features_to_use=features_to_use, return_features=return_features)
         self.relevance_table = relevance_table
         self.top_k = top_k
         self.use_rank = use_rank
         self.greater_is_better = False if use_rank else relevance_table.greater_is_better
         self.relevance_params = relevance_params
 
     def _compute_relevance_table(self, df: pd.DataFrame, features: List[str]) -> pd.DataFrame:
@@ -337,15 +340,15 @@
     ) -> List[str]:
         """Choose n features from given ones according to relevance_matrix."""
         features_relevance = {feature: relevance_table[feature][segment] for segment, feature in matches.items()}
         sorted_features = sorted(features_relevance.items(), key=lambda item: item[1], reverse=greater_is_better)
         selected_features = [feature[0] for feature in sorted_features][:n]
         return selected_features
 
-    def fit(self, df: pd.DataFrame) -> "GaleShapleyFeatureSelectionTransform":
+    def _fit(self, df: pd.DataFrame) -> "GaleShapleyFeatureSelectionTransform":
         """Fit Gale-Shapley algo and find a pool of ``top_k`` features.
 
         Parameters
         ----------
         df:
             dataframe to fit algo
         """
@@ -364,15 +367,15 @@
         )
         last_step_features_number = self.top_k % len(segment_features_ranking)
         for step in range(gale_shapley_steps_number):
             matches = self._gale_shapley_iteration(
                 segment_features_ranking=segment_features_ranking,
                 feature_segments_ranking=feature_segments_ranking,
             )
-            if step == gale_shapley_steps_number - 1:
+            if step == gale_shapley_steps_number - 1 and last_step_features_number != 0:
                 selected_features = self._process_last_step(
                     matches=matches,
                     relevance_table=relevance_table,
                     n=last_step_features_number,
                     greater_is_better=self.greater_is_better,
                 )
             else:
```

### Comparing `etna-1.9.0/etna/transforms/math/__init__.py` & `etna-2.0.0/etna/transforms/math/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from etna.transforms.math.add_constant import AddConstTransform
+from etna.transforms.math.apply_lambda import LambdaTransform
 from etna.transforms.math.differencing import DifferencingTransform
 from etna.transforms.math.lags import LagTransform
 from etna.transforms.math.log import LogTransform
 from etna.transforms.math.power import BoxCoxTransform
 from etna.transforms.math.power import YeoJohnsonTransform
 from etna.transforms.math.scalers import MaxAbsScalerTransform
 from etna.transforms.math.scalers import MinMaxScalerTransform
 from etna.transforms.math.scalers import RobustScalerTransform
 from etna.transforms.math.scalers import StandardScalerTransform
 from etna.transforms.math.sklearn import SklearnTransform
 from etna.transforms.math.statistics import MADTransform
 from etna.transforms.math.statistics import MaxTransform
 from etna.transforms.math.statistics import MeanTransform
 from etna.transforms.math.statistics import MedianTransform
+from etna.transforms.math.statistics import MinMaxDifferenceTransform
 from etna.transforms.math.statistics import MinTransform
 from etna.transforms.math.statistics import QuantileTransform
 from etna.transforms.math.statistics import StdTransform
+from etna.transforms.math.statistics import SumTransform
 from etna.transforms.math.statistics import WindowStatisticsTransform
```

### Comparing `etna-1.9.0/etna/transforms/math/add_constant.py` & `etna-2.0.0/etna/transforms/math/power.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,131 +1,113 @@
-import warnings
+from typing import List
 from typing import Optional
+from typing import Union
 
-import pandas as pd
+from sklearn.preprocessing import PowerTransformer
 
-from etna.transforms.base import PerSegmentWrapper
-from etna.transforms.base import Transform
-from etna.transforms.utils import match_target_quantiles
+from etna.transforms.math.sklearn import SklearnTransform
+from etna.transforms.math.sklearn import TransformMode
 
 
-class _OneSegmentAddConstTransform(Transform):
-    def __init__(self, in_column: str, out_column: str, value: float, inplace: bool = True):
-        """
-        Init _OneSegmentAddConstTransform.
-
-        Parameters
-        ----------
-        in_column:
-            column to apply transform
-        out_column:
-            name of added column
-        value:
-            value that should be added to the series
-        inplace:
-
-            * if True, apply add constant transformation inplace to in_column,
-
-            * if False, add transformed column to dataset
-
-        """
-        self.in_column = in_column
-        self.value = value
-        self.inplace = inplace
-        self.out_column = out_column
-
-    def fit(self, df: pd.DataFrame) -> "_OneSegmentAddConstTransform":
-        """
-        Fit preprocess method, does nothing in _OneSegmentAddConstTransform case.
+class YeoJohnsonTransform(SklearnTransform):
+    """YeoJohnsonTransform applies Yeo-Johns transformation to a DataFrame.
 
-        Returns
-        -------
-        :
-        """
-        return self
+    Warning
+    -------
+    This transform can suffer from look-ahead bias. For transforming data at some timestamp
+    it uses information from the whole train part.
+    """
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def __init__(
+        self,
+        in_column: Optional[Union[str, List[str]]] = None,
+        inplace: bool = True,
+        out_column: Optional[str] = None,
+        standardize: bool = True,
+        mode: Union[TransformMode, str] = "per-segment",
+    ):
         """
-        Transform method: add given value to all the series values.
+        Create instance of YeoJohnsonTransform.
 
         Parameters
         ----------
-        df:
-            DataFrame to transform
-
-        Returns
-        -------
-        :
-            transformed series
-        """
-        result_df = df.copy()
-        result_df[self.out_column] = result_df[self.in_column] + self.value
-        return result_df
+        in_column:
+            columns to be transformed, if None - all columns will be transformed.
+        inplace:
 
-    def inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Apply inverse transformation: subtract given value from all the series values.
+            * if True, apply transformation inplace to in_column,
 
-        Parameters
-        ----------
-        df:
-            DataFrame to apply inverse transformation
+            * if False, add column to dataset.
 
-        Returns
-        -------
-        :
-            transformed series
+        out_column:
+            base for the names of generated columns, uses ``self.__repr__()`` if not given.
+        standardize:
+            Set to True to apply zero-mean, unit-variance normalization to the
+            transformed output.
+
+        Raises
+        ------
+        ValueError:
+            if incorrect mode given
         """
-        result_df = df.copy()
-        if self.inplace:
-            result_df[self.in_column] = result_df[self.out_column] - self.value
-            if self.in_column == "target":
-                quantiles = match_target_quantiles(set(result_df.columns))
-                for quantile_column_nm in quantiles:
-                    result_df[quantile_column_nm] = result_df[quantile_column_nm] - self.value
-        return result_df
+        self.standardize = standardize
+        super().__init__(
+            in_column=in_column,
+            inplace=inplace,
+            out_column=out_column,
+            transformer=PowerTransformer(method="yeo-johnson", standardize=self.standardize),
+            mode=mode,
+        )
 
 
-class AddConstTransform(PerSegmentWrapper):
-    """AddConstTransform add constant for given series."""
+class BoxCoxTransform(SklearnTransform):
+    """BoxCoxTransform applies Box-Cox transformation to DataFrame.
 
-    def __init__(self, in_column: str, value: float, inplace: bool = True, out_column: Optional[str] = None):
+    Warning
+    -------
+    This transform can suffer from look-ahead bias. For transforming data at some timestamp
+    it uses information from the whole train part.
+    """
+
+    def __init__(
+        self,
+        in_column: Optional[Union[str, List[str]]] = None,
+        inplace: bool = True,
+        out_column: Optional[str] = None,
+        standardize: bool = True,
+        mode: Union[TransformMode, str] = "per-segment",
+    ):
         """
-        Init AddConstTransform.
+        Create instance of BoxCoxTransform.
 
         Parameters
         ----------
         in_column:
-            column to apply transform
-        value:
-            value that should be added to the series
+            columns to be transformed, if None - all columns will be transformed.
         inplace:
 
-            * if True, apply add constant transformation inplace to in_column,
+            * if True, apply transformation inplace to in_column,
 
-            * if False, add transformed column to dataset
+            * if False, add column to dataset.
 
         out_column:
-            name of added column. If not given, use ``self.__repr__()``
+            base for the names of generated columns, uses ``self.__repr__()`` if not given.
+        standardize:
+            Set to True to apply zero-mean, unit-variance normalization to the
+            transformed output.
+
+        Raises
+        ------
+        ValueError:
+            if incorrect mode given
         """
-        self.in_column = in_column
-        self.value = value
-        self.inplace = inplace
-        self.out_column = out_column
-
-        if self.inplace and out_column:
-            warnings.warn("Transformation will be applied inplace, out_column param will be ignored")
-
-        if self.inplace:
-            out_column_result = self.in_column
-        elif self.out_column:
-            out_column_result = self.out_column
-        else:
-            out_column_result = self.__repr__()
+        self.standardize = standardize
         super().__init__(
-            transform=_OneSegmentAddConstTransform(
-                in_column=in_column, value=value, inplace=inplace, out_column=out_column_result
-            )
+            in_column=in_column,
+            inplace=inplace,
+            out_column=out_column,
+            transformer=PowerTransformer(method="box-cox", standardize=self.standardize),
+            mode=mode,
         )
 
 
-__all__ = ["AddConstTransform"]
+__all__ = ["BoxCoxTransform", "YeoJohnsonTransform"]
```

### Comparing `etna-1.9.0/etna/transforms/math/differencing.py` & `etna-2.0.0/etna/transforms/math/differencing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Union
+from typing import cast
 
 import numpy as np
 import pandas as pd
 
-from etna.transforms.base import Transform
+from etna.datasets import TSDataset
+from etna.transforms.base import ReversibleTransform
+from etna.transforms.utils import check_new_segments
 from etna.transforms.utils import match_target_quantiles
 
 
-class _SingleDifferencingTransform(Transform):
+class _SingleDifferencingTransform(ReversibleTransform):
     """Calculate a time series differences of order 1.
 
-    This transform can work with NaNs at the beginning of the segment, but fails when meets NaN inside the segment.
+    During ``fit`` this transform can work with NaNs at the beginning of the segment, but fails when meets NaN inside the segment.
+    During ``transform`` and ``inverse_transform`` there is no special treatment of NaNs.
 
     Notes
     -----
     To understand how transform works we recommend:
     `Stationarity and Differencing <https://otexts.com/fpp2/stationarity.html>`_
     """
 
@@ -50,91 +54,110 @@
             * if isn't set, name will be based on ``self.__repr__()``
 
         Raises
         ------
         ValueError:
             if period is not integer >= 1
         """
+        super().__init__(required_features=[in_column])
         self.in_column = in_column
 
         if not isinstance(period, int) or period < 1:
             raise ValueError("Period should be at least 1")
         self.period = period
 
         self.inplace = inplace
         self.out_column = out_column
 
         self._train_timestamp: Optional[pd.DatetimeIndex] = None
         self._train_init_dict: Optional[Dict[str, pd.Series]] = None
         self._test_init_df: Optional[pd.DataFrame] = None
+        self.in_column_regressor: Optional[bool] = None
 
     def _get_column_name(self) -> str:
+        if self.inplace:
+            return self.in_column
         if self.out_column is None:
             return self.__repr__()
         else:
             return self.out_column
 
-    def fit(self, df: pd.DataFrame) -> "_SingleDifferencingTransform":
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        if self.in_column_regressor is None:
+            raise ValueError("Fit the transform to get the correct regressors info!")
+        if self.inplace:
+            return []
+        return [self._get_column_name()] if self.in_column_regressor else []
+
+    def fit(self, ts: TSDataset) -> "_SingleDifferencingTransform":
+        """Fit the transform."""
+        self.in_column_regressor = self.in_column in ts.regressors
+        super().fit(ts)
+        return self
+
+    def _fit(self, df: pd.DataFrame) -> "_SingleDifferencingTransform":
         """Fit the transform.
 
         Parameters
         ----------
         df:
             dataframe with data.
 
         Returns
         -------
         result: _SingleDifferencingTransform
+
+        Raises
+        ------
+        ValueError:
+            if NaNs are present inside the segment
         """
         segments = sorted(set(df.columns.get_level_values("segment")))
         fit_df = df.loc[:, pd.IndexSlice[segments, self.in_column]].copy()
 
-        self._train_timestamp = fit_df.index
-        self._train_init_dict = {}
+        train_init_dict = {}
         for current_segment in segments:
             cur_series = fit_df.loc[:, pd.IndexSlice[current_segment, self.in_column]]
             cur_series = cur_series.loc[cur_series.first_valid_index() :]
 
             if cur_series.isna().sum() > 0:
                 raise ValueError(f"There should be no NaNs inside the segments")
 
-            self._train_init_dict[current_segment] = cur_series[: self.period]
+            train_init_dict[current_segment] = cur_series[: self.period]
+
+        self._train_init_dict = train_init_dict
+        self._train_timestamp = fit_df.index
         self._test_init_df = fit_df.iloc[-self.period :, :]
         # make multiindex levels consistent
         self._test_init_df.columns = self._test_init_df.columns.remove_unused_levels()
         return self
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """Make a differencing transformation.
 
         Parameters
         ----------
         df:
             dataframe with data to transform.
 
         Returns
         -------
-        result: pd.Dataframe
+        result:
             transformed dataframe
         """
-        if self._train_init_dict is None or self._test_init_df is None or self._train_timestamp is None:
-            raise AttributeError("Transform is not fitted")
-
         segments = sorted(set(df.columns.get_level_values("segment")))
-        transformed = df.loc[:, pd.IndexSlice[segments, self.in_column]].copy()
+        transformed = df.loc[:, pd.IndexSlice[segments, self.in_column]]
         for current_segment in segments:
             to_transform = transformed.loc[:, pd.IndexSlice[current_segment, self.in_column]]
-            start_idx = to_transform.first_valid_index()
             # make a differentiation
-            transformed.loc[start_idx:, pd.IndexSlice[current_segment, self.in_column]] = to_transform.loc[
-                start_idx:
-            ].diff(periods=self.period)
+            transformed.loc[:, pd.IndexSlice[current_segment, self.in_column]] = to_transform.diff(periods=self.period)
 
         if self.inplace:
-            result_df = df.copy()
+            result_df = df
             result_df.loc[:, pd.IndexSlice[segments, self.in_column]] = transformed
         else:
             transformed_features = pd.DataFrame(
                 transformed, columns=df.loc[:, pd.IndexSlice[segments, self.in_column]].columns, index=df.index
             )
             column_name = self._get_column_name()
             transformed_features.columns = pd.MultiIndex.from_product([segments, [column_name]])
@@ -157,15 +180,15 @@
         # impute values for reconstruction and run reconstruction
         for current_segment in segments:
             init_segment = self._train_init_dict[current_segment]  # type: ignore
             for column in columns_to_inverse:
                 cur_series = result_df.loc[:, pd.IndexSlice[current_segment, column]]
                 cur_series[init_segment.index] = init_segment.values
                 cur_series = self._make_inv_diff(cur_series)
-                result_df.loc[cur_series.index, pd.IndexSlice[current_segment, column]] = cur_series
+                result_df.loc[:, pd.IndexSlice[current_segment, column]] = cur_series
         return result_df
 
     def _reconstruct_test(self, df: pd.DataFrame, columns_to_inverse: Set[str]) -> pd.DataFrame:
         """Reconstruct the test in ``inverse_transform``."""
         segments = sorted(set(df.columns.get_level_values("segment")))
         result_df = df.copy()
 
@@ -180,41 +203,60 @@
             raise ValueError("Test should go after the train without gaps")
 
         # we can reconstruct the values by concatenating saved fit values before test values
         for column in columns_to_inverse:
             to_transform = df.loc[:, pd.IndexSlice[segments, column]].copy()
             init_df = self._test_init_df.copy()  # type: ignore
             init_df.columns.set_levels([column], level="feature", inplace=True)
+            init_df = init_df[segments]
             to_transform = pd.concat([init_df, to_transform])
 
-            # validate values inside the series to transform
-            if to_transform.isna().sum().sum() > 0:
-                raise ValueError(f"There should be no NaNs inside the segments")
-
             # run reconstruction and save the result
             to_transform = self._make_inv_diff(to_transform)
-            result_df.loc[:, pd.IndexSlice[segments, column]] = to_transform
+            result_df.loc[:, pd.IndexSlice[segments, column]] = to_transform.loc[result_df.index]
 
         return result_df
 
-    def inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _fit_transform(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Fit and transform dataframe.
+
+        Parameters
+        ----------
+        df:
+            Dataframe to transform.
+
+        Returns
+        -------
+        :
+            Transformed dataframe.
+        """
+        return self._fit(df=df)._transform(df=df)
+
+    def _inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """Apply inverse transformation to DataFrame.
 
         Parameters
         ----------
         df:
             DataFrame to apply inverse transform.
 
         Returns
         -------
-        result: pd.DataFrame
+        result:
             transformed DataFrame.
+
+        Raises
+        ------
+        ValueError:
+            if inverse transform is applied not to full train nor to test that goes after train
+        ValueError:
+            if inverse transform is applied to test that goes after train with gap
         """
-        if self._train_init_dict is None or self._test_init_df is None or self._train_timestamp is None:
-            raise AttributeError("Transform is not fitted")
+        # we assume this to be fitted
+        self._train_timestamp = cast(pd.DatetimeIndex, self._train_timestamp)
 
         if not self.inplace:
             return df
 
         columns_to_inverse = {self.in_column}
 
         # if we are working with in_column="target" then there can be quantiles to inverse too
@@ -232,18 +274,19 @@
 
         else:
             raise ValueError("Inverse transform can be applied only to full train or test that should be in the future")
 
         return result_df
 
 
-class DifferencingTransform(Transform):
+class DifferencingTransform(ReversibleTransform):
     """Calculate a time series differences.
 
-    This transform can work with NaNs at the beginning of the segment, but fails when meets NaN inside the segment.
+    During ``fit`` this transform can work with NaNs at the beginning of the segment, but fails when meets NaN inside the segment.
+    During ``transform`` and ``inverse_transform`` there is no special treatment of NaNs.
 
     Notes
     -----
     To understand how transform works we recommend:
     `Stationarity and Differencing <https://otexts.com/fpp2/stationarity.html>`_
     """
 
@@ -280,14 +323,15 @@
         Raises
         ------
         ValueError:
             if period is not integer >= 1
         ValueError:
             if order is not integer >= 1
         """
+        super().__init__(required_features=[in_column])
         self.in_column = in_column
 
         if not isinstance(period, int) or period < 1:
             raise ValueError("Period should be at least 1")
         self.period = period
 
         if not isinstance(order, int) or order < 1:
@@ -307,72 +351,125 @@
             )
         )
         # other transforms should make differences inplace
         for _ in range(self.order - 1):
             self._differencing_transforms.append(
                 _SingleDifferencingTransform(in_column=result_out_column, period=self.period, inplace=True)
             )
+        self._fit_segments: Optional[List[str]] = None
+        self.in_column_regressor: Optional[bool] = None
 
     def _get_column_name(self) -> str:
         if self.inplace:
             return self.in_column
         if self.out_column is None:
             return self.__repr__()
         else:
             return self.out_column
 
-    def fit(self, df: pd.DataFrame) -> "DifferencingTransform":
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        if self.in_column_regressor is None:
+            raise ValueError("Fit the transform to get the correct regressors info!")
+        if self.inplace:
+            return []
+        return [self._get_column_name()] if self.in_column_regressor else []
+
+    def fit(self, ts: TSDataset) -> "DifferencingTransform":
+        """Fit the transform."""
+        self.in_column_regressor = self.in_column in ts.regressors
+        super().fit(ts)
+        return self
+
+    def _fit(self, df: pd.DataFrame) -> "DifferencingTransform":
         """Fit the transform.
 
         Parameters
         ----------
         df:
             dataframe with data.
 
         Returns
         -------
         result: DifferencingTransform
+
+        Raises
+        ------
+        ValueError:
+            if NaNs are present inside the segment
         """
         # this is made because transforms of high order may need some columns created by transforms of lower order
-        result_df = df.copy()
+        result_df = df
         for transform in self._differencing_transforms:
-            result_df = transform.fit_transform(result_df)
+            result_df = transform._fit_transform(result_df)
+        self._fit_segments = df.columns.get_level_values("segment").unique().tolist()
         return self
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _check_is_fitted(self):
+        if self._fit_segments is None:
+            raise ValueError("Transform is not fitted!")
+
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """Make a differencing transformation.
 
         Parameters
         ----------
         df:
             dataframe with data to transform.
 
         Returns
         -------
-        result: pd.Dataframe
+        result:
             transformed dataframe
+
+        Raises
+        ------
+        ValueError:
+            if transform isn't fitted
+        NotImplementedError:
+            if there are segments that weren't present during training
         """
-        result_df = df.copy()
+        self._check_is_fitted()
+        segments = df.columns.get_level_values("segment").unique().tolist()
+        if self.inplace:
+            check_new_segments(transform_segments=segments, fit_segments=self._fit_segments)
+
+        result_df = df
         for transform in self._differencing_transforms:
-            result_df = transform.transform(result_df)
+            result_df = transform._transform(result_df)
         return result_df
 
-    def inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """Apply inverse transformation to DataFrame.
 
         Parameters
         ----------
         df:
             DataFrame to apply inverse transform.
 
         Returns
         -------
-        result: pd.DataFrame
+        result:
             transformed DataFrame.
+
+        Raises
+        ------
+        ValueError:
+            if transform isn't fitted
+        NotImplementedError:
+            if there are segments that weren't present during training
+        ValueError:
+            if inverse transform is applied not to full train nor to test that goes after train
+        ValueError:
+            if inverse transform is applied to test that goes after train with gap
         """
+        self._check_is_fitted()
         if not self.inplace:
             return df
 
-        result_df = df.copy()
+        segments = df.columns.get_level_values("segment").unique().tolist()
+        check_new_segments(transform_segments=segments, fit_segments=self._fit_segments)
+
+        result_df = df
         for transform in self._differencing_transforms[::-1]:
-            result_df = transform.inverse_transform(result_df)
+            result_df = transform._inverse_transform(result_df)
         return result_df
```

### Comparing `etna-1.9.0/etna/transforms/math/lags.py` & `etna-2.0.0/etna/transforms/math/lags.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,43 @@
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from etna.transforms.base import FutureMixin
-from etna.transforms.base import PerSegmentWrapper
-from etna.transforms.base import Transform
+from etna.transforms.base import IrreversibleTransform
 
 
-class _OneSegmentLagTransform(Transform):
-    """Generates series of lags from given segment."""
+class LagTransform(IrreversibleTransform, FutureMixin):
+    """Generates series of lags from given dataframe."""
 
     def __init__(self, in_column: str, lags: Union[List[int], int], out_column: Optional[str] = None):
+        """Create instance of LagTransform.
+
+        Parameters
+        ----------
+        in_column:
+            name of processed column
+        lags:
+            int value or list of values for lags computation; if int, generate range of lags from 1 to given value
+        out_column:
+            base for the name of created columns;
+
+            * if set the final name is '{out_column}_{lag_number}';
+
+            * if don't set, name will be ``transform.__repr__()``,
+              repr will be made for transform that creates exactly this column
+
+        Raises
+        ------
+        ValueError:
+            if lags value contains non-positive values
+        """
+        super().__init__(required_features=[in_column])
         if isinstance(lags, int):
             if lags < 1:
                 raise ValueError(f"{type(self).__name__} works only with positive lags values, {lags} given")
             self.lags = list(range(1, lags + 1))
         else:
             if any(lag_value < 1 for lag_value in lags):
                 raise ValueError(f"{type(self).__name__} works only with positive lags values")
@@ -28,49 +49,50 @@
     def _get_column_name(self, lag: int) -> str:
         if self.out_column is None:
             temp_transform = LagTransform(in_column=self.in_column, out_column=self.out_column, lags=[lag])
             return repr(temp_transform)
         else:
             return f"{self.out_column}_{lag}"
 
-    def fit(self, *args) -> "_OneSegmentLagTransform":
-        return self
-
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
-        result = df.copy()
-        for lag in self.lags:
-            result[self._get_column_name(lag)] = df[self.in_column].shift(lag)
-        return result
+    def _fit(self, df: pd.DataFrame) -> "LagTransform":
+        """Fit method does nothing and is kept for compatibility.
 
+        Parameters
+        ----------
+        df:
+            dataframe with data.
 
-class LagTransform(PerSegmentWrapper, FutureMixin):
-    """Generates series of lags from given dataframe."""
+        Returns
+        -------
+        result: LagTransform
+        """
+        return self
 
-    def __init__(self, in_column: str, lags: Union[List[int], int], out_column: Optional[str] = None):
-        """Create instance of LagTransform.
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Add lags to the dataset.
 
         Parameters
         ----------
-        in_column:
-            name of processed column
-        lags:
-            int value or list of values for lags computation; if int, generate range of lags from 1 to given value
-        out_column:
-            base for the name of created columns;
+        df:
+            dataframe with data to transform.
 
-            * if set the final name is '{out_column}_{lag_number}';
-
-            * if don't set, name will be ``transform.__repr__()``,
-              repr will be made for transform that creates exactly this column
-
-        Raises
-        ------
-        ValueError:
-            if lags value contains non-positive values
+        Returns
+        -------
+        result: pd.Dataframe
+            transformed dataframe
         """
-        self.in_column = in_column
-        self.lags = lags
-        self.out_column = out_column
+        result = df
+        segments = sorted(set(df.columns.get_level_values("segment")))
+        all_transformed_features = []
+        features = df.loc[:, pd.IndexSlice[:, self.in_column]]
+        for lag in self.lags:
+            column_name = self._get_column_name(lag)
+            transformed_features = features.shift(lag)
+            transformed_features.columns = pd.MultiIndex.from_product([segments, [column_name]])
+            all_transformed_features.append(transformed_features)
+        result = pd.concat([result] + all_transformed_features, axis=1)
+        result = result.sort_index(axis=1)
+        return result
 
-        super().__init__(
-            transform=_OneSegmentLagTransform(in_column=self.in_column, lags=self.lags, out_column=self.out_column)
-        )
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        return [self._get_column_name(lag) for lag in self.lags]
```

### Comparing `etna-1.9.0/etna/transforms/math/log.py` & `etna-2.0.0/etna/transforms/math/add_constant.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,138 +1,143 @@
 import warnings
-from math import log
-from math import pow
+from typing import List
 from typing import Optional
 
 import pandas as pd
 
-from etna.transforms.base import PerSegmentWrapper
-from etna.transforms.base import Transform
+from etna.datasets import TSDataset
+from etna.datasets import set_columns_wide
+from etna.transforms.base import ReversibleTransform
 from etna.transforms.utils import match_target_quantiles
 
 
-class _OneSegmentLogTransform(Transform):
-    """Instance of this class applies logarithmic transformation to one segment data."""
+class AddConstTransform(ReversibleTransform):
+    """AddConstTransform add constant for given series."""
 
-    def __init__(self, in_column: str, base: int = 10, inplace: bool = True, out_column: Optional[str] = None):
+    def __init__(self, in_column: str, value: float, inplace: bool = True, out_column: Optional[str] = None):
         """
-        Init OneSegmentLogTransform.
+        Init AddConstTransform.
 
         Parameters
         ----------
         in_column:
-            column to apply transform.
-        base:
-            base of logarithm to apply to series.
+            column to apply transform
+        value:
+            value that should be added to the series
         inplace:
 
-            * if True, apply logarithm transformation inplace to in_column,
+            * if True, apply add constant transformation inplace to in_column,
 
-            * if False, add transformed column to dataset.
+            * if False, add transformed column to dataset
 
         out_column:
             name of added column. If not given, use ``self.__repr__()``
         """
-        self.base = base
+        super().__init__(required_features=[in_column])
         self.in_column = in_column
+        self.value = value
         self.inplace = inplace
         self.out_column = out_column
+        self.in_column_regressor: Optional[bool] = None
 
-    def fit(self, df: pd.Series) -> "_OneSegmentLogTransform":
-        """Fit preprocess method, does nothing in OneSegmentLogTransform case.
+        if self.inplace and out_column:
+            warnings.warn("Transformation will be applied inplace, out_column param will be ignored")
 
-        Returns
-        -------
-        :
-        """
-        return self
+    def _get_column_name(self) -> str:
+        if self.inplace:
+            return self.in_column
+        elif self.out_column:
+            return self.out_column
+        else:
+            return self.__repr__()
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
-        """Apply log transformation to series from df.
+    def _fit(self, df: pd.DataFrame) -> "AddConstTransform":
+        """Fit method does nothing and is kept for compatibility.
 
         Parameters
         ----------
         df:
-            series to transform
+            dataframe with data.
 
         Returns
         -------
-        :
-            transformed series
-
-        Raises
-        ------
-        ValueError:
-            if given series contains negative samples
+        result: AddConstTransform
         """
-        if (df[self.in_column] < 0).any():
-            raise ValueError("LogPreprocess can be applied only to non-negative series")
-        result_df = df.copy()
-        result_df[self.out_column] = result_df[self.in_column].apply(lambda x: log(x + 1, self.base))
-        return result_df
+        return self
+
+    def fit(self, ts: TSDataset) -> "AddConstTransform":
+        """Fit the transform."""
+        self.in_column_regressor = self.in_column in ts.regressors
+        super().fit(ts)
+        return self
 
-    def inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
-        """Apply inverse transformation to the series from df.
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Apply adding constant to the dataset.
 
         Parameters
         ----------
         df:
-            series to transform
+            dataframe with data to transform.
 
         Returns
         -------
-        :
-            transformed series
+        result: pd.Dataframe
+            transformed dataframe
         """
-        result_df = df.copy()
+        segments = sorted(set(df.columns.get_level_values("segment")))
+        result = df
+        features = df.loc[:, pd.IndexSlice[:, self.in_column]]
+        transformed_features = features + self.value
         if self.inplace:
-            result_df[self.in_column] = result_df[self.out_column].apply(lambda x: pow(self.base, x) - 1)
-            if self.in_column == "target":
-                quantiles = match_target_quantiles(set(result_df.columns))
-                for quantile_column_nm in quantiles:
-                    result_df[quantile_column_nm] = result_df[quantile_column_nm].apply(lambda x: pow(self.base, x) - 1)
-        return result_df
-
-
-class LogTransform(PerSegmentWrapper):
-    """LogTransform applies logarithm transformation for given series."""
+            result = set_columns_wide(
+                result, transformed_features, features_left=[self.in_column], features_right=[self.in_column]
+            )
+        else:
+            column_name = self._get_column_name()
+            transformed_features.columns = pd.MultiIndex.from_product([segments, [column_name]])
+            result = pd.concat((result, transformed_features), axis=1)
+            result = result.sort_index(axis=1)
+        return result
 
-    def __init__(self, in_column: str, base: int = 10, inplace: bool = True, out_column: Optional[str] = None):
-        """Init LogTransform.
+    def _inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Apply inverse transformation to the dataset.
 
         Parameters
         ----------
-        in_column:
-            column to apply transform
-        base:
-            base of logarithm to apply to series
-        inplace:
-
-            * if True, apply logarithm transformation inplace to in_column,
-
-            * if False, add column add transformed column to dataset
+        df:
+            dataframe with data to transform.
 
-        out_column:
-            name of added column. If not given, use ``self.__repr__()``
+        Returns
+        -------
+        result: pd.DataFrame
+            transformed series
         """
-        self.in_column = in_column
-        self.base = base
-        self.inplace = inplace
-        self.out_column = out_column
-        if self.inplace and out_column:
-            warnings.warn("Transformation will be applied inplace, out_column param will be ignored")
-
+        result = df
         if self.inplace:
-            result_out_column = self.in_column
-        elif out_column:
-            result_out_column = out_column
-        else:
-            result_out_column = self.__repr__()
-
-        super().__init__(
-            transform=_OneSegmentLogTransform(
-                in_column=in_column, base=base, inplace=inplace, out_column=result_out_column
+            features = df.loc[:, pd.IndexSlice[:, self.in_column]]
+            transformed_features = features - self.value
+            result = set_columns_wide(
+                result, transformed_features, features_left=[self.in_column], features_right=[self.in_column]
             )
-        )
+            if self.in_column == "target":
+                segment_columns = result.columns.get_level_values("feature").tolist()
+                quantiles = match_target_quantiles(set(segment_columns))
+                for quantile_column_nm in quantiles:
+                    features = df.loc[:, pd.IndexSlice[:, quantile_column_nm]]
+                    transformed_features = features - self.value
+                    result = set_columns_wide(
+                        result,
+                        transformed_features,
+                        features_left=[quantile_column_nm],
+                        features_right=[quantile_column_nm],
+                    )
+
+        return result
+
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        if self.in_column_regressor is None:
+            raise ValueError("Fit the transform to get the correct regressors info!")
+        return [self._get_column_name()] if self.in_column_regressor and not self.inplace else []
 
 
-__all__ = ["LogTransform"]
+__all__ = ["AddConstTransform"]
```

### Comparing `etna-1.9.0/etna/transforms/math/scalers.py` & `etna-2.0.0/etna/transforms/math/scalers.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         ValueError:
             if incorrect mode given
         """
         self.with_mean = with_mean
         self.with_std = with_std
         super().__init__(
             in_column=in_column,
-            transformer=StandardScaler(with_mean=self.with_mean, with_std=self.with_std, copy=True),
+            transformer=StandardScaler(with_mean=self.with_mean, with_std=self.with_std, copy=False),
             out_column=out_column,
             inplace=inplace,
             mode=mode,
         )
 
 
 class RobustScalerTransform(SklearnTransform):
@@ -136,15 +136,15 @@
             inplace=inplace,
             out_column=out_column,
             transformer=RobustScaler(
                 with_centering=self.with_centering,
                 with_scaling=self.with_scaling,
                 quantile_range=self.quantile_range,
                 unit_variance=self.unit_variance,
-                copy=True,
+                copy=False,
             ),
             mode=mode,
         )
 
 
 class MinMaxScalerTransform(SklearnTransform):
     """Transform features by scaling each feature to a given range.
@@ -195,15 +195,15 @@
         """
         self.feature_range = feature_range
         self.clip = clip
         super().__init__(
             in_column=in_column,
             inplace=inplace,
             out_column=out_column,
-            transformer=MinMaxScaler(feature_range=self.feature_range, clip=self.clip, copy=True),
+            transformer=MinMaxScaler(feature_range=self.feature_range, clip=self.clip, copy=False),
             mode=mode,
         )
 
 
 class MaxAbsScalerTransform(SklearnTransform):
     """Scale each feature by its maximum absolute value.
 
@@ -244,13 +244,13 @@
         ValueError:
             if incorrect mode given
         """
         super().__init__(
             in_column=in_column,
             inplace=inplace,
             out_column=out_column,
-            transformer=MaxAbsScaler(copy=True),
+            transformer=MaxAbsScaler(copy=False),
             mode=mode,
         )
 
 
 __all__ = ["MaxAbsScalerTransform", "MinMaxScalerTransform", "RobustScalerTransform", "StandardScalerTransform"]
```

### Comparing `etna-1.9.0/etna/transforms/math/statistics.py` & `etna-2.0.0/etna/transforms/math/statistics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from abc import ABC
 from abc import abstractmethod
+from typing import List
 from typing import Optional
 
 import bottleneck as bn
 import numpy as np
 import pandas as pd
 
-from etna.transforms.base import Transform
+from etna.datasets import TSDataset
+from etna.transforms.base import IrreversibleTransform
 
 
-class WindowStatisticsTransform(Transform, ABC):
+class WindowStatisticsTransform(IrreversibleTransform, ABC):
     """WindowStatisticsTransform handles computation of statistical features on windows."""
 
     def __init__(
         self,
         in_column: str,
         out_column: str,
         window: int,
@@ -36,32 +38,40 @@
             seasonality of lags to compute window's aggregation with
         min_periods: int
             min number of targets in window to compute aggregation;
             if there is less than ``min_periods`` number of targets return None
         fillna: float
             value to fill results NaNs with
         """
+        super().__init__(required_features=[in_column])
         self.in_column = in_column
         self.out_column_name = out_column
         self.window = window
         self.seasonality = seasonality
         self.min_periods = min_periods
         self.fillna = fillna
         self.kwargs = kwargs
+        self.in_column_regressor: Optional[bool] = None
 
-    def fit(self, *args) -> "WindowStatisticsTransform":
+    def fit(self, ts: TSDataset) -> "WindowStatisticsTransform":
+        """Fit the transform."""
+        self.in_column_regressor = self.in_column in ts.regressors
+        super().fit(ts)
+        return self
+
+    def _fit(self, df: pd.DataFrame) -> "WindowStatisticsTransform":
         """Fits transform."""
         return self
 
     @abstractmethod
     def _aggregate(self, series: np.ndarray) -> np.ndarray:
         """Aggregate targets from given series."""
         pass
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """Compute feature's value.
 
         Parameters
         ----------
         df: pd.DataFrame
             dataframe to generate features for
 
@@ -69,15 +79,16 @@
         -------
         result: pd.DataFrame
             dataframe with results
         """
         history = self.seasonality * self.window if self.window != -1 else len(df)
         segments = sorted(df.columns.get_level_values("segment").unique())
 
-        x = df.loc[pd.IndexSlice[:], pd.IndexSlice[segments, self.in_column]].values[::-1]
+        df_slice = df.loc[:, pd.IndexSlice[:, self.in_column]].sort_index(axis=1)
+        x = df_slice.values[::-1]
 
         # Addend NaNs to obtain a window of length "history" for each point
         x = np.append(x, np.empty((history - 1, x.shape[1])) * np.nan, axis=0)
         isnan = np.isnan(x)
 
         isnan = np.lib.stride_tricks.sliding_window_view(isnan, window_shape=(history, 1))[:, :, :: self.seasonality]
         isnan = np.squeeze(isnan, axis=-1)  # (len(df), n_segments, window)
@@ -91,14 +102,20 @@
 
         result = df.join(
             pd.DataFrame(y, columns=pd.MultiIndex.from_product([segments, [self.out_column_name]]), index=df.index)
         )
         result = result.sort_index(axis=1)
         return result
 
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        if self.in_column_regressor is None:
+            raise ValueError("Fit the transform to get the correct regressors info!")
+        return [self.out_column_name] if self.in_column_regressor else []
+
 
 class MeanTransform(WindowStatisticsTransform):
     """MeanTransform computes average value for given window.
 
     .. math::
        MeanTransform(x_t) = \\sum_{i=1}^{window}{x_{t - i}\\cdot\\alpha^{i - 1}}
     """
@@ -146,31 +163,31 @@
             window=window,
             seasonality=seasonality,
             min_periods=min_periods,
             out_column=self.out_column if self.out_column is not None else self.__repr__(),
             fillna=fillna,
         )
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """Compute feature's value.
 
         Parameters
         ----------
         df: pd.DataFrame
             dataframe to generate features for
 
         Returns
         -------
         result: pd.DataFrame
             dataframe with results
         """
         window = self.window if self.window != -1 else len(df)
-        self._alpha_range = np.array([self.alpha ** i for i in range(window)])
+        self._alpha_range = np.array([self.alpha**i for i in range(window)])
         self._alpha_range = np.expand_dims(self._alpha_range, axis=0)  # (1, window)
-        return super().transform(df)
+        return super()._transform(df)
 
     def _aggregate(self, series: np.ndarray) -> np.ndarray:
         """Compute weighted average for window series."""
         mean = np.zeros((series.shape[0], series.shape[1]))
         for segment in range(mean.shape[1]):
             # Loop prevents from memory overflow, 3d tensor is materialized after multiplication
             mean[:, segment] = bn.nanmean(series[:, segment] * self._alpha_range, axis=1)
@@ -499,17 +516,124 @@
         for segment in range(mad.shape[1]):
             # Loop prevents from memory overflow, 3d tensor is materialized after multiplication
             ad = np.abs(series[:, segment] - mean[:, segment])
             mad[:, segment] = bn.nanmean(ad, axis=1)
         return mad
 
 
+class MinMaxDifferenceTransform(WindowStatisticsTransform):
+    """MinMaxDifferenceTransform computes difference between max and min values for given window."""
+
+    def __init__(
+        self,
+        in_column: str,
+        window: int,
+        seasonality: int = 1,
+        min_periods: int = 1,
+        fillna: float = 0,
+        out_column: Optional[str] = None,
+    ):
+        """Init MaxTransform.
+
+        Parameters
+        ----------
+        in_column: str
+            name of processed column
+        window: int
+            size of window to aggregate
+        seasonality: int
+            seasonality of lags to compute window's aggregation with
+        min_periods: int
+            min number of targets in window to compute aggregation;
+            if there is less than ``min_periods`` number of targets return None
+        fillna: float
+            value to fill results NaNs with
+        out_column: str, optional
+            result column name. If not given use ``self.__repr__()``
+        """
+        self.in_column = in_column
+        self.window = window
+        self.seasonality = seasonality
+        self.min_periods = min_periods
+        self.fillna = fillna
+        self.out_column = out_column
+        super().__init__(
+            window=window,
+            in_column=in_column,
+            seasonality=seasonality,
+            min_periods=min_periods,
+            out_column=self.out_column if self.out_column is not None else self.__repr__(),
+            fillna=fillna,
+        )
+
+    def _aggregate(self, series: np.ndarray) -> np.ndarray:
+        """Compute max over the series."""
+        max_values = bn.nanmax(series, axis=2)
+        min_values = bn.nanmin(series, axis=2)
+        result = max_values - min_values
+        return result
+
+
+class SumTransform(WindowStatisticsTransform):
+    """SumTransform computes sum of values over given window."""
+
+    def __init__(
+        self,
+        in_column: str,
+        window: int,
+        seasonality: int = 1,
+        min_periods: int = 1,
+        fillna: float = 0,
+        out_column: Optional[str] = None,
+    ):
+        """Init SumTransform.
+
+        Parameters
+        ----------
+        in_column:
+            name of processed column
+        window:
+            size of window to aggregate, if window == -1 compute rolling sum all over the given series
+        seasonality:
+            seasonality of lags to compute window's aggregation with
+        min_periods:
+            min number of targets in window to compute aggregation;
+            if there is less than ``min_periods`` number of targets return None
+        fillna:
+            value to fill results NaNs with
+        out_column:
+            result column name. If not given use ``self.__repr__()``
+        """
+        self.in_column = in_column
+        self.window = window
+        self.seasonality = seasonality
+        self.min_periods = min_periods
+        self.fillna = fillna
+        self.out_column = out_column
+
+        super().__init__(
+            in_column=in_column,
+            out_column=self.out_column if self.out_column is not None else self.__repr__(),
+            window=window,
+            seasonality=seasonality,
+            min_periods=min_periods,
+            fillna=fillna,
+        )
+
+    def _aggregate(self, series: np.ndarray) -> np.ndarray:
+        """Compute sum over the series."""
+        series = bn.nansum(series, axis=2)
+        return series
+
+
 __all__ = [
     "MedianTransform",
     "MaxTransform",
     "MinTransform",
     "QuantileTransform",
     "StdTransform",
     "MeanTransform",
     "WindowStatisticsTransform",
     "MADTransform",
+    "MinMaxDifferenceTransform",
+    "SumTransform",
 ]
```

### Comparing `etna-1.9.0/etna/transforms/missing_values/imputation.py` & `etna-2.0.0/etna/transforms/missing_values/imputation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,83 +1,94 @@
 from enum import Enum
 from typing import List
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 
-from etna.transforms.base import PerSegmentWrapper
-from etna.transforms.base import Transform
+from etna.transforms.base import OneSegmentTransform
+from etna.transforms.base import ReversiblePerSegmentWrapper
 
 
 class ImputerMode(str, Enum):
     """Enum for different imputation strategy."""
 
-    zero = "zero"
     mean = "mean"
     running_mean = "running_mean"
     forward_fill = "forward_fill"
     seasonal = "seasonal"
+    constant = "constant"
 
 
-class _OneSegmentTimeSeriesImputerTransform(Transform):
+class _OneSegmentTimeSeriesImputerTransform(OneSegmentTransform):
     """One segment version of transform to fill NaNs in series of a given dataframe.
 
     - It is assumed that given series begins with first non NaN value.
 
     - This transform can't fill NaNs in the future, only on train data.
 
     - This transform can't fill NaNs if all values are NaNs. In this case exception is raised.
 
     """
 
-    def __init__(self, in_column: str, strategy: str, window: int, seasonality: int, default_value: Optional[float]):
+    def __init__(
+        self,
+        in_column: str,
+        strategy: str,
+        window: int,
+        seasonality: int,
+        default_value: Optional[float],
+        constant_value: float = 0,
+    ):
         """
         Create instance of _OneSegmentTimeSeriesImputerTransform.
 
         Parameters
         ----------
         in_column:
             name of processed column
         strategy:
             filling value in missing timestamps:
 
-            - If "zero", then replace missing dates with zeros
-
             - If "mean", then replace missing dates using the mean in fit stage.
 
             - If "running_mean" then replace missing dates using mean of subset of data
 
             - If "forward_fill" then replace missing dates using last existing value
 
             - If "seasonal" then replace missing dates using seasonal moving average
 
+            - If "constant" then replace missing dates using constant value.
+
         window:
             In case of moving average and seasonality.
 
             * If ``window=-1`` all previous dates are taken in account
 
             * Otherwise only window previous dates
 
         seasonality:
             the length of the seasonality
         default_value:
             value which will be used to impute the NaNs left after applying the imputer with the chosen strategy
+        constant_value:
+            value to fill gaps in "constant" strategy
 
         Raises
         ------
         ValueError:
             if incorrect strategy given
         """
         self.in_column = in_column
         self.strategy = ImputerMode(strategy)
         self.window = window
         self.seasonality = seasonality
         self.default_value = default_value
-        self.fill_value: Optional[int] = None
+        self.constant_value = constant_value
+        self.fill_value: Optional[float] = None
         self.nan_timestamps: Optional[List[pd.Timestamp]] = None
 
     def fit(self, df: pd.DataFrame) -> "_OneSegmentTimeSeriesImputerTransform":
         """
         Fit preprocess params.
 
         Parameters
@@ -91,16 +102,16 @@
             fitted preprocess
         """
         raw_series = df[self.in_column]
         if np.all(raw_series.isna()):
             raise ValueError("Series hasn't non NaN values which means it is empty and can't be filled.")
         series = raw_series[raw_series.first_valid_index() :]
         self.nan_timestamps = series[series.isna()].index
-        if self.strategy == ImputerMode.zero:
-            self.fill_value = 0
+        if self.strategy == ImputerMode.constant:
+            self.fill_value = self.constant_value
         elif self.strategy == ImputerMode.mean:
             self.fill_value = series.mean()
         return self
 
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Transform given series.
@@ -111,15 +122,15 @@
             transform ``in_column`` series of given dataframe
 
         Returns
         -------
         result: pd.DataFrame
             dataframe with in_column series with filled gaps
         """
-        result_df = df.copy()
+        result_df = df
         cur_nans = result_df[result_df[self.in_column].isna()].index
 
         result_df[self.in_column] = self._fill(result_df[self.in_column])
 
         # restore nans not in self.nan_timestamps
         restore_nans = cur_nans.difference(self.nan_timestamps)
         result_df.loc[restore_nans, self.in_column] = np.nan
@@ -136,15 +147,15 @@
             inverse transform ``in_column`` series of given dataframe
 
         Returns
         -------
         result: pd.DataFrame
             dataframe with in_column series with initial values
         """
-        result_df = df.copy()
+        result_df = df
         index = result_df.index.intersection(self.nan_timestamps)
         result_df.loc[index, self.in_column] = np.nan
         return result_df
 
     def _fill(self, df: pd.Series) -> pd.Series:
         """
         Create new Series taking all previous dates and adding missing dates.
@@ -159,15 +170,15 @@
         Returns
         -------
         result: pd.Series
         """
         if self.nan_timestamps is None:
             raise ValueError("Trying to apply the unfitted transform! First fit the transform.")
 
-        if self.strategy == ImputerMode.zero or self.strategy == ImputerMode.mean:
+        if self.strategy == ImputerMode.mean or self.strategy == ImputerMode.constant:
             df = df.fillna(value=self.fill_value)
         elif self.strategy == ImputerMode.forward_fill:
             df = df.fillna(method="ffill")
         elif self.strategy == ImputerMode.running_mean or self.strategy == ImputerMode.seasonal:
             history = self.seasonality * self.window if self.window != -1 else len(df)
             timestamps = list(df.index)
             for timestamp in self.nan_timestamps:
@@ -177,15 +188,15 @@
                 df.iloc[i] = np.nanmean(df.iloc[indexes])
 
         if self.default_value:
             df = df.fillna(value=self.default_value)
         return df
 
 
-class TimeSeriesImputerTransform(PerSegmentWrapper):
+class TimeSeriesImputerTransform(ReversiblePerSegmentWrapper):
     """Transform to fill NaNs in series of a given dataframe.
 
     - It is assumed that given series begins with first non NaN value.
 
     - This transform can't fill NaNs in the future, only on train data.
 
     - This transform can't fill NaNs if all values are NaNs. In this case exception is raised.
@@ -195,66 +206,76 @@
     This transform can suffer from look-ahead bias in 'mean' mode. For transforming data at some timestamp
     it uses information from the whole train part.
     """
 
     def __init__(
         self,
         in_column: str = "target",
-        strategy: str = ImputerMode.zero,
+        strategy: str = ImputerMode.constant,
         window: int = -1,
         seasonality: int = 1,
         default_value: Optional[float] = None,
+        constant_value: float = 0,
     ):
         """
         Create instance of TimeSeriesImputerTransform.
 
         Parameters
         ----------
         in_column:
             name of processed column
         strategy:
             filling value in missing timestamps:
 
-            - If "zero", then replace missing dates with zeros
-
             - If "mean", then replace missing dates using the mean in fit stage.
 
             - If "running_mean" then replace missing dates using mean of subset of data
 
             - If "forward_fill" then replace missing dates using last existing value
 
             - If "seasonal" then replace missing dates using seasonal moving average
 
+            - If "constant" then replace missing dates using constant value.
+
         window:
             In case of moving average and seasonality.
 
             * If ``window=-1`` all previous dates are taken in account
 
             * Otherwise only window previous dates
 
         seasonality:
             the length of the seasonality
         default_value:
             value which will be used to impute the NaNs left after applying the imputer with the chosen strategy
+        constant_value:
+            value to fill gaps in "constant" strategy
 
         Raises
         ------
         ValueError:
             if incorrect strategy given
         """
         self.in_column = in_column
         self.strategy = strategy
         self.window = window
         self.seasonality = seasonality
         self.default_value = default_value
+        self.constant_value = constant_value
         super().__init__(
             transform=_OneSegmentTimeSeriesImputerTransform(
                 in_column=self.in_column,
                 strategy=self.strategy,
                 window=self.window,
                 seasonality=self.seasonality,
                 default_value=self.default_value,
-            )
+                constant_value=self.constant_value,
+            ),
+            required_features=[self.in_column],
         )
 
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        return []
+
 
 __all__ = ["TimeSeriesImputerTransform"]
```

### Comparing `etna-1.9.0/etna/transforms/missing_values/resample.py` & `etna-2.0.0/etna/transforms/missing_values/resample.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import warnings
 from typing import List
 from typing import Optional
 
 import pandas as pd
 
-from etna.transforms.base import PerSegmentWrapper
-from etna.transforms.base import Transform
+from etna.datasets import TSDataset
+from etna.transforms.base import IrreversiblePerSegmentWrapper
+from etna.transforms.base import OneSegmentTransform
 
 
-class _OneSegmentResampleWithDistributionTransform(Transform):
+class _OneSegmentResampleWithDistributionTransform(OneSegmentTransform):
     """_OneSegmentResampleWithDistributionTransform resamples the given column using the distribution of the other column."""
 
-    def __init__(self, in_column: str, distribution_column: str, inplace: bool, out_column: Optional[str]):
+    def __init__(self, in_column: str, distribution_column: str, inplace: bool, out_column: str):
         """
         Init _OneSegmentResampleWithDistributionTransform.
 
         Parameters
         ----------
         in_column:
             name of column to be resampled
@@ -30,15 +31,15 @@
         out_column:
             name of added column. If not given, use ``self.__repr__()``
         """
         self.in_column = in_column
         self.distribution_column = distribution_column
         self.inplace = inplace
         self.out_column = out_column
-        self.distribution: pd.DataFrame = None
+        self.distribution: Optional[pd.DataFrame] = None
 
     def _get_folds(self, df: pd.DataFrame) -> List[int]:
         """
         Generate fold number for each timestamp of the dataframe.
 
         Here the ``in_column`` frequency gap is divided into the folds with the size of dataset frequency gap.
         """
@@ -52,15 +53,15 @@
         dataset_freq = df.index[1] - df.index[0]
         n_folds_per_gap = in_column_freq // dataset_freq
         n_periods = len(df) // n_folds_per_gap + 2
 
         in_column_start_index = in_column_index[0]
         left_tie_len = len(df[:in_column_start_index]) - 1
         right_tie_len = len(df[in_column_start_index:])
-        folds_for_left_tie = [fold for fold in range(n_folds_per_gap - left_tie_len, n_folds_per_gap)]
+        folds_for_left_tie = list(range(n_folds_per_gap - left_tie_len, n_folds_per_gap))
         folds_for_right_tie = [fold for _ in range(n_periods) for fold in range(n_folds_per_gap)][:right_tie_len]
         return folds_for_left_tie + folds_for_right_tie
 
     def fit(self, df: pd.DataFrame) -> "_OneSegmentResampleWithDistributionTransform":
         """
         Obtain the resampling frequency and distribution from ``distribution_column``.
 
@@ -97,16 +98,20 @@
         """
         df["fold"] = self._get_folds(df)
         df = df.reset_index().merge(self.distribution, on="fold").set_index("timestamp").sort_index()
         df[self.out_column] = df[self.in_column].ffill() * df["distribution"]
         df = df.drop(["fold", "distribution"], axis=1)
         return df
 
+    def inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Inverse transform Dataframe."""
+        return df
+
 
-class ResampleWithDistributionTransform(PerSegmentWrapper):
+class ResampleWithDistributionTransform(IrreversiblePerSegmentWrapper):
     """ResampleWithDistributionTransform resamples the given column using the distribution of the other column.
 
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
     it uses information from the whole train part.
     """
@@ -132,25 +137,41 @@
         out_column:
             name of added column. If not given, use ``self.__repr__()``
         """
         self.in_column = in_column
         self.distribution_column = distribution_column
         self.inplace = inplace
         self.out_column = self._get_out_column(out_column)
+        self.in_column_regressor: Optional[bool] = None
         super().__init__(
             transform=_OneSegmentResampleWithDistributionTransform(
                 in_column=in_column,
                 distribution_column=distribution_column,
                 inplace=inplace,
                 out_column=self.out_column,
-            )
+            ),
+            required_features=[in_column, distribution_column],
         )
 
     def _get_out_column(self, out_column: Optional[str]) -> str:
         """Get the `out_column` depending on the transform's parameters."""
         if self.inplace and out_column:
             warnings.warn("Transformation will be applied inplace, out_column param will be ignored")
         if self.inplace:
             return self.in_column
         if out_column:
             return out_column
         return self.__repr__()
+
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        if self.in_column_regressor is None:
+            raise ValueError("Fit the transform to get the correct regressors info!")
+        if self.inplace:
+            return []
+        return [self.out_column] if self.in_column_regressor else []
+
+    def fit(self, ts: TSDataset) -> "ResampleWithDistributionTransform":
+        """Fit the transform."""
+        self.in_column_regressor = self.in_column in ts.regressors
+        super().fit(ts)
+        return self
```

### Comparing `etna-1.9.0/etna/transforms/outliers/base.py` & `etna-2.0.0/etna/transforms/outliers/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,32 +4,45 @@
 from typing import List
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 
 from etna.datasets import TSDataset
-from etna.transforms.base import Transform
+from etna.transforms.base import ReversibleTransform
+from etna.transforms.utils import check_new_segments
 
 
-class OutliersTransform(Transform, ABC):
+class OutliersTransform(ReversibleTransform, ABC):
     """Finds outliers in specific columns of DataFrame and replaces it with NaNs."""
 
     def __init__(self, in_column: str):
         """
         Create instance of OutliersTransform.
 
         Parameters
         ----------
         in_column:
             name of processed column
         """
+        super().__init__(required_features=[in_column])
         self.in_column = in_column
         self.outliers_timestamps: Optional[Dict[str, List[pd.Timestamp]]] = None
         self.original_values: Optional[Dict[str, List[pd.Timestamp]]] = None
+        self._fit_segments: Optional[List[str]] = None
+
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform.
+
+        Returns
+        -------
+        :
+            List with regressors created by the transform.
+        """
+        return []
 
     def _save_original_values(self, ts: TSDataset):
         """
         Save values to be replaced with NaNs.
 
         Parameters
         ----------
@@ -40,15 +53,15 @@
             raise ValueError("Something went wrong during outliers detection stage! Check the transform parameters.")
         self.original_values = dict()
         for segment, timestamps in self.outliers_timestamps.items():
             segment_ts = ts[:, segment, :]
             segment_values = segment_ts[segment_ts.index.isin(timestamps)].droplevel("segment", axis=1)[self.in_column]
             self.original_values[segment] = segment_values
 
-    def fit(self, df: pd.DataFrame) -> "OutliersTransform":
+    def _fit(self, df: pd.DataFrame) -> "OutliersTransform":
         """
         Find outliers using detection method.
 
         Parameters
         ----------
         df:
             dataframe with series to find outliers
@@ -57,59 +70,78 @@
         -------
         result: OutliersTransform
             instance with saved outliers
         """
         ts = TSDataset(df, freq=pd.infer_freq(df.index))
         self.outliers_timestamps = self.detect_outliers(ts)
         self._save_original_values(ts)
+        self._fit_segments = ts.segments
 
         return self
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Replace found outliers with NaNs.
 
         Parameters
         ----------
         df:
             transform ``in_column`` series of given dataframe
 
         Returns
         -------
-        result: pd.DataFrame
+        result:
             dataframe with in_column series with filled with NaNs
+
+        Raises
+        ------
+        ValueError:
+            If transform isn't fitted.
+        NotImplementedError:
+            If there are segments that weren't present during training.
         """
         if self.outliers_timestamps is None:
             raise ValueError("Transform is not fitted! Fit the Transform before calling transform method.")
-        result_df = df.copy()
-        for segment in df.columns.get_level_values("segment").unique():
-            result_df.loc[self.outliers_timestamps[segment], pd.IndexSlice[segment, self.in_column]] = np.NaN
-        return result_df
+        segments = df.columns.get_level_values("segment").unique().tolist()
+        check_new_segments(transform_segments=segments, fit_segments=self._fit_segments)
+        for segment in segments:
+            # to locate only present indices
+            segment_outliers_timestamps = df.index.intersection(self.outliers_timestamps[segment])
+            df.loc[segment_outliers_timestamps, pd.IndexSlice[segment, self.in_column]] = np.NaN
+        return df
 
-    def inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Inverse transformation. Returns back deleted values.
 
         Parameters
         ----------
         df:
             data to transform
 
         Returns
         -------
-        result: pd.DataFrame
+        result:
             data with reconstructed values
+
+        Raises
+        ------
+        ValueError:
+            If transform isn't fitted.
+        NotImplementedError:
+            If there are segments that weren't present during training.
         """
         if self.original_values is None or self.outliers_timestamps is None:
             raise ValueError("Transform is not fitted! Fit the Transform before calling inverse_transform method.")
-        result = df.copy()
-        for segment in self.original_values.keys():
-            segment_ts = result[segment, self.in_column]
+        segments = df.columns.get_level_values("segment").unique().tolist()
+        check_new_segments(transform_segments=segments, fit_segments=self._fit_segments)
+        for segment in segments:
+            segment_ts = df[segment, self.in_column]
             segment_ts[segment_ts.index.isin(self.outliers_timestamps[segment])] = self.original_values[segment]
-        return result
+        return df
 
     @abstractmethod
     def detect_outliers(self, ts: TSDataset) -> Dict[str, List[pd.Timestamp]]:
         """Call function for detection outliers with self parameters.
 
         Parameters
         ----------
```

### Comparing `etna-1.9.0/etna/transforms/outliers/point_outliers.py` & `etna-2.0.0/etna/transforms/outliers/point_outliers.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,19 @@
 
         Returns
         -------
         :
             dict of outliers in format {segment: [outliers_timestamps]}
         """
         return get_anomalies_prediction_interval(
-            ts=ts, model=self.model, interval_width=self.interval_width, in_column=self.in_column, **self.model_kwargs
+            ts=ts,
+            model=self.model,
+            interval_width=self.interval_width,
+            in_column=self.in_column,
+            **self.model_kwargs,
         )
 
 
 __all__ = [
     "MedianOutliersTransform",
     "DensityOutliersTransform",
     "PredictionIntervalOutliersTransform",
```

### Comparing `etna-1.9.0/etna/transforms/timestamp/date_flags.py` & `etna-2.0.0/etna/transforms/timestamp/date_flags.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from copy import deepcopy
 from math import ceil
+from typing import List
 from typing import Optional
 from typing import Sequence
 
 import numpy as np
 import pandas as pd
 
 from etna.transforms.base import FutureMixin
-from etna.transforms.base import Transform
+from etna.transforms.base import IrreversibleTransform
 
 
-class DateFlagsTransform(Transform, FutureMixin):
+class DateFlagsTransform(IrreversibleTransform, FutureMixin):
     """DateFlagsTransform is a class that implements extraction of the main date-based features from datetime column.
 
     Notes
     -----
     Small example of ``week_number_in_month`` and ``week_number_in_year`` features
 
     =============  ======================  ========================  ========================
@@ -99,15 +100,15 @@
         ):
             raise ValueError(
                 f"{type(self).__name__} feature does nothing with given init args configuration, "
                 f"at least one of day_number_in_week, day_number_in_month, day_number_in_year, week_number_in_month, "
                 f"week_number_in_year, month_number_in_year, season_number, year_number, is_weekend should be True or any of "
                 f"special_days_in_week, special_days_in_month should be not empty."
             )
-
+        super().__init__(required_features=["target"])
         self.day_number_in_week = day_number_in_week
         self.day_number_in_month = day_number_in_month
         self.day_number_in_year = day_number_in_year
         self.week_number_in_month = week_number_in_month
         self.week_number_in_year = week_number_in_year
         self.month_number_in_year = month_number_in_year
         self.season_number = season_number
@@ -133,25 +134,45 @@
             special_days_in_week=(),
             special_days_in_month=(),
         )
 
     def _get_column_name(self, feature_name: str) -> str:
         if self.out_column is None:
             init_parameters = deepcopy(self._empty_parameters)
-            init_parameters[feature_name] = self.__dict__[feature_name]
+            init_parameters[feature_name] = getattr(self, feature_name)
             temp_transform = DateFlagsTransform(**init_parameters, out_column=self.out_column)  # type: ignore
             return temp_transform.__repr__()
         else:
             return f"{self.out_column}_{feature_name}"
 
-    def fit(self, *args) -> "DateFlagsTransform":
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        features = [
+            "day_number_in_week",
+            "day_number_in_month",
+            "day_number_in_year",
+            "week_number_in_month",
+            "week_number_in_year",
+            "month_number_in_year",
+            "season_number",
+            "year_number",
+            "is_weekend",
+            "special_days_in_week",
+            "special_days_in_month",
+        ]
+        output_columns = [
+            self._get_column_name(feature_name=feature_name) for feature_name in features if getattr(self, feature_name)
+        ]
+        return output_columns
+
+    def _fit(self, df: pd.DataFrame) -> "DateFlagsTransform":
         """Fit model. In this case of DateFlags does nothing."""
         return self
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """Get required features from df.
 
         Parameters
         ----------
         df:
             dataframe for feature extraction, should contain 'timestamp' column
```

### Comparing `etna-1.9.0/etna/transforms/timestamp/fourier.py` & `etna-2.0.0/etna/transforms/timestamp/fourier.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import math
+from typing import List
 from typing import Optional
 from typing import Sequence
 
 import numpy as np
 import pandas as pd
 
 from etna.transforms.base import FutureMixin
-from etna.transforms.base import Transform
+from etna.transforms.base import IrreversibleTransform
 
 
-class FourierTransform(Transform, FutureMixin):
+class FourierTransform(IrreversibleTransform, FutureMixin):
     """Adds fourier features to the dataset.
 
     Notes
     -----
     To understand how transform works we recommend:
     `Fourier series <https://otexts.com/fpp2/useful-predictors.html#fourier-series>`_.
 
@@ -79,52 +80,58 @@
             self.mods = [mod for mod in range(1, 2 * order + 1) if mod < period]
         elif mods is not None and order is None:
             if min(mods) < 1 or max(mods) >= period:
                 raise ValueError("Every mod should be within [1, int(period)) range")
             self.mods = mods
         else:
             raise ValueError("There should be exactly one option set: order or mods")
-
+        self.order = None
         self.out_column = out_column
+        super().__init__(required_features=["target"])
+
+    def _get_column_name(self, mod: int) -> str:
+        if self.out_column is None:
+            return f"{FourierTransform(period=self.period, mods=[mod]).__repr__()}"
+        else:
+            return f"{self.out_column}_{mod}"
 
-    def fit(self, df: pd.DataFrame) -> "FourierTransform":
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        output_columns = [self._get_column_name(mod=mod) for mod in self.mods]
+        return output_columns
+
+    def _fit(self, df: pd.DataFrame) -> "FourierTransform":
         """Fit method does nothing and is kept for compatibility.
 
         Parameters
         ----------
         df:
             dataframe with data.
 
         Returns
         -------
         result: FourierTransform
         """
         return self
 
-    def _get_column_name(self, mod: int) -> str:
-        if self.out_column is None:
-            return f"{FourierTransform(period=self.period, mods=[mod]).__repr__()}"
-        else:
-            return f"{self.out_column}_{mod}"
-
     @staticmethod
     def _construct_answer(df: pd.DataFrame, features: pd.DataFrame) -> pd.DataFrame:
         dataframes = []
         for seg in df.columns.get_level_values("segment").unique():
             tmp = df[seg].join(features)
             _idx = tmp.columns.to_frame()
             _idx.insert(0, "segment", seg)
             tmp.columns = pd.MultiIndex.from_frame(_idx)
             dataframes.append(tmp)
 
         result = pd.concat(dataframes, axis=1).sort_index(axis=1)
         result.columns.names = ["segment", "feature"]
         return result
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """Add harmonics to the dataset.
 
         Parameters
         ----------
         df:
             dataframe with data to transform.
```

### Comparing `etna-1.9.0/etna/transforms/timestamp/holiday.py` & `etna-2.0.0/etna/transforms/timestamp/holiday.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 import datetime
+from typing import List
 from typing import Optional
 
 import holidays
 import numpy as np
 import pandas as pd
 
 from etna.transforms.base import FutureMixin
-from etna.transforms.base import Transform
+from etna.transforms.base import IrreversibleTransform
 
 
-class HolidayTransform(Transform, FutureMixin):
+class HolidayTransform(IrreversibleTransform, FutureMixin):
     """HolidayTransform generates series that indicates holidays in given dataframe."""
 
     def __init__(self, iso_code: str = "RUS", out_column: Optional[str] = None):
         """
         Create instance of HolidayTransform.
 
         Parameters
         ----------
         iso_code:
             internationally recognised codes, designated to country for which we want to find the holidays
         out_column:
             name of added column. Use ``self.__repr__()`` if not given.
         """
+        super().__init__(required_features=["target"])
         self.iso_code = iso_code
         self.holidays = holidays.CountryHoliday(iso_code)
         self.out_column = out_column
-        self.out_column = self.out_column if self.out_column is not None else self.__repr__()
 
-    def fit(self, df: pd.DataFrame) -> "HolidayTransform":
+    def _get_column_name(self) -> str:
+        if self.out_column:
+            return self.out_column
+        else:
+            return self.__repr__()
+
+    def _fit(self, df: pd.DataFrame) -> "HolidayTransform":
         """
         Fit HolidayTransform with data from df. Does nothing in this case.
 
         Parameters
         ----------
         df: pd.DataFrame
             value series with index column in timestamp format
         """
         return self
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Transform data from df with HolidayTransform and generate a column of holidays flags.
 
         Parameters
         ----------
         df: pd.DataFrame
             value series with index column in timestamp format
@@ -54,19 +61,29 @@
             pd.DataFrame with added holidays
         """
         if (df.index[1] - df.index[0]) > datetime.timedelta(days=1):
             raise ValueError("Frequency of data should be no more than daily.")
 
         cols = df.columns.get_level_values("segment").unique()
 
+        out_column = self._get_column_name()
         encoded_matrix = np.array([int(x in self.holidays) for x in df.index])
         encoded_matrix = encoded_matrix.reshape(-1, 1).repeat(len(cols), axis=1)
         encoded_df = pd.DataFrame(
             encoded_matrix,
-            columns=pd.MultiIndex.from_product([cols, [self.out_column]], names=("segment", "feature")),
+            columns=pd.MultiIndex.from_product([cols, [out_column]], names=("segment", "feature")),
             index=df.index,
         )
         encoded_df = encoded_df.astype("category")
 
         df = df.join(encoded_df)
         df = df.sort_index(axis=1)
         return df
+
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform.
+        Returns
+        -------
+        :
+            List with regressors created by the transform.
+        """
+        return [self._get_column_name()]
```

### Comparing `etna-1.9.0/etna/transforms/timestamp/special_days.py` & `etna-2.0.0/etna/transforms/timestamp/special_days.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import datetime
+from typing import Any
+from typing import Dict
+from typing import List
 from typing import Optional
 from typing import Tuple
 
 import pandas as pd
 
 from etna.transforms.base import FutureMixin
-from etna.transforms.base import PerSegmentWrapper
-from etna.transforms.base import Transform
+from etna.transforms.base import IrreversiblePerSegmentWrapper
+from etna.transforms.base import OneSegmentTransform
 
 
 def calc_day_number_in_week(datetime_day: datetime.datetime) -> int:
     return datetime_day.weekday()
 
 
 def calc_day_number_in_month(datetime_day: datetime.datetime) -> int:
     return datetime_day.day
 
 
-class _OneSegmentSpecialDaysTransform(Transform):
+class _OneSegmentSpecialDaysTransform(OneSegmentTransform):
     """
     Search for anomalies in values, marked this days as 1 (and return new column with 1 in corresponding places).
 
     Notes
     -----
     You can read more about other anomalies detection methods in:
     `Time Series of Price Anomaly Detection <https://towardsdatascience.com/time-series-of-price-anomaly-detection-13586cd5ff46>`_
@@ -51,22 +54,23 @@
 
         self.find_special_weekday = find_special_weekday
         self.find_special_month_day = find_special_month_day
 
         self.anomaly_week_days: Optional[Tuple[int]] = None
         self.anomaly_month_days: Optional[Tuple[int]] = None
 
+        self.res_type: Dict[str, Any]
         if self.find_special_weekday and find_special_month_day:
             self.res_type = {"df_sample": (0, 0), "columns": ["anomaly_weekdays", "anomaly_monthdays"]}
         elif self.find_special_weekday:
             self.res_type = {"df_sample": 0, "columns": ["anomaly_weekdays"]}
         elif self.find_special_month_day:
             self.res_type = {"df_sample": 0, "columns": ["anomaly_monthdays"]}
         else:
-            assert False, "nothing to do"
+            raise ValueError("nothing to do")
 
     def fit(self, df: pd.DataFrame) -> "_OneSegmentSpecialDaysTransform":
         """
         Fit _OneSegmentSpecialDaysTransform with data from df.
 
         Parameters
         ----------
@@ -112,16 +116,15 @@
         if self.find_special_month_day:
             if self.anomaly_month_days is None:
                 raise ValueError("Transform is not fitted! Fit the Transform before calling transform method.")
             to_add["anomaly_monthdays"] += self._marked_special_month_day(common_df, self.anomaly_month_days)
             to_add["anomaly_monthdays"] = to_add["anomaly_monthdays"].astype("category")
 
         to_add.index = df.index
-        to_return = df.copy()
-        to_return = pd.concat([to_return, to_add], axis=1)
+        to_return = pd.concat([df, to_add], axis=1)
         to_return.columns.names = df.columns.names
         return to_return
 
     @staticmethod
     def _find_anomaly_day_in_week(df: pd.DataFrame, agg_func=pd.core.groupby.SeriesGroupBy.mean) -> Tuple[int]:
         cp_df = df.copy()
 
@@ -161,16 +164,20 @@
         """Mark desired month day in dataframe, return column with original length."""
 
         def check(x):
             return calc_day_number_in_month(x["datetime"]) in month_days
 
         return df.loc[:, ["datetime"]].apply(check, axis=1).rename("anomaly_monthdays")
 
+    def inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Inverse transform Dataframe."""
+        return df
 
-class SpecialDaysTransform(PerSegmentWrapper, FutureMixin):
+
+class SpecialDaysTransform(IrreversiblePerSegmentWrapper, FutureMixin):
     """SpecialDaysTransform generates series that indicates is weekday/monthday is special in given dataframe.
 
     Creates columns 'anomaly_weekdays' and 'anomaly_monthdays'.
 
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
@@ -192,12 +199,22 @@
         ------
         ValueError:
             if all the modes are False
         """
         self.find_special_weekday = find_special_weekday
         self.find_special_month_day = find_special_month_day
         super().__init__(
-            transform=_OneSegmentSpecialDaysTransform(self.find_special_weekday, self.find_special_month_day)
+            transform=_OneSegmentSpecialDaysTransform(self.find_special_weekday, self.find_special_month_day),
+            required_features=["target"],
         )
 
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        output_columns = []
+        if self.find_special_weekday:
+            output_columns.append("anomaly_weekdays")
+        if self.find_special_month_day:
+            output_columns.append("anomaly_monthdays")
+        return output_columns
+
 
 __all__ = ["SpecialDaysTransform"]
```

### Comparing `etna-1.9.0/etna/transforms/timestamp/time_flags.py` & `etna-2.0.0/etna/transforms/timestamp/time_flags.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from copy import deepcopy
+from typing import List
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 
 from etna.transforms.base import FutureMixin
-from etna.transforms.base import Transform
+from etna.transforms.base import IrreversibleTransform
 
 
-class TimeFlagsTransform(Transform, FutureMixin):
+class TimeFlagsTransform(IrreversibleTransform, FutureMixin):
     """TimeFlagsTransform is a class that implements extraction of the main time-based features from datetime column."""
 
     def __init__(
         self,
         minute_in_hour_number: bool = True,
         fifteen_minutes_in_hour_number: bool = False,
         hour_number: bool = True,
@@ -64,15 +65,15 @@
             ]
         ):
             raise ValueError(
                 f"{type(self).__name__} feature does nothing with given init args configuration, "
                 f"at least one of minute_in_hour_number, fifteen_minutes_in_hour_number, hour_number, "
                 f"half_hour_number, half_day_number, one_third_day_number should be True."
             )
-
+        super().__init__(required_features=["target"])
         self.date_column_name = None
         self.minute_in_hour_number: bool = minute_in_hour_number
         self.fifteen_minutes_in_hour_number: bool = fifteen_minutes_in_hour_number
         self.hour_number: bool = hour_number
         self.half_hour_number: bool = half_hour_number
         self.half_day_number: bool = half_day_number
         self.one_third_day_number: bool = one_third_day_number
@@ -88,25 +89,40 @@
             half_day_number=False,
             one_third_day_number=False,
         )
 
     def _get_column_name(self, feature_name: str) -> str:
         if self.out_column is None:
             init_parameters = deepcopy(self._empty_parameters)
-            init_parameters[feature_name] = self.__dict__[feature_name]
+            init_parameters[feature_name] = getattr(self, feature_name)
             temp_transform = TimeFlagsTransform(**init_parameters, out_column=self.out_column)  # type: ignore
             return repr(temp_transform)
         else:
             return f"{self.out_column}_{feature_name}"
 
-    def fit(self, *args, **kwargs) -> "TimeFlagsTransform":
+    def get_regressors_info(self) -> List[str]:
+        """Return the list with regressors created by the transform."""
+        features = [
+            "minute_in_hour_number",
+            "fifteen_minutes_in_hour_number",
+            "hour_number",
+            "half_hour_number",
+            "half_day_number",
+            "one_third_day_number",
+        ]
+        output_columns = [
+            self._get_column_name(feature_name=feature_name) for feature_name in features if getattr(self, feature_name)
+        ]
+        return output_columns
+
+    def _fit(self, *args, **kwargs) -> "TimeFlagsTransform":
         """Fit datetime model."""
         return self
 
-    def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Transform method for features based on time.
 
         Parameters
         ----------
         df:
             Features dataframe with time
```

### Comparing `etna-1.9.0/PKG-INFO` & `etna-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,92 +1,107 @@
 Metadata-Version: 2.1
 Name: etna
-Version: 1.9.0
+Version: 2.0.0
 Summary: ETNA is the first python open source framework of Tinkoff.ru AI Center. It is designed to make working with time series simple, productive, and fun.
 Home-page: https://github.com/tinkoff-ai/etna
 License: Apache-2.0
 Author: Andrey Alekseev
-Author-email: an.alekseev@tinkoff.ru
-Requires-Python: >=3.7.1,<3.10.0
-Classifier: Development Status :: 4 - Beta
+Author-email: ilekseev@gmail.com
+Requires-Python: >=3.8.0,<3.11.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Provides-Extra: all-dev
+Provides-Extra: auto
+Provides-Extra: classification
 Provides-Extra: docs
 Provides-Extra: jupyter
 Provides-Extra: prophet
 Provides-Extra: release
 Provides-Extra: style
 Provides-Extra: tests
 Provides-Extra: torch
 Provides-Extra: wandb
 Requires-Dist: Bottleneck (>=1.3.4,<2.0.0)
-Requires-Dist: GitPython (>=3.1.20,<4.0.0); extra == "docs" or extra == "all-dev"
-Requires-Dist: Sphinx (>=4.1,<5.0); extra == "docs" or extra == "all-dev"
-Requires-Dist: black (==21.9b0); extra == "style" or extra == "all-dev"
+Requires-Dist: Deprecated (==1.2.13)
+Requires-Dist: GitPython (>=3.1.20,<4.0.0) ; extra == "docs" or extra == "all-dev"
+Requires-Dist: Sphinx (>=4.1,<5.0) ; extra == "docs" or extra == "all-dev"
+Requires-Dist: black[jupyter] (>=22.3.0,<23.0.0) ; extra == "jupyter" or extra == "style" or extra == "all-dev"
 Requires-Dist: boto3 (>=1.5,<2.0)
 Requires-Dist: botocore
 Requires-Dist: catboost (>=0.21)
-Requires-Dist: click (>=8.0.1,<8.1); extra == "release" or extra == "all-dev" or extra == "all-dev"
-Requires-Dist: codespell (>=2.0.0,<3.0.0); extra == "style" or extra == "all-dev"
-Requires-Dist: coverage (>=5.4,<6.0); extra == "tests" or extra == "all-dev"
+Requires-Dist: click (>=8.0.1,<8.1) ; extra == "release" or extra == "all-dev" or extra == "all-dev"
+Requires-Dist: codespell (>=2.0.0,<3.0.0) ; extra == "style" or extra == "all-dev"
+Requires-Dist: coverage (>=5.4,<6.0) ; extra == "tests" or extra == "all-dev"
 Requires-Dist: dill (>=0.3.4,<0.4.0)
-Requires-Dist: flake8 (>=3.9.2,<4.0.0); extra == "style" or extra == "all-dev"
-Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0); extra == "style" or extra == "all-dev"
-Requires-Dist: flake8-mutable (>=1.2.0,<2.0.0); extra == "style" or extra == "all-dev"
-Requires-Dist: holidays (>=0.11.3,<0.12.0)
+Requires-Dist: flake8 (>=3.9.2,<4.0.0) ; extra == "style" or extra == "all-dev"
+Requires-Dist: flake8-bugbear (>=22.4.25,<23.0.0) ; extra == "style" or extra == "all-dev"
+Requires-Dist: flake8-comprehensions (>=3.9.0,<4.0.0) ; extra == "style" or extra == "all-dev"
+Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "style" or extra == "all-dev"
+Requires-Dist: holidays (>=0.13,<0.14)
 Requires-Dist: hydra-slayer (>=0.2.0,<0.3.0)
 Requires-Dist: hydra_slayer
 Requires-Dist: ipywidgets (>=7.6.5,<8.0.0)
-Requires-Dist: isort (>=5.8.0,<6.0.0); extra == "style" or extra == "all-dev"
+Requires-Dist: isort (>=5.8.0,<6.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: joblib
-Requires-Dist: jupyter; extra == "jupyter" or extra == "all-dev"
+Requires-Dist: jupyter ; extra == "jupyter" or extra == "all-dev"
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: matplotlib
-Requires-Dist: mypy (>=0.910,<0.911); extra == "style" or extra == "all-dev"
-Requires-Dist: myst-parser (>=0.15.0,<0.16.0); extra == "docs" or extra == "all-dev"
-Requires-Dist: nbconvert; extra == "jupyter" or extra == "all-dev"
-Requires-Dist: nbsphinx (>=0.8.2,<0.9.0); extra == "docs" or extra == "all-dev"
+Requires-Dist: mypy (>=0.950,<0.951) ; extra == "style" or extra == "all-dev"
+Requires-Dist: myst-parser (>=0.15.0,<0.16.0) ; extra == "docs" or extra == "all-dev"
+Requires-Dist: nbconvert ; extra == "jupyter" or extra == "all-dev"
+Requires-Dist: nbsphinx (>=0.8.2,<0.9.0) ; extra == "docs" or extra == "all-dev"
 Requires-Dist: numba (>=0.53.1,<0.56.0)
 Requires-Dist: numpy
-Requires-Dist: numpydoc (>=1.1.0,<2.0.0); extra == "docs" or extra == "all-dev"
+Requires-Dist: numpydoc (>=1.1.0,<2.0.0) ; extra == "docs" or extra == "all-dev"
 Requires-Dist: omegaconf (>=2.1.1,<3.0.0)
-Requires-Dist: pandas (>=1,<2)
-Requires-Dist: pep8-naming (>=0.12.1,<0.13.0); extra == "style" or extra == "all-dev"
+Requires-Dist: optuna (>=2.5.0,<3.0.0) ; extra == "auto" or extra == "all" or extra == "all-dev"
+Requires-Dist: pandas (>=1.1,<2.0)
+Requires-Dist: pep8-naming (>=0.12.1,<0.13.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: plotly
-Requires-Dist: prophet (>=1.0,<2.0); extra == "prophet" or extra == "all" or extra == "all-dev"
-Requires-Dist: pytest (>=6.2,<7.0); extra == "tests" or extra == "all-dev"
-Requires-Dist: pytest-cov (>=2.11.1,<3.0.0); extra == "tests" or extra == "all-dev"
-Requires-Dist: pytorch-forecasting (>=0.9.0,<0.10.0); extra == "torch" or extra == "all" or extra == "all-dev"
-Requires-Dist: pytorch-lightning; extra == "torch"
+Requires-Dist: pmdarima (>=1.8.0)
+Requires-Dist: prophet (>=1.0,<2.0) ; extra == "prophet" or extra == "all" or extra == "all-dev"
+Requires-Dist: pytest (>=6.2,<7.0) ; extra == "tests" or extra == "all-dev"
+Requires-Dist: pytest-cov (>=2.11.1,<3.0.0) ; extra == "tests" or extra == "all-dev"
+Requires-Dist: pytorch-forecasting (>=0.9.0,<0.10.0) ; extra == "torch" or extra == "all" or extra == "all-dev"
+Requires-Dist: pytorch-lightning ; extra == "torch"
+Requires-Dist: pyts (>=0.12.0,<0.13.0) ; extra == "classification" or extra == "all" or extra == "all-dev"
 Requires-Dist: ruptures (==1.1.5)
 Requires-Dist: scikit-learn (>=0.24,<2)
 Requires-Dist: scipy (<1.8.0)
 Requires-Dist: seaborn (>=0.11.1,<0.12.0)
-Requires-Dist: semver (>=2.13.0,<3.0.0); extra == "release" or extra == "all-dev" or extra == "all-dev"
-Requires-Dist: sphinx-mathjax-offline (>=0.0.1,<0.0.2); extra == "docs" or extra == "all-dev"
-Requires-Dist: sphinx-rtd-theme (>=0.5.1,<0.6.0); extra == "docs" or extra == "all-dev"
+Requires-Dist: semver (>=2.13.0,<3.0.0) ; extra == "release" or extra == "all-dev" or extra == "all-dev"
+Requires-Dist: sphinx-mathjax-offline (>=0.0.1,<0.0.2) ; extra == "docs" or extra == "all-dev"
+Requires-Dist: sphinx-rtd-theme (>=0.5.1,<0.6.0) ; extra == "docs" or extra == "all-dev"
 Requires-Dist: statsmodels (>=0.12,<0.14)
+Requires-Dist: tbats (>=1.1.0,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: torch (>=1.8.0,<1.12.0); extra == "torch" or extra == "all" or extra == "all-dev"
+Requires-Dist: torch (>=1.8.0,<1.12.0) ; extra == "torch" or extra == "all" or extra == "all-dev"
 Requires-Dist: typer (>=0.4.0,<0.5.0)
-Requires-Dist: types-PyYAML (>=6.0.0,<7.0.0); extra == "style" or extra == "all-dev"
+Requires-Dist: types-Deprecated (==1.2.9)
+Requires-Dist: types-PyYAML (>=6.0.0,<7.0.0) ; extra == "style" or extra == "all-dev"
+Requires-Dist: types-setuptools (>=65.7.0,<66.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: typing_extensions
-Requires-Dist: wandb (>=0.12.2,<0.13.0); extra == "wandb" or extra == "all" or extra == "all-dev"
+Requires-Dist: wandb (>=0.12.2,<0.13.0) ; extra == "wandb" or extra == "all" or extra == "all-dev"
 Project-URL: Repository, https://github.com/tinkoff-ai/etna
 Description-Content-Type: text/markdown
 
 <div align="center">
 <img src="etna_logo.png" width="100%"/>
 </div>
 
@@ -96,22 +111,21 @@
   <a href="https://pypi.org/project/etna/"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/etna.svg" /></a>
   <a href="https://pypi.org/project/etna/"><img alt="Python versions" src="https://img.shields.io/pypi/pyversions/etna.svg" /></a>
   <a href="https://pepy.tech/project/etna"><img alt="Downloads" src="https://static.pepy.tech/personalized-badge/etna?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" /></a>
 </p>
  
 <p align="center">
   <a href="https://codecov.io/gh/tinkoff-ai/etna"><img alt="Coverage" src="https://img.shields.io/codecov/c/github/tinkoff-ai/etna.svg" /></a>
-  <a href="https://github.com/tinkoff-ai/etna/actions/workflows/test.yml?query=branch%3Amaster++"><img alt="Test passing" src="https://img.shields.io/github/workflow/status/tinkoff-ai/etna/Test/master?label=tests" /></a>
-  <a href="https://github.com/tinkoff-ai/etna/actions/workflows/publish.yml"><img alt="Docs publish" src="https://img.shields.io/github/workflow/status/tinkoff-ai/etna/Publish?label=docs" /></a>
+  <a href="https://github.com/tinkoff-ai/etna/actions/workflows/test.yml?query=branch%3Amaster++"><img alt="Test passing" src="https://img.shields.io/github/actions/workflow/status/tinkoff-ai/etna/test.yml?branch=master&label=tests" /></a>
+  <a href="https://github.com/tinkoff-ai/etna/actions/workflows/publish.yml"><img alt="Docs publish" src="https://img.shields.io/github/actions/workflow/status/tinkoff-ai/etna/publish.yml?label=docs" /></a>
   <a href="https://github.com/tinkoff-ai/etna/blob/master/LICENSE"><img alt="License" src="https://img.shields.io/github/license/tinkoff-ai/etna.svg" /></a>
 </p>
 
 <p align="center">
   <a href="https://t.me/etna_support"><img alt="Telegram" src="https://img.shields.io/badge/channel-telegram-blue" /></a>
-  <a href="https://opendatascience.slack.com/archives/C02Q62NEPH8"><img alt="Slack" src="https://img.shields.io/badge/slack-ods.ai-orange" /></a>
   <a href="https://github.com/tinkoff-ai/etna/discussions"><img alt="GitHub Discussions" src="https://img.shields.io/github/discussions/tinkoff-ai/etna" /></a>
   <a href="https://github.com/tinkoff-ai/etna/graphs/contributors"><img alt="Contributors" src="https://img.shields.io/github/contributors/tinkoff-ai/etna.svg" /></a>
   <a href="https://github.com/tinkoff-ai/etna/stargazers"><img alt="Stars" src="https://img.shields.io/github/stars/tinkoff-ai/etna?style=social" /></a>
 </p>
 
 <p align="center">
   <a href="https://etna.tinkoff.ru">Homepage</a> | 
@@ -153,15 +167,15 @@
 
 # Make train/test split
 train_ts, test_ts = ts.train_test_split(test_size=HORIZON)
 ```
 
 Define transformations and model:
 ```python
-from etna.models import CatBoostModelMultiSegment
+from etna.models import CatBoostMultiSegmentModel
 from etna.transforms import DateFlagsTransform
 from etna.transforms import DensityOutliersTransform
 from etna.transforms import FourierTransform
 from etna.transforms import LagTransform
 from etna.transforms import LinearTrendTransform
 from etna.transforms import MeanTransform
 from etna.transforms import SegmentEncoderTransform
@@ -179,15 +193,15 @@
     FourierTransform(period=360.25, order=6, out_column="fourier"),
     SegmentEncoderTransform(),
     MeanTransform(in_column=f"target_lag_{HORIZON}", window=12, seasonality=7),
     MeanTransform(in_column=f"target_lag_{HORIZON}", window=7),
 ]
 
 # Prepare model
-model = CatBoostModelMultiSegment()
+model = CatBoostMultiSegmentModel()
 ```
 
 Fit `Pipeline` and make a prediction:
 ```python
 from etna.pipeline import Pipeline
 
 # Create and fit the pipeline
@@ -262,62 +276,80 @@
 | [Get started](https://github.com/tinkoff-ai/etna/tree/master/examples/get_started.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/get_started.ipynb) |
 | [Backtest](https://github.com/tinkoff-ai/etna/tree/master/examples/backtest.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/backtest.ipynb) |
 | [EDA](https://github.com/tinkoff-ai/etna/tree/master/examples/EDA.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/EDA.ipynb) |
 | [Outliers](https://github.com/tinkoff-ai/etna/tree/master/examples/outliers.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/outliers.ipynb) |
 | [Clustering](https://github.com/tinkoff-ai/etna/tree/master/examples/clustering.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/clustering.ipynb) |
 | [Deep learning models](https://github.com/tinkoff-ai/etna/tree/master/examples/NN_examples.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/NN_examples.ipynb) |
 | [Ensembles](https://github.com/tinkoff-ai/etna/tree/master/examples/ensembles.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/ensembles.ipynb) |
+| [Custom Transform and Model](https://github.com/tinkoff-ai/etna/tree/master/examples/custom_transform_and_model.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/custom_transform_and_model.ipynb) |
+| [Exogenous data](https://github.com/tinkoff-ai/etna/tree/master/examples/exogenous_data.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/exogenous_data.ipynb) |
+| [Forecasting strategies](https://github.com/tinkoff-ai/etna/blob/master/examples/forecasting_strategies.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/forecasting_strategies.ipynb) |
+| [Classification](https://github.com/tinkoff-ai/etna/blob/master/examples/classification.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/classification.ipynb) |
+| [Hierarchical time series](https://github.com/tinkoff-ai/etna/blob/master/examples/hierarchical_pipeline.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/hierarchical_pipeline.ipynb) |
 
 ## Documentation
 
 ETNA documentation is available [here](https://etna-docs.netlify.app/).
 
 ## Community
 
 To ask the questions or discuss the library you can join our [telegram chat](t.me/etna_support). 
 [Discussions section](https://github.com/tinkoff-ai/etna/discussions) on github is also open for this purpose.
 
 ## Resources
 
 - [Forecasting with ETNA: Fast and Furious](https://medium.com/its-tinkoff/forecasting-with-etna-fast-and-furious-1b58e1453809) on Medium
 
+- [ETNA Regressors](https://medium.com/its-tinkoff/etna-regressors-d2722923e88e) on Medium
+
+- [Time series forecasting with ETNA: first steps](https://medium.com/its-tinkoff/time-series-forecasting-with-etna-first-steps-dfaf90c5b919) on Medium
+
+- [ETNA: Time Series Analysis. What, why and how?](https://medium.com/its-tinkoff/etna-time-series-analysis-what-why-and-how-e45557af4f6c) on Medium
+
 - [Tabular Playground Series - Mar 2022 (7th place!)](https://www.kaggle.com/code/chikovalexander/tps-mar-2022-etna/notebook?scriptVersionId=91575908) on Kaggle
 
 - [Store sales prediction with etna library](https://www.kaggle.com/dmitrybunin/store-sales-prediction-with-etna-library?scriptVersionId=81104235) on Kaggle
 
 - [Tabular Playground Series - Jan 2022](https://www.kaggle.com/code/chikovalexander/tps-jan-2022-etna/notebook) on Kaggle
 
 - [EDA notebook for Ubiquant Market Prediction](https://www.kaggle.com/code/martins0n/ubiquant-eda-toy-predictions-etna) on Kaggle
 
 - [PyCon Russia September 2021 talk](https://youtu.be/VxWHLEFgXnE) on YouTube
 
-- ETNA Tutorial [Part 1 (Rus)](https://youtu.be/4iFVRfB2j30), [Part 2 (Rus)](https://youtu.be/Ct9dyUdHlmc),  [Part 3 (Rus)](https://youtu.be/Qof38dtigtE) on YouTube thanks to [RC Gewissta](https://github.com/Gewissta)
+- [ETNA Meetup Jun 2022](https://www.youtube.com/watch?v=N1Xy3EqY058&list=PLLrf_044z4JrSsjMd-3dF6VbBLPI_yOxG) on YouTube
 
+- [DUMP May 2022 talk](https://youtu.be/12uuxepdtks) on YouTube
+ 
 ## Acknowledgments
 
 ### ETNA.Team
 
 [Andrey Alekseev](https://github.com/iKintosh),
 [Nikita Barinov](https://github.com/diadorer),
 [Dmitriy Bunin](https://github.com/Mr-Geekman),
 [Aleksandr Chikov](https://github.com/alex-hse-repository),
 [Vladislav Denisov](https://github.com/v-v-denisov),
 [Martin Gabdushev](https://github.com/martins0n),
 [Sergey Kolesnikov](https://github.com/Scitator),
 [Artem Makhin](https://github.com/Ama16),
 [Ivan Mitskovets](https://github.com/imitskovets),
 [Albina Munirova](https://github.com/albinamunirova),
-[Nikolay Romantsov](https://github.com/WinstonDovlatov),
-[Julia Shenshina](https://github.com/julia-shenshina)
+[Julia Shenshina](https://github.com/julia-shenshina),
+[Yuriy Tarasyuk](https://github.com/DBcreator),
+[Konstantin Vedernikov](https://github.com/scanhex12)
 
 ### ETNA.Contributors
 
+[WinstonDovlatov](https://github.com/WinstonDovlatov),
+[mvakhmenin](https://github.com/mvakhmenin),
+[Carlosbogo](https://github.com/Carlosbogo),
+[Pacman1984](https://github.com/Pacman1984),
+[looopka](https://github.com/looopka),
 [Artem Levashov](https://github.com/soft1q),
-[Aleksey Podkidyshev](https://github.com/alekseyen),
-[Carlosbogo](https://github.com/Carlosbogo)
+[Aleksey Podkidyshev](https://github.com/alekseyen)
 
 ## License
 
 Feel free to use our library in your commercial and private applications.
 
 ETNA is covered by [Apache 2.0](/LICENSE). 
 Read more about this license [here](https://choosealicense.com/licenses/apache-2.0/)
```

