# Comparing `tmp/anylabeling-0.1.0.tar.gz` & `tmp/anylabeling-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.1.0.tar", last modified: Wed Apr 12 14:08:58 2023, max compression
+gzip compressed data, was "anylabeling-0.1.1.tar", last modified: Wed Apr 12 14:50:49 2023, max compression
```

## Comparing `anylabeling-0.1.0.tar` & `anylabeling-0.1.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.354022 anylabeling-0.1.0/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.1.0/LICENSE
--rw-r--r--   0 vietanhdev   (501) staff       (20)      112 2023-04-12 01:46:44.000000 anylabeling-0.1.0/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 14:08:58.353872 anylabeling-0.1.0/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.1.0/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.338033 anylabeling-0.1.0/anylabeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       24 2023-04-12 13:22:41.000000 anylabeling-0.1.0/anylabeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1062 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/app.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      114 2023-04-12 13:33:27.000000 anylabeling-0.1.0/anylabeling/app_info.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.339525 anylabeling-0.1.0/anylabeling/configs/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/configs/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.339651 anylabeling-0.1.0/anylabeling/configs/__pycache__/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.1.0/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/configs/anylabeling_config.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)      315 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/configs/autolabel_segment_anything.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/configs/autolabel_yolov5m.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/configs/autolabel_yolov5s.yaml
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.339869 anylabeling-0.1.0/anylabeling/resources/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/resources/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)   477689 2023-04-12 01:37:51.000000 anylabeling-0.1.0/anylabeling/resources/resources.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.340275 anylabeling-0.1.0/anylabeling/services/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/services/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.341000 anylabeling-0.1.0/anylabeling/services/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3520 2023-04-12 13:27:43.000000 anylabeling-0.1.0/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5371 2023-04-12 13:27:43.000000 anylabeling-0.1.0/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9862 2023-04-12 13:51:14.000000 anylabeling-0.1.0/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1284 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5152 2023-04-12 13:27:43.000000 anylabeling-0.1.0/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/utils.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.341223 anylabeling-0.1.0/anylabeling/views/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/views/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.341563 anylabeling-0.1.0/anylabeling/views/common/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/views/common/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/views/common/tableview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.342720 anylabeling-0.1.0/anylabeling/views/labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:53:51.000000 anylabeling-0.1.0/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5590 2023-04-12 13:22:41.000000 anylabeling-0.1.0/anylabeling/views/labeling/__main__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2763 2023-04-12 02:01:24.000000 anylabeling-0.1.0/anylabeling/views/labeling/config.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.351073 anylabeling-0.1.0/anylabeling/views/labeling/icons/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6148 2023-04-09 05:07:05.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/.DS_Store
--rw-r--r--   0 vietanhdev   (501) staff       (20)        8 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/app.icns
--rw-r--r--   0 vietanhdev   (501) staff       (20)    31379 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/app.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1645 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/app.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    28068 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6844 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/cancel.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    11383 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/cartesian.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15818 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/circle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/color-line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    23824 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/color.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/color_line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10021 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/copy.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7842 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/delete.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/done.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22232 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/done.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15023 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/edit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7718 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/expert.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      278 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/expert1.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      335 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/expert2.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    37652 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/eye.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8059 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/feBlend-icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/file.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    17368 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/fit-width.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2186 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/fit-window.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2262 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/fit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4156 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/format_createml.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      786 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/format_voc.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      675 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/format_yolo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14479 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/help.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)  1128131 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/icon.icns
--rw-r--r--   0 vietanhdev   (501) staff       (20)   183198 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/icon.ico
--rw-r--r--   0 vietanhdev   (501) staff       (20)    44771 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2381 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/labels.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    36694 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/labels.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7253 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/line-strip.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9457 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      977 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/new.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7482 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/next.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26255 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/objects.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/open.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10572 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/paste.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    13847 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/point.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14286 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/polygon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7275 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/prev.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22460 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/quit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2136 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/rectangle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3637 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/resetall.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2811 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/save-as.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6118 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/save.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2004 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/undo-cross.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2018 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/undo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    18083 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/upload_brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3041 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/verify.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1099 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/zoom-in.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1074 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/zoom-out.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1139 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/zoom.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5945 2023-04-12 13:18:06.000000 anylabeling-0.1.0/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    89228 2023-04-12 14:03:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      610 2023-04-12 01:47:51.000000 anylabeling-0.1.0/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1786 2023-04-12 01:57:00.000000 anylabeling-0.1.0/anylabeling/views/labeling/logger.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/shape.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.351844 anylabeling-0.1.0/anylabeling/views/labeling/utils/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      510 2023-04-12 13:55:17.000000 anylabeling-0.1.0/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-12 13:27:43.000000 anylabeling-0.1.0/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.353275 anylabeling-0.1.0/anylabeling/views/labeling/widgets/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-12 13:27:43.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.353655 anylabeling-0.1.0/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6889 2023-04-12 13:27:43.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    46815 2023-04-12 13:54:32.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8023 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5778 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1394 2023-04-12 01:47:30.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      915 2023-04-12 13:44:49.000000 anylabeling-0.1.0/anylabeling/views/mainwindow.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.338913 anylabeling-0.1.0/anylabeling.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 14:08:58.000000 anylabeling-0.1.0/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5055 2023-04-12 14:08:58.000000 anylabeling-0.1.0/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-12 14:08:58.000000 anylabeling-0.1.0/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-12 14:08:58.000000 anylabeling-0.1.0/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      235 2023-04-12 14:08:58.000000 anylabeling-0.1.0/anylabeling.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-12 14:08:58.000000 anylabeling-0.1.0/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.1.0/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-12 14:08:58.354066 anylabeling-0.1.0/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2454 2023-04-12 13:17:03.000000 anylabeling-0.1.0/setup.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.973286 anylabeling-0.1.1/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.1.1/LICENSE
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      112 2023-04-12 01:46:44.000000 anylabeling-0.1.1/MANIFEST.in
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 14:50:49.973114 anylabeling-0.1.1/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.1.1/README.md
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.949183 anylabeling-0.1.1/anylabeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       24 2023-04-12 13:22:41.000000 anylabeling-0.1.1/anylabeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1062 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/app.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      114 2023-04-12 14:50:44.000000 anylabeling-0.1.1/anylabeling/app_info.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.951160 anylabeling-0.1.1/anylabeling/configs/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.1/anylabeling/configs/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.951292 anylabeling-0.1.1/anylabeling/configs/__pycache__/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.1.1/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/configs/anylabeling_config.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      315 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/configs/autolabel_segment_anything.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/configs/autolabel_yolov5m.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/configs/autolabel_yolov5s.yaml
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.951700 anylabeling-0.1.1/anylabeling/resources/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.1/anylabeling/resources/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   477689 2023-04-12 01:37:51.000000 anylabeling-0.1.1/anylabeling/resources/resources.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.952386 anylabeling-0.1.1/anylabeling/services/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.1/anylabeling/services/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.953248 anylabeling-0.1.1/anylabeling/services/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3520 2023-04-12 13:27:43.000000 anylabeling-0.1.1/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5371 2023-04-12 13:27:43.000000 anylabeling-0.1.1/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9862 2023-04-12 13:51:14.000000 anylabeling-0.1.1/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1323 2023-04-12 14:49:36.000000 anylabeling-0.1.1/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5152 2023-04-12 13:27:43.000000 anylabeling-0.1.1/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/utils.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.953536 anylabeling-0.1.1/anylabeling/views/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.1/anylabeling/views/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.953919 anylabeling-0.1.1/anylabeling/views/common/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.1/anylabeling/views/common/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.1.1/anylabeling/views/common/tableview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.1.1/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.955143 anylabeling-0.1.1/anylabeling/views/labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:53:51.000000 anylabeling-0.1.1/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5590 2023-04-12 13:22:41.000000 anylabeling-0.1.1/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2763 2023-04-12 02:01:24.000000 anylabeling-0.1.1/anylabeling/views/labeling/config.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.970207 anylabeling-0.1.1/anylabeling/views/labeling/icons/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6148 2023-04-09 05:07:05.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/.DS_Store
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        8 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/app.icns
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    31379 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/app.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1645 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/app.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    28068 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/brain.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6844 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/cancel.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    11383 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/cartesian.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    15818 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/circle.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/color-line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    23824 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/color.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/color_line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10021 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/copy.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7842 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/delete.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/done.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    22232 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/done.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    15023 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/edit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7718 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/expert.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      278 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/expert1.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      335 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/expert2.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    37652 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/eye.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8059 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/feBlend-icon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/file.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    17368 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/fit-width.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2186 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/fit-window.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2262 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/fit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4156 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/format_createml.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      786 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/format_voc.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      675 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/format_yolo.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    14479 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/help.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)  1128131 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/icon.icns
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   183198 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/icon.ico
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    44771 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/icon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2381 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/labels.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    36694 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/labels.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7253 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/line-strip.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9457 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      977 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/new.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7482 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/next.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26255 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/objects.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/open.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10572 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/paste.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    13847 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/point.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    14286 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/polygon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7275 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/prev.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    22460 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/quit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2136 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/rectangle.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3637 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/resetall.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2811 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/save-as.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6118 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/save.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2004 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/undo-cross.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2018 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/undo.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    18083 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/upload_brain.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3041 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/verify.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1099 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/zoom-in.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1074 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/zoom-out.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1139 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/icons/zoom.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5945 2023-04-12 13:18:06.000000 anylabeling-0.1.1/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    89220 2023-04-12 14:49:37.000000 anylabeling-0.1.1/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      610 2023-04-12 01:47:51.000000 anylabeling-0.1.1/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1786 2023-04-12 01:57:00.000000 anylabeling-0.1.1/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.971047 anylabeling-0.1.1/anylabeling/views/labeling/utils/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      510 2023-04-12 14:49:37.000000 anylabeling-0.1.1/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-12 13:27:43.000000 anylabeling-0.1.1/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.972494 anylabeling-0.1.1/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-12 13:27:43.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.972880 anylabeling-0.1.1/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7373 2023-04-12 14:49:36.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    46602 2023-04-12 14:49:36.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8027 2023-04-12 14:39:39.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5778 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1394 2023-04-12 01:47:30.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.1.1/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      915 2023-04-12 13:44:49.000000 anylabeling-0.1.1/anylabeling/views/mainwindow.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:50:49.950426 anylabeling-0.1.1/anylabeling.egg-info/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 14:50:49.000000 anylabeling-0.1.1/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5055 2023-04-12 14:50:49.000000 anylabeling-0.1.1/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-12 14:50:49.000000 anylabeling-0.1.1/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-12 14:50:49.000000 anylabeling-0.1.1/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      235 2023-04-12 14:50:49.000000 anylabeling-0.1.1/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-12 14:50:49.000000 anylabeling-0.1.1/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.1.1/pyproject.toml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-12 14:50:49.973328 anylabeling-0.1.1/setup.cfg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2454 2023-04-12 13:17:03.000000 anylabeling-0.1.1/setup.py
```

### Comparing `anylabeling-0.1.0/LICENSE` & `anylabeling-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/PKG-INFO` & `anylabeling-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.1.0
+Version: 0.1.1
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
-Metadata-Version: 2.1 Name: anylabeling Version: 0.1.0 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.1.1 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.1.0/README.md` & `anylabeling-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/app.py` & `anylabeling-0.1.1/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.1.1/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/configs/autolabel_yolov5m.yaml` & `anylabeling-0.1.1/anylabeling/configs/autolabel_yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/configs/autolabel_yolov5s.yaml` & `anylabeling-0.1.1/anylabeling/configs/autolabel_yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/resources/resources.py` & `anylabeling-0.1.1/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.1.1/anylabeling/services/auto_labeling/model.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.1.1/anylabeling/services/auto_labeling/model_manager.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/services/auto_labeling/segment_anything.py` & `anylabeling-0.1.1/anylabeling/services/auto_labeling/segment_anything.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.1.1/anylabeling/services/auto_labeling/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,14 @@
         """
 
         self.shapes = shapes
         self.replace = replace
 
 
 class AutoLabelingMode:
-    NONE = None
     OBJECT = "AUTOLABEL_OBJECT"
     ADD = "AUTOLABEL_ADD"
     REMOVE = "AUTOLABEL_REMOVE"
     POINT = "point"
     RECTANGLE = "rectangle"
 
     def __init__(self, edit_mode, shape_type):
@@ -39,7 +38,10 @@
     def __eq__(self, other):
         if not isinstance(other, AutoLabelingMode):
             return False
         return (
             self.edit_mode == other.edit_mode
             and self.shape_type == other.shape_type
         )
+
+
+AutoLabelingMode.NONE = AutoLabelingMode(None, None)
```

### Comparing `anylabeling-0.1.0/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.1.1/anylabeling/services/auto_labeling/yolov5.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/common/tableview.py` & `anylabeling-0.1.1/anylabeling/views/common/tableview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/common/toaster.py` & `anylabeling-0.1.1/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/__main__.py` & `anylabeling-0.1.1/anylabeling/views/labeling/__main__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/config.py` & `anylabeling-0.1.1/anylabeling/views/labeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/.DS_Store` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/app.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/app.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/app.svg` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/app.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/brain.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/cancel.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/cartesian.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/cartesian.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/circle.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/circle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/color-line.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/color.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/color.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/color_line.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/color_line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/copy.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/copy.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/delete.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/delete.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/done.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/done.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/done.svg` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/done.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/edit.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/edit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/expert.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/expert.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/eye.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/eye.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/feBlend-icon.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/file.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/file.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/fit-width.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/fit-window.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/fit.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/fit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/format_createml.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/format_createml.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/format_voc.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/format_voc.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/format_yolo.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/format_yolo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/help.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/help.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/icon.icns` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/icon.ico` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/icon.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/labels.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/labels.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/labels.svg` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/line-strip.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/line-strip.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/line.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/new.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/new.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/next.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/next.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/objects.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/objects.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/open.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/open.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/paste.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/paste.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/point.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/point.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/polygon.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/prev.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/prev.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/quit.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/quit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/rectangle.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/resetall.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/resetall.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/save-as.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/save.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/save.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/undo-cross.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/undo.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/undo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/upload_brain.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/upload_brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/verify.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/verify.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/zoom-in.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/zoom-out.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/icons/zoom.png` & `anylabeling-0.1.1/anylabeling/views/labeling/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/label_file.py` & `anylabeling-0.1.1/anylabeling/views/labeling/label_file.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.1.1/anylabeling/views/labeling/label_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -860,17 +860,14 @@
         )
         self.auto_labeling_widget.clear_auto_labeling_action_requested.connect(
             self.clear_auto_labeling_marks
         )
         self.auto_labeling_widget.finish_auto_labeling_object_action_requested.connect(
             self.finish_auto_labeling_object
         )
-        self.canvas.auto_labeling_mode_changed.connect(
-            lambda mode: self.auto_labeling_widget.update_button_colors(mode)
-        )
         self.auto_labeling_widget.hide()  # Hide by default
         central_layout.addWidget(self.label_instruction)
         central_layout.addWidget(self.auto_labeling_widget)
         central_layout.addWidget(scroll_area)
         layout.addItem(central_layout)
 
         # Save central area for resize
@@ -1197,14 +1194,18 @@
                 self.actions.create_point_mode.setEnabled(True)
                 self.actions.create_line_strip_mode.setEnabled(False)
             else:
                 raise ValueError(f"Unsupported create_mode: {create_mode}")
         self.actions.edit_mode.setEnabled(not edit)
 
     def set_edit_mode(self):
+        # Diable auto labeling
+        self.clear_auto_labeling_marks()
+        self.auto_labeling_widget.set_auto_labeling_mode(None)
+
         self.toggle_draw_mode(True)
 
     def update_file_menu(self):
         current = self.filename
 
         def exists(filename):
             return osp.exists(str(filename))
```

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.1.1/anylabeling/views/labeling/label_wrapper.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/logger.py` & `anylabeling-0.1.1/anylabeling/views/labeling/logger.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/shape.py` & `anylabeling-0.1.1/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/testing.py` & `anylabeling-0.1.1/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.1.1/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.1.1/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.1.1/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.1.1/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.1.1/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,16 +90,20 @@
         self.button_close.clicked.connect(self.unload_and_hide)
 
         # Handle model select combobox
         self.model_select_combobox.currentIndexChanged.connect(
             self.on_model_select_combobox_changed
         )
 
+        self.auto_labeling_mode_changed.connect(self.update_button_colors)
+        self.auto_labeling_mode = AutoLabelingMode.NONE
+        self.auto_labeling_mode_changed.emit(self.auto_labeling_mode)
+
     @pyqtSlot()
-    def update_button_colors(self, auto_labeling_mode):
+    def update_button_colors(self):
         """Update button colors"""
         style_sheet = """
             text-align: center;
             margin-right: 3px;
             border-radius: 5px;
             padding: 4px 8px;
             border: 1px solid #999999;
