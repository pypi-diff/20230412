# Comparing `tmp/anylabeling-0.0.3.tar.gz` & `tmp/anylabeling-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.0.3.tar", last modified: Wed Apr 12 01:16:45 2023, max compression
+gzip compressed data, was "anylabeling-0.0.4.tar", last modified: Wed Apr 12 01:33:04 2023, max compression
```

## Comparing `anylabeling-0.0.3.tar` & `anylabeling-0.0.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.298288 anylabeling-0.0.3/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.0.3/LICENSE
--rw-r--r--   0 vietanhdev   (501) staff       (20)      120 2023-04-08 18:53:13.000000 anylabeling-0.0.3/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2807 2023-04-12 01:16:45.298109 anylabeling-0.0.3/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.0.3/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.288836 anylabeling-0.0.3/anylabeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       22 2023-04-12 01:16:35.000000 anylabeling-0.0.3/anylabeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1062 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/app.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.290269 anylabeling-0.0.3/anylabeling/configs/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/configs/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.290391 anylabeling-0.0.3/anylabeling/configs/__pycache__/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.0.3/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/configs/anylabeling_config.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)      315 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/configs/autolabel_segment_anything.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/configs/autolabel_yolov5m.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/configs/autolabel_yolov5s.yaml
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.290844 anylabeling-0.0.3/anylabeling/resources/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/resources/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)   423402 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/resources/resources.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.291566 anylabeling-0.0.3/anylabeling/services/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/services/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.292309 anylabeling-0.0.3/anylabeling/services/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2955 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5277 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9837 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1284 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5127 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/utils.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.292783 anylabeling-0.0.3/anylabeling/views/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/views/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.293158 anylabeling-0.0.3/anylabeling/views/common/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/views/common/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/views/common/tableview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.0.3/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.294763 anylabeling-0.0.3/anylabeling/views/labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      343 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5758 2023-04-08 20:04:23.000000 anylabeling-0.0.3/anylabeling/views/labeling/__main__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2717 2023-04-09 06:42:35.000000 anylabeling-0.0.3/anylabeling/views/labeling/config.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6405 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    88768 2023-04-11 18:18:40.000000 anylabeling-0.0.3/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      606 2023-04-08 20:07:28.000000 anylabeling-0.0.3/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1811 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/logger.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/shape.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.295667 anylabeling-0.0.3/anylabeling/views/labeling/utils/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.297301 anylabeling-0.0.3/anylabeling/views/labeling/widgets/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.297885 anylabeling-0.0.3/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6906 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    46264 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8023 2023-04-08 19:49:25.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5778 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1390 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      768 2023-04-08 20:09:45.000000 anylabeling-0.0.3/anylabeling/views/maintabs.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      981 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/mainwindow.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1458 2023-04-11 17:52:02.000000 anylabeling-0.0.3/anylabeling/views/mainwindow_tabs.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:16:45.289682 anylabeling-0.0.3/anylabeling.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2807 2023-04-12 01:16:45.000000 anylabeling-0.0.3/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2620 2023-04-12 01:16:45.000000 anylabeling-0.0.3/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-12 01:16:45.000000 anylabeling-0.0.3/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-12 01:16:45.000000 anylabeling-0.0.3/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      235 2023-04-12 01:16:45.000000 anylabeling-0.0.3/anylabeling.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-12 01:16:45.000000 anylabeling-0.0.3/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.0.3/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-12 01:16:45.298336 anylabeling-0.0.3/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2503 2023-04-11 17:52:02.000000 anylabeling-0.0.3/setup.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.024191 anylabeling-0.0.4/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.0.4/LICENSE
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      120 2023-04-08 18:53:13.000000 anylabeling-0.0.4/MANIFEST.in
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2807 2023-04-12 01:33:04.024030 anylabeling-0.0.4/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.0.4/README.md
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.011370 anylabeling-0.0.4/anylabeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       22 2023-04-12 01:31:27.000000 anylabeling-0.0.4/anylabeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1062 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/app.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.012852 anylabeling-0.0.4/anylabeling/configs/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.4/anylabeling/configs/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.012989 anylabeling-0.0.4/anylabeling/configs/__pycache__/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.0.4/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/configs/anylabeling_config.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      315 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/configs/autolabel_segment_anything.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/configs/autolabel_yolov5m.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/configs/autolabel_yolov5s.yaml
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.013233 anylabeling-0.0.4/anylabeling/resources/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.4/anylabeling/resources/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   423402 2023-04-08 18:49:39.000000 anylabeling-0.0.4/anylabeling/resources/resources.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.014647 anylabeling-0.0.4/anylabeling/services/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.4/anylabeling/services/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.015469 anylabeling-0.0.4/anylabeling/services/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3443 2023-04-12 01:31:17.000000 anylabeling-0.0.4/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5355 2023-04-12 01:27:25.000000 anylabeling-0.0.4/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9861 2023-04-12 01:26:18.000000 anylabeling-0.0.4/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1284 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5151 2023-04-12 01:26:25.000000 anylabeling-0.0.4/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/utils.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.016309 anylabeling-0.0.4/anylabeling/views/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.4/anylabeling/views/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.016945 anylabeling-0.0.4/anylabeling/views/common/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.4/anylabeling/views/common/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.0.4/anylabeling/views/common/tableview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.0.4/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.019800 anylabeling-0.0.4/anylabeling/views/labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      343 2023-04-08 19:49:25.000000 anylabeling-0.0.4/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5758 2023-04-08 20:04:23.000000 anylabeling-0.0.4/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2717 2023-04-09 06:42:35.000000 anylabeling-0.0.4/anylabeling/views/labeling/config.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6405 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    88768 2023-04-11 18:18:40.000000 anylabeling-0.0.4/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      606 2023-04-08 20:07:28.000000 anylabeling-0.0.4/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1811 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 19:49:25.000000 anylabeling-0.0.4/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.0.4/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.020885 anylabeling-0.0.4/anylabeling/views/labeling/utils/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.0.4/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.0.4/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.0.4/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.023307 anylabeling-0.0.4/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.023807 anylabeling-0.0.4/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6906 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    46264 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8023 2023-04-08 19:49:25.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5778 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1390 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      768 2023-04-08 20:09:45.000000 anylabeling-0.0.4/anylabeling/views/maintabs.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      981 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/mainwindow.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1458 2023-04-11 17:52:02.000000 anylabeling-0.0.4/anylabeling/views/mainwindow_tabs.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:33:04.012230 anylabeling-0.0.4/anylabeling.egg-info/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2807 2023-04-12 01:33:03.000000 anylabeling-0.0.4/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2620 2023-04-12 01:33:03.000000 anylabeling-0.0.4/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-12 01:33:03.000000 anylabeling-0.0.4/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-12 01:33:03.000000 anylabeling-0.0.4/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      235 2023-04-12 01:33:03.000000 anylabeling-0.0.4/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-12 01:33:03.000000 anylabeling-0.0.4/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.0.4/pyproject.toml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-12 01:33:04.024234 anylabeling-0.0.4/setup.cfg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2503 2023-04-11 17:52:02.000000 anylabeling-0.0.4/setup.py
```

### Comparing `anylabeling-0.0.3/LICENSE` & `anylabeling-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/PKG-INFO` & `anylabeling-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.0.3
+Version: 0.0.4
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.0.3 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.0.4 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `anylabeling-0.0.3/README.md` & `anylabeling-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/app.py` & `anylabeling-0.0.4/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.0.4/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/configs/autolabel_yolov5m.yaml` & `anylabeling-0.0.4/anylabeling/configs/autolabel_yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/configs/autolabel_yolov5s.yaml` & `anylabeling-0.0.4/anylabeling/configs/autolabel_yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/resources/resources.py` & `anylabeling-0.0.4/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.0.4/anylabeling/services/auto_labeling/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,16 @@
         "https://github.com/vietanhdev/anylabeling-assets/raw/main/"
     )
 
     class Meta:
         required_config_names = []
         buttons = ["button_run"]
 
-    def __init__(self, model_config) -> None:
+    def __init__(self, model_config, on_message) -> None:
+        self.on_message = on_message
         # Load and check config
         if isinstance(model_config, str):
             if not os.path.isfile(model_config):
                 raise Exception(f"Config file not found: {model_config}")
             with open(model_config, "r") as f:
                 self.config = yaml.safe_load(f)
         elif isinstance(model_config, dict):
@@ -46,14 +47,17 @@
         # Try getting model path from config folder
         model_abs_path = os.path.abspath(model_path)
         if os.path.exists(model_abs_path):
             return model_abs_path
 
         # Try download model from url
         if model_path.startswith("anylabeling_assets/"):
+            self.on_message(
+                "Downloading model from model registry. This may take a while..."
+            )
             relative_path = model_path.replace("anylabeling_assets/", "")
             download_url = self.BASE_DOWNLOAD_URL + relative_path
             model_abs_path = os.path.join(
                 os.path.abspath("data"), relative_path
             )
             if os.path.exists(model_abs_path):
                 return model_abs_path
@@ -61,17 +65,26 @@
                 parents=True, exist_ok=True
             )
 
             # Download model from url
             logging.info(
                 f"Downloading model from {download_url} to {model_abs_path}"
             )
-            data = urllib.request.urlopen(download_url).read()
-            with open(model_abs_path, "wb") as f:
-                f.write(data)
+
+            try:
+                data = urllib.request.urlopen(download_url).read()
+                with open(model_abs_path, "wb") as f:
+                    f.write(data)
+            except Exception as e:
+                self.on_message(
+                    f"Could not downloading model from {download_url}"
+                )
+                raise Exception(
+                    f"Could not downloading model from {download_url}: {e}"
+                )
 
             return model_abs_path
 
         return None
 
     def check_missing_config(self, config_names, config):
         """
```

