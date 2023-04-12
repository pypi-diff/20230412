# Comparing `tmp/interpret-community-0.9.1.tar.gz` & `tmp/interpret-community-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\interpret-community-0.9.1.tar", last modified: Fri Apr  3 20:44:00 2020, max compression
+gzip compressed data, was "dist\interpret-community-0.9.2.tar", last modified: Mon Apr  6 21:30:55 2020, max compression
```

## Comparing `interpret-community-0.9.1.tar` & `interpret-community-0.9.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2020-04-03 20:44:00.000000 interpret-community-0.9.1/
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:58.000000 interpret-community-0.9.1/interpret_community/
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:59.000000 interpret-community-0.9.1/interpret_community/common/
--rw-rw-rw-   0        0        0     4779 2019-12-04 15:32:29.000000 interpret-community-0.9.1/interpret_community/common/aggregate.py
--rw-rw-rw-   0        0        0     2709 2019-11-13 17:30:15.000000 interpret-community-0.9.1/interpret_community/common/base_explainer.py
--rw-rw-rw-   0        0        0    13095 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/common/blackbox_explainer.py
--rw-rw-rw-   0        0        0      640 2019-11-13 17:30:15.000000 interpret-community-0.9.1/interpret_community/common/chained_identity.py
--rw-rw-rw-   0        0        0     8283 2020-03-28 03:17:52.000000 interpret-community-0.9.1/interpret_community/common/constants.py
--rw-rw-rw-   0        0        0      358 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/common/error_handling.py
--rw-rw-rw-   0        0        0    17182 2020-03-26 17:38:46.000000 interpret-community-0.9.1/interpret_community/common/explanation_utils.py
--rw-rw-rw-   0        0        0     2976 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/common/metrics.py
--rw-rw-rw-   0        0        0     1446 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/common/model_summary.py
--rw-rw-rw-   0        0        0    16747 2020-04-01 18:36:32.000000 interpret-community-0.9.1/interpret_community/common/model_wrapper.py
--rw-rw-rw-   0        0        0     6075 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/common/policy.py
--rw-rw-rw-   0        0        0     1021 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/common/progress.py
--rw-rw-rw-   0        0        0     2274 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/common/structured_model_explainer.py
--rw-rw-rw-   0        0        0      342 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/common/__init__.py
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:59.000000 interpret-community-0.9.1/interpret_community/community/
--rw-rw-rw-   0        0        0      384 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/community/__init__.py
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:59.000000 interpret-community-0.9.1/interpret_community/dataset/
--rw-rw-rw-   0        0        0    30331 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/dataset/dataset_wrapper.py
--rw-rw-rw-   0        0        0     1767 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/dataset/decorator.py
--rw-rw-rw-   0        0        0      269 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:59.000000 interpret-community-0.9.1/interpret_community/explanation/
--rw-rw-rw-   0        0        0    81252 2020-04-01 19:22:16.000000 interpret-community-0.9.1/interpret_community/explanation/explanation.py
--rw-rw-rw-   0        0        0      261 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/explanation/__init__.py
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:59.000000 interpret-community-0.9.1/interpret_community/mimic/
--rw-rw-rw-   0        0        0    36500 2020-04-03 19:41:42.000000 interpret-community-0.9.1/interpret_community/mimic/mimic_explainer.py
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:59.000000 interpret-community-0.9.1/interpret_community/mimic/models/
--rw-rw-rw-   0        0        0     2845 2020-04-03 20:36:42.000000 interpret-community-0.9.1/interpret_community/mimic/models/explainable_model.py
--rw-rw-rw-   0        0        0    14629 2020-04-03 20:36:42.000000 interpret-community-0.9.1/interpret_community/mimic/models/lightgbm_model.py
--rw-rw-rw-   0        0        0    21895 2020-03-19 16:44:21.000000 interpret-community-0.9.1/interpret_community/mimic/models/linear_model.py
--rw-rw-rw-   0        0        0     8772 2020-01-02 16:18:12.000000 interpret-community-0.9.1/interpret_community/mimic/models/tree_model.py
--rw-rw-rw-   0        0        0     5499 2019-11-13 17:30:15.000000 interpret-community-0.9.1/interpret_community/mimic/models/tree_model_utils.py
--rw-rw-rw-   0        0        0      628 2019-11-13 17:30:15.000000 interpret-community-0.9.1/interpret_community/mimic/models/__init__.py
--rw-rw-rw-   0        0        0     4045 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/mimic/model_distill.py
--rw-rw-rw-   0        0        0      330 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/mimic/__init__.py
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:59.000000 interpret-community-0.9.1/interpret_community/permutation/
--rw-rw-rw-   0        0        0     1182 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/permutation/metric_constants.py
--rw-rw-rw-   0        0        0    30241 2020-03-09 17:07:44.000000 interpret-community-0.9.1/interpret_community/permutation/permutation_importance.py
--rw-rw-rw-   0        0        0      317 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/permutation/__init__.py
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:59.000000 interpret-community-0.9.1/interpret_community/shap/
--rw-rw-rw-   0        0        0    21245 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/shap/deep_explainer.py
--rw-rw-rw-   0        0        0    22386 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/shap/kernel_explainer.py
--rw-rw-rw-   0        0        0     1363 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/shap/kwargs_utils.py
--rw-rw-rw-   0        0        0    16131 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/shap/linear_explainer.py
--rw-rw-rw-   0        0        0    17018 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/shap/tree_explainer.py
--rw-rw-rw-   0        0        0      513 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/shap/__init__.py
--rw-rw-rw-   0        0        0    13770 2020-03-02 15:37:11.000000 interpret-community-0.9.1/interpret_community/tabular_explainer.py
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:59.000000 interpret-community-0.9.1/interpret_community/widget/
--rw-rw-rw-   0        0        0     9676 2020-03-24 14:12:48.000000 interpret-community-0.9.1/interpret_community/widget/explanation_dashboard.py
--rw-rw-rw-   0        0        0    11280 2020-03-24 14:12:48.000000 interpret-community-0.9.1/interpret_community/widget/explanation_dashboard_input.py
-drwxrwxrwx   0        0        0        0 2020-04-03 20:44:00.000000 interpret-community-0.9.1/interpret_community/widget/static/
--rw-rw-rw-   0        0        0  4290596 2020-03-27 20:53:03.000000 interpret-community-0.9.1/interpret_community/widget/static/index.js
--rw-rw-rw-   0        0        0 15904949 2020-03-27 20:53:03.000000 interpret-community-0.9.1/interpret_community/widget/static/index.js.map
-drwxrwxrwx   0        0        0        0 2020-04-03 20:44:00.000000 interpret-community-0.9.1/interpret_community/widget/templates/
--rw-rw-rw-   0        0        0      536 2020-01-17 16:50:40.000000 interpret-community-0.9.1/interpret_community/widget/templates/dashboard.html
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:59.000000 interpret-community-0.9.1/interpret_community/widget/_internal/
--rw-rw-rw-   0        0        0     1531 2020-03-24 14:12:48.000000 interpret-community-0.9.1/interpret_community/widget/_internal/constants.py
--rw-rw-rw-   0        0        0      287 2019-11-13 17:30:15.000000 interpret-community-0.9.1/interpret_community/widget/_internal/__init__.py
--rw-rw-rw-   0        0        0      486 2019-11-13 17:30:15.000000 interpret-community-0.9.1/interpret_community/widget/_version.py
--rw-rw-rw-   0        0        0      330 2020-03-24 14:12:48.000000 interpret-community-0.9.1/interpret_community/widget/__init__.py
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:59.000000 interpret-community-0.9.1/interpret_community/_internal/
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:59.000000 interpret-community-0.9.1/interpret_community/_internal/raw_explain/
--rw-rw-rw-   0        0        0    10521 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/_internal/raw_explain/data_mapper.py
--rw-rw-rw-   0        0        0     4088 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/_internal/raw_explain/data_mapper_utils.py
--rw-rw-rw-   0        0        0    10663 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/_internal/raw_explain/feature_mappers.py
--rw-rw-rw-   0        0        0     2238 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/_internal/raw_explain/raw_explain_utils.py
--rw-rw-rw-   0        0        0      250 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/_internal/raw_explain/__init__.py
--rw-rw-rw-   0        0        0      237 2019-09-18 21:57:21.000000 interpret-community-0.9.1/interpret_community/_internal/__init__.py
--rw-rw-rw-   0        0        0     1216 2019-12-12 03:24:19.000000 interpret-community-0.9.1/interpret_community/__init__.py
-drwxrwxrwx   0        0        0        0 2020-04-03 20:43:59.000000 interpret-community-0.9.1/interpret_community.egg-info/
--rw-rw-rw-   0        0        0        1 2020-04-03 20:43:58.000000 interpret-community-0.9.1/interpret_community.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      805 2020-04-03 20:43:58.000000 interpret-community-0.9.1/interpret_community.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-04-03 20:43:58.000000 interpret-community-0.9.1/interpret_community.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3056 2020-04-03 20:43:58.000000 interpret-community-0.9.1/interpret_community.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2020-04-03 20:43:58.000000 interpret-community-0.9.1/interpret_community.egg-info/requires.txt
--rw-rw-rw-   0        0        0     2902 2020-04-03 20:43:58.000000 interpret-community-0.9.1/interpret_community.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       20 2020-04-03 20:43:58.000000 interpret-community-0.9.1/interpret_community.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1162 2020-04-03 20:43:58.000000 interpret-community-0.9.1/LICENSE.txt
--rw-rw-rw-   0        0        0      229 2020-01-17 16:50:40.000000 interpret-community-0.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3056 2020-04-03 20:44:00.000000 interpret-community-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     1811 2019-11-13 17:30:15.000000 interpret-community-0.9.1/README.md
--rw-rw-rw-   0        0        0       84 2020-04-03 20:44:00.000000 interpret-community-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     3566 2020-04-03 20:41:45.000000 interpret-community-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:55.000000 interpret-community-0.9.2/
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community/
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community/common/
+-rw-rw-rw-   0        0        0     4779 2019-12-04 15:32:29.000000 interpret-community-0.9.2/interpret_community/common/aggregate.py
+-rw-rw-rw-   0        0        0     2709 2019-11-13 17:30:15.000000 interpret-community-0.9.2/interpret_community/common/base_explainer.py
+-rw-rw-rw-   0        0        0    13095 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/common/blackbox_explainer.py
+-rw-rw-rw-   0        0        0      640 2019-11-13 17:30:15.000000 interpret-community-0.9.2/interpret_community/common/chained_identity.py
+-rw-rw-rw-   0        0        0     8283 2020-03-28 03:17:52.000000 interpret-community-0.9.2/interpret_community/common/constants.py
+-rw-rw-rw-   0        0        0      358 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/common/error_handling.py
+-rw-rw-rw-   0        0        0    17182 2020-03-26 17:38:46.000000 interpret-community-0.9.2/interpret_community/common/explanation_utils.py
+-rw-rw-rw-   0        0        0     2976 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/common/metrics.py
+-rw-rw-rw-   0        0        0     1446 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/common/model_summary.py
+-rw-rw-rw-   0        0        0    16747 2020-04-01 18:36:32.000000 interpret-community-0.9.2/interpret_community/common/model_wrapper.py
+-rw-rw-rw-   0        0        0     6075 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/common/policy.py
+-rw-rw-rw-   0        0        0     1021 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/common/progress.py
+-rw-rw-rw-   0        0        0     2274 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/common/structured_model_explainer.py
+-rw-rw-rw-   0        0        0      342 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/common/__init__.py
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community/community/
+-rw-rw-rw-   0        0        0      384 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/community/__init__.py
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community/dataset/
+-rw-rw-rw-   0        0        0    30331 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/dataset/dataset_wrapper.py
+-rw-rw-rw-   0        0        0     1767 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/dataset/decorator.py
+-rw-rw-rw-   0        0        0      269 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community/explanation/
+-rw-rw-rw-   0        0        0    81882 2020-04-06 21:23:03.000000 interpret-community-0.9.2/interpret_community/explanation/explanation.py
+-rw-rw-rw-   0        0        0      261 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/explanation/__init__.py
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community/mimic/
+-rw-rw-rw-   0        0        0    36792 2020-04-06 20:54:38.000000 interpret-community-0.9.2/interpret_community/mimic/mimic_explainer.py
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community/mimic/models/
+-rw-rw-rw-   0        0        0     2845 2020-04-04 02:16:49.000000 interpret-community-0.9.2/interpret_community/mimic/models/explainable_model.py
+-rw-rw-rw-   0        0        0    14623 2020-04-06 20:54:38.000000 interpret-community-0.9.2/interpret_community/mimic/models/lightgbm_model.py
+-rw-rw-rw-   0        0        0    21883 2020-04-06 20:54:38.000000 interpret-community-0.9.2/interpret_community/mimic/models/linear_model.py
+-rw-rw-rw-   0        0        0     8766 2020-04-06 20:54:38.000000 interpret-community-0.9.2/interpret_community/mimic/models/tree_model.py
+-rw-rw-rw-   0        0        0     5499 2019-11-13 17:30:15.000000 interpret-community-0.9.2/interpret_community/mimic/models/tree_model_utils.py
+-rw-rw-rw-   0        0        0      628 2019-11-13 17:30:15.000000 interpret-community-0.9.2/interpret_community/mimic/models/__init__.py
+-rw-rw-rw-   0        0        0     4045 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/mimic/model_distill.py
+-rw-rw-rw-   0        0        0      330 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/mimic/__init__.py
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community/permutation/
+-rw-rw-rw-   0        0        0     1182 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/permutation/metric_constants.py
+-rw-rw-rw-   0        0        0    30241 2020-03-09 17:07:44.000000 interpret-community-0.9.2/interpret_community/permutation/permutation_importance.py
+-rw-rw-rw-   0        0        0      317 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/permutation/__init__.py
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community/shap/
+-rw-rw-rw-   0        0        0    21245 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/shap/deep_explainer.py
+-rw-rw-rw-   0        0        0    22386 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/shap/kernel_explainer.py
+-rw-rw-rw-   0        0        0     1363 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/shap/kwargs_utils.py
+-rw-rw-rw-   0        0        0    16131 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/shap/linear_explainer.py
+-rw-rw-rw-   0        0        0    17018 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/shap/tree_explainer.py
+-rw-rw-rw-   0        0        0      513 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/shap/__init__.py
+-rw-rw-rw-   0        0        0    13770 2020-03-02 15:37:11.000000 interpret-community-0.9.2/interpret_community/tabular_explainer.py
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community/widget/
+-rw-rw-rw-   0        0        0     9676 2020-03-24 14:12:48.000000 interpret-community-0.9.2/interpret_community/widget/explanation_dashboard.py
+-rw-rw-rw-   0        0        0    11280 2020-03-24 14:12:48.000000 interpret-community-0.9.2/interpret_community/widget/explanation_dashboard_input.py
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:55.000000 interpret-community-0.9.2/interpret_community/widget/static/
+-rw-rw-rw-   0        0        0  4290596 2020-03-27 20:53:03.000000 interpret-community-0.9.2/interpret_community/widget/static/index.js
+-rw-rw-rw-   0        0        0 15904949 2020-03-27 20:53:03.000000 interpret-community-0.9.2/interpret_community/widget/static/index.js.map
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:55.000000 interpret-community-0.9.2/interpret_community/widget/templates/
+-rw-rw-rw-   0        0        0      536 2020-01-17 16:50:40.000000 interpret-community-0.9.2/interpret_community/widget/templates/dashboard.html
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community/widget/_internal/
+-rw-rw-rw-   0        0        0     1531 2020-03-24 14:12:48.000000 interpret-community-0.9.2/interpret_community/widget/_internal/constants.py
+-rw-rw-rw-   0        0        0      287 2019-11-13 17:30:15.000000 interpret-community-0.9.2/interpret_community/widget/_internal/__init__.py
+-rw-rw-rw-   0        0        0      486 2019-11-13 17:30:15.000000 interpret-community-0.9.2/interpret_community/widget/_version.py
+-rw-rw-rw-   0        0        0      330 2020-03-24 14:12:48.000000 interpret-community-0.9.2/interpret_community/widget/__init__.py
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community/_internal/
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community/_internal/raw_explain/
+-rw-rw-rw-   0        0        0    10521 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/_internal/raw_explain/data_mapper.py
+-rw-rw-rw-   0        0        0     4088 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/_internal/raw_explain/data_mapper_utils.py
+-rw-rw-rw-   0        0        0    10663 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/_internal/raw_explain/feature_mappers.py
+-rw-rw-rw-   0        0        0     2238 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/_internal/raw_explain/raw_explain_utils.py
+-rw-rw-rw-   0        0        0      250 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/_internal/raw_explain/__init__.py
+-rw-rw-rw-   0        0        0      237 2019-09-18 21:57:21.000000 interpret-community-0.9.2/interpret_community/_internal/__init__.py
+-rw-rw-rw-   0        0        0     1216 2019-12-12 03:24:19.000000 interpret-community-0.9.2/interpret_community/__init__.py
+drwxrwxrwx   0        0        0        0 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community.egg-info/
+-rw-rw-rw-   0        0        0        1 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      805 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3056 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     2902 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       20 2020-04-06 21:30:54.000000 interpret-community-0.9.2/interpret_community.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1162 2020-04-06 21:30:53.000000 interpret-community-0.9.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      229 2020-01-17 16:50:40.000000 interpret-community-0.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3056 2020-04-06 21:30:55.000000 interpret-community-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1811 2019-11-13 17:30:15.000000 interpret-community-0.9.2/README.md
+-rw-rw-rw-   0        0        0       84 2020-04-06 21:30:55.000000 interpret-community-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     3566 2020-04-06 21:26:34.000000 interpret-community-0.9.2/setup.py
```

### Comparing `interpret-community-0.9.1/interpret_community/common/aggregate.py` & `interpret-community-0.9.2/interpret_community/common/aggregate.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/common/base_explainer.py` & `interpret-community-0.9.2/interpret_community/common/base_explainer.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/common/blackbox_explainer.py` & `interpret-community-0.9.2/interpret_community/common/blackbox_explainer.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/common/chained_identity.py` & `interpret-community-0.9.2/interpret_community/common/chained_identity.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/common/constants.py` & `interpret-community-0.9.2/interpret_community/common/constants.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/common/explanation_utils.py` & `interpret-community-0.9.2/interpret_community/common/explanation_utils.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/common/metrics.py` & `interpret-community-0.9.2/interpret_community/common/metrics.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/common/model_summary.py` & `interpret-community-0.9.2/interpret_community/common/model_summary.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/common/model_wrapper.py` & `interpret-community-0.9.2/interpret_community/common/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/common/policy.py` & `interpret-community-0.9.2/interpret_community/common/policy.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/common/progress.py` & `interpret-community-0.9.2/interpret_community/common/progress.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/common/structured_model_explainer.py` & `interpret-community-0.9.2/interpret_community/common/structured_model_explainer.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/dataset/dataset_wrapper.py` & `interpret-community-0.9.2/interpret_community/dataset/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/dataset/decorator.py` & `interpret-community-0.9.2/interpret_community/dataset/decorator.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/explanation/explanation.py` & `interpret-community-0.9.2/interpret_community/explanation/explanation.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,18 +184,28 @@
                 self.explanation_type, feature_type
             )
         )
 
     @property
     @abstractmethod
     def selector(self):
