# Comparing `tmp/kognic-io-1.1.8.tar.gz` & `tmp/kognic-io-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kognic-io-1.1.8.tar", last modified: Fri Mar 17 10:22:51 2023, max compression
+gzip compressed data, was "kognic-io-1.1.9.tar", last modified: Wed Apr 12 12:52:31 2023, max compression
```

## Comparing `kognic-io-1.1.8.tar` & `kognic-io-1.1.9.tar`

### file list

```diff
@@ -1,127 +1,130 @@
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.750684 kognic-io-1.1.8/
--rw-r--r--   0 caltaluc   (501) staff       (20)    18058 2023-03-17 10:22:51.750155 kognic-io-1.1.8/PKG-INFO
--rw-r--r--   0 caltaluc   (501) staff       (20)    17476 2023-03-17 10:22:28.000000 kognic-io-1.1.8/README.md
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.731175 kognic-io-1.1.8/bin/
--rw-r--r--   0 caltaluc   (501) staff       (20)      110 2022-11-30 23:08:46.000000 kognic-io-1.1.8/bin/kognicutil
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.728797 kognic-io-1.1.8/kognic/
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.732310 kognic-io-1.1.8/kognic/io/
--rw-r--r--   0 caltaluc   (501) staff       (20)      125 2023-03-17 10:22:07.000000 kognic-io-1.1.8/kognic/io/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     3588 2023-02-22 13:48:35.000000 kognic-io-1.1.8/kognic/io/client.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     5527 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/kognicutil.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      797 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/logger.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.733114 kognic-io-1.1.8/kognic/io/model/
--rw-r--r--   0 caltaluc   (501) staff       (20)      197 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/__init__.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.733605 kognic-io-1.1.8/kognic/io/model/annotation/
--rw-r--r--   0 caltaluc   (501) staff       (20)       87 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/annotation/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      593 2023-02-22 13:48:35.000000 kognic-io-1.1.8/kognic/io/model/annotation/client_annotation.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      437 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/base_serializer.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.734354 kognic-io-1.1.8/kognic/io/model/calibration/
--rw-r--r--   0 caltaluc   (501) staff       (20)      295 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/calibration/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     2392 2023-03-15 20:22:28.000000 kognic-io-1.1.8/kognic/io/model/calibration/calib.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.735669 kognic-io-1.1.8/kognic/io/model/calibration/camera/
--rw-r--r--   0 caltaluc   (501) staff       (20)      500 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/calibration/camera/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      485 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/calibration/camera/common.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      333 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/calibration/camera/fisheye_calibration.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      547 2023-03-15 20:22:28.000000 kognic-io-1.1.8/kognic/io/model/calibration/camera/fused_cylindrical_calibration.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      634 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/calibration/camera/kannala_calibration.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      319 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/calibration/camera/pinhole_calibration.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     1072 2023-03-15 14:14:01.000000 kognic-io-1.1.8/kognic/io/model/calibration/camera/principal_point_distortion_calibration.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      584 2023-03-15 20:22:28.000000 kognic-io-1.1.8/kognic/io/model/calibration/common.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.736162 kognic-io-1.1.8/kognic/io/model/calibration/lidar/
--rw-r--r--   0 caltaluc   (501) staff       (20)       99 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/calibration/lidar/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      438 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/calibration/lidar/lidar_calibration.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.737127 kognic-io-1.1.8/kognic/io/model/ego/
--rw-r--r--   0 caltaluc   (501) staff       (20)      166 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/ego/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      483 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/ego/imu_data.py
--rw-r--r--   0 caltaluc   (501) staff       (20)       70 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/ego/utils.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      444 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/ego/validated_imu_data.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      320 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/ego/vehicle_pose.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      222 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/files_to_upload.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.738948 kognic-io-1.1.8/kognic/io/model/input/
--rw-r--r--   0 caltaluc   (501) staff       (20)      358 2023-02-22 13:48:35.000000 kognic-io-1.1.8/kognic/io/model/input/__init__.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.739873 kognic-io-1.1.8/kognic/io/model/input/abstract/
--rw-r--r--   0 caltaluc   (501) staff       (20)      101 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/abstract/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      428 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/abstract/base_frame.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      406 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/abstract/base_input.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      528 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/abstract/base_input_with_imu_data.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      273 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/abstract/sequence_frame.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.740553 kognic-io-1.1.8/kognic/io/model/input/aggregated_lidars_and_cameras_seq/
--rw-r--r--   0 caltaluc   (501) staff       (20)      216 2023-02-22 13:48:35.000000 kognic-io-1.1.8/kognic/io/model/input/aggregated_lidars_and_cameras_seq/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      870 2023-02-22 13:48:35.000000 kognic-io-1.1.8/kognic/io/model/input/aggregated_lidars_and_cameras_seq/aggregated_lidars_and_cameras_seq.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      844 2023-02-22 13:48:35.000000 kognic-io-1.1.8/kognic/io/model/input/aggregated_lidars_and_cameras_seq/frame.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.741460 kognic-io-1.1.8/kognic/io/model/input/cameras/
--rw-r--r--   0 caltaluc   (501) staff       (20)      112 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/cameras/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      602 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/cameras/cameras.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      322 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/cameras/frame.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.742081 kognic-io-1.1.8/kognic/io/model/input/cameras_sequence/
--rw-r--r--   0 caltaluc   (501) staff       (20)      147 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/cameras_sequence/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      784 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/cameras_sequence/cameras_sequence.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      466 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/cameras_sequence/frame.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     1052 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/feature_flags.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      121 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/initialized_input.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      862 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/input_entry.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      235 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/input_from_scene_request.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      553 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/input_job.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      173 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/invalidated_reason_input.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.742692 kognic-io-1.1.8/kognic/io/model/input/lidars/
--rw-r--r--   0 caltaluc   (501) staff       (20)      108 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/lidars/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      462 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/lidars/frame.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      457 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/lidars/lidars.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.743329 kognic-io-1.1.8/kognic/io/model/input/lidars_and_cameras/
--rw-r--r--   0 caltaluc   (501) staff       (20)      154 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/lidars_and_cameras/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      664 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/lidars_and_cameras/frame.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      672 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/lidars_and_cameras/lidars_and_cameras.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.743868 kognic-io-1.1.8/kognic/io/model/input/lidars_and_cameras_sequence/
--rw-r--r--   0 caltaluc   (501) staff       (20)      189 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/lidars_and_cameras_sequence/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      861 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/lidars_and_cameras_sequence/frame.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      854 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/lidars_and_cameras_sequence/lidars_and_cameras_sequence.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.744348 kognic-io-1.1.8/kognic/io/model/input/lidars_sequence/
--rw-r--r--   0 caltaluc   (501) staff       (20)      143 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/lidars_sequence/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      570 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/lidars_sequence/frame.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      639 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/lidars_sequence/lidars_sequence.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.744510 kognic-io-1.1.8/kognic/io/model/input/metadata/
--rw-r--r--   0 caltaluc   (501) staff       (20)     1425 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/metadata/metadata.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.745306 kognic-io-1.1.8/kognic/io/model/input/resources/
--rw-r--r--   0 caltaluc   (501) staff       (20)      115 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/resources/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      646 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/resources/image.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      488 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/resources/point_cloud.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     2166 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/resources/resource.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      345 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/resources/video.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      320 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/input/sensor_specification.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.746095 kognic-io-1.1.8/kognic/io/model/projects/
--rw-r--r--   0 caltaluc   (501) staff       (20)       89 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/projects/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      250 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/projects/project.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      458 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/projects/project_batch.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      247 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/model/upload_url.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.730546 kognic-io-1.1.8/kognic/io/resources/
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.746580 kognic-io-1.1.8/kognic/io/resources/abstract/
--rw-r--r--   0 caltaluc   (501) staff       (20)       92 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/resources/abstract/__init__.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     7648 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/resources/abstract/creatable_io_resource.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     1715 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/resources/abstract/io_resource.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.746732 kognic-io-1.1.8/kognic/io/resources/annotation/
--rw-r--r--   0 caltaluc   (501) staff       (20)     2385 2023-02-22 13:48:35.000000 kognic-io-1.1.8/kognic/io/resources/annotation/annotation.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.746886 kognic-io-1.1.8/kognic/io/resources/calibration/
--rw-r--r--   0 caltaluc   (501) staff       (20)     2111 2023-03-14 21:07:37.000000 kognic-io-1.1.8/kognic/io/resources/calibration/calibration.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.748735 kognic-io-1.1.8/kognic/io/resources/input/
--rw-r--r--   0 caltaluc   (501) staff       (20)     2487 2023-02-22 13:48:35.000000 kognic-io-1.1.8/kognic/io/resources/input/aggregated_lidars_and_cameras_seq.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     2135 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/resources/input/cameras.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     2318 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/resources/input/cameras_sequence.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     2581 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/resources/input/file_data.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     3681 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/resources/input/input.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     2174 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/resources/input/lidars.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     2349 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/resources/input/lidars_and_cameras.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     2394 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/resources/input/lidars_and_cameras_sequence.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     2261 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/resources/input/lidars_sequence.py
--rw-r--r--   0 caltaluc   (501) staff       (20)     1201 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/resources/input/pre_annotation.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.748902 kognic-io-1.1.8/kognic/io/resources/project/
--rw-r--r--   0 caltaluc   (501) staff       (20)     2684 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/resources/project/project.py
--rw-r--r--   0 caltaluc   (501) staff       (20)      954 2022-11-30 23:08:46.000000 kognic-io-1.1.8/kognic/io/util.py
-drwxr-xr-x   0 caltaluc   (501) staff       (20)        0 2023-03-17 10:22:51.749876 kognic-io-1.1.8/kognic_io.egg-info/
--rw-r--r--   0 caltaluc   (501) staff       (20)    18058 2023-03-17 10:22:51.000000 kognic-io-1.1.8/kognic_io.egg-info/PKG-INFO
--rw-r--r--   0 caltaluc   (501) staff       (20)     4172 2023-03-17 10:22:51.000000 kognic-io-1.1.8/kognic_io.egg-info/SOURCES.txt
--rw-r--r--   0 caltaluc   (501) staff       (20)        1 2023-03-17 10:22:51.000000 kognic-io-1.1.8/kognic_io.egg-info/dependency_links.txt
--rw-r--r--   0 caltaluc   (501) staff       (20)        7 2023-03-17 10:22:51.000000 kognic-io-1.1.8/kognic_io.egg-info/namespace_packages.txt
--rw-r--r--   0 caltaluc   (501) staff       (20)      183 2023-03-17 10:22:51.000000 kognic-io-1.1.8/kognic_io.egg-info/requires.txt
--rw-r--r--   0 caltaluc   (501) staff       (20)        7 2023-03-17 10:22:51.000000 kognic-io-1.1.8/kognic_io.egg-info/top_level.txt
--rw-r--r--   0 caltaluc   (501) staff       (20)       38 2023-03-17 10:22:51.750759 kognic-io-1.1.8/setup.cfg
--rw-r--r--   0 caltaluc   (501) staff       (20)     1851 2022-11-30 23:08:46.000000 kognic-io-1.1.8/setup.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.190501 kognic-io-1.1.9/
+-rw-r--r--   0 oskarolin   (501) staff       (20)    18319 2023-04-12 12:52:31.190212 kognic-io-1.1.9/PKG-INFO
+-rw-r--r--   0 oskarolin   (501) staff       (20)    17737 2023-04-12 12:47:31.000000 kognic-io-1.1.9/README.md
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.153558 kognic-io-1.1.9/bin/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      110 2023-01-20 14:42:20.000000 kognic-io-1.1.9/bin/kognicutil
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.148788 kognic-io-1.1.9/kognic/
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.156070 kognic-io-1.1.9/kognic/io/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      125 2023-04-12 12:47:31.000000 kognic-io-1.1.9/kognic/io/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     3588 2023-04-11 11:15:49.000000 kognic-io-1.1.9/kognic/io/client.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     5527 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/kognicutil.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      797 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/logger.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.158892 kognic-io-1.1.9/kognic/io/model/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      197 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/__init__.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.160146 kognic-io-1.1.9/kognic/io/model/annotation/
+-rw-r--r--   0 oskarolin   (501) staff       (20)       87 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/annotation/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      593 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/annotation/client_annotation.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      437 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/base_serializer.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.161381 kognic-io-1.1.9/kognic/io/model/calibration/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      295 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/calibration/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     2392 2023-04-12 12:47:31.000000 kognic-io-1.1.9/kognic/io/model/calibration/calib.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.163819 kognic-io-1.1.9/kognic/io/model/calibration/camera/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      500 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/calibration/camera/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      485 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/calibration/camera/common.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      333 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/calibration/camera/fisheye_calibration.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      547 2023-04-12 12:47:31.000000 kognic-io-1.1.9/kognic/io/model/calibration/camera/fused_cylindrical_calibration.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      634 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/calibration/camera/kannala_calibration.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      319 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/calibration/camera/pinhole_calibration.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     1072 2023-04-12 12:47:31.000000 kognic-io-1.1.9/kognic/io/model/calibration/camera/principal_point_distortion_calibration.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      584 2023-04-12 12:47:31.000000 kognic-io-1.1.9/kognic/io/model/calibration/common.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.164411 kognic-io-1.1.9/kognic/io/model/calibration/lidar/
+-rw-r--r--   0 oskarolin   (501) staff       (20)       99 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/calibration/lidar/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      438 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/calibration/lidar/lidar_calibration.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.166411 kognic-io-1.1.9/kognic/io/model/ego/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      166 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/ego/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      483 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/ego/imu_data.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)       70 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/ego/utils.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      444 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/ego/validated_imu_data.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      320 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/ego/vehicle_pose.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      222 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/files_to_upload.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.170195 kognic-io-1.1.9/kognic/io/model/input/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      358 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/__init__.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.171943 kognic-io-1.1.9/kognic/io/model/input/abstract/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      101 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/abstract/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      428 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/abstract/base_frame.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      406 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/abstract/base_input.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      528 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/abstract/base_input_with_imu_data.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      273 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/abstract/sequence_frame.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.172948 kognic-io-1.1.9/kognic/io/model/input/aggregated_lidars_and_cameras_seq/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      216 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/aggregated_lidars_and_cameras_seq/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      870 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/aggregated_lidars_and_cameras_seq/aggregated_lidars_and_cameras_seq.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      844 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/aggregated_lidars_and_cameras_seq/frame.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.173875 kognic-io-1.1.9/kognic/io/model/input/cameras/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      112 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/cameras/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      602 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/cameras/cameras.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      322 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/cameras/frame.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.174929 kognic-io-1.1.9/kognic/io/model/input/cameras_sequence/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      147 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/cameras_sequence/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      784 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/cameras_sequence/cameras_sequence.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      466 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/cameras_sequence/frame.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     1052 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/feature_flags.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      121 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/initialized_input.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      862 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/input_entry.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      235 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/input_from_scene_request.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      553 2023-02-14 15:24:24.000000 kognic-io-1.1.9/kognic/io/model/input/input_job.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      173 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/invalidated_reason_input.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.175932 kognic-io-1.1.9/kognic/io/model/input/lidars/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      108 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/lidars/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      462 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/lidars/frame.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      457 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/lidars/lidars.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.176908 kognic-io-1.1.9/kognic/io/model/input/lidars_and_cameras/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      154 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/lidars_and_cameras/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      664 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/lidars_and_cameras/frame.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      672 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/lidars_and_cameras/lidars_and_cameras.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.177876 kognic-io-1.1.9/kognic/io/model/input/lidars_and_cameras_sequence/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      189 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/lidars_and_cameras_sequence/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      861 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/lidars_and_cameras_sequence/frame.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      854 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/lidars_and_cameras_sequence/lidars_and_cameras_sequence.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.178866 kognic-io-1.1.9/kognic/io/model/input/lidars_sequence/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      143 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/lidars_sequence/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      570 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/lidars_sequence/frame.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      639 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/lidars_sequence/lidars_sequence.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.179255 kognic-io-1.1.9/kognic/io/model/input/metadata/
+-rw-r--r--   0 oskarolin   (501) staff       (20)     1425 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/metadata/metadata.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.180812 kognic-io-1.1.9/kognic/io/model/input/resources/
+-rw-r--r--   0 oskarolin   (501) staff       (20)      115 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/resources/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      646 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/resources/image.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      488 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/resources/point_cloud.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     2166 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/resources/resource.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      345 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/resources/video.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      320 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/input/sensor_specification.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.181899 kognic-io-1.1.9/kognic/io/model/projects/
+-rw-r--r--   0 oskarolin   (501) staff       (20)       89 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/projects/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      250 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/projects/project.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      458 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/projects/project_batch.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      247 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/model/upload_url.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.152440 kognic-io-1.1.9/kognic/io/resources/
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.183065 kognic-io-1.1.9/kognic/io/resources/abstract/
+-rw-r--r--   0 oskarolin   (501) staff       (20)       92 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/resources/abstract/__init__.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     7648 2023-02-14 15:24:24.000000 kognic-io-1.1.9/kognic/io/resources/abstract/creatable_io_resource.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     1715 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/resources/abstract/io_resource.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.183640 kognic-io-1.1.9/kognic/io/resources/annotation/
+-rw-r--r--   0 oskarolin   (501) staff       (20)     2385 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/resources/annotation/annotation.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.183945 kognic-io-1.1.9/kognic/io/resources/calibration/
+-rw-r--r--   0 oskarolin   (501) staff       (20)     2111 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/resources/calibration/calibration.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.187694 kognic-io-1.1.9/kognic/io/resources/input/
+-rw-r--r--   0 oskarolin   (501) staff       (20)     2487 2023-02-14 15:24:24.000000 kognic-io-1.1.9/kognic/io/resources/input/aggregated_lidars_and_cameras_seq.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     2135 2023-02-14 15:24:24.000000 kognic-io-1.1.9/kognic/io/resources/input/cameras.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     2318 2023-02-14 15:24:24.000000 kognic-io-1.1.9/kognic/io/resources/input/cameras_sequence.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     2581 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/resources/input/file_data.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     3681 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/resources/input/input.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     2174 2023-02-14 15:24:24.000000 kognic-io-1.1.9/kognic/io/resources/input/lidars.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     2349 2023-02-14 15:24:24.000000 kognic-io-1.1.9/kognic/io/resources/input/lidars_and_cameras.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     2394 2023-02-14 15:24:24.000000 kognic-io-1.1.9/kognic/io/resources/input/lidars_and_cameras_sequence.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     2261 2023-02-14 15:24:24.000000 kognic-io-1.1.9/kognic/io/resources/input/lidars_sequence.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     1201 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/resources/input/pre_annotation.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.188000 kognic-io-1.1.9/kognic/io/resources/project/
+-rw-r--r--   0 oskarolin   (501) staff       (20)     2684 2023-01-20 14:42:20.000000 kognic-io-1.1.9/kognic/io/resources/project/project.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.188508 kognic-io-1.1.9/kognic/io/tools/
+-rw-r--r--   0 oskarolin   (501) staff       (20)     8385 2023-04-12 12:47:31.000000 kognic-io-1.1.9/kognic/io/tools/input_creation.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)     1733 2023-04-12 12:47:31.000000 kognic-io-1.1.9/kognic/io/tools/model.py
+-rw-r--r--   0 oskarolin   (501) staff       (20)      954 2023-03-20 10:06:28.000000 kognic-io-1.1.9/kognic/io/util.py
+drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2023-04-12 12:52:31.189790 kognic-io-1.1.9/kognic_io.egg-info/
+-rw-r--r--   0 oskarolin   (501) staff       (20)    18319 2023-04-12 12:52:31.000000 kognic-io-1.1.9/kognic_io.egg-info/PKG-INFO
+-rw-r--r--   0 oskarolin   (501) staff       (20)     4231 2023-04-12 12:52:31.000000 kognic-io-1.1.9/kognic_io.egg-info/SOURCES.txt
+-rw-r--r--   0 oskarolin   (501) staff       (20)        1 2023-04-12 12:52:31.000000 kognic-io-1.1.9/kognic_io.egg-info/dependency_links.txt
+-rw-r--r--   0 oskarolin   (501) staff       (20)        7 2023-04-12 12:52:31.000000 kognic-io-1.1.9/kognic_io.egg-info/namespace_packages.txt
+-rw-r--r--   0 oskarolin   (501) staff       (20)      188 2023-04-12 12:52:31.000000 kognic-io-1.1.9/kognic_io.egg-info/requires.txt
+-rw-r--r--   0 oskarolin   (501) staff       (20)        7 2023-04-12 12:52:31.000000 kognic-io-1.1.9/kognic_io.egg-info/top_level.txt
+-rw-r--r--   0 oskarolin   (501) staff       (20)       38 2023-04-12 12:52:31.190575 kognic-io-1.1.9/setup.cfg
+-rw-r--r--   0 oskarolin   (501) staff       (20)     1867 2023-04-12 12:47:31.000000 kognic-io-1.1.9/setup.py
```

### Comparing `kognic-io-1.1.8/PKG-INFO` & `kognic-io-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kognic-io
-Version: 1.1.8
+Version: 1.1.9
 Summary: Kognic IO Client
 Home-page: https://github.com/annotell/annotell-python
