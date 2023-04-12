# Comparing `tmp/pcleaner-1.3.0.tar.gz` & `tmp/pcleaner-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-1.3.0.tar", last modified: Sat Apr  8 15:28:53 2023, max compression
+gzip compressed data, was "pcleaner-1.4.0.tar", last modified: Wed Apr 12 04:07:00 2023, max compression
```

## Comparing `pcleaner-1.3.0.tar` & `pcleaner-1.4.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-08 15:28:53.206610 pcleaner-1.3.0/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-03-13 00:41:01.000000 pcleaner-1.3.0/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11477 2023-04-08 15:28:53.206610 pcleaner-1.3.0/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10852 2023-03-25 19:50:27.000000 pcleaner-1.3.0/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-08 15:28:53.196610 pcleaner-1.3.0/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       47 2023-04-08 15:28:15.000000 pcleaner-1.3.0/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    17213 2023-04-08 15:25:59.000000 pcleaner-1.3.0/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7402 2023-04-08 15:01:09.000000 pcleaner-1.3.0/pcleaner/cleaner.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5672 2023-03-25 19:50:27.000000 pcleaner-1.3.0/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-08 15:28:53.199944 pcleaner-1.3.0/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-08 15:28:53.199944 pcleaner-1.3.0/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-08 15:28:53.199944 pcleaner-1.3.0/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-08 15:28:53.206610 pcleaner-1.3.0/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1869 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    31792 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4555 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/ctd_interface.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3843 2023-04-07 01:18:40.000000 pcleaner-1.3.0/pcleaner/denoiser.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20356 2023-04-07 01:05:12.000000 pcleaner-1.3.0/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    22247 2023-04-08 14:40:09.000000 pcleaner-1.3.0/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4717 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/model_downloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7564 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/pre_processor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    12895 2023-04-08 14:39:15.000000 pcleaner-1.3.0/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-08 15:28:53.199944 pcleaner-1.3.0/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11477 2023-04-08 15:28:53.000000 pcleaner-1.3.0/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1392 2023-04-08 15:28:53.000000 pcleaner-1.3.0/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-08 15:28:53.000000 pcleaner-1.3.0/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-08 15:28:53.000000 pcleaner-1.3.0/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      171 2023-04-08 15:28:53.000000 pcleaner-1.3.0/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-08 15:28:53.000000 pcleaner-1.3.0/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-03-13 00:41:01.000000 pcleaner-1.3.0/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1039 2023-04-08 15:28:53.206610 pcleaner-1.3.0/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-03-13 00:41:01.000000 pcleaner-1.3.0/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 04:07:00.675750 pcleaner-1.4.0/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.4.0/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-12 04:07:00.675750 pcleaner-1.4.0/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.4.0/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 04:07:00.672417 pcleaner-1.4.0/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       47 2023-04-12 04:06:51.000000 pcleaner-1.4.0/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    17222 2023-04-11 21:05:32.000000 pcleaner-1.4.0/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8532 2023-04-12 03:17:45.000000 pcleaner-1.4.0/pcleaner/cleaner.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5672 2023-01-23 03:12:00.000000 pcleaner-1.4.0/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 04:07:00.672417 pcleaner-1.4.0/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 04:07:00.672417 pcleaner-1.4.0/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 04:07:00.672417 pcleaner-1.4.0/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 04:07:00.675750 pcleaner-1.4.0/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2007 2023-04-11 20:28:36.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.4.0/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    33652 2023-04-12 03:17:56.000000 pcleaner-1.4.0/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5736 2023-04-12 03:29:15.000000 pcleaner-1.4.0/pcleaner/ctd_interface.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4714 2023-04-11 20:27:33.000000 pcleaner-1.4.0/pcleaner/denoiser.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    21190 2023-04-12 00:09:46.000000 pcleaner-1.4.0/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    22404 2023-04-12 03:17:45.000000 pcleaner-1.4.0/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4717 2023-01-08 14:40:11.000000 pcleaner-1.4.0/pcleaner/model_downloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7679 2023-04-12 03:17:45.000000 pcleaner-1.4.0/pcleaner/pre_processor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.4.0/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    12959 2023-04-11 02:23:20.000000 pcleaner-1.4.0/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 04:07:00.672417 pcleaner-1.4.0/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-12 04:07:00.000000 pcleaner-1.4.0/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1392 2023-04-12 04:07:00.000000 pcleaner-1.4.0/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-12 04:07:00.000000 pcleaner-1.4.0/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-12 04:07:00.000000 pcleaner-1.4.0/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      171 2023-04-12 04:07:00.000000 pcleaner-1.4.0/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-12 04:07:00.000000 pcleaner-1.4.0/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.4.0/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1039 2023-04-12 04:07:00.675750 pcleaner-1.4.0/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.4.0/setup.py
```

### Comparing `pcleaner-1.3.0/LICENSE` & `pcleaner-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/PKG-INFO` & `pcleaner-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.3.0
+Version: 1.4.0
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
@@ -64,21 +64,25 @@
 
 - Supports CUDA acceleration, if your hardware supports it.
 
 - Supports batch processing of images and directories.
 
 - Can handle bubbles on any solid grayscale background color.
 
+- Can also cut out the text from the rest of the image, e.g. to paste it over a colored rendition.
+
 - Can also run OCR on the pages and output the text to a file.
 
 
 ## Limitations
 
 - It only supports Japanese and English text.
 
