# Comparing `tmp/Simba-UW-tf-dev-1.56.1.tar.gz` & `tmp/Simba-UW-tf-dev-1.56.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.56.1.tar", last modified: Mon Apr 10 20:28:02 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.56.2.tar", last modified: Wed Apr 12 13:54:04 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.56.1.tar` & `Simba-UW-tf-dev-1.56.2.tar`

### file list

```diff
@@ -1,385 +1,385 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/
--rw-r--r--   0 simon      (501) staff       (20)    32475 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.1/simba/video_processing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.56.1/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    10851 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/unsupervised_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-03-21 14:26:03.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/misc.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7227 2023-03-21 11:41:26.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     4061 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/data_extractors.py
--rw-r--r--   0 simon      (501) staff       (20)    11192 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/dbcv.py
--rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7526 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/umap_embedder.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/visualization_tools/
--rw-r--r--   0 simon      (501) staff       (20)     2019 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/visualization_tools/vtk_embeddings.py
--rw-r--r--   0 simon      (501) staff       (20)      150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/ui_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    49992 2023-03-22 15:08:56.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-03-21 15:42:27.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6642 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3789 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     5630 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/unsupervised/cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    19273 2023-04-10 14:46:51.000000 Simba-UW-tf-dev-1.56.1/simba/enums.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/bounding_box_tools/find_bounderies.py
--rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.56.1/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-10 20:26:31.000000 Simba-UW-tf-dev-1.56.1/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42839 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21591 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)    19620 2023-04-03 12:08:14.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/fish_feature_extractor_2023.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    28019 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-10 20:22:57.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2317 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    36798 2023-03-15 17:04:48.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/extract_features_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    46505 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    24092 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16809 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/plotly_create_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.56.1/simba/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.1/simba/severity_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.56.1/simba/user_pose_config_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.56.1/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    41856 2023-04-05 17:24:50.000000 Simba-UW-tf-dev-1.56.1/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-04-07 13:58:40.000000 Simba-UW-tf-dev-1.56.1/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-06 14:21:49.000000 Simba-UW-tf-dev-1.56.1/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    34563 2023-04-10 20:12:42.000000 Simba-UW-tf-dev-1.56.1/simba/machine_model_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.1/simba/remove_keypoints_in_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/solomon_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)    12866 2023-04-10 14:41:24.000000 Simba-UW-tf-dev-1.56.1/simba/FSTTC_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.56.1/simba/create_project_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.1/simba/video_info_table.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/extract_frames_fast.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.56.1/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.1/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     4141 2023-04-10 14:46:51.000000 Simba-UW-tf-dev-1.56.1/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14398 2023-04-10 19:08:11.000000 Simba-UW-tf-dev-1.56.1/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)     1042 2023-04-10 14:46:51.000000 Simba-UW-tf-dev-1.56.1/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.1/simba/timebins_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    46383 2023-04-10 20:10:32.000000 Simba-UW-tf-dev-1.56.1/simba/train_model_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.1/simba/timebins_clf_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.56.1/simba/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.1/simba/movement_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/pybursts.py
--rw-r--r--   0 simon      (501) staff       (20)     2856 2023-04-10 15:29:30.000000 Simba-UW-tf-dev-1.56.1/simba/rw_dfs.py
--rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/reverse_2_animal_tracking.py
--rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.56.1/simba/Directing_animals_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     4337 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.56.1/simba/Validate_model_one_video_run_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9548 2023-04-06 00:40:25.000000 Simba-UW-tf-dev-1.56.1/simba/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.56.1/simba/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.56.1/simba/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.56.1/simba/run_inference.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14661 2023-04-10 20:11:46.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/misc_visualizations.py
--rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/plotting/heat_mapper_location_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/interpolate_smooth_post_hoc.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/reverse_tracking_order.py
--rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.56.1/simba/concatenator_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/extract_annotation_frames.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_image.py
--rw-r--r--   0 simon      (501) staff       (20)    56847 2023-04-10 15:09:41.000000 Simba-UW-tf-dev-1.56.1/simba/misc_tools.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.1/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.1/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.1/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)    16536 2023-03-20 13:30:18.000000 Simba-UW-tf-dev-1.56.1/simba/pose_importers/import_trk.py
--rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.1/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.56.1/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.1/simba/pose_importers/trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)   232870 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.1/simba/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/extract_seqframes.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/1.png
--rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/get_coordinates_tools_v2.py
--rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.56.1/simba/pup_retrieval_protocol.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.1/simba/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)    17627 2023-04-10 20:01:08.000000 Simba-UW-tf-dev-1.56.1/simba/train_mutiple_models.py
--rw-r--r--   0 simon      (501) staff       (20)    62620 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.56.1/simba/SimBA.py
--rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/labelling_advanced_interface.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:22:57.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-10 20:24:04.000000 Simba-UW-tf-dev-1.56.1/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 20:22:06.000000 Simba-UW-tf-dev-1.56.1/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)    44067 2023-04-10 20:17:11.000000 Simba-UW-tf-dev-1.56.1/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.56.1/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   318858 2023-04-10 20:19:47.000000 Simba-UW-tf-dev-1.56.1/simba/assets/img/splash_old.mp4
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.56.1/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.56.1/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/assets/TheGoldenLab.PNG
--rw-r--r--   0 simon      (501) staff       (20)    21460 2023-04-10 14:41:24.000000 Simba-UW-tf-dev-1.56.1/simba/drop_bp_cords.py
--rw-r--r--   0 simon      (501) staff       (20)     8116 2023-03-19 18:27:51.000000 Simba-UW-tf-dev-1.56.1/simba/read_config_unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/project_config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.56.1/simba/set_hyperparameters.py
--rw-r--r--   0 simon      (501) staff       (20)    20742 2023-04-10 19:52:46.000000 Simba-UW-tf-dev-1.56.1/simba/train_single_model.py
--rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/create_clf_log.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/simba/batch_process_videos/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.56.1/simba/batch_process_videos/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    24896 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.1/simba/batch_process_videos/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/batch_process_videos/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10882 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.56.1/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.1/simba/Kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.1/simba/reorganize_keypoint_in_pose.py
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.56.1/simba/~$features.pptx
--rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.1/simba/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-10 20:28:01.000000 Simba-UW-tf-dev-1.56.1/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    13006 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-10 20:28:01.000000 Simba-UW-tf-dev-1.56.1/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      640 2023-04-10 20:28:01.000000 Simba-UW-tf-dev-1.56.1/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-10 20:28:01.000000 Simba-UW-tf-dev-1.56.1/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-10 20:28:01.000000 Simba-UW-tf-dev-1.56.1/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.56.1/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.56.1/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.56.1/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-10 20:12:06.000000 Simba-UW-tf-dev-1.56.1/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-10 20:28:02.000000 Simba-UW-tf-dev-1.56.1/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/
+-rw-r--r--   0 simon      (501) staff       (20)    32475 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.2/simba/video_processing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.56.2/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    10851 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/unsupervised_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6566 2023-03-21 14:26:03.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/misc.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7227 2023-03-21 11:41:26.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4061 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/data_extractors.py
+-rw-r--r--   0 simon      (501) staff       (20)    11192 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/dbcv.py
+-rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7526 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/umap_embedder.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/visualization_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     2019 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/visualization_tools/vtk_embeddings.py
+-rw-r--r--   0 simon      (501) staff       (20)      150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/ui_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    49992 2023-03-22 15:08:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-03-21 15:42:27.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6642 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3789 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     5630 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/unsupervised/cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    19383 2023-04-12 13:53:16.000000 Simba-UW-tf-dev-1.56.2/simba/enums.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/find_bounderies.py
+-rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-11 16:58:43.000000 Simba-UW-tf-dev-1.56.2/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42839 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21591 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21399 2023-04-11 16:58:31.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    28019 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-11 20:41:01.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2317 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    36798 2023-03-15 17:04:48.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/extract_features_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    46505 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24092 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16809 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/plotly_create_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.56.2/simba/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.2/simba/severity_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.56.2/simba/user_pose_config_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.56.2/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    41856 2023-04-05 17:24:50.000000 Simba-UW-tf-dev-1.56.2/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-04-07 13:58:40.000000 Simba-UW-tf-dev-1.56.2/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.56.2/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    34563 2023-04-10 20:12:42.000000 Simba-UW-tf-dev-1.56.2/simba/machine_model_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.2/simba/remove_keypoints_in_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/solomon_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)    12866 2023-04-10 14:41:24.000000 Simba-UW-tf-dev-1.56.2/simba/FSTTC_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.56.2/simba/create_project_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.2/simba/video_info_table.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/extract_frames_fast.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.56.2/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.2/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     4142 2023-04-12 12:21:03.000000 Simba-UW-tf-dev-1.56.2/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14398 2023-04-10 19:08:11.000000 Simba-UW-tf-dev-1.56.2/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.56.2/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.2/simba/timebins_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    46383 2023-04-10 20:10:32.000000 Simba-UW-tf-dev-1.56.2/simba/train_model_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.2/simba/timebins_clf_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.56.2/simba/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.2/simba/movement_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pybursts.py
+-rw-r--r--   0 simon      (501) staff       (20)     3798 2023-04-12 13:45:31.000000 Simba-UW-tf-dev-1.56.2/simba/rw_dfs.py
+-rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/reverse_2_animal_tracking.py
+-rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.56.2/simba/Directing_animals_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.56.2/simba/Validate_model_one_video_run_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9548 2023-04-06 00:40:25.000000 Simba-UW-tf-dev-1.56.2/simba/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.56.2/simba/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.56.2/simba/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.56.2/simba/run_inference.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14661 2023-04-10 20:11:46.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/misc_visualizations.py
+-rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_location_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/interpolate_smooth_post_hoc.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/reverse_tracking_order.py
+-rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.56.2/simba/concatenator_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/extract_annotation_frames.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_image.py
+-rw-r--r--   0 simon      (501) staff       (20)    56847 2023-04-10 15:09:41.000000 Simba-UW-tf-dev-1.56.2/simba/misc_tools.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)    16536 2023-03-20 13:30:18.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/import_trk.py
+-rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.2/simba/pose_importers/trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)   232870 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.2/simba/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/extract_seqframes.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/1.png
+-rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/get_coordinates_tools_v2.py
+-rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.56.2/simba/pup_retrieval_protocol.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.2/simba/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)    17627 2023-04-10 20:01:08.000000 Simba-UW-tf-dev-1.56.2/simba/train_mutiple_models.py
+-rw-r--r--   0 simon      (501) staff       (20)    64156 2023-04-12 13:52:14.000000 Simba-UW-tf-dev-1.56.2/simba/SimBA.py
+-rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/labelling_advanced_interface.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-11 20:46:03.000000 Simba-UW-tf-dev-1.56.2/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.56.2/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.56.2/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/assets/TheGoldenLab.PNG
+-rw-r--r--   0 simon      (501) staff       (20)    21460 2023-04-10 14:41:24.000000 Simba-UW-tf-dev-1.56.2/simba/drop_bp_cords.py
+-rw-r--r--   0 simon      (501) staff       (20)     8085 2023-04-12 13:31:27.000000 Simba-UW-tf-dev-1.56.2/simba/read_config_unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/project_config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.56.2/simba/set_hyperparameters.py
+-rw-r--r--   0 simon      (501) staff       (20)    20742 2023-04-10 19:52:46.000000 Simba-UW-tf-dev-1.56.2/simba/train_single_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/create_clf_log.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    24896 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10882 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.2/simba/Kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.2/simba/reorganize_keypoint_in_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.56.2/simba/~$features.pptx
+-rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.2/simba/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    13039 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      638 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.56.2/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.56.2/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.56.2/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1895 2023-04-12 13:53:57.000000 Simba-UW-tf-dev-1.56.2/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-12 13:54:04.000000 Simba-UW-tf-dev-1.56.2/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.56.1/PKG-INFO` & `Simba-UW-tf-dev-1.56.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.56.1
+Version: 1.56.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.56.1/simba/video_processing.py` & `Simba-UW-tf-dev-1.56.2/simba/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/unsupervised_ui.py` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/unsupervised_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/misc.py` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/misc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/data_extractors.py` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/data_extractors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/dbcv.py` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/dbcv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/visualizers.py` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/visualization_tools/vtk_embeddings.py` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/visualization_tools/vtk_embeddings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.56.2/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/enums.py` & `Simba-UW-tf-dev-1.56.2/simba/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from enum import Enum, unique
+from enum import Enum
+import pkg_resources
 from pathlib import Path
 import cv2
 
 class ReadConfig(Enum):
     GENERAL_SETTINGS = 'General settings'
     PROJECT_PATH = 'project_path'
     SML_SETTINGS = 'SML settings'
@@ -121,14 +122,15 @@
 class Formats(Enum):
     MP4_CODEC = 'mp4v'
     AVI_CODEC = 'XVID'
     LABELFRAME_HEADER_FORMAT = ('Helvetica', 12, 'bold')
     LABELFRAME_HEADER_CLICKABLE_FORMAT = ('Helvetica', 12, 'bold', 'underline')
     LABELFRAME_HEADER_CLICKABLE_COLOR = f'#{5:02x}{99:02x}{193:02x}'
     CSV = 'csv'
+    PARQUET = 'parquet'
     PERIMETER = 'perimeter'
     AREA = 'area'
     H5 = 'h5'
     ROOT_WINDOW_SIZE = "750x750"
     FONT = cv2.FONT_HERSHEY_TRIPLEX
     TKINTER_FONT = ("Rockwell", 11)
 
@@ -184,15 +186,15 @@
                                             'Annotations EVENT COUNT conflict',
                                             'Annotations data file NOT FOUND']
 
 class Defaults(Enum):
     MAX_TASK_PER_CHILD = 10
     CHUNK_SIZE = 1
     SPLASH_TIME = 2500
-    WELCOME_MSG = 'Welcome fellow scientists! \n'
+    WELCOME_MSG = f'Welcome fellow scientists! \n SimBA v.{pkg_resources.get_distribution("simba-uw-tf-dev").version} \n '
     BROWSE_FOLDER_BTN_TEXT = 'Browse Folder'
     BROWSE_FILE_BTN_TEXT = 'Browse File'
     NO_FILE_SELECTED_TEXT = 'No file selected'
     STR_SPLIT_DELIMITER = '\t'
 
 class TagNames(Enum):
     GREETING = 'greeting'
```