+        """Get the local or global selector.
+
+        :return: The selector as a pandas dataframe of records.
+        :rtype: pd.DataFrame
+        """
         return None
 
     @property
     def name(self):
+        """Get the name of the explanation.
+
+        :return: The name of the explanation.
+        :rtype: str
+        """
         return gen_name_from_class(self)
 
     @staticmethod
     def _does_quack(explanation):
         """Validate that the explanation object passed in is a valid BaseExplanation.
 
         :param explanation: The explanation to be validated.
@@ -538,14 +548,19 @@
                     InterpretData.MLI: mli_data}
         else:
             data_dict = self._local_data(parent_data, key=key)
             return data_dict
 
     @property
     def selector(self):
+        """Get the local selector.
+
+        :return: The selector as a pandas dataframe of records.
+        :rtype: pd.DataFrame
+        """
         predicted = self._eval_y_predicted
         dataset_shape = np.empty((self._local_importance_values.shape[-2], 1))
         return gen_local_selector(dataset_shape, None, predicted.flatten())
 
     @classmethod
     def _does_quack(cls, explanation):
         """Validate that the explanation object passed in is a valid LocalExplanation.
@@ -762,14 +777,19 @@
             return {InterpretData.OVERALL: global_data, InterpretData.SPECIFIC: specific,
                     InterpretData.MLI: mli_data}
         else:
             return parent_data
 
     @property
     def selector(self):