### Comparing `anylabeling-0.0.3/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.0.4/anylabeling/services/auto_labeling/model_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,20 +104,20 @@
             self.auto_segmentation_model_unselected.emit()
 
         model_info = copy.deepcopy(self.model_infos[model_name])
 
         if model_info["type"] == "yolov5":
             from .yolov5 import YOLOv5
 
-            model_info["model"] = YOLOv5(model_info)
+            model_info["model"] = YOLOv5(model_info, on_message=self.new_model_status.emit)
             self.auto_segmentation_model_unselected.emit()
         elif model_info["type"] == "segment_anything":
             from .segment_anything import SegmentAnything
 
-            model_info["model"] = SegmentAnything(model_info)
+            model_info["model"] = SegmentAnything(model_info, on_message=self.new_model_status.emit)
             self.auto_segmentation_model_selected.emit()
         else:
             raise Exception(f"Unknown model type: {model_info['type']}")
 
         self.loaded_model_info = model_info
         return self.loaded_model_info
```

### Comparing `anylabeling-0.0.3/anylabeling/services/auto_labeling/segment_anything.py` & `anylabeling-0.0.4/anylabeling/services/auto_labeling/segment_anything.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
             "button_remove_point",
             "button_add_rect",
             # "button_undo", # Dont support undo now
             "button_clear",
             "button_finish_object",
         ]
 