### Comparing `Simba-UW-tf-dev-1.56.1/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/bounding_box_tools/find_bounderies.py` & `Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/find_bounderies.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.56.2/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -509,18 +509,18 @@
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 0013 0000 000b  ................
 00002010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00002020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00002030: 0000 0041 3fd9 0000 000b 005f 005f 0070  ...A?......_._.p
+00002030: 0000 0041 3e1a 0000 000b 005f 005f 0070  ...A>......_._.p
 00002040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00002050: 6d6f 4444 626c 6f62 0000 0008 5667 2fa4  moDDblob....Vg/.
-00002060: 52f2 c441 0000 000b 005f 005f 0070 0079  R..A....._._.p.y
+00002050: 6d6f 4444 626c 6f62 0000 0008 e5ad 83c6  moDDblob........
+00002060: d8f2 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00002070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 00002080: 6444 626c 6f62 0000 0008 5667 2fa4 52f2  dDblob....Vg/.R.
 00002090: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000020a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000020b0: 636f 6d70 0000 0000 004f 1000 0000 0006  comp.....O......
 000020c0: 0061 0073 0073 0065 0074 0073 6277 7370  .a.s.s.e.t.sbwsp
 000020d0: 626c 6f62 0000 00c7 6270 6c69 7374 3030  blob....bplist00
@@ -533,15 +533,15 @@
 00002140: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
 00002150: 7208 0809 0809 5f10 167b 7b30 2c20 3230  r....._..{{0, 20
 00002160: 307d 2c20 7b37 3730 2c20 3433 367d 7d09  0}, {770, 436}}.
 00002170: 0817 2531 3d49 606d 797a 7b7c 7d7e 9700  ..%1=I`myz{|}~..
 00002180: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 00002190: 0000 0000 0000 0000 0000 0000 0000 9800  ................
 000021a0: 0000 0600 6100 7300 7300 6500 7400 736c  ....a.s.s.e.t.sl
-000021b0: 6731 5363 6f6d 7000 0000 0000 80dc ec00  g1Scomp.........
+000021b0: 6731 5363 6f6d 7000 0000 0000 7dc8 d600  g1Scomp.....}...
 000021c0: 0000 0600 6100 7300 7300 6500 7400 736c  ....a.s.s.e.t.sl
 000021d0: 7376 4362 6c6f 6200 0002 b062 706c 6973  svCblob....bplis
 000021e0: 7430 30da 0102 0304 0506 0708 090a 0b0c  t00.............
 000021f0: 0d18 4849 484a 4b0c 5f10 1276 6965 774f  ..HIHJK._..viewO
 00002200: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
 00002210: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 00002220: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
@@ -628,15 +628,15 @@
 00002730: 0000 0000 0000 0000 0000 01dd 0000 0006  ................
 00002740: 0061 0073 0073 0065 0074 0073 6d6f 4444  .a.s.s.e.t.smoDD
 00002750: 626c 6f62 0000 0008 cf95 8ce8 d0e1 c441  blob...........A
 00002760: 0000 0006 0061 0073 0073 0065 0074 0073  .....a.s.s.e.t.s
 00002770: 6d6f 6444 626c 6f62 0000 0008 cf95 8ce8  modDblob........
 00002780: d0e1 c441 0000 0006 0061 0073 0073 0065  ...A.....a.s.s.e
 00002790: 0074 0073 7068 3153 636f 6d70 0000 0000  .t.sph1Scomp....
-000027a0: 0084 9000 0000 0006 0061 0073 0073 0065  .........a.s.s.e
+000027a0: 0081 8000 0000 0006 0061 0073 0073 0065  .........a.s.s.e
 000027b0: 0074 0073 7653 726e 6c6f 6e67 0000 0001  .t.svSrnlong....
 000027c0: 0000 0014 0062 0061 0074 0063 0068 005f  .....b.a.t.c.h._
 000027d0: 0070 0072 006f 0063 0065 0073 0073 005f  .p.r.o.c.e.s.s._
 000027e0: 0076 0069 0064 0065 006f 0073 6277 7370  .v.i.d.e.o.sbwsp
 000027f0: 626c 6f62 0000 00ca 6270 6c69 7374 3030  blob....bplist00
 00002800: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
 00002810: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
@@ -954,26 +954,26 @@
 00003b90: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
 00003ba0: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
 00003bb0: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
 00003bc0: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
 00003bd0: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
 00003be0: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
 00003bf0: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-00003c00: 0808 0908 095f 1019 7b7b 3437 322c 2031  ....._..{{472, 1
-00003c10: 3432 7d2c 207b 3130 3736 2c20 3632 317d  42}, {1076, 621}
+00003c00: 0808 0908 095f 1019 7b7b 3932 302c 2031  ....._..{{920, 1
+00003c10: 3531 7d2c 207b 3130 3736 2c20 3435 317d  51}, {1076, 451}
 00003c20: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
 00003c30: 9a00 0000 0000 0001 0100 0000 0000 0000  ................
 00003c40: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
 00003c50: 9b00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
 00003c60: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
 00003c70: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
 00003c80: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
 00003c90: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00003ca0: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
-00003cb0: 6d70 0000 0000 0011 bf82 0000 0012 0066  mp.............f
+00003cb0: 6d70 0000 0000 0011 c675 0000 0012 0066  mp.......u.....f
 00003cc0: 0065 0061 0074 0075 0072 0065 005f 0065  .e.a.t.u.r.e._.e
 00003cd0: 0078 0074 0072 0061 0063 0074 006f 0072  .x.t.r.a.c.t.o.r
 00003ce0: 0073 6c73 7643 626c 6f62 0000 02b8 6270  .slsvCblob....bp
 00003cf0: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
 00003d00: 0a0b 0c0d 1a48 4948 4a4b 0c5f 1012 7669  .....HIHJK._..vi
 00003d10: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
 00003d20: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
@@ -1029,15 +1029,15 @@
 00004040: ec48 4ecf 38f2 c441 0000 0012 0066 0065  .HN.8..A.....f.e
 00004050: 0061 0074 0075 0072 0065 005f 0065 0078  .a.t.u.r.e._.e.x
 00004060: 0074 0072 0061 0063 0074 006f 0072 0073  .t.r.a.c.t.o.r.s
 00004070: 6d6f 6444 626c 6f62 0000 0008 ec48 4ecf  modDblob.....HN.
 00004080: 38f2 c441 0000 0012 0066 0065 0061 0074  8..A.....f.e.a.t
 00004090: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
 000040a0: 0061 0063 0074 006f 0072 0073 7068 3153  .a.c.t.o.r.sph1S
-000040b0: 636f 6d70 0000 0000 0013 e000 0000 0012  comp............
+000040b0: 636f 6d70 0000 0000 0013 f000 0000 0012  comp............
 000040c0: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
 000040d0: 0065 0078 0074 0072 0061 0063 0074 006f  .e.x.t.r.a.c.t.o
 000040e0: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
 000040f0: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
 00004100: 6277 7370 626c 6f62 0000 00c9 6270 6c69  bwspblob....bpli
 00004110: 7374 3030 d701 0203 0405 0607 0808 0a08  st00............
 00004120: 0a0d 0a5d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
```

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/fish_feature_extractor_2023.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import division
 import numpy as np
 import math
