# Comparing `tmp/anylabeling-0.0.6.tar.gz` & `tmp/anylabeling-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.0.6.tar", last modified: Wed Apr 12 01:50:59 2023, max compression
+gzip compressed data, was "anylabeling-0.0.8.tar", last modified: Wed Apr 12 01:58:12 2023, max compression
```

## Comparing `anylabeling-0.0.6.tar` & `anylabeling-0.0.8.tar`

### file list

```diff
@@ -1,137 +1,138 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.980353 anylabeling-0.0.6/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.0.6/LICENSE
--rw-r--r--   0 vietanhdev   (501) staff       (20)      112 2023-04-12 01:46:44.000000 anylabeling-0.0.6/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 01:50:59.980139 anylabeling-0.0.6/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.0.6/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.961061 anylabeling-0.0.6/anylabeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       22 2023-04-12 01:50:53.000000 anylabeling-0.0.6/anylabeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1062 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/app.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.962522 anylabeling-0.0.6/anylabeling/configs/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/configs/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.962660 anylabeling-0.0.6/anylabeling/configs/__pycache__/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.0.6/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/configs/anylabeling_config.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)      315 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/configs/autolabel_segment_anything.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/configs/autolabel_yolov5m.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/configs/autolabel_yolov5s.yaml
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.963108 anylabeling-0.0.6/anylabeling/resources/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/resources/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)   477689 2023-04-12 01:37:51.000000 anylabeling-0.0.6/anylabeling/resources/resources.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.963527 anylabeling-0.0.6/anylabeling/services/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/services/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.964493 anylabeling-0.0.6/anylabeling/services/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3443 2023-04-12 01:31:17.000000 anylabeling-0.0.6/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5355 2023-04-12 01:27:25.000000 anylabeling-0.0.6/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9861 2023-04-12 01:26:18.000000 anylabeling-0.0.6/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1284 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5151 2023-04-12 01:26:25.000000 anylabeling-0.0.6/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/utils.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.964986 anylabeling-0.0.6/anylabeling/views/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/views/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.965347 anylabeling-0.0.6/anylabeling/views/common/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/views/common/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/views/common/tableview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.0.6/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.966481 anylabeling-0.0.6/anylabeling/views/labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5766 2023-04-12 01:48:44.000000 anylabeling-0.0.6/anylabeling/views/labeling/__main__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2725 2023-04-12 01:48:11.000000 anylabeling-0.0.6/anylabeling/views/labeling/config.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.977013 anylabeling-0.0.6/anylabeling/views/labeling/icons/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6148 2023-04-09 05:07:05.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/.DS_Store
--rw-r--r--   0 vietanhdev   (501) staff       (20)        8 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/app.icns
--rw-r--r--   0 vietanhdev   (501) staff       (20)    31379 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/app.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1645 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/app.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    28068 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6844 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/cancel.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    11383 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/cartesian.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15818 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/circle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/color-line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    23824 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/color.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/color_line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10021 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/copy.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7842 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/delete.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/done.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22232 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/done.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15023 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/edit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7718 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/expert.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      278 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/expert1.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      335 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/expert2.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    37652 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/eye.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8059 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/feBlend-icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/file.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    17368 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/fit-width.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2186 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/fit-window.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2262 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/fit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4156 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/format_createml.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      786 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/format_voc.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      675 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/format_yolo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14479 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/help.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)  1128131 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/icon.icns
--rw-r--r--   0 vietanhdev   (501) staff       (20)   183198 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/icon.ico
--rw-r--r--   0 vietanhdev   (501) staff       (20)    44771 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2381 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/labels.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    36694 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/labels.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7253 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/line-strip.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9457 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      977 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/new.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7482 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/next.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26255 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/objects.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/open.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10572 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/paste.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    13847 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/point.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14286 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/polygon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7275 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/prev.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22460 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/quit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2136 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/rectangle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3637 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/resetall.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2811 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/save-as.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6118 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/save.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2004 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/undo-cross.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2018 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/undo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    18083 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/upload_brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3041 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/verify.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1099 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/zoom-in.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1074 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/zoom-out.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1139 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/icons/zoom.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6409 2023-04-12 01:48:23.000000 anylabeling-0.0.6/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    88710 2023-04-12 01:49:13.000000 anylabeling-0.0.6/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      610 2023-04-12 01:47:51.000000 anylabeling-0.0.6/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1811 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/logger.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/shape.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.977895 anylabeling-0.0.6/anylabeling/views/labeling/utils/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.979443 anylabeling-0.0.6/anylabeling/views/labeling/widgets/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.979840 anylabeling-0.0.6/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6906 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    46264 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8023 2023-04-08 19:49:25.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5778 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1394 2023-04-12 01:47:30.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      768 2023-04-08 20:09:45.000000 anylabeling-0.0.6/anylabeling/views/maintabs.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      981 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/mainwindow.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1458 2023-04-11 17:52:02.000000 anylabeling-0.0.6/anylabeling/views/mainwindow_tabs.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:50:59.961857 anylabeling-0.0.6/anylabeling.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 01:50:59.000000 anylabeling-0.0.6/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5059 2023-04-12 01:50:59.000000 anylabeling-0.0.6/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-12 01:50:59.000000 anylabeling-0.0.6/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-12 01:50:59.000000 anylabeling-0.0.6/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      235 2023-04-12 01:50:59.000000 anylabeling-0.0.6/anylabeling.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-12 01:50:59.000000 anylabeling-0.0.6/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.0.6/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-12 01:50:59.980407 anylabeling-0.0.6/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2454 2023-04-12 01:44:44.000000 anylabeling-0.0.6/setup.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.400581 anylabeling-0.0.8/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.0.8/LICENSE
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      112 2023-04-12 01:46:44.000000 anylabeling-0.0.8/MANIFEST.in
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 01:58:12.400420 anylabeling-0.0.8/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.0.8/README.md
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.379545 anylabeling-0.0.8/anylabeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       50 2023-04-12 01:58:09.000000 anylabeling-0.0.8/anylabeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1062 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/app.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.381271 anylabeling-0.0.8/anylabeling/configs/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.8/anylabeling/configs/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.381405 anylabeling-0.0.8/anylabeling/configs/__pycache__/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.0.8/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/configs/anylabeling_config.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      315 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/configs/autolabel_segment_anything.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/configs/autolabel_yolov5m.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/configs/autolabel_yolov5s.yaml
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.381630 anylabeling-0.0.8/anylabeling/resources/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.8/anylabeling/resources/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   477689 2023-04-12 01:37:51.000000 anylabeling-0.0.8/anylabeling/resources/resources.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.382337 anylabeling-0.0.8/anylabeling/services/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.8/anylabeling/services/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.383085 anylabeling-0.0.8/anylabeling/services/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3443 2023-04-12 01:31:17.000000 anylabeling-0.0.8/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5355 2023-04-12 01:27:25.000000 anylabeling-0.0.8/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9861 2023-04-12 01:26:18.000000 anylabeling-0.0.8/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1284 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5151 2023-04-12 01:26:25.000000 anylabeling-0.0.8/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/utils.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.383566 anylabeling-0.0.8/anylabeling/views/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.8/anylabeling/views/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.383927 anylabeling-0.0.8/anylabeling/views/common/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.8/anylabeling/views/common/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.0.8/anylabeling/views/common/tableview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.0.8/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.385136 anylabeling-0.0.8/anylabeling/views/labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:53:51.000000 anylabeling-0.0.8/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5569 2023-04-12 01:56:58.000000 anylabeling-0.0.8/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2725 2023-04-12 01:48:11.000000 anylabeling-0.0.8/anylabeling/views/labeling/config.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.397391 anylabeling-0.0.8/anylabeling/views/labeling/icons/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6148 2023-04-09 05:07:05.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/.DS_Store
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        8 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/app.icns
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    31379 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/app.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1645 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/app.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    28068 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/brain.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6844 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/cancel.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    11383 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/cartesian.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    15818 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/circle.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/color-line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    23824 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/color.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/color_line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10021 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/copy.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7842 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/delete.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/done.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    22232 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/done.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    15023 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/edit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7718 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/expert.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      278 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/expert1.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      335 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/expert2.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    37652 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/eye.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8059 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/feBlend-icon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/file.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    17368 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/fit-width.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2186 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/fit-window.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2262 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/fit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4156 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/format_createml.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      786 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/format_voc.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      675 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/format_yolo.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    14479 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/help.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)  1128131 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/icon.icns
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   183198 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/icon.ico
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    44771 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/icon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2381 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/labels.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    36694 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/labels.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7253 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/line-strip.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9457 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      977 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/new.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7482 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/next.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26255 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/objects.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/open.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10572 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/paste.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    13847 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/point.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    14286 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/polygon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7275 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/prev.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    22460 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/quit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2136 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/rectangle.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3637 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/resetall.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2811 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/save-as.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6118 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/save.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2004 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/undo-cross.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2018 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/undo.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    18083 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/upload_brain.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3041 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/verify.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1099 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/zoom-in.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1074 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/zoom-out.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1139 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/icons/zoom.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5909 2023-04-12 01:56:33.000000 anylabeling-0.0.8/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    88726 2023-04-12 01:55:33.000000 anylabeling-0.0.8/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      610 2023-04-12 01:47:51.000000 anylabeling-0.0.8/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1786 2023-04-12 01:57:00.000000 anylabeling-0.0.8/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.398313 anylabeling-0.0.8/anylabeling/views/labeling/utils/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.399785 anylabeling-0.0.8/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.400193 anylabeling-0.0.8/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6906 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    46264 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8023 2023-04-08 19:49:25.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5778 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1394 2023-04-12 01:47:30.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      768 2023-04-08 20:09:45.000000 anylabeling-0.0.8/anylabeling/views/maintabs.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      981 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/mainwindow.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1458 2023-04-11 17:52:02.000000 anylabeling-0.0.8/anylabeling/views/mainwindow_tabs.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:58:12.380594 anylabeling-0.0.8/anylabeling.egg-info/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 01:58:12.000000 anylabeling-0.0.8/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5098 2023-04-12 01:58:12.000000 anylabeling-0.0.8/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-12 01:58:12.000000 anylabeling-0.0.8/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-12 01:58:12.000000 anylabeling-0.0.8/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      235 2023-04-12 01:58:12.000000 anylabeling-0.0.8/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-12 01:58:12.000000 anylabeling-0.0.8/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.0.8/pyproject.toml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-12 01:58:12.400624 anylabeling-0.0.8/setup.cfg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2454 2023-04-12 01:44:44.000000 anylabeling-0.0.8/setup.py
```

### Comparing `anylabeling-0.0.6/LICENSE` & `anylabeling-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/PKG-INFO` & `anylabeling-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.0.6
+Version: 0.0.8
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
-Metadata-Version: 2.1 Name: anylabeling Version: 0.0.6 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.0.8 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.0.6/README.md` & `anylabeling-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/app.py` & `anylabeling-0.0.8/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.0.8/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/configs/autolabel_yolov5m.yaml` & `anylabeling-0.0.8/anylabeling/configs/autolabel_yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/configs/autolabel_yolov5s.yaml` & `anylabeling-0.0.8/anylabeling/configs/autolabel_yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/resources/resources.py` & `anylabeling-0.0.8/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.0.8/anylabeling/services/auto_labeling/model.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.0.8/anylabeling/services/auto_labeling/model_manager.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/services/auto_labeling/segment_anything.py` & `anylabeling-0.0.8/anylabeling/services/auto_labeling/segment_anything.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.0.8/anylabeling/services/auto_labeling/types.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.0.8/anylabeling/services/auto_labeling/yolov5.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/common/tableview.py` & `anylabeling-0.0.8/anylabeling/views/common/tableview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/common/toaster.py` & `anylabeling-0.0.8/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/__main__.py` & `anylabeling-0.0.8/anylabeling/views/labeling/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
+__appname__ = "AnyLabeling"
+
 import argparse
 import codecs
 import logging
 import os
 import os.path as osp
 import sys
 
 import yaml
 from PyQt5 import QtCore, QtWidgets
 