@@ -109,34 +113,41 @@
             self.button_remove_point,
             self.button_add_rect,
             self.button_clear,
             self.button_undo,
             self.button_finish_object,
         ]:
             button.setStyleSheet(style_sheet + "background-color: #ffffff;")
-        if auto_labeling_mode.edit_mode == AutoLabelingMode.ADD:
-            if auto_labeling_mode.shape_type == AutoLabelingMode.POINT:
+        if self.auto_labeling_mode == AutoLabelingMode.NONE:
+            return
+        if self.auto_labeling_mode.edit_mode == AutoLabelingMode.ADD:
+            if self.auto_labeling_mode.shape_type == AutoLabelingMode.POINT:
                 self.button_add_point.setStyleSheet(
                     style_sheet + "background-color: #00ff00;"
                 )
-            elif auto_labeling_mode.shape_type == AutoLabelingMode.RECTANGLE:
+            elif (
+                self.auto_labeling_mode.shape_type
+                == AutoLabelingMode.RECTANGLE
+            ):
                 self.button_add_rect.setStyleSheet(
                     style_sheet + "background-color: #00ff00;"
                 )
-        elif auto_labeling_mode.edit_mode == AutoLabelingMode.REMOVE:
-            if auto_labeling_mode.shape_type == AutoLabelingMode.POINT:
+        elif self.auto_labeling_mode.edit_mode == AutoLabelingMode.REMOVE:
+            if self.auto_labeling_mode.shape_type == AutoLabelingMode.POINT:
                 self.button_remove_point.setStyleSheet(
                     style_sheet + "background-color: #ff0000;"
                 )
 