+
+import pandas as pd
+
 from simba.read_config_unit_tests import (read_project_path_and_file_type,
                                           check_if_filepath_list_is_empty)
 from scipy.spatial import ConvexHull
 from scipy.spatial.qhull import QhullError
 from numba import jit, prange
 from simba.drop_bp_cords import *
 from simba.feature_extractors.unit_tests import read_video_info, check_minimum_roll_windows
 from simba.drop_bp_cords import get_fn_ext, getBpNames, getBpHeaders
-from simba.misc_tools import SimbaTimer
+from simba.misc_tools import SimbaTimer, detect_bouts
 from itertools import combinations
 from joblib import Parallel, delayed
 
 TAIL_BP_NAMES = ['objectA', 'peduncle_base']
 CENTER_BP_NAMES = ['midpoint']
 MOUTH = ['mouth']
 
@@ -48,15 +51,14 @@
 
         self.roll_windows_values = check_minimum_roll_windows([20, 15, 10, 4, 2], self.video_info_df['fps'].min())
         self.roll_windows_values = [x for x in self.roll_windows_values if x >= 2]
         self.files_found = glob.glob(self.input_file_dir + '/*.{}'.format(self.file_type))
         check_if_filepath_list_is_empty(filepaths=self.files_found, error_msg='SIMBA ERROR: No file in {} directory'.format(self.input_file_dir))
         print('Extracting features from {} {}...'.format(str(len(self.files_found)), 'file(s)'))
 
-
         for file_path in self.files_found:
             video_timer = SimbaTimer()
             video_timer.start_timer()
             dir_name, file_name, ext = get_fn_ext(file_path)
             self.save_path = os.path.join(self.save_dir, os.path.basename(file_path))
             video_info, self.px_per_mm, self.fps = read_video_info(self.video_info_df, file_name)
             self.video_width, self.video_height = video_info['Resolution_width'].values, video_info['Resolution_height'].values
@@ -71,15 +73,16 @@
             csv_df_shifted.columns = self.col_headers_shifted
             self.csv_df_combined = pd.concat([self.csv_df, csv_df_shifted], axis=1, join='inner').fillna(0)
             self.calc_X_relative_to_Y_movement()
             self.calc_movement()
             self.calc_X_relative_to_Y_movement_rolling_windows()
             self.calc_velocity()
             self.calc_rotation()
-            self.calc_direction_switches()
+            self.calc_N_degree_direction_switches()
+            self.calc_45_degree_direction_switches()
             self.hot_end_encode_compass()
             self.calc_directional_switches_in_rolling_windows()
             self.calc_angular_dispersion()
             self.calc_border_distances()
             self.calc_distances_between_body_part()
             self.calc_convex_hulls()
             self.pose_confidence_probabilities()
@@ -192,14 +195,34 @@
             currentColName = f'Directionality_of_switches_switches_{i}'
             self.csv_df_combined[currentColName] = self.csv_df_combined['Switch_direction_value'].rolling(i, min_periods=1).sum()
 
     def calc_velocity(self):
         for bp in self.bp_names:
             self.csv_df_combined[bp + '_velocity'] = self.csv_df_combined[bp + '_movement'].rolling(int(self.fps), min_periods=1).sum()
 
+    def calc_N_degree_direction_switches(self):
+        degree_lk_180 = {'N': ['S'], 'NE': ['SW'], 'E': ['W'], 'SE': ['NW']}
+        degree_lk_90 = {'N': ['W', 'E'], 'NE': ['NW', 'SE'], 'NW': ['SW', 'NE'], 'SW': ['NW', 'SE'], 'SE': ['NE', 'SW'], 'S': ['W', 'E'], 'E': ['N', 'S'], 'W': ['N', 'S']}
+        dg_df = pd.DataFrame(self.csv_df_combined['Compass_direction'])
+        for window in self.roll_windows_values:
+            dg_df[f'Compass_direction_{window}'] = dg_df['Compass_direction'].shift(window)
+            dg_df[f'Compass_direction_{window}'].fillna(dg_df['Compass_direction'], inplace=True)
+            dg_df[f'180_degree_switch_{window}'] = 0
+            dg_df[f'90_degree_switch_{window}'] = 0
+            for k, v in degree_lk_180.items():
+                for value in v:
+                    dg_df.loc[(dg_df['Compass_direction'] == k) & (dg_df[f'Compass_direction_{window}'] == value), f'180_degree_switch_{window}'] = 1
+                    dg_df.loc[(dg_df[f'Compass_direction_{window}'] == k) & (dg_df['Compass_direction'] == value), f'180_degree_switch_{window}'] = 1
+            for k, v in degree_lk_90.items():
+                for value in v:
+                    dg_df.loc[(dg_df['Compass_direction'] == k) & (dg_df[f'Compass_direction_{window}'] == value), f'90_degree_switch_{window}'] = 1
+                    dg_df.loc[(dg_df[f'Compass_direction_{window}'] == k) & (dg_df['Compass_direction'] == value), f'90_degree_switch_{window}'] = 1
+            self.csv_df_combined[f'180_degree_switch_{window}'] = dg_df[f'180_degree_switch_{window}']
+            self.csv_df_combined[f'90_degree_switch_{window}'] = dg_df[f'90_degree_switch_{window}']
+
     def calc_rotation(self):
         self.csv_df_combined['Clockwise_angle_degrees'] = self.csv_df_combined.apply(lambda x: self.angle2pt_degrees(x[CENTER_BP_NAMES[0] + '_x'], x[CENTER_BP_NAMES[0] + '_y'], x[TAIL_BP_NAMES[0] + '_x'], x[TAIL_BP_NAMES[0] + '_y']), axis=1)
         self.csv_df_combined['Angle_radians'] = self.angle2pt_radians(self.csv_df_combined['Clockwise_angle_degrees'])
         self.csv_df_combined['Angle_sin'] = self.csv_df_combined.apply(lambda x: self.angle2pt_sin(x['Angle_radians']),  axis=1)
         self.csv_df_combined['Angle_cos'] = self.csv_df_combined.apply(lambda x: self.angle2pt_cos(x['Angle_radians']), axis=1)
         self.csv_df_combined['Angle_sin_cumsum'] = self.csv_df_combined['Angle_sin'].cumsum()
         self.csv_df_combined['Angle_cos_cumsum'] = self.csv_df_combined['Angle_cos'].cumsum()
@@ -217,15 +240,15 @@
             self.csv_df_combined[column_name] = self.csv_df_combined['Clockwise_angle_degrees'].rolling(i, min_periods=1).mean()
 
     def hot_end_encode_compass(self):
         compass_hot_end = pd.get_dummies(self.csv_df_combined['Compass_direction'], prefix='Direction')
         compass_hot_end = compass_hot_end.T.reindex(self.compass_brackets_long).T.fillna(0)
         self.csv_df_combined = pd.concat([self.csv_df_combined, compass_hot_end], axis=1)
 
-    def calc_direction_switches(self):
+    def calc_45_degree_direction_switches(self):
         self.grouped_df = pd.DataFrame()
         v = (self.csv_df_combined['Compass_digit'] != self.csv_df_combined['Compass_digit'].shift()).cumsum()
         u = self.csv_df_combined.groupby(v)['Compass_digit'].agg(['all', 'count'])
         m = u['all'] & u['count'].ge(1)
         self.grouped_df['groups'] = self.csv_df_combined.groupby(v).apply(lambda x: (x.index[0], x.index[-1]))[m]
         currdirectionList, DirectionSwitchIndexList, currdirectionListValue = [], [], []
         for indexes, row in self.grouped_df.iterrows():
```

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 000012d0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 000012e0: 6261 7208 0809 0809 5f10 177b 7b35 302c  bar....._..{{50,
 000012f0: 2036 357d 2c20 7b31 3037 362c 2034 3531   65}, {1076, 451
 00001300: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
 00001310: 7e98 0000 0000 0000 0101 0000 0000 0000  ~...............
 00001320: 000f 0000 0000 0000 0000 0000 0000 0000  ................
 00001330: 0099 0000 0004 006d 0069 0073 0063 6c67  .......m.i.s.clg
-00001340: 3153 636f 6d70 0000 0000 0001 d3d1 0000  1Scomp..........
+00001340: 3153 636f 6d70 0000 0000 0001 dac4 0000  1Scomp..........
 00001350: 0004 006d 0069 0073 0063 6c73 7643 626c  ...m.i.s.clsvCbl
 00001360: 6f62 0000 02b0 6270 6c69 7374 3030 da01  ob....bplist00..
 00001370: 0203 0405 0607 0809 0a0b 0c0d 1848 4948  .............HIH
 00001380: 4a4b 0c5f 1012 7669 6577 4f70 7469 6f6e  JK._..viewOption
 00001390: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
 000013a0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
 000013b0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
@@ -391,19 +391,19 @@
 00001860: 6b01 6d01 6e01 6f01 7801 7a01 7c01 7d01  k.m.n.o.x.z.|.}.
 00001870: 7e01 8701 8901 8b01 8c01 8d01 9601 9801  ~...............
 00001880: 9a01 9b01 9c01 a501 a701 a901 aa01 ab01  ................
 00001890: b401 b501 b801 b901 bb01 bc01 c501 ce01  ................
 000018a0: d301 dc00 0000 0000 0002 0100 0000 0000  ................
 000018b0: 0000 4c00 0000 0000 0000 0000 0000 0000  ..L.............
 000018c0: 0001 dd00 0000 0400 6d00 6900 7300 636d  ........m.i.s.cm
-000018d0: 6f44 4462 6c6f 6200 0000 08f4 cb24 e0ff  oDDblob......$..
-000018e0: f0c4 4100 0000 0400 6d00 6900 7300 636d  ..A.....m.i.s.cm
-000018f0: 6f64 4462 6c6f 6200 0000 08f4 cb24 e0ff  odDblob......$..
-00001900: f0c4 4100 0000 0400 6d00 6900 7300 6370  ..A.....m.i.s.cp
-00001910: 6831 5363 6f6d 7000 0000 0000 0270 0000  h1Scomp......p..
+000018d0: 6f44 4462 6c6f 6200 0000 0848 ebac 9be4  oDDblob....H....
+000018e0: f2c4 4100 0000 0400 6d00 6900 7300 636d  ..A.....m.i.s.cm
+000018f0: 6f64 4462 6c6f 6200 0000 0848 ebac 9be4  odDblob....H....
+00001900: f2c4 4100 0000 0400 6d00 6900 7300 6370  ..A.....m.i.s.cp
+00001910: 6831 5363 6f6d 7000 0000 0000 0280 0000  h1Scomp.........
 00001920: 0000 0400 6d00 6900 7300 6376 5372 6e6c  ....m.i.s.cvSrnl
 00001930: 6f6e 6700 0000 0100 0000 0000 0000 0000  ong.............
 00001940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/extract_features_9bp.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/extract_features_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/unit_tests.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.56.2/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotly_create_h5.py` & `Simba-UW-tf-dev-1.56.2/simba/plotly_create_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/requirements.txt` & `Simba-UW-tf-dev-1.56.2/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/severity_processor.py` & `Simba-UW-tf-dev-1.56.2/simba/severity_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/user_pose_config_creator.py` & `Simba-UW-tf-dev-1.56.2/simba/user_pose_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.56.2/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.56.2/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.56.2/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/machine_model_settings_pop_up.py` & `Simba-UW-tf-dev-1.56.2/simba/machine_model_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/remove_keypoints_in_pose.py` & `Simba-UW-tf-dev-1.56.2/simba/remove_keypoints_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.56.2/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/multi_cropper.py` & `Simba-UW-tf-dev-1.56.2/simba/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/FSTTC_calculator.py` & `Simba-UW-tf-dev-1.56.2/simba/FSTTC_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/create_project_pop_up.py` & `Simba-UW-tf-dev-1.56.2/simba/create_project_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/video_info_table.py` & `Simba-UW-tf-dev-1.56.2/simba/video_info_table.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.56.2/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/extract_frames_fast.py` & `Simba-UW-tf-dev-1.56.2/simba/extract_frames_fast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.56.2/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.56.2/simba/utils/lookups.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,7 +99,8 @@
 
 
 
 
 
 
 
+
```