-from . import __appname__, __version__
 from .config import get_config
 from .label_widget import MainWindow
 from .logger import logger
 from .utils import new_icon
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument(
-        "--version", "-V", action="store_true", help="show version"
-    )
-    parser.add_argument(
         "--reset-config", action="store_true", help="reset qt config"
     )
     parser.add_argument(
         "--logger-level",
         default="info",
         choices=["debug", "info", "warning", "fatal", "error"],
         help="logger level",
@@ -106,18 +104,14 @@
         "--epsilon",
         type=float,
         help="epsilon to find nearest vertex on canvas",
         default=argparse.SUPPRESS,
     )
     args = parser.parse_args()
 
-    if args.version:
-        print(f"{__appname__} {__version__}")
-        sys.exit(0)
-
     logger.setLevel(getattr(logging, args.logger_level.upper()))
 
     if hasattr(args, "flags"):
         if os.path.isfile(args.flags):
             with codecs.open(args.flags, "r", encoding="utf-8") as f:
                 args.flags = [line.strip() for line in f if line.strip()]
         else:
```

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/config.py` & `anylabeling-0.0.8/anylabeling/views/labeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/.DS_Store` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/app.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/app.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/app.svg` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/app.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/brain.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/cancel.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/cartesian.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/cartesian.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/circle.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/circle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/color-line.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/color.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/color.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/color_line.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/color_line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/copy.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/copy.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/delete.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/delete.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/done.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/done.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/done.svg` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/done.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/edit.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/edit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/expert.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/expert.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/eye.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/eye.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/feBlend-icon.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/file.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/file.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/fit-width.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/fit-window.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/fit.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/fit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/format_createml.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/format_createml.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/format_voc.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/format_voc.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/format_yolo.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/format_yolo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/help.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/help.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/icon.icns` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/icon.ico` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/icon.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/labels.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/labels.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/labels.svg` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/line-strip.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/line-strip.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/line.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/new.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/new.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/next.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/next.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/objects.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/objects.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/open.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/open.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/paste.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/paste.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/point.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/point.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/polygon.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/prev.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/prev.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/quit.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/quit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/rectangle.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/resetall.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/resetall.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/save-as.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/save.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/save.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/undo-cross.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/undo.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/undo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/upload_brain.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/upload_brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/verify.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/verify.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/zoom-in.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/zoom-out.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/icons/zoom.png` & `anylabeling-0.0.8/anylabeling/views/labeling/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/label_file.py` & `anylabeling-0.0.8/anylabeling/views/labeling/label_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import contextlib
 import io
 import json
 import os.path as osp
 
 import PIL.Image
 
-from . import __version__, utils
+from . import utils
 from .logger import logger
 
 PIL.Image.MAX_IMAGE_PIXELS = None
 
 
 @contextlib.contextmanager
 def io_open(name, mode):
@@ -78,27 +78,14 @@
             with io_open(filename, "r") as f:
                 data = json.load(f)
             version = data.get("version")
             if version is None:
                 logger.warning(
                     "Loading JSON file (%s) of unknown version", filename
                 )
-            elif (
-                version.split(".")[0] != __version__.split(".", maxsplit=1)[0]
-            ):
-                logger.warning(
-                    (
-                        "This JSON file (%s) may be incompatible with "
-                        "current AnyLabeling. version in file: %s, "
-                        "current version: %s"
-                    ),
-                    filename,
-                    version,
-                    __version__,
-                )
 
             if data["imageData"] is not None:
                 image_data = base64.b64decode(data["imageData"])
             else:
                 # relative path from label file to relative path from cwd
                 image_path = osp.join(osp.dirname(filename), data["imagePath"])
                 image_data = self.load_image_file(image_path)
```

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.0.8/anylabeling/views/labeling/label_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__appname__ = "AnyLabeling"
+
 import functools
 import html
 import math
 import os
 import os.path as osp
 import re
 import webbrowser
