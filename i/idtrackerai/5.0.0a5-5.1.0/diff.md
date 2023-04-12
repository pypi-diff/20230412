# Comparing `tmp/idtrackerai-5.0.0a5.tar.gz` & `tmp/idtrackerai-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idtrackerai-5.0.0a5.tar", last modified: Fri Mar 17 13:07:24 2023, max compression
+gzip compressed data, was "idtrackerai-5.1.0.tar", last modified: Wed Apr 12 10:06:47 2023, max compression
```

## Comparing `idtrackerai-5.0.0a5.tar` & `idtrackerai-5.1.0.tar`

### file list

```diff
@@ -1,159 +1,149 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.145169 idtrackerai-5.0.0a5/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    35987 2023-02-10 16:03:19.000000 idtrackerai-5.0.0a5/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2573 2023-03-17 13:07:24.145169 idtrackerai-5.0.0a5/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1495 2023-03-09 12:20:58.000000 idtrackerai-5.0.0a5/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2825 2023-03-17 13:04:34.000000 idtrackerai-5.0.0a5/pyproject.toml
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-03-17 13:07:24.145169 idtrackerai-5.0.0a5/setup.cfg
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.129168 idtrackerai-5.0.0a5/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.129168 idtrackerai-5.0.0a5/src/idtrackerai/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      587 2023-03-05 17:48:26.000000 idtrackerai-5.0.0a5/src/idtrackerai/__init__.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.129168 idtrackerai-5.0.0a5/src/idtrackerai/animals_detection/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/animals_detection/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5785 2023-03-13 19:41:53.000000 idtrackerai-5.0.0a5/src/idtrackerai/animals_detection/animals_detection.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    19882 2023-03-15 10:17:44.000000 idtrackerai-5.0.0a5/src/idtrackerai/animals_detection/segmentation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    33133 2023-03-17 12:29:39.000000 idtrackerai-5.0.0a5/src/idtrackerai/blob.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3330 2023-03-10 09:57:51.000000 idtrackerai-5.0.0a5/src/idtrackerai/constants.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.129168 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       96 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7712 2023-03-15 12:57:17.000000 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/crossing_detector.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3305 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/crossings_detection.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.129168 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/dataset/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/dataset/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3866 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7282 2023-03-15 10:07:04.000000 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4633 2023-03-10 14:30:44.000000 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/model_area.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.129168 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4011 2023-03-15 10:46:36.000000 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/network/network_params_crossings.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2727 2023-03-15 10:46:36.000000 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5442 2023-03-15 11:52:37.000000 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4364 2023-03-15 11:50:22.000000 idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.137169 idtrackerai-5.0.0a5/src/idtrackerai/data/
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5933626 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/data/test_A.avi
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5976882 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/data/test_B.avi
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    26622 2023-03-16 10:10:11.000000 idtrackerai-5.0.0a5/src/idtrackerai/fragment.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.141168 idtrackerai-5.0.0a5/src/idtrackerai/fragmentation/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       78 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/fragmentation/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5058 2023-03-15 10:04:17.000000 idtrackerai-5.0.0a5/src/idtrackerai/fragmentation/fragmentation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8921 2023-03-16 11:16:40.000000 idtrackerai-5.0.0a5/src/idtrackerai/globalfragment.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.141168 idtrackerai-5.0.0a5/src/idtrackerai/groundtruth_utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/groundtruth_utils/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    23440 2023-03-10 14:35:44.000000 idtrackerai-5.0.0a5/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    21976 2023-03-10 14:35:44.000000 idtrackerai-5.0.0a5/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3924 2023-02-28 10:28:32.000000 idtrackerai-5.0.0a5/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5613 2023-02-28 09:51:15.000000 idtrackerai-5.0.0a5/src/idtrackerai/groundtruth_utils/generate_groundtruth.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4232 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    15970 2023-03-16 09:50:24.000000 idtrackerai-5.0.0a5/src/idtrackerai/list_of_blobs.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    24047 2023-03-16 11:00:10.000000 idtrackerai-5.0.0a5/src/idtrackerai/list_of_fragments.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    13051 2023-03-16 09:58:53.000000 idtrackerai-5.0.0a5/src/idtrackerai/list_of_global_fragments.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.141168 idtrackerai-5.0.0a5/src/idtrackerai/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4319 2023-03-16 10:51:07.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/evaluate.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.141168 idtrackerai-5.0.0a5/src/idtrackerai/network/learners/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       81 2023-03-15 10:47:16.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/learners/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5278 2023-03-16 15:36:19.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/learners/learners.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.141168 idtrackerai-5.0.0a5/src/idtrackerai/network/models/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/models/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1651 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/models/models_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8236 2023-03-02 09:13:03.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/models/pytorch_architectures.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.141168 idtrackerai-5.0.0a5/src/idtrackerai/network/modules/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/modules/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3465 2023-03-02 09:13:03.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/modules/criterion.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2666 2023-03-16 10:06:47.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/modules/pairwise.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6026 2023-03-15 10:36:24.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/train.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.141168 idtrackerai-5.0.0a5/src/idtrackerai/network/utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/utils/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4828 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/utils/metric.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1409 2023-03-15 10:36:33.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/utils/task.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1553 2023-03-02 09:13:03.000000 idtrackerai-5.0.0a5/src/idtrackerai/network/utils/utils.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.141168 idtrackerai-5.0.0a5/src/idtrackerai/postprocess/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      292 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/postprocess/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    27574 2023-03-15 10:04:17.000000 idtrackerai-5.0.0a5/src/idtrackerai/postprocess/assign_them_all.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2715 2023-03-15 10:02:35.000000 idtrackerai-5.0.0a5/src/idtrackerai/postprocess/compute_velocity_model.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    21549 2023-03-15 10:04:17.000000 idtrackerai-5.0.0a5/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3598 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/postprocess/erosion.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8551 2023-03-15 10:13:06.000000 idtrackerai-5.0.0a5/src/idtrackerai/postprocess/get_trajectories.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2592 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5113 2023-03-02 09:13:03.000000 idtrackerai-5.0.0a5/src/idtrackerai/postprocess/trajectories_creation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4129 2023-03-15 10:36:42.000000 idtrackerai-5.0.0a5/src/idtrackerai/postprocess/trajectories_to_csv.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.141168 idtrackerai-5.0.0a5/src/idtrackerai/tracker/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    36646 2023-03-16 10:35:46.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/accumulation_manager.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3151 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/accumulation_manager_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8743 2023-03-16 10:54:00.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/accumulator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6597 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/assigner.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.141168 idtrackerai-5.0.0a5/src/idtrackerai/tracker/dataset/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/dataset/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3711 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/dataset/identification_dataloader.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6666 2023-03-15 10:36:56.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/dataset/identification_dataset.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5414 2023-03-13 12:06:52.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/identity_transfer.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.141168 idtrackerai-5.0.0a5/src/idtrackerai/tracker/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3277 2023-03-16 14:41:32.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/network/get_predictions.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5119 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/network/network_params.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8824 2023-03-15 11:57:03.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/network/stop_training_criteria.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5129 2023-03-15 11:50:31.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/network/trainer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7561 2023-03-15 13:13:54.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/pre_trainer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    34926 2023-03-16 11:52:46.000000 idtrackerai-5.0.0a5/src/idtrackerai/tracker/tracker.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.141168 idtrackerai-5.0.0a5/src/idtrackerai/utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1108 2023-03-14 17:29:09.000000 idtrackerai-5.0.0a5/src/idtrackerai/utils/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2151 2023-03-14 17:14:44.000000 idtrackerai-5.0.0a5/src/idtrackerai/utils/check_PyPI_version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1143 2023-02-28 09:52:48.000000 idtrackerai-5.0.0a5/src/idtrackerai/utils/confparams.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1551 2023-03-14 14:56:38.000000 idtrackerai-5.0.0a5/src/idtrackerai/utils/init_logger.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    12027 2023-03-16 11:36:29.000000 idtrackerai-5.0.0a5/src/idtrackerai/utils/py_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    31754 2023-03-16 10:47:12.000000 idtrackerai-5.0.0a5/src/idtrackerai/video.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.129168 idtrackerai-5.0.0a5/src/idtrackerai.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2573 2023-03-17 13:07:24.000000 idtrackerai-5.0.0a5/src/idtrackerai.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6095 2023-03-17 13:07:24.000000 idtrackerai-5.0.0a5/src/idtrackerai.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-03-17 13:07:24.000000 idtrackerai-5.0.0a5/src/idtrackerai.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      305 2023-03-17 13:07:24.000000 idtrackerai-5.0.0a5/src/idtrackerai.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      316 2023-03-17 13:07:24.000000 idtrackerai-5.0.0a5/src/idtrackerai.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       96 2023-03-17 13:07:24.000000 idtrackerai-5.0.0a5/src/idtrackerai.egg-info/top_level.txt
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.141168 idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5807 2023-03-15 20:52:36.000000 idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/GUI_main_base.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      794 2023-03-14 12:16:35.000000 idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2448 2023-03-02 09:13:03.000000 idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    66516 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/logo_256.png
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    10027 2023-03-09 15:26:00.000000 idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/themes.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      619 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/tooltips.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.145169 idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/widgets_utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5429 2023-03-14 17:20:04.000000 idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/widgets_utils/canvas.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5834 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5938 2023-03-15 19:54:56.000000 idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2780 2023-02-27 17:58:52.000000 idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    12594 2023-03-15 20:19:53.000000 idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/widgets_utils/video_player.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.145169 idtrackerai-5.0.0a5/src/idtrackerai_start_app/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4944 2023-03-14 14:57:48.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/__main__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1546 2023-03-09 12:20:58.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/all_valid_parameters.dat
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6730 2023-03-10 15:28:48.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/arg_parser.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6079 2023-03-14 16:06:16.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/run_idtrackerai.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    15075 2023-03-15 20:51:47.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_GUI.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.145169 idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7733 2023-03-14 12:45:24.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      482 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6621 2023-03-14 09:09:17.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5769 2023-03-15 10:37:27.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2579 2023-03-14 12:34:55.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2370 2023-02-28 09:42:23.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6618 2023-03-15 13:34:33.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5007 2023-02-28 09:43:15.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2586 2023-03-15 19:05:00.000000 idtrackerai-5.0.0a5/src/idtrackerai_start_app/tooltips.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.145169 idtrackerai-5.0.0a5/src/idtrackerai_validator/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-03-02 09:13:04.000000 idtrackerai-5.0.0a5/src/idtrackerai_validator/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      638 2023-03-04 12:27:37.000000 idtrackerai-5.0.0a5/src/idtrackerai_validator/__main__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      715 2023-03-09 12:20:58.000000 idtrackerai-5.0.0a5/src/idtrackerai_validator/tooltips.toml
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    31383 2023-03-17 12:58:50.000000 idtrackerai-5.0.0a5/src/idtrackerai_validator/validation_GUI.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.145169 idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      425 2023-02-21 09:02:12.000000 idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8102 2023-03-15 20:24:06.000000 idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/errors_explorer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6176 2023-03-15 20:37:31.000000 idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/id_groups.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1654 2023-03-15 13:35:59.000000 idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/id_labels.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    12948 2023-03-15 20:35:07.000000 idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/interpolator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6243 2023-03-14 12:09:06.000000 idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/paint_blobs.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4940 2023-03-15 20:39:10.000000 idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/setup_points.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-03-17 13:07:24.145169 idtrackerai-5.0.0a5/src/idtrackerai_video/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-03-02 09:13:04.000000 idtrackerai-5.0.0a5/src/idtrackerai_video/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5300 2023-03-15 10:04:04.000000 idtrackerai-5.0.0a5/src/idtrackerai_video/general_video.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4014 2023-03-16 10:15:49.000000 idtrackerai-5.0.0a5/src/idtrackerai_video/individual_videos.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2840 2023-03-10 14:30:44.000000 idtrackerai-5.0.0a5/src/idtrackerai_video/main.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    35987 2023-02-10 16:03:19.000000 idtrackerai-5.1.0/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2741 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1587 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2994 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/pyproject.toml
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/setup.cfg
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.575685 idtrackerai-5.1.0/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.575685 idtrackerai-5.1.0/src/idmatcherai/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idmatcherai/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     9058 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idmatcherai/main.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3678 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idmatcherai/matcher.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.575685 idtrackerai-5.1.0/src/idtrackerai/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      587 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/__init__.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.575685 idtrackerai-5.1.0/src/idtrackerai/animals_detection/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/animals_detection/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5785 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/animals_detection/animals_detection.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    20011 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/animals_detection/segmentation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    33131 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/blob.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3215 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/constants.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.575685 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       96 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7404 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/crossing_detector.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3305 2023-03-21 11:15:37.000000 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/crossings_detection.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.575685 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/dataset/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:28.000000 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/dataset/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3854 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7286 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4648 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/model_area.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.575685 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:28.000000 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      761 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5415 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4174 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.579685 idtrackerai-5.1.0/src/idtrackerai/data/
+-rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5933626 2023-03-20 08:48:28.000000 idtrackerai-5.1.0/src/idtrackerai/data/test_A.avi
+-rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5976882 2023-03-20 08:48:29.000000 idtrackerai-5.1.0/src/idtrackerai/data/test_B.avi
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    25588 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/fragment.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.583685 idtrackerai-5.1.0/src/idtrackerai/fragmentation/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       78 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/fragmentation/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5058 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/fragmentation/fragmentation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8915 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/globalfragment.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.583685 idtrackerai-5.1.0/src/idtrackerai/groundtruth_utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.0/src/idtrackerai/groundtruth_utils/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    22092 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    20302 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3924 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5589 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/groundtruth_utils/generate_groundtruth.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3989 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    15846 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/list_of_blobs.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    23986 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/list_of_fragments.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    13045 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/list_of_global_fragments.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.583685 idtrackerai-5.1.0/src/idtrackerai/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      456 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4273 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/network/evaluate.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3854 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/network/learners.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6563 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/network/models.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1878 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/network/network_params.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4509 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/network/train.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8886 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/network/utils.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/src/idtrackerai/postprocess/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      292 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/postprocess/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    27574 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/postprocess/assign_them_all.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2715 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/postprocess/compute_velocity_model.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    21435 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3598 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/postprocess/erosion.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8545 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/postprocess/get_trajectories.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2592 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5113 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/postprocess/trajectories_creation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4129 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/postprocess/trajectories_to_csv.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/src/idtrackerai/tracker/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    36593 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/accumulation_manager.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3151 2023-03-21 11:15:37.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/accumulation_manager_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8680 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/accumulator.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4270 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/assigner.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/src/idtrackerai/tracker/dataset/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/dataset/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3700 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/dataset/identification_dataloader.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6666 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/dataset/identification_dataset.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5432 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/identity_transfer.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/src/idtrackerai/tracker/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1452 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/network/get_predictions.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8824 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/network/stop_training_criteria.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5035 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/network/trainer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7147 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/pre_trainer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    34367 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/tracker/tracker.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/src/idtrackerai/utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1108 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/utils/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2151 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/utils/check_PyPI_version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1143 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai/utils/confparams.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1622 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/utils/init_logger.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    11984 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/utils/py_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    32391 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai/video.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.575685 idtrackerai-5.1.0/src/idtrackerai.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2741 2023-04-12 10:06:47.000000 idtrackerai-5.1.0/src/idtrackerai.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5669 2023-04-12 10:06:47.000000 idtrackerai-5.1.0/src/idtrackerai.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-12 10:06:47.000000 idtrackerai-5.1.0/src/idtrackerai.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      341 2023-04-12 10:06:47.000000 idtrackerai-5.1.0/src/idtrackerai.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      362 2023-04-12 10:06:47.000000 idtrackerai-5.1.0/src/idtrackerai.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      108 2023-04-12 10:06:47.000000 idtrackerai-5.1.0/src/idtrackerai.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/src/idtrackerai_GUI_tools/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5955 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_GUI_tools/GUI_main_base.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      794 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai_GUI_tools/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2448 2023-03-20 08:48:29.000000 idtrackerai-5.1.0/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    66516 2023-03-20 08:48:29.000000 idtrackerai-5.1.0/src/idtrackerai_GUI_tools/logo_256.png
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10027 2023-04-12 07:40:32.000000 idtrackerai-5.1.0/src/idtrackerai_GUI_tools/themes.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      619 2023-03-20 08:48:29.000000 idtrackerai-5.1.0/src/idtrackerai_GUI_tools/tooltips.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/src/idtrackerai_GUI_tools/widgets_utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5429 2023-03-21 11:15:37.000000 idtrackerai-5.1.0/src/idtrackerai_GUI_tools/widgets_utils/canvas.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5909 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5939 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2863 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    12598 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_GUI_tools/widgets_utils/video_player.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/src/idtrackerai_start_app/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4937 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/__main__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1515 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/all_valid_parameters.dat
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6826 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/arg_parser.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6110 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/run_idtrackerai.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    15533 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_GUI.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8021 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      482 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6621 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5715 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2617 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2370 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6625 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5007 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2713 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_start_app/tooltips.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/src/idtrackerai_validator/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_validator/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      638 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai_validator/__main__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      715 2023-03-20 08:48:29.000000 idtrackerai-5.1.0/src/idtrackerai_validator/tooltips.toml
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    31409 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_validator/validation_GUI.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      425 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8104 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/errors_explorer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6146 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/id_groups.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1654 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/id_labels.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    12948 2023-03-21 11:17:49.000000 idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/interpolator.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6246 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/paint_blobs.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4918 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/setup_points.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:47.587685 idtrackerai-5.1.0/src/idtrackerai_video/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_video/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6020 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_video/general_video.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4866 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_video/individual_videos.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2058 2023-04-12 10:06:11.000000 idtrackerai-5.1.0/src/idtrackerai_video/main.py
```

### Comparing `idtrackerai-5.0.0a5/LICENSE` & `idtrackerai-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/PKG-INFO` & `idtrackerai-5.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 Metadata-Version: 2.1
 Name: idtrackerai
-Version: 5.0.0a5
+Version: 5.1.0
 Summary: A multi-animal tracking algorithm based on convolutional neural networks