-    def __init__(self, config_path) -> None:
+    def __init__(self, config_path, on_message) -> None:
         # Run the parent class's init method
-        super().__init__(config_path)
+        super().__init__(config_path, on_message)
         self.input_size = self.config["input_size"]
         self.max_width = self.config["max_width"]
         self.max_height = self.config["max_height"]
 
         # Get encoder and decoder model paths
         encoder_model_abs_path = self.get_model_abs_path(
             self.config["encoder_model_path"]
```

### Comparing `anylabeling-0.0.3/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.0.4/anylabeling/services/auto_labeling/types.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.0.4/anylabeling/services/auto_labeling/yolov5.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
             "score_threshold",
             "nms_threshold",
             "confidence_threshold",
             "classes",
         ]
         buttons = ["button_run"]
 
-    def __init__(self, model_config) -> None:
+    def __init__(self, model_config, on_message) -> None:
         # Run the parent class's init method
-        super().__init__(model_config)
+        super().__init__(model_config, on_message)
 
         model_abs_path = self.get_model_abs_path(self.config["model_path"])
         if not os.path.isfile(model_abs_path):
             raise Exception(f"Model not found: {model_abs_path}")
 
         self.net = cv2.dnn.readNet(model_abs_path)
         self.classes = self.config["classes"]
```

### Comparing `anylabeling-0.0.3/anylabeling/views/common/tableview.py` & `anylabeling-0.0.4/anylabeling/views/common/tableview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/common/toaster.py` & `anylabeling-0.0.4/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/__main__.py` & `anylabeling-0.0.4/anylabeling/views/labeling/__main__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/config.py` & `anylabeling-0.0.4/anylabeling/views/labeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/label_file.py` & `anylabeling-0.0.4/anylabeling/views/labeling/label_file.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.0.4/anylabeling/views/labeling/label_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.0.4/anylabeling/views/labeling/label_wrapper.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/logger.py` & `anylabeling-0.0.4/anylabeling/views/labeling/logger.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/shape.py` & `anylabeling-0.0.4/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/testing.py` & `anylabeling-0.0.4/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/utils/__init__.py` & `anylabeling-0.0.4/anylabeling/views/labeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.0.4/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.0.4/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.0.4/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.0.4/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.0.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.0.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.0.4/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.0.4/anylabeling/views/labeling/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.0.4/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.0.4/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.0.4/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.0.4/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.0.4/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.0.4/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.0.4/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/maintabs.py` & `anylabeling-0.0.4/anylabeling/views/maintabs.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/mainwindow.py` & `anylabeling-0.0.4/anylabeling/views/mainwindow.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling/views/mainwindow_tabs.py` & `anylabeling-0.0.4/anylabeling/views/mainwindow_tabs.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.0.4/anylabeling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.0.3
+Version: 0.0.4
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.0.3 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.0.4 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `anylabeling-0.0.3/anylabeling.egg-info/SOURCES.txt` & `anylabeling-0.0.4/anylabeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.3/setup.py` & `anylabeling-0.0.4/setup.py`

 * *Files identical despite different names*

