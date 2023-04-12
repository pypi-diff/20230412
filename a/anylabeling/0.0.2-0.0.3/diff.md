# Comparing `tmp/anylabeling-0.0.2.tar.gz` & `tmp/anylabeling-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.0.2.tar", last modified: Tue Apr 11 18:27:41 2023, max compression
+gzip compressed data, was "anylabeling-0.0.3.tar", last modified: Wed Apr 12 01:16:45 2023, max compression
```

## Comparing `anylabeling-0.0.2.tar` & `anylabeling-0.0.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.274711 anylabeling-0.0.2/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.0.2/LICENSE
--rw-r--r--   0 vietanhdev   (501) staff       (20)      120 2023-04-08 18:53:13.000000 anylabeling-0.0.2/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2039 2023-04-11 18:27:41.274552 anylabeling-0.0.2/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1153 2023-04-11 17:52:02.000000 anylabeling-0.0.2/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.262849 anylabeling-0.0.2/anylabeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       22 2023-04-11 18:19:13.000000 anylabeling-0.0.2/anylabeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1062 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/app.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.264833 anylabeling-0.0.2/anylabeling/configs/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/configs/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.264981 anylabeling-0.0.2/anylabeling/configs/__pycache__/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.0.2/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/configs/anylabeling_config.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)      315 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/configs/autolabel_segment_anything.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/configs/autolabel_yolov5m.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/configs/autolabel_yolov5s.yaml
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.265213 anylabeling-0.0.2/anylabeling/resources/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/resources/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)   423402 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/resources/resources.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.266562 anylabeling-0.0.2/anylabeling/services/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/services/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.267300 anylabeling-0.0.2/anylabeling/services/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2955 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5277 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9837 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1284 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5127 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/utils.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.267918 anylabeling-0.0.2/anylabeling/views/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/views/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.268486 anylabeling-0.0.2/anylabeling/views/common/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/views/common/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/views/common/tableview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.270836 anylabeling-0.0.2/anylabeling/views/labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      343 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5758 2023-04-08 20:04:23.000000 anylabeling-0.0.2/anylabeling/views/labeling/__main__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2717 2023-04-09 06:42:35.000000 anylabeling-0.0.2/anylabeling/views/labeling/config.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6405 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    88768 2023-04-11 18:18:40.000000 anylabeling-0.0.2/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      606 2023-04-08 20:07:28.000000 anylabeling-0.0.2/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1811 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/logger.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/shape.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.271873 anylabeling-0.0.2/anylabeling/views/labeling/utils/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.273915 anylabeling-0.0.2/anylabeling/views/labeling/widgets/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.274338 anylabeling-0.0.2/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6906 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    46264 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8023 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5778 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1390 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      768 2023-04-08 20:09:45.000000 anylabeling-0.0.2/anylabeling/views/maintabs.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      981 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/mainwindow.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1458 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/mainwindow_tabs.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.264124 anylabeling-0.0.2/anylabeling.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2039 2023-04-11 18:27:41.000000 anylabeling-0.0.2/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2620 2023-04-11 18:27:41.000000 anylabeling-0.0.2/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-11 18:27:41.000000 anylabeling-0.0.2/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-11 18:27:41.000000 anylabeling-0.0.2/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      235 2023-04-11 18:27:41.000000 anylabeling-0.0.2/anylabeling.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-11 18:27:41.000000 anylabeling-0.0.2/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.0.2/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-11 18:27:41.274754 anylabeling-0.0.2/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2503 2023-04-11 17:52:02.000000 anylabeling-0.0.2/setup.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.298288 anylabeling-0.0.3/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.0.3/LICENSE
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      120 2023-04-08 18:53:13.000000 anylabeling-0.0.3/MANIFEST.in
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2807 2023-04-12 01:16:45.298109 anylabeling-0.0.3/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.0.3/README.md
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.288836 anylabeling-0.0.3/anylabeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       22 2023-04-12 01:16:35.000000 anylabeling-0.0.3/anylabeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1062 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/app.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.290269 anylabeling-0.0.3/anylabeling/configs/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/configs/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.290391 anylabeling-0.0.3/anylabeling/configs/__pycache__/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.0.3/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/configs/anylabeling_config.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      315 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/configs/autolabel_segment_anything.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/configs/autolabel_yolov5m.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/configs/autolabel_yolov5s.yaml
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.290844 anylabeling-0.0.3/anylabeling/resources/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/resources/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   423402 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/resources/resources.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.291566 anylabeling-0.0.3/anylabeling/services/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/services/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.292309 anylabeling-0.0.3/anylabeling/services/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2955 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5277 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9837 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1284 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5127 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/utils.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.292783 anylabeling-0.0.3/anylabeling/views/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/views/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.293158 anylabeling-0.0.3/anylabeling/views/common/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/views/common/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/views/common/tableview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.294763 anylabeling-0.0.3/anylabeling/views/labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      343 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5758 2023-04-08 20:04:23.000000 anylabeling-0.0.3/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2717 2023-04-09 06:42:35.000000 anylabeling-0.0.3/anylabeling/views/labeling/config.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6405 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    88768 2023-04-11 18:18:40.000000 anylabeling-0.0.3/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      606 2023-04-08 20:07:28.000000 anylabeling-0.0.3/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1811 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.295667 anylabeling-0.0.3/anylabeling/views/labeling/utils/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.297301 anylabeling-0.0.3/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.297885 anylabeling-0.0.3/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6906 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    46264 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8023 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5778 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1390 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      768 2023-04-08 20:09:45.000000 anylabeling-0.0.3/anylabeling/views/maintabs.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      981 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/mainwindow.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1458 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/mainwindow_tabs.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.289682 anylabeling-0.0.3/anylabeling.egg-info/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2807 2023-04-12 01:16:45.000000 anylabeling-0.0.3/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2620 2023-04-12 01:16:45.000000 anylabeling-0.0.3/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-12 01:16:45.000000 anylabeling-0.0.3/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-12 01:16:45.000000 anylabeling-0.0.3/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      235 2023-04-12 01:16:45.000000 anylabeling-0.0.3/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-12 01:16:45.000000 anylabeling-0.0.3/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.0.3/pyproject.toml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-12 01:16:45.298336 anylabeling-0.0.3/setup.cfg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2503 2023-04-11 17:52:02.000000 anylabeling-0.0.3/setup.py
```

### Comparing `anylabeling-0.0.2/LICENSE` & `anylabeling-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/PKG-INFO` & `anylabeling-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 616e 796c  : 2.1.Name: anyl
 00000020: 6162 656c 696e 670a 5665 7273 696f 6e3a  abeling.Version:
