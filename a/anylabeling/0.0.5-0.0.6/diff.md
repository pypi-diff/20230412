# Comparing `tmp/anylabeling-0.0.5.tar.gz` & `tmp/anylabeling-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.0.5.tar", last modified: Wed Apr 12 01:40:29 2023, max compression
+gzip compressed data, was "anylabeling-0.0.6.tar", last modified: Wed Apr 12 01:50:59 2023, max compression
```

## Comparing `anylabeling-0.0.5.tar` & `anylabeling-0.0.6.tar`

### file list

```diff
@@ -1,81 +1,137 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.713143 anylabeling-0.0.5/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.0.5/LICENSE
--rw-r--r--   0 vietanhdev   (501) staff       (20)      120 2023-04-08 18:53:13.000000 anylabeling-0.0.5/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2807 2023-04-12 01:40:29.712979 anylabeling-0.0.5/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.0.5/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.700427 anylabeling-0.0.5/anylabeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       22 2023-04-12 01:38:22.000000 anylabeling-0.0.5/anylabeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1062 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/app.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.702887 anylabeling-0.0.5/anylabeling/configs/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.5/anylabeling/configs/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.703096 anylabeling-0.0.5/anylabeling/configs/__pycache__/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.0.5/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/configs/anylabeling_config.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)      315 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/configs/autolabel_segment_anything.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/configs/autolabel_yolov5m.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/configs/autolabel_yolov5s.yaml
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.703468 anylabeling-0.0.5/anylabeling/resources/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.5/anylabeling/resources/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)   477689 2023-04-12 01:37:51.000000 anylabeling-0.0.5/anylabeling/resources/resources.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.703873 anylabeling-0.0.5/anylabeling/services/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.5/anylabeling/services/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.704653 anylabeling-0.0.5/anylabeling/services/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3443 2023-04-12 01:31:17.000000 anylabeling-0.0.5/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5355 2023-04-12 01:27:25.000000 anylabeling-0.0.5/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9861 2023-04-12 01:26:18.000000 anylabeling-0.0.5/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1284 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5151 2023-04-12 01:26:25.000000 anylabeling-0.0.5/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/utils.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.705433 anylabeling-0.0.5/anylabeling/views/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.5/anylabeling/views/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.706067 anylabeling-0.0.5/anylabeling/views/common/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.5/anylabeling/views/common/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.0.5/anylabeling/views/common/tableview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.0.5/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.708725 anylabeling-0.0.5/anylabeling/views/labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      343 2023-04-08 19:49:25.000000 anylabeling-0.0.5/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5758 2023-04-08 20:04:23.000000 anylabeling-0.0.5/anylabeling/views/labeling/__main__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2717 2023-04-09 06:42:35.000000 anylabeling-0.0.5/anylabeling/views/labeling/config.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6405 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    88768 2023-04-11 18:18:40.000000 anylabeling-0.0.5/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      606 2023-04-08 20:07:28.000000 anylabeling-0.0.5/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1811 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/logger.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 19:49:25.000000 anylabeling-0.0.5/anylabeling/views/labeling/shape.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.0.5/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.710001 anylabeling-0.0.5/anylabeling/views/labeling/utils/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.0.5/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.0.5/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.0.5/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.712200 anylabeling-0.0.5/anylabeling/views/labeling/widgets/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.712732 anylabeling-0.0.5/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6906 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    46264 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8023 2023-04-08 19:49:25.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5778 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1390 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      768 2023-04-08 20:09:45.000000 anylabeling-0.0.5/anylabeling/views/maintabs.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      981 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/mainwindow.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1458 2023-04-11 17:52:02.000000 anylabeling-0.0.5/anylabeling/views/mainwindow_tabs.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:40:29.702029 anylabeling-0.0.5/anylabeling.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2807 2023-04-12 01:40:29.000000 anylabeling-0.0.5/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2620 2023-04-12 01:40:29.000000 anylabeling-0.0.5/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-12 01:40:29.000000 anylabeling-0.0.5/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-12 01:40:29.000000 anylabeling-0.0.5/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      235 2023-04-12 01:40:29.000000 anylabeling-0.0.5/anylabeling.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-12 01:40:29.000000 anylabeling-0.0.5/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.0.5/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-12 01:40:29.713190 anylabeling-0.0.5/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2503 2023-04-11 17:52:02.000000 anylabeling-0.0.5/setup.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.980353 anylabeling-0.0.6/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.0.6/LICENSE
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      112 2023-04-12 01:46:44.000000 anylabeling-0.0.6/MANIFEST.in
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 01:50:59.980139 anylabeling-0.0.6/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.0.6/README.md
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.961061 anylabeling-0.0.6/anylabeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       22 2023-04-12 01:50:53.000000 anylabeling-0.0.6/anylabeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1062 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/app.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.962522 anylabeling-0.0.6/anylabeling/configs/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/configs/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.962660 anylabeling-0.0.6/anylabeling/configs/__pycache__/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.0.6/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/configs/anylabeling_config.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      315 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/configs/autolabel_segment_anything.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/configs/autolabel_yolov5m.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/configs/autolabel_yolov5s.yaml
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.963108 anylabeling-0.0.6/anylabeling/resources/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/resources/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   477689 2023-04-12 01:37:51.000000 anylabeling-0.0.6/anylabeling/resources/resources.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.963527 anylabeling-0.0.6/anylabeling/services/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/services/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.964493 anylabeling-0.0.6/anylabeling/services/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3443 2023-04-12 01:31:17.000000 anylabeling-0.0.6/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5355 2023-04-12 01:27:25.000000 anylabeling-0.0.6/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9861 2023-04-12 01:26:18.000000 anylabeling-0.0.6/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1284 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5151 2023-04-12 01:26:25.000000 anylabeling-0.0.6/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/utils.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.964986 anylabeling-0.0.6/anylabeling/views/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/views/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.965347 anylabeling-0.0.6/anylabeling/views/common/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/views/common/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/views/common/tableview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.966481 anylabeling-0.0.6/anylabeling/views/labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5766 2023-04-12 01:48:44.000000 anylabeling-0.0.6/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2725 2023-04-12 01:48:11.000000 anylabeling-0.0.6/anylabeling/views/labeling/config.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.977013 anylabeling-0.0.6/anylabeling/views/labeling/icons/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6148 2023-04-09 05:07:05.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/.DS_Store
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        8 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/app.icns
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    31379 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/app.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1645 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/app.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    28068 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/brain.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6844 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/cancel.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    11383 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/cartesian.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    15818 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/circle.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/color-line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    23824 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/color.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/color_line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10021 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/copy.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7842 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/delete.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/done.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    22232 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/done.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    15023 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/edit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7718 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/expert.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      278 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/expert1.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      335 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/expert2.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    37652 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/eye.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8059 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/feBlend-icon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/file.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    17368 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/fit-width.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2186 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/fit-window.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2262 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/fit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4156 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/format_createml.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      786 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/format_voc.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      675 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/format_yolo.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    14479 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/help.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)  1128131 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/icon.icns
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   183198 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/icon.ico
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    44771 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/icon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2381 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/labels.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    36694 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/labels.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7253 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/line-strip.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9457 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      977 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/new.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7482 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/next.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26255 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/objects.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/open.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10572 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/paste.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    13847 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/point.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    14286 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/polygon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7275 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/prev.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    22460 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/quit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2136 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/rectangle.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3637 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/resetall.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2811 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/save-as.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6118 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/save.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2004 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/undo-cross.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2018 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/undo.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    18083 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/upload_brain.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3041 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/verify.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1099 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/zoom-in.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1074 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/zoom-out.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1139 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/zoom.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6409 2023-04-12 01:48:23.000000 anylabeling-0.0.6/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    88710 2023-04-12 01:49:13.000000 anylabeling-0.0.6/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      610 2023-04-12 01:47:51.000000 anylabeling-0.0.6/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1811 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.977895 anylabeling-0.0.6/anylabeling/views/labeling/utils/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.979443 anylabeling-0.0.6/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.979840 anylabeling-0.0.6/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6906 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    46264 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8023 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5778 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1394 2023-04-12 01:47:30.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      768 2023-04-08 20:09:45.000000 anylabeling-0.0.6/anylabeling/views/maintabs.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      981 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/mainwindow.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1458 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/mainwindow_tabs.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.961857 anylabeling-0.0.6/anylabeling.egg-info/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 01:50:59.000000 anylabeling-0.0.6/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5059 2023-04-12 01:50:59.000000 anylabeling-0.0.6/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-12 01:50:59.000000 anylabeling-0.0.6/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-12 01:50:59.000000 anylabeling-0.0.6/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      235 2023-04-12 01:50:59.000000 anylabeling-0.0.6/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-12 01:50:59.000000 anylabeling-0.0.6/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.0.6/pyproject.toml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-12 01:50:59.980407 anylabeling-0.0.6/setup.cfg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2454 2023-04-12 01:44:44.000000 anylabeling-0.0.6/setup.py
```

### Comparing `anylabeling-0.0.5/LICENSE` & `anylabeling-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/PKG-INFO` & `anylabeling-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.0.5
+Version: 0.0.6
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.0.5 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.0.6 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only Description-Content-
-Type: text/markdown License-File: LICENSE
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Only Description-Content-Type: text/markdown License-File: LICENSE
                       ****** ð AnyLabeling ð ******
    Effortless data labeling with AI support from YOLO and Segment Anything!
         AnyLabeling = LabelImg + Labelme + Improved UI + Auto-labeling
 ![](https://i.imgur.com/waxVImv.png) [![PyPI](https://img.shields.io/pypi/v/
 anylabeling)](https://pypi.org/project/anylabeling) [![license](https://
 img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/blob/master/LICENSE) [![open issues](https://
```

### Comparing `anylabeling-0.0.5/README.md` & `anylabeling-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/app.py` & `anylabeling-0.0.6/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.0.6/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/configs/autolabel_yolov5m.yaml` & `anylabeling-0.0.6/anylabeling/configs/autolabel_yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/configs/autolabel_yolov5s.yaml` & `anylabeling-0.0.6/anylabeling/configs/autolabel_yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/resources/resources.py` & `anylabeling-0.0.6/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.0.6/anylabeling/services/auto_labeling/model.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.0.6/anylabeling/services/auto_labeling/model_manager.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/services/auto_labeling/segment_anything.py` & `anylabeling-0.0.6/anylabeling/services/auto_labeling/segment_anything.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.0.6/anylabeling/services/auto_labeling/types.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.0.6/anylabeling/services/auto_labeling/yolov5.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/common/tableview.py` & `anylabeling-0.0.6/anylabeling/views/common/tableview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/common/toaster.py` & `anylabeling-0.0.6/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/__main__.py` & `anylabeling-0.0.6/anylabeling/views/labeling/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         "-O",
         "-o",
         help=(
             "output file or directory (if it ends with .json it is "
             "recognized as file, else as directory)"
         ),
     )
-    default_config_file = os.path.join(os.path.expanduser("~"), ".labelmerc")
+    default_config_file = os.path.join(os.path.expanduser("~"), ".anylabelingrc")
     parser.add_argument(
         "--config",
         dest="config",
         help=(
             "config file or yaml-format string (default:"
             f" {default_config_file})"
         ),
@@ -145,15 +145,15 @@
     config_file_or_yaml = config_from_args.pop("config")
     config = get_config(config_file_or_yaml, config_from_args)
 
     if not config["labels"] and config["validate_label"]:
         logger.error(
             "--labels must be specified with --validatelabel or "
             "validate_label: true in the config file "
-            "(ex. ~/.labelmerc)."
+            "(ex. ~/.anylabelingrc)."
         )
         sys.exit(1)
 
     output_file = None
     output_dir = None
     if output is not None:
         if output.endswith(".json"):
```

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/config.py` & `anylabeling-0.0.6/anylabeling/views/labeling/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 
 def get_default_config():
     config_file = "anylabeling_config.yaml"
     with pkg_resources.open_text(anylabeling_configs, config_file) as f:
         config = yaml.safe_load(f)
 
-    # save default config to ~/.labelmerc
-    user_config_file = osp.join(osp.expanduser("~"), ".labelmerc")
+    # save default config to ~/.anylabelingrc
+    user_config_file = osp.join(osp.expanduser("~"), ".anylabelingrc")
     if not osp.exists(user_config_file):
         try:
             shutil.copy(config_file, user_config_file)
         except Exception:
             logger.warning("Failed to save config: %s", user_config_file)
 
     return config
```

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/label_file.py` & `anylabeling-0.0.6/anylabeling/views/labeling/label_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 )
             elif (
                 version.split(".")[0] != __version__.split(".", maxsplit=1)[0]
             ):
                 logger.warning(
                     (
                         "This JSON file (%s) may be incompatible with "
-                        "current labelme. version in file: %s, "
+                        "current AnyLabeling. version in file: %s, "
                         "current version: %s"
                     ),
                     filename,
                     version,
                     __version__,
                 )
```

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.0.6/anylabeling/views/labeling/label_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"""This module defines labelme widget, where all labeling happens"""
-
 import functools
 import html
 import math
 import os
 import os.path as osp
 import re
 import webbrowser
@@ -72,15 +70,15 @@
 
         self.filename = None
         self.image_path = None
         self.image_data = None
         self.label_file = None
         self.other_data = {}
 
-        # see configs/labelme_config.yaml for valid configuration
+        # see configs/anylabeling_config.yaml for valid configuration
         if config is None:
             config = get_config()
         self._config = config
 
         # set default shape colors
         Shape.line_color = QtGui.QColor(*self._config["shape"]["line_color"])
         Shape.fill_color = QtGui.QColor(*self._config["shape"]["fill_color"])
@@ -970,15 +968,15 @@
 
         if config["file_search"]:
             self.file_search.setText(config["file_search"])
             self.file_search_changed()
 
         # XXX: Could be completely declarative.
         # Restore application settings.
-        self.settings = QtCore.QSettings("labelme", "labelme")
+        self.settings = QtCore.QSettings("anylabeling", "anylabeling")
         self.recent_files = self.settings.value("recent_files", []) or []
         size = self.settings.value("window/size", QtCore.QSize(600, 500))
         position = self.settings.value("window/position", QtCore.QPoint(0, 0))
         # state = self.settings.value("window/state", QtCore.QByteArray())
         self.resize(size)
         self.move(position)
         # or simply:
```

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.0.6/anylabeling/views/labeling/label_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""This module defines labelme wrapper and related functions"""
+"""This module defines labeling wrapper and related functions"""
 
 from PyQt5.QtWidgets import QVBoxLayout, QWidget
 
 from .label_widget import LabelmeWidget
 
 
 class LabelingWrapper(QWidget):
-    """Wrapper widget for labelme module"""
+    """Wrapper widget for labeling module"""
 
     def __init__(self, parent):
         super().__init__()
         self.parent = parent
 
-        # Create a labelme widget
+        # Create a labeling widget
         view = LabelmeWidget(self)
 
-        # Create the main layout and put labelme into
+        # Create the main layout and put labeling into
         main_layout = QVBoxLayout()
         main_layout.setContentsMargins(0, 0, 0, 0)
         main_layout.addWidget(view)
         self.setLayout(main_layout)
```

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/logger.py` & `anylabeling-0.0.6/anylabeling/views/labeling/logger.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/shape.py` & `anylabeling-0.0.6/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/testing.py` & `anylabeling-0.0.6/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/utils/__init__.py` & `anylabeling-0.0.6/anylabeling/views/labeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.0.6/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.0.6/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.0.6/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.0.6/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.0.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.0.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.0.6/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.0.6/anylabeling/views/labeling/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.0.6/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.0.6/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.0.6/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.0.6/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.0.6/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Defines toolbar for labelme, including """
+"""Defines toolbar for anylabeling, including """
 
 from PyQt5 import QtCore, QtWidgets
 
 
 class ToolBar(QtWidgets.QToolBar):
     """Toolbar widget for labeling tool"""
```

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.0.6/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.0.6/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/maintabs.py` & `anylabeling-0.0.6/anylabeling/views/maintabs.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/mainwindow.py` & `anylabeling-0.0.6/anylabeling/views/mainwindow.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling/views/mainwindow_tabs.py` & `anylabeling-0.0.6/anylabeling/views/mainwindow_tabs.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.5/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.0.6/anylabeling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.0.5
+Version: 0.0.6
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.0.5 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.0.6 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only Description-Content-
-Type: text/markdown License-File: LICENSE
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Only Description-Content-Type: text/markdown License-File: LICENSE
                       ****** ð AnyLabeling ð ******
    Effortless data labeling with AI support from YOLO and Segment Anything!
         AnyLabeling = LabelImg + Labelme + Improved UI + Auto-labeling
 ![](https://i.imgur.com/waxVImv.png) [![PyPI](https://img.shields.io/pypi/v/
 anylabeling)](https://pypi.org/project/anylabeling) [![license](https://
 img.shields.io/github/license/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/blob/master/LICENSE) [![open issues](https://
```

### Comparing `anylabeling-0.0.5/setup.py` & `anylabeling-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     keywords="Image Annotation, Machine Learning, Deep Learning",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
     ],
     include_package_data=True,
```