+        """Get the global selector if this is only a global explanation otherwise local.
+
+        :return: The selector as a pandas dataframe of records.
+        :rtype: pd.DataFrame
+        """
         if LocalExplanation._does_quack(self):
             return LocalExplanation.selector.__get__(self)
         nan_predicted = np.empty((1, 1))
         nan_predicted[:] = np.nan
         feature_types = ["numeric"] * len(self.features)
         return gen_global_selector(nan_predicted, self.features, feature_types, self.global_importance_values)
```

### Comparing `interpret-community-0.9.1/interpret_community/mimic/mimic_explainer.py` & `interpret-community-0.9.2/interpret_community/mimic/mimic_explainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,15 @@
         :param batch_size: If include_local is False, specifies the batch size for aggregating
             local explanations to global.
         :type batch_size: int
         :return: Args for explain_global.
         :rtype: dict
         """
         classification = self.predict_proba_flag
-        kwargs = {ExplainParams.METHOD: ExplainType.MIMIC}
+        kwargs = {ExplainParams.METHOD: self._get_method}
         if classification:
             kwargs[ExplainParams.CLASSES] = self.classes
         if evaluation_examples is not None:
 
             # Aggregate local explanation to global, either through computing the local
             # explanation and then aggregating or streaming the local explanation to global
             if include_local:
@@ -415,14 +415,23 @@
         explanation = _create_global_explanation(**kwargs)
 
         # if transformations have been passed, then return raw features explanation
         raw_kwargs = _get_raw_explainer_create_explanation_kwargs(kwargs=kwargs)
         return explanation if self._datamapper is None else _create_raw_feats_global_explanation(
             explanation, feature_maps=[self._datamapper.feature_map], features=self.features, **raw_kwargs)
 
+    @property
+    def _get_method(self):
+        """Get the method for this explainer, or mimic with surrogate model type.
+
+        :return: The method, or mimic with surrogate model type.
+        :rtype: str
+        """
+        return "{}.{}".format(ExplainType.MIMIC, self._method)
+
     def _get_explain_local_kwargs(self, evaluation_examples):
         """Get the kwargs for explain_local to create a local explanation.
 
         :param evaluation_examples: A matrix of feature vector examples (# examples x # features) on which
             to explain the model's output.
         :type evaluation_examples: numpy.array or pandas.DataFrame or scipy.sparse.csr_matrix
         :return: Args for explain_local.
@@ -447,15 +456,15 @@
 
         kwargs[ExplainParams.NUM_FEATURES] = evaluation_examples.num_features
 
         local_importance_values = self.surrogate_model.explain_local(dataset, probabilities=probabilities)
         classification = isinstance(local_importance_values, list) or self.predict_proba_flag
         is_sparse = sp.sparse.issparse(local_importance_values) or sp.sparse.issparse(local_importance_values[0])
         expected_values = self.surrogate_model.expected_values
-        kwargs[ExplainParams.METHOD] = ExplainType.MIMIC
+        kwargs[ExplainParams.METHOD] = self._get_method
         self.features = evaluation_examples.get_features(features=self.features)
         kwargs[ExplainParams.FEATURES] = self.features
 
         if self.predict_proba_flag and not is_sparse:
             if self.surrogate_model.multiclass:
                 # For multiclass case, convert to array, but only if not sparse
                 local_importance_values = np.array(local_importance_values)
```

### Comparing `interpret-community-0.9.1/interpret_community/mimic/models/explainable_model.py` & `interpret-community-0.9.2/interpret_community/mimic/models/explainable_model.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/mimic/models/lightgbm_model.py` & `interpret-community-0.9.2/interpret_community/mimic/models/lightgbm_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         if self.multiclass:
             initializer = LGBMClassifier
         else:
             initializer = LGBMRegressor
         self._lgbm = initializer(random_state=random_state, **initializer_args)
         super(LGBMExplainableModel, self).__init__(**kwargs)
         self._logger.debug('Initializing LGBMExplainableModel')
-        self._method = 'mimic.lightgbm'
+        self._method = 'lightgbm'
         self._tree_explainer = None
         self._shap_values_output = shap_values_output
         self._classification = classification
 
     try:
         __init__.__doc__ = (__init__.__doc__ +
                             '\nIf multiclass=True, uses the parameters for LGBMClassifier:\n' +
```

### Comparing `interpret-community-0.9.1/interpret_community/mimic/models/linear_model.py` & `interpret-community-0.9.2/interpret_community/mimic/models/linear_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
                 initializer = Lasso
             else:
                 initializer = LinearRegression
         initializer_args = _get_initializer_args(kwargs)
         self._linear = initializer(**initializer_args)
         super(LinearExplainableModel, self).__init__(**kwargs)
         self._logger.debug('Initializing LinearExplainableModel')
-        self._method = 'mimic.linear'
+        self._method = 'linear'
         self._linear_explainer = None
         self._classification = classification
 
     __init__.__doc__ = (__init__.__doc__ +
                         '\nIf multiclass=True, uses the parameters for LogisticRegression:\n' +
                         _clean_doc(LogisticRegression.__doc__) +
                         '\nOtherwise, if multiclass=False, uses the parameters for LinearRegression:\n' +
@@ -361,15 +361,15 @@
             initializer = SGDClassifier
         else:
             initializer = SGDRegressor
         initializer_args = _get_initializer_args(kwargs)
         self._sgd = initializer(random_state=random_state, **initializer_args)
         super(SGDExplainableModel, self).__init__(**kwargs)
         self._logger.debug('Initializing SGDExplainableModel')
-        self._method = 'mimic.sgd'
+        self._method = 'sgd'
         self._sgd_explainer = None
         self._classification = classification
 
     __init__.__doc__ = (__init__.__doc__ +
                         '\nIf multiclass=True, uses the parameters for SGDClassifier:\n' +
                         _clean_doc(SGDClassifier.__doc__) +
                         '\nOtherwise, if multiclass=False, uses the parameters for SGDRegressor:\n' +
```

### Comparing `interpret-community-0.9.1/interpret_community/mimic/models/tree_model.py` & `interpret-community-0.9.2/interpret_community/mimic/models/tree_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             initializer = DecisionTreeClassifier
         else:
             initializer = DecisionTreeRegressor
         initializer_args = _get_initializer_args(kwargs)
         self._tree = initializer(**initializer_args)
         super(DecisionTreeExplainableModel, self).__init__(**kwargs)
         self._logger.debug('Initializing DecisionTreeExplainableModel')
-        self._method = 'mimic.tree'
+        self._method = 'tree'
         self._tree_explainer = None
         self._shap_values_output = shap_values_output
         self._classification = classification
 
     __init__.__doc__ = (__init__.__doc__ +
                         '\nIf multiclass=True, uses the parameters for DecisionTreeClassifier:\n' +
                         _clean_doc(DecisionTreeClassifier.__doc__) +
```

### Comparing `interpret-community-0.9.1/interpret_community/mimic/models/tree_model_utils.py` & `interpret-community-0.9.2/interpret_community/mimic/models/tree_model_utils.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/mimic/models/__init__.py` & `interpret-community-0.9.2/interpret_community/mimic/models/__init__.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/mimic/model_distill.py` & `interpret-community-0.9.2/interpret_community/mimic/model_distill.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/permutation/metric_constants.py` & `interpret-community-0.9.2/interpret_community/permutation/metric_constants.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/permutation/permutation_importance.py` & `interpret-community-0.9.2/interpret_community/permutation/permutation_importance.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/shap/deep_explainer.py` & `interpret-community-0.9.2/interpret_community/shap/deep_explainer.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/shap/kernel_explainer.py` & `interpret-community-0.9.2/interpret_community/shap/kernel_explainer.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/shap/kwargs_utils.py` & `interpret-community-0.9.2/interpret_community/shap/kwargs_utils.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/shap/linear_explainer.py` & `interpret-community-0.9.2/interpret_community/shap/linear_explainer.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/shap/tree_explainer.py` & `interpret-community-0.9.2/interpret_community/shap/tree_explainer.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/shap/__init__.py` & `interpret-community-0.9.2/interpret_community/shap/__init__.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/tabular_explainer.py` & `interpret-community-0.9.2/interpret_community/tabular_explainer.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/widget/explanation_dashboard.py` & `interpret-community-0.9.2/interpret_community/widget/explanation_dashboard.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/widget/explanation_dashboard_input.py` & `interpret-community-0.9.2/interpret_community/widget/explanation_dashboard_input.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/widget/static/index.js` & `interpret-community-0.9.2/interpret_community/widget/static/index.js`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/widget/static/index.js.map` & `interpret-community-0.9.2/interpret_community/widget/static/index.js.map`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/widget/templates/dashboard.html` & `interpret-community-0.9.2/interpret_community/widget/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/widget/_internal/constants.py` & `interpret-community-0.9.2/interpret_community/widget/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/_internal/raw_explain/data_mapper.py` & `interpret-community-0.9.2/interpret_community/_internal/raw_explain/data_mapper.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/_internal/raw_explain/data_mapper_utils.py` & `interpret-community-0.9.2/interpret_community/_internal/raw_explain/data_mapper_utils.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/_internal/raw_explain/feature_mappers.py` & `interpret-community-0.9.2/interpret_community/_internal/raw_explain/feature_mappers.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/_internal/raw_explain/raw_explain_utils.py` & `interpret-community-0.9.2/interpret_community/_internal/raw_explain/raw_explain_utils.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community/__init__.py` & `interpret-community-0.9.2/interpret_community/__init__.py`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community.egg-info/entry_points.txt` & `interpret-community-0.9.2/interpret_community.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/interpret_community.egg-info/PKG-INFO` & `interpret-community-0.9.2/interpret_community.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpret-community
-Version: 0.9.1
+Version: 0.9.2
 Summary: Microsoft Interpret Extensions SDK for Python
 Home-page: https://github.com/interpretml/interpret-community
 Author: Microsoft Corp
 Author-email: ilmat@microsoft.com
 License: MIT License
 Description: # Microsoft Interpret Community SDK for Python
```

### Comparing `interpret-community-0.9.1/interpret_community.egg-info/SOURCES.txt` & `interpret-community-0.9.2/interpret_community.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/LICENSE.txt` & `interpret-community-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/PKG-INFO` & `interpret-community-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpret-community
-Version: 0.9.1
+Version: 0.9.2
 Summary: Microsoft Interpret Extensions SDK for Python
 Home-page: https://github.com/interpretml/interpret-community
 Author: Microsoft Corp
 Author-email: ilmat@microsoft.com
 License: MIT License
 Description: # Microsoft Interpret Community SDK for Python
```

### Comparing `interpret-community-0.9.1/README.md` & `interpret-community-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `interpret-community-0.9.1/setup.py` & `interpret-community-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """Setup file for interpret-community package."""
 from setuptools import setup, find_packages
 import os
 import shutil
 
 _major = '0'
 _minor = '9'
-_patch = '1'
+_patch = '2'
 
 README_FILE = 'README.md'
 LICENSE_FILE = 'LICENSE.txt'
 
 # Note: used when generating the wheel but not on pip install of the package
 if os.path.exists('../LICENSE'):
     shutil.copyfile('../LICENSE', LICENSE_FILE)
```