-00000030: 2030 2e30 2e32 0a53 756d 6d61 7279 3a20   0.0.2.Summary: 
+00000030: 2030 2e30 2e33 0a53 756d 6d61 7279 3a20   0.0.3.Summary: 
 00000040: 4566 666f 7274 6c65 7373 2064 6174 6120  Effortless data 
 00000050: 6c61 6265 6c69 6e67 2077 6974 6820 4149  labeling with AI
 00000060: 2073 7570 706f 7274 0a48 6f6d 652d 7061   support.Home-pa
 00000070: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 00000080: 7562 2e63 6f6d 2f76 6965 7461 6e68 6465  ub.com/vietanhde
 00000090: 762f 616e 796c 6162 656c 696e 670a 4175  v/anylabeling.Au
 000000a0: 7468 6f72 3a20 5669 6574 2d41 6e68 204e  thor: Viet-Anh N
@@ -69,60 +69,108 @@
 00000440: 794c 6162 656c 696e 6720 3d20 4c61 6265  yLabeling = Labe
 00000450: 6c49 6d67 202b 204c 6162 656c 6d65 202b  lImg + Labelme +
 00000460: 2049 6d70 726f 7665 6420 5549 202b 2041   Improved UI + A
 00000470: 7574 6f2d 6c61 6265 6c69 6e67 3c2f 623e  uto-labeling</b>
 00000480: 3c70 3e0a 3c2f 703e 0a0a 215b 5d28 6874  <p>.</p>..![](ht
 00000490: 7470 733a 2f2f 692e 696d 6775 722e 636f  tps://i.imgur.co
 000004a0: 6d2f 7761 7856 496d 762e 706e 6729 0a0a  m/waxVImv.png)..