-Author: Jordi Torrents, Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
-Project-URL: Homepage, https://idtrackerai.readthedocs.io/en/latest/
+Author: Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
+Author-email: Jordi Torrents <jordi.torrentsm@gmail.com>
+Project-URL: Homepage, https://idtracker.ai/
 Project-URL: Repository, https://gitlab.com/polavieja_lab/idtrackerai
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
+Classifier: Environment :: X11 Applications :: Qt
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
-[![image](http://img.shields.io/pypi/v/idtrackerai.svg)](https://pypi.python.org/pypi/idtrackerai/)
-![pipeline](https://gitlab.com/polavieja_lab/idtrackerai/badges/v5-dev/pipeline.svg)
-[![Supported Python versions](https://img.shields.io/pypi/pyversions/idtrackerai.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/idtrackerai/)
-![pylint](https://gitlab.com/polavieja_lab/idtrackerai/-/jobs/artifacts/v5-dev/raw/pylint/pylint.svg?job=test)
-[![PyPI downloads](https://img.shields.io/pypi/dm/idtrackerai.svg)](https://pypistats.org/packages/idtrackerai)
-![Licence](https://img.shields.io/gitlab/license/polavieja_lab/idtrackerai.svg)
+[![image](http://img.shields.io/pypi/v/idtrackerai.svg)](https://pypi.python.org/pypi/idtrackerai/) ![pipeline](https://gitlab.com/polavieja_lab/idtrackerai/badges/master/pipeline.svg) [![Documentation Status](https://readthedocs.org/projects/idtrackerai/badge/?version=latest)](https://idtracker.ai/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/idtrackerai.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/idtrackerai/) ![pylint](https://gitlab.com/polavieja_lab/idtrackerai/-/jobs/artifacts/master/raw/pylint/pylint.svg?job=test) [![PyPI downloads](https://img.shields.io/pypi/dm/idtrackerai.svg)](https://pypistats.org/packages/idtrackerai) ![Licence](https://img.shields.io/gitlab/license/polavieja_lab/idtrackerai.svg)
 
-Idtracker.ai is a multi-animal tracking software for laboratory conditions. This work has been published in [Nature Methods](https://doi.org/10.1038/s41592-018-0295-5) ([pdf here](https://drive.google.com/file/d/1fYBcmH6PPlwy0AQcr4D0iS2Qd-r7xU9n/view?usp=sharing))
+# Find everything you are looking for in [our website](https://idtracker.ai)
 
-Find everything you are looking for in [our website](https://idtracker.ai)
+Idtracker.ai is a multi-animal tracking software for laboratory conditions. This work has been published in [Nature Methods](https://doi.org/10.1038/s41592-018-0295-5) ([pdf here](https://drive.google.com/file/d/1fYBcmH6PPlwy0AQcr4D0iS2Qd-r7xU9n/view?usp=sharing))
 
 ## Installation for developers.
 
 On an environment with Python 3.10 and a working installation of Pytorch (Torch and Torchvision) you can install idtracker.ai for devs by cloning the repo and installing:
 
 ``` bash
-git clone https://gitlab.com/polavieja_lab/idtrackerai
-pip install -e ./idtrackerai[dev]
+pip install git+https://gitlab.com/polavieja_lab/idtrackerai
 ```
 
 ## Contributors
 * Jordi Torrents (2022-)
 * Antonio Ortega (2021-)
 * Francisco Romero-Ferrero (2015-2022)
 * Mattia G. Bergomi (2015-2018)
```

### Comparing `idtrackerai-5.0.0a5/README.md` & `idtrackerai-5.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-[![image](http://img.shields.io/pypi/v/idtrackerai.svg)](https://pypi.python.org/pypi/idtrackerai/)
-![pipeline](https://gitlab.com/polavieja_lab/idtrackerai/badges/v5-dev/pipeline.svg)
-[![Supported Python versions](https://img.shields.io/pypi/pyversions/idtrackerai.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/idtrackerai/)
-![pylint](https://gitlab.com/polavieja_lab/idtrackerai/-/jobs/artifacts/v5-dev/raw/pylint/pylint.svg?job=test)
-[![PyPI downloads](https://img.shields.io/pypi/dm/idtrackerai.svg)](https://pypistats.org/packages/idtrackerai)
-![Licence](https://img.shields.io/gitlab/license/polavieja_lab/idtrackerai.svg)
+[![image](http://img.shields.io/pypi/v/idtrackerai.svg)](https://pypi.python.org/pypi/idtrackerai/) ![pipeline](https://gitlab.com/polavieja_lab/idtrackerai/badges/master/pipeline.svg) [![Documentation Status](https://readthedocs.org/projects/idtrackerai/badge/?version=latest)](https://idtracker.ai/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/idtrackerai.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/idtrackerai/) ![pylint](https://gitlab.com/polavieja_lab/idtrackerai/-/jobs/artifacts/master/raw/pylint/pylint.svg?job=test) [![PyPI downloads](https://img.shields.io/pypi/dm/idtrackerai.svg)](https://pypistats.org/packages/idtrackerai) ![Licence](https://img.shields.io/gitlab/license/polavieja_lab/idtrackerai.svg)
 
-Idtracker.ai is a multi-animal tracking software for laboratory conditions. This work has been published in [Nature Methods](https://doi.org/10.1038/s41592-018-0295-5) ([pdf here](https://drive.google.com/file/d/1fYBcmH6PPlwy0AQcr4D0iS2Qd-r7xU9n/view?usp=sharing))
+# Find everything you are looking for in [our website](https://idtracker.ai)
 
-Find everything you are looking for in [our website](https://idtracker.ai)
+Idtracker.ai is a multi-animal tracking software for laboratory conditions. This work has been published in [Nature Methods](https://doi.org/10.1038/s41592-018-0295-5) ([pdf here](https://drive.google.com/file/d/1fYBcmH6PPlwy0AQcr4D0iS2Qd-r7xU9n/view?usp=sharing))
 
 ## Installation for developers.
 
 On an environment with Python 3.10 and a working installation of Pytorch (Torch and Torchvision) you can install idtracker.ai for devs by cloning the repo and installing:
 
 ``` bash
-git clone https://gitlab.com/polavieja_lab/idtrackerai
-pip install -e ./idtrackerai[dev]
+pip install git+https://gitlab.com/polavieja_lab/idtrackerai
 ```
 
 ## Contributors
 * Jordi Torrents (2022-)
 * Antonio Ortega (2021-)
 * Francisco Romero-Ferrero (2015-2022)
 * Mattia G. Bergomi (2015-2018)
 * Ricardo Ribeiro (2018-2020)
-* Francisco J.H. Heras (2015-2022)
+* Francisco J.H. Heras (2015-2022)
```

### Comparing `idtrackerai-5.0.0a5/pyproject.toml` & `idtrackerai-5.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,71 +1,79 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "idtrackerai"
-version = "5.0.0a5"
+version = "5.1.0"
 authors = [
-    { name = "Jordi Torrents" },
+    { name = "Jordi Torrents", email = "jordi.torrentsm@gmail.com" },
     { name = "Francisco Romero Ferrero" },
     { name = "Mattia G. Bergomi" },
     { name = "Francisco J.H. Heras" },
     { name = "Ricardo Ribeiro" },
 ]
 description = "A multi-animal tracking algorithm based on convolutional neural networks"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
+    "Environment :: X11 Applications :: Qt",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "numpy >= 1.24.2",
     "rich >= 13.3.1",
     "scikit-learn >= 1.2.1",
     "h5py >= 3.8.0",
     "scipy >= 1.10.0",
-    "opencv-python >= 4.7.0",
+    "opencv-python-headless >= 4.7.0",
     "pyqt6 >= 6.4.2",
     'superqt >= 0.4.1',
     'toml >= 0.10.2',
+    "matplotlib >= 3.7.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     'pytest',
     "black",
     'pylint',
     'vulture',
     'isort',
-    "pydata_sphinx_theme",
-    "sphinx-copybutton",
-    "sphinx_design",
-    "sphinx==5.3.0",
+
+
+    "twine",
+    "build",
+    'pre-commit',
 ]
 docs = [
     "pydata_sphinx_theme",
     "sphinx-copybutton",
     "sphinx_design",
     "sphinx==5.3.0",
+    "nbsphinx",
+    "ipykernel",
+    'sphinx-toolbox',
+    'sphinx-togglebutton',
+    'esbonio',
 ]
 
 [project.urls]
-"Homepage" = "https://idtrackerai.readthedocs.io/en/latest/"
+"Homepage" = "https://idtracker.ai/"
 "Repository" = "https://gitlab.com/polavieja_lab/idtrackerai"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 [tool.setuptools.package-data]
 "idtrackerai.data" = ["**"]                          # for Gitlab CICD
 idtrackerai = ["*.avi", "*.toml"]
@@ -75,19 +83,19 @@
 
 [project.scripts]
 idtrackerai_test = "idtrackerai_start_app.__main__:general_test"
 idtrackerai = "idtrackerai_start_app.__main__:main"
 idtrackerai_validate = "idtrackerai_validator.__main__:main"
 idtrackerai_video = "idtrackerai_video.main:main"
 idtrackerai_csv = "idtrackerai.postprocess.trajectories_to_csv:main"
+idmatcherai = "idmatcherai.main:main"
 
 [tool.pytest.ini_options]
 log_file_format = "[%(asctime)s %(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_file = 'pytest.log'
-testpaths = ["tests"]
 log_file_level = 0
 addopts = '-v'
 
 
 [tool.black]
 skip-magic-trailing-comma = true
 preview = true
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/__init__.py` & `idtrackerai-5.1.0/src/idtrackerai/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/animals_detection/animals_detection.py` & `idtrackerai-5.1.0/src/idtrackerai/animals_detection/animals_detection.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     n_frames_with_all_visible = sum(
         len(blobs) == video.number_of_animals for blobs in list_of_blobs.blobs_in_video
     )
 
     if n_frames_with_all_visible == 0:
         raise CustomError(
             "There is not any frames where the number of blobs is equal "
-            "to the number of animals stated by the user. idTracker.ai "
+            "to the number of animals stated by the user. Idtracker.ai "
             "needs those frame to work"
         )
 
     error_frames = [
         frame
         for frame, blobs in enumerate(list_of_blobs.blobs_in_video)
         if len(blobs) > video.number_of_animals
@@ -136,21 +136,21 @@
         logging.warning(
             "This can be detrimental for the proper functioning of the system"
         )
         if n_error_frames < 25:
             logging.warning(f"Frames with more blobs than animals: {error_frames}")
         else:
             logging.warning(
-                "Too much frames with more blobs than animals "
-                "for printing their indexes in log"
+                "Too many frames with more blobs than animals "
+                "for printing their indices in log"
             )
 
         output_path = video.session_folder / "inconsistent_frames.csv"
         logging.info(
-            f"Saving indexes of frames with more blobs than animals in {output_path}"
+            f"Saving indices of frames with more blobs than animals in {output_path}"
         )
         output_path.write_text("\n".join(map(str, error_frames)))
 
         if video.check_segmentation:
             list_of_blobs.save(video.blobs_path)
             raise CustomError(
                 f"Check_segmentation is {True}, exiting...\n"
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/animals_detection/segmentation.py` & `idtrackerai-5.1.0/src/idtrackerai/animals_detection/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     return blobs_in_frame
 
 
 def process_frame(
     frame,
     intensity_ths,
     area_ths,
-    ROI_mask,
+    ROI_mask: np.ndarray | None,
     bkg_model,
     resolution_reduction,
     sigma_blurring=None,
 ) -> tuple[list[int], list[np.ndarray], np.ndarray]:
     frame = gaussian_blur(frame, sigma=sigma_blurring)
     # avg_brightness = segmentation_parameters["avg_brightness"]
 
@@ -361,15 +361,19 @@
             return None
         if progress_bar:
             progress_bar.emit(i)
     return frame_stack
 
 
 def generate_background_from_frame_stack(
-    frame_stack, ROI_mask, stat=None, progress_bar=None, abort: Callable = lambda: False
+    frame_stack: np.ndarray,
+    ROI_mask: np.ndarray | None,
+    stat=None,
+    progress_bar=None,
+    abort: Callable = lambda: False,
 ) -> np.ndarray | None:
     if stat is None:
         stat = conf.BACKGROUND_SUBTRACTION_STAT
     logging.info(f"Computing background from a frame stack using '{stat}'")
     averages = np.asarray(
         [get_frame_average_intensity(frame, ROI_mask) for frame in frame_stack]
     )
@@ -438,14 +442,17 @@
     if stat is None:
         stat = conf.BACKGROUND_SUBTRACTION_STAT
 
     frame_stack = generate_frame_stack(
         video_paths, episodes, n_frames_for_background, progress_bar
     )
 
+    if frame_stack is None:
+        return None
+
     background = generate_background_from_frame_stack(frame_stack, ROI_mask, stat)
 
     return background
 
 
 def gaussian_blur(frame: np.ndarray, sigma=None) -> np.ndarray:
     if sigma is not None and sigma > 0:
@@ -455,15 +462,17 @@
 
 def to_gray_scale(frame: np.ndarray) -> np.ndarray:
     if len(frame.shape) > 2:
         frame = cv2.cvtColor(frame, cv2.COLOR_RGB2GRAY)
     return frame
 
 
-def get_frame_average_intensity(frame: np.ndarray, mask: np.ndarray) -> np.float32:
+def get_frame_average_intensity(
+    frame: np.ndarray, mask: np.ndarray | None
+) -> np.float32:
     """Computes the average intensity of a given frame considering the maks.
     Only pixels with values
     different than zero in the mask are considered to compute the average
     intensity
 
     Parameters
     ----------
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/blob.py` & `idtrackerai-5.1.0/src/idtrackerai/blob.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,15 +401,15 @@
         """
         if isinstance(other, Blob):
             return ((np.asarray(self.centroid) - np.asarray(other.centroid)) ** 2).sum()
 
         if isinstance(other, (tuple, list, np.ndarray)):
             return ((np.asarray(self.centroid) - np.asarray(other)) ** 2).sum()
 
-        raise ValueError()
+        raise ValueError
 
     def distance_to(self, other: "Blob|tuple|list|np.ndarray") -> float:
         return sqrt(self.square_distance_to(other))
 
     def distance_from_countour_to(self, point):
         """Returns the distance between `point` and the closest
         point in the contour of the blob.
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/crossing_detector.py` & `idtrackerai-5.1.0/src/idtrackerai/crossings_detection/crossing_detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,23 +32,25 @@
 
 import torch
 from torch import nn
 from torch.backends import cudnn
 from torch.optim.lr_scheduler import MultiStepLR
 
 from idtrackerai import Blob, ListOfBlobs, Video
-from idtrackerai.network.learners.learners import LearnerClassification
-from idtrackerai.network.utils.utils import weights_xavier_init
+from idtrackerai.network import (
+    LearnerClassification,
+    NetworkParams,
+    weights_xavier_init,
+)
 from idtrackerai.utils import conf
 
 from .dataset.crossings_dataloader import get_training_data_loaders
 from .dataset.crossings_dataset import get_train_validation_and_eval_blobs
 from .model_area import ModelArea
-from .network.network_params_crossings import NetworkParamsCrossings
-from .network.predictor_crossing_detector import GetPredictionCrossigns
+from .network.predictor_crossing_detector import get_predictions_crossigns
 from .network.stop_training_criteria_crossings import StopTraining
 from .network.trainer_crossing_detector import train_deep_crossing
 
 
 def _apply_area_and_unicity_heuristics(
     blobs_in_video: list[list[Blob]], number_of_animals: int, model_area: ModelArea
 ):
@@ -106,39 +108,33 @@
         logging.debug("There are not enough crossings to train the crossing detector")
         return
     logging.info("There are enough crossings to train the crossing detector")
     train_loader, val_loader = get_training_data_loaders(
         video.id_images_file_paths, train_blobs, val_blobs
     )
     logging.info("Setting crossing detector network parameters")
-    network_params = NetworkParamsCrossings(
+    network_params = NetworkParams(
         number_of_classes=2,
         architecture="DCD",
         save_folder=video.crossings_detector_folder,
-        saveid="",
         model_name="crossing_detector",
         image_size=video.id_image_size,
         loss="CE",
-        print_freq=-1,
         use_gpu=True,
         optimizer="Adam",
         schedule=[30, 60],
         optim_args={"lr": conf.LEARNING_RATE_DCD},
         apply_mask=False,
         dataset="supervised",
         skip_eval=False,
         epochs=conf.MAXIMUM_NUMBER_OF_EPOCHS_DCD,
-        plot_flag=False,
     )
     logging.info("Setting training criterion")
     criterion = nn.CrossEntropyLoss(weight=torch.tensor(train_blobs["weights"]))
-    logging.info("Setting learner class")
-    learner_class = LearnerClassification
-    logging.info("Creating model")
-    crossing_detector_model = learner_class.create_model(network_params)  # type: ignore
+    crossing_detector_model = LearnerClassification.create_model(network_params)
     logging.info("Initialize networks params with Xavier initialization")
     crossing_detector_model.apply(weights_xavier_init)
 
     if network_params.use_gpu:
         torch.cuda.set_device(0)
         logging.info(
             'Sending model and criterion to GPU: "%s"', torch.cuda.get_device_name()
@@ -150,15 +146,17 @@
     logging.info("Setting optimizer")
     optimizer = torch.optim.__dict__[network_params.optimizer](
         crossing_detector_model.parameters(), **network_params.optim_args
     )
     logging.info("Setting scheduler")
     scheduler = MultiStepLR(optimizer, milestones=network_params.schedule, gamma=0.1)
     logging.info("Setting the learner")
-    learner = learner_class(crossing_detector_model, criterion, optimizer, scheduler)
+    learner = LearnerClassification(
+        crossing_detector_model, criterion, optimizer, scheduler
+    )
     logging.info("Setting the stopping criteria")
     # set criteria to stop the training
     stop_training = StopTraining(
         check_for_loss_plateau=True, num_epochs=network_params.epochs
     )
 
     model_diverged, best_model_path = train_deep_crossing(
@@ -176,18 +174,20 @@
     del val_loader
 
     model_state = torch.load(best_model_path)
     crossing_detector_model.load_state_dict(model_state, strict=True)
     logging.info("Loaded best model weights from %s", best_model_path)
 
     logging.info("Using crossing detector to classify individuals and crossings")
-    crossings_predictor = GetPredictionCrossigns(
-        video.id_images_file_paths, crossing_detector_model, eval_blobs, network_params
+    predictions = get_predictions_crossigns(
+        video.id_images_file_paths,
+        crossing_detector_model,
+        eval_blobs,
+        network_params.use_gpu,
     )
-    predictions = crossings_predictor.get_all_predictions()
 
     logging.info(
         "Prediction results: %d individuals and %d crossings",
         predictions.count(0),
         predictions.count(1),
     )
     for blob, prediction in zip(eval_blobs, predictions):
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/crossings_detection.py` & `idtrackerai-5.1.0/src/idtrackerai/crossings_detection/crossings_detection.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py` & `idtrackerai-5.1.0/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from pathlib import Path
 
 from torch.utils.data import DataLoader
 from torchvision import transforms
 
 from idtrackerai import Blob
 from idtrackerai.crossings_detection.dataset.crossings_dataset import CrossingDataset
-from idtrackerai.network.utils.utils import Normalize
+from idtrackerai.network import Normalize
 from idtrackerai.utils import conf
 
 if os.name == "nt":  # windows
     # Using multipricessing in Windows causes a
     # recursion limit error difficut to debug
     num_workers_train = 0
     num_workers_val = 0
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py` & `idtrackerai-5.1.0/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,16 @@
 
 
 def get_train_validation_and_eval_blobs(
     blobs_in_video: list[list[Blob]],
     number_of_animals: int,
     ratio_validation: float = 0.1,
 ) -> tuple[dict[str, list[Blob]], dict[str, list[Blob]], list[Blob]]:
-    """Given a list of blobs return 2 dictionaries (training_blobs, validation_blobs), and a list (toassign_blobs).
+    """Given a list of blobs return 2 dictionaries (training_blobs, validation_blobs),
+    and a list (toassign_blobs).
 
     :param list_of_blobs:
     :param ratio_validation:
     :return: training_blobs, validation_blobs, toassign_blobs
     """
     logging.info("Get list of blobs for training, validation and eval")
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/model_area.py` & `idtrackerai-5.1.0/src/idtrackerai/crossings_detection/model_area.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,16 @@
       some description
     """
 
     def __init__(self, blobs_in_video: list[list[Blob]], number_of_animals: int):
         """computes the median and standard deviation of the area of all the blobs
         in the the video and the median of the the diagonal of the bounding box.
         """
-        # areas are collected throughout the entire video in the cores of the global fragments
+        # areas are collected throughout the entire video inthe cores of the
+        # global fragments
         logging.info(
             "Initializing ModelArea for individual/crossing blob initial classification"
         )
         areas = []
         for blobs_in_frame in blobs_in_video:
             if len(blobs_in_frame) == number_of_animals:
                 for blob in blobs_in_frame:
@@ -99,15 +100,16 @@
         return (area - self.median) < self.tolerance
 
 
 def compute_body_length(
     blobs_in_video: list[list[Blob]], number_of_animals: int
 ) -> float:
     """computes the median of the the diagonal of the bounding box."""
-    # areas are collected throughout the entire video in the cores of the global fragments
+    # areas are collected throughout the entire video in the cores of
+    # the global fragments
     body_lengths = []
     for blobs_in_frame in blobs_in_video:
         if len(blobs_in_frame) == number_of_animals:
             for blob in blobs_in_frame:
                 body_lengths.append(blob.estimated_body_length)
     median = np.median(body_lengths)
     logging.info(f"Median body length: {median} pixels")
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py` & `idtrackerai-5.1.0/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,29 @@
     """Stops the training of the network according to the conditions specified
     in __call__
     """
 
     def __init__(
         self,
         epochs_before_checking_stopping_conditions=10,
-        check_for_loss_plateau=True,
+        check_for_loss_plateau: bool = True,
         num_epochs=10,
     ):
         self.num_epochs = num_epochs  # maximal num of epochs
         self.number_of_classes = 2
         self.epochs_before_checking_stopping_conditions = (
             epochs_before_checking_stopping_conditions
         )
-        # number of epochs in which the network is overfitting before stopping the training
-        self.overfitting_counter = 0
-        # bool: if true the training is stopped if the loss is not decreasing enough
+        self.overfitting_counter: int = 0
+        """Number of epochs in which the network is overfitting before
+        stopping the training"""
+
         self.check_for_loss_plateau = check_for_loss_plateau
+        """if true the training is stopped if the loss is not decreasing enough"""
+
         self.epochs_completed = -1
 
     def __call__(
         self,
         loss_training: list,
         loss_validation: list,
         accuracy_validation: list,
@@ -104,25 +107,24 @@
                 if self.overfitting_counter >= conf.OVERFITTING_COUNTER_THRESHOLD_DCD:
                     status.stop()
                     logging.info("Overfitting")
                     return True
             else:
                 self.overfitting_counter = 0
             # check if the error is not decreasing much
-            if self.check_for_loss_plateau:
-                if np.abs(
-                    losses_difference
-                ) < conf.LEARNING_PERCENTAGE_DIFFERENCE_2_DCD * 10 ** (
-                    int(np.log10(current_loss)) - 1
-                ):
-                    status.stop()
-                    logging.info(
-                        "The losses difference is very small, we stop the training"
-                    )
-                    return True
+            if self.check_for_loss_plateau and np.abs(
+                losses_difference
+            ) < conf.LEARNING_PERCENTAGE_DIFFERENCE_2_DCD * 10 ** (
+                int(np.log10(current_loss)) - 1
+            ):
+                status.stop()
+                logging.info(
+                    "The losses difference is very small, we stop the training"
+                )
+                return True
             # if the individual accuracies in validation are 1. for all the animals
             if accuracy_validation[-1] == 1.0:
                 status.stop()
                 logging.info("The accuracy in validation is 100%, we stop the training")
                 return True
             # if the validation loss is 0.
             if previous_loss == 0.0 or current_loss == 0.0:
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py` & `idtrackerai-5.1.0/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,32 +25,30 @@
 # de Polavieja, G.G., Nature Methods, 2019.
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import logging
+from contextlib import suppress
 from pathlib import Path
 
 import numpy as np
 from rich.console import Console
 
-from idtrackerai.network.evaluate import evaluate
-from idtrackerai.network.learners.learners import LearnerClassification
-from idtrackerai.network.train import train
+from idtrackerai.network import LearnerClassification, NetworkParams, evaluate, train
 
-from ..network.network_params_crossings import NetworkParamsCrossings
-from ..network.stop_training_criteria_crossings import StopTraining
+from .stop_training_criteria_crossings import StopTraining
 
 
 def train_deep_crossing(
     learner: LearnerClassification,
     train_loader,
     val_loader,
-    network_params: NetworkParamsCrossings,
+    network_params: NetworkParams,
     stop_training: StopTraining,
 ) -> tuple[bool, Path]:
     logging.info("Training Deep Crossing Detector")
 
     # Initialize metric storage
     train_losses = []
     if network_params.loss in ("CEMCL", "CEMCL_weighted"):
@@ -86,21 +84,19 @@
                 if network_params.loss in ("CEMCL", "CEMCL_weighted"):
                     val_losses_CE.append(loss_CE)
                     val_losses_MCL.append(loss_MCL)
                 val_accs.append(val_acc)
             # Save checkpoint at each LR steps and the end of optimization
             best_model_path = learner.snapshot(
                 network_params.save_folder
-                / f"{network_params.dataset}_{network_params.model_name}_{network_params.saveid}"
+                / f"{network_params.dataset}_{network_params.model_name}"
             )
-            try:
+            with suppress(IndexError):
                 status.update(
                     f"[red]Epochs loop {epoch}: training loss ="
                     f" {train_losses[-1]:.6f}, validation loss ="
                     f" {val_losses[-1]:.6f} and accuracy = {val_accs[-1]:.4%}"
                 )
-            except IndexError:
-                pass
 
         logging.info("Last epoch loop: %s", status.status, extra={"markup": True})
 
     return np.isnan(train_losses[-1]) or np.isnan(val_losses[-1]), best_model_path
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/data/test_A.avi` & `idtrackerai-5.1.0/src/idtrackerai/data/test_A.avi`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/data/test_B.avi` & `idtrackerai-5.1.0/src/idtrackerai/data/test_B.avi`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/fragment.py` & `idtrackerai-5.1.0/src/idtrackerai/fragment.py`

 * *Files 3% similar despite different names*

```diff
@@ -377,18 +377,18 @@
         Returns
         -------
         bool
             True if the identification of self with `temporary_id` does not
             cause any duplication of identities.
 
         """
-        for coexisting_fragment in self.coexisting_individual_fragments:
-            if coexisting_fragment.temporary_id == temporary_id:
-                return False
-        return True
+        return all(
+            coexisting_fragment.temporary_id != temporary_id
+            for coexisting_fragment in self.coexisting_individual_fragments
+        )
 
     def compute_identification_statistics(
         self, predictions: np.ndarray | list, softmax_probs, number_of_animals=None
     ):
         """Computes the statistics necessary for the identification of the
         fragment.
 
@@ -402,27 +402,24 @@
             whose rows are the result of applying the softmax function to the
             predictions outputted by the idCNN per image
         number_of_animals : int
             Description of parameter `number_of_animals`.
 
         See Also
         --------
-        :meth:`compute_identification_frequencies_individual_fragment`
         :meth:`set_P1_from_frequencies`
         :meth:`compute_median_softmax`
         :meth:`compute_certainty_of_individual_fragment`
         """
         assert self.is_an_individual
         number_of_animals = (
             self.number_of_animals if number_of_animals is None else number_of_animals
         )
         self.set_P1_from_frequencies(
-            self.compute_identification_frequencies_individual_fragment(
-                np.asarray(predictions), number_of_animals
-            )
+            np.bincount(predictions, minlength=number_of_animals + 1)[1:]
         )
         median_softmax = self.compute_median_softmax(softmax_probs, number_of_animals)
         self.certainty = self.compute_certainty_of_individual_fragment(
             self.P1_vector, median_softmax
         )
 
     def set_P1_vector_accumulated(self):
@@ -498,37 +495,14 @@
                 if P2_second_max == 0
                 else P2_first_max / P2_second_max
             )
         else:
             self.P2_vector = np.zeros(self.number_of_animals)
             self.certainty_P2 = 0.0
 
-    @staticmethod
-    def compute_identification_frequencies_individual_fragment(
-        predictions: np.ndarray, number_of_animals: int
-    ) -> np.ndarray:
-        """Counts the argmax of predictions per identity
-
-        Parameters
-        ----------
-        predictions : numpy array
-            Array of shape [number of images in fragment, 1] with the identity
-            assigned to each image in the fragment.
-            Predictions come from 1 to number of animals to be tracked.
-        number_of_animals : int
-            number of animals to be tracked
-
-        Returns
-        -------
-        ndarray
-            array of shape [1, number_of_animals], whose i-th component counts
-            how many predictions have maximum components at the identity i
-        """
-        return np.bincount(predictions, minlength=number_of_animals + 1)[1:]
-
     def set_P1_from_frequencies(self, frequencies: np.ndarray):
         """Given the frequencies of a individual fragment
         computer the P1 vector.
 
         P1 is the softmax of the frequencies with base 2 for each identity.
         Numpy array indicating the number of images assigned with each of
         the possible identities
@@ -593,15 +567,15 @@
             Fragment's certainty
 
         """
         argsort_p1_vector = P1_vector.argsort()
         sorted_p1_vector = P1_vector[argsort_p1_vector]
         sorted_softmax_probs = median_softmax[argsort_p1_vector]
         certainty = (
-            np.diff(np.multiply(sorted_p1_vector, sorted_softmax_probs)[-2:])
+            np.diff((sorted_p1_vector * sorted_softmax_probs)[-2:])
             / sorted_p1_vector[-2:].sum()
         )
         return certainty[0]
 
     def get_neighbour_fragment(
         self,
         fragments: list["Fragment"],
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/fragmentation/fragmentation.py` & `idtrackerai-5.1.0/src/idtrackerai/fragmentation/fragmentation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/globalfragment.py` & `idtrackerai-5.1.0/src/idtrackerai/globalfragment.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,34 +108,34 @@
     @property
     def is_unique(self):
         """Boolean indicating that the global fragment has unique
         identities, i.e. it does not have duplications."""
         return (
             len(
                 set(range(self.number_of_animals))
-                - set(fragment.temporary_id for fragment in self.individual_fragments)
+                - {fragment.temporary_id for fragment in self.individual_fragments}
             )
             == 0
         )
 
     @property
     def is_partially_unique(self):
         """Boolean indicating that a subset of the fragments in the global
         fragment have unique identities"""
 
         identities_acceptable_for_training = [
             fragment.temporary_id
             for fragment in self.individual_fragments
             if fragment.acceptable_for_training
         ]
-        self.duplicated_identities = set(
+        self.duplicated_identities = {
             x
             for x in identities_acceptable_for_training
             if identities_acceptable_for_training.count(x) > 1
-        )
+        }
         return len(self.duplicated_identities) == 0
 
     def _init_attributes(self):
         """Initializes some attributes required for the cascade of
         training and identification protocols"""
         self.predictions = []
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py` & `idtrackerai-5.1.0/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,72 +1,41 @@
-# This file is part of idtracker.ai a multiple animals tracking system
-# described in [1].
-# Copyright (C) 2017- Francisco Romero Ferrero, Mattia G. Bergomi,
-# Francisco J.H. Heras, Robert Hinz, Gonzalo G. de Polavieja and the
-# Champalimaud Foundation.
-#
-# idtracker.ai is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details. In addition, we require
-# derivatives or applications to acknowledge the authors by citing [1].
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-# For more information please send an email (idtrackerai@gmail.com) or
-# use the tools available at https://gitlab.com/polavieja_lab/idtrackerai.git.
-#
-# [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
-# de Polavieja, G.G., Nature Methods, 2019.
-# idtracker.ai: tracking all individuals in small or large collectives of
-# unmarked animals.
-# (F.R.-F. and M.G.B. contributed equally to this work.
-# Correspondence should be addressed to G.G.d.P:
-# gonzalo.polavieja@neuro.fchampalimaud.org)
+"""Given two list of blobs_in_video, one deduced from human groundtruth and the other
+generated by the tracking algorithm, compares them and gives back some statistics
 
+Crossing: crossings are a special case. We ...
+"""
 import logging
 import os
 import sys
 
 import numpy as np
 
 from idtrackerai import ListOfBlobs
 
-"""Given two list of blobs_in_video, one deduced from human groundtruth and the other
-generated by the tracking algorithm, compares them and gives back some statistics
-
-Crossing: crossings are a special case. We ...
-"""
-
 
 def compare_tracking_against_groundtruth_no_gaps(
     number_of_animals,
     groundtruth,
     blobs_in_video_groundtruth,
     blobs_in_video,
     identities_dictionary_permutation,
 ):
     """
     blobs_in_video_groundtruth: cut groundtruth.blobs_in_video using start
     and end of the groundtruth object
     blobs_in_video: cut list_of_blobs.blobs_in_video using start and end of
     the groundtruth object
     """
-    results = {}
-    results["number_of_blobs_per_identity"] = {
-        identity: 0 for identity in range(1, number_of_animals + 1)
-    }
-    results["number_of_individuals_badly_assigned"] = {
-        identity: 0 for identity in range(1, number_of_animals + 1)
+    results = {
+        "number_of_blobs_per_identity": {
+            identity: 0 for identity in range(1, number_of_animals + 1)
+        },
+        "number_of_individuals_badly_assigned": {
+            identity: 0 for identity in range(1, number_of_animals + 1)
+        },
     }
     if identities_dictionary_permutation is not None:
         results["number_of_individuals_badly_interpolated"] = {
             identities_dictionary_permutation[
                 identity
             ]: groundtruth.wrong_crossing_counter[identity]
             for identity in groundtruth.wrong_crossing_counter
@@ -107,17 +76,20 @@
                     if identity != 0:
                         results["number_of_blobs_per_identity"][identity] += 1
             elif gt_identity is None:
                 logging.debug(
                     "***************************************unidentified blobs"
                 )
 
-            if blob_gt.is_an_individual and not blob_gt.was_a_crossing:
-                if gt_identity != blob.assigned_identities:
-                    results["number_of_individuals_badly_assigned"][gt_identity] += 1
+            if (
+                blob_gt.is_an_individual
+                and not blob_gt.was_a_crossing
+                and gt_identity != blob.assigned_identities
+            ):
+                results["number_of_individuals_badly_assigned"][gt_identity] += 1
 
     results["number_of_errors_in_all_blobs"] = {
         i: (
             results["number_of_individuals_badly_assigned"][i]
             + results["number_of_individuals_badly_interpolated"][i]
         )
         for i in range(1, number_of_animals + 1)
@@ -146,75 +118,75 @@
         number_of_animals,
         groundtruth,
         blobs_in_video_groundtruth,
         blobs_in_video,
         identities_dictionary_permutation,
     )
 
-    accuracies = {}
-    accuracies["individual_accuracy"] = {
-        i: (
-            1.0
-            - results["number_of_errors_in_all_blobs"][i]
-            / results["number_of_blobs_per_identity"][i]
-        )
-        for i in range(1, number_of_animals + 1)
+    accuracies = {
+        "individual_accuracy": {
+            i: (
+                1.0
+                - results["number_of_errors_in_all_blobs"][i]
+                / results["number_of_blobs_per_identity"][i]
+            )
+            for i in range(1, number_of_animals + 1)
+        }
     }
     accuracies["accuracy"] = np.mean(list(accuracies["individual_accuracy"].values()))
     logging.info(accuracies)
     logging.info(results)
     return accuracies, results
 
 
 def compare_tracking_against_groundtruth(
     number_of_animals,
     blobs_in_video_groundtruth,
     blobs_in_video,
     identities_dictionary_permutation,
 ):
     # create dictionary to store eventual corrections made by the user
-    results = {}
-    results["number_of_blobs_per_identity"] = {
-        i: 0 for i in range(1, number_of_animals + 1)
-    }
-    results["sum_individual_P2"] = {i: 0 for i in range(1, number_of_animals + 1)}
-    results["number_of_assigned_blobs_per_identity"] = {
-        i: 0 for i in range(1, number_of_animals + 1)
-    }
-    results["number_of_blobs_assigned_during_accumulation_per_identity"] = {
-        i: 0 for i in range(1, number_of_animals + 1)
-    }
-    results["number_of_blobs_after_accumulation_per_identity"] = {
-        i: 0 for i in range(1, number_of_animals + 1)
-    }
-    results["number_of_errors_in_all_blobs"] = {
-        i: 0 for i in range(1, number_of_animals + 1)
-    }
-    results["number_of_errors_in_assigned_blobs"] = {
-        i: 0 for i in range(1, number_of_animals + 1)
+    results = {
+        "number_of_blobs_per_identity": {i: 0 for i in range(1, number_of_animals + 1)},
+        "sum_individual_P2": {i: 0 for i in range(1, number_of_animals + 1)},
+        "number_of_assigned_blobs_per_identity": {
+            i: 0 for i in range(1, number_of_animals + 1)
+        },
+        "number_of_blobs_assigned_during_accumulation_per_identity": {
+            i: 0 for i in range(1, number_of_animals + 1)
+        },
+        "number_of_blobs_after_accumulation_per_identity": {
+            i: 0 for i in range(1, number_of_animals + 1)
+        },
+        "number_of_errors_in_all_blobs": {
+            i: 0 for i in range(1, number_of_animals + 1)
+        },
+        "number_of_errors_in_assigned_blobs": {
+            i: 0 for i in range(1, number_of_animals + 1)
+        },
+        "number_of_errors_in_blobs_assigned_during_accumulation": {
+            i: 0 for i in range(1, number_of_animals + 1)
+        },
+        "number_of_errors_in_blobs_after_accumulation": {
+            i: 0 for i in range(1, number_of_animals + 1)
+        },
+        "number_of_errors_in_blobs_assigned_after_accumulation": {
+            i: 0 for i in range(1, number_of_animals + 1)
+        },
+        "number_of_individual_blobs": 0,
+        "number_of_crossing_blobs": 0,
+        "number_of_crossings_blobs_assigned_as_individuals": 0,
+        "frames_with_identity_errors": [],
+        "fragment_identifiers_with_identity_errors": [],
+        "frames_with_crossing_errors": [],
+        "fragment_identifiers_with_crossing_errors": [],
+        "frames_with_zeros_in_groundtruth": [],
+        "number_of_crossing_fragments": 0,
+        "fragments_identifiers_of_crossings": [],
     }
-    results["number_of_errors_in_blobs_assigned_during_accumulation"] = {
-        i: 0 for i in range(1, number_of_animals + 1)
-    }
-    results["number_of_errors_in_blobs_after_accumulation"] = {
-        i: 0 for i in range(1, number_of_animals + 1)
-    }
-    results["number_of_errors_in_blobs_assigned_after_accumulation"] = {
-        i: 0 for i in range(1, number_of_animals + 1)
-    }
-    results["number_of_individual_blobs"] = 0
-    results["number_of_crossing_blobs"] = 0
-    results["number_of_crossings_blobs_assigned_as_individuals"] = 0
-    results["frames_with_identity_errors"] = []
-    results["fragment_identifiers_with_identity_errors"] = []
-    results["frames_with_crossing_errors"] = []
-    results["fragment_identifiers_with_crossing_errors"] = []
-    results["frames_with_zeros_in_groundtruth"] = []
-    results["number_of_crossing_fragments"] = 0
-    results["fragments_identifiers_of_crossings"] = []
 
     for groundtruth_blobs_in_frame, blobs_in_frame in zip(
         blobs_in_video_groundtruth, blobs_in_video
     ):
         for groundtruth_blob, blob in zip(groundtruth_blobs_in_frame, blobs_in_frame):
             if identities_dictionary_permutation is not None:
                 gt_identity = identities_dictionary_permutation[
@@ -293,23 +265,22 @@
                         blob.fragment_identifier
                     )
                     results["number_of_crossing_fragments"] += 1
                 results["number_of_crossing_blobs"] += 1
                 results["number_of_crossings_blobs_assigned_as_individuals"] += (
                     1 if blob.is_an_individual else 0
                 )
-                if blob.is_an_individual:
-                    if (
+                if blob.is_an_individual and (
+                    blob.fragment_identifier
+                    not in results["fragment_identifiers_with_crossing_errors"]
+                ):
+                    results["frames_with_crossing_errors"].append(blob.frame_number)
+                    results["fragment_identifiers_with_crossing_errors"].append(
                         blob.fragment_identifier
-                        not in results["fragment_identifiers_with_crossing_errors"]
-                    ):
-                        results["frames_with_crossing_errors"].append(blob.frame_number)
-                        results["fragment_identifiers_with_crossing_errors"].append(
-                            blob.fragment_identifier
-                        )
+                    )
 
     return results
 
 
 def check_ground_truth_consistency(
     blobs_in_video_groundtruth, blobs_in_video, first_frame_first_global_fragment
 ):
@@ -386,76 +357,78 @@
     results = compare_tracking_against_groundtruth(
         number_of_animals,
         blobs_in_video_groundtruth,
         blobs_in_video,
         identities_dictionary_permutation,
     )
     if len(results["frames_with_zeros_in_groundtruth"]) == 0:
-        accuracies = {}
-        accuracies["percentage_of_unoccluded_images"] = results[
-            "number_of_individual_blobs"
-        ] / (
-            results["number_of_individual_blobs"] + results["number_of_crossing_blobs"]
-        )
-        accuracies["individual_P2_in_validated_part"] = {
-            i: (
-                results["sum_individual_P2"][i]
-                / results["number_of_blobs_per_identity"][i]
-            )
-            for i in range(1, number_of_animals + 1)
-        }
-        accuracies["mean_individual_P2_in_validated_part"] = np.sum(
-            list(results["sum_individual_P2"].values())
-        ) / np.sum(list(results["number_of_blobs_per_identity"].values()))
-        accuracies["individual_accuracy"] = {
-            i: (
-                1
-                - results["number_of_errors_in_all_blobs"][i]
-                / results["number_of_blobs_per_identity"][i]
-            )
-            for i in range(1, number_of_animals + 1)
-        }
-        accuracies["accuracy"] = 1.0 - np.sum(
-            list(results["number_of_errors_in_all_blobs"].values())
-        ) / np.sum(list(results["number_of_blobs_per_identity"].values()))
-        accuracies["individual_accuracy_assigned"] = {
-            i: (
-                1
-                - results["number_of_errors_in_assigned_blobs"][i]
-                / results["number_of_assigned_blobs_per_identity"][i]
-            )
-            for i in range(1, number_of_animals + 1)
-        }
-        accuracies["accuracy_assigned"] = 1.0 - np.sum(
-            list(results["number_of_errors_in_assigned_blobs"].values())
-        ) / np.sum(list(results["number_of_assigned_blobs_per_identity"].values()))
-        accuracies["individual_accuracy_in_accumulation"] = {
-            i: (
-                1
-                - results["number_of_errors_in_blobs_assigned_during_accumulation"][i]
-                / results["number_of_blobs_assigned_during_accumulation_per_identity"][
-                    i
-                ]
-            )
-            for i in range(1, number_of_animals + 1)
+        accuracies = {
+            "percentage_of_unoccluded_images": results["number_of_individual_blobs"] / (
+                results["number_of_individual_blobs"]
+                + results["number_of_crossing_blobs"]
+            ),
+            "individual_P2_in_validated_part": {
+                i: (
+                    results["sum_individual_P2"][i]
+                    / results["number_of_blobs_per_identity"][i]
+                )
+                for i in range(1, number_of_animals + 1)
+            },
+            "mean_individual_P2_in_validated_part": np.sum(
+                list(results["sum_individual_P2"].values())
+            ) / np.sum(list(results["number_of_blobs_per_identity"].values())),
+            "individual_accuracy": {
+                i: (
+                    1
+                    - results["number_of_errors_in_all_blobs"][i]
+                    / results["number_of_blobs_per_identity"][i]
+                )
+                for i in range(1, number_of_animals + 1)
+            },
+            "accuracy": 1.0 - np.sum(
+                list(results["number_of_errors_in_all_blobs"].values())
+            ) / np.sum(list(results["number_of_blobs_per_identity"].values())),
+            "individual_accuracy_assigned": {
+                i: (
+                    1
+                    - results["number_of_errors_in_assigned_blobs"][i]
+                    / results["number_of_assigned_blobs_per_identity"][i]
+                )
+                for i in range(1, number_of_animals + 1)
+            },
+            "accuracy_assigned": 1.0 - np.sum(
+                list(results["number_of_errors_in_assigned_blobs"].values())
+            ) / np.sum(list(results["number_of_assigned_blobs_per_identity"].values())),
+            "individual_accuracy_in_accumulation": {
+                i: (
+                    1
+                    - results["number_of_errors_in_blobs_assigned_during_accumulation"][
+                        i
+                    ]
+                    / results[
+                        "number_of_blobs_assigned_during_accumulation_per_identity"
+                    ][i]
+                )
+                for i in range(1, number_of_animals + 1)
+            },
+            "accuracy_in_accumulation": 1.0 - np.sum(
+                list(
+                    results[
+                        "number_of_errors_in_blobs_assigned_during_accumulation"
+                    ].values()
+                )
+            ) / np.sum(
+                list(
+                    results[
+                        "number_of_blobs_assigned_during_accumulation_per_identity"
+                    ].values()
+                )
+            ),
+            "individual_accuracy_after_accumulation": {},
         }
-        accuracies["accuracy_in_accumulation"] = 1.0 - np.sum(
-            list(
-                results[
-                    "number_of_errors_in_blobs_assigned_during_accumulation"
-                ].values()
-            )
-        ) / np.sum(
-            list(
-                results[
-                    "number_of_blobs_assigned_during_accumulation_per_identity"
-                ].values()
-            )
-        )
-        accuracies["individual_accuracy_after_accumulation"] = {}
         for i in range(1, number_of_animals + 1):
             if results["number_of_blobs_after_accumulation_per_identity"][i] != 0:
                 accuracies["individual_accuracy_after_accumulation"][i] = (
                     1
                     - results["number_of_errors_in_blobs_after_accumulation"][i]
                     / results["number_of_blobs_after_accumulation_per_identity"][i]
                 )
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py` & `idtrackerai-5.1.0/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,21 @@
-# This file is part of idtracker.ai a multiple animals tracking system
-# described in [1].
-# Copyright (C) 2017- Francisco Romero Ferrero, Mattia G. Bergomi,
-# Francisco J.H. Heras, Robert Hinz, Gonzalo G. de Polavieja and the
-# Champalimaud Foundation.
-#
-# idtracker.ai is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details. In addition, we require
-# derivatives or applications to acknowledge the authors by citing [1].
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-# For more information please send an email (idtrackerai@gmail.com) or
-# use the tools available at https://gitlab.com/polavieja_lab/idtrackerai.git.
-#
-# [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
-# de Polavieja, G.G., Nature Methods, 2019.
-# idtracker.ai: tracking all individuals in small or large collectives of
-# unmarked animals.
-# (F.R.-F. and M.G.B. contributed equally to this work.
-# Correspondence should be addressed to G.G.d.P:
-# gonzalo.polavieja@neuro.fchampalimaud.org)
+"""Given two list of blobs_in_video, one deduced from human ground_truth and the
+other generated by the tracking algorithm, compares them and gives back some
+statistics
 
+Crossing: crossings are a special case. We ...
+"""
 import logging
 import os
 from pprint import pprint
 
 import numpy as np
 
 from idtrackerai import ListOfBlobs, Video
 
-"""Given two list of blobs_in_video, one deduced from human ground_truth and the
-other generated by the tracking algorithm, compares them and gives back some
-statistics
-
-Crossing: crossings are a special case. We ...
-"""
-
 
 def get_corresponding_gt_blob(blob, gt_blobs_in_frame):
     """Returs the blobs in the `gt_blobs_in_frame` that overlap (in pixels)
     with a given `blob` of the tracked trajectories.
 
     :param blob: <Blob object>
     :param gt_blobs_in_frame: list of <GroundTruthBlob objects> corresponding
@@ -175,48 +143,42 @@
 
 
 def per_id_counter_dict(num_animals):
     return {i: 0 for i in range(1, num_animals + 1)}
 
 
 def init_results_dict(num_animals):
-    results = {}
-    results["num_blobs"] = per_id_counter_dict(num_animals)
-    results["sum_indiv_P2"] = per_id_counter_dict(num_animals)
-    results["num_id_blobs"] = per_id_counter_dict(num_animals)
-    results["num_id_blobs_accum"] = per_id_counter_dict(num_animals)
-    results["num_blobs_after_accum"] = per_id_counter_dict(num_animals)
-    results["errors_blobs"] = per_id_counter_dict(num_animals)
-    results["errors_id_blobs"] = per_id_counter_dict(num_animals)
-    results["errors_blobs_after_accum"] = per_id_counter_dict(num_animals)
-    results["errors_id_blobs_accum"] = per_id_counter_dict(num_animals)
-    results["errors_id_blobs_after_accum"] = per_id_counter_dict(num_animals)
-
-    results["frames_w_id_errors"] = set()
-    results["frag_w_id_errors"] = set()
-    results["frames_w_crossing_errors"] = set()
-    results["frag_w_crossing_errors"] = set()
-    results["frames_w_0_id_in_gt"] = set()
-    results["num_crossing_frags"] = 0
-    results["frag_crossings"] = set()
-
-    # Crossing detector
-    results["crossing_detector_tn"] = 0
-    results["crossing_detector_fn"] = 0
-    results["crossing_detector_tp"] = 0
-    results["crossing_detector_fp"] = 0
-
-    results["num_indiv_gt_blobs"] = 0
-    results["num_crossing_gt_blobs"] = 0
-    results["num_indiv_blobs"] = 0
-    results["num_crossing_blobs"] = 0
-
-    results["frame_with_crossing_detection_error"] = set()
-
-    return results
+    return {
+        "num_blobs": per_id_counter_dict(num_animals),
+        "sum_indiv_P2": per_id_counter_dict(num_animals),
+        "num_id_blobs": per_id_counter_dict(num_animals),
+        "num_id_blobs_accum": per_id_counter_dict(num_animals),
+        "num_blobs_after_accum": per_id_counter_dict(num_animals),
+        "errors_blobs": per_id_counter_dict(num_animals),
+        "errors_id_blobs": per_id_counter_dict(num_animals),
+        "errors_blobs_after_accum": per_id_counter_dict(num_animals),
+        "errors_id_blobs_accum": per_id_counter_dict(num_animals),
+        "errors_id_blobs_after_accum": per_id_counter_dict(num_animals),
+        "frames_w_id_errors": set(),
+        "frag_w_id_errors": set(),
+        "frames_w_crossing_errors": set(),
+        "frag_w_crossing_errors": set(),
+        "frames_w_0_id_in_gt": set(),
+        "num_crossing_frags": 0,
+        "frag_crossings": set(),
+        "crossing_detector_tn": 0,
+        "crossing_detector_fn": 0,
+        "crossing_detector_tp": 0,
+        "crossing_detector_fp": 0,
+        "num_indiv_gt_blobs": 0,
+        "num_crossing_gt_blobs": 0,
+        "num_indiv_blobs": 0,
+        "num_crossing_blobs": 0,
+        "frame_with_crossing_detection_error": set(),
+    }
 
 
 def aggregate_counters(results):
     results["total_sum_P2"] = np.sum(list(results["sum_indiv_P2"].values()))
     results["total_num_blobs"] = (
         results["num_indiv_gt_blobs"] + results["num_crossing_gt_blobs"]
     )
@@ -340,23 +302,22 @@
             raise Exception("No identities permutation found")
     logging.info(f"The identities permutation is {ids_perm_dict}")
     assert len(ids_perm_dict) == video.number_of_animals
     return ids_perm_dict
 
 
 def compute_performance(results, number_of_animals):
-    accuracies = {}
-
-    accuracies["percentage_of_unoccluded_images"] = (
-        results["num_indiv_gt_blobs"] / results["total_num_blobs"]
-    )
-
-    accuracies["mean_individual_P2_in_validated_part"] = (
-        results["total_sum_P2"] / results["total_indiv_blobs"]
-    )
+    accuracies = {
+        "percentage_of_unoccluded_images": (
+            results["num_indiv_gt_blobs"] / results["total_num_blobs"]
+        ),
+        "mean_individual_P2_in_validated_part": (
+            results["total_sum_P2"] / results["total_indiv_blobs"]
+        ),
+    }
 
     error_rate = results["total_num_errors"] / results["total_indiv_blobs"]
     accuracies["accuracy"] = 1.0 - error_rate
 
     error_rate = (
         results["total_errors_assigned_blobs"] / results["total_assigned_blobs"]
     )
@@ -483,15 +444,15 @@
 
 def compute_and_save_session_accuracy_wrt_groundtruth(video: Video, gt_type=None):
     if gt_type == "normal":
         list_of_blobs_path = video.blobs_path
         performance_func = get_accuracy_wrt_groundtruth
     elif gt_type == "no_gaps":
         raise Exception(f"No performance_func to compute for {gt_type}")
-        ### TODO: fixh get_accuracy_wrt_groundtruth_no_gaps
+        # TODO: fixh get_accuracy_wrt_groundtruth_no_gaps
         # list_of_blobs_path = video.blobs_no_gaps_path
         # gt_path = os.path.join(
         #     video.video_folder, "_groundtruth_with_crossing_identified.npy"
         # )
         # performance_func = get_accuracy_wrt_groundtruth_no_gaps
 
     else:
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py` & `idtrackerai-5.1.0/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/groundtruth_utils/generate_groundtruth.py` & `idtrackerai-5.1.0/src/idtrackerai/groundtruth_utils/generate_groundtruth.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,17 @@
     def __init__(self, blob):
         self.attributes = ATTRIBUTES_TO_COPY
         self.set_attributes(blob)
 
     def set_attributes(self, blob):
         for attribute in self.attributes:
             if attribute == "identities":
-                setattr(self, attribute, getattr(blob, "final_identities"))
+                setattr(self, attribute, blob.final_identities)
             elif attribute == "centroids":
-                setattr(self, attribute, getattr(blob, "final_centroids"))
+                setattr(self, attribute, blob.final_centroids)
             else:
                 setattr(self, attribute, getattr(blob, attribute))
 
     @property
     def gt_identity(self):
         if hasattr(self, "identity"):
             return self.identity
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py` & `idtrackerai-5.1.0/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,45 +39,41 @@
     """Lighter blob objects.
     Attributes:
         identity (preferring the one assigned by the user, if it is not None)
         centroid
         pixels (pixels is stored to check the groundtruth in crossings)
     """
 
-    def __init__(
-        self,
-        attributes_to_get=[
-            "identity",
-            "assigned_identity",
-            "used_for_training",
-            "accumulation_step",
-            "centroid",
-            "pixels",
-            "frame_number",
-            "is_an_individual",
-            "is_a_crossing",
-            "blob_index",
-            "fragment_identifier",
-        ],
-    ):
-        self.attributes = attributes_to_get
+    attributes = [
+        "identity",
+        "assigned_identity",
+        "used_for_training",
+        "accumulation_step",
+        "centroid",
+        "pixels",
+        "frame_number",
+        "is_an_individual",
+        "is_a_crossing",
+        "blob_index",
+        "fragment_identifier",
+    ]
 
     def get_attribute(self, blob):
         for attribute in self.attributes:
             if attribute == "identity":
-                setattr(self, attribute, getattr(blob, "final_identity"))
+                setattr(self, attribute, blob.final_identity)
             else:
                 setattr(self, attribute, getattr(blob, attribute))
 
 
 class IndividualGroundTruth:
     def __init__(
         self,
-        video=[],
-        individual_blobs_in_video=[],
+        video,
+        individual_blobs_in_video,
         start=None,
         end=None,
         validated_identity=None,
     ):
         self.video = video
         self.individual_blobs_in_video = individual_blobs_in_video
         self.start = start
@@ -102,15 +98,14 @@
 ):
     """Generates a list of light blobs_in_video, given a video object corresponding to a
     tracked video
     """
     individual_blobs_in_video_groundtruth = []
 
     for blobs_in_frame in blobs_in_video:
-        identities_in_frame = set([blob.final_identity for blob in blobs_in_frame])
         for blob in blobs_in_frame:
             if blob.final_identity == validated_identity:
                 gt_blob = GroundTruthBlob()
                 gt_blob.get_attribute(blob)
                 individual_blobs_in_video_groundtruth.append(gt_blob)
 
     groundtruth = IndividualGroundTruth(
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/list_of_blobs.py` & `idtrackerai-5.1.0/src/idtrackerai/list_of_blobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import itertools
 import logging
 import pickle
+from contextlib import suppress
 from multiprocessing import Pool
 from pathlib import Path
 from typing import Optional
 
 import h5py
 import numpy as np
 
@@ -112,21 +113,17 @@
                 self.blobs_in_video[frame_i], self.blobs_in_video[frame_i + 1]
             ):
                 if blob_0.overlaps_with(blob_1):
                     blob_0.now_points_to(blob_1)
         self.blobs_are_connected = True
 
         # clean cached property
-        for blob in self.all_blobs:
-            try:
+        with suppress(AttributeError):
+            for blob in self.all_blobs:
                 del blob.convexHull
-            except AttributeError:
-                # Some blob'b bboxes do not overlap with any other blob so their
-                # convexHull is not computed
-                pass
 
     def save(self, path: Path | str):
         """Saves instance of the class
 
         Parameters
         ----------
         path_to_save : str, optional
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/list_of_fragments.py` & `idtrackerai-5.1.0/src/idtrackerai/list_of_fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,27 +361,24 @@
         ----------
         list_of_global_fragments : :class:`list_of_global_fragments.ListOfGlobalFragments`
             Object collecting the global fragment objects (instances of the
             class :class:`globalfragment.GlobalFragment`) detected in the
             entire video.
 
         """
-        self.accumulable_individual_fragments = set(
+        self.accumulable_individual_fragments = {
             identifier
             for glob_frag in accumulable_global_fragments
             for identifier in glob_frag.individual_fragments_identifiers
-        )
-        self.not_accumulable_individual_fragments = (
-            set(
-                identifier
-                for glob_frag in non_accumulable_global_fragments
-                for identifier in glob_frag.individual_fragments_identifiers
-            )
-            - self.accumulable_individual_fragments
-        )
+        }
+        self.not_accumulable_individual_fragments = {
+            identifier
+            for glob_frag in non_accumulable_global_fragments
+            for identifier in glob_frag.individual_fragments_identifiers
+        } - self.accumulable_individual_fragments
 
         for fragment in self.fragments:
             if fragment.identifier in self.accumulable_individual_fragments:
                 fragment.accumulable = True
             elif fragment.identifier in self.not_accumulable_individual_fragments:
                 fragment.accumulable = False
             else:
@@ -434,19 +431,19 @@
             (not fragment.is_in_a_global_fragment and fragment.is_an_individual)
             * fragment.number_of_images
             for fragment in self.fragments
         )
 
     @property
     def fragments_not_accumulated(self) -> set[int]:
-        return self.accumulable_individual_fragments & set(
+        return self.accumulable_individual_fragments & {
             fragment.identifier
             for fragment in self.fragments
             if not fragment.used_for_training
-        )
+        }
 
     @property
     def number_of_globally_accumulated_individual_fragments(self) -> int:
         return sum(
             fragment.accumulated_globally and fragment.is_an_individual
             for fragment in self.fragments
         )
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/list_of_global_fragments.py` & `idtrackerai-5.1.0/src/idtrackerai/list_of_global_fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,17 +321,17 @@
 
     def _same_fragment_identifier(
         blobs_in_frame: list[Blob], blobs_in_frame_past: list[Blob]
     ) -> bool:
         """Return True if the set of fragments identifiers in the current frame
         is the same as in the previous frame, otherwise returns false
         """
-        same_fragment_identifier = set(
-            b.fragment_identifier for b in blobs_in_frame
-        ) == set(b.fragment_identifier for b in blobs_in_frame_past)
+        same_fragment_identifier = {b.fragment_identifier for b in blobs_in_frame} == {
+            b.fragment_identifier for b in blobs_in_frame_past
+        }
         condition_2 = (
             all(b.is_an_individual for b in blobs_in_frame_past)
             and len(blobs_in_frame_past) == num_animals
         )
         return same_fragment_identifier or not condition_2
 
     return [
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/network/evaluate.py` & `idtrackerai-5.1.0/src/idtrackerai/network/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 
 from statistics import fmean
 
 import numpy as np
 import torch
 
-from .utils.metric import Confusion
-from .utils.task import prepare_task_target
+from .utils import Confusion, prepare_task_target
 
 
 def evaluate(
     eval_loader, model, args, learner=None
 ) -> tuple[float | None, float | None, float | None, float]:
     with torch.no_grad():
         # Initialize all meters
@@ -50,15 +49,15 @@
         confusion = Confusion(args.number_of_classes)
 
     # print("---- Evaluation ----")
     if learner is not None:
         learner.eval()
     if model is not None:
         model.eval()
-    for i, (input_, target) in enumerate(eval_loader):
+    for input_, target in eval_loader:
         # mask
         mask = None
         if args.apply_mask:
             mask = torch.from_numpy(~np.eye(len(target), dtype=bool))
         # Prepare the inputs
         if args.use_gpu:
             with torch.no_grad():
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/network/modules/pairwise.py` & `idtrackerai-5.1.0/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,37 +24,40 @@
 # [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
 # de Polavieja, G.G., Nature Methods, 2019.
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
+import logging
 
+from idtrackerai import ListOfBlobs
 
-def Class2Simi(x, mode="cls", mask=None):
-    """
-    Give a 1d torch tensor with classes in dense format, returns the pairwise similarity matrix liniarized. A mask can
-    be applied to discard some elements of the similarity matrix.
 
-    :param x: 1d torch tensor with classes in dense format
-    :param mode: 'cls' for classification 'hinge' for clustering
-    :param mask: 2d torch tensor with the mask to be applied to the pairwise similarity matrix
-    :return: 1d torch tensor with the elements to be considered
-    """
-    # Convert class label to pairwise similarity
-    n = x.nelement()
-    assert (n - x.ndimension() + 1) == n, "Dimension of Label is not right"
-    expand1 = x.view(-1, 1).expand(n, n)
-    expand2 = x.view(1, -1).expand(n, n)
-    out = expand1 - expand2
-    out[out != 0] = -1  # dissimilar pair: label=-1
-    out[out == 0] = 1  # Similar pair: label=1
-    if mode == "cls":
-        out[out == -1] = 0  # dissimilar pair: label=0
-    if mode == "hinge":
-        out = out.float()  # hingeloss require float type
-    if mask is None:
-        out = out.view(-1)
-    else:
-        mask = mask.detach()
-        out = out[mask]
-    return out
+def assign_zeros_with_interpolation_identities(
+    list_of_blobs: ListOfBlobs, list_of_blobs_no_gaps: ListOfBlobs
+):
+    logging.debug("creating copy of list_of_blobs")
+
+    for blobs_in_frame, blobs_in_frame_no_gaps in zip(
+        list_of_blobs.blobs_in_video, list_of_blobs_no_gaps.blobs_in_video
+    ):
+        unassigned_blobs = [
+            blob
+            for blob in blobs_in_frame
+            if blob.is_an_individual and blob.assigned_identities[0] == 0
+        ]
+        for unassigned_blob in unassigned_blobs:
+            candidate_blobs = [
+                blob
+                for blob in blobs_in_frame_no_gaps
+                if blob.fragment_identifier == unassigned_blob.fragment_identifier
+            ]
+            if (
+                len(candidate_blobs) == 1
+                and len(candidate_blobs[0].assigned_identities) == 1
+            ):
+                unassigned_blob.identities_corrected_closing_gaps = candidate_blobs[
+                    0
+                ].assigned_identities
+
+    return list_of_blobs
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/network/train.py` & `idtrackerai-5.1.0/src/idtrackerai/network/train.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 
 from statistics import fmean
 
 import numpy as np
 import torch
 
-from idtrackerai.network.utils.metric import Confusion
-from idtrackerai.network.utils.task import prepare_task_target
+from .utils import Confusion, prepare_task_target
 
 
 def train(epoch, train_loader, learner, network_params):
     """Trains trains a network using a learner, a given train_loader and a set of network_params
 
     :param epoch: current epoch
     :param train_loader: dataloader
@@ -55,25 +54,15 @@
         losses_MCL = []
     confusion = Confusion(network_params.number_of_classes)
 
     # Setup learner's configuration
     learner.train()
 
     # The optimization loop
-
-    if network_params.print_freq > 0:  # Enable to print mini-log
-        if network_params.loss in ("CEMCL", "CEMCL_weighted"):
-            print(
-                "Itr            |Batch time     |Data Time      |Loss         |CE loss "
-                "     |MCL loss"
-            )
-        else:
-            print("Itr            |Batch time     |Data Time      |Loss")
-
-    for i, (input_, target) in enumerate(train_loader):
+    for input_, target in train_loader:
         # mask
         mask = None
         if network_params.apply_mask:
             mask = torch.from_numpy(~np.eye(len(target), dtype=bool))
         # Prepare the inputs
         if network_params.use_gpu:
             input_ = input_.cuda()
@@ -100,39 +89,15 @@
                 confusion.add(output, eval_target)
 
         # Mini-Logs
         losses += [loss] * input_.size(0)
         if network_params.loss in ("CEMCL", "CEMCL_weighted"):
             losses_CE += [output[1]] * input_.size(0)
             losses_MCL += [output[2]] * input_.size(0)
-        if network_params.print_freq > 0 and (
-            (i % network_params.print_freq == 0) or (i == len(train_loader) - 1)
-        ):
-            if "CEMCL" in network_params.loss:
-                print(  # TODO what
-                    "[{0:6d}/{1:6d}]\t"
-                    "{loss.val:.3f} ({loss.avg:.3f})"
-                    "{loss_CE.val:.3f} ({loss_CE.avg:.3f})\t"
-                    "{loss_MCL.val:.3f} ({loss_MCL.avg:.3f})\t".format(
-                        i,
-                        len(train_loader),
-                        loss=losses,
-                        loss_CE=losses_CE,
-                        loss_MCL=losses_MCL,
-                    )
-                )
-            else:
-                print(
-                    "[{0:6d}/{1:6d}]\t"
-                    "{batch_time.val:.4f} ({batch_time.avg:.4f})\t"
-                    "{data_time.val:.4f} ({data_time.avg:.4f})\t"
-                    "{loss.val:.3f} ({loss.avg:.3f})".format(
-                        i, len(train_loader), loss=losses
-                    )
-                )
+
     learner.step_schedule(epoch)
     # print loss avg
     # print(losses.avg)
     # Loss-specific information
     if network_params.loss == "CE":
         pass
         # print("[Train] ACC: ", confusion.acc())
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/postprocess/assign_them_all.py` & `idtrackerai-5.1.0/src/idtrackerai/postprocess/assign_them_all.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/postprocess/compute_velocity_model.py` & `idtrackerai-5.1.0/src/idtrackerai/postprocess/compute_velocity_model.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py` & `idtrackerai-5.1.0/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""The correct_impossible_velocity_jumps module"""
 # This file is part of idtracker.ai a multiple animals tracking system
 # described in [1].
 # Copyright (C) 2017- Francisco Romero Ferrero, Mattia G. Bergomi,
 # Francisco J.H. Heras, Robert Hinz, Gonzalo G. de Polavieja and the
 # Champalimaud Foundation.
 #
 # idtracker.ai is free software: you can redistribute it and/or modify
@@ -30,18 +31,14 @@
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 
 import numpy as np
 
 from idtrackerai import Fragment, ListOfFragments, Video
 from idtrackerai.utils import track
 
-"""
-The correct_impossible_velocity_jumps module
-"""
-
 
 def get_candidate_identities_by_minimum_speed(
     fragment: Fragment,
     fragments: list[Fragment],
     available_identities: set,
     impossible_velocity_threshold: float,
 ) -> tuple[np.ndarray, np.ndarray]:
@@ -197,28 +194,24 @@
     :class:`fragment.Fragment`
     :meth:`get_available_and_non_available_identities`
     :meth:`get_candidate_identities_by_minimum_speed`
     :meth:`get_candidate_identities_above_random_P2`
 
     """
 
-    non_available_identities = set(
+    non_available_identities = {
         coexisting_fragment.assigned_identities[0]
         for coexisting_fragment in fragment.coexisting_individual_fragments
-    )
+    }
     available_identities = (
         set(range(1, fragment.number_of_animals + 1)) - non_available_identities
     )
-    if (
-        fragment.assigned_identities[0] is not None
-        and fragment.assigned_identities[0] != 0
-    ):
-        available_identities = available_identities | set(
-            [fragment.assigned_identities[0]]
-        )
+    if fragment.assigned_identities[0] not in (None, 0):
+        available_identities.add(fragment.assigned_identities[0])
+
     if 0 in non_available_identities:
         non_available_identities.remove(0)
     non_available_identities = np.asarray(list(non_available_identities))
 
     if len(available_identities) == 1:
         candidate_id = available_identities.pop()
     else:
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/postprocess/erosion.py` & `idtrackerai-5.1.0/src/idtrackerai/postprocess/erosion.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/postprocess/get_trajectories.py` & `idtrackerai-5.1.0/src/idtrackerai/postprocess/get_trajectories.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,19 +112,19 @@
         track(blobs_in_video, "Creating trajectories")
     ):
         if abort():
             return None
         if progress_bar:
             progress_bar.emit(frame_number)
         try:
-            identifiers_next = set(
+            identifiers_next = {
                 b.fragment_identifier for b in blobs_in_video[frame_number + 1]
-            )
+            }
         except IndexError:  # last frame
-            identifiers_next = set(b.fragment_identifier for b in blobs_in_frame)
+            identifiers_next = {b.fragment_identifier for b in blobs_in_frame}
 
         for blob in blobs_in_frame:
             if blob.is_an_individual:
                 if blob.fragment_identifier in identifiers_prev:
                     column = np.argwhere(identifiers_prev == blob.fragment_identifier)[
                         0
                     ][0]
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/postprocess/trajectories_creation.py` & `idtrackerai-5.1.0/src/idtrackerai/postprocess/trajectories_creation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/postprocess/trajectories_to_csv.py` & `idtrackerai-5.1.0/src/idtrackerai/postprocess/trajectories_to_csv.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/tracker/accumulation_manager.py` & `idtrackerai-5.1.0/src/idtrackerai/tracker/accumulation_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,31 +27,26 @@
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import logging
 import random
 from pathlib import Path
-from typing import Any
 
 import numpy as np
 
 from idtrackerai import Fragment, GlobalFragment, ListOfFragments, ListOfGlobalFragments
 from idtrackerai.utils import conf, load_id_images
 
 from .accumulation_manager_utils import (
     get_P1_array_and_argsort,
     p1_below_random,
     set_fragment_temporary_id,
 )
-from .assigner import assign
-
-"""
-The accumulation manager module
-"""
+from .network.get_predictions import get_predictions_identities
 
 
 class AccumulationManager:
     """Manages the process of accumulating images for training the network.
 
     Attributes
     ----------
@@ -305,20 +300,20 @@
         Returns
         -------
         individual_fragments_used_for_training : list
             List of Fragment objects.
 
         """
         return list(
-            set(
+            {
                 fragment.identifier
                 for fragment in self.list_of_fragments.fragments
                 if fragment.used_for_training
                 and fragment.identifier not in self.individual_fragments_used
-            )
+            }
         )
 
     def update_list_of_individual_fragments_used(self):
         """Updates the list of individual fragments used for training and
         their identities.
         If an individual fragment was added before is not added again.
         """
@@ -441,17 +436,15 @@
             and self.ratio_accumulated_images
             > min_number_of_imgs_accumulated_to_start_partial_accumulation
             and self.ratio_accumulated_images < self.threshold_early_stop_accumulation
         ):
             logging.debug("Accumulating by partial strategy")
             self.accumulation_strategy = "partial"
             self.reset_accumulation_variables()
-            for i, global_fragment in enumerate(
-                self.list_of_global_fragments.global_fragments
-            ):
+            for global_fragment in self.list_of_global_fragments.global_fragments:
                 if not global_fragment.used_for_training:
                     self.check_if_is_acceptable_for_training(global_fragment)
         elif (
             self.ratio_accumulated_images
             < min_number_of_imgs_accumulated_to_start_partial_accumulation
         ):
             logging.info(
@@ -782,16 +775,19 @@
         if fragment.is_an_individual and not fragment.used_for_training:
             images.extend(list(zip(fragment.images, fragment.episodes)))
             lengths.append(fragment.number_of_images)
             candidate_individual_fragments_identifiers.append(fragment.identifier)
 
     assert images
     images = load_id_images(id_images_file_paths, images)
-    assigner = assign(identification_model, images, network_params)
 
-    assert sum(lengths) == len(assigner._predictions)
+    predictions, softmax_probs = get_predictions_identities(
+        identification_model, images, network_params
+    )
+
+    assert sum(lengths) == len(predictions)
     return (
-        assigner._predictions,
-        assigner._softmax_probs,
+        predictions,
+        softmax_probs,
         np.cumsum(lengths)[:-1],
         candidate_individual_fragments_identifiers,
     )
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/tracker/accumulation_manager_utils.py` & `idtrackerai-5.1.0/src/idtrackerai/tracker/accumulation_manager_utils.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/tracker/accumulator.py` & `idtrackerai-5.1.0/src/idtrackerai/tracker/accumulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,31 +26,29 @@
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import logging
 
-import numpy as np
 import torch
 from torch import nn
 from torch.backends import cudnn
 from torch.optim.lr_scheduler import MultiStepLR
 
 from idtrackerai import Video
-from idtrackerai.network.learners import LearnerClassification
+from idtrackerai.network import LearnerClassification, NetworkParams
 from idtrackerai.utils import conf
 
 from .accumulation_manager import (
     AccumulationManager,
     get_predictions_of_candidates_fragments,
 )
 from .dataset.identification_dataloader import get_training_data_loaders
 from .dataset.identification_dataset import split_data_train_and_validation
-from .network.network_params import NetworkParams
 from .network.stop_training_criteria import StopTraining
 from .network.trainer import TrainIdentification
 
 
 def perform_one_accumulation_step(
     accumulation_manager: AccumulationManager,
     video: Video,
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/tracker/dataset/identification_dataloader.py` & `idtrackerai-5.1.0/src/idtrackerai/tracker/dataset/identification_dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 import logging
 import os
 
 from torch.utils.data import DataLoader
 from torchvision import transforms
 
-from idtrackerai.network.utils.utils import Normalize
+from idtrackerai.network import Normalize
 from idtrackerai.utils import conf
 
 from .identification_dataset import IdentificationDataset
 
 if os.name == "nt":  # windows
     # Using multipricessing in Windows causes a
     # recursion limit error difficut to debug
@@ -82,15 +82,15 @@
     )
     val_loader.num_classes = number_of_animals
     val_loader.image_shape = validation_set[0][0].shape
     return train_loader, val_loader
 
 
 def get_test_data_loader(test_data, number_of_classes):
-    logging.info("Creating test IdentificationDataset")
+    logging.debug("Creating test IdentificationDataset")
     test_set = IdentificationDataset(
         test_data,
         scope="predict",
         transform=transforms.Compose([transforms.ToTensor(), Normalize()]),
     )
     test_loader = DataLoader(
         test_set,
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/tracker/dataset/identification_dataset.py` & `idtrackerai-5.1.0/src/idtrackerai/tracker/dataset/identification_dataset.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/tracker/identity_transfer.py` & `idtrackerai-5.1.0/src/idtrackerai/tracker/identity_transfer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import logging
 
 import numpy as np
 from torch.nn import Module
 
 from idtrackerai import GlobalFragment, Video
-from idtrackerai.network.utils.utils import fc_weights_reinit
-from idtrackerai.tracker.accumulation_manager_utils import (
+from idtrackerai.network import NetworkParams, fc_weights_reinit
+from idtrackerai.utils import conf
+
+from .accumulation_manager_utils import (
     get_P1_array_and_argsort,
     p1_below_random,
     set_fragment_temporary_id,
 )
-from idtrackerai.tracker.assigner import (
-    assign,
-    compute_identification_statistics_for_non_accumulated_fragments,
-)
-from idtrackerai.tracker.network.network_params import NetworkParams
-from idtrackerai.utils import conf
+from .assigner import compute_identification_statistics_for_non_accumulated_fragments
+from .network.get_predictions import get_predictions_identities
 
 
 def identify_first_global_fragment_for_accumulation(
     first_global_fragment_for_accumulation: GlobalFragment,
     video: Video,
     identification_model: Module,
     network_params: NetworkParams,
@@ -77,19 +75,22 @@
     network_params: NetworkParams,
     knowledge_transfer_info_dict: dict,
 ) -> list | None:
     (images, _) = first_global_fragment_for_accumulation.get_images_and_labels(
         video.id_images_file_paths
     )
 
-    assigner = assign(identification_model, images, network_params)
+    predictions, softmax_probs = get_predictions_identities(
+        identification_model, images, network_params
+    )
 
     compute_identification_statistics_for_non_accumulated_fragments(
         first_global_fragment_for_accumulation.individual_fragments,
-        assigner,
+        predictions,
+        softmax_probs,
         network_params.number_of_classes,
     )
 
     # Check certainties of the individual fragments in the global fragment
     # for individual_fragment_identifier in global_fragment.individual_fragments_identifiers:
 
     for fragment in first_global_fragment_for_accumulation.individual_fragments:
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/tracker/network/stop_training_criteria.py` & `idtrackerai-5.1.0/src/idtrackerai/tracker/network/stop_training_criteria.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/tracker/network/trainer.py` & `idtrackerai-5.1.0/src/idtrackerai/tracker/network/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,26 +25,24 @@
 # de Polavieja, G.G., Nature Methods, 2019.
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import logging
+from contextlib import suppress
 from pathlib import Path
 
 import numpy as np
 from rich.console import Console
 from torch.utils.data import DataLoader
 
-from idtrackerai.network.evaluate import evaluate
-from idtrackerai.network.learners import LearnerClassification
-from idtrackerai.network.train import train
+from idtrackerai.network import LearnerClassification, NetworkParams, evaluate, train
+from idtrackerai.tracker.accumulation_manager import AccumulationManager
 
-from ..accumulation_manager import AccumulationManager
-from .network_params import NetworkParams
 from .stop_training_criteria import StopTraining
 
 
 def TrainIdentification(
     learner: LearnerClassification,
     train_loader: DataLoader,
     val_loader: DataLoader,
@@ -94,24 +92,22 @@
                 )
                 val_losses.append(loss)
                 if network_params.loss in ("CEMCL", "CEMCL_weighted"):
                     val_losses_CE.append(loss_CE)
                     val_losses_MCL.append(loss_MCL)
                 val_accs.append(val_acc)
             # Save checkpoint at each LR steps and the end of optimization
-            ## TODO: Consider saving only best model
+            # TODO: Consider saving only best model
             best_model_path = learner.snapshot(network_params.save_model_path)
-            try:
+            with suppress(IndexError):
                 status.update(
                     f"[red]Epochs loop {epoch}: training loss = {train_losses[-1]:.6f},"
                     f" validation loss = {val_losses[-1]:.6f} and accuracy ="
                     f" {val_accs[-1]:.4%}"
                 )
-            except IndexError:
-                pass
 
         logging.info("Last epoch loop: %s", status.status, extra={"markup": True})
 
     if np.isnan(train_losses[-1]) or np.isnan(val_losses[-1]):
         logging.warning(
             "The model diverged. Falling back to individual-crossing "
             "discrimination by average area model."
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/tracker/pre_trainer.py` & `idtrackerai-5.1.0/src/idtrackerai/tracker/pre_trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,21 +32,19 @@
 
 import torch
 from torch import nn
 from torch.backends import cudnn
 from torch.optim.lr_scheduler import MultiStepLR
 
 from idtrackerai import GlobalFragment, ListOfFragments
-from idtrackerai.network.learners import LearnerClassification
-from idtrackerai.network.utils.utils import fc_weights_reinit
+from idtrackerai.network import LearnerClassification, NetworkParams, fc_weights_reinit
 from idtrackerai.utils import conf
 
 from .dataset.identification_dataloader import get_training_data_loaders
 from .dataset.identification_dataset import split_data_train_and_validation
-from .network.network_params import NetworkParams
 from .network.stop_training_criteria import StopTraining
 from .network.trainer import TrainIdentification
 
 
 def pre_train_global_fragment(
     number_of_animals: int,
     accumulation_step: int,
@@ -78,21 +76,14 @@
     save_summaries : bool
         if True tensorflow summaries will be generated and stored to allow
         tensorboard visualisation of both loss and activity histograms
     store_training_accuracy_and_loss_data : <Store_Accuracy_and_Loss object>
         an instance of the class :class:`~Store_Accuracy_and_Loss`
     store_validation_accuracy_and_loss_data : <Store_Accuracy_and_Loss object>
         an instance of the class :class:`~Store_Accuracy_and_Loss`
-    print_flag : bool
-        if True additional information are printed in the terminal
-    plot_flag : bool
-        if True training and validation loss, accuracy and individual accuracy
-        are plot in a graph at the end of the training session
-    batch_size : int
-        size of the batch of images used for training
 
     Returns
     -------
     <ConvNetwork object>
         network with updated parameters after training
     float
         ration of images used for pretraining over the total number of
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/tracker/tracker.py` & `idtrackerai-5.1.0/src/idtrackerai/tracker/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,26 @@
 import logging
 
 import numpy as np
 import torch
 from torch.backends import cudnn
 
 from idtrackerai import ListOfBlobs, ListOfFragments, ListOfGlobalFragments, Video
-from idtrackerai.network.learners.learners import LearnerClassification
-from idtrackerai.network.utils.utils import fc_weights_reinit, weights_xavier_init
+from idtrackerai.network import (
+    LearnerClassification,
+    NetworkParams,
+    fc_weights_reinit,
+    weights_xavier_init,
+)
 from idtrackerai.utils import CustomError, conf, create_dir, json_object_hook
 
 from .accumulation_manager import AccumulationManager
 from .accumulator import perform_one_accumulation_step
 from .assigner import assign_remaining_fragments
 from .identity_transfer import identify_first_global_fragment_for_accumulation
-from .network.network_params import NetworkParams
 from .pre_trainer import pre_train_global_fragment
 
 
 class TrackerAPI:
     def __init__(
         self,
         video: Video,
@@ -62,16 +65,16 @@
         self.list_of_global_fragments = list_of_global_fragments
 
         if self.video.knowledge_transfer_folder is not None:
             kt_info_dict_path = (
                 self.video.knowledge_transfer_folder / "model_params.json"
             )
             try:
-                self.knowledge_transfer_info_dict: dict = json.loads(
-                    kt_info_dict_path.read_text(), object_hook=json_object_hook
+                self.knowledge_transfer_info_dict: dict = json.load(
+                    kt_info_dict_path.open(), object_hook=json_object_hook
                 )
             except FileNotFoundError:
                 # Transferring from v4
                 self.knowledge_transfer_info_dict: dict = np.load(
                     kt_info_dict_path.with_suffix(".npy"), allow_pickle=True
                 ).item()
         else:
@@ -148,44 +151,44 @@
         #     self.postprocess_impossible_jumps()
         #     raise NotImplementedError("New tracking methods are not allwoed")
 
     def _track_with_protocols_cascade(self):
         logging.info("******* Start tracking with protocol cascade ********")
         # Restoring
 
-        delete = not self.processes_to_restore.get("protocols1_and_2", False)
+        delete = not self.processes_to_restore.get("protocols1_and_2")
         # Create accumulation folder
         self.video.create_accumulation_folder(iteration_number=0, delete=delete)
 
         self.init_accumulation_idCNN_params()
 
         # Restoring
         self.restoring_first_accumulation = False
-        if self.processes_to_restore.get("post_processing", False):
-            raise NotImplementedError()
+        if self.processes_to_restore.get("post_processing"):
+            raise NotImplementedError
             # self.restore_trajectories()
             # self.restore_crossings_solved()
             # self.restore_trajectories_wo_gaps()
 
-        if self.processes_to_restore.get("residual_identification", False):
-            raise NotImplementedError()
+        if self.processes_to_restore.get("residual_identification"):
+            raise NotImplementedError
             # if self.video.track_wo_identities:
             # TODO: bring restoring back to life
             # raise
             # self.restore_trajectories()
 
             # else:
             # TODO: bring restoring back to life
             # raise
             # logging.info("Restoring residual identification")
             # self.restore_identification()
             # self.create_trajectories()
 
-        if self.processes_to_restore.get("protocol3_accumulation", False):
-            raise NotImplementedError()
+        if self.processes_to_restore.get("protocol3_accumulation"):
+            raise NotImplementedError
             # logging.info("Restoring second accumulation")
             # # self.restore_second_accumulation()
             # self.video._first_frame_first_global_fragment = (
             #     self.video._first_frame_first_global_fragment
             # )
             # logging.warning(
             #     "first_frame_first_global_fragment "
@@ -193,17 +196,17 @@
             #         self.video.first_frame_first_global_fragment
             #     )
             # )
             # logging.info("Starting identification")
             #
             # self.create_trajectories()
 
-        if self.processes_to_restore.get("protocol3_pretraining", False):
+        if self.processes_to_restore.get("protocol3_pretraining"):
             # TODO: bring restoring back to life
-            raise NotImplementedError()
+            raise NotImplementedError
             # logging.info("Restoring pretraining")
             # logging.info("Initialising pretraining network")
             # self.init_pretraining_net()
             # logging.info("Restoring pretraining")
             # self.accumulation_step_finished = True
             # self.restore_first_accumulation()
             # self.restore_pretraining()
@@ -217,17 +220,17 @@
             # self.video._percentage_of_accumulated_images = [
             #     self.video.percentage_of_accumulated_images[0]
             # ]
             # logging.info("Start accumulation parachute")
             #
             # self.accumulate()
 
-        if self.processes_to_restore.get("protocols1_and_2", False):
+        if self.processes_to_restore.get("protocols1_and_2"):
             # TODO: bring restoring back to life
-            raise NotImplementedError()
+            raise NotImplementedError
             # logging.info("Restoring protocol 1 and 2")
             # self.restoring_first_accumulation = True
             # # self.restore_first_accumulation()
             # self.accumulation_manager.ratio_accumulated_images =
             # self.video.percentage_of_accumulated_images[0]
             # self.video._first_frame_first_global_fragment = [
             #     self.video._first_frame_first_global_fragment[
@@ -237,42 +240,37 @@
             # self.video._percentage_of_accumulated_images = [
             #     self.video.percentage_of_accumulated_images[0]
             # ]
             # self.accumulation_step_finished = True
             #
             # self.accumulate()
 
-        if not self.processes_to_restore.get("protocols1_and_2", False):
+        if not self.processes_to_restore.get("protocols1_and_2"):
             logging.info("Starting protocol cascade")
             self.protocol1()
 
     def init_accumulation_idCNN_params(self):
         self.accumulation_network_params = NetworkParams(
             number_of_classes=self.video.number_of_animals,
             architecture=conf.IDCNN_NETWORK_NAME,
             save_folder=self.video.accumulation_folder,
-            knowledge_transfer_model_file=self.video.knowledge_transfer_folder,
-            saveid="",
+            knowledge_transfer_folder=self.video.knowledge_transfer_folder,
             model_name="identification_network",
             image_size=self.video.id_image_size,
             scopes_layers_to_optimize=conf.LAYERS_TO_OPTIMISE_PRETRAINING,
             loss="CE",
-            print_freq=-1,
             use_gpu=True,
             optimizer="SGD",
             schedule=[30, 60],
-            optim_args={"lr": conf.LEARNING_RATE_IDCNN_ACCUMULATION},
+            optim_args={"lr": conf.LEARNING_RATE_IDCNN_ACCUMULATION, "momentum": 0.9},
             apply_mask=False,
             dataset="supervised",
             skip_eval=False,
             epochs=conf.MAXIMUM_NUMBER_OF_EPOCHS_IDCNN,
-            plot_flag=False,
             return_store_objects=False,
-            layers_to_optimize=conf.LAYERS_TO_OPTIMISE_ACCUMULATION,
-            video_paths=self.video.video_paths,
         )
         # Save network params
         self.accumulation_network_params.save()
 
     def protocol1(self):
         self.video.protocol1_timer.start()
 
@@ -512,66 +510,60 @@
         )
 
         if self.video.knowledge_transfer_folder:
             logging.info(
                 "Performing knowledge transfer from %s"
                 % self.video.knowledge_transfer_folder
             )
-            self.pretrain_network_params.knowledge_transfer_model_file = (
+            self.pretrain_network_params.knowledge_transfer_folder = (
                 self.video.knowledge_transfer_folder
             )
 
         logging.info("Start pretraining")
         self.pretraining_step_finished = True
         self.pretraining_loop()
 
     def init_pretraining_variables(self):
         self.init_pretraining_net()
         self.ratio_of_pretrained_images = 0
 
         # Initialize network
         self.learner_class = LearnerClassification
-        logging.info("Creating model")
         if self.video.knowledge_transfer_folder:
             self.identification_model = self.learner_class.load_model(
                 self.pretrain_network_params, scope="knowledge_transfer"
             )
             self.identification_model.apply(fc_weights_reinit)
         else:
             self.identification_model = self.learner_class.create_model(
                 self.pretrain_network_params
             )
             self.identification_model.apply(weights_xavier_init)
 
     def init_pretraining_net(self):
-        delete = not self.processes_to_restore.get("protocol3_pretraining", False)
+        delete = not self.processes_to_restore.get("protocol3_pretraining")
         create_dir(self.video.pretraining_folder, remove_existing=delete)
 
         self.pretrain_network_params = NetworkParams(
             number_of_classes=self.video.number_of_animals,
             architecture=conf.IDCNN_NETWORK_NAME,
             save_folder=self.video.pretraining_folder,
-            saveid="",
             model_name="identification_network",
             image_size=self.video.id_image_size,
             scopes_layers_to_optimize=conf.LAYERS_TO_OPTIMISE_PRETRAINING,
             loss="CE",
-            print_freq=-1,
             use_gpu=True,
             optimizer="SGD",
             schedule=[30, 60],
-            optim_args={"lr": conf.LEARNING_RATE_IDCNN_ACCUMULATION},
+            optim_args={"lr": conf.LEARNING_RATE_IDCNN_ACCUMULATION, "momentum": 0.9},
             apply_mask=False,
             dataset="supervised",
             skip_eval=False,
             epochs=conf.MAXIMUM_NUMBER_OF_EPOCHS_IDCNN,
-            plot_flag=False,
             return_store_objects=False,
-            layers_to_optimize=conf.LAYERS_TO_OPTIMISE_ACCUMULATION,
-            video_paths=self.video.video_paths,
         )
 
     def pretraining_loop(self):
         self.list_of_fragments.reset(roll_back_to="fragmentation")
         self.list_of_global_fragments.order_by_distance_travelled()
         self.one_shot_pretraining()
         self.continue_pretraining()
@@ -616,15 +608,15 @@
 
     """ parachute """
 
     def accumulation_parachute_init(self, iteration_number):
         logging.debug("------------------------> accumulation_parachute_init")
         logging.info("Starting accumulation %i" % iteration_number)
 
-        delete = not self.processes_to_restore.get("protocol3_accumulation", False)
+        delete = not self.processes_to_restore.get("protocol3_accumulation")
 
         self.video.create_accumulation_folder(
             iteration_number=iteration_number, delete=delete
         )
         self.video.accumulation_trial = iteration_number
         self.list_of_fragments.reset(roll_back_to="fragmentation")
         self.list_of_global_fragments.reset(roll_back_to="fragmentation")
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/utils/__init__.py` & `idtrackerai-5.1.0/src/idtrackerai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/utils/check_PyPI_version.py` & `idtrackerai-5.1.0/src/idtrackerai/utils/check_PyPI_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,25 +46,25 @@
         filter(lambda line: "yanked" not in line, out_text.splitlines())
     )
     versions: list[tuple[str, str]] = re.findall(
         ">idtrackerai-(.+?)(.tar.gz|-py3-none-any.whl)<", no_yanked_versions
     )
 
     current_version = idtrackerai.__version__
-    for version, file_extension in versions:
+    for version, _file_extension in versions:
         if not version.replace(".", "").isdigit():
             continue  # not a stable version
 
         if available_is_greater(version, current_version):
             return (
                 True,
                 (
                     f"A new release of idtracker.ai available: {current_version} ->"
                     f"{version}\n"
-                    "To update, run: python3 -m pip install --upgrade idtrackerai"
+                    "To update, run: python -m pip install --upgrade idtrackerai"
                 ),
             )
 
     return (
         False,
         (
             "There are currently no updates available.\n"
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/utils/confparams.py` & `idtrackerai-5.1.0/src/idtrackerai/utils/confparams.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/utils/init_logger.py` & `idtrackerai-5.1.0/src/idtrackerai/utils/init_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,46 +6,46 @@
 
 from rich.console import Console
 from rich.logging import RichHandler
 
 from .check_PyPI_version import check_version_on_console_thread
 
 
-def initLogger(testing=False, check_version=True):
+def initLogger(testing=False, check_version=True, level: int = logging.DEBUG):
     logger_width_when_no_terminal = 150
     try:
         os.get_terminal_size()
     except OSError:
         # stdout is sent to file. We define logger width to a constant
         size = logger_width_when_no_terminal
     else:
         # stdout is sent to terminal
         # We define logger width to adapt to the terminal width
         size = None
 
     # The first handler is the terminal, the second one the .log file,
     # both rendered with Rich and full logging (level=0)
     logging.basicConfig(
-        level=logging.DEBUG,
+        level=level,
         format="%(message)s",
         datefmt="%H:%M:%S",
         force=not testing,
         handlers=[
             RichHandler(console=Console(width=size)),
             RichHandler(
                 console=Console(
-                    file=open("idtrackerai.log", "w", encoding="utf_8"),
+                    file=open("idtrackerai.log", "w", encoding="utf_8"),  # noqa SIM115
                     width=logger_width_when_no_terminal,
                 )
             ),
         ],
     )
 
     logging.getLogger("PyQt6").setLevel(logging.INFO)
-    logging.info("Welcome to idtracker.ai")
+    logging.info("Welcome to idtracker.ai %s", metadata.version("idtrackerai"))
     logging.debug(
-        f"Running idTracker.ai '{metadata.version('idtrackerai')}'"
+        f"Running idtracker.ai '{metadata.version('idtrackerai')}'"
         f" on Python '{sys.version.split(' ')[0]}'\nPlatform: '{platform(True)}'"
     )
 
     if check_version:
         check_version_on_console_thread()
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/utils/py_utils.py` & `idtrackerai-5.1.0/src/idtrackerai/utils/py_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import json
 import logging
 from dataclasses import dataclass
 from pathlib import Path
 from shutil import rmtree
 from time import perf_counter
-from typing import Iterable, Optional, Sequence, TypeVar
+from typing import Iterable, Optional, TypeVar
 
 import cv2
 import h5py
 import numpy as np
 from rich.progress import BarColumn, Progress, TaskProgressColumn, TimeRemainingColumn
 
 InputType = TypeVar("InputType")
@@ -73,14 +73,16 @@
         if remove_existing:
             rmtree(path)
             path.mkdir()
             logging.info(f"Directory {path} has been cleaned")
         else:
             logging.info(f"Directory {path} already exists")
     else:
+        if not path.parent.is_dir():
+            path.parent.mkdir()
         path.mkdir()
         logging.info(f"Directory {path} has been created")
 
 
 def remove_dir(path: Path):
     if path.is_dir():
         rmtree(path, ignore_errors=True)
@@ -117,28 +119,28 @@
         raise TypeError(label)
 
     if close:
         return np.vstack([vertices, vertices[0]]).astype(np.int32)
     return vertices.astype(np.int32)
 
 
-def build_ROI_mask_from_list(width, height, list_of_ROIs: None | list[str] | str):
+def build_ROI_mask_from_list(
+    list_of_ROIs: None | list[str] | str, width, height
+) -> np.ndarray | None:
     """Transforms a list of polygons (as type str) from
     ROI widget (idtrackerai_app) into a boolean np.array mask"""
-    if not list_of_ROIs:
-        return np.ones((height, width), bool)
+
+    if list_of_ROIs is None:
+        return None
+
+    ROI_mask = np.zeros((height, width), np.uint8)
 
     if isinstance(list_of_ROIs, str):
         list_of_ROIs = list(list_of_ROIs)
 
-    if list_of_ROIs[0][0] == "+":
-        ROI_mask = np.zeros((height, width), np.uint8)
-    else:
-        ROI_mask = np.ones((height, width), np.uint8)
-
     for line in list_of_ROIs:
         vertices = get_vertices_from_label(line)
         if line[0] == "+":
             cv2.fillPoly(ROI_mask, [vertices][::-1], color=1)
         elif line[0] == "-":
             cv2.fillPoly(ROI_mask, [vertices][::-1], color=0)
         else:
@@ -226,15 +228,15 @@
             "To perform identity transfer you "
             "need to provide a path for the variable "
             "'KNOWLEDGE_TRANSFER_FOLDER'"
         )
 
     kt_info_dict_path = knowledge_transfer_folder / "model_params.json"
     if kt_info_dict_path.is_file():
-        knowledge_transfer_info_dict = json.loads(kt_info_dict_path.read_text())
+        knowledge_transfer_info_dict = json.load(kt_info_dict_path.open())
         assert "image_size" in knowledge_transfer_info_dict
 
     elif kt_info_dict_path.with_suffix(".npy").is_file():
         knowledge_transfer_info_dict: dict = np.load(
             kt_info_dict_path.with_suffix(".npy"), allow_pickle=True
         ).item()  # loading from v4
         assert "image_size" in knowledge_transfer_info_dict
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai/video.py` & `idtrackerai-5.1.0/src/idtrackerai/video.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import json
 import logging
+import sys
 from copy import copy
 from importlib import metadata
 from math import sqrt
 from pathlib import Path
 from typing import Iterable
 
 import cv2
@@ -206,15 +207,15 @@
             ).resolve()
         create_dir(self.session_folder)
         create_dir(self.preprocessing_folder)
 
         self.ROI_list = roi_list
 
         self.ROI_mask = build_ROI_mask_from_list(
-            self.original_width, self.original_height, list_of_ROIs=roi_list
+            roi_list, self.original_width, self.original_height
         )
 
         if conf.IDENTIFICATION_IMAGE_SIZE > 0:
             self.id_image_size = [
                 conf.IDENTIFICATION_IMAGE_SIZE,
                 conf.IDENTIFICATION_IMAGE_SIZE,
                 1,
@@ -276,14 +277,17 @@
         self.identify_timer = Timer("Identification")
         self.impossible_jumps_timer = Timer("Impossible jumps correction")
         self.crossing_solver_timer = Timer("Crossings solver")
         self.create_trajectories_timer = Timer("Trajectories creation")
 
         self.general_timer.start()
 
+    def __str__(self) -> str:
+        return f"<session {self.session_folder}>"
+
     def set_id_image_size(self, median_body_length: int | float, reset=False):
         self.median_body_length = median_body_length
         if reset or not self.id_image_size:
             side_length = int(median_body_length / sqrt(2))
             side_length += side_length % 2
             self.id_image_size = [side_length, side_length, 1]
         logging.info(f"Identification image size set to {self.id_image_size}")
@@ -324,15 +328,15 @@
 
     @ROI_mask.setter
     def ROI_mask(self, mask: np.ndarray | None):
         if mask is None:
             del self.ROI_mask
         else:
             cv2.imwrite(str(self.ROI_mask_path), (mask * 255).astype(np.uint8))
-            logging.info(f"Background saved at {self.background_path}")
+            logging.info(f"ROI mask saved at {self.ROI_mask_path}")
 
     @ROI_mask.deleter
     def ROI_mask(self):
         self.ROI_mask_path.unlink(missing_ok=True)
 
     def set_video_paths(self, video_paths: list[Path | str]):
         if not isinstance(video_paths, list):
@@ -460,14 +464,18 @@
         return self.preprocessing_folder / "list_of_blobs_no_gaps.pickle"
 
     @property
     def blobs_path_validated(self) -> Path:
         return self.preprocessing_folder / "list_of_blobs_validated.pickle"
 
     @property
+    def idmatcher_results_path(self) -> Path:
+        return self.session_folder / "matching_results"
+
+    @property
     def global_fragments_path(self) -> Path:
         """get the path to save the list of global fragments after
         fragmentation"""
         return self.preprocessing_folder / "list_of_global_fragments.pickle"
 
     @property
     def fragments_path(self) -> Path:
@@ -536,24 +544,33 @@
                 "Could not load video episodes probably due to loading an old version"
                 " session"
             )
         return video
 
     @classmethod
     def open_from_v4(cls, path: Path) -> dict:
+        from . import network
+
         logging.warning("Loading from v4: %s", path)
+
+        # v4 compatibility
+        sys.modules["idtrackerai.tracker.network.network_params"] = network
         _dict: dict = np.load(path, allow_pickle=True).item().__dict__
+        del sys.modules["idtrackerai.tracker.network.network_params"]
+
+        _dict["version"] = "4.0.12 or below"
         _dict["video_paths"] = list(map(Path, _dict.pop("_video_paths")))
         _dict["session_folder"] = path.parent
         _dict["median_body_length"] = _dict.pop("_median_body_length")
         _dict["frames_per_second"] = _dict.pop("_frames_per_second")
         _dict["original_width"] = _dict.pop("_original_width")
         _dict["original_height"] = _dict.pop("_original_height")
         _dict["number_of_frames"] = _dict.pop("_number_of_frames")
         _dict["identities_groups"] = _dict.pop("_identities_groups")
+        _dict["id_image_size"] = list(_dict.pop("_identification_image_size"))
         _dict["setup_points"] = _dict.pop("_setup_points")
         _dict["number_of_animals"] = _dict["_user_defined_parameters"][
             "number_of_animals"
         ]
         _dict["tracking_intervals"] = _dict["_user_defined_parameters"][
             "tracking_interval"
         ]
@@ -562,14 +579,18 @@
         ]
         _dict["track_wo_identities"] = _dict["_user_defined_parameters"][
             "track_wo_identification"
         ]
         _dict["identities_labels"] = list(
             map(str, range(1, _dict["number_of_animals"] + 1))
         )
+        _dict["accumulation_folder"] = (
+            path.parent / Path(_dict.pop("_accumulation_folder")).name
+        )
+        _dict["_user_defined_parameters"].pop("mask")
         return _dict
 
     def update_paths(
         self, new_video_object_path: Path, user_video_paths_dir: Path | None = None
     ):
         """Update paths of objects (e.g. blobs_path, preprocessing_folder...)
         according to the new location of the new video object given
@@ -579,24 +600,22 @@
         ----------
         new_video_object_path : str
             Path to a video_object.npy
         """
         logging.info(
             f"Searching video files: {[str(path.name) for path in self.video_paths]}"
         )
-        folder_candidates: set[Path | None] = set(
-            (
-                user_video_paths_dir,
-                self.video_paths[0],
-                new_video_object_path,
-                new_video_object_path.parent,
-                self.session_folder.parent,
-                self.session_folder,
-            )
-        )
+        folder_candidates: set[Path | None] = {
+            user_video_paths_dir,
+            self.video_paths[0],
+            new_video_object_path,
+            new_video_object_path.parent,
+            self.session_folder.parent,
+            self.session_folder,
+        }
 
         for folder_candidate in folder_candidates:
             if folder_candidate is None:
                 continue
             if folder_candidate.is_file():
                 folder_candidate = folder_candidate.parent
 
@@ -760,15 +779,15 @@
         tracking_intervals_changes = list(np.asarray(tracking_intervals).flatten())
 
         # Take into account tracking interval changes
         # and video path changes to compute episodes
         limits = video_paths_changes + tracking_intervals_changes
 
         # clean repeated limits and sort them
-        limits = sorted(list(set(limits)))
+        limits = sorted(set(limits))
 
         # Create "long episodes" as the intervals between any video path
         # change or tracking interval change (keeping only the ones that
         # are inside a tracking interval)
         long_episodes = []
         for start, end in zip(limits[:-1], limits[1:]):
             if (
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai.egg-info/PKG-INFO` & `idtrackerai-5.1.0/src/idtrackerai.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 Metadata-Version: 2.1
 Name: idtrackerai
-Version: 5.0.0a5
+Version: 5.1.0
 Summary: A multi-animal tracking algorithm based on convolutional neural networks
-Author: Jordi Torrents, Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
-Project-URL: Homepage, https://idtrackerai.readthedocs.io/en/latest/
+Author: Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
+Author-email: Jordi Torrents <jordi.torrentsm@gmail.com>
+Project-URL: Homepage, https://idtracker.ai/
 Project-URL: Repository, https://gitlab.com/polavieja_lab/idtrackerai
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
+Classifier: Environment :: X11 Applications :: Qt
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
-[![image](http://img.shields.io/pypi/v/idtrackerai.svg)](https://pypi.python.org/pypi/idtrackerai/)
-![pipeline](https://gitlab.com/polavieja_lab/idtrackerai/badges/v5-dev/pipeline.svg)
-[![Supported Python versions](https://img.shields.io/pypi/pyversions/idtrackerai.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/idtrackerai/)
-![pylint](https://gitlab.com/polavieja_lab/idtrackerai/-/jobs/artifacts/v5-dev/raw/pylint/pylint.svg?job=test)
-[![PyPI downloads](https://img.shields.io/pypi/dm/idtrackerai.svg)](https://pypistats.org/packages/idtrackerai)
-![Licence](https://img.shields.io/gitlab/license/polavieja_lab/idtrackerai.svg)
+[![image](http://img.shields.io/pypi/v/idtrackerai.svg)](https://pypi.python.org/pypi/idtrackerai/) ![pipeline](https://gitlab.com/polavieja_lab/idtrackerai/badges/master/pipeline.svg) [![Documentation Status](https://readthedocs.org/projects/idtrackerai/badge/?version=latest)](https://idtracker.ai/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/idtrackerai.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/idtrackerai/) ![pylint](https://gitlab.com/polavieja_lab/idtrackerai/-/jobs/artifacts/master/raw/pylint/pylint.svg?job=test) [![PyPI downloads](https://img.shields.io/pypi/dm/idtrackerai.svg)](https://pypistats.org/packages/idtrackerai) ![Licence](https://img.shields.io/gitlab/license/polavieja_lab/idtrackerai.svg)
 
-Idtracker.ai is a multi-animal tracking software for laboratory conditions. This work has been published in [Nature Methods](https://doi.org/10.1038/s41592-018-0295-5) ([pdf here](https://drive.google.com/file/d/1fYBcmH6PPlwy0AQcr4D0iS2Qd-r7xU9n/view?usp=sharing))
+# Find everything you are looking for in [our website](https://idtracker.ai)
 
-Find everything you are looking for in [our website](https://idtracker.ai)
+Idtracker.ai is a multi-animal tracking software for laboratory conditions. This work has been published in [Nature Methods](https://doi.org/10.1038/s41592-018-0295-5) ([pdf here](https://drive.google.com/file/d/1fYBcmH6PPlwy0AQcr4D0iS2Qd-r7xU9n/view?usp=sharing))
 
 ## Installation for developers.
 
 On an environment with Python 3.10 and a working installation of Pytorch (Torch and Torchvision) you can install idtracker.ai for devs by cloning the repo and installing:
 
 ``` bash
-git clone https://gitlab.com/polavieja_lab/idtrackerai
-pip install -e ./idtrackerai[dev]
+pip install git+https://gitlab.com/polavieja_lab/idtrackerai
 ```
 
 ## Contributors
 * Jordi Torrents (2022-)
 * Antonio Ortega (2021-)
 * Francisco Romero-Ferrero (2015-2022)
 * Mattia G. Bergomi (2015-2018)
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai.egg-info/SOURCES.txt` & `idtrackerai-5.1.0/src/idtrackerai.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
+src/idmatcherai/__init__.py
+src/idmatcherai/main.py
+src/idmatcherai/matcher.py
 src/idtrackerai/__init__.py
 src/idtrackerai/blob.py
 src/idtrackerai/constants.toml
 src/idtrackerai/fragment.py
 src/idtrackerai/globalfragment.py
 src/idtrackerai/list_of_blobs.py
 src/idtrackerai/list_of_fragments.py
@@ -23,15 +26,14 @@
 src/idtrackerai/crossings_detection/crossing_detector.py
 src/idtrackerai/crossings_detection/crossings_detection.py
 src/idtrackerai/crossings_detection/model_area.py
 src/idtrackerai/crossings_detection/dataset/__init__.py
 src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py
 src/idtrackerai/crossings_detection/dataset/crossings_dataset.py
 src/idtrackerai/crossings_detection/network/__init__.py
-src/idtrackerai/crossings_detection/network/network_params_crossings.py
 src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py
 src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py
 src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py
 src/idtrackerai/data/test_A.avi
 src/idtrackerai/data/test_B.avi
 src/idtrackerai/fragmentation/__init__.py
 src/idtrackerai/fragmentation/fragmentation.py
@@ -39,27 +41,19 @@
 src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
 src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
 src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py
 src/idtrackerai/groundtruth_utils/generate_groundtruth.py
 src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py
 src/idtrackerai/network/__init__.py
 src/idtrackerai/network/evaluate.py
+src/idtrackerai/network/learners.py
+src/idtrackerai/network/models.py
+src/idtrackerai/network/network_params.py
 src/idtrackerai/network/train.py
-src/idtrackerai/network/learners/__init__.py
-src/idtrackerai/network/learners/learners.py
-src/idtrackerai/network/models/__init__.py
-src/idtrackerai/network/models/models_utils.py
-src/idtrackerai/network/models/pytorch_architectures.py
-src/idtrackerai/network/modules/__init__.py
-src/idtrackerai/network/modules/criterion.py
-src/idtrackerai/network/modules/pairwise.py
-src/idtrackerai/network/utils/__init__.py
-src/idtrackerai/network/utils/metric.py
-src/idtrackerai/network/utils/task.py
-src/idtrackerai/network/utils/utils.py
+src/idtrackerai/network/utils.py
 src/idtrackerai/postprocess/__init__.py
 src/idtrackerai/postprocess/assign_them_all.py
 src/idtrackerai/postprocess/compute_velocity_model.py
 src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py
 src/idtrackerai/postprocess/erosion.py
 src/idtrackerai/postprocess/get_trajectories.py
 src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
@@ -74,15 +68,14 @@
 src/idtrackerai/tracker/pre_trainer.py
 src/idtrackerai/tracker/tracker.py
 src/idtrackerai/tracker/dataset/__init__.py
 src/idtrackerai/tracker/dataset/identification_dataloader.py
 src/idtrackerai/tracker/dataset/identification_dataset.py
 src/idtrackerai/tracker/network/__init__.py
 src/idtrackerai/tracker/network/get_predictions.py
-src/idtrackerai/tracker/network/network_params.py
 src/idtrackerai/tracker/network/stop_training_criteria.py
 src/idtrackerai/tracker/network/trainer.py
 src/idtrackerai/utils/__init__.py
 src/idtrackerai/utils/check_PyPI_version.py
 src/idtrackerai/utils/confparams.py
 src/idtrackerai/utils/init_logger.py
 src/idtrackerai/utils/py_utils.py
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/GUI_main_base.py` & `idtrackerai-5.1.0/src/idtrackerai_GUI_tools/GUI_main_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 
 from .themes import dark, light
 
 
 class GUIBase(QMainWindow):
     def __init__(self):
         logging.debug(f"Initializing {self.__class__.__name__}")
-        if "Fusion" in QStyleFactory.keys():
+        if "Fusion" in QStyleFactory.keys():  # noqa SIM118
             QApplication.setStyle("Fusion")
         super().__init__()
 
-        QApplication.setApplicationDisplayName("idTracker.ai")
-        QApplication.setApplicationName("idTracker.ai")
+        QApplication.setApplicationDisplayName("idtracker.ai")
+        QApplication.setApplicationName("idtracker.ai")
         self.setWindowIcon(QIcon(str(Path(__file__).parent / "logo_256.png")))
 
         self.setCentralWidget(QWidget())
         self.centralWidget().setLayout(QHBoxLayout())
 
         self.documentation_url: str = ""
         """Link to documentation appearing in the menu bar"""
@@ -102,14 +102,17 @@
 
     def change_theme(self, dark_theme: bool):
         if dark_theme:
             QApplication.setPalette(dark)
         else:
             QApplication.setPalette(light)
 
+        # in some computers, the tooltip text is white ignoring the palette
+        self.setStyleSheet("QToolTip { color: black;}")
+
     def closeEvent(self, event: QCloseEvent):
         json.dump(
             {
                 "dark_theme": self.themeAction.isChecked(),
                 "fontsize": self.font().pointSize(),
             },
             self.json_path.open("w"),
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/__init__.py` & `idtrackerai-5.1.0/src/idtrackerai_GUI_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat` & `idtrackerai-5.1.0/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/logo_256.png` & `idtrackerai-5.1.0/src/idtrackerai_GUI_tools/logo_256.png`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/themes.py` & `idtrackerai-5.1.0/src/idtrackerai_GUI_tools/themes.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/tooltips.toml` & `idtrackerai-5.1.0/src/idtrackerai_GUI_tools/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/widgets_utils/canvas.py` & `idtrackerai-5.1.0/src/idtrackerai_GUI_tools/widgets_utils/canvas.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py` & `idtrackerai-5.1.0/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         self.max_n_row = max_n_row
 
         self.setAlternatingRowColors(True)
 
         self.ListChanged.connect(self.update_height)
         self.model().rowsInserted.connect(self.ListChanged.emit)
         self.model().rowsRemoved.connect(self.ListChanged.emit)
+        self.model().rowsMoved.connect(self.ListChanged.emit)
         self.itemPressed.connect(self.item_selected)
         self.currentItemChanged.connect(lambda x, y: self.item_selected(x))
         self.selected_item = None
 
     def focusOutEvent(self, event):
         self.clearSelection()
         item = self.itemWidget(self.selected_item)
@@ -81,21 +82,21 @@
 
     def add_str(self, text: str, color: QColor | int | None = None):
         item = QListWidgetItem()
         cw = CustomListItem(
             text, remove_func=self.remove_item, parent=item, color=color
         )
         item.setData(Qt.ItemDataRole.UserRole, text)
-        self.addItem(item)
+        self.insertItem(-1, item)
         self.setItemWidget(item, cw)
 
     def getValue(self) -> list[str]:
         return [
             self.item(i).data(Qt.ItemDataRole.UserRole) for i in range(self.count())
-        ]
+        ][::-1]
 
 
 class CustomListItem(QWidget):
     def __init__(
         self,
         text,
         parent: QListWidgetItem,
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py` & `idtrackerai-5.1.0/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,23 @@
         self.setEnabled(False)
 
     def changeEvent(self, event: QEvent):
         if event.type() == QEvent.Type.EnabledChange:
             self.setEnabled(False)
 
 
-def build_ROI_patches_from_list(width, height, list_of_ROIs) -> QPainterPath:
+def build_ROI_patches_from_list(
+    width: int, height: int, list_of_ROIs: list[str] | None
+) -> QPainterPath:
     path = QPainterPath()
-    if not list_of_ROIs:
+
+    if list_of_ROIs is None:
         return path
 
-    if list_of_ROIs[0][0] == "+":
-        path.addRect(0, 0, width, height)
+    path.addRect(0, 0, width, height)
 
     for line in list_of_ROIs:
         points = get_vertices_from_label(line)
         path_i = QPainterPath(QPointF(*points[0]))
         for point in points[1:]:
             path_i.lineTo(*point)
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py` & `idtrackerai-5.1.0/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,32 +40,34 @@
             self.frame_small_cache.cache_clear()
 
     def frame(self, frame_number: int, color: bool):
         if self.reduced_cache:
             return self.frame_small_cache(frame_number, color)
         return self.frame_large_cache(frame_number, color)
 
-    @lru_cache(128)
+    # TODO check flake8 warnings
+    @lru_cache(128)  # noqa: B019
     def frame_large_cache(self, frame_number: int, color: bool):
         return self.read_frame(frame_number, color)
 
-    @lru_cache(16)
+    @lru_cache(16)  # noqa: B019
     def frame_small_cache(self, frame_number: int, color: bool):
         return self.read_frame(frame_number, color)
 
     def read_frame(self, frame_number: int, color: bool) -> np.ndarray:
         if not self.video_loaded:
             return np.array([[]])
-        for path, (start, end) in self.interval_dict.items():
+        for _path, (start, end) in self.interval_dict.items():
             if start <= frame_number < end:
                 break
         else:
             raise ValueError(
                 f"Frame number {frame_number} not in intervals {self.interval_dict}"
             )
+        path = _path
 
         if path != self.current_captured_video_path:
             self.cap = cv2.VideoCapture(str(path))
             self.current_captured_video_path = path
 
         frame_number_in_path = frame_number - start
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_GUI_tools/widgets_utils/video_player.py` & `idtrackerai-5.1.0/src/idtrackerai_GUI_tools/widgets_utils/video_player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from contextlib import suppress
 from pathlib import Path
 from time import perf_counter
 
 import numpy as np
 import toml
 from PyQt6.QtCore import QEvent, QRectF, QSize, Qt, QTimer, pyqtSignal
 from PyQt6.QtGui import (
@@ -140,15 +141,15 @@
 
         self.reduce_cache = QAction("Reduce memory usage", self)
         self.reduce_cache.setCheckable(True)
         menu.addAction(self.reduce_cache)
         self.VideoPlayer_param_path = Path(__file__).parent / "video_player.json"
         self.reduce_cache.toggled.connect(self.video_path_holder.set_cache_mode)
         self.reduce_cache.setChecked(
-            json.loads(self.VideoPlayer_param_path.read_text())["reduce_cache"]
+            json.load(self.VideoPlayer_param_path.open())["reduce_cache"]
             if self.VideoPlayer_param_path.is_file()
             else False
         )
 
         def limit_framerate_toggled(state: bool):
             self.min_time_between_frames = 1 / self.fps if state else 0
 
@@ -309,18 +310,16 @@
             self.freeze = True
             self.forward_timer.start()
             self.play_pause_button.setChecked(False)
         elif key in (Qt.Key.Key_A, Qt.Key.Key_Left):
             self.freeze = True
             self.backward_timer.start()
             self.play_pause_button.setChecked(False)
-        try:
+        with suppress(ValueError):
             self.setSpeed(int(event.text()))
-        except ValueError:
-            pass
 
     def keyReleaseEvent(self, event: QKeyEvent):
         if event.isAutoRepeat():
             return
         key = event.key()
         if key in (Qt.Key.Key_D, Qt.Key.Key_Right):
             self.forward_timer.stop()
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_start_app/__main__.py` & `idtrackerai-5.1.0/src/idtrackerai_start_app/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     if ready_to_track:
         from .run_idtrackerai import RunIdTrackerAi
 
         check_version_on_console_thread()
 
         return RunIdTrackerAi(parameters).track_video()
     run_segmentation_GUI(parameters)
-    if parameters.get("run_idtrackerai", False):
+    if parameters.get("run_idtrackerai"):
         from .run_idtrackerai import RunIdTrackerAi
 
         return RunIdTrackerAi(parameters).track_video()
     return False
 
 
 def run_segmentation_GUI(params: dict):
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_start_app/all_valid_parameters.dat` & `idtrackerai-5.1.0/src/idtrackerai_start_app/all_valid_parameters.dat`

 * *Files 18% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 batch_size_dcd
 batch_size_predictions_dcd
 learning_percentage_difference_1_dcd
 learning_percentage_difference_2_dcd
 overfitting_counter_threshold_dcd
 maximum_number_of_epochs_dcd
 minimum_number_of_frames_to_be_a_candidate_for_accumulation
-layers_to_optimise_accumulation
 available_video_extension
 layers_to_optimise_pretraining
 learning_rate_idcnn_accumulation
 validation_proportion
 batch_size_idcnn
 batch_size_predictions_idcnn
 learning_percentage_difference_1_idcnn
@@ -52,8 +51,8 @@
 ratio_old
 ratio_new
 certainty_threshold
 max_ratio_of_pretrained_images
 minimum_ratio_of_images_accumulated_globally_to_start_partial_accumulation
 fixed_identity_threshold
 vel_percentile
-protocol3_action
+protocol3_action
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_start_app/arg_parser.py` & `idtrackerai-5.1.0/src/idtrackerai_start_app/arg_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import ast
 from argparse import ArgumentParser
 from importlib.resources import files
 from pathlib import Path
+from typing import Optional
 
 import toml
 
 
 def Bool(value: str):
     valid = {"true": True, "t": True, "1": True, "false": False, "f": False, "0": False}
 
     lower_value = value.lower()
     if lower_value not in valid:
         raise ValueError
     return valid[lower_value]
 
 
 def path(value: str):
-    return_path = Path(value).expanduser().resolve()
+    return_path = Path(value).expanduser().resolve().absolute()
     if not return_path.exists():
-        raise ValueError()
+        raise ValueError
     return return_path
 
 
 def pair_of_ints(value: str):
     out = ast.literal_eval(value)
     if not isinstance(out, (tuple, list)):
         raise ValueError
@@ -31,17 +32,19 @@
     if len(out) != 2:
         raise ValueError
     if any(not isinstance(x, int) for x in out):
         raise ValueError
     return out
 
 
-def get_parser(defaults: dict = {}) -> ArgumentParser:
+def get_parser(defaults: Optional[dict] = None) -> ArgumentParser:
+    if defaults is None:
+        defaults = {}
     parser = ArgumentParser(
-        prog="idTracker.ai", epilog="For more info visit https://idtracker.ai"
+        prog="idtracker.ai", epilog="For more info visit https://idtracker.ai"
     )
 
     def add_argument(name: str, help: str, type, metavar: str = "", **kwargs):
         name = name.lower()
 
         metavar = f"<{type.__name__.lower()}>"
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_start_app/run_idtrackerai.py` & `idtrackerai-5.1.0/src/idtrackerai_start_app/run_idtrackerai.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                     "Tracking without identities finished\n"
                     "No estimated accuracy computed."
                 )
             else:
                 logging.info(f"Estimated accuracy: {self.video.estimated_accuracy:.4%}")
 
             self.video.delete_data()
-            logging.info("Success")
+            logging.info("[green]Success", extra={"markup": True})
             success = True
 
         except CustomError as error:
             logging.error(
                 "An error occurred, saving data before "
                 "printing traceback and exiting the program"
             )
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_GUI.py` & `idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,17 @@
     """
 
     def __init__(self, GUI_out_params: dict):
         super().__init__()
 
         self.setWindowTitle("Segmentation App")
         self.user_params = GUI_out_params
-        self.documentation_url = "https://idtrackerai.readthedocs.io/en/latest/"
+        self.documentation_url = (
+            "https://idtracker.ai/en/latest/user_guide/segmentation_app.html"
+        )
 
         self.open_widget = OpenVideoWidget(self)
         self.videoPlayer = VideoPlayer(self)
         self.frame_analyzer = FrameAnalyzer()
         self.blobInfo = BlobInfoWidget()
         self.bkg_widget = BkgWidget(self)
         self.ROI_Widget = ROIWidget(self)
@@ -241,15 +243,15 @@
         """Loads configuration from `load_dict` setting the corresponding widgets status
 
         Parameters
         ----------
         load_dict : dict
             Parameters to load
         """
-        self.open_widget.open_video_paths(load_dict.get("video_paths", None))
+        self.open_widget.open_video_paths(load_dict.get("video_paths"))
         self.resreduct.setValue(int(load_dict["resolution_reduction"] * 100))
         self.tracking_interval.setValue(load_dict["tracking_intervals"])
         self.ROI_Widget.setValue(load_dict["roi_list"])
         self.intensity_thresholds.setValue(load_dict.get("intensity_ths", (0, 155)))
         self.area_thresholds.setValue(load_dict.get("area_ths", (50, 99999999999)))
         self.n_animals.setValue(load_dict.get("number_of_animals", 0))
         self.track_wo_id.setChecked(load_dict["track_wo_identities"])
@@ -257,24 +259,20 @@
         self.session.setText(load_dict.get("session", ""))
         self.bkg_widget.checkBox.setChecked(load_dict["use_bkg"])
         self.videoPlayer.update()
 
     def close_and_track_video(self):
         """Action when clicked "close and track video".
         It gathers widgets parameters, writes them in self.user_params and exits"""
-        if self.n_animals.value() == 0:
-            QMessageBox.warning(
-                self,
-                "Missing parameter",
-                "Please, define the number of animals in the video",
-            )
+        parameters = self.out_parameters()
+        if self.unacceptable_parameters(parameters):
             return
-        GUI_params = self.out_parameters()
-        logging.info(pprint_dict(GUI_params, "GUI params"), extra={"markup": True})
-        self.user_params.update(GUI_params)
+
+        logging.info(pprint_dict(parameters, "GUI params"), extra={"markup": True})
+        self.user_params.update(parameters)
         self.user_params["bkg_model"] = self.bkg_widget.getBkg()
         # signal to start tracking after closing app
         self.user_params["run_idtrackerai"] = True
         self.close()
 
     def getSessionName(self) -> str:
         session_name = self.session.text()
@@ -298,33 +296,51 @@
             "use_bkg": self.bkg_widget.checkBox.isChecked(),
             "check_segmentation": self.check_segm.isChecked(),
             "resolution_reduction": self.resreduct.value() / 100,
             "track_wo_identities": self.track_wo_id.isChecked(),
             "roi_list": self.ROI_Widget.getValue(),
         }
 
-    def save_parameters_func(self):
-        if self.n_animals.value() == 0:
+    def unacceptable_parameters(self, parameters: dict) -> bool:
+        if parameters["number_of_animals"] == 0:
             QMessageBox.warning(
                 self,
                 "Missing parameters",
                 "Please, define the number of animals in the video",
             )
+            return True
+        if parameters["roi_list"] is not None and len(parameters["roi_list"]) == 0:
+            QMessageBox.warning(
+                self,
+                "Missing parameters",
+                (
+                    "Please, add a region of interest or uncheck the Regions of"
+                    " interest parameter."
+                ),
+            )
+            return True
+        return False
+
+    def save_parameters_func(self):
+        parameters = self.out_parameters()
+
+        if self.unacceptable_parameters(parameters):
             return
+
         fileName, _ = QFileDialog.getSaveFileName(
             self,
             "Save parameter file",
             str(Path.cwd() / (self.getSessionName() + ".toml")),
             filter="TOML (*.toml)",
         )
         if not fileName:
             return
 
         with open(fileName, "w", encoding="utf_8") as file:
-            for key, value in self.out_parameters().items():
+            for key, value in parameters.items():
                 file.write(f"{key} = {toml_format(value)}\n")
 
     def new_video_paths(
         self,
         video_paths: list[str],
         video_size: tuple[int, int],
         n_frames: int,
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py` & `idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from math import sqrt
-
 import numpy as np
 from cv2 import fitEllipse
 from PyQt6.QtCore import Qt, pyqtSignal
 from PyQt6.QtGui import QColor, QPainterPath
 from PyQt6.QtWidgets import (
     QCheckBox,
     QDialog,
     QGridLayout,
     QHBoxLayout,
+    QListView,
     QListWidgetItem,
     QMessageBox,
     QPushButton,
     QSizePolicy,
     QToolButton,
     QVBoxLayout,
     QWidget,
@@ -25,15 +24,15 @@
     CustomList,
     build_ROI_patches_from_list,
 )
 
 
 class ROIWidget(QWidget):
     needToDraw = pyqtSignal()
-    valueChanged = pyqtSignal(np.ndarray)
+    valueChanged = pyqtSignal(object)  # np.ndarray | None
 
     def __init__(self, parent):
         super().__init__()
 
         self.CheckBox = QCheckBox("Regions of interest")
         self.CheckBox.stateChanged.connect(self.CheckBox_changed)
 
@@ -42,41 +41,43 @@
         self.add.setCheckable(True)
         self.add.setVisible(False)
         self.addAction("", Qt.Key.Key_Return, lambda: self.add.setChecked(False))
 
         self.list = CustomList()
         self.list.setVisible(False)
 
-        # self.list.ListChanged.connect(self.list.update_height)
+        self.list.setDefaultDropAction(Qt.DropAction.MoveAction)
+        self.list.setMovement(QListView.Movement.Free)
 
         Controls_HBox = QHBoxLayout()
         Controls_HBox.addWidget(self.CheckBox)
         Controls_HBox.addWidget(self.add)
 
         layout = QVBoxLayout()
         layout.setSpacing(2)
         self.setLayout(layout)
         layout.addLayout(Controls_HBox)
         layout.addWidget(self.list)
 
         self.add.toggled.connect(self.add_clicked)
         self.list.ListChanged.connect(self.update_Patches)
+        self.CheckBox.stateChanged.connect(self.update_Patches)
         self.list.ListChanged.connect(lambda: self.valueChanged.emit(self.getMask()))
 
         self.ROI_popup = ROI_PopUp(parent)
         self.list.newItemSelected.connect(self.paint_selected_polygon)
         self.mask_path = QPainterPath()
         self.clicked_points = []
         self.ListItem_clicked = False
 
-    def getValue(self) -> list[str]:
-        return self.list.getValue() if self.CheckBox.isChecked() else []
+    def getValue(self) -> list[str] | None:
+        return self.list.getValue() if self.CheckBox.isChecked() else None
 
-    def getMask(self) -> np.ndarray:
-        return build_ROI_mask_from_list(*self.video_size, list_of_ROIs=self.getValue())
+    def getMask(self) -> np.ndarray | None:
+        return build_ROI_mask_from_list(self.getValue(), *self.video_size)
 
     def CheckBox_changed(self, enabled):
         if self.add.isChecked():
             self.add.click()
         self.list.setVisible(enabled)
         self.add.setVisible(enabled)
         self.valueChanged.emit(self.getMask())
@@ -106,60 +107,60 @@
 
         else:
             self.ListItem_clicked = False
             self.clicked_points.clear()
         self.needToDraw.emit()
 
     def add_clicked(self, checked):
+        xy, self.clicked_points = self.clicked_points, []
+
         if checked:
-            if self.ROI_popup.exec():
-                self.ROI_type = self.ROI_popup.value
-                self.needToDraw.emit()
-            else:
+            self.ROI_type = self.ROI_popup.exec(self.list.count() == 0)
+            if self.ROI_type is None:
                 self.add.setChecked(False)
-        else:
-            xy = self.clicked_points
-            if not xy:  # any drawn points
-                return
-            self.needToDraw.emit()
+            return
 
-            if self.ROI_type[2:9] == "Polygon":
-                if len(xy) < 3:
-                    QMessageBox.warning(
-                        self,
-                        "ROI error",
-                        "Polygons can only be defined with 3 points or more",
-                    )
-                else:
-                    self.list.add_str(
-                        f"{self.ROI_type} ["
-                        + ", ".join([f"[{x:.1f}, {y:.1f}]" for x, y in xy])
-                        + "]"
-                    )
-            elif self.ROI_type[2:9] == "Ellipse":
-                if len(xy) < 5:
-                    QMessageBox.warning(
-                        self,
-                        "ROI error",
-                        (
-                            "Ellipses can only be defined with 5 points"
-                            "(exact fit) or more (approximated fit)"
-                        ),
-                    )
-                else:
-                    center, axis, angle = fitEllipse(np.asarray(xy, dtype="f"))
-                    axis = axis[0] / 2.0, axis[1] / 2.0
-                    self.list.add_str(
-                        f"{self.ROI_type} "
-                        + "{"
-                        + f"'center': [{center[0]:.0f}, {center[1]:.0f}], "
-                        f"'axes': [{axis[0]:.0f}, {axis[1]:.0f}], 'angle': {angle:.0f}"
-                        + "}"
-                    )
-        self.clicked_points.clear()
+        if not xy:  # any drawn points
+            return
+
+        assert self.ROI_type is not None
+
+        if self.ROI_type[2:9] == "Polygon":
+            if len(xy) < 3:
+                QMessageBox.warning(
+                    self,
+                    "ROI error",
+                    "Polygons can only be defined with 3 points or more",
+                )
+            else:
+                self.list.add_str(
+                    f"{self.ROI_type} ["
+                    + ", ".join([f"[{x:.1f}, {y:.1f}]" for x, y in xy])
+                    + "]"
+                )
+        elif self.ROI_type[2:9] == "Ellipse":
+            if len(xy) < 5:
+                QMessageBox.warning(
+                    self,
+                    "ROI error",
+                    (
+                        "Ellipses can only be defined with 5 points"
+                        "(exact fit) or more (approximated fit)"
+                    ),
+                )
+            else:
+                center, axis, angle = fitEllipse(np.asarray(xy, dtype="f"))
+                axis = axis[0] / 2.0, axis[1] / 2.0
+                self.list.add_str(
+                    f"{self.ROI_type} "
+                    + "{"
+                    + f"'center': [{center[0]:.0f}, {center[1]:.0f}], "
+                    f"'axes': [{axis[0]:.0f}, {axis[1]:.0f}], 'angle': {angle:.0f}"
+                    + "}"
+                )
 
     def set_video_size(self, video_size):
         self.video_size = video_size
 
     def update_Patches(self):
         self.mask_path = build_ROI_patches_from_list(
             *self.video_size, list_of_ROIs=self.getValue()
@@ -196,33 +197,39 @@
         super().__init__(parent=parent)
         self.setWindowModality(Qt.WindowModality.ApplicationModal)
         self.setFixedSize(300, 100)
         self.setWindowTitle("Add ROI type")
         layout = QGridLayout()
         self.setLayout(layout)
 
-        PP_button = QPushButton("+ Polygon")
-        PE_button = QPushButton("+ Ellipse")
-        NP_button = QPushButton("- Polygon")
-        NE_button = QPushButton("- Ellipse")
+        self.PP_button = QPushButton("+ Polygon")
+        self.PE_button = QPushButton("+ Ellipse")
+        self.NP_button = QPushButton("- Polygon")
+        self.NE_button = QPushButton("- Ellipse")
 
         policy = QSizePolicy.Policy.Expanding
-        PP_button.setSizePolicy(policy, policy)
-        PE_button.setSizePolicy(policy, policy)
-        NP_button.setSizePolicy(policy, policy)
-        NE_button.setSizePolicy(policy, policy)
-
-        PP_button.clicked.connect(self.clicked_event)
-        PE_button.clicked.connect(self.clicked_event)
-        NP_button.clicked.connect(self.clicked_event)
-        NE_button.clicked.connect(self.clicked_event)
-
-        layout.addWidget(PP_button, 0, 0)
-        layout.addWidget(PE_button, 0, 1)
-        layout.addWidget(NP_button, 1, 0)
-        layout.addWidget(NE_button, 1, 1)
+        self.PP_button.setSizePolicy(policy, policy)
+        self.PE_button.setSizePolicy(policy, policy)
+        self.NP_button.setSizePolicy(policy, policy)
+        self.NE_button.setSizePolicy(policy, policy)
+
+        self.PP_button.clicked.connect(self.clicked_event)
+        self.PE_button.clicked.connect(self.clicked_event)
+        self.NP_button.clicked.connect(self.clicked_event)
+        self.NE_button.clicked.connect(self.clicked_event)
+
+        layout.addWidget(self.PP_button, 0, 0)
+        layout.addWidget(self.PE_button, 0, 1)
+        layout.addWidget(self.NP_button, 1, 0)
+        layout.addWidget(self.NE_button, 1, 1)
 
     def clicked_event(self):
         sender = self.sender()
         assert isinstance(sender, QPushButton)
         self.value = sender.text()
         self.accept()
+
+    def exec(self, only_positive: bool = False) -> str | None:
+        self.NP_button.setEnabled(not only_positive)
+        self.NE_button.setEnabled(not only_positive)
+
+        return self.value if super().exec() == QDialog.DialogCode.Accepted else None
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py` & `idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py` & `idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,15 @@
         self.n_animals = 0
         self.tracking_intervals: list[list[int]] | None = None
         self.setMinimumSize(100, 100)
 
     def in_tracking_intervals(self, frame) -> bool:
         if self.tracking_intervals is None:
             return True
-        for start, end in self.tracking_intervals:
-            if start <= frame < end:
-                return True
-        return False
+        return any(start <= frame < end for start, end in self.tracking_intervals)
 
     def setAreas(self, frame: int, areas: list[int]):
         self.frame = frame
         self.areas = areas
         self.update()
 
     def setNAnimals(self, n_animals):
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py` & `idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 from PyQt6.QtCore import pyqtSignal
 from PyQt6.QtGui import QPolygon
 from PyQt6.QtWidgets import QWidget
 
 from idtrackerai.animals_detection.segmentation import process_frame
 from idtrackerai_GUI_tools import CanvasPainter
 
@@ -12,15 +13,15 @@
 
     def set_bkg(self, bkg_model):
         self.bkg_model = bkg_model
         self.use_bkg = bkg_model is not None
         self.need_to_redraw = True
         self.new_parameters.emit()
 
-    def set_ROI_mask(self, ROI_mask):
+    def set_ROI_mask(self, ROI_mask: np.ndarray | None):
         self.ROI_mask = ROI_mask
         self.need_to_redraw = True
         self.new_parameters.emit()
 
     def set_resolution_reduction(self, resolution_reduction: float):
         self.resolution_reduction = resolution_reduction
         self.need_to_redraw = True
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py` & `idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py` & `idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         video_paths, _ = QFileDialog.getOpenFileNames(
             self.parent_widget,
             "Open a video file to track",
             filter=self.extension_filter,
         )
         self.open_video_paths(sorted(video_paths))
 
-    def open_video_paths(self, video_paths: Sequence[str | Path]):
+    def open_video_paths(self, video_paths: Sequence[str | Path] | None):
         if not video_paths:
             return
         try:
             video_paths = [Path(path).expanduser().resolve() for path in video_paths]
             Video.assert_video_paths(video_paths)
             self.video_width, self.video_height, self.fps = (
                 Video.get_info_from_video_paths(video_paths)
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py` & `idtrackerai-5.1.0/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_start_app/tooltips.toml` & `idtrackerai-5.1.0/src/idtrackerai_start_app/tooltips.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 open_btn = '<qt>Select the video file(s) to track. Select multiple files to track them as if they were concatenated, intended for consecutive clips of the same experiment.'
 open_path_label = '<qt>Current video path to be tracked'
 open_path_list = '<qt>List of video paths in the order they are going to be tracked. Click on one of them to set the video player to its beginning. Drag and drop to reorder'
 tacking_interval = '<qt>Set the time interval(s) to track (in units of frames). Frames outside the specified ranges will be neglected'
-region_of_interest = '<qt>Define an area on the video for idtrackerai to look for blobs (positive) or to ignore blobs (negative). Click "Add", select the desired region shape and start clicking on the video player to define the desired contour (left click to add points and right click to erase them)'
+region_of_interest = '<qt>Define an area on the video for idtrackerai to look for blobs (positive) or to ignore blobs (negative). By default, the whole video area is a negative region when this tool is active. Click "Add", select the desired region type and start clicking on the video player to define the desired region contour (left click to add points and right click to erase them). Drag and drop to reorder existing ROIs.'
 background_subtraction = '<qt>Compute the video background and use it together with "Background difference threshold" to detect blobs'
 number_of_animals = '<qt>Insert the number of animals appearing in the video'
 check_segm = "<qt>If checked, idtrackerai will exit if frames with more blobs than animals are found. If not checked, idtracker.ai will only emit a warning about those frames and it will go on"
 area_thresholds = "<qt>Defines tha valid blob's area range. Smaller or larger blobs will be neglected"
 intensity_thresholds_nobkg = "<qt>Defines tha valid blob's brightness range (being 0 black and 255 white). Any cluster of pixels whose brightness is in this range will conform a blob. Tip: for dark animals on a bright background set the lower threshold to the minimum, otherwise set the upper threshold to the maximum."
 intensity_thresholds_yesbkg = "<qt>Defines the pixel to background brightness difference threshold. Any cluster of pixels whose brighntess difference with the background is greater than the threshold will conform a blob"
 resolution_reduction = '<qt>Reduces the video resolution. Useful for videos with very big animals (rats, mices...) which blobs get too big (areas > 10k px)'
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_validator/__main__.py` & `idtrackerai-5.1.0/src/idtrackerai_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_validator/tooltips.toml` & `idtrackerai-5.1.0/src/idtrackerai_validator/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_validator/validation_GUI.py` & `idtrackerai-5.1.0/src/idtrackerai_validator/validation_GUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 
 class DblClickDialog(QDialog):
     class Answers(Enum):
         Cancel = 0
         ChangeId = 1
         Interpolate = 2
 
-    # TODO pop up dialog when closing without saving
     def __init__(self, parent: QWidget, n_animals: int):
         super().__init__(parent)
         self.spinbox = QSpinBox()
         self.spinbox.setMinimum(-1)
         self.spinbox.setMaximum(n_animals)
         main_layout = QVBoxLayout()
         self.setLayout(main_layout)
@@ -152,16 +151,18 @@
 
 class ValidationGUI(GUIBase):
     def __init__(self, session_path: Path | None = None):
         super().__init__()
 
         # TODO logging.getLogger().addHandler(WarningRedirector(self))
 
-        self.setWindowTitle("idTracker.ai | Validation GUI")
-        self.documentation_url = "https://idtrackerai.readthedocs.io/en/latest/"
+        self.setWindowTitle("idtracker.ai | Validation GUI")
+        self.documentation_url = (
+            "https://idtracker.ai/en/latest/user_guide/validator.html"
+        )
 
         self.video_player = VideoPlayer(self)
         self.video_player.limit_framerate.setChecked(True)
         self.widgets_to_close.append(self.video_player)
 
         self.video_player.canvas.click_event.connect(self.click_on_canvas)
         self.video_player.canvas.double_click_event.connect(self.double_click_on_canvas)
@@ -505,14 +506,15 @@
             self.trajectories, self.unidentified, self.duplicated, self.blobs
         )
         self.video_player.update()
         self.unsaved_changes = False
 
         if hasattr(self.video, "ROI_list") and self.video.ROI_list:
             self.view_ROIs.setEnabled(True)
+            self.view_ROIs.setChecked(True)
             self.ROI_pathces = build_ROI_patches_from_list(
                 self.video.width, self.video.height, self.video.ROI_list
             )
         else:
             self.view_ROIs.setChecked(False)
             self.view_ROIs.setEnabled(False)
 
@@ -596,15 +598,15 @@
             cmap, cmap_alpha = self.id_groups.get_cmaps(self.video.number_of_animals)
         else:
             cmap, cmap_alpha = self.cmap, self.cmap_alpha
 
         update_info_widget = frame_number != self.current_frame_number
         self.current_frame_number = frame_number
 
-        if not self.selected_blob is None and self.selected_blob not in blobs_in_frame:
+        if self.selected_blob is not None and self.selected_blob not in blobs_in_frame:
             self.selected_blob, self.selection_last_location = find_selected_blob(
                 blobs_in_frame, self.selected_id, self.selection_last_location
             )
 
         if self.view_trails.isChecked():
             paintTrails(self.current_frame_number, painter, self.trajectories, cmap)
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/errors_explorer.py` & `idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/errors_explorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             except RuntimeWarning:
                 return []
 
         too_fast = (
             speed > (mean + self.jumps_th.value() * std)
         ) & self.non_accepted_jumps
         out = get_list_of_Trues_for_id(too_fast)
-        for id, start, length in out:
+        for _id, start, _length in out:
             start += 1
         return out
 
 
 def get_list_of_Trues(arr: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
     """Returns the start and the length of every True cluster in an array
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/id_groups.py` & `idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/id_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,20 +74,19 @@
         layout.addWidget(edit_btn)
         layout.addWidget(remove_btn)
         row.setLayout(layout)
         self.main_layout.addWidget(row)
         return row
 
     def uncheck_btns(self, exception: QToolButton | None):
-        for btns, group in self.id_groups.values():
+        for btns, _group in self.id_groups.values():
             for widget in btns.findChildren(QToolButton):
                 assert isinstance(widget, QToolButton)
-                if widget != exception:
-                    if widget.isChecked():
-                        widget.setChecked(False)
+                if widget != exception and widget.isChecked():
+                    widget.setChecked(False)
 
     def view_btn_clicked(self, btn: QToolButton, name: str, checked: bool):
         if checked:
             self.uncheck_btns(btn)
             self.view.add(name)
         else:
             self.view.remove(name)
@@ -131,15 +130,15 @@
             self, "idtracker.ai", "Enter identity group name:"
         )
         name = name.strip()
 
         if not ok or not name:
             return
 
-        if name in self.id_groups.keys():
+        if name in self.id_groups:
             edit_btn = self.id_groups[name][0].findChild(QToolButton, "edit")
             assert isinstance(edit_btn, QToolButton)
             edit_btn.setChecked(True)
             return
 
         btns, group = self.generate_row(name, set()), set()
         self.id_groups[name] = btns, group
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/id_labels.py` & `idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/id_labels.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/interpolator.py` & `idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/interpolator.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/paint_blobs.py` & `idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/paint_blobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         x, y = selected_centroid
         painter.setPenColor(0x000000)
         painter.drawEllipse(QRectF(x - radius / 2, y - radius / 2, radius, radius))
 
     # colored centroids
     if draw_centroids:
         painter.setPen(Qt.PenStyle.NoPen)
-        for color, idstr, (x, y) in labels_to_draw:
+        for color, _idstr, (x, y) in labels_to_draw:
             painter.setBrush(color)
             painter.drawBigPoint(x, y)
 
     # labels lines
     if draw_labels:
         zoom = painter.applied_zoom
         for color, idstr, (x, y) in labels_to_draw:
@@ -129,15 +129,15 @@
                 painter.setPenColor(color)
                 painter.drawLine(pointA, pointB)
 
     # black centroid contour
     if draw_centroids:
         painter.setBrush(Qt.BrushStyle.NoBrush)
         painter.setPenColor(0x000000)
-        for color, idstr, (x, y) in labels_to_draw:
+        for _color, _idstr, (x, y) in labels_to_draw:
             painter.drawBigPoint(x, y)
 
     # label text
     if draw_labels:
         zoom = painter.applied_zoom
         for color, idstr, (x, y) in labels_to_draw:
             if idstr:
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_validator/validator_widgets/setup_points.py` & `idtrackerai-5.1.0/src/idtrackerai_validator/validator_widgets/setup_points.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from math import sqrt
 from re import compile
 
 from PyQt6.QtCore import Qt, pyqtSignal
 from PyQt6.QtWidgets import QInputDialog, QToolButton, QVBoxLayout, QWidget
 
 from idtrackerai_GUI_tools import CanvasMouseEvent, CanvasPainter, CustomList
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_video/general_video.py` & `idtrackerai-5.1.0/src/idtrackerai_video/general_video.py`

 * *Files 9% similar despite different names*

```diff
@@ -97,31 +97,48 @@
             )
 
     return arr_img
 
 
 def generate_trajectories_video(
     video: Video,
-    trajectories: np.ndarray,
+    trajectories_path: Path | None,
     draw_in_gray: bool,
     centroid_trace_length: int,
     starting_frame: int,
     ending_frame: int,
 ):
-    draw_in_gray = draw_in_gray
+    if trajectories_path is None:
+        if (video.trajectories_folder / "trajectories_wo_gaps.npy").is_file():
+            trajectories = np.load(
+                video.trajectories_folder / "trajectories_wo_gaps.npy",
+                allow_pickle=True,
+            ).item()["trajectories"]
+        elif (video.trajectories_folder / "trajectories.npy").is_file():
+            trajectories = np.load(
+                video.trajectories_folder / "trajectories.npy", allow_pickle=True
+            ).item()["trajectories"]
+        else:
+            raise FileNotFoundError(
+                f"Could not find the trajectory file in {video.trajectories_folder}"
+            )
+    else:
+        trajectories = np.load(trajectories_path, allow_pickle=True).item()[
+            "trajectories"
+        ]
+
     if draw_in_gray:
         logging.info("Drawing original video in grayscale")
 
     resize_factor = min(1920 / video.original_width, 1080 / video.original_height, 1)
 
     if resize_factor != 1:
         logging.info(f"Applying resize of factor {resize_factor}")
 
     trajectories = np.nan_to_num(trajectories * resize_factor, nan=-1).astype(int)
-    centroid_trace_length = centroid_trace_length
 
     video_name = video.video_paths[0].stem + "_tracked.avi"
 
     colors = setColormap(video.number_of_animals)
 
     labels = video.identities_labels
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_video/individual_videos.py` & `idtrackerai-5.1.0/src/idtrackerai_video/individual_videos.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from pathlib import Path
 
 import cv2
 import numpy as np
 
 from idtrackerai import Video
 from idtrackerai.utils import create_dir, track
 from idtrackerai_GUI_tools import VideoPathHolder
@@ -19,37 +20,57 @@
         draw_x, draw_y = positions[cur_id]
         canvas[draw_y : draw_y + size, draw_x : draw_x + size] = miniframes[cur_id]
 
 
 def read_individual_miniframes(
     frame: np.ndarray, ordered_centroid: np.ndarray, miniframes: np.ndarray
 ):
+    if frame.ndim == 2:
+        frame = frame[..., None]
     miniframes[:] = 0
     size2 = miniframes.shape[1] // 2
     for cur_id, (x, y) in enumerate(ordered_centroid):
         if x > 0 and y > 0:
             miniframe = frame[
                 max(0, y - size2) : y + size2, max(0, x - size2) : x + size2
             ]
             miniframes[cur_id, 0 : miniframe.shape[0], 0 : miniframe.shape[1]] = (
                 miniframe
             )
 
 
 def generate_individual_video(
     video: Video,
-    trajectories: np.ndarray,
+    trajectories_path: Path | None,
     draw_in_gray: bool,
     starting_frame: int,
     ending_frame: int | None,
 ):
-    draw_in_gray = draw_in_gray
     if draw_in_gray:
         logging.info("Drawing original video in grayscale")
 
+    if trajectories_path is None:
+        if (video.trajectories_folder / "trajectories_wo_gaps.npy").is_file():
+            trajectories = np.load(
+                video.trajectories_folder / "trajectories_wo_gaps.npy",
+                allow_pickle=True,
+            ).item()["trajectories"]
+        elif (video.trajectories_folder / "trajectories.npy").is_file():
+            trajectories = np.load(
+                video.trajectories_folder / "trajectories.npy", allow_pickle=True
+            ).item()["trajectories"]
+        else:
+            raise FileNotFoundError(
+                f"Could not find the trajectory file in {video.trajectories_folder}"
+            )
+    else:
+        trajectories = np.load(trajectories_path, allow_pickle=True).item()[
+            "trajectories"
+        ]
+
     trajectories[np.isnan(trajectories)] = -1
     trajectories = np.nan_to_num(trajectories, nan=-1).astype(int)
 
     create_dir(video.individual_videos_folder)
 
     n_rows = int(np.sqrt(video.number_of_animals))
     n_cols = int(video.number_of_animals / n_rows - 0.0001) + 1
```

### Comparing `idtrackerai-5.0.0a5/src/idtrackerai_video/main.py` & `idtrackerai-5.1.0/src/idtrackerai_video/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from pathlib import Path
 
-import numpy as np
-
 from idtrackerai import Video
 from idtrackerai.utils import initLogger
 
 from .general_video import generate_trajectories_video
 from .individual_videos import generate_individual_video
 
 
@@ -55,42 +53,27 @@
     )
     parser.add_argument(
         "--e", type=int, default=None, help="Frame where to end the video", metavar=""
     )
     args = parser.parse_args()
 
     video = Video.load(args.session_path)
-    if args.t is None:
-        if (video.trajectories_folder / "trajectories_wo_gaps.npy").is_file():
-            trajectories = np.load(
-                video.trajectories_folder / "trajectories_wo_gaps.npy",
-                allow_pickle=True,
-            ).item()["trajectories"]
-        elif (video.trajectories_folder / "trajectories.npy").is_file():
-            trajectories = np.load(
-                video.trajectories_folder / "trajectories.npy", allow_pickle=True
-            ).item()["trajectories"]
-        else:
-            raise FileNotFoundError(
-                f"Could not find the trajectory file in {video.trajectories_folder}"
-            )
-    else:
-        trajectories = np.load(args.t, allow_pickle=True).item()["trajectories"]
+
     if args.individual:
         generate_individual_video(
             video,
-            trajectories,
+            args.t,
             draw_in_gray=args.gray,
             starting_frame=args.s,
             ending_frame=args.e,
         )
     else:
         generate_trajectories_video(
             video,
-            trajectories,
+            args.t,
             draw_in_gray=args.gray,
             centroid_trace_length=args.tl,
             starting_frame=args.s,
             ending_frame=args.e,
         )
```