+- Supported file types: .jpeg, .jpg, .png, .bmp, .tiff, .tif, .jp2, .dib, .webp, .ppm
+
 - The program relies on AI for the initial text detection, which by nature is imperfect. Sometimes it will miss little bits of text or think part of the bubble belongs to the text, which will prevent that bubble from being cleaned. From testing, this typically affects between 2–8% of bubbles, depending on your settings.
 
 - Due to the conservative approach taken in the selection of masks, if the program can't clean the bubble to a satisfying degree, it will skip that bubble outright. This does, however, also prevent false positives.
 
 - For masks, only grayscale is currently supported. This means it can cover up text in white, black, or gray bubbles, but not colored ones.
```

### Comparing `pcleaner-1.3.0/README.md` & `pcleaner-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,21 +49,25 @@
 
 - Supports CUDA acceleration, if your hardware supports it.
 
 - Supports batch processing of images and directories.
 
 - Can handle bubbles on any solid grayscale background color.
 
+- Can also cut out the text from the rest of the image, e.g. to paste it over a colored rendition.
+
 - Can also run OCR on the pages and output the text to a file.
 
 
 ## Limitations
 
 - It only supports Japanese and English text.
 
+- Supported file types: .jpeg, .jpg, .png, .bmp, .tiff, .tif, .jp2, .dib, .webp, .ppm
+
 - The program relies on AI for the initial text detection, which by nature is imperfect. Sometimes it will miss little bits of text or think part of the bubble belongs to the text, which will prevent that bubble from being cleaned. From testing, this typically affects between 2–8% of bubbles, depending on your settings.
 
 - Due to the conservative approach taken in the selection of masks, if the program can't clean the bubble to a satisfying degree, it will skip that bubble outright. This does, however, also prevent false positives.
 
 - For masks, only grayscale is currently supported. This means it can cover up text in white, black, or gray bubbles, but not colored ones.
```

### Comparing `pcleaner-1.3.0/pcleaner/analytics.py` & `pcleaner-1.4.0/pcleaner/analytics.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import pcleaner.structures as st
 
 
 # I'll admit this file is a mess.
 # These bar chart creators should be abstracted into a single implementation, not 3 different ones.
 
+
 def terminal_width() -> int:
     # Use a fallback of 50 for unsupported terminals.
     width = shutil.get_terminal_size((50, 50)).columns
     # Make sure the width is at least 20, to avoid weirdness.
     return max(width, 20)
 
 
@@ -207,15 +208,15 @@
     perfect_masks = sum(1 for analytics in analytics if analytics[1] and analytics[3] == 0)
     average_border_deviation = (
         f"{sum(analytics[3] for analytics in analytics if analytics[1]) / masks_succeeded:.2f}"
         if masks_succeeded
         else "N/A"
     )
     success_rate = f"{masks_succeeded / total_boxes:.0%}" if total_boxes else "N/A"
-    perfect_mask_rate = f"{perfect_masks / total_boxes:.0%}" if total_boxes else "N/A"
+    perfect_mask_rate = f"{perfect_masks / masks_succeeded:.0%}" if masks_succeeded else "N/A"
     masks_failed = total_boxes - masks_succeeded
 
     highest_mask_index = max(analytics[2] for analytics in analytics if analytics[1])
     # Count the number of times each mask index was used.
     mask_usages_by_index = [0] * (highest_mask_index + 1)
     # Count the number of times each mask was perfect.
     perfect_mask_usages_by_index = [0] * (highest_mask_index + 1)
```

### Comparing `pcleaner-1.3.0/pcleaner/cleaner.py` & `pcleaner-1.4.0/pcleaner/cleaner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 
 from PIL import Image