### Comparing `Simba-UW-tf-dev-1.56.1/simba/utils/errors.py` & `Simba-UW-tf-dev-1.56.2/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/utils/printing.py` & `Simba-UW-tf-dev-1.56.2/simba/utils/printing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from simba.enums import TagNames, Defaults
 
 def stdout_success(msg: str, elapsed_time: str or None=None) -> None:
     if elapsed_time:
-        print(f'SIMBA COMPLETE: {msg} (elapsed time: {elapsed_time}) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.COMPLETE.value}')
+        print(f'SIMBA COMPLETE: {msg} (elapsed time: {elapsed_time}s) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.COMPLETE.value}')
     else:
         print(f'SIMBA COMPLETE: {msg} {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.COMPLETE.value}')
 
 def stdout_warning(msg: str, elapsed_time: str or None=None) -> None:
     if elapsed_time:
-        print(f'SIMBA WARNING: {msg} (elapsed time: {elapsed_time}) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.WARNING.value}')
+        print(f'SIMBA WARNING: {msg} (elapsed time: {elapsed_time}s) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.WARNING.value}')
     else:
         print(f'SIMBA WARNING: {msg} {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.WARNING.value}')
 
 def stdout_trash(msg: str, elapsed_time: str or None=None) -> None:
     if elapsed_time:
-        print(f'SIMBA COMPLETE: {msg} (elapsed time: {elapsed_time}) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.TRASH.value}')
+        print(f'SIMBA COMPLETE: {msg} (elapsed time: {elapsed_time}s) {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.TRASH.value}')
     else:
         print(f'SIMBA COMPLETE: {msg} {Defaults.STR_SPLIT_DELIMITER.value}{TagNames.TRASH.value}')
```

### Comparing `Simba-UW-tf-dev-1.56.1/simba/labelling_interface.py` & `Simba-UW-tf-dev-1.56.2/simba/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/timebins_movement_analyzer.py` & `Simba-UW-tf-dev-1.56.2/simba/timebins_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/train_model_functions.py` & `Simba-UW-tf-dev-1.56.2/simba/train_model_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.56.2/simba/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/timebins_clf_analyzer.py` & `Simba-UW-tf-dev-1.56.2/simba/timebins_clf_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/calculate_px_dist.py` & `Simba-UW-tf-dev-1.56.2/simba/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/movement_processor.py` & `Simba-UW-tf-dev-1.56.2/simba/movement_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pybursts.py` & `Simba-UW-tf-dev-1.56.2/simba/pybursts.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/reverse_2_animal_tracking.py` & `Simba-UW-tf-dev-1.56.2/simba/reverse_2_animal_tracking.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/Directing_animals_analyzer.py` & `Simba-UW-tf-dev-1.56.2/simba/Directing_animals_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/Validate_model_one_video_run_clf.py` & `Simba-UW-tf-dev-1.56.2/simba/Validate_model_one_video_run_clf.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from simba.read_config_unit_tests import (read_config_file,
                                           check_file_exist_and_readable,
                                           read_project_path_and_file_type)
 
 from simba.rw_dfs import (read_df,
                           save_df)
-from simba.train_model_functions import read_pickle
+from simba.train_model_functions import (read_pickle,
+                                         clf_predict_proba)
 from simba.drop_bp_cords import (get_fn_ext,
                                  drop_bp_cords)
 from copy import deepcopy
 from simba.utils.printing import stdout_success
 from simba.utils.errors import FeatureNumberMismatchError
 import warnings
 import time
@@ -56,33 +57,16 @@
         check_file_exist_and_readable(clf_path)
         _, file_name, _ = get_fn_ext(str(input_file_path))
         _, classifier_name, _ = get_fn_ext(clf_path)
         data_df = read_df(input_file_path, self.file_type)
         output_df = deepcopy(data_df)
         data_df = drop_bp_cords(data_df, config_path)
         clf = read_pickle(file_path=clf_path)
-        probability_col_name = 'Probability_{}'.format(classifier_name)
-
-        try:
-            prediction = clf.predict_proba(data_df)
-        except ValueError as e:
-            vals = [int(s) for s in e.args[0].split() if s.isdigit()]
-            if len(vals) == 2:
-                raise FeatureNumberMismatchError(msg=f'Mismatch in the number of features in selected input file ({file_name}) and what is expected from the selected model ({classifier_name}). The model expects {str(vals[0])} features, but the file contains {str(vals[1])} features.')
-            else:
-                print(e.args)
-                raise ValueError
-
-        try:
-            output_df[probability_col_name] = prediction[:, 1]
-        except IndexError as e:
-            print(e.args)
-            print('SIMBA INDEXERROR: Your classifier has not been created properly. See The SimBA GitHub FAQ page for more information and suggested fixes.')
-            raise IndexError
-
+        probability_col_name = f'Probability_{classifier_name}'
+        output_df[probability_col_name] = clf_predict_proba(clf=clf, x_df=data_df)
         save_filename = os.path.join(self.save_path, file_name + '.' + self.file_type)
         save_df(output_df, self.file_type, save_filename)
         elapsed_time = str(round(time.time() - self.start_time, 2))
 
         stdout_success(msg=f'Validation predictions generated for "{file_name}" within the project_folder/csv/validation directory', elapsed_time=elapsed_time)
         print('Click on "Interactive probability plot" to inspect classifier probability thresholds. If satisfactory proceed to specify threshold and minimum bout length and click on "Validate" to create video.')
 #
```

### Comparing `Simba-UW-tf-dev-1.56.1/simba/tkinter_functions.py` & `Simba-UW-tf-dev-1.56.2/simba/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/setting_menu.py` & `Simba-UW-tf-dev-1.56.2/simba/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/interpolate_pose.py` & `Simba-UW-tf-dev-1.56.2/simba/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/run_inference.py` & `Simba-UW-tf-dev-1.56.2/simba/run_inference.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/misc_visualizations.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/misc_visualizations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.56.2/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.56.2/simba/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/interpolate_smooth_post_hoc.py` & `Simba-UW-tf-dev-1.56.2/simba/interpolate_smooth_post_hoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/dash_app.py` & `Simba-UW-tf-dev-1.56.2/simba/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/reverse_tracking_order.py` & `Simba-UW-tf-dev-1.56.2/simba/reverse_tracking_order.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/concatenator_pop_up.py` & `Simba-UW-tf-dev-1.56.2/simba/concatenator_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/extract_annotation_frames.py` & `Simba-UW-tf-dev-1.56.2/simba/extract_annotation_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.56.2/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/misc_tools.py` & `Simba-UW-tf-dev-1.56.2/simba/misc_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.56.2/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.56.2/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.56.2/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.56.2/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.56.2/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_importers/import_trk.py` & `Simba-UW-tf-dev-1.56.2/simba/pose_importers/import_trk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.56.2/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.56.2/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.56.2/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pop_up_classes.py` & `Simba-UW-tf-dev-1.56.2/simba/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/extract_seqframes.py` & `Simba-UW-tf-dev-1.56.2/simba/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.56.2/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/get_coordinates_tools_v2.py` & `Simba-UW-tf-dev-1.56.2/simba/get_coordinates_tools_v2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pup_retrieval_protocol.py` & `Simba-UW-tf-dev-1.56.2/simba/pup_retrieval_protocol.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.56.2/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/pose_reset.py` & `Simba-UW-tf-dev-1.56.2/simba/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/train_mutiple_models.py` & `Simba-UW-tf-dev-1.56.2/simba/train_mutiple_models.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/SimBA.py` & `Simba-UW-tf-dev-1.56.2/simba/SimBA.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 from simba.bounding_box_tools.boundary_menus import BoundaryMenus
 from simba.labelling_interface import select_labelling_video
 from simba.labelling_advanced_interface import select_labelling_video_advanced
 from simba.enums import (Formats,
                          OS,
                          Defaults,
                          TagNames)
+from simba.utils.errors import InvalidInputError
 from simba.utils.lookups import get_bp_config_code_class_pairs, get_icons_paths
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.create_project_pop_up import ProjectCreatorPopUp
 from simba.plotly_create_h5 import create_plotly_container
 from simba.utils.lookups import get_emojis
 #from simba.unsupervised.unsupervised_ui import UnsupervisedGUI
 import sys
