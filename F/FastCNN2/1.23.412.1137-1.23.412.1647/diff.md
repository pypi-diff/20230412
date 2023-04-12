# Comparing `tmp/FastCNN2-1.23.412.1137.tar.gz` & `tmp/FastCNN2-1.23.412.1647.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FastCNN2-1.23.412.1137.tar", last modified: Wed Apr 12 03:37:52 2023, max compression
+gzip compressed data, was "dist\FastCNN2-1.23.412.1647.tar", last modified: Wed Apr 12 08:47:37 2023, max compression
```

## Comparing `FastCNN2-1.23.412.1137.tar` & `FastCNN2-1.23.412.1647.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/
-drwxrwxrwx   0        0        0        0 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN/
-drwxrwxrwx   0        0        0        0 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN/api/
--rw-rw-rw-   0        0        0     5922 2022-07-25 09:49:16.000000 FastCNN2-1.23.412.1137/FastCNN/api/camera_.py
--rw-rw-rw-   0        0        0     2527 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/api/fastcnn_.py
--rw-rw-rw-   0        0        0     4866 2022-06-02 00:26:53.000000 FastCNN2-1.23.412.1137/FastCNN/api/pytorchfastcnn_.py
-drwxrwxrwx   0        0        0        0 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN/datasets/
--rw-rw-rw-   0        0        0     4588 2022-06-01 11:01:02.000000 FastCNN2-1.23.412.1137/FastCNN/datasets/fastcsv.py
-drwxrwxrwx   0        0        0        0 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN/entry/
--rw-rw-rw-   0        0        0      943 2022-07-13 02:13:51.000000 FastCNN2-1.23.412.1137/FastCNN/entry/camera.py
--rw-rw-rw-   0        0        0     3133 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/entry/gongda.py
--rw-rw-rw-   0        0        0      143 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/entry/intergrate.py
--rw-rw-rw-   0        0        0      987 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/entry/server.py
--rw-rw-rw-   0        0        0      951 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/entry/server2.py
--rw-rw-rw-   0        0        0     1354 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/entry/train.py
--rw-rw-rw-   0        0        0     1355 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/entry/train2.py
--rw-rw-rw-   0        0        0     1318 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/entry/trainvisiable.py
--rw-rw-rw-   0        0        0     1338 2022-06-01 12:50:39.000000 FastCNN2-1.23.412.1137/FastCNN/entry/trainyolov5.py
-drwxrwxrwx   0        0        0        0 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN/models/
--rw-rw-rw-   0        0        0    36119 2022-06-01 19:52:23.000000 FastCNN2-1.23.412.1137/FastCNN/models/common.py
--rw-rw-rw-   0        0        0     4238 2022-06-01 14:26:38.000000 FastCNN2-1.23.412.1137/FastCNN/models/experimental.py
--rw-rw-rw-   0        0        0    15741 2022-06-01 14:27:01.000000 FastCNN2-1.23.412.1137/FastCNN/models/yolo.py
-drwxrwxrwx   0        0        0        0 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN/nn/
--rw-rw-rw-   0        0        0     1925 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/nn/alexnet.py
--rw-rw-rw-   0        0        0     3697 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/nn/efficientnets.py
--rw-rw-rw-   0        0        0     4222 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1137/FastCNN/nn/experimental.py
--rw-rw-rw-   0        0        0     1128 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/nn/lenet.py
--rw-rw-rw-   0        0        0      777 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/nn/neuralnets.py
--rw-rw-rw-   0        0        0     1122 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/nn/standard.py
--rw-rw-rw-   0        0        0     3713 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/nn/torchnn.py
--rw-rw-rw-   0        0        0     4843 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/nn/vgg.py
--rw-rw-rw-   0        0        0    15693 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1137/FastCNN/nn/yolo.py
-drwxrwxrwx   0        0        0        0 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN/prx/
--rw-rw-rw-   0        0        0     2952 2022-07-27 06:32:53.000000 FastCNN2-1.23.412.1137/FastCNN/prx/CameraProxy.py
--rw-rw-rw-   0        0        0     1190 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/prx/DatasetProxy.py
--rw-rw-rw-   0        0        0    14401 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/prx/GongDaProxy.py
--rw-rw-rw-   0        0        0    14149 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/prx/GongDaProxy1.py
--rw-rw-rw-   0        0        0     6584 2022-07-14 02:49:05.000000 FastCNN2-1.23.412.1137/FastCNN/prx/PathProxy.py
--rw-rw-rw-   0        0        0     6100 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/prx/TrainProxy.py
--rw-rw-rw-   0        0        0     6484 2022-06-01 10:08:55.000000 FastCNN2-1.23.412.1137/FastCNN/prx/TrainProxy2.py
--rw-rw-rw-   0        0        0     7938 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/prx/ValidProxy.py
--rw-rw-rw-   0        0        0     4258 2023-04-12 03:37:13.000000 FastCNN2-1.23.412.1137/FastCNN/prx/ValidProxy2.py
--rw-rw-rw-   0        0        0    19317 2022-07-07 01:24:00.000000 FastCNN2-1.23.412.1137/FastCNN/prx/YoloV5DetectProxy.py
--rw-rw-rw-   0        0        0     2406 2022-06-01 12:39:44.000000 FastCNN2-1.23.412.1137/FastCNN/prx/YoloV5Proxy.py
--rw-rw-rw-   0        0        0    43732 2022-06-02 00:45:04.000000 FastCNN2-1.23.412.1137/FastCNN/prx/YoloV5TrainProxy.py
--rw-rw-rw-   0        0        0    20311 2022-06-01 17:08:57.000000 FastCNN2-1.23.412.1137/FastCNN/prx/YoloV5ValidProxy.py
--rw-rw-rw-   0        0        0    30570 2022-06-01 19:53:11.000000 FastCNN2-1.23.412.1137/FastCNN/prx/export.py
-drwxrwxrwx   0        0        0        0 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN/utils/
--rw-rw-rw-   0        0        0     8413 2022-06-01 18:18:09.000000 FastCNN2-1.23.412.1137/FastCNN/utils/CallBacks.py
--rw-rw-rw-   0        0        0     1542 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1137/FastCNN/utils/Logs.py
--rw-rw-rw-   0        0        0    12210 2022-06-01 12:08:37.000000 FastCNN2-1.23.412.1137/FastCNN/utils/augmentations.py
--rw-rw-rw-   0        0        0     7613 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1137/FastCNN/utils/autoanchor.py
--rw-rw-rw-   0        0        0     2256 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1137/FastCNN/utils/autobatch.py
--rw-rw-rw-   0        0        0    67782 2022-06-01 17:32:09.000000 FastCNN2-1.23.412.1137/FastCNN/utils/dataloaders.py
--rw-rw-rw-   0        0        0     7289 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1137/FastCNN/utils/downloads.py
--rw-rw-rw-   0        0        0    42735 2022-06-01 12:07:38.000000 FastCNN2-1.23.412.1137/FastCNN/utils/general.py
-drwxrwxrwx   0        0        0        0 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN/utils/loggers/
--rw-rw-rw-   0        0        0     8282 2023-04-12 03:37:24.000000 FastCNN2-1.23.412.1137/FastCNN/utils/loggers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN/utils/loggers/wandb/
--rw-rw-rw-   0        0        0       30 2023-04-12 03:37:24.000000 FastCNN2-1.23.412.1137/FastCNN/utils/loggers/wandb/__init__.py
--rw-rw-rw-   0        0        0     1059 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1137/FastCNN/utils/loggers/wandb/log_dataset.py
--rw-rw-rw-   0        0        0     1254 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1137/FastCNN/utils/loggers/wandb/sweep.py
--rw-rw-rw-   0        0        0    28163 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1137/FastCNN/utils/loggers/wandb/wandb_utils.py
--rw-rw-rw-   0        0        0    10145 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1137/FastCNN/utils/loss.py
--rw-rw-rw-   0        0        0    14716 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1137/FastCNN/utils/metrics.py
--rw-rw-rw-   0        0        0    21526 2022-06-01 12:09:58.000000 FastCNN2-1.23.412.1137/FastCNN/utils/plots.py
--rw-rw-rw-   0        0        0    13884 2022-06-01 12:09:30.000000 FastCNN2-1.23.412.1137/FastCNN/utils/torch_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN2.egg-info/
--rw-rw-rw-   0        0        0      219 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1740 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      309 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      123 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/FastCNN2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1082 2022-04-08 05:42:42.000000 FastCNN2-1.23.412.1137/LICENSE
--rw-rw-rw-   0        0        0      219 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/PKG-INFO
--rw-rw-rw-   0        0        0        2 2022-04-08 05:42:42.000000 FastCNN2-1.23.412.1137/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 03:37:52.000000 FastCNN2-1.23.412.1137/setup.cfg
--rw-rw-rw-   0        0        0     1530 2023-04-12 03:37:24.000000 FastCNN2-1.23.412.1137/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/
+drwxrwxrwx   0        0        0        0 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN/
+drwxrwxrwx   0        0        0        0 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN/api/
+-rw-rw-rw-   0        0        0     5922 2022-07-25 09:49:16.000000 FastCNN2-1.23.412.1647/FastCNN/api/camera_.py
+-rw-rw-rw-   0        0        0     2527 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/api/fastcnn_.py
+-rw-rw-rw-   0        0        0     4866 2022-06-02 00:26:53.000000 FastCNN2-1.23.412.1647/FastCNN/api/pytorchfastcnn_.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN/datasets/
+-rw-rw-rw-   0        0        0     4588 2022-06-01 11:01:02.000000 FastCNN2-1.23.412.1647/FastCNN/datasets/fastcsv.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN/entry/
+-rw-rw-rw-   0        0        0      943 2022-07-13 02:13:51.000000 FastCNN2-1.23.412.1647/FastCNN/entry/camera.py
+-rw-rw-rw-   0        0        0     3133 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/entry/gongda.py
+-rw-rw-rw-   0        0        0      143 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/entry/intergrate.py
+-rw-rw-rw-   0        0        0      987 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/entry/server.py
+-rw-rw-rw-   0        0        0      951 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/entry/server2.py
+-rw-rw-rw-   0        0        0     1354 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/entry/train.py
+-rw-rw-rw-   0        0        0     1355 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/entry/train2.py
+-rw-rw-rw-   0        0        0     1318 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/entry/trainvisiable.py
+-rw-rw-rw-   0        0        0     1338 2022-06-01 12:50:39.000000 FastCNN2-1.23.412.1647/FastCNN/entry/trainyolov5.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN/models/
+-rw-rw-rw-   0        0        0    36119 2022-06-01 19:52:23.000000 FastCNN2-1.23.412.1647/FastCNN/models/common.py
+-rw-rw-rw-   0        0        0     4238 2022-06-01 14:26:38.000000 FastCNN2-1.23.412.1647/FastCNN/models/experimental.py
+-rw-rw-rw-   0        0        0    15741 2022-06-01 14:27:01.000000 FastCNN2-1.23.412.1647/FastCNN/models/yolo.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN/nn/
+-rw-rw-rw-   0        0        0     1925 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/nn/alexnet.py
+-rw-rw-rw-   0        0        0     3697 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/nn/efficientnets.py
+-rw-rw-rw-   0        0        0     4222 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1647/FastCNN/nn/experimental.py
+-rw-rw-rw-   0        0        0     1128 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/nn/lenet.py
+-rw-rw-rw-   0        0        0      777 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/nn/neuralnets.py
+-rw-rw-rw-   0        0        0     1122 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/nn/standard.py
+-rw-rw-rw-   0        0        0     3713 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/nn/torchnn.py
+-rw-rw-rw-   0        0        0     4843 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/nn/vgg.py
+-rw-rw-rw-   0        0        0    15693 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1647/FastCNN/nn/yolo.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN/prx/
+-rw-rw-rw-   0        0        0     2952 2022-07-27 06:32:53.000000 FastCNN2-1.23.412.1647/FastCNN/prx/CameraProxy.py
+-rw-rw-rw-   0        0        0     1190 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/prx/DatasetProxy.py
+-rw-rw-rw-   0        0        0    14401 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/prx/GongDaProxy.py
+-rw-rw-rw-   0        0        0    14149 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/prx/GongDaProxy1.py
+-rw-rw-rw-   0        0        0     6584 2022-07-14 02:49:05.000000 FastCNN2-1.23.412.1647/FastCNN/prx/PathProxy.py
+-rw-rw-rw-   0        0        0     6100 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/prx/TrainProxy.py
+-rw-rw-rw-   0        0        0     6484 2022-06-01 10:08:55.000000 FastCNN2-1.23.412.1647/FastCNN/prx/TrainProxy2.py
+-rw-rw-rw-   0        0        0     7938 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/prx/ValidProxy.py
+-rw-rw-rw-   0        0        0     4574 2023-04-12 08:15:06.000000 FastCNN2-1.23.412.1647/FastCNN/prx/ValidProxy2.py
+-rw-rw-rw-   0        0        0    21036 2023-04-12 08:46:52.000000 FastCNN2-1.23.412.1647/FastCNN/prx/YoloV5DetectProxy.py
+-rw-rw-rw-   0        0        0     2406 2022-06-01 12:39:44.000000 FastCNN2-1.23.412.1647/FastCNN/prx/YoloV5Proxy.py
+-rw-rw-rw-   0        0        0    43732 2022-06-02 00:45:04.000000 FastCNN2-1.23.412.1647/FastCNN/prx/YoloV5TrainProxy.py
+-rw-rw-rw-   0        0        0    20311 2022-06-01 17:08:57.000000 FastCNN2-1.23.412.1647/FastCNN/prx/YoloV5ValidProxy.py
+-rw-rw-rw-   0        0        0    30570 2022-06-01 19:53:11.000000 FastCNN2-1.23.412.1647/FastCNN/prx/export.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN/utils/
+-rw-rw-rw-   0        0        0     8413 2022-06-01 18:18:09.000000 FastCNN2-1.23.412.1647/FastCNN/utils/CallBacks.py
+-rw-rw-rw-   0        0        0     1542 2022-06-01 09:36:12.000000 FastCNN2-1.23.412.1647/FastCNN/utils/Logs.py
+-rw-rw-rw-   0        0        0    12210 2022-06-01 12:08:37.000000 FastCNN2-1.23.412.1647/FastCNN/utils/augmentations.py
+-rw-rw-rw-   0        0        0     7613 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1647/FastCNN/utils/autoanchor.py
+-rw-rw-rw-   0        0        0     2256 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1647/FastCNN/utils/autobatch.py
+-rw-rw-rw-   0        0        0    67782 2022-06-01 17:32:09.000000 FastCNN2-1.23.412.1647/FastCNN/utils/dataloaders.py
+-rw-rw-rw-   0        0        0     7289 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1647/FastCNN/utils/downloads.py
+-rw-rw-rw-   0        0        0    42735 2022-06-01 12:07:38.000000 FastCNN2-1.23.412.1647/FastCNN/utils/general.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN/utils/loggers/
+-rw-rw-rw-   0        0        0     8282 2023-04-12 08:47:22.000000 FastCNN2-1.23.412.1647/FastCNN/utils/loggers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN/utils/loggers/wandb/
+-rw-rw-rw-   0        0        0       30 2023-04-12 08:47:22.000000 FastCNN2-1.23.412.1647/FastCNN/utils/loggers/wandb/__init__.py
+-rw-rw-rw-   0        0        0     1059 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1647/FastCNN/utils/loggers/wandb/log_dataset.py
+-rw-rw-rw-   0        0        0     1254 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1647/FastCNN/utils/loggers/wandb/sweep.py
+-rw-rw-rw-   0        0        0    28163 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1647/FastCNN/utils/loggers/wandb/wandb_utils.py
+-rw-rw-rw-   0        0        0    10145 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1647/FastCNN/utils/loss.py
+-rw-rw-rw-   0        0        0    14716 2022-05-28 09:10:50.000000 FastCNN2-1.23.412.1647/FastCNN/utils/metrics.py
+-rw-rw-rw-   0        0        0    21526 2022-06-01 12:09:58.000000 FastCNN2-1.23.412.1647/FastCNN/utils/plots.py
+-rw-rw-rw-   0        0        0    13884 2022-06-01 12:09:30.000000 FastCNN2-1.23.412.1647/FastCNN/utils/torch_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN2.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1740 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      309 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      123 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/FastCNN2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1082 2022-04-08 05:42:42.000000 FastCNN2-1.23.412.1647/LICENSE
+-rw-rw-rw-   0        0        0      219 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2022-04-08 05:42:42.000000 FastCNN2-1.23.412.1647/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 08:47:37.000000 FastCNN2-1.23.412.1647/setup.cfg
+-rw-rw-rw-   0        0        0     1530 2023-04-12 08:47:22.000000 FastCNN2-1.23.412.1647/setup.py
```

### Comparing `FastCNN2-1.23.412.1137/FastCNN/api/camera_.py` & `FastCNN2-1.23.412.1647/FastCNN/api/camera_.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/api/fastcnn_.py` & `FastCNN2-1.23.412.1647/FastCNN/api/fastcnn_.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/api/pytorchfastcnn_.py` & `FastCNN2-1.23.412.1647/FastCNN/api/pytorchfastcnn_.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/datasets/fastcsv.py` & `FastCNN2-1.23.412.1647/FastCNN/datasets/fastcsv.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/entry/camera.py` & `FastCNN2-1.23.412.1647/FastCNN/entry/camera.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/entry/gongda.py` & `FastCNN2-1.23.412.1647/FastCNN/entry/gongda.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/entry/server.py` & `FastCNN2-1.23.412.1647/FastCNN/entry/server.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/entry/server2.py` & `FastCNN2-1.23.412.1647/FastCNN/entry/server2.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/entry/train.py` & `FastCNN2-1.23.412.1647/FastCNN/entry/train.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/entry/train2.py` & `FastCNN2-1.23.412.1647/FastCNN/entry/train2.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/entry/trainvisiable.py` & `FastCNN2-1.23.412.1647/FastCNN/entry/trainvisiable.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/entry/trainyolov5.py` & `FastCNN2-1.23.412.1647/FastCNN/entry/trainyolov5.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/models/common.py` & `FastCNN2-1.23.412.1647/FastCNN/models/common.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/models/experimental.py` & `FastCNN2-1.23.412.1647/FastCNN/models/experimental.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/models/yolo.py` & `FastCNN2-1.23.412.1647/FastCNN/models/yolo.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/nn/alexnet.py` & `FastCNN2-1.23.412.1647/FastCNN/nn/alexnet.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/nn/efficientnets.py` & `FastCNN2-1.23.412.1647/FastCNN/nn/efficientnets.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/nn/experimental.py` & `FastCNN2-1.23.412.1647/FastCNN/nn/experimental.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/nn/lenet.py` & `FastCNN2-1.23.412.1647/FastCNN/nn/lenet.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/nn/neuralnets.py` & `FastCNN2-1.23.412.1647/FastCNN/nn/neuralnets.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/nn/standard.py` & `FastCNN2-1.23.412.1647/FastCNN/nn/standard.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/nn/torchnn.py` & `FastCNN2-1.23.412.1647/FastCNN/nn/torchnn.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/nn/vgg.py` & `FastCNN2-1.23.412.1647/FastCNN/nn/vgg.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/nn/yolo.py` & `FastCNN2-1.23.412.1647/FastCNN/nn/yolo.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/CameraProxy.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/CameraProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/DatasetProxy.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/DatasetProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/GongDaProxy.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/GongDaProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/GongDaProxy1.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/GongDaProxy1.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/PathProxy.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/PathProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/TrainProxy.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/TrainProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/TrainProxy2.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/TrainProxy2.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/ValidProxy.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/ValidProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/ValidProxy2.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/ValidProxy2.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,19 +19,24 @@
 
 from FastCNN.prx.YoloV5DetectProxy import _model as ymodel
 
 class DivValidObj:
     _model = None
     _labels = None
     _pre = None