-000004b0: 0a23 2320 492e 2049 6e73 7461 6c6c 2061  .## I. Install a
-000004c0: 6e64 2072 756e 0a0a 2d20 5265 7175 6972  nd run..- Requir
-000004d0: 656d 656e 7473 3a20 5079 7468 6f6e 203e  ements: Python >
-000004e0: 3d20 332e 380a 2d20 5265 636f 6d6d 656e  = 3.8.- Recommen
-000004f0: 6465 643a 204d 696e 6963 6f6e 6461 2f41  ded: Miniconda/A
-00000500: 6e61 636f 6e64 6120 3c68 7474 7073 3a2f  naconda <https:/
-00000510: 2f64 6f63 732e 636f 6e64 612e 696f 2f65  /docs.conda.io/e
-00000520: 6e2f 6c61 7465 7374 2f6d 696e 6963 6f6e  n/latest/minicon
-00000530: 6461 2e68 746d 6c3e 0a0a 2d20 4372 6561  da.html>..- Crea
-00000540: 7465 2065 6e76 6972 6f6e 6d65 6e74 3a0a  te environment:.
-00000550: 0a60 6060 0a63 6f6e 6461 2063 7265 6174  .```.conda creat
-00000560: 6520 2d6e 2061 6e79 6c61 6265 6c69 6e67  e -n anylabeling
-00000570: 2070 7974 686f 6e3d 332e 380a 636f 6e64   python=3.8.cond
-00000580: 6120 6163 7469 7661 7465 2061 6e79 6c61  a activate anyla
-00000590: 6265 6c69 6e67 0a60 6060 0a0a 2d20 2a2a  beling.```..- **
-000005a0: 2846 6f72 206d 6163 4f53 206f 6e6c 7929  (For macOS only)
-000005b0: 2a2a 2049 6e73 7461 6c6c 2050 7951 7435  ** Install PyQt5
-000005c0: 2075 7369 6e67 2043 6f6e 6461 3a0a 0a60   using Conda:..`
-000005d0: 6060 0a63 6f6e 6461 2069 6e73 7461 6c6c  ``.conda install
-000005e0: 202d 6320 636f 6e64 612d 666f 7267 6520   -c conda-forge 
-000005f0: 7079 7174 3d3d 352e 3135 2e37 0a60 6060  pyqt==5.15.7.```
-00000600: 0a0a 2d20 496e 7374 616c 6c20 616e 796c  ..- Install anyl
-00000610: 6162 656c 696e 673a 0a0a 6060 600a 7069  abeling:..```.pi
-00000620: 7020 696e 7374 616c 6c20 616e 796c 6162  p install anylab
-00000630: 656c 696e 670a 6060 600a 0a2d 2052 756e  eling.```..- Run
-00000640: 2061 7070 3a0a 0a60 6060 0a61 6e79 6c61   app:..```.anyla
-00000650: 6265 6c69 6e67 0a60 6060 0a0a 4f72 0a0a  beling.```..Or..
-00000660: 6060 600a 7079 7468 6f6e 202d 6d20 616e  ```.python -m an
-00000670: 796c 6162 656c 696e 672e 6170 700a 6060  ylabeling.app.``
-00000680: 600a 0a23 2320 4949 2e20 4465 7665 6c6f  `..## II. Develo
-00000690: 706d 656e 740a 0a2d 2047 656e 6572 6174  pment..- Generat
-000006a0: 6520 7265 736f 7572 6365 733a 0a0a 6060  e resources:..``
-000006b0: 600a 7079 7263 6335 202d 6f20 616e 796c  `.pyrcc5 -o anyl
-000006c0: 6162 656c 696e 672f 7265 736f 7572 6365  abeling/resource
-000006d0: 732f 7265 736f 7572 6365 732e 7079 2061  s/resources.py a
-000006e0: 6e79 6c61 6265 6c69 6e67 2f72 6573 6f75  nylabeling/resou
-000006f0: 7263 6573 2f72 6573 6f75 7263 6573 2e71  rces/resources.q
-00000700: 7263 0a60 6060 0a0a 2d20 5275 6e20 6170  rc.```..- Run ap
-00000710: 703a 0a0a 6060 600a 7079 7468 6f6e 2061  p:..```.python a
-00000720: 6e79 6c61 6265 6c69 6e67 2f61 7070 2e70  nylabeling/app.p
-00000730: 790a 6060 600a 0a23 2320 4949 492e 2052  y.```..## III. R
-00000740: 6566 6572 656e 6365 730a 0a2d 204c 6162  eferences..- Lab
-00000750: 656c 696e 6720 5549 2062 7569 6c74 2077  eling UI built w
-00000760: 6974 6820 6964 6561 7320 616e 6420 636f  ith ideas and co
-00000770: 6d70 6f6e 656e 7473 2066 726f 6d20 5b4c  mponents from [L
-00000780: 6162 656c 496d 675d 2868 7474 7073 3a2f  abelImg](https:/
-00000790: 2f67 6974 6875 622e 636f 6d2f 6865 6172  /github.com/hear
-000007a0: 7465 786c 6162 732f 6c61 6265 6c49 6d67  texlabs/labelImg
-000007b0: 292c 205b 6c61 6265 6c6d 655d 2868 7474  ), [labelme](htt
-000007c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000007d0: 776b 656e 7461 726f 2f6c 6162 656c 6d65  wkentaro/labelme
-000007e0: 292e 0a2d 2049 636f 6e73 3a20 466c 6174  )..- Icons: Flat
-000007f0: 2049 636f 6e73 0a                         Icons.
+000004b0: 5b21 5b50 7950 495d 2868 7474 7073 3a2f  [![PyPI](https:/
+000004c0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000004d0: 7079 7069 2f76 2f61 6e79 6c61 6265 6c69  pypi/v/anylabeli
+000004e0: 6e67 295d 2868 7474 7073 3a2f 2f70 7970  ng)](https://pyp
+000004f0: 692e 6f72 672f 7072 6f6a 6563 742f 616e  i.org/project/an
+00000500: 796c 6162 656c 696e 6729 0a5b 215b 6c69  ylabeling).[![li
+00000510: 6365 6e73 655d 2868 7474 7073 3a2f 2f69  cense](https://i
+00000520: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00000530: 7468 7562 2f6c 6963 656e 7365 2f76 6965  thub/license/vie
+00000540: 7461 6e68 6465 762f 616e 796c 6162 656c  tanhdev/anylabel
+00000550: 696e 672e 7376 6729 5d28 6874 7470 733a  ing.svg)](https:
+00000560: 2f2f 6769 7468 7562 2e63 6f6d 2f76 6965  //github.com/vie
+00000570: 7461 6e68 6465 762f 616e 796c 6162 656c  tanhdev/anylabel
+00000580: 696e 672f 626c 6f62 2f6d 6173 7465 722f  ing/blob/master/
+00000590: 4c49 4345 4e53 4529 0a5b 215b 6f70 656e  LICENSE).[![open
+000005a0: 2069 7373 7565 735d 2868 7474 7073 3a2f   issues](https:/
+000005b0: 2f69 7369 746d 6169 6e74 6169 6e65 642e  /isitmaintained.
+000005c0: 636f 6d2f 6261 6467 652f 6f70 656e 2f76  com/badge/open/v
+000005d0: 6965 7461 6e68 6465 762f 616e 796c 6162  ietanhdev/anylab
+000005e0: 656c 696e 672e 7376 6729 5d28 6874 7470  eling.svg)](http
+000005f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f76  s://github.com/v
+00000600: 6965 7461 6e68 6465 762f 616e 796c 6162  ietanhdev/anylab
+00000610: 656c 696e 672f 6973 7375 6573 290a 5b21  eling/issues).[!
+00000620: 5b50 7970 6920 446f 776e 6c6f 6164 735d  [Pypi Downloads]
+00000630: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
+00000640: 6368 2f62 6164 6765 2f61 6e79 6c61 6265  ch/badge/anylabe
+00000650: 6c69 6e67 295d 2868 7474 7073 3a2f 2f70  ling)](https://p
+00000660: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00000670: 616e 796c 6162 656c 696e 672f 290a 0a3c  anylabeling/)..<
+00000680: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000690: 7777 772e 796f 7574 7562 652e 636f 6d2f  www.youtube.com/
+000006a0: 7761 7463 683f 763d 3569 5153 474c 3765  watch?v=5iQSGL7e
+000006b0: 6258 4522 3e0a 2020 3c69 6d67 2061 6c74  bXE">.  <img alt
+000006c0: 3d22 416e 794c 6162 656c 696e 6722 2073  ="AnyLabeling" s
+000006d0: 7263 3d22 6874 7470 733a 2f2f 7573 6572  rc="https://user
+000006e0: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
+000006f0: 6572 636f 6e74 656e 742e 636f 6d2f 3138  ercontent.com/18
+00000700: 3332 3934 3731 2f32 3331 3332 3034 3838  329471/231320488
+00000710: 2d32 6638 3133 3362 632d 3662 3531 2d34  -2f8133bc-6b51-4
+00000720: 3866 382d 3832 6136 2d64 6433 6232 3637  8f8-82a6-dd3b267
+00000730: 6635 3135 362e 706e 6722 2f3e 0a3c 2f61  f5156.png"/>.</a
+00000740: 3e0a 0a2a 2a59 6f75 7475 6265 2044 656d  >..**Youtube Dem
+00000750: 6f3a 2a2a 205b 6874 7470 733a 2f2f 7777  o:** [https://ww
+00000760: 772e 796f 7574 7562 652e 636f 6d2f 7761  w.youtube.com/wa
+00000770: 7463 683f 763d 3569 5153 474c 3765 6258  tch?v=5iQSGL7ebX
+00000780: 455d 2868 7474 7073 3a2f 2f77 7777 2e79  E](https://www.y
+00000790: 6f75 7475 6265 2e63 6f6d 2f77 6174 6368  outube.com/watch
+000007a0: 3f76 3d35 6951 5347 4c37 6562 5845 290a  ?v=5iQSGL7ebXE).
+000007b0: 0a23 2320 492e 2049 6e73 7461 6c6c 2061  .## I. Install a
+000007c0: 6e64 2072 756e 0a0a 2d20 5265 7175 6972  nd run..- Requir
+000007d0: 656d 656e 7473 3a20 5079 7468 6f6e 203e  ements: Python >
+000007e0: 3d20 332e 380a 2d20 5265 636f 6d6d 656e  = 3.8.- Recommen
+000007f0: 6465 643a 204d 696e 6963 6f6e 6461 2f41  ded: Miniconda/A
+00000800: 6e61 636f 6e64 6120 3c68 7474 7073 3a2f  naconda <https:/
+00000810: 2f64 6f63 732e 636f 6e64 612e 696f 2f65  /docs.conda.io/e
+00000820: 6e2f 6c61 7465 7374 2f6d 696e 6963 6f6e  n/latest/minicon
+00000830: 6461 2e68 746d 6c3e 0a0a 2d20 4372 6561  da.html>..- Crea
+00000840: 7465 2065 6e76 6972 6f6e 6d65 6e74 3a0a  te environment:.
+00000850: 0a60 6060 0a63 6f6e 6461 2063 7265 6174  .```.conda creat
+00000860: 6520 2d6e 2061 6e79 6c61 6265 6c69 6e67  e -n anylabeling
+00000870: 2070 7974 686f 6e3d 332e 380a 636f 6e64   python=3.8.cond
+00000880: 6120 6163 7469 7661 7465 2061 6e79 6c61  a activate anyla
+00000890: 6265 6c69 6e67 0a60 6060 0a0a 2d20 2a2a  beling.```..- **
+000008a0: 2846 6f72 206d 6163 4f53 206f 6e6c 7929  (For macOS only)
+000008b0: 2a2a 2049 6e73 7461 6c6c 2050 7951 7435  ** Install PyQt5
+000008c0: 2075 7369 6e67 2043 6f6e 6461 3a0a 0a60   using Conda:..`
+000008d0: 6060 0a63 6f6e 6461 2069 6e73 7461 6c6c  ``.conda install
+000008e0: 202d 6320 636f 6e64 612d 666f 7267 6520   -c conda-forge 
+000008f0: 7079 7174 3d3d 352e 3135 2e37 0a60 6060  pyqt==5.15.7.```
+00000900: 0a0a 2d20 496e 7374 616c 6c20 616e 796c  ..- Install anyl
+00000910: 6162 656c 696e 673a 0a0a 6060 600a 7069  abeling:..```.pi
+00000920: 7020 696e 7374 616c 6c20 616e 796c 6162  p install anylab
+00000930: 656c 696e 670a 6060 600a 0a2d 2052 756e  eling.```..- Run
+00000940: 2061 7070 3a0a 0a60 6060 0a61 6e79 6c61   app:..```.anyla
+00000950: 6265 6c69 6e67 0a60 6060 0a0a 4f72 0a0a  beling.```..Or..
+00000960: 6060 600a 7079 7468 6f6e 202d 6d20 616e  ```.python -m an
+00000970: 796c 6162 656c 696e 672e 6170 700a 6060  ylabeling.app.``
+00000980: 600a 0a23 2320 4949 2e20 4465 7665 6c6f  `..## II. Develo
+00000990: 706d 656e 740a 0a2d 2047 656e 6572 6174  pment..- Generat
+000009a0: 6520 7265 736f 7572 6365 733a 0a0a 6060  e resources:..``
+000009b0: 600a 7079 7263 6335 202d 6f20 616e 796c  `.pyrcc5 -o anyl
+000009c0: 6162 656c 696e 672f 7265 736f 7572 6365  abeling/resource
+000009d0: 732f 7265 736f 7572 6365 732e 7079 2061  s/resources.py a
+000009e0: 6e79 6c61 6265 6c69 6e67 2f72 6573 6f75  nylabeling/resou
+000009f0: 7263 6573 2f72 6573 6f75 7263 6573 2e71  rces/resources.q
+00000a00: 7263 0a60 6060 0a0a 2d20 5275 6e20 6170  rc.```..- Run ap
+00000a10: 703a 0a0a 6060 600a 7079 7468 6f6e 2061  p:..```.python a
+00000a20: 6e79 6c61 6265 6c69 6e67 2f61 7070 2e70  nylabeling/app.p
+00000a30: 790a 6060 600a 0a23 2320 4949 492e 2052  y.```..## III. R
+00000a40: 6566 6572 656e 6365 730a 0a2d 204c 6162  eferences..- Lab
+00000a50: 656c 696e 6720 5549 2062 7569 6c74 2077  eling UI built w
+00000a60: 6974 6820 6964 6561 7320 616e 6420 636f  ith ideas and co
+00000a70: 6d70 6f6e 656e 7473 2066 726f 6d20 5b4c  mponents from [L
+00000a80: 6162 656c 496d 675d 2868 7474 7073 3a2f  abelImg](https:/
+00000a90: 2f67 6974 6875 622e 636f 6d2f 6865 6172  /github.com/hear
+00000aa0: 7465 786c 6162 732f 6c61 6265 6c49 6d67  texlabs/labelImg
+00000ab0: 292c 205b 6c61 6265 6c6d 655d 2868 7474  ), [labelme](htt
+00000ac0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000ad0: 776b 656e 7461 726f 2f6c 6162 656c 6d65  wkentaro/labelme
+00000ae0: 292e 0a2d 2049 636f 6e73 3a20 466c 6174  )..- Icons: Flat
+00000af0: 2049 636f 6e73 0a                         Icons.
```

### Comparing `anylabeling-0.0.2/anylabeling/app.py` & `anylabeling-0.0.3/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.0.3/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/configs/autolabel_yolov5m.yaml` & `anylabeling-0.0.3/anylabeling/configs/autolabel_yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/configs/autolabel_yolov5s.yaml` & `anylabeling-0.0.3/anylabeling/configs/autolabel_yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/resources/resources.py` & `anylabeling-0.0.3/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.0.3/anylabeling/services/auto_labeling/model.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.0.3/anylabeling/services/auto_labeling/model_manager.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/services/auto_labeling/segment_anything.py` & `anylabeling-0.0.3/anylabeling/services/auto_labeling/segment_anything.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.0.3/anylabeling/services/auto_labeling/types.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.0.3/anylabeling/services/auto_labeling/yolov5.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/common/tableview.py` & `anylabeling-0.0.3/anylabeling/views/common/tableview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/common/toaster.py` & `anylabeling-0.0.3/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/__main__.py` & `anylabeling-0.0.3/anylabeling/views/labeling/__main__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/config.py` & `anylabeling-0.0.3/anylabeling/views/labeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/label_file.py` & `anylabeling-0.0.3/anylabeling/views/labeling/label_file.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.0.3/anylabeling/views/labeling/label_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.0.3/anylabeling/views/labeling/label_wrapper.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/logger.py` & `anylabeling-0.0.3/anylabeling/views/labeling/logger.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/shape.py` & `anylabeling-0.0.3/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/testing.py` & `anylabeling-0.0.3/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/utils/__init__.py` & `anylabeling-0.0.3/anylabeling/views/labeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.0.3/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.0.3/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.0.3/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.0.3/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.0.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.0.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.0.3/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.0.3/anylabeling/views/labeling/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.0.3/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.0.3/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.0.3/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.0.3/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.0.3/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.0.3/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.0.3/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/maintabs.py` & `anylabeling-0.0.3/anylabeling/views/maintabs.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/mainwindow.py` & `anylabeling-0.0.3/anylabeling/views/mainwindow.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling/views/mainwindow_tabs.py` & `anylabeling-0.0.3/anylabeling/views/mainwindow_tabs.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.0.3/anylabeling.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 616e 796c  : 2.1.Name: anyl
 00000020: 6162 656c 696e 670a 5665 7273 696f 6e3a  abeling.Version:
