# Comparing `tmp/anylabeling-0.0.9.tar.gz` & `tmp/anylabeling-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.0.9.tar", last modified: Wed Apr 12 02:01:50 2023, max compression
+gzip compressed data, was "anylabeling-0.1.0.tar", last modified: Wed Apr 12 14:08:58 2023, max compression
```

## Comparing `anylabeling-0.0.9.tar` & `anylabeling-0.1.0.tar`

### file list

```diff
@@ -1,138 +1,137 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.294983 anylabeling-0.0.9/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.0.9/LICENSE
--rw-r--r--   0 vietanhdev   (501) staff       (20)      112 2023-04-12 01:46:44.000000 anylabeling-0.0.9/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 02:01:50.294812 anylabeling-0.0.9/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.0.9/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.275519 anylabeling-0.0.9/anylabeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       50 2023-04-12 02:01:37.000000 anylabeling-0.0.9/anylabeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1062 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/app.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.276973 anylabeling-0.0.9/anylabeling/configs/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.9/anylabeling/configs/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.277196 anylabeling-0.0.9/anylabeling/configs/__pycache__/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.0.9/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/configs/anylabeling_config.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)      315 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/configs/autolabel_segment_anything.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/configs/autolabel_yolov5m.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/configs/autolabel_yolov5s.yaml
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.277535 anylabeling-0.0.9/anylabeling/resources/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.9/anylabeling/resources/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)   477689 2023-04-12 01:37:51.000000 anylabeling-0.0.9/anylabeling/resources/resources.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.278200 anylabeling-0.0.9/anylabeling/services/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.9/anylabeling/services/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.279018 anylabeling-0.0.9/anylabeling/services/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3443 2023-04-12 01:31:17.000000 anylabeling-0.0.9/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5355 2023-04-12 01:27:25.000000 anylabeling-0.0.9/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9861 2023-04-12 01:26:18.000000 anylabeling-0.0.9/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1284 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5151 2023-04-12 01:26:25.000000 anylabeling-0.0.9/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/utils.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.279495 anylabeling-0.0.9/anylabeling/views/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.9/anylabeling/views/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.279892 anylabeling-0.0.9/anylabeling/views/common/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.9/anylabeling/views/common/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.0.9/anylabeling/views/common/tableview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.0.9/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.281082 anylabeling-0.0.9/anylabeling/views/labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:53:51.000000 anylabeling-0.0.9/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5569 2023-04-12 01:56:58.000000 anylabeling-0.0.9/anylabeling/views/labeling/__main__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2763 2023-04-12 02:01:24.000000 anylabeling-0.0.9/anylabeling/views/labeling/config.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.292056 anylabeling-0.0.9/anylabeling/views/labeling/icons/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6148 2023-04-09 05:07:05.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/.DS_Store
--rw-r--r--   0 vietanhdev   (501) staff       (20)        8 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/app.icns
--rw-r--r--   0 vietanhdev   (501) staff       (20)    31379 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/app.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1645 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/app.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    28068 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6844 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/cancel.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    11383 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/cartesian.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15818 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/circle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/color-line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    23824 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/color.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/color_line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10021 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/copy.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7842 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/delete.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/done.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22232 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/done.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15023 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/edit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7718 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/expert.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      278 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/expert1.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      335 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/expert2.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    37652 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/eye.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8059 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/feBlend-icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/file.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    17368 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/fit-width.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2186 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/fit-window.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2262 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/fit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4156 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/format_createml.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      786 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/format_voc.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      675 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/format_yolo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14479 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/help.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)  1128131 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/icon.icns
--rw-r--r--   0 vietanhdev   (501) staff       (20)   183198 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/icon.ico
--rw-r--r--   0 vietanhdev   (501) staff       (20)    44771 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2381 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/labels.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    36694 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/labels.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7253 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/line-strip.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9457 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      977 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/new.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7482 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/next.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26255 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/objects.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/open.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10572 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/paste.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    13847 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/point.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14286 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/polygon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7275 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/prev.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22460 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/quit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2136 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/rectangle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3637 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/resetall.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2811 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/save-as.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6118 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/save.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2004 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/undo-cross.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2018 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/undo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    18083 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/upload_brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3041 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/verify.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1099 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/zoom-in.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1074 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/zoom-out.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1139 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/icons/zoom.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5909 2023-04-12 01:56:33.000000 anylabeling-0.0.9/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    88726 2023-04-12 01:55:33.000000 anylabeling-0.0.9/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      610 2023-04-12 01:47:51.000000 anylabeling-0.0.9/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1786 2023-04-12 01:57:00.000000 anylabeling-0.0.9/anylabeling/views/labeling/logger.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/shape.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.292816 anylabeling-0.0.9/anylabeling/views/labeling/utils/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.294208 anylabeling-0.0.9/anylabeling/views/labeling/widgets/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.294595 anylabeling-0.0.9/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6906 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    46264 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8023 2023-04-08 19:49:25.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5778 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1394 2023-04-12 01:47:30.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      768 2023-04-08 20:09:45.000000 anylabeling-0.0.9/anylabeling/views/maintabs.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      981 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/mainwindow.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1458 2023-04-11 17:52:02.000000 anylabeling-0.0.9/anylabeling/views/mainwindow_tabs.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 02:01:50.276370 anylabeling-0.0.9/anylabeling.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 02:01:50.000000 anylabeling-0.0.9/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5098 2023-04-12 02:01:50.000000 anylabeling-0.0.9/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-12 02:01:50.000000 anylabeling-0.0.9/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-12 02:01:50.000000 anylabeling-0.0.9/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      235 2023-04-12 02:01:50.000000 anylabeling-0.0.9/anylabeling.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-12 02:01:50.000000 anylabeling-0.0.9/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.0.9/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-12 02:01:50.295027 anylabeling-0.0.9/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2454 2023-04-12 01:44:44.000000 anylabeling-0.0.9/setup.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.354022 anylabeling-0.1.0/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.1.0/LICENSE
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      112 2023-04-12 01:46:44.000000 anylabeling-0.1.0/MANIFEST.in
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 14:08:58.353872 anylabeling-0.1.0/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.1.0/README.md
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.338033 anylabeling-0.1.0/anylabeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       24 2023-04-12 13:22:41.000000 anylabeling-0.1.0/anylabeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1062 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/app.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      114 2023-04-12 13:33:27.000000 anylabeling-0.1.0/anylabeling/app_info.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.339525 anylabeling-0.1.0/anylabeling/configs/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/configs/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.339651 anylabeling-0.1.0/anylabeling/configs/__pycache__/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.1.0/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/configs/anylabeling_config.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      315 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/configs/autolabel_segment_anything.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/configs/autolabel_yolov5m.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/configs/autolabel_yolov5s.yaml
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.339869 anylabeling-0.1.0/anylabeling/resources/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/resources/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   477689 2023-04-12 01:37:51.000000 anylabeling-0.1.0/anylabeling/resources/resources.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.340275 anylabeling-0.1.0/anylabeling/services/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/services/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.341000 anylabeling-0.1.0/anylabeling/services/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3520 2023-04-12 13:27:43.000000 anylabeling-0.1.0/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5371 2023-04-12 13:27:43.000000 anylabeling-0.1.0/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9862 2023-04-12 13:51:14.000000 anylabeling-0.1.0/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1284 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5152 2023-04-12 13:27:43.000000 anylabeling-0.1.0/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/utils.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.341223 anylabeling-0.1.0/anylabeling/views/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/views/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.341563 anylabeling-0.1.0/anylabeling/views/common/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/views/common/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/views/common/tableview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.1.0/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.342720 anylabeling-0.1.0/anylabeling/views/labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:53:51.000000 anylabeling-0.1.0/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5590 2023-04-12 13:22:41.000000 anylabeling-0.1.0/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2763 2023-04-12 02:01:24.000000 anylabeling-0.1.0/anylabeling/views/labeling/config.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.351073 anylabeling-0.1.0/anylabeling/views/labeling/icons/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6148 2023-04-09 05:07:05.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/.DS_Store
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        8 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/app.icns
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    31379 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/app.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1645 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/app.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    28068 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/brain.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6844 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/cancel.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    11383 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/cartesian.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    15818 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/circle.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/color-line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    23824 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/color.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/color_line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10021 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/copy.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7842 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/delete.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/done.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    22232 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/done.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    15023 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/edit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7718 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/expert.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      278 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/expert1.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      335 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/expert2.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    37652 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/eye.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8059 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/feBlend-icon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/file.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    17368 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/fit-width.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2186 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/fit-window.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2262 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/fit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4156 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/format_createml.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      786 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/format_voc.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      675 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/format_yolo.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    14479 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/help.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)  1128131 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/icon.icns
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   183198 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/icon.ico
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    44771 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/icon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2381 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/labels.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    36694 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/labels.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7253 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/line-strip.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9457 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      977 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/new.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7482 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/next.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26255 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/objects.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/open.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10572 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/paste.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    13847 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/point.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    14286 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/polygon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7275 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/prev.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    22460 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/quit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2136 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/rectangle.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3637 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/resetall.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2811 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/save-as.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6118 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/save.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2004 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/undo-cross.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2018 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/undo.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    18083 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/upload_brain.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3041 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/verify.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1099 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/zoom-in.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1074 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/zoom-out.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1139 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/icons/zoom.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5945 2023-04-12 13:18:06.000000 anylabeling-0.1.0/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    89228 2023-04-12 14:03:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      610 2023-04-12 01:47:51.000000 anylabeling-0.1.0/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1786 2023-04-12 01:57:00.000000 anylabeling-0.1.0/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.351844 anylabeling-0.1.0/anylabeling/views/labeling/utils/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      510 2023-04-12 13:55:17.000000 anylabeling-0.1.0/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-12 13:27:43.000000 anylabeling-0.1.0/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.353275 anylabeling-0.1.0/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-12 13:27:43.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.353655 anylabeling-0.1.0/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6889 2023-04-12 13:27:43.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    46815 2023-04-12 13:54:32.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8023 2023-04-08 19:49:25.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5778 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1394 2023-04-12 01:47:30.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.1.0/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      915 2023-04-12 13:44:49.000000 anylabeling-0.1.0/anylabeling/views/mainwindow.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-12 14:08:58.338913 anylabeling-0.1.0/anylabeling.egg-info/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-12 14:08:58.000000 anylabeling-0.1.0/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5055 2023-04-12 14:08:58.000000 anylabeling-0.1.0/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-12 14:08:58.000000 anylabeling-0.1.0/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-12 14:08:58.000000 anylabeling-0.1.0/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      235 2023-04-12 14:08:58.000000 anylabeling-0.1.0/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-12 14:08:58.000000 anylabeling-0.1.0/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.1.0/pyproject.toml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-12 14:08:58.354066 anylabeling-0.1.0/setup.cfg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2454 2023-04-12 13:17:03.000000 anylabeling-0.1.0/setup.py
```

### Comparing `anylabeling-0.0.9/LICENSE` & `anylabeling-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/PKG-INFO` & `anylabeling-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.0.9
+Version: 0.1.0
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
-Metadata-Version: 2.1 Name: anylabeling Version: 0.0.9 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.1.0 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.0.9/README.md` & `anylabeling-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/app.py` & `anylabeling-0.1.0/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.1.0/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/configs/autolabel_yolov5m.yaml` & `anylabeling-0.1.0/anylabeling/configs/autolabel_yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/configs/autolabel_yolov5s.yaml` & `anylabeling-0.1.0/anylabeling/configs/autolabel_yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/resources/resources.py` & `anylabeling-0.1.0/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.1.0/anylabeling/services/auto_labeling/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from abc import abstractmethod
 import logging
 import os
 import pathlib
 import urllib.request