@@ -15,15 +17,15 @@
     QHBoxLayout,
     QLabel,
     QPlainTextEdit,
     QVBoxLayout,
     QWhatsThis,
 )
 
-from . import __appname__, utils
+from . import utils
 from .config import get_config
 from .label_file import LabelFile, LabelFileError
 from .logger import logger
 from .shape import Shape
 from .widgets import (
     BrightnessContrastDialog,
     Canvas,
```

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.0.8/anylabeling/views/labeling/label_wrapper.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/logger.py` & `anylabeling-0.0.8/anylabeling/views/labeling/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import termcolor
 
 if os.name == "nt":  # Windows
     import colorama
 
     colorama.init()
 
-from . import __appname__
-
 COLORS = {
     "WARNING": "yellow",
     "INFO": "white",
     "DEBUG": "blue",
     "CRITICAL": "red",
     "ERROR": "red",
 }
@@ -60,9 +58,9 @@
 
         console = logging.StreamHandler()
         console.setFormatter(color_formatter)
 
         self.addHandler(console)
 
 
-logger = logging.getLogger(__appname__)
+logger = logging.getLogger("AnyLabeling")
 logger.__class__ = ColoredLogger
```

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/shape.py` & `anylabeling-0.0.8/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/testing.py` & `anylabeling-0.0.8/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/utils/__init__.py` & `anylabeling-0.0.8/anylabeling/views/labeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.0.8/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.0.8/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.0.8/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.0.8/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.0.8/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.0.8/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.0.8/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.0.8/anylabeling/views/labeling/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.0.8/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.0.8/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.0.8/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.0.8/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.0.8/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.0.8/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.0.8/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/maintabs.py` & `anylabeling-0.0.8/anylabeling/views/maintabs.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/mainwindow.py` & `anylabeling-0.0.8/anylabeling/views/mainwindow.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling/views/mainwindow_tabs.py` & `anylabeling-0.0.8/anylabeling/views/mainwindow_tabs.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.6/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.0.8/anylabeling.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.0.6
+Version: 0.0.8
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
-Metadata-Version: 2.1 Name: anylabeling Version: 0.0.6 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.0.8 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.0.6/anylabeling.egg-info/SOURCES.txt` & `anylabeling-0.0.8/anylabeling.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 anylabeling/views/__init__.py
 anylabeling/views/maintabs.py
 anylabeling/views/mainwindow.py
 anylabeling/views/mainwindow_tabs.py
 anylabeling/views/common/__init__.py
 anylabeling/views/common/tableview.py
 anylabeling/views/common/toaster.py
+anylabeling/views/labeling/__init__.py
 anylabeling/views/labeling/__main__.py
 anylabeling/views/labeling/config.py
 anylabeling/views/labeling/label_file.py
 anylabeling/views/labeling/label_widget.py
 anylabeling/views/labeling/label_wrapper.py
 anylabeling/views/labeling/logger.py
 anylabeling/views/labeling/shape.py
```

### Comparing `anylabeling-0.0.6/setup.py` & `anylabeling-0.0.8/setup.py`

 * *Files identical despite different names*