-00000030: 2030 2e30 2e32 0a53 756d 6d61 7279 3a20   0.0.2.Summary: 
+00000030: 2030 2e30 2e33 0a53 756d 6d61 7279 3a20   0.0.3.Summary: 
 00000040: 4566 666f 7274 6c65 7373 2064 6174 6120  Effortless data 
 00000050: 6c61 6265 6c69 6e67 2077 6974 6820 4149  labeling with AI
 00000060: 2073 7570 706f 7274 0a48 6f6d 652d 7061   support.Home-pa
 00000070: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 00000080: 7562 2e63 6f6d 2f76 6965 7461 6e68 6465  ub.com/vietanhde
 00000090: 762f 616e 796c 6162 656c 696e 670a 4175  v/anylabeling.Au
 000000a0: 7468 6f72 3a20 5669 6574 2d41 6e68 204e  thor: Viet-Anh N
@@ -69,60 +69,108 @@
 00000440: 794c 6162 656c 696e 6720 3d20 4c61 6265  yLabeling = Labe
 00000450: 6c49 6d67 202b 204c 6162 656c 6d65 202b  lImg + Labelme +
 00000460: 2049 6d70 726f 7665 6420 5549 202b 2041   Improved UI + A
 00000470: 7574 6f2d 6c61 6265 6c69 6e67 3c2f 623e  uto-labeling</b>
 00000480: 3c70 3e0a 3c2f 703e 0a0a 215b 5d28 6874  <p>.</p>..![](ht
 00000490: 7470 733a 2f2f 692e 696d 6775 722e 636f  tps://i.imgur.co
 000004a0: 6d2f 7761 7856 496d 762e 706e 6729 0a0a  m/waxVImv.png)..