+from abc import abstractmethod
+
 import yaml
 
 from .types import AutoLabelingResult
 
 
 class Model:
     BASE_DOWNLOAD_URL = (
@@ -48,20 +49,22 @@
         model_abs_path = os.path.abspath(model_path)
         if os.path.exists(model_abs_path):
             return model_abs_path
 
         # Try download model from url
         if model_path.startswith("anylabeling_assets/"):
             self.on_message(
-                "Downloading model from model registry. This may take a while..."
+                "Downloading model from model registry. This may take a"
+                " while..."
             )
             relative_path = model_path.replace("anylabeling_assets/", "")
             download_url = self.BASE_DOWNLOAD_URL + relative_path
-            model_abs_path = os.path.join(
-                os.path.abspath("data"), relative_path
+            home_dir = os.path.expanduser("~")
+            model_abs_path = os.path.abspath(
+                os.path.join(home_dir, "data", relative_path)
             )
             if os.path.exists(model_abs_path):
                 return model_abs_path
             pathlib.Path(os.path.dirname(model_abs_path)).mkdir(
                 parents=True, exist_ok=True
             )
```

### Comparing `anylabeling-0.0.9/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.1.0/anylabeling/services/auto_labeling/model_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import copy
-import yaml
+import importlib.resources as pkg_resources
 from threading import Lock
-from PyQt5.QtCore import QObject, pyqtSignal
+
+import yaml
 from PyQt5.QtCore import QObject, QThread, pyqtSignal, pyqtSlot
-from anylabeling.utils import GenericWorker
-import importlib.resources as pkg_resources
 
 from anylabeling import configs as anylabeling_configs
 from anylabeling.services.auto_labeling.types import AutoLabelingResult
+from anylabeling.utils import GenericWorker
 
 
 class ModelManager(QObject):
     """Model manager"""
 
     new_model_status = pyqtSignal(str)
     model_loaded = pyqtSignal(list)
@@ -104,20 +104,24 @@
             self.auto_segmentation_model_unselected.emit()
 
         model_info = copy.deepcopy(self.model_infos[model_name])
 
         if model_info["type"] == "yolov5":
             from .yolov5 import YOLOv5
 
-            model_info["model"] = YOLOv5(model_info, on_message=self.new_model_status.emit)
+            model_info["model"] = YOLOv5(
+                model_info, on_message=self.new_model_status.emit
+            )
             self.auto_segmentation_model_unselected.emit()
         elif model_info["type"] == "segment_anything":
             from .segment_anything import SegmentAnything
 
-            model_info["model"] = SegmentAnything(model_info, on_message=self.new_model_status.emit)
+            model_info["model"] = SegmentAnything(
+                model_info, on_message=self.new_model_status.emit
+            )
             self.auto_segmentation_model_selected.emit()
         else:
             raise Exception(f"Unknown model type: {model_info['type']}")
 
         self.loaded_model_info = model_info
         return self.loaded_model_info
```

### Comparing `anylabeling-0.0.9/anylabeling/services/auto_labeling/segment_anything.py` & `anylabeling-0.1.0/anylabeling/services/auto_labeling/segment_anything.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 import os
 from copy import deepcopy
 
-import onnxruntime
 import cv2
 import numpy as np
+import onnxruntime
 from PyQt5 import QtCore
 
 from anylabeling.views.labeling.shape import Shape
 from anylabeling.views.labeling.utils.opencv import qt_img_to_cv_img
+
 from .model import Model
 from .types import AutoLabelingResult
 
 
 class SegmentAnything(Model):
     """Segmentation model using SegmentAnything"""
```

### Comparing `anylabeling-0.0.9/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.1.0/anylabeling/services/auto_labeling/types.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.1.0/anylabeling/services/auto_labeling/yolov5.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import cv2
 import numpy as np
 from PyQt5 import QtCore
 
 from anylabeling.views.labeling.shape import Shape
 from anylabeling.views.labeling.utils.opencv import qt_img_to_cv_img
+
 from .model import Model
 from .types import AutoLabelingResult
 
 
 class YOLOv5(Model):
     """Object detection model using YOLOv5"""
```

### Comparing `anylabeling-0.0.9/anylabeling/views/common/tableview.py` & `anylabeling-0.1.0/anylabeling/views/common/tableview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/common/toaster.py` & `anylabeling-0.1.0/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/__main__.py` & `anylabeling-0.1.0/anylabeling/views/labeling/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-__appname__ = "AnyLabeling"
-
 import argparse
 import codecs
 import logging
 import os
 import os.path as osp
 import sys
 
 import yaml
 from PyQt5 import QtCore, QtWidgets
 
+from ...app_info import __appname__
 from .config import get_config
 from .label_widget import MainWindow
 from .logger import logger
 from .utils import new_icon
 
 
 def main():
@@ -33,15 +32,17 @@
         "-O",
         "-o",
         help=(
             "output file or directory (if it ends with .json it is "
             "recognized as file, else as directory)"
         ),
     )
-    default_config_file = os.path.join(os.path.expanduser("~"), ".anylabelingrc")
+    default_config_file = os.path.join(
+        os.path.expanduser("~"), ".anylabelingrc"
+    )
     parser.add_argument(
         "--config",
         dest="config",
         help=(
             "config file or yaml-format string (default:"
             f" {default_config_file})"
         ),
```

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/config.py` & `anylabeling-0.1.0/anylabeling/views/labeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/.DS_Store` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/app.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/app.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/app.svg` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/app.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/brain.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/cancel.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/cartesian.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/cartesian.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/circle.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/circle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/color-line.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/color.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/color.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/color_line.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/color_line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/copy.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/copy.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/delete.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/delete.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/done.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/done.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/done.svg` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/done.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/edit.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/edit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/expert.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/expert.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/eye.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/eye.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/feBlend-icon.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/file.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/file.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/fit-width.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/fit-window.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/fit.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/fit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/format_createml.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/format_createml.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/format_voc.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/format_voc.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/format_yolo.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/format_yolo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/help.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/help.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/icon.icns` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/icon.ico` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/icon.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/labels.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/labels.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/labels.svg` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/line-strip.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/line-strip.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/line.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/new.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/new.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/next.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/next.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/objects.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/objects.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/open.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/open.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/paste.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/paste.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/point.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/point.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/polygon.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/prev.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/prev.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/quit.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/quit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/rectangle.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/resetall.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/resetall.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/save-as.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/save.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/save.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/undo-cross.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/undo.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/undo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/upload_brain.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/upload_brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/verify.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/verify.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/zoom-in.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/zoom-out.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/icons/zoom.png` & `anylabeling-0.1.0/anylabeling/views/labeling/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/label_file.py` & `anylabeling-0.1.0/anylabeling/views/labeling/label_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import contextlib
 import io
 import json
 import os.path as osp
 
 import PIL.Image
 
+from ...app_info import __version__
 from . import utils
 from .logger import logger
 
 PIL.Image.MAX_IMAGE_PIXELS = None
 
 
 @contextlib.contextmanager
```

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.1.0/anylabeling/views/labeling/label_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,34 @@
-__appname__ = "AnyLabeling"
-
 import functools
 import html
 import math
 import os
 import os.path as osp
 import re
 import webbrowser
 
 import imgviz
 import natsort
 from PyQt5 import QtCore, QtGui, QtWidgets
 from PyQt5.QtCore import Qt, pyqtSlot
-from PyQt5.QtWidgets import (
-    QDockWidget,
-    QHBoxLayout,
-    QLabel,
-    QPlainTextEdit,
-    QVBoxLayout,
-    QWhatsThis,
-)
+from PyQt5.QtWidgets import (QDockWidget, QHBoxLayout, QLabel, QPlainTextEdit,
+                             QVBoxLayout, QWhatsThis)
+
+from anylabeling.services.auto_labeling.types import AutoLabelingMode
 
+from ...app_info import __appname__
 from . import utils
 from .config import get_config
 from .label_file import LabelFile, LabelFileError
 from .logger import logger
 from .shape import Shape
-from .widgets import (
-    BrightnessContrastDialog,
-    Canvas,
-    FileDialogPreview,
-    LabelDialog,
-    LabelListWidget,
-    LabelListWidgetItem,
-    ToolBar,
-    UniqueLabelQListWidget,
-    ZoomWidget,
-    AutoLabelingWidget,
-)
-
-from anylabeling.services.auto_labeling.types import AutoLabelingMode
+from .widgets import (AutoLabelingWidget, BrightnessContrastDialog, Canvas,
+                      FileDialogPreview, LabelDialog, LabelListWidget,
+                      LabelListWidgetItem, ToolBar, UniqueLabelQListWidget,
+                      ZoomWidget)
 
 LABEL_COLORMAP = imgviz.label_colormap()
 
 # Green for the first label
 LABEL_COLORMAP[2] = LABEL_COLORMAP[1]
 LABEL_COLORMAP[1] = [0, 180, 33]
 
@@ -1492,15 +1477,26 @@
                     group_id=s.group_id,
                     shape_type=s.shape_type,
                     flags=s.flags,
                 )
             )
             return data
 