-from logzero import logger
+from logzero import logger, loglevel, DEBUG, INFO
 
 import pcleaner.image_ops as ops
 import pcleaner.structures as st
 
 
 def clean_page(c_data: st.CleanerData) -> list[tuple[Path, bool, int, float]]:
     """
@@ -22,15 +22,17 @@
     cleaner_conf = c_data.cleaner_config
 
     original_img_path_as_png = Path(page_data.original_path).with_suffix(
         ".png"
     )  # Make sure all derived file names are .png.
     # Clobber protection prefixes have the form "[A-Z]{4}-\d+_file name", ex. JMCF-0_0023.json
     clobber_protection_prefix = c_data.json_path.stem.split("_")[0]
-    cache_out_path = c_data.cache_dir / f"{clobber_protection_prefix}_{original_img_path_as_png.name}"
+    cache_out_path = (
+        c_data.cache_dir / f"{clobber_protection_prefix}_{original_img_path_as_png.name}"
+    )
     logger.debug(f"Masking {cache_out_path.name}...")
 
     def save_mask(img, name_suffix):
         if c_data.show_masks:
             img.save(cache_out_path.with_stem(cache_out_path.stem + name_suffix))
 
     # Load the base image.
@@ -56,14 +58,15 @@
         ops.pick_best_mask(
             base=base_image,
             precise_mask=cut_mask,
             box_mask=box_mask,
             masking_box=masking_box,
             reference_box=reference_box,
             cleaner_conf=cleaner_conf,
+            save_masks=c_data.show_masks,
             analytics_page_path=Path(original_img_path_as_png),
         )
         for masking_box, reference_box in zip(
             page_data.merged_extended_boxes, page_data.reference_boxes
         )
     ]
     # Take out all entries that are None, since these masks were false positives.
@@ -119,14 +122,33 @@
                 original_img_path_as_png.parent / c_data.output_dir / original_img_path_as_png.name
             )
 
         final_out_path.parent.mkdir(parents=True, exist_ok=True)
         final_cleaned_out_path = final_out_path.with_name(final_out_path.stem + "_clean.png")
         final_mask_out_path = final_out_path.with_name(final_out_path.stem + "_mask.png")
 
+        # Check what the preferred output format is.
+        if cleaner_conf.preferred_file_type is None:
+            # Use the original file type.
+            final_cleaned_out_path = final_cleaned_out_path.with_suffix(
+                Path(page_data.original_path).suffix
+            )
+        else:
+            final_cleaned_out_path = final_cleaned_out_path.with_suffix(
+                cleaner_conf.preferred_file_type
+            )
+
+        if cleaner_conf.preferred_mask_file_type is None:
+            # Use png by default.
+            final_mask_out_path = final_mask_out_path.with_suffix(".png")
+        else:
+            final_mask_out_path = final_mask_out_path.with_suffix(
+                cleaner_conf.preferred_mask_file_type
+            )
+
         logger.debug(f"Final output path: {final_cleaned_out_path}")
 
         # The arg parser should ensure that both can't be true at once, not like that'd be an issue, just plain silly.
         if not c_data.save_only_mask and not c_data.save_only_text:
             # Save the final image.
             logger.debug(f"Saving final image to {final_cleaned_out_path}")
             base_image.save(final_cleaned_out_path)
@@ -139,17 +161,21 @@
         if c_data.extract_text:
             # Extract the text layer from the image.
             logger.debug(f"Extracting text from {final_cleaned_out_path}")
             # Reload the image, since it was modified.
             base_image = Image.open(page_data.image_path)
             text_img = ops.extract_text(base_image, combined_mask)
             text_out_path = final_out_path.with_name(final_out_path.stem + "_text.png")
+            if cleaner_conf.preferred_mask_file_type is None:
+                # Use png by default.
+                text_out_path = text_out_path.with_suffix(".png")
+            else:
+                text_out_path = text_out_path.with_suffix(cleaner_conf.preferred_mask_file_type)
             text_img.save(text_out_path)
 
-
     return analytics
 
 
 def save_denoising_data(
     original_path: Path,
     target_path: Path,
     cleaned_path: Path,
@@ -174,9 +200,11 @@
     :param mask_fitments: The mask fitments.
     """
 
     # Gather the data needed for denoising.
     boxes_with_deviation = [m.noise_mask_data for m in mask_fitments]
 
     # Save the data.
-    mask_data = st.MaskData(original_path, target_path, cleaned_path, mask_path, boxes_with_deviation)
+    mask_data = st.MaskData(
+        original_path, target_path, cleaned_path, mask_path, boxes_with_deviation
+    )
     mask_data.write_json(cache_path.with_name(cache_path.stem + "_mask_data.json"))
```

### Comparing `pcleaner-1.3.0/pcleaner/cli_utils.py` & `pcleaner-1.4.0/pcleaner/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/inference.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import os.path as osp
 import glob
 from pathlib import Path
 import cv2
 import numpy as np
 import json
 