-000004b0: 0a23 2320 492e 2049 6e73 7461 6c6c 2061  .## I. Install a
-000004c0: 6e64 2072 756e 0a0a 2d20 5265 7175 6972  nd run..- Requir
-000004d0: 656d 656e 7473 3a20 5079 7468 6f6e 203e  ements: Python >
-000004e0: 3d20 332e 380a 2d20 5265 636f 6d6d 656e  = 3.8.- Recommen
-000004f0: 6465 643a 204d 696e 6963 6f6e 6461 2f41  ded: Miniconda/A
-00000500: 6e61 636f 6e64 6120 3c68 7474 7073 3a2f  naconda <https:/
-00000510: 2f64 6f63 732e 636f 6e64 612e 696f 2f65  /docs.conda.io/e
-00000520: 6e2f 6c61 7465 7374 2f6d 696e 6963 6f6e  n/latest/minicon
-00000530: 6461 2e68 746d 6c3e 0a0a 2d20 4372 6561  da.html>..- Crea
-00000540: 7465 2065 6e76 6972 6f6e 6d65 6e74 3a0a  te environment:.
-00000550: 0a60 6060 0a63 6f6e 6461 2063 7265 6174  .```.conda creat
-00000560: 6520 2d6e 2061 6e79 6c61 6265 6c69 6e67  e -n anylabeling
-00000570: 2070 7974 686f 6e3d 332e 380a 636f 6e64   python=3.8.cond
-00000580: 6120 6163 7469 7661 7465 2061 6e79 6c61  a activate anyla
-00000590: 6265 6c69 6e67 0a60 6060 0a0a 2d20 2a2a  beling.```..- **
-000005a0: 2846 6f72 206d 6163 4f53 206f 6e6c 7929  (For macOS only)
-000005b0: 2a2a 2049 6e73 7461 6c6c 2050 7951 7435  ** Install PyQt5
-000005c0: 2075 7369 6e67 2043 6f6e 6461 3a0a 0a60   using Conda:..`
-000005d0: 6060 0a63 6f6e 6461 2069 6e73 7461 6c6c  ``.conda install
-000005e0: 202d 6320 636f 6e64 612d 666f 7267 6520   -c conda-forge 
-000005f0: 7079 7174 3d3d 352e 3135 2e37 0a60 6060  pyqt==5.15.7.```
-00000600: 0a0a 2d20 496e 7374 616c 6c20 616e 796c  ..- Install anyl
-00000610: 6162 656c 696e 673a 0a0a 6060 600a 7069  abeling:..```.pi
-00000620: 7020 696e 7374 616c 6c20 616e 796c 6162  p install anylab
-00000630: 656c 696e 670a 6060 600a 0a2d 2052 756e  eling.```..- Run
-00000640: 2061 7070 3a0a 0a60 6060 0a61 6e79 6c61   app:..```.anyla
-00000650: 6265 6c69 6e67 0a60 6060 0a0a 4f72 0a0a  beling.```..Or..
-00000660: 6060 600a 7079 7468 6f6e 202d 6d20 616e  ```.python -m an
-00000670: 796c 6162 656c 696e 672e 6170 700a 6060  ylabeling.app.``
-00000680: 600a 0a23 2320 4949 2e20 4465 7665 6c6f  `..## II. Develo
-00000690: 706d 656e 740a 0a2d 2047 656e 6572 6174  pment..- Generat
-000006a0: 6520 7265 736f 7572 6365 733a 0a0a 6060  e resources:..``
-000006b0: 600a 7079 7263 6335 202d 6f20 616e 796c  `.pyrcc5 -o anyl
-000006c0: 6162 656c 696e 672f 7265 736f 7572 6365  abeling/resource
-000006d0: 732f 7265 736f 7572 6365 732e 7079 2061  s/resources.py a
-000006e0: 6e79 6c61 6265 6c69 6e67 2f72 6573 6f75  nylabeling/resou
-000006f0: 7263 6573 2f72 6573 6f75 7263 6573 2e71  rces/resources.q
-00000700: 7263 0a60 6060 0a0a 2d20 5275 6e20 6170  rc.```..- Run ap
-00000710: 703a 0a0a 6060 600a 7079 7468 6f6e 2061  p:..```.python a
-00000720: 6e79 6c61 6265 6c69 6e67 2f61 7070 2e70  nylabeling/app.p
-00000730: 790a 6060 600a 0a23 2320 4949 492e 2052  y.```..## III. R
-00000740: 6566 6572 656e 6365 730a 0a2d 204c 6162  eferences..- Lab
-00000750: 656c 696e 6720 5549 2062 7569 6c74 2077  eling UI built w
-00000760: 6974 6820 6964 6561 7320 616e 6420 636f  ith ideas and co
-00000770: 6d70 6f6e 656e 7473 2066 726f 6d20 5b4c  mponents from [L
-00000780: 6162 656c 496d 675d 2868 7474 7073 3a2f  abelImg](https:/
-00000790: 2f67 6974 6875 622e 636f 6d2f 6865 6172  /github.com/hear
-000007a0: 7465 786c 6162 732f 6c61 6265 6c49 6d67  texlabs/labelImg
-000007b0: 292c 205b 6c61 6265 6c6d 655d 2868 7474  ), [labelme](htt
-000007c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000007d0: 776b 656e 7461 726f 2f6c 6162 656c 6d65  wkentaro/labelme
-000007e0: 292e 0a2d 2049 636f 6e73 3a20 466c 6174  )..- Icons: Flat
-000007f0: 2049 636f 6e73 0a                         Icons.
+000004b0: 5b21 5b50 7950 495d 2868 7474 7073 3a2f  [![PyPI](https:/
+000004c0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000004d0: 7079 7069 2f76 2f61 6e79 6c61 6265 6c69  pypi/v/anylabeli
+000004e0: 6e67 295d 2868 7474 7073 3a2f 2f70 7970  ng)](https://pyp
+000004f0: 692e 6f72 672f 7072 6f6a 6563 742f 616e  i.org/project/an
+00000500: 796c 6162 656c 696e 6729 0a5b 215b 6c69  ylabeling).[![li
+00000510: 6365 6e73 655d 2868 7474 7073 3a2f 2f69  cense](https://i
+00000520: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00000530: 7468 7562 2f6c 6963 656e 7365 2f76 6965  thub/license/vie
+00000540: 7461 6e68 6465 762f 616e 796c 6162 656c  tanhdev/anylabel
+00000550: 696e 672e 7376 6729 5d28 6874 7470 733a  ing.svg)](https:
+00000560: 2f2f 6769 7468 7562 2e63 6f6d 2f76 6965  //github.com/vie
+00000570: 7461 6e68 6465 762f 616e 796c 6162 656c  tanhdev/anylabel
+00000580: 696e 672f 626c 6f62 2f6d 6173 7465 722f  ing/blob/master/
+00000590: 4c49 4345 4e53 4529 0a5b 215b 6f70 656e  LICENSE).[![open
+000005a0: 2069 7373 7565 735d 2868 7474 7073 3a2f   issues](https:/
+000005b0: 2f69 7369 746d 6169 6e74 6169 6e65 642e  /isitmaintained.
+000005c0: 636f 6d2f 6261 6467 652f 6f70 656e 2f76  com/badge/open/v
+000005d0: 6965 7461 6e68 6465 762f 616e 796c 6162  ietanhdev/anylab
+000005e0: 656c 696e 672e 7376 6729 5d28 6874 7470  eling.svg)](http
+000005f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f76  s://github.com/v
+00000600: 6965 7461 6e68 6465 762f 616e 796c 6162  ietanhdev/anylab
+00000610: 656c 696e 672f 6973 7375 6573 290a 5b21  eling/issues).[!
+00000620: 5b50 7970 6920 446f 776e 6c6f 6164 735d  [Pypi Downloads]
+00000630: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
+00000640: 6368 2f62 6164 6765 2f61 6e79 6c61 6265  ch/badge/anylabe
+00000650: 6c69 6e67 295d 2868 7474 7073 3a2f 2f70  ling)](https://p
+00000660: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00000670: 616e 796c 6162 656c 696e 672f 290a 0a3c  anylabeling/)..<
+00000680: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000690: 7777 772e 796f 7574 7562 652e 636f 6d2f  www.youtube.com/
+000006a0: 7761 7463 683f 763d 3569 5153 474c 3765  watch?v=5iQSGL7e
+000006b0: 6258 4522 3e0a 2020 3c69 6d67 2061 6c74  bXE">.  <img alt
+000006c0: 3d22 416e 794c 6162 656c 696e 6722 2073  ="AnyLabeling" s
+000006d0: 7263 3d22 6874 7470 733a 2f2f 7573 6572  rc="https://user
+000006e0: 2d69 6d61 6765 732e 6769 7468 7562 7573  -images.githubus
+000006f0: 6572 636f 6e74 656e 742e 636f 6d2f 3138  ercontent.com/18
+00000700: 3332 3934 3731 2f32 3331 3332 3034 3838  329471/231320488
+00000710: 2d32 6638 3133 3362 632d 3662 3531 2d34  -2f8133bc-6b51-4
+00000720: 3866 382d 3832 6136 2d64 6433 6232 3637  8f8-82a6-dd3b267
+00000730: 6635 3135 362e 706e 6722 2f3e 0a3c 2f61  f5156.png"/>.</a
+00000740: 3e0a 0a2a 2a59 6f75 7475 6265 2044 656d  >..**Youtube Dem
+00000750: 6f3a 2a2a 205b 6874 7470 733a 2f2f 7777  o:** [https://ww
+00000760: 772e 796f 7574 7562 652e 636f 6d2f 7761  w.youtube.com/wa
+00000770: 7463 683f 763d 3569 5153 474c 3765 6258  tch?v=5iQSGL7ebX
+00000780: 455d 2868 7474 7073 3a2f 2f77 7777 2e79  E](https://www.y
+00000790: 6f75 7475 6265 2e63 6f6d 2f77 6174 6368  outube.com/watch
+000007a0: 3f76 3d35 6951 5347 4c37 6562 5845 290a  ?v=5iQSGL7ebXE).
+000007b0: 0a23 2320 492e 2049 6e73 7461 6c6c 2061  .## I. Install a
+000007c0: 6e64 2072 756e 0a0a 2d20 5265 7175 6972  nd run..- Requir
+000007d0: 656d 656e 7473 3a20 5079 7468 6f6e 203e  ements: Python >
+000007e0: 3d20 332e 380a 2d20 5265 636f 6d6d 656e  = 3.8.- Recommen
+000007f0: 6465 643a 204d 696e 6963 6f6e 6461 2f41  ded: Miniconda/A
+00000800: 6e61 636f 6e64 6120 3c68 7474 7073 3a2f  naconda <https:/
+00000810: 2f64 6f63 732e 636f 6e64 612e 696f 2f65  /docs.conda.io/e
+00000820: 6e2f 6c61 7465 7374 2f6d 696e 6963 6f6e  n/latest/minicon
+00000830: 6461 2e68 746d 6c3e 0a0a 2d20 4372 6561  da.html>..- Crea
+00000840: 7465 2065 6e76 6972 6f6e 6d65 6e74 3a0a  te environment:.
+00000850: 0a60 6060 0a63 6f6e 6461 2063 7265 6174  .```.conda creat
+00000860: 6520 2d6e 2061 6e79 6c61 6265 6c69 6e67  e -n anylabeling
+00000870: 2070 7974 686f 6e3d 332e 380a 636f 6e64   python=3.8.cond
+00000880: 6120 6163 7469 7661 7465 2061 6e79 6c61  a activate anyla
+00000890: 6265 6c69 6e67 0a60 6060 0a0a 2d20 2a2a  beling.```..- **
+000008a0: 2846 6f72 206d 6163 4f53 206f 6e6c 7929  (For macOS only)
+000008b0: 2a2a 2049 6e73 7461 6c6c 2050 7951 7435  ** Install PyQt5
+000008c0: 2075 7369 6e67 2043 6f6e 6461 3a0a 0a60   using Conda:..`
+000008d0: 6060 0a63 6f6e 6461 2069 6e73 7461 6c6c  ``.conda install
+000008e0: 202d 6320 636f 6e64 612d 666f 7267 6520   -c conda-forge 
+000008f0: 7079 7174 3d3d 352e 3135 2e37 0a60 6060  pyqt==5.15.7.```
+00000900: 0a0a 2d20 496e 7374 616c 6c20 616e 796c  ..- Install anyl
+00000910: 6162 656c 696e 673a 0a0a 6060 600a 7069  abeling:..```.pi
+00000920: 7020 696e 7374 616c 6c20 616e 796c 6162  p install anylab
+00000930: 656c 696e 670a 6060 600a 0a2d 2052 756e  eling.```..- Run
+00000940: 2061 7070 3a0a 0a60 6060 0a61 6e79 6c61   app:..```.anyla
+00000950: 6265 6c69 6e67 0a60 6060 0a0a 4f72 0a0a  beling.```..Or..
+00000960: 6060 600a 7079 7468 6f6e 202d 6d20 616e  ```.python -m an
+00000970: 796c 6162 656c 696e 672e 6170 700a 6060  ylabeling.app.``
+00000980: 600a 0a23 2320 4949 2e20 4465 7665 6c6f  `..## II. Develo
+00000990: 706d 656e 740a 0a2d 2047 656e 6572 6174  pment..- Generat
+000009a0: 6520 7265 736f 7572 6365 733a 0a0a 6060  e resources:..``
+000009b0: 600a 7079 7263 6335 202d 6f20 616e 796c  `.pyrcc5 -o anyl
+000009c0: 6162 656c 696e 672f 7265 736f 7572 6365  abeling/resource
+000009d0: 732f 7265 736f 7572 6365 732e 7079 2061  s/resources.py a
+000009e0: 6e79 6c61 6265 6c69 6e67 2f72 6573 6f75  nylabeling/resou
+000009f0: 7263 6573 2f72 6573 6f75 7263 6573 2e71  rces/resources.q
+00000a00: 7263 0a60 6060 0a0a 2d20 5275 6e20 6170  rc.```..- Run ap
+00000a10: 703a 0a0a 6060 600a 7079 7468 6f6e 2061  p:..```.python a
+00000a20: 6e79 6c61 6265 6c69 6e67 2f61 7070 2e70  nylabeling/app.p
+00000a30: 790a 6060 600a 0a23 2320 4949 492e 2052  y.```..## III. R
+00000a40: 6566 6572 656e 6365 730a 0a2d 204c 6162  eferences..- Lab
+00000a50: 656c 696e 6720 5549 2062 7569 6c74 2077  eling UI built w
+00000a60: 6974 6820 6964 6561 7320 616e 6420 636f  ith ideas and co
+00000a70: 6d70 6f6e 656e 7473 2066 726f 6d20 5b4c  mponents from [L
+00000a80: 6162 656c 496d 675d 2868 7474 7073 3a2f  abelImg](https:/
+00000a90: 2f67 6974 6875 622e 636f 6d2f 6865 6172  /github.com/hear
+00000aa0: 7465 786c 6162 732f 6c61 6265 6c49 6d67  texlabs/labelImg
+00000ab0: 292c 205b 6c61 6265 6c6d 655d 2868 7474  ), [labelme](htt
+00000ac0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000ad0: 776b 656e 7461 726f 2f6c 6162 656c 6d65  wkentaro/labelme
+00000ae0: 292e 0a2d 2049 636f 6e73 3a20 466c 6174  )..- Icons: Flat
+00000af0: 2049 636f 6e73 0a                         Icons.
```

### Comparing `anylabeling-0.0.2/anylabeling.egg-info/SOURCES.txt` & `anylabeling-0.0.3/anylabeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.2/setup.py` & `anylabeling-0.0.3/setup.py`

 * *Files identical despite different names*