-        shapes = [format_shape(item.shape()) for item in self.label_list]
+        # Get current shapes
+        # Excluding auto labeling special shapes
+        shapes = [
+            format_shape(item.shape())
+            for item in self.label_list
+            if item.shape().label
+            not in [
+                AutoLabelingMode.OBJECT,
+                AutoLabelingMode.ADD,
+                AutoLabelingMode.REMOVE,
+            ]
+        ]
         flags = {}
         for i in range(self.flag_widget.count()):
             item = self.flag_widget.item(i)
             key = item.text()
             flag = item.checkState() == Qt.Checked
             flags[key] = flag
         try:
@@ -1724,14 +1720,16 @@
     def toggle_polygons(self, value):
         for item in self.label_list:
             item.setCheckState(Qt.Checked if value else Qt.Unchecked)
 
     def load_file(self, filename=None):
         """Load the specified file, or the last opened file if None."""
 
+        self.clear_auto_labeling_marks()
+
         # Changing file_list_widget loads file
         if filename in self.image_list and (
             self.file_list_widget.currentRow()
             != self.image_list.index(filename)
         ):
             self.file_list_widget.setCurrentRow(
                 self.image_list.index(filename)
@@ -2360,33 +2358,62 @@
             return
         # Clear existing shapes
         if auto_labeling_result.replace:
             self.load_shapes([], replace=True)
             self.label_list.clear()
             self.load_shapes(auto_labeling_result.shapes, replace=True)
         else:  # Just update existing shapes
-            # Remove shapes with label "AUTOLABEL_OBJECT"
+            # Remove shapes with label AutoLabelingMode.OBJECT
             for shape in self.canvas.shapes:
-                if shape.label == "AUTOLABEL_OBJECT":
+                if shape.label == AutoLabelingMode.OBJECT:
                     item = self.label_list.find_item_by_shape(shape)
                     self.label_list.remove_item(item)
             self.load_shapes(auto_labeling_result.shapes, replace=False)
 
         self.set_dirty()
 
     def clear_auto_labeling_marks(self):
-        """Clear auto labeling marks."""
+        """Clear auto labeling marks from the current image."""
+        # Clean up label list
         for shape in self.canvas.shapes:
             if shape.label in [
                 AutoLabelingMode.OBJECT,
                 AutoLabelingMode.ADD,
                 AutoLabelingMode.REMOVE,
             ]:
-                item = self.label_list.find_item_by_shape(shape)
-                self.label_list.remove_item(item)
+                try:
+                    item = self.label_list.find_item_by_shape(shape)
+                    self.label_list.remove_item(item)
+                except ValueError:
+                    pass
+
+        # Clean up unique label list
+        for shape_label in [
+            AutoLabelingMode.OBJECT,
+            AutoLabelingMode.ADD,
+            AutoLabelingMode.REMOVE,
+        ]:
+            for item in self.unique_label_list.find_items_by_label(
+                shape_label
+            ):
+                self.unique_label_list.takeItem(
+                    self.unique_label_list.row(item)
+                )
+
+        # Remove shapes from the canvas
+        self.canvas.shapes = [
+            shape
+            for shape in self.canvas.shapes
+            if shape.label
+            not in [
+                AutoLabelingMode.OBJECT,
+                AutoLabelingMode.ADD,
+                AutoLabelingMode.REMOVE,
+            ]
+        ]
         self.canvas.update()
 
     def finish_auto_labeling_object(self):
         """Finish auto labeling object."""
         has_object = False
         for shape in self.canvas.shapes:
             if shape.label == AutoLabelingMode.OBJECT:
@@ -2420,16 +2447,18 @@
             if shape.label == AutoLabelingMode.OBJECT:
                 updated_shapes = True
                 shape.label = text
                 shape.flags = flags
                 shape.group_id = group_id
                 # Update unique label list
                 if not self.unique_label_list.find_items_by_label(shape.label):
-                    unique_label_item = self.unique_label_list.create_item_from_label(
-                        shape.label
+                    unique_label_item = (
+                        self.unique_label_list.create_item_from_label(
+                            shape.label
+                        )
                     )
                     self.unique_label_list.addItem(unique_label_item)
                     rgb = self._get_rgb_by_label(shape.label)
                     self.unique_label_list.set_item_label(
                         unique_label_item, shape.label, rgb
                     )
 
@@ -2441,33 +2470,16 @@
                         '{} <font color="#{:02x}{:02x}{:02x}">●</font>'.format(
                             html.escape(shape.label), *color
                         )
                     )
                 else:
                     item.setText(f"{shape.label} ({shape.group_id})")
 
-        # Remove all ADD and REMOVE marks
-        for shape in self.canvas.shapes:
-            if shape.label in [AutoLabelingMode.ADD, AutoLabelingMode.REMOVE]:
-                item = self.label_list.find_item_by_shape(shape)
-                self.label_list.remove_item(item)
-
-        # Remove all auto labeling marks from unique label list
-        for item in self.unique_label_list.find_items_by_label(
-            AutoLabelingMode.OBJECT
-        ):
-            self.unique_label_list.takeItem(self.unique_label_list.row(item))
-        for item in self.unique_label_list.find_items_by_label(
-            AutoLabelingMode.ADD
-        ):
-            self.unique_label_list.takeItem(self.unique_label_list.row(item))
-        for item in self.unique_label_list.find_items_by_label(
-            AutoLabelingMode.REMOVE
-        ):
-            self.unique_label_list.takeItem(self.unique_label_list.row(item))
+        # Clean up auto labeling objects
+        self.clear_auto_labeling_marks()
 
         # Update shape colors
         for shape in self.canvas.shapes:
             self._update_shape_color(shape)
 
         if updated_shapes:
             self.set_dirty()
```

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.1.0/anylabeling/views/labeling/label_wrapper.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/logger.py` & `anylabeling-0.1.0/anylabeling/views/labeling/logger.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/shape.py` & `anylabeling-0.1.0/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/testing.py` & `anylabeling-0.1.0/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.1.0/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.1.0/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.1.0/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.1.0/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.1.0/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 
-from PyQt5 import uic
-from PyQt5.QtWidgets import QWidget
+from PyQt5 import QtGui, uic
 from PyQt5.QtCore import pyqtSignal, pyqtSlot
-from PyQt5 import QtGui
+from PyQt5.QtWidgets import QWidget
 
 from anylabeling.services.auto_labeling.model_manager import ModelManager
 from anylabeling.services.auto_labeling.types import AutoLabelingMode
 
 
 class AutoLabelingWidget(QWidget):
     new_model_selected = pyqtSignal(str)
```

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.1.0/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.1.0/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.1.0/anylabeling/views/labeling/widgets/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """This module defines Canvas widget - the core component for drawing image labels"""
 import imgviz
 from PyQt5 import QtCore, QtGui, QtWidgets
 from PyQt5.QtCore import Qt
 from PyQt5.QtGui import QWheelEvent
 
+from anylabeling.services.auto_labeling.types import AutoLabelingMode
+
 from .. import utils
 from ..shape import Shape
 
-from anylabeling.services.auto_labeling.types import AutoLabelingMode
-
 CURSOR_DEFAULT = QtCore.Qt.ArrowCursor
 CURSOR_POINT = QtCore.Qt.PointingHandCursor
 CURSOR_DRAW = QtCore.Qt.CrossCursor
 CURSOR_MOVE = QtCore.Qt.ClosedHandCursor
 CURSOR_GRAB = QtCore.Qt.OpenHandCursor
 
 MOVE_SPEED = 5.0
@@ -865,14 +865,24 @@
 
     def finalise(self):
         """Finish drawing for a shape"""
         assert self.current
         if self.is_auto_labeling:
             self.current.label = self.auto_labeling_mode.edit_mode
         self.current.close()
+        # Sort tl -> br for rectangle
+        if self.current.shape_type == "rectangle":
+            x_min = min(self.current.points[0].x(), self.current.points[1].x())
+            y_min = min(self.current.points[0].y(), self.current.points[1].y())
+            x_max = max(self.current.points[0].x(), self.current.points[1].x())
+            y_max = max(self.current.points[0].y(), self.current.points[1].y())
+            self.current.points = [
+                QtCore.QPointF(x_min, y_min),
+                QtCore.QPointF(x_max, y_max),
+            ]
         self.shapes.append(self.current)
         self.store_shapes()
         self.current = None
         self.set_hiding(False)
         self.new_shape.emit()
         self.update()
         if self.is_auto_labeling:
```

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.1.0/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.1.0/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.1.0/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.1.0/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.1.0/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.1.0/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.1.0/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.9/anylabeling/views/mainwindow.py` & `anylabeling-0.1.0/anylabeling/views/mainwindow.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 """This module defines the main application window"""
 
-from PyQt5.QtGui import QFont
-from PyQt5.QtWidgets import (
-    QHBoxLayout,
-    QLabel,
-    QMainWindow,
-    QStatusBar,
-    QVBoxLayout,
-    QWidget,
-)
+from PyQt5.QtWidgets import QMainWindow, QStatusBar, QVBoxLayout, QWidget
 
+from ..app_info import __appdescription__, __appname__
 from .labeling.label_wrapper import LabelingWrapper
 
 
 class MainWindow(QMainWindow):
     """Main application window"""
 
     def __init__(self, app):
         super().__init__()
         self.app = app
 
         self.setContentsMargins(0, 0, 0, 0)
-        self.setWindowTitle("AnyLabeling")
+        self.setWindowTitle(__appname__)
 
         main_layout = QVBoxLayout()
         main_layout.setContentsMargins(10, 10, 10, 10)
         self.labeling_widget = LabelingWrapper(self)
         main_layout.addWidget(self.labeling_widget)
         widget = QWidget()
         widget.setLayout(main_layout)
         self.setCentralWidget(widget)
 
         status_bar = QStatusBar()
-        status_bar.showMessage(
-            "AnyLabeling - Effortless data labeling with AI support"
-        )
+        status_bar.showMessage(f"{__appname__} - {__appdescription__}")
         self.setStatusBar(status_bar)
```

### Comparing `anylabeling-0.0.9/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.1.0/anylabeling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.0.9
+Version: 0.1.0
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
-Metadata-Version: 2.1 Name: anylabeling Version: 0.0.9 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.1.0 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.0.9/anylabeling.egg-info/SOURCES.txt` & `anylabeling-0.1.0/anylabeling.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 anylabeling/__init__.py
 anylabeling/app.py
+anylabeling/app_info.py
 anylabeling/utils.py
 anylabeling.egg-info/PKG-INFO
 anylabeling.egg-info/SOURCES.txt
 anylabeling.egg-info/dependency_links.txt
 anylabeling.egg-info/entry_points.txt
 anylabeling.egg-info/requires.txt
 anylabeling.egg-info/top_level.txt
@@ -24,17 +25,15 @@
 anylabeling/services/auto_labeling/__init__.py
 anylabeling/services/auto_labeling/model.py
 anylabeling/services/auto_labeling/model_manager.py
 anylabeling/services/auto_labeling/segment_anything.py
 anylabeling/services/auto_labeling/types.py
 anylabeling/services/auto_labeling/yolov5.py
 anylabeling/views/__init__.py
-anylabeling/views/maintabs.py
 anylabeling/views/mainwindow.py
-anylabeling/views/mainwindow_tabs.py
 anylabeling/views/common/__init__.py
 anylabeling/views/common/tableview.py
 anylabeling/views/common/toaster.py
 anylabeling/views/labeling/__init__.py
 anylabeling/views/labeling/__main__.py
 anylabeling/views/labeling/config.py
 anylabeling/views/labeling/label_file.py
```

### Comparing `anylabeling-0.0.9/setup.py` & `anylabeling-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import re
 
 from setuptools import find_packages, setup
 
 
 def get_version():
-    """Get package version from __init__.py file"""
-    filename = "anylabeling/__init__.py"
+    """Get package version from app_info.py file"""
+    filename = "anylabeling/app_info.py"
     with open(filename, encoding="utf-8") as f:
         match = re.search(
             r"""^__version__ = ['"]([^'"]*)['"]""", f.read(), re.M
         )
     if not match:
         raise RuntimeError(f"{filename} doesn't contain __version__")
     version = match.groups()[0]
```