-    def set_auto_labeling_mode(self, edit_mode, shape_type):
+    def set_auto_labeling_mode(self, edit_mode, shape_type=None):
         """Set auto labeling mode"""
-        self.auto_labeling_mode_changed.emit(
-            AutoLabelingMode(edit_mode, shape_type)
-        )
+        if edit_mode is None:
+            self.auto_labeling_mode = AutoLabelingMode.NONE
+        else:
+            self.auto_labeling_mode = AutoLabelingMode(edit_mode, shape_type)
+        self.auto_labeling_mode_changed.emit(self.auto_labeling_mode)
 
     def run_prediction(self):
         """Run prediction"""
         if self.parent.image_path:
             self.prediction_requested.emit(self.parent.image)
 
     def unload_and_hide(self):
```

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.1.1/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.1.1/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.1.1/anylabeling/views/labeling/widgets/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     scroll_request = QtCore.pyqtSignal(int, int)
     new_shape = QtCore.pyqtSignal()
     selection_changed = QtCore.pyqtSignal(list)
     shape_moved = QtCore.pyqtSignal()
     drawing_polygon = QtCore.pyqtSignal(bool)
     vertex_selected = QtCore.pyqtSignal(bool)
     auto_labeling_marks_updated = QtCore.pyqtSignal(list)
-    auto_labeling_mode_changed = QtCore.pyqtSignal(AutoLabelingMode)
 
     CREATE, EDIT = 0, 1
 
     # polygon, rectangle, line, or point
     _create_mode = "polygon"
 
     _fill_drawing = False
@@ -95,19 +94,22 @@
         self.setFocusPolicy(QtCore.Qt.WheelFocus)
         self.show_cross_line = True
         self.show_shape_groups = True
         self.show_texts = True
 
     def set_auto_labeling_mode(self, mode: AutoLabelingMode):
         """Set auto labeling mode"""
-        self.is_auto_labeling = True
-        self.auto_labeling_mode = mode
-        self.create_mode = mode.shape_type
-        self.parent.toggle_draw_mode(False, mode.shape_type)
-        self.auto_labeling_mode_changed.emit(mode)
+        if mode == AutoLabelingMode.NONE:
+            self.is_auto_labeling = False
+            self.auto_labeling_mode = mode
+        else:
+            self.is_auto_labeling = True
+            self.auto_labeling_mode = mode
+            self.create_mode = mode.shape_type
+            self.parent.toggle_draw_mode(False, mode.shape_type)
 
     def fill_drawing(self):
         """Get option to fill shapes by color"""
         return self._fill_drawing
 
     def set_fill_drawing(self, value):
         """Set shape filling option"""
@@ -194,22 +196,16 @@
         """Check if user is editing (mode==EDIT)"""
         return self.mode == self.EDIT
 
     def set_auto_labeling(self, value=True):
         """Set auto labeling mode"""
         self.is_auto_labeling = value
         if self.auto_labeling_mode is None:
-            self.auto_labeling_mode = AutoLabelingMode.get_default_mode()
-            self.parent.toggle_draw_mode(
-                False, self.auto_labeling_mode.shape_type
-            )
-        if not self.auto_labeling_mode:
-            self.auto_labeling_mode_changed.emit(None)
-        else:
-            self.auto_labeling_mode_changed.emit(self.auto_labeling_mode)
+            self.auto_labeling_mode = AutoLabelingMode.NONE
+            self.parent.toggle_draw_mode(False, "rectangle")
 
     def get_mode(self):
         """Get current mode"""
         if self.is_auto_labeling:
             return "Auto Labeling"
         if self.mode == self.CREATE:
             return "Drawing"
```

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.1.1/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.1.1/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.1.1/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self.edit_group_id.setPlaceholderText("Group ID")
         self.edit_group_id.setValidator(
             QtGui.QRegularExpressionValidator(
                 QtCore.QRegularExpression(r"\d*"), None
             )
         )
         layout = QtWidgets.QVBoxLayout()
-        layout.setContentsMargins(0, 0, 0, 0)
+        layout.setContentsMargins(10, 10, 10, 10)
         if show_text_field:
             layout_edit = QtWidgets.QHBoxLayout()
             layout_edit.addWidget(self.edit, 6)
             layout_edit.addWidget(self.edit_group_id, 2)
             layout.addLayout(layout_edit)
         # buttons
         self.button_box = bb = QtWidgets.QDialogButtonBox(
```

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.1.1/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.1.1/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.1.1/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.1.1/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling/views/mainwindow.py` & `anylabeling-0.1.1/anylabeling/views/mainwindow.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.1.1/anylabeling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.1.0
+Version: 0.1.1
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
-Metadata-Version: 2.1 Name: anylabeling Version: 0.1.0 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.1.1 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.1.0/anylabeling.egg-info/SOURCES.txt` & `anylabeling-0.1.1/anylabeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.0/setup.py` & `anylabeling-0.1.1/setup.py`

 * *Files identical despite different names*