-IMG_EXT = [".bmp", ".jpg", ".png", ".jpeg"]
+# These need to be restored after patching to a new version of the comic text detector.
+IMG_EXT = [".jpeg", ".jpg", ".png", ".bmp", ".tiff", ".tif", ".jp2", ".dib", ".webp", ".ppm"]
 
 NP_BOOL_TYPES = (np.bool_, np.bool8)
 NP_FLOAT_TYPES = (np.float_, np.float16, np.float32, np.float64)
 NP_INT_TYPES = (
     np.int_,
     np.int8,
     np.int16,
```

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-1.4.0/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/config.py` & `pcleaner-1.4.0/pcleaner/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 RESERVED_PROFILE_NAMES = ["builtin", "none"]
 
 
 @dataclass
 class TextDetectorConfig:
     model_path: str | None = None
+    concurrent_models: int = 1
 
     def export_to_conf(self, config_updater: cu.ConfigUpdater) -> None:
         """
         Write the config to the config updater object.
 
         No add_after_section here since it is the first section.
 
@@ -29,28 +30,36 @@
         [TextDetector]
         
         # Path to the text detection model, leave empty to use the built-in model.
         # The model can be found here:
         # https://github.com/zyddnys/manga-image-translator/releases/latest
         model_path = {none_to_empty(self.model_path)}
         
+        # Number of models to run in parallel. This is useful if you have enough RAM
+        # (or VRAM with CUDA) to run multiple models at the same time.
+        # This, of course, will increase the speed of the process, but can also
+        # crash your computer if you overestimate your hardware.
+        # I recommend using 1 model per 2 GB of memory available.
+        concurrent_models = {self.concurrent_models}
+        
         """
         config_updater.read_string(multi_left_strip(config_str))
 
     def import_from_conf(self, config_updater: cu.ConfigUpdater) -> None:
         """
         Read the config from the config updater object.
 
         :param config_updater: An existing config updater object.
         """
         if not config_updater.has_section("TextDetector"):
             logger.info("No TextDetector section found in the profile, using defaults.")
             return
 
         try_to_load(self, config_updater, "TextDetector", str | None, "model_path")
+        try_to_load(self, config_updater, "TextDetector", int, "concurrent_models")
 
 
 @dataclass
 class PreProcessorConfig:
     box_min_size: int = 20 * 20
     suspicious_box_min_size: int = 200 * 200
     ocr_enabled: bool = True
@@ -144,32 +153,45 @@
         try_to_load(self, config_updater, section, int, "box_padding_extended")
         try_to_load(self, config_updater, section, int, "box_right_padding_extended")
         try_to_load(self, config_updater, section, int, "box_reference_padding")
 
 
 @dataclass
 class CleanerConfig:
+    preferred_file_type: str | None = None
+    preferred_mask_file_type: str | None = None
     mask_growth_step_pixels: int = 2
     mask_growth_steps: int = 11
     off_white_max_threshold: int = 240
     mask_improvement_threshold: float = 0.1
+    mask_selection_fast: bool = False
     mask_max_standard_deviation: float = 15
     debug_mask_color: tuple[int, int, int, int] = (108, 30, 240, 127)
 
     def export_to_conf(self, config_updater: cu.ConfigUpdater, add_after_section: str) -> None:
         """
         Write the config to the config updater object.
 
         :param config_updater: An existing config updater object.
         :param add_after_section: The section to add the new section after.
         """
         config_str = f"""\
         [Cleaner]
         
-        # Number of pixels to grow the mask by each step. 
+        
+        # Preferred file type to save the cleaned image as.
+        # If no file type is specified, the original file type will be used.
+        preferred_file_type = {self.preferred_file_type if self.preferred_file_type else ""}
+        
+        # Preferred file type to save the mask as.
+        # If no file type is specified, png will be used.
+        # This is because the mask image must use transparency, which is not supported by all image formats.
+        preferred_mask_file_type = {self.preferred_mask_file_type if self.preferred_mask_file_type else ""}
+        
+        # Number of pixels to grow the mask by each step.
         # This bulks up the outline of the mask, so smaller values will be more accurate but slower.
         mask_growth_step_pixels = {self.mask_growth_step_pixels}
         
         # Number of steps to grow the mask by.
         # A higher number will make more and larger masks, ultimately limited by the reference box size.
         mask_growth_steps = {self.mask_growth_steps}
         
@@ -183,14 +205,20 @@
         # The standard deviation refers to the variation is color along the edge of a mask.
         # A low variation means that the mask sits in a solid color,
         # which means it doesn't intersect any text or other objects.
         # Setting a higher value here requires a higher improvement to consider a smaller mask,
         # to give a preference to larger masks.
         mask_improvement_threshold = {self.mask_improvement_threshold}
         
+        
+        # Whether to use the fast mask selection algorithm.
+        # When true, the mask selection algorith with pick the first perfect mask, if one if found early.
+        # This is faster, but may not find the best mask, if a slightly bigger one would have been better.
+        mask_selection_fast = {self.mask_selection_fast}
+        
         # The maximum standard deviation of a mask to consider.
         # A high value here means a higher tolerance for the mask intersecting text or other objects,
         # which isn't a good mask, as it will require inpainting anyway.
         mask_max_standard_deviation = {self.mask_max_standard_deviation}
         
         # Color to use for the debug mask. This is a tuple of RGBA values.
         debug_mask_color = {','.join(map(str, self.debug_mask_color))}
@@ -208,18 +236,21 @@
         :param config_updater: An existing config updater object.
         """
         section = "Cleaner"
         if not config_updater.has_section(section):
             logger.info(f"No {section} section found in the profile, using defaults.")
             return
 
+        try_to_load(self, config_updater, section, str | None, "preferred_file_type")
+        try_to_load(self, config_updater, section, str | None, "preferred_mask_file_type")
         try_to_load(self, config_updater, section, int, "mask_growth_step_pixels")
         try_to_load(self, config_updater, section, int, "mask_growth_steps")
         try_to_load(self, config_updater, section, int, "off_white_max_threshold")
         try_to_load(self, config_updater, section, float, "mask_improvement_threshold")
+        try_to_load(self, config_updater, section, bool, "mask_selection_fast")
         try_to_load(self, config_updater, section, float, "mask_max_standard_deviation")
         try:
             color_tuple: tuple[int, ...] = tuple(
                 int(x) for x in config_updater["Cleaner"]["debug_mask_color"].value.split(",")
             )
             if len(color_tuple) != 4:
                 raise ValueError(
```

### Comparing `pcleaner-1.3.0/pcleaner/ctd_interface.py` & `pcleaner-1.4.0/pcleaner/ctd_interface.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,102 +11,149 @@
 
 The code present in the pcleaner/comic_text_detector folder is a
 slimmed-down version of the original project, containing only the
 necessary files to run the model and the function below.
 """
 
 import json
-import random
+import uuid
 import string
 from pathlib import Path
+import multiprocessing as mp
 
 from tqdm import tqdm
+import torch
 
+import pcleaner.config as cfg
 from .comic_text_detector.inference import TextDetector
 from .comic_text_detector.utils.io_utils import imread, imwrite, find_all_imgs, NumpyEncoder
 from .comic_text_detector.utils.textmask import REFINEMASK_ANNOTATION
 
 
-def model2annotations(model_path: Path, img_paths: str | Path | list[str | Path], save_dir: Path):
+def model2annotations(
+    config: cfg.TextDetectorConfig,
+    model_path: Path,
+    img_paths: str | Path | list[str | Path],
+    save_dir: Path,
+):
     """
     Run the model on a directory of images and produce the following
     for each image inside the save_dir directory:
     - A copy of the original image as a .png file.
     - A .png file containing the text mask, filename: <image_name>_mask.png.
     - A .json file containing each box of text, as well as other metadata,
       filename: <image_name>.json.
 
     For this modified version, include the image name and mask name in the
     json file.
 
+    :param config: Text detector configuration, part of the profile.
     :param model_path: Path to the model file. This ends either in .pt or .onnx (torch or cv2 format).
     :param img_paths: Path or a list of paths to an image or directory of images.
     :param save_dir: Path to the directory where the results will be saved.
     :return:
     """
+    # Scan for images, shallow search in given directories.
     if isinstance(img_paths, str | Path):
         img_paths = [img_paths]
-    device = "cuda" if model_path.suffix == ".pt" else "cpu"
-    print(f"Using device for text detection model: {device}")
-    model = TextDetector(model_path=str(model_path), input_size=1024, device=device)
+
     img_list = []
 
     for img_dir in img_paths:
         if Path(img_dir).is_dir():
             img_list.extend(find_all_imgs(img_dir, abs_path=True))
         elif Path(img_dir).is_file():
             img_list.append(img_dir)
         else:
             raise FileNotFoundError(f"Image path {img_dir} does not exist.")
 
     if not img_list:
         print("No images found.")
         return
 
-    # Make a batch prefix, which is a random string of uppercase letters.
-    # This is used to avoid overwriting files with the same name, even
-    # between different runs of the program.
-    batch_prefix = get_random_uppercase_string(4)
-    digits = len(str(len(img_list) - 1))
-
-    for index, img_path in enumerate(tqdm(img_list)):
-        img = imread(img_path)
-        img_path = Path(img_path).absolute()
-
-        # Prepend an index to prevent name clobbering between different files.
-        prefix = f"{batch_prefix}-{index:0{digits}}_"
-
-        img_name = prefix + img_path.stem
-        maskname = img_name + "_mask.png"
-
-        # Make names absolute paths.
-        img_name = str((save_dir / (img_name + ".png")).absolute())
-        maskname = str((save_dir / maskname).absolute())
-
-        mask, mask_refined, blk_list = model(
-            img, refine_mode=REFINEMASK_ANNOTATION, keep_undetected_mask=True
-        )
-        blk_xyxy = []
-        blk_dict_list = []
-        for blk in blk_list:
-            blk_xyxy.append(blk.xyxy)
-            blk_dict_list.append(blk.to_dict())
-
-        # Inject the img_name.png and mask name and original path into the json.
-        data = {
-            "image_path": img_name,
-            "mask_path": maskname,
-            "original_path": str(img_path),
-            "blk_list": blk_dict_list,
-        }
-
-        with open(Path(img_name).with_suffix(".json"), "w", encoding="utf8") as f:
-            json.dump(data, f, ensure_ascii=False, cls=NumpyEncoder, indent=4)
-        imwrite(img_name, img)
-        imwrite(maskname, mask_refined)
+    device = "cuda" if model_path.suffix == ".pt" else "cpu"
+    print(f"Using device for text detection model: {device}")
+    # Determine the number of processes to use
+    num_processes = min(config.concurrent_models, len(img_list))
+    print(f"Using {num_processes} processes for text detection.")
+
+    if num_processes > 1:
+
+        mp.freeze_support()
+        mp.set_start_method("spawn")
+
+        with mp.Pool(num_processes) as pool:
+
+            # Distribute the images evenly among the processes.
+            batches = [list() for _ in range(num_processes)]
+            for i, img_path in enumerate(img_list):
+                batches[i % num_processes].append(img_path)
+
+            args = [(batch, model_path, device, save_dir) for batch in batches]
+
+            for _ in tqdm(pool.imap_unordered(process_image_batch, args), total=len(args)):
+                pass  # do nothing, just iterate through the results
+
+    else:
+        model = TextDetector(model_path=str(model_path), input_size=1024, device=device)
+
+        for index, img_path in enumerate(tqdm(img_list)):
+            process_image(img_path, model, save_dir)
+
+
+def process_image_batch(args):
+    img_batch, model_path, device, save_dir = args
+    model = TextDetector(model_path=str(model_path), input_size=1024, device=device)
+    for img_path in img_batch:
+        process_image(img_path, model, save_dir)
+
+    del model
+
+    if device == "cuda":
+        # Release CUDA resources.
+        torch.cuda.ipc_collect()
+        torch.cuda.empty_cache()
+
+
+def process_image(img_path: str | Path, model: TextDetector, save_dir: Path):
+
+    img = imread(img_path)
+    img_path = Path(img_path).absolute()
+
+    # Prepend an index to prevent name clobbering between different files.
+    prefix = f"{uuid.uuid4()}_"
+
+    img_name = prefix + img_path.stem
+    maskname = img_name + "_mask.png"
+
+    # Make names absolute paths.
+    img_name = str((save_dir / (img_name + ".png")).absolute())
+    maskname = str((save_dir / maskname).absolute())
+
+    mask, mask_refined, blk_list = model(
+        img, refine_mode=REFINEMASK_ANNOTATION, keep_undetected_mask=True
+    )
+    blk_xyxy = []
+    blk_dict_list = []
+    for blk in blk_list:
+        blk_xyxy.append(blk.xyxy)
+        blk_dict_list.append(blk.to_dict())
+
+    # Inject the img_name.png and mask name and original path into the json.
+    data = {
+        "image_path": img_name,
+        "mask_path": maskname,
+        "original_path": str(img_path),
+        "blk_list": blk_dict_list,
+    }
+
+    with open(Path(img_name).with_suffix(".json"), "w", encoding="utf8") as f:
+        json.dump(data, f, ensure_ascii=False, cls=NumpyEncoder, indent=4)
+    imwrite(img_name, img)
+    imwrite(maskname, mask_refined)
 
 
 def get_random_uppercase_string(length: int = 4) -> str:
     """
     Return a random string of uppercase letters of the given length.
 
     :param length: The length of the string to return.
```

### Comparing `pcleaner-1.3.0/pcleaner/denoiser.py` & `pcleaner-1.4.0/pcleaner/denoiser.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     # Load all the cached data.
     mask_data = st.MaskData.from_json(d_data.json_path.read_text())
     cleaned_image = Image.open(mask_data.cleaned_path)
     mask_image = Image.open(mask_data.mask_path)
 
     # Alias.
     d_conf = d_data.denoiser_config
+    c_conf = d_data.cleaner_config
 
     # Filter for the min deviation to consider for denoising.
     boxes_to_denoise: list[tuple[int, int, int, int]] = [
         box
         for box, deviation in mask_data.boxes_with_deviation
         if deviation > d_conf.noise_min_standard_deviation
     ]
@@ -43,24 +44,37 @@
     # Settle on the final output path for the cleaned image.
     if d_data.output_dir.is_absolute():
         final_out_path = d_data.output_dir / mask_data.target_path.name
     else:
         # Take the original image path, and place the image in a subdirectory.
         # This is for when multiple directories were passed in.
         final_out_path = (
-                mask_data.target_path.parent / d_data.output_dir / mask_data.target_path.name
+            mask_data.target_path.parent / d_data.output_dir / mask_data.target_path.name
         )
 
     final_out_path.parent.mkdir(parents=True, exist_ok=True)
     final_cleaned_out_path = final_out_path.with_name(final_out_path.stem + "_clean.png")
     final_mask_out_path = final_out_path.with_name(final_out_path.stem + "_mask.png")
     final_mask_denoised_out_path = final_out_path.with_name(
         final_out_path.stem + "_denoised_mask.png"
     )
 
+    # Check what the preferred output format is.
+    if c_conf.preferred_file_type is None:
+        # Use the original file type.
+        final_cleaned_out_path = final_cleaned_out_path.with_suffix(mask_data.original_path.suffix)
+    else:
+        final_cleaned_out_path = final_cleaned_out_path.with_suffix(c_conf.preferred_file_type)
+
+    if c_conf.preferred_mask_file_type is None:
+        # Use png by default.
+        final_mask_out_path = final_mask_out_path.with_suffix(".png")
+    else:
+        final_mask_out_path = final_mask_out_path.with_suffix(c_conf.preferred_mask_file_type)
+
     logger.debug(f"Final output path: {final_cleaned_out_path}")
 
     # The arg parser should ensure that both can't be true at once, not like that'd be an issue, just plain silly.
     if not d_data.save_only_mask:
         # Save the final image.
         logger.debug(f"Saving final image to {final_cleaned_out_path}")
         cleaned_image.save(final_cleaned_out_path)
@@ -81,11 +95,16 @@
 
     if d_data.extract_text:
         # Extract the text layer from the image.
         logger.debug(f"Extracting text from {mask_data.original_path}")
         base_image = Image.open(mask_data.original_path)
         text_img = ops.extract_text(base_image, mask_image)
         text_out_path = final_out_path.with_name(final_out_path.stem + "_text.png")
+        if c_conf.preferred_mask_file_type is None:
+            # Use png by default.
+            text_out_path = text_out_path.with_suffix(".png")
+        else:
+            text_out_path = text_out_path.with_suffix(c_conf.preferred_mask_file_type)
         text_img.save(text_out_path)
 
     # Package the analytics. We're only interested in the std deviations.
     return st.DenoiseAnalytic(tuple(deviation for _, deviation in mask_data.boxes_with_deviation))
```

### Comparing `pcleaner-1.3.0/pcleaner/image_ops.py` & `pcleaner-1.4.0/pcleaner/image_ops.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import colorsys
 from pathlib import Path
+from typing import Generator
 
 import numpy as np
 import cv2
 import scipy
 from PIL import Image, ImageFilter
 from logzero import logger
 
@@ -138,25 +139,26 @@
     alpha_mask = alpha_mask.point(lambda x: min(x, 153))
     base_image.paste(combined_mask, (0, 0), alpha_mask)
 
     # Save the image.
     base_image.save(output_path)
 
 
-def make_mask_steps_convolution(mask: Image, growth_step: int = 2, steps: int = 11) -> list[Image]:
+def make_mask_steps_convolution(
+    mask: Image, growth_step: int = 2, steps: int = 11
+) -> Generator[list[Image], None, None]:
     """
     Use convolution to make various sizes of the original mask.
     In each step, the outline of the mask is grown by growth_step pixels.
 
     :param mask: The mask to make steps of.
     :param growth_step: The amount to grow the mask by each step.
     :param steps: The number of steps to make.
     :return:
     """
-    masks = []
     grow_size = growth_step * 2
     mask = mask.convert("L")
     mask_array = np.array(mask, dtype=np.uint8)
     # Make a convolution kernel.
     kernel = np.ones((grow_size + 1, grow_size + 1))
     # Remove the corner pixels from the kernel, this will give 45 degree corners.
     kernel[0, 0] = 0
@@ -166,20 +168,15 @@
     # Pad the image so that the convolution can handle the edges.
     padded_mask = np.pad(mask_array, ((grow_size, grow_size), (grow_size, grow_size)), mode="edge")
 
     for _ in range(steps):
         # Apply convolve2d to the image.
         padded_mask = scipy.signal.convolve2d(padded_mask, kernel, mode="same")
         cropped_mask = padded_mask[grow_size:-grow_size, grow_size:-grow_size]
-        masks.append(
-            Image.fromarray(np.where(cropped_mask > 0, 255, 0).astype(np.uint8)).convert("1")
-        )
-
-    # Return them ordered from smallest to largest.
-    return masks
+        yield Image.fromarray(np.where(cropped_mask > 0, 255, 0).astype(np.uint8)).convert("1")
 
 
 def border_std_deviation(base: Image, mask: Image, off_white_threshold: int) -> tuple[float, int]:
     """
     Calculate the border uniformity of a mask.
     For this, find the edge pixels of the mask and then calculate the median color of the pixels around them.
     Also calculate the standard deviation of the colors around the edge pixels.
@@ -264,14 +261,15 @@
 def pick_best_mask(
     base: Image,
     precise_mask: Image,
     box_mask: Image,
     masking_box: tuple[int, int, int, int],
     reference_box: tuple[int, int, int, int],
     cleaner_conf: cfg.CleanerConfig,
+    save_masks: bool,
     analytics_page_path: Path,
 ) -> None | st.MaskFittingResults:
     """
     Generate various sizes of the precise mask and pick the best one from
     among them, and the box mask.
 
     Return the best mask, the median color of the border, and the coordinates of the mask.
@@ -289,14 +287,15 @@
 
     :param base: The base image.
     :param precise_mask: The precise mask.
     :param box_mask: The box mask.
     :param masking_box: The box to cut the mask out of.
     :param reference_box: The box to cut the base image out of.
     :param cleaner_conf: The cleaner config.
+    :param save_masks: Whether to save the masks.
     :param analytics_page_path: The path to the original image for the analytics.
     :return: The best mask and what color to make it and the box (along with analytics). If no best
         mask was found, return None for the mask and color.
     """
     # Calculate offset coords between the reference box and the mask box.
     # The mask box was grown by n pixels in each direction to make the reference box,
     # but it could not exceed the image dimensions.
@@ -314,39 +313,59 @@
         logger.warning("Found an empty mask, this is likely due to name collisions.")
         return None
 
     box_mask = cut_out_mask(box_mask, masking_box, base.size, x_offset, y_offset)
 
     # Generate masks of various sizes for the precise mask, then add the box mask to the list.
     # The generated masks are in ascending size order.
-    masks = make_mask_steps_convolution(
+    mask_gen = make_mask_steps_convolution(
         precise_mask, cleaner_conf.mask_growth_step_pixels, cleaner_conf.mask_growth_steps
     )
-    masks.append(box_mask)
+    # When using the fast mask selection, make a new generator with the box mask as the first mask,
+    # followed by the generated masks.
+    def generator_with_first(generator, first):
+        yield first
+        yield from generator
+
+    def generator_with_last(generator, last):
+        yield from generator
+        yield last
+
+    if cleaner_conf.mask_selection_fast:
+        mask_stream = generator_with_first(mask_gen, box_mask)
+    else:
+        mask_stream = generator_with_last(mask_gen, box_mask)
 
     # Calculate the border uniformity of each mask.
     # Border deviations: (std deviation, median color)
     border_deviations: list[tuple[Image, int]] = []
-    for mask in masks:
+    masks = []
+    for mask in mask_stream:
         try:
-            border_deviations.append(
-                border_std_deviation(base, mask, cleaner_conf.off_white_max_threshold)
+            masks.append(mask)
+            current_deviation = border_std_deviation(
+                base, mask, cleaner_conf.off_white_max_threshold
             )
+            border_deviations.append(current_deviation)
+            # Break on the first perfect mask if using the fast mask selection.
+            if cleaner_conf.mask_selection_fast and current_deviation[0] == 0:
+                break
         except BlankMaskError:
             return None
     # Find the best mask.
     best_mask = None
     lowest_border_deviation = None
     lowest_deviation_color = None
-    for i in range(len(masks)):
-        if i == 0 or border_deviations[i][0] <= (
+    for i, border_deviation in enumerate(border_deviations):
+        mask_deviation, mask_color = border_deviation
+        if i == 0 or mask_deviation <= (
             lowest_border_deviation * (1 - cleaner_conf.mask_improvement_threshold)
         ):
-            lowest_border_deviation = border_deviations[i][0]
-            lowest_deviation_color = border_deviations[i][1]
+            lowest_border_deviation = mask_deviation
+            lowest_deviation_color = mask_color
             best_mask = masks[i]
 
     # If the std deviation is too high, return None.
     if lowest_border_deviation > cleaner_conf.mask_max_standard_deviation:
         return st.MaskFittingResults(
             best_mask=None,
             median_color=lowest_deviation_color,
```

### Comparing `pcleaner-1.3.0/pcleaner/main.py` & `pcleaner-1.4.0/pcleaner/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,14 @@
 import pcleaner.pre_processor as pp
 import pcleaner.analytics as an
 import pcleaner.structures as st
 import pcleaner.profile_cli as pc
 import pcleaner.denoiser as dn
 import pcleaner.model_downloader as md
 
-# TODO mask data and beyond isn't clobber protexted.
 
 def main():
 
     args = magic_docopt(__doc__, version=f"Panel Cleaner {__version__}")
     # Loglevel is info by default.
     if args.debug:
         loglevel(DEBUG)
@@ -287,15 +286,23 @@
         if len(list(cache_dir.glob("*"))) > 0 and not keep_cache:
             cli.empty_cache_dir(cache_dir)
         # Get the model file, downloading it if necessary.
         cuda = torch.cuda.is_available()
         model_path = config.get_model_path(cuda)
 
         print("Running text detection AI model...")
-        pp.generate_mask_data(image_paths, model_path=model_path, output_dir=cache_dir)
+        print(profile.text_detector)
+        pp.generate_mask_data(
+            image_paths, config=profile.text_detector, model_path=model_path, output_dir=cache_dir
+        )
+
+        if debug:
+            loglevel(DEBUG)
+        else:
+            loglevel(INFO)
 
         # Leave some extra space here if drawing analytics, so it looks better.
         if not hide_analytics:
             print("\n")
 
     if not skip_pre_processing:
         # Flush it so it shows up before the progress bar.
@@ -367,14 +374,15 @@
         # Zip together the json files and the out path thing.
         data = [
             st.DenoiserData(
                 json_file,
                 output_dir,
                 cache_dir,
                 profile.denoiser,
+                profile.cleaner,
                 save_only_mask,
                 save_only_cleaned,
                 extract_text,
                 separate_noise_mask,
                 cache_masks,
                 debug,
             )
```

### Comparing `pcleaner-1.3.0/pcleaner/model_downloader.py` & `pcleaner-1.4.0/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/pre_processor.py` & `pcleaner-1.4.0/pcleaner/pre_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 from manga_ocr import MangaOcr
 
 import pcleaner.ctd_interface as ctm
 import pcleaner.structures as st
 import pcleaner.config as cfg
 
 
-def generate_mask_data(image_path: list[Path], model_path: Path, output_dir: Path) -> None:
+def generate_mask_data(
+    image_path: list[Path], config: cfg.TextDetectorConfig, model_path: Path, output_dir: Path
+) -> None:
     """
     Run the ai model to generate masks and box data for the given image,
     or all images in the given directory.
 
     :param image_path: Path to the image or directory of images.
+    :param config: Text detector configuration, part of the profile.
     :param model_path: Path to the model file.
     :param output_dir: Path to the directory where the results will be saved.
     """
 
-    ctm.model2annotations(model_path, image_path, output_dir)
+    ctm.model2annotations(config, model_path, image_path, output_dir)
 
 
 def prep_json_file(
     json_file_path: Path,
     pre_processor_conf: cfg.PreProcessorConfig,
     cache_masks: bool,
     mocr: MangaOcr | None = None,
```

### Comparing `pcleaner-1.3.0/pcleaner/profile_cli.py` & `pcleaner-1.4.0/pcleaner/profile_cli.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/pcleaner/structures.py` & `pcleaner-1.4.0/pcleaner/structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,26 +346,28 @@
     """
     This is a simple struct to hold the inputs for the denoiser.
     The data is a tuple of:
     - The json file path.
     - The image output directory.
     - The image cache directory.
     - The denoiser config.
+    - The cleaner config.
     - The save only mask flag.
     - The save only cleaned flag.
     - The extract text flag.
     - The separate noise mask flag.
     - The show masks flag. (when true, save intermediate masks to the cache directory)
     - The debug flag.
     """
 
     json_path: Path
     output_dir: Path
     cache_dir: Path
     denoiser_config: cfg.DenoiserConfig
+    cleaner_config: cfg.CleanerConfig
     save_only_mask: bool
     save_only_cleaned: bool
     extract_text: bool
     separate_noise_masks: bool
     show_masks: bool
     debug: bool
```

### Comparing `pcleaner-1.3.0/pcleaner.egg-info/PKG-INFO` & `pcleaner-1.4.0/pcleaner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.3.0
+Version: 1.4.0
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
@@ -64,21 +64,25 @@
 
 - Supports CUDA acceleration, if your hardware supports it.
 
 - Supports batch processing of images and directories.
 
 - Can handle bubbles on any solid grayscale background color.
 
+- Can also cut out the text from the rest of the image, e.g. to paste it over a colored rendition.
+
 - Can also run OCR on the pages and output the text to a file.
 
 
 ## Limitations
 
 - It only supports Japanese and English text.
 
+- Supported file types: .jpeg, .jpg, .png, .bmp, .tiff, .tif, .jp2, .dib, .webp, .ppm
+
 - The program relies on AI for the initial text detection, which by nature is imperfect. Sometimes it will miss little bits of text or think part of the bubble belongs to the text, which will prevent that bubble from being cleaned. From testing, this typically affects between 2–8% of bubbles, depending on your settings.
 
 - Due to the conservative approach taken in the selection of masks, if the program can't clean the bubble to a satisfying degree, it will skip that bubble outright. This does, however, also prevent false positives.
 
 - For masks, only grayscale is currently supported. This means it can cover up text in white, black, or gray bubbles, but not colored ones.
```

### Comparing `pcleaner-1.3.0/pcleaner.egg-info/SOURCES.txt` & `pcleaner-1.4.0/pcleaner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcleaner-1.3.0/setup.cfg` & `pcleaner-1.4.0/setup.cfg`

 * *Files identical despite different names*