+    _projid = ""
+    _modelid = ""
+    _busy = False
     
     def __init__(self):
         pass
     
     def setModel(self,projectid,modelid,mtype="valid"):
+        self._projid = projectid
+        self._modelid = modelid
         config = ValidProxy.getConfig(projectid,modelid)
         self._labels = config["LabelList"]
         
         net_name = config["Type"]
         
         net = getNeuralNet(net_name)
         net.initModel(len(self._labels))
@@ -47,14 +52,15 @@
             self._model = net.loadModel(valid_ckpt)
         else:
             raise Exception("unrecorgnised model type,you should try from 'train' or 'valid'")
         
         pass
     
     def predict(self,imgpath):
+        self._busy = True
         if self._model == None:
             raise Exception("Model has not initialed")
         s = time.time()
         img=Image.open(imgpath).convert('RGB')
     
         
         img = self._pre(img).unsqueeze(0).cuda()
@@ -70,16 +76,20 @@
         e = time.time()
         result = {
             "name":imgpath,
             "maybetype":ptype,
             "percent":str(round(percentage,3)),
             "spend":str(round(e-s,2))
             }
+        self._busy = False
         return result
     
+    def isTheModel(self,projectid,modelid):
+        return projectid == self._projid and modelid == self._modelid and (not _busy)
+    
     
 class ValidProxy:
     _div_ = []
     
     def __init__(self):
         pass