@@ -817,24 +818,34 @@
         links_menu.add_command(label='Gitter Chatroom', command=lambda: webbrowser.open_new(str(r'https://gitter.im/SimBA-Resource/community')))
         links_menu.add_command(label='Install FFmpeg',command =lambda: webbrowser.open_new(str(r'https://m.wikihow.com/Install-FFmpeg-on-Windows')))
         links_menu.add_command(label='Install graphviz', command=lambda: webbrowser.open_new(str(r'https://bobswift.atlassian.net/wiki/spaces/GVIZ/pages/20971549/How+to+install+Graphviz+software')))
         help_menu.add_cascade(label="Links",menu=links_menu, compound='left', image=self.menu_icons['link']['img'])
         help_menu.add_command(label='About', compound='left', image=self.menu_icons['about']['img'], command=AboutSimBAPopUp)
 
         self.frame = Frame(background, bd=2, relief=SUNKEN, width=750, height=300)
+        self.r_click_menu = Menu(self.root, tearoff=0)
+        self.r_click_menu.add_command(label="Copy selection", command=lambda: self.copy_selection_to_clipboard())
+        self.r_click_menu.add_command(label="Copy all", command=lambda: self.copy_all_to_clipboard())
+        self.r_click_menu.add_command(label="Paste", command=lambda: self.paste_to_txt())
+        self.r_click_menu.add_separator()
+        self.r_click_menu.add_command(label="Clear", command=lambda: self.clean_txt())
         y_sb = Scrollbar(self.frame, orient=VERTICAL)
         self.frame.pack(expand=True)
         self.txt = Text(self.frame, bg='white', insertborderwidth=2, height=30, width=100, yscrollcommand=y_sb)
+        if currentPlatform == OS.WINDOWS.value:
+            self.txt.bind("<Button-3>", self.show_right_click_pop_up)
+        if currentPlatform == OS.MAC.value:
+            self.txt.bind("<Button-2>", self.show_right_click_pop_up)
         self.txt.tag_configure(TagNames.GREETING.value, justify='center', foreground='blue', font=("Rockwell", 16, 'bold'))
         self.txt.tag_configure(TagNames.ERROR.value, justify='left', foreground='red', font=Formats.TKINTER_FONT.value)
         self.txt.tag_configure(TagNames.STANDARD.value, justify='left', foreground='black', font=Formats.TKINTER_FONT.value)
-        self.txt.tag_configure(TagNames.COMPLETE.value, justify='left', foreground='blue', font=Formats.TKINTER_FONT.value)
+        self.txt.tag_configure(TagNames.COMPLETE.value, justify='left', foreground='darkgreen', font=Formats.TKINTER_FONT.value)
         self.txt.tag_configure(TagNames.WARNING.value, justify='left', foreground='darkorange', font=Formats.TKINTER_FONT.value)
         self.txt.insert(INSERT, Defaults.WELCOME_MSG.value + emojis['relaxed'] + '\n' * 2)
-        self.txt.tag_add(TagNames.GREETING.value, "1.0", "2.25")
+        self.txt.tag_add(TagNames.GREETING.value, "1.0", "3.25")
         y_sb.pack(side=RIGHT, fill=Y)
         self.txt.pack(expand=True, fill='both')
         y_sb.config(command=self.txt.yview)
         self.txt.config(state=DISABLED, font=Formats.TKINTER_FONT.value)
 
         clear_txt_btn = Button(self.frame, text=' CLEAR', compound=LEFT, image=self.menu_icons['clean']['img'], font=Formats.LABELFRAME_HEADER_FORMAT.value, command=lambda: self.clean_txt())
         clear_txt_btn.pack(side=BOTTOM, fill=X)
@@ -848,14 +859,36 @@
             python = sys.executable
             os.execl(python, python, *sys.argv)
 
     def clean_txt(self):
         self.txt.config(state=NORMAL)
         self.txt.delete('1.0', END)
 
+    def show_right_click_pop_up(self, event):
+        try:
+            self.r_click_menu.tk_popup(event.x_root, event.y_root)
+        finally:
+            self.r_click_menu.grab_release()
+
+    def copy_selection_to_clipboard(self):
+        self.root.clipboard_clear()
+        text = self.txt.get('sel.first', 'sel.last')
+        text = text.encode("ascii", "ignore").decode()
+        self.root.clipboard_append(text)
+
+    def copy_all_to_clipboard(self):
+        self.root.clipboard_clear()
+        self.root.clipboard_append(self.txt.get("1.0", "end-1c"))
+
+    def paste_to_txt(self):
+        try:
+            print(self.root.clipboard_get())
+        except UnicodeDecodeError:
+            raise InvalidInputError(msg='Can only paste utf-8 compatible text')
+
 class StdRedirector(object):
     def __init__(self, text_widget):
         self.text_space = text_widget
         self.emojis = get_emojis()
 
     def write(self, s: str):
         tag_name = TagNames.STANDARD.value
```

### Comparing `Simba-UW-tf-dev-1.56.1/simba/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.56.2/simba/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.56.2/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.56.2/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/assets/.DS_Store`

 * *Files 7% similar despite different names*

```diff
@@ -491,30 +491,30 @@
 00001ea0: 01c5 1af0 c441 0000 0005 0069 0063 006f  .....A.....i.c.o
 00001eb0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
 00001ec0: da62 afb9 1af0 c441 0000 0005 0069 0063  .b.....A.....i.c
 00001ed0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
 00001ee0: 0000 0007 f000 0000 0005 0069 0063 006f  ...........i.c.o
 00001ef0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00001f00: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