-Download-URL: https://github.com/annotell/annotell-python/tarball/1.1.8
+Download-URL: https://github.com/annotell/annotell-python/tarball/1.1.9
 Author: Kognic
 Author-email: Team Scenes & Predictions <scenes-and-predictions@kognic.com>
 License: MIT
 Keywords: API,Kognic
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -25,14 +25,20 @@
 
 Documentation about how to use the library can be found [here](https://developers.kognic.com/)
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [1.1.9] - 2023-04-12
+
+### Added
+
+- Wrapper function `create_inputs` that allows creation of multiple inputs (with or without a pre-annotation) with a single call. This is useful since it contains wait-logic for the scene to be ready before creating inputs.
+
 ## [1.1.8] - 2023-03-17
 
 ### Added
 
 - Support for custom lens projection coefficients for Principal Point Distortion model. 
 
 ## [1.1.6] - 2023-03-14
```

### Comparing `kognic-io-1.1.8/README.md` & `kognic-io-1.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 
 Documentation about how to use the library can be found [here](https://developers.kognic.com/)
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [1.1.9] - 2023-04-12
+
+### Added
+
+- Wrapper function `create_inputs` that allows creation of multiple inputs (with or without a pre-annotation) with a single call. This is useful since it contains wait-logic for the scene to be ready before creating inputs.
+
 ## [1.1.8] - 2023-03-17
 
 ### Added
 
 - Support for custom lens projection coefficients for Principal Point Distortion model. 
 
 ## [1.1.6] - 2023-03-14
```

### Comparing `kognic-io-1.1.8/kognic/io/client.py` & `kognic-io-1.1.9/kognic/io/client.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/kognicutil.py` & `kognic-io-1.1.9/kognic/io/kognicutil.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/logger.py` & `kognic-io-1.1.9/kognic/io/logger.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/annotation/client_annotation.py` & `kognic-io-1.1.9/kognic/io/model/annotation/client_annotation.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/calibration/calib.py` & `kognic-io-1.1.9/kognic/io/model/calibration/calib.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/calibration/camera/fused_cylindrical_calibration.py` & `kognic-io-1.1.9/kognic/io/model/calibration/camera/fused_cylindrical_calibration.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/calibration/camera/kannala_calibration.py` & `kognic-io-1.1.9/kognic/io/model/calibration/camera/kannala_calibration.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/calibration/camera/principal_point_distortion_calibration.py` & `kognic-io-1.1.9/kognic/io/model/calibration/camera/principal_point_distortion_calibration.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/calibration/common.py` & `kognic-io-1.1.9/kognic/io/model/calibration/common.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/abstract/base_input_with_imu_data.py` & `kognic-io-1.1.9/kognic/io/model/input/abstract/base_input_with_imu_data.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/aggregated_lidars_and_cameras_seq/aggregated_lidars_and_cameras_seq.py` & `kognic-io-1.1.9/kognic/io/model/input/aggregated_lidars_and_cameras_seq/aggregated_lidars_and_cameras_seq.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/aggregated_lidars_and_cameras_seq/frame.py` & `kognic-io-1.1.9/kognic/io/model/input/aggregated_lidars_and_cameras_seq/frame.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/cameras/cameras.py` & `kognic-io-1.1.9/kognic/io/model/input/cameras/cameras.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/cameras_sequence/cameras_sequence.py` & `kognic-io-1.1.9/kognic/io/model/input/cameras_sequence/cameras_sequence.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/feature_flags.py` & `kognic-io-1.1.9/kognic/io/model/input/feature_flags.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/input_entry.py` & `kognic-io-1.1.9/kognic/io/model/input/input_entry.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/input_job.py` & `kognic-io-1.1.9/kognic/io/model/input/input_job.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/lidars_and_cameras/frame.py` & `kognic-io-1.1.9/kognic/io/model/input/lidars_and_cameras/frame.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/lidars_and_cameras/lidars_and_cameras.py` & `kognic-io-1.1.9/kognic/io/model/input/lidars_and_cameras/lidars_and_cameras.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/lidars_and_cameras_sequence/frame.py` & `kognic-io-1.1.9/kognic/io/model/input/lidars_and_cameras_sequence/frame.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/lidars_and_cameras_sequence/lidars_and_cameras_sequence.py` & `kognic-io-1.1.9/kognic/io/model/input/lidars_and_cameras_sequence/lidars_and_cameras_sequence.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/lidars_sequence/frame.py` & `kognic-io-1.1.9/kognic/io/model/input/lidars_sequence/frame.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/lidars_sequence/lidars_sequence.py` & `kognic-io-1.1.9/kognic/io/model/input/lidars_sequence/lidars_sequence.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/metadata/metadata.py` & `kognic-io-1.1.9/kognic/io/model/input/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/resources/image.py` & `kognic-io-1.1.9/kognic/io/model/input/resources/image.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/model/input/resources/resource.py` & `kognic-io-1.1.9/kognic/io/model/input/resources/resource.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/abstract/creatable_io_resource.py` & `kognic-io-1.1.9/kognic/io/resources/abstract/creatable_io_resource.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/abstract/io_resource.py` & `kognic-io-1.1.9/kognic/io/resources/abstract/io_resource.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/annotation/annotation.py` & `kognic-io-1.1.9/kognic/io/resources/annotation/annotation.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/calibration/calibration.py` & `kognic-io-1.1.9/kognic/io/resources/calibration/calibration.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/input/aggregated_lidars_and_cameras_seq.py` & `kognic-io-1.1.9/kognic/io/resources/input/aggregated_lidars_and_cameras_seq.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/input/cameras.py` & `kognic-io-1.1.9/kognic/io/resources/input/cameras.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/input/cameras_sequence.py` & `kognic-io-1.1.9/kognic/io/resources/input/cameras_sequence.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/input/file_data.py` & `kognic-io-1.1.9/kognic/io/resources/input/file_data.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/input/input.py` & `kognic-io-1.1.9/kognic/io/resources/input/input.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/input/lidars.py` & `kognic-io-1.1.9/kognic/io/resources/input/lidars.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/input/lidars_and_cameras.py` & `kognic-io-1.1.9/kognic/io/resources/input/lidars_and_cameras.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/input/lidars_and_cameras_sequence.py` & `kognic-io-1.1.9/kognic/io/resources/input/lidars_and_cameras_sequence.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/input/lidars_sequence.py` & `kognic-io-1.1.9/kognic/io/resources/input/lidars_sequence.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/input/pre_annotation.py` & `kognic-io-1.1.9/kognic/io/resources/input/pre_annotation.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/resources/project/project.py` & `kognic-io-1.1.9/kognic/io/resources/project/project.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic/io/util.py` & `kognic-io-1.1.9/kognic/io/util.py`

 * *Files identical despite different names*

### Comparing `kognic-io-1.1.8/kognic_io.egg-info/PKG-INFO` & `kognic-io-1.1.9/kognic_io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kognic-io
-Version: 1.1.8
+Version: 1.1.9
 Summary: Kognic IO Client
 Home-page: https://github.com/annotell/annotell-python
-Download-URL: https://github.com/annotell/annotell-python/tarball/1.1.8
+Download-URL: https://github.com/annotell/annotell-python/tarball/1.1.9
 Author: Kognic
 Author-email: Team Scenes & Predictions <scenes-and-predictions@kognic.com>
 License: MIT
 Keywords: API,Kognic
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -25,14 +25,20 @@
 
 Documentation about how to use the library can be found [here](https://developers.kognic.com/)
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [1.1.9] - 2023-04-12
+
+### Added
+
+- Wrapper function `create_inputs` that allows creation of multiple inputs (with or without a pre-annotation) with a single call. This is useful since it contains wait-logic for the scene to be ready before creating inputs.
+
 ## [1.1.8] - 2023-03-17
 
 ### Added
 
 - Support for custom lens projection coefficients for Principal Point Distortion model. 
 
 ## [1.1.6] - 2023-03-14
```

### Comparing `kognic-io-1.1.8/kognic_io.egg-info/SOURCES.txt` & `kognic-io-1.1.9/kognic_io.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -84,13 +84,15 @@
 kognic/io/resources/input/input.py
 kognic/io/resources/input/lidars.py
 kognic/io/resources/input/lidars_and_cameras.py
 kognic/io/resources/input/lidars_and_cameras_sequence.py
 kognic/io/resources/input/lidars_sequence.py
 kognic/io/resources/input/pre_annotation.py
 kognic/io/resources/project/project.py
+kognic/io/tools/input_creation.py
+kognic/io/tools/model.py
 kognic_io.egg-info/PKG-INFO
 kognic_io.egg-info/SOURCES.txt
 kognic_io.egg-info/dependency_links.txt
 kognic_io.egg-info/namespace_packages.txt
 kognic_io.egg-info/requires.txt
 kognic_io.egg-info/top_level.txt
```

### Comparing `kognic-io-1.1.8/setup.py` & `kognic-io-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         'click>=7.1.1',
         'Pillow>=7.0.0',
         'requests>=2.23.0',
         'tabulate>=0.8.7',
         'python-dateutil',
         "pydantic",
         "pyhumps",
-        "Deprecated"
+        "Deprecated",
+        "tqdm"
     ],
     python_requires='>=3.7',
     include_package_data=True,
     package_data={
         '': ['*.md', 'LICENSE'],
     },
     classifiers=[
```