```

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/YoloV5DetectProxy.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/YoloV5DetectProxy.py`

 * *Files 9% similar despite different names*

```diff
@@ -272,28 +272,44 @@
             item = self.dePool()
         return item
     
     def getItems(self):
         return self.cs
     pass
 
+class ObjValidObj:
+    _model = None
+    _labels = None
+    _pre = None
+    _projid = ""
+    _modelid = ""
+    _busy = False
+    
+    def __init__(self,projectid,modelid,model)
+        self._projid = projectid
+        self._modelid = modelid
+        self._model = model
+        
+        pass
+
 class SelectModel:
     def __init__(self):
         
         #self._model = None
-        self._pool = ResourcePool([None,None,None,None])
+        #self._pool = ResourcePool([None,None,None,None])
+        self._pool = []
         pass
     
     def size(self):
         rtn = 0
         if self._model:
             rtn = sum([np.prod(list(p.size())) for p in self._model.parameters()]) *4/1000/1000
         return rtn
     
-    def loadModel(self,projectid,modelid):
+    def loadModel0(self,projectid,modelid):
         saver = PathProxy.getValidCKPT(projectid,modelid)[:-1]
         
         device = select_device("")
         #self._model = DetectMultiBackend(saver, device=device, dnn=False, data=False, fp16=False)
         p = []
         
         try:
@@ -301,23 +317,56 @@
                 md = DetectMultiBackend(saver, device=device, dnn=False, data=False, fp16=False)
                 p.append(md)
             
             self._pool = ResourcePool(p)
         except Exception as err:
             print(err)
     
+    def loadModel(self,projectid,modelid,clr = True):
+        saver = PathProxy.getValidCKPT(projectid,modelid)[:-1]
+        
+        device = select_device("")
+        #self._model = DetectMultiBackend(saver, device=device, dnn=False, data=False, fp16=False)
+        try:
+            md = DetectMultiBackend(saver, device=device, dnn=False, data=False, fp16=False)
+            o = ObjValidObj(projectid,modelid,md)
+            if clr:
+                self._pool.clear()
+            self._pool.append(o)
+        except Exception as err:
+            print(err)
+    
+    def loadModels(self,projmdls):
+        self._pool.clear()
+        for projectid,modelid in projmdls:
+            self.loadModel(projectid,modelid,False)
+        
+        pass
+    
     def getModel(self):
-        model = self._pool.dePoolAsync()
+        if len(self._pool) > 0:
+            model = self._pool[0]
         return model
     
-    def reModel(self,model):
-        self._pool.enPool(model)
-        pass
+    def getModelByID(self,projectid,modelid):
+        mdl = None
+        for m in self._pool:
+            if m._projid == projectid and m._modelid == modelid and (not _busy):
+                mdl = m
+                break
+        return mdl
+    
+    def predictByID(self,projectid,modelid,imgpath):
+        mdl = self.getModelByID(projectid,modelid)
+        if mdl != None:
+            return self.predictSingle(imgpath,mdl)
+        else:
+            raise Exception("No model setted projectid:{}-modelid:{}".format(projectid,modelid))
     
-    def predictSingle(self,imgpath):
+    def predictSingle(self,imgpath,modelobj = None):
         device = select_device("")
         
         imgsz=(640, 640)
         conf_thres=0.25
         iou_thres=0.45
         max_det=1000
         
@@ -326,18 +375,22 @@
         augment=False  # augmented inference
         visualize=False # visualize features
         
         line_thickness=3  # bounding box thickness (pixels)
         hide_labels=False  # hide labels
         hide_conf=False  # hide confidences
         
-        #model = self._model
-        model = self.getModel()
-        if not model:
+        if modelobj == None:
+            modelobj = self.getModel()
+            
+        if not modelobj:
             return None
+        model = modelobj._model
+        modelobj._busy = True
+        
         stride, names, pt = model.stride, model.names, model.pt
         imgsz = check_img_size(imgsz, s=stride)  # check image size
 
         rtn = {'results':""}
         dataset = LoadImages(imgpath, img_size=imgsz, stride=stride, auto=pt)
         bs = 1  # batch_size
         vid_path, vid_writer = [None] * bs, [None] * bs
@@ -416,15 +469,15 @@
                         for cor in xywh:
                             if len(rtn['results']) > 0:
                                 rtn['results'] += ","
                             
                             rtn['results'] += str(round(cor,2))
                         
             rtn["spend"] = dt[0]+dt[1]+dt[2]
-        self.reModel(model)
+        modelobj._busy = False
         return rtn
 
 _model = SelectModel()
 
 if __name__ == "__main__":
     #opt = parse_opt()
     #main(opt)
```

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/YoloV5Proxy.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/YoloV5Proxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/YoloV5TrainProxy.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/YoloV5TrainProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/YoloV5ValidProxy.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/YoloV5ValidProxy.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/prx/export.py` & `FastCNN2-1.23.412.1647/FastCNN/prx/export.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/CallBacks.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/CallBacks.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/Logs.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/Logs.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/augmentations.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/autoanchor.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/autobatch.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/dataloaders.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/downloads.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/general.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/general.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/loggers/__init__.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/loggers/wandb/log_dataset.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/loggers/wandb/log_dataset.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/loggers/wandb/sweep.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/loggers/wandb/sweep.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/loggers/wandb/wandb_utils.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/loggers/wandb/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/loss.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/loss.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/metrics.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/plots.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/plots.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN/utils/torch_utils.py` & `FastCNN2-1.23.412.1647/FastCNN/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/FastCNN2.egg-info/SOURCES.txt` & `FastCNN2-1.23.412.1647/FastCNN2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/LICENSE` & `FastCNN2-1.23.412.1647/LICENSE`

 * *Files identical despite different names*

### Comparing `FastCNN2-1.23.412.1137/setup.py` & `FastCNN2-1.23.412.1647/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 
 """
 set App Name
 """
 name = "FastCNN2"
-version = '1.23.0412.1137'
+version = '1.23.0412.1647'
 
 author = "Iuty"
 author_email = "dfdfggg@126.com"
 
 """
 set entry_points
 """
```