-00001f10: 6f62 0000 00c7 6270 6c69 7374 3030 d701  ob....bplist00..
+00001f10: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
 00001f20: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00001f30: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00001f40: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00001f50: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00001f60: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00001f70: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00001f80: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00001f90: 0809 0809 5f10 167b 7b30 2c20 3230 307d  ...._..{{0, 200}
-00001fa0: 2c20 7b37 3730 2c20 3433 367d 7d09 0817  , {770, 436}}...
-00001fb0: 2531 3d49 606d 797a 7b7c 7d7e 9700 0000  %1=I`myz{|}~....
-00001fc0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-00001fd0: 0000 0000 0000 0000 0000 0000 9800 0000  ................
-00001fe0: 0300 6900 6d00 676c 6731 5363 6f6d 7000  ..i.m.glg1Scomp.
-00001ff0: 0000 0000 1424 d500 0000 0300 6900 6d00  .....$......i.m.
-00002000: 676c 7376 0000 0000 0000 0012 0000 0005  glsv............
+00001f90: 0809 0809 5f10 197b 7b33 3838 2c20 3231  ...._..{{388, 21
+00001fa0: 367d 2c20 7b31 3039 322c 2034 3232 7d7d  6}, {1092, 422}}
+00001fb0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
+00001fc0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
+00001fd0: 0000 0000 0000 0000 0000 0000 0000 009b  ................
+00001fe0: 0000 0003 0069 006d 0067 6c67 3153 636f  .....i.m.glg1Sco
+00001ff0: 6d70 0000 0000 0011 10bf 0000 0003 0069  mp.............i
+00002000: 006d 0067 0000 0000 0000 0012 0000 0005  .m.g............
 00002010: 0069 0063 006f 006e 0073 6277 7370 626c  .i.c.o.n.sbwspbl
 00002020: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
 00002030: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00002040: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00002050: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00002060: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00002070: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
@@ -619,139 +619,139 @@
 000026a0: afb9 1af0 c441 0000 0005 0069 0063 006f  .....A.....i.c.o
 000026b0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
 000026c0: da62 afb9 1af0 c441 0000 0005 0069 0063  .b.....A.....i.c
 000026d0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
 000026e0: 0000 0007 f000 0000 0005 0069 0063 006f  ...........i.c.o
 000026f0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00002700: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
-00002710: 6f62 0000 00c7 6270 6c69 7374 3030 d701  ob....bplist00..
+00002710: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
 00002720: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00002730: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00002740: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00002750: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00002760: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00002770: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00002780: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00002790: 0809 0809 5f10 167b 7b30 2c20 3230 307d  ...._..{{0, 200}
-000027a0: 2c20 7b37 3730 2c20 3433 367d 7d09 0817  , {770, 436}}...
-000027b0: 2531 3d49 606d 797a 7b7c 7d7e 9700 0000  %1=I`myz{|}~....
-000027c0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-000027d0: 0000 0000 0000 0000 0000 0000 9800 0000  ................
-000027e0: 0300 6900 6d00 676c 6731 5363 6f6d 7000  ..i.m.glg1Scomp.
-000027f0: 0000 0000 1424 d500 0000 0300 6900 6d00  .....$......i.m.
-00002800: 676c 7376 4362 6c6f 6200 0002 b062 706c  glsvCblob....bpl
-00002810: 6973 7430 30da 0102 0304 0506 0708 090a  ist00...........
-00002820: 0b0c 0d18 4849 484a 0c4c 5869 636f 6e53  ....HIHJ.LXiconS
-00002830: 697a 655f 100f 7368 6f77 4963 6f6e 5072  ize_..showIconPr
-00002840: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00002850: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-00002860: 735f 100f 7363 726f 6c6c 506f 7369 7469  s_..scrollPositi
-00002870: 6f6e 5958 7465 7874 5369 7a65 5f10 0f73  onYXtextSize_..s
-00002880: 6372 6f6c 6c50 6f73 6974 696f 6e58 5a73  crollPositionXZs
-00002890: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
-000028a0: 656c 6174 6976 6544 6174 6573 5f10 1276  elativeDates_..v
-000028b0: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
-000028c0: 6e23 4030 0000 0000 0000 09ab 0e17 1c21  n#@0...........!
-000028d0: 252a 2f34 393e 43d4 0f10 1112 0c14 0c16  %*/49>C.........
-000028e0: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-000028f0: 7363 656e 6469 6e67 5a69 6465 6e74 6966  scendingZidentif
-00002900: 6965 7209 1101 2709 546e 616d 65d4 0f10  ier...'.Tname...
-00002910: 1112 1819 181b 0810 2308 5875 6269 7175  ........#.Xubiqu
-00002920: 6974 79d4 0f10 1112 0c1e 1820 0910 b508  ity........ ....
-00002930: 5c64 6174 654d 6f64 6966 6965 64d4 0f10  \dateModified...
-00002940: 1112 181e 1824 0808 5b64 6174 6543 7265  .....$..[dateCre
-00002950: 6174 6564 d40f 1011 120c 2718 2909 1061  ated......'.)..a
-00002960: 0854 7369 7a65 d40f 1011 120c 2c0c 2e09  .Tsize......,...
-00002970: 1073 0954 6b69 6e64 d40f 1011 1218 310c  .s.Tkind......1.
-00002980: 3308 1064 0955 6c61 6265 6cd4 0f10 1112  3..d.Ulabel.....
-00002990: 1836 0c38 0810 4b09 5776 6572 7369 6f6e  .6.8..K.Wversion
-000029a0: d40f 1011 1218 3b0c 3d08 1101 2c09 5863  ......;.=...,.Xc
-000029b0: 6f6d 6d65 6e74 73d4 0f10 1112 1840 1842  omments......@.B
-000029c0: 0810 c808 5e64 6174 654c 6173 744f 7065  ....^dateLastOpe
-000029d0: 6e65 64d4 0f10 1112 181e 1846 0808 5964  ned........F..Yd
-000029e0: 6174 6541 6464 6564 0823 0000 0000 0000  ateAdded.#......
-000029f0: 0000 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
-00002a00: 0910 0100 0800 1d00 2600 3800 4000 5400  ........&.8.@.T.
-00002a10: 6600 6f00 8100 8c00 9f00 b400 bd00 be00  f.o.............
-00002a20: ca00 d300 db00 e100 eb00 f600 f700 fa00  ................
-00002a30: fb01 0001 0901 0a01 0c01 0d01 1601 1f01  ................
-00002a40: 2001 2201 2301 3001 3901 3a01 3b01 4701   .".#.0.9.:.;.G.
-00002a50: 5001 5101 5301 5401 5901 6201 6301 6501  P.Q.S.T.Y.b.c.e.
-00002a60: 6601 6b01 7401 7501 7701 7801 7e01 8701  f.k.t.u.w.x.~...
-00002a70: 8801 8a01 8b01 9301 9c01 9d01 a001 a101  ................
-00002a80: aa01 b301 b401 b601 b701 c601 cf01 d001  ................
-00002a90: d101 db01 dc01 e501 ee01 f301 f400 0000  ................
-00002aa0: 0000 0002 0100 0000 0000 0000 4d00 0000  ............M...
-00002ab0: 0000 0000 0000 0000 0000 0001 f600 0000  ................
-00002ac0: 0300 6900 6d00 676c 7376 7062 6c6f 6200  ..i.m.glsvpblob.
-00002ad0: 0002 9562 706c 6973 7430 30da 0102 0304  ...bplist00.....
-00002ae0: 0506 0708 090a 0b0c 0d1f 4849 484a 0c26  ..........HIHJ.&
-00002af0: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
-00002b00: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-00002b10: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-00002b20: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
-00002b30: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
-00002b40: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
-00002b50: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e5f  ionXZsortColumn_
-00002b60: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-00002b70: 6573 5f10 1276 6965 774f 7074 696f 6e73  es_..viewOptions
-00002b80: 5665 7273 696f 6e23 4030 0000 0000 0000  Version#@0......
-00002b90: 09d9 0e0f 1011 1213 1415 1617 2025 2a2e  ............ %*.
-00002ba0: 3338 3d42 5863 6f6d 6d65 6e74 735e 6461  38=BXcomments^da
-00002bb0: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
-00002bc0: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
-00002bd0: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
-00002be0: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
-00002bf0: 6d65 d418 191a 1b1c 1d0c 1f55 696e 6465  me.........Uinde
-00002c00: 7855 7769 6474 6859 6173 6365 6e64 696e  xUwidthYascendin
-00002c10: 6757 7669 7369 626c 6510 0711 012c 0908  gWvisible....,..
-00002c20: d418 191a 1b21 221f 1f10 0810 c808 08d4  .....!".........
-00002c30: 1819 1a1b 2627 1f0c 1001 10b5 0809 d418  ....&'..........
-00002c40: 191a 1b2b 271f 1f10 0208 08d4 1819 1a1b  ...+'...........
-00002c50: 2f30 1f0c 1003 1061 0809 d418 191a 1b34  /0.....a.......4
-00002c60: 350c 1f10 0510 6409 08d4 1819 1a1b 393a  5.....d.......9:
-00002c70: 0c0c 1004 1073 0909 d418 191a 1b3e 3f0c  .....s.......>?.
-00002c80: 1f10 0610 4b09 08d4 1819 1a1b 4344 0c0c  ....K.......CD..
-00002c90: 1000 1101 2709 0908 2300 0000 0000 0000  ....'...#.......
-00002ca0: 0023 4028 0000 0000 0000 546e 616d 6509  .#@(......Tname.
-00002cb0: 0008 001d 0026 0038 0040 0054 0066 006f  .....&.8.@.T.f.o
-00002cc0: 0081 008c 009f 00b4 00bd 00be 00d1 00da  ................
-00002cd0: 00e9 00f6 0102 0107 010d 0112 011a 011f  ................
-00002ce0: 0128 012e 0134 013e 0146 0148 014b 014c  .(...4.>.F.H.K.L
-00002cf0: 014d 0156 0158 015a 015b 015c 0165 0167  .M.V.X.Z.[.\.e.g
-00002d00: 0169 016a 016b 0174 0176 0177 0178 0181  .i.j.k.t.v.w.x..
-00002d10: 0183 0185 0186 0187 0190 0192 0194 0195  ................
-00002d20: 0196 019f 01a1 01a3 01a4 01a5 01ae 01b0  ................
-00002d30: 01b2 01b3 01b4 01bd 01bf 01c2 01c3 01c4  ................
-00002d40: 01c5 01ce 01d7 01dc 0000 0000 0000 0201  ................
-00002d50: 0000 0000 0000 004c 0000 0000 0000 0000  .......L........
-00002d60: 0000 0000 0000 01dd 0000 0003 0069 006d  .............i.m
-00002d70: 0067 6d6f 4444 626c 6f62 0000 0008 affb  .gmoDDblob......
-00002d80: 97b4 53f2 c441 0000 0003 0069 006d 0067  ..S..A.....i.m.g
-00002d90: 6d6f 6444 626c 6f62 0000 0008 affb 97b4  modDblob........
-00002da0: 53f2 c441 0000 0003 0069 006d 0067 7068  S..A.....i.m.gph
-00002db0: 3153 636f 6d70 0000 0000 0014 4000 0000  1Scomp......@...
-00002dc0: 0003 0069 006d 0067 7653 726e 6c6f 6e67  ...i.m.gvSrnlong
-00002dd0: 0000 0001 0000 0007 006c 006f 006f 006b  .........l.o.o.k
-00002de0: 0075 0070 0073 6277 7370 626c 6f62 0000  .u.p.sbwspblob..
-00002df0: 00c8 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-00002e00: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
-00002e10: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-00002e20: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-00002e30: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00002e40: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00002e50: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-00002e60: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
-00002e70: 5f10 177b 7b30 2c20 3131 367d 2c20 7b31  _..{{0, 116}, {1
-00002e80: 3235 302c 2037 3631 7d7d 0908 1725 313d  250, 761}}...%1=
-00002e90: 4960 6d79 7a7b 7c7d 7e98 0000 0000 0000  I`myz{|}~.......
-00002ea0: 0101 0000 0000 0000 000f 0000 0000 0000  ................
-00002eb0: 0000 0000 0000 0000 0099 0000 0007 006c  ...............l
-00002ec0: 006f 006f 006b 0075 0070 0073 6c67 3153  .o.o.k.u.p.slg1S
-00002ed0: 636f 6d70 0000 0000 0004 b1fb 0000 0000  comp............
+00002790: 0809 0809 5f10 197b 7b33 3838 2c20 3231  ...._..{{388, 21
+000027a0: 367d 2c20 7b31 3039 322c 2034 3232 7d7d  6}, {1092, 422}}
+000027b0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
+000027c0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
+000027d0: 0000 0000 0000 0000 0000 0000 0000 009b  ................
+000027e0: 0000 0003 0069 006d 0067 6c67 3153 636f  .....i.m.glg1Sco
+000027f0: 6d70 0000 0000 0011 10bf 0000 0003 0069  mp.............i
+00002800: 006d 0067 6c73 7643 626c 6f62 0000 02b0  .m.glsvCblob....
+00002810: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
+00002820: 0809 0a0b 0c0d 1a48 4948 4a0c 4c5f 1012  .......HIHJ.L_..
+00002830: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00002840: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00002850: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00002860: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00002870: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+00002880: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
+00002890: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
+000028a0: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+000028b0: 6c61 7469 7665 4461 7465 7358 6963 6f6e  lativeDatesXicon
+000028c0: 5369 7a65 1001 09ab 0e17 1c21 252a 2f34  Size.......!%*/4
+000028d0: 393e 43d4 0f10 1112 1314 0c0c 5a69 6465  9>C.........Zide
+000028e0: 6e74 6966 6965 7255 7769 6474 6859 6173  ntifierUwidthYas
+000028f0: 6365 6e64 696e 6757 7669 7369 626c 6554  cendingWvisibleT
+00002900: 6e61 6d65 1101 3709 09d4 0f10 1112 1819  name..7.........
+00002910: 1a1a 5875 6269 7175 6974 7910 2308 08d4  ..Xubiquity.#...
+00002920: 0f10 1112 1d1e 1a0c 5c64 6174 654d 6f64  ........\dateMod
+00002930: 6966 6965 6410 b508 09d4 0f10 1112 221e  ified.........".
+00002940: 1a1a 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
+00002950: d40f 1011 1226 271a 0c54 7369 7a65 1061  .....&'..Tsize.a
+00002960: 0809 d40f 1011 122b 2c0c 0c54 6b69 6e64  .......+,..Tkind
+00002970: 1073 0909 d40f 1011 1230 310c 1a55 6c61  .s.......01..Ula
+00002980: 6265 6c10 6409 08d4 0f10 1112 3536 0c1a  bel.d.......56..
+00002990: 5776 6572 7369 6f6e 104b 0908 d40f 1011  Wversion.K......
+000029a0: 123a 3b0c 1a58 636f 6d6d 656e 7473 1101  .:;..Xcomments..
+000029b0: 2c09 08d4 0f10 1112 3f40 1a1a 5e64 6174  ,.......?@..^dat
+000029c0: 654c 6173 744f 7065 6e65 6410 c808 08d4  eLastOpened.....
+000029d0: 0f10 1112 441e 1a1a 5964 6174 6541 6464  ....D...YdateAdd
+000029e0: 6564 0808 0823 0000 0000 0000 0000 2340  ed...#........#@
+000029f0: 2800 0000 0000 0054 6e61 6d65 0923 4030  (......Tname.#@0
+00002a00: 0000 0000 0000 0008 001d 0032 0044 004c  ...........2.D.L
+00002a10: 0060 0072 007b 008d 0098 00ab 00b4 00b6  .`.r.{..........
+00002a20: 00b7 00c3 00cc 00d7 00dd 00e7 00ef 00f4  ................
+00002a30: 00f7 00f8 00f9 0102 010b 010d 010e 010f  ................
+00002a40: 0118 0125 0127 0128 0129 0132 013e 013f  ...%.'.(.).2.>.?
+00002a50: 0140 0149 014e 0150 0151 0152 015b 0160  .@.I.N.P.Q.R.[.`
+00002a60: 0162 0163 0164 016d 0173 0175 0176 0177  .b.c.d.m.s.u.v.w
+00002a70: 0180 0188 018a 018b 018c 0195 019e 01a1  ................
+00002a80: 01a2 01a3 01ac 01bb 01bd 01be 01bf 01c8  ................
+00002a90: 01d2 01d3 01d4 01d5 01de 01e7 01ec 01ed  ................
+00002aa0: 0000 0000 0000 0201 0000 0000 0000 004d  ...............M
+00002ab0: 0000 0000 0000 0000 0000 0000 0000 01f6  ................
+00002ac0: 0000 0003 0069 006d 0067 6c73 7670 626c  .....i.m.glsvpbl
+00002ad0: 6f62 0000 0295 6270 6c69 7374 3030 da01  ob....bplist00..
+00002ae0: 0203 0405 0607 0809 0a0b 0c0d 1c47 4847  .............GHG
+00002af0: 490c 4b5f 1012 7669 6577 4f70 7469 6f6e  I.K_..viewOption
+00002b00: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
+00002b10: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
+00002b20: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
+00002b30: 6c53 697a 6573 5f10 0f73 6372 6f6c 6c50  lSizes_..scrollP
+00002b40: 6f73 6974 696f 6e59 5874 6578 7453 697a  ositionYXtextSiz
+00002b50: 655f 100f 7363 726f 6c6c 506f 7369 7469  e_..scrollPositi
+00002b60: 6f6e 585a 736f 7274 436f 6c75 6d6e 5f10  onXZsortColumn_.
+00002b70: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
+00002b80: 7358 6963 6f6e 5369 7a65 1001 09d9 0e0f  sXiconSize......
+00002b90: 1011 1213 1415 1617 2025 292d 3237 3c41  ........ %)-27<A
+00002ba0: 5863 6f6d 6d65 6e74 735e 6461 7465 4c61  Xcomments^dateLa
+00002bb0: 7374 4f70 656e 6564 5c64 6174 654d 6f64  stOpened\dateMod
+00002bc0: 6966 6965 645b 6461 7465 4372 6561 7465  ified[dateCreate
+00002bd0: 6454 7369 7a65 556c 6162 656c 546b 696e  dTsizeUlabelTkin
+00002be0: 6457 7665 7273 696f 6e54 6e61 6d65 d418  dWversionTname..
+00002bf0: 191a 1b1c 1d0c 1f57 7669 7369 626c 6555  .......WvisibleU
+00002c00: 7769 6474 6859 6173 6365 6e64 696e 6755  widthYascendingU
+00002c10: 696e 6465 7808 1101 2c09 1007 d418 191a  index...,.......
+00002c20: 1b1c 221c 2408 10c8 0810 08d4 1819 1a1b  ..".$...........
+00002c30: 0c27 1c0b 0910 b508 d418 191a 1b1c 271c  .'............'.
+00002c40: 2c08 0810 02d4 1819 1a1b 0c2f 1c31 0910  ,........../.1..
+00002c50: 6108 1003 d418 191a 1b1c 340c 3608 1064  a.........4.6..d
+00002c60: 0910 05d4 1819 1a1b 0c39 0c3b 0910 7309  .........9.;..s.
+00002c70: 1004 d418 191a 1b1c 3e0c 4008 104b 0910  ........>.@..K..
+00002c80: 06d4 1819 1a1b 0c43 0c45 0911 0137 0910  .......C.E...7..
+00002c90: 0008 2300 0000 0000 0000 0023 4028 0000  ..#........#@(..
+00002ca0: 0000 0000 546e 616d 6509 2340 3000 0000  ....Tname.#@0...
+00002cb0: 0000 0000 0800 1d00 3200 4400 4c00 6000  ........2.D.L.`.
+00002cc0: 7200 7b00 8d00 9800 ab00 b400 b600 b700  r.{.............
+00002cd0: ca00 d300 e200 ef00 fb01 0001 0601 0b01  ................
+00002ce0: 1301 1801 2101 2901 2f01 3901 3f01 4001  ....!.)./.9.?.@.
+00002cf0: 4301 4401 4601 4f01 5001 5201 5301 5501  C.D.F.O.P.R.S.U.
+00002d00: 5e01 5f01 6101 6201 6b01 6c01 6d01 6f01  ^._.a.b.k.l.m.o.
+00002d10: 7801 7901 7b01 7c01 7e01 8701 8801 8a01  x.y.{.|.~.......
+00002d20: 8b01 8d01 9601 9701 9901 9a01 9c01 a501  ................
+00002d30: a601 a801 a901 ab01 b401 b501 b801 b901  ................
+00002d40: bb01 bc01 c501 ce01 d301 d400 0000 0000  ................
+00002d50: 0002 0100 0000 0000 0000 4c00 0000 0000  ..........L.....
+00002d60: 0000 0000 0000 0000 0001 dd00 0000 0300  ................
+00002d70: 6900 6d00 676d 6f44 4462 6c6f 6200 0000  i.m.gmoDDblob...
+00002d80: 0869 d309 0c67 f2c4 4100 0000 0300 6900  .i...g..A.....i.
+00002d90: 6d00 676d 6f64 4462 6c6f 6200 0000 0869  m.gmodDblob....i
+00002da0: d309 0c67 f2c4 4100 0000 0300 6900 6d00  ...g..A.....i.m.
+00002db0: 6770 6831 5363 6f6d 7000 0000 0000 1130  gph1Scomp......0
+00002dc0: 0000 0000 0300 6900 6d00 6776 5372 6e6c  ......i.m.gvSrnl
+00002dd0: 6f6e 6700 0000 0100 0000 0700 6c00 6f00  ong.........l.o.
+00002de0: 6f00 6b00 7500 7000 7362 7773 7062 6c6f  o.k.u.p.sbwspblo
+00002df0: 6200 0000 c862 706c 6973 7430 30d7 0102  b....bplist00...
+00002e00: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
+00002e10: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
+00002e20: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
+00002e30: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
+00002e40: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
+00002e50: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
+00002e60: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
+00002e70: 0908 095f 1017 7b7b 302c 2031 3136 7d2c  ..._..{{0, 116},
+00002e80: 207b 3132 3530 2c20 3736 317d 7d09 0817   {1250, 761}}...
+00002e90: 2531 3d49 606d 797a 7b7c 7d7e 9800 0000  %1=I`myz{|}~....
+00002ea0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
+00002eb0: 0000 0000 0000 0000 0000 0000 9900 0000  ................
+00002ec0: 0700 6c00 6f00 6f00 6b00 7500 7000 736c  ..l.o.o.k.u.p.sl
+00002ed0: 6731 5363 6f6d 7000 0000 0000 04b1 fb00  g1Scomp.........
 00002ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -875,30 +875,30 @@
 000036a0: 01c5 1af0 c441 0000 0005 0069 0063 006f  .....A.....i.c.o
 000036b0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
 000036c0: da62 afb9 1af0 c441 0000 0005 0069 0063  .b.....A.....i.c
 000036d0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
 000036e0: 0000 0007 f000 0000 0005 0069 0063 006f  ...........i.c.o
 000036f0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00003700: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
-00003710: 6f62 0000 00c7 6270 6c69 7374 3030 d701  ob....bplist00..
+00003710: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
 00003720: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00003730: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00003740: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00003750: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00003760: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00003770: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00003780: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00003790: 0809 0809 5f10 167b 7b30 2c20 3230 307d  ...._..{{0, 200}
-000037a0: 2c20 7b37 3730 2c20 3433 367d 7d09 0817  , {770, 436}}...
-000037b0: 2531 3d49 606d 797a 7b7c 7d7e 9700 0000  %1=I`myz{|}~....
-000037c0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-000037d0: 0000 0000 0000 0000 0000 0000 9800 0000  ................
-000037e0: 0300 6900 6d00 676c 6731 5363 6f6d 7000  ..i.m.glg1Scomp.
-000037f0: 0000 0000 1424 d500 0000 0300 6900 6d00  .....$......i.m.
-00003800: 676c 7376 0000 0006 0000 0000 0000 380b  glsv..........8.
+00003790: 0809 0809 5f10 197b 7b33 3838 2c20 3231  ...._..{{388, 21
+000037a0: 367d 2c20 7b31 3039 322c 2034 3232 7d7d  6}, {1092, 422}}
+000037b0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
+000037c0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
+000037d0: 0000 0000 0000 0000 0000 0000 0000 009b  ................
+000037e0: 0000 0003 0069 006d 0067 6c67 3153 636f  .....i.m.glg1Sco
+000037f0: 6d70 0000 0000 0011 10bf 0000 0003 0069  mp.............i
+00003800: 006d 0067 0000 0006 0000 0000 0000 380b  .m.g..........8.
 00003810: 0000 0045 0000 100b 0000 300b 0000 200c  ...E......0... .
 00003820: 0000 180b 0000 0000 0000 0000 0000 0000  ................
 00003830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1003,23 +1003,23 @@
 00003ea0: 01c5 1af0 c441 0000 0005 0069 0063 006f  .....A.....i.c.o
 00003eb0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
 00003ec0: da62 afb9 1af0 c441 0000 0005 0069 0063  .b.....A.....i.c
 00003ed0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
 00003ee0: 0000 0007 f000 0000 0005 0069 0063 006f  ...........i.c.o
 00003ef0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00003f00: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
-00003f10: 6f62 0000 00c7 6270 6c69 7374 3030 d701  ob....bplist00..
+00003f10: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
 00003f20: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00003f30: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00003f40: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00003f50: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00003f60: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00003f70: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00003f80: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00003f90: 0809 0809 5f10 167b 7b30 2c20 3230 307d  ...._..{{0, 200}
-00003fa0: 2c20 7b37 3730 2c20 3433 367d 7d09 0817  , {770, 436}}...
-00003fb0: 2531 3d49 606d 797a 7b7c 7d7e 9700 0000  %1=I`myz{|}~....
-00003fc0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-00003fd0: 0000 0000 0000 0000 0000 0000 9800 0000  ................
-00003fe0: 0300 6900 6d00 676c 6731 5363 6f6d 7000  ..i.m.glg1Scomp.
-00003ff0: 0000 0000 1424 d500 0000 0300 6900 6d00  .....$......i.m.
-00004000: 676c 7376                                glsv
+00003f90: 0809 0809 5f10 197b 7b33 3838 2c20 3231  ...._..{{388, 21
+00003fa0: 367d 2c20 7b31 3039 322c 2034 3232 7d7d  6}, {1092, 422}}
+00003fb0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
+00003fc0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
+00003fd0: 0000 0000 0000 0000 0000 0000 0000 009b  ................
+00003fe0: 0000 0003 0069 006d 0067 6c67 3153 636f  .....i.m.glg1Sco
+00003ff0: 6d70 0000 0000 0011 10bf 0000 0003 0069  mp.............i
+00004000: 006d 0067                                .m.g
```

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.56.2/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.56.2/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.56.2/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.56.2/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.56.2/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.56.2/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.56.2/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.56.2/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.56.2/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.56.2/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.56.2/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.56.2/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.56.2/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/drop_bp_cords.py` & `Simba-UW-tf-dev-1.56.2/simba/drop_bp_cords.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/read_config_unit_tests.py` & `Simba-UW-tf-dev-1.56.2/simba/read_config_unit_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 __author__ = "Simon Nilsson", "JJ Choong"
 
 import configparser
 import trafaret as t
 import os
 import pandas as pd
 from simba.enums import ReadConfig, Dtypes, Formats
-from configparser import ConfigParser, MissingSectionHeaderError
+from configparser import ConfigParser
+from simba.utils.warnings import NoFileFoundWarning
 from simba.utils.errors import (NoFilesFoundError,
                                 IntegerError,
                                 InvalidInputError,
                                 StringError,
                                 FloatError,
                                 NotDirectoryError,
                                 MissingProjectConfigEntryError,
                                 CorruptedFileError,
-                                ColumnNotFoundError)
+                                ColumnNotFoundError,
+                                CountError)
 
 def check_int(name, value, max_value=None, min_value=None):
     try:
         t.Int().check(value)
     except t.DataError as e:
         print(e)
         raise IntegerError(msg=f'{name} should be an integer number in SimBA, but is set to {str(value)}')
@@ -106,16 +108,15 @@
     from simba.misc_tools import find_files_of_filetypes_in_directory
     file_paths = find_files_of_filetypes_in_directory(directory=folder_path, extensions=['.csv'])
     meta_file_lst = []
     for i in file_paths:
         if i.__contains__("meta"):
             meta_file_lst.append(os.path.join(folder_path, i))
     if len(meta_file_lst) == 0:
-        print(
-            'SIMBA WARNING: The training meta-files folder (project_folder/configs) does not have any meta files inside it (no files in this folder has the "meta" substring in the filename')
+        NoFileFoundWarning(msg=f'The training meta-files folder in your project ({folder_path}) does not have any meta files inside it (no files in this folder has the "meta" substring in the filename)')
     return meta_file_lst
 
 
 def read_meta_file(meta_file_path):
     return pd.read_csv(meta_file_path, index_col=False).to_dict(orient='records')[0]
 
 
@@ -125,32 +126,31 @@
     elif not os.access(file_path, os.R_OK):
         raise CorruptedFileError(f'{file_path} is not readable')
 
 def read_config_file(ini_path: str):
     config = ConfigParser()
     try:
         config.read(str(ini_path))
-    except MissingSectionHeaderError:
-        print('ERROR: Not a valid project_config file. Please check the project_config.ini path.')
-        raise MissingSectionHeaderError
+    except Exception as e:
+        print(e.args)
+        raise MissingProjectConfigEntryError(msg=f'{ini_path} is not a valid project_config file. Please check the project_config.ini path.')
     return config
 
 def check_if_dir_exists(in_dir: str):
     if not os.path.isdir(in_dir):
         raise NotDirectoryError(msg=f'{in_dir} is not a valid directory')
 
 def insert_default_headers_for_feature_extraction(df: pd.DataFrame,
                                                   headers: list,
                                                   pose_config: str,
                                                   filename: str):
     if len(headers) != len(df.columns):
-        raise ValueError('SIMBA ERROR: Your SimBA project is set to using the default {} pose-configuration. '
-                         'SimBA therefore expects {} columns of data inside the files within the project_folder. However, '
-                         'within file {} file, SimBA found {} columns.'.format(pose_config, str(len(headers)), filename,
-                                                                               str(len(df.columns))))
+        raise CountError(f'Your SimBA project is set to using the default {pose_config} pose-configuration. '
+                         f'SimBA therefore expects {str(len(headers))} columns of data inside the files within the project_folder. However, '
+                         f'within file {filename} file, SimBA found {str(len(df.columns))} columns.')
     else:
         df.columns = headers
         return df
 
 
 def check_that_column_exist(df: pd.DataFrame,
                             column_name: str,
@@ -173,11 +173,8 @@
                                      data_type=ReadConfig.FOLDER_PATH.value)
     file_type = read_config_entry(config=config,
                                   section=ReadConfig.GENERAL_SETTINGS.value,
                                   option=ReadConfig.FILE_TYPE.value,
                                   data_type=Dtypes.STR.value,
                                   default_value=Formats.CSV.value)
 
-    return project_path, file_type
-
-
-
+    return project_path, file_type
```

### Comparing `Simba-UW-tf-dev-1.56.1/simba/project_config_creator.py` & `Simba-UW-tf-dev-1.56.2/simba/project_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/set_hyperparameters.py` & `Simba-UW-tf-dev-1.56.2/simba/set_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/train_single_model.py` & `Simba-UW-tf-dev-1.56.2/simba/train_single_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/create_clf_log.py` & `Simba-UW-tf-dev-1.56.2/simba/create_clf_log.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/batch_process_videos/.DS_Store` & `Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/batch_process_videos/batch_process_menus.py` & `Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.56.2/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/Kleinberg_calculator.py` & `Simba-UW-tf-dev-1.56.2/simba/Kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/reorganize_keypoint_in_pose.py` & `Simba-UW-tf-dev-1.56.2/simba/reorganize_keypoint_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/simba/play_annotation_video.py` & `Simba-UW-tf-dev-1.56.2/simba/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.56.1
+Version: 1.56.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.56.1/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,14 @@
 simba/assets/icons/concat_icons/vertical.png
 simba/assets/img/.DS_Store
 simba/assets/img/about_me.png
 simba/assets/img/bg.png
 simba/assets/img/bg_2.png
 simba/assets/img/splash.mp4
 simba/assets/img/splash.pptx
-simba/assets/img/splash_old.mp4
 simba/assets/lookups/.DS_Store
 simba/assets/lookups/feature_extraction_headers.csv
 simba/assets/lookups/features.csv
 simba/assets/lookups/model_names.parquet
 simba/assets/lookups/unsupervised_example_x.csv
 simba/assets/shap/.DS_Store
 simba/assets/shap/UbuntuMono-Regular.ttf
@@ -207,17 +206,18 @@
 simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
 simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
 simba/feature_extractors/misc/.DS_Store
 simba/feature_extractors/misc/add_probability_cnt_features.py
 simba/feature_extractors/misc/convex_hull_3_scratch_3.py
 simba/feature_extractors/misc/convex_hull_scratch_1.py
 simba/feature_extractors/misc/convex_hull_scratch_2.py
+simba/feature_extractors/misc/count_values_in_range.py
 simba/feature_extractors/misc/egocentrical_aligner.py
 simba/feature_extractors/misc/fish_feature_extractor_2022.py
-simba/feature_extractors/misc/fish_feature_extractor_2023.py
+simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
 simba/feature_extractors/misc/graph_3d_plotter.py
 simba/feature_extractors/misc/graph_creator.py
 simba/feature_extractors/misc/make_splash.py
 simba/feature_extractors/misc/mutual_exclusive.py
 simba/feature_extractors/misc/read_in_mp.py
 simba/feature_extractors/misc/termite_rois.csv
 simba/mixins/.DS_Store
```

### Comparing `Simba-UW-tf-dev-1.56.1/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.56.2/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 graphviz==0.11
 imblearn==0.0
 imgaug==0.4.0
 imutils==0.5.2
 matplotlib==3.0.3
 numpy==1.18.1
 opencv-python==3.4.5.20
-pandas==0.25.3
+pandas==1.4.0
 scikit-image==0.14.2
 scipy==1.1.0
 seaborn==0.9.0
 scikit-learn==0.22.2
 tabulate==0.8.3
 tqdm==4.30.0
 xgboost==0.90
@@ -27,13 +27,13 @@
 dash_html_components==1.0.3
 h5py==2.9.0
 numba==0.52.0
 numexpr==2.6.9
 plotly==4.9.0
 statsmodels==0.9.0
 cefpython3==66.0
-pyarrow==0.17.1
+pyarrow==6.0.1
 shap==0.35.0
 h5py==2.9.0
 tables==3.6.1
 xlrd==1.2.0
 trafaret==2.1.1
```

### Comparing `Simba-UW-tf-dev-1.56.1/LICENSE.md` & `Simba-UW-tf-dev-1.56.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/README.md` & `Simba-UW-tf-dev-1.56.2/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.1/setup.py` & `Simba-UW-tf-dev-1.56.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.56.1",
+    version="1.56.2",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
-              'opencv-python == 3.4.5.20','pandas == 0.25.3','scikit-image == 0.14.2', 'scipy == 1.1.0','seaborn == 0.9.0',
+              'opencv-python == 3.4.5.20','pandas == 1.4.0','scikit-image == 0.14.2', 'scipy == 1.1.0','seaborn == 0.9.0',
               'scikit-learn == 0.22.2','tabulate == 0.8.3','tqdm == 4.30.0','xgboost == 0.90',
               'yellowbrick == 0.9.1', 'dash == 1.14.0', 'dash_color_picker == 0.0.1', 'dash_core_components == 1.10.2',
 			  'dash_colorscales == 0.0.4', 'dash_html_components == 1.0.3', 'h5py == 2.9.0', 'numba == 0.52.0', 'numexpr == 2.6.9',
-			  'plotly == 4.9.0', 'statsmodels == 0.9.0', 'cefpython3 == 66.0', "pyarrow == 0.17.1", "shap == 0.35.0","h5py==2.9.0",
+			  'plotly == 4.9.0', 'statsmodels == 0.9.0', 'cefpython3 == 66.0', "pyarrow == 6.0.1", "shap == 0.35.0","h5py==2.9.0",
 			  "tables==3.6.1", "xlrd==1.2.0", "trafaret==2.1.1"],
     license='GNU Lesser General Public License v3 (LGPLv3)',
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=(
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
```

