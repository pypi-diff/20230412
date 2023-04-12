# Comparing `tmp/clarifai-9.3.1.tar.gz` & `tmp/clarifai-9.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-9.3.1.tar", last modified: Tue Apr 11 15:56:54 2023, max compression
+gzip compressed data, was "clarifai-9.3.2.tar", last modified: Wed Apr 12 18:10:29 2023, max compression
```

## Comparing `clarifai-9.3.1.tar` & `clarifai-9.3.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.734809 clarifai-9.3.1/
--rw-r--r--   0 zeiler     (503) staff       (20)      555 2021-12-09 18:28:59.000000 clarifai-9.3.1/LICENSE
--rw-r--r--   0 zeiler     (503) staff       (20)       21 2022-07-01 04:22:44.000000 clarifai-9.3.1/MANIFEST.in
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-04-11 15:56:54.734598 clarifai-9.3.1/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     2347 2023-01-03 21:48:03.000000 clarifai-9.3.1/README.md
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.721911 clarifai-9.3.1/clarifai/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.722861 clarifai-9.3.1/clarifai/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.723595 clarifai-9.3.1/clarifai/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.724118 clarifai-9.3.1/clarifai/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/data_upload/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.725368 clarifai-9.3.1/clarifai/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.726019 clarifai-9.3.1/clarifai/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.727920 clarifai-9.3.1/clarifai/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7710 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.728681 clarifai-9.3.1/clarifai/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.729052 clarifai-9.3.1/clarifai/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.3.1/clarifai/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.3.1/clarifai/urls/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.722612 clarifai-9.3.1/clarifai.egg-info/
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-04-11 15:56:54.000000 clarifai-9.3.1/clarifai.egg-info/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     2555 2023-04-11 15:56:54.000000 clarifai-9.3.1/clarifai.egg-info/SOURCES.txt
--rw-r--r--   0 zeiler     (503) staff       (20)        1 2023-04-11 15:56:54.000000 clarifai-9.3.1/clarifai.egg-info/dependency_links.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       21 2023-04-11 15:56:54.000000 clarifai-9.3.1/clarifai.egg-info/requires.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       24 2023-04-11 15:56:54.000000 clarifai-9.3.1/clarifai.egg-info/top_level.txt
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.729314 clarifai-9.3.1/clarifai_utils/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.729546 clarifai-9.3.1/clarifai_utils/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.729960 clarifai-9.3.1/clarifai_utils/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.730339 clarifai-9.3.1/clarifai_utils/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/data_upload/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.731032 clarifai-9.3.1/clarifai_utils/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.731654 clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.733324 clarifai-9.3.1/clarifai_utils/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai_utils/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7710 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai_utils/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai_utils/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai_utils/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.734064 clarifai-9.3.1/clarifai_utils/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.734373 clarifai-9.3.1/clarifai_utils/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.3.1/clarifai_utils/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.3.1/clarifai_utils/urls/helper.py
--rw-r--r--   0 zeiler     (503) staff       (20)       38 2023-04-11 15:56:54.734866 clarifai-9.3.1/setup.cfg
--rw-r--r--   0 zeiler     (503) staff       (20)      887 2023-04-11 15:55:59.000000 clarifai-9.3.1/setup.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.564670 clarifai-9.3.2/
+-rw-r--r--   0 zeiler     (503) staff       (20)      555 2021-12-09 18:28:59.000000 clarifai-9.3.2/LICENSE
+-rw-r--r--   0 zeiler     (503) staff       (20)       21 2022-07-01 04:22:44.000000 clarifai-9.3.2/MANIFEST.in
+-rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-04-12 18:10:29.564470 clarifai-9.3.2/PKG-INFO
+-rw-r--r--   0 zeiler     (503) staff       (20)     2347 2023-01-03 21:48:03.000000 clarifai-9.3.2/README.md
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.552491 clarifai-9.3.2/clarifai/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.553402 clarifai-9.3.2/clarifai/auth/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/auth/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/auth/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.554028 clarifai-9.3.2/clarifai/client/
+-rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/client/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/client/abc.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/client/stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.554527 clarifai-9.3.2/clarifai/data_upload/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/data_upload/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.555547 clarifai-9.3.2/clarifai/data_upload/datasets/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/base.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/features.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/image.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/text.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.556330 clarifai-9.3.2/clarifai/data_upload/datasets/zoo/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/examples.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/data_upload/upload.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.558333 clarifai-9.3.2/clarifai/listing/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/listing/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/listing/concepts.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/listing/datasets.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/listing/inputs.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.3.2/clarifai/listing/installed_module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-04-12 16:48:35.000000 clarifai-9.3.2/clarifai/listing/lister.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/listing/models.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.3.2/clarifai/listing/module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.3.2/clarifai/listing/modules.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.558991 clarifai-9.3.2/clarifai/modules/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/modules/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/modules/css.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai/modules/pages.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai/modules/style.css
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.559375 clarifai-9.3.2/clarifai/urls/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.3.2/clarifai/urls/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.3.2/clarifai/urls/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.553162 clarifai-9.3.2/clarifai.egg-info/
+-rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-04-12 18:10:29.000000 clarifai-9.3.2/clarifai.egg-info/PKG-INFO
+-rw-r--r--   0 zeiler     (503) staff       (20)     2555 2023-04-12 18:10:29.000000 clarifai-9.3.2/clarifai.egg-info/SOURCES.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)        1 2023-04-12 18:10:29.000000 clarifai-9.3.2/clarifai.egg-info/dependency_links.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)       21 2023-04-12 18:10:29.000000 clarifai-9.3.2/clarifai.egg-info/requires.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)       24 2023-04-12 18:10:29.000000 clarifai-9.3.2/clarifai.egg-info/top_level.txt
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.559715 clarifai-9.3.2/clarifai_utils/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.560001 clarifai-9.3.2/clarifai_utils/auth/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/auth/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/auth/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.560467 clarifai-9.3.2/clarifai_utils/client/
+-rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/client/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/client/abc.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/client/stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.560878 clarifai-9.3.2/clarifai_utils/data_upload/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/data_upload/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.561575 clarifai-9.3.2/clarifai_utils/data_upload/datasets/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/base.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/features.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/image.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/text.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.562129 clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/examples.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/data_upload/upload.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.563430 clarifai-9.3.2/clarifai_utils/listing/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/listing/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/listing/concepts.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/listing/datasets.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/listing/inputs.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.3.2/clarifai_utils/listing/installed_module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-04-12 16:48:35.000000 clarifai-9.3.2/clarifai_utils/listing/lister.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/listing/models.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.3.2/clarifai_utils/listing/module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.3.2/clarifai_utils/listing/modules.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.563970 clarifai-9.3.2/clarifai_utils/modules/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/modules/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/modules/css.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.3.2/clarifai_utils/modules/pages.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.3.2/clarifai_utils/modules/style.css
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-12 18:10:29.564228 clarifai-9.3.2/clarifai_utils/urls/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.3.2/clarifai_utils/urls/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.3.2/clarifai_utils/urls/helper.py
+-rw-r--r--   0 zeiler     (503) staff       (20)       38 2023-04-12 18:10:29.564720 clarifai-9.3.2/setup.cfg
+-rw-r--r--   0 zeiler     (503) staff       (20)      887 2023-04-12 18:10:12.000000 clarifai-9.3.2/setup.py
```

### Comparing `clarifai-9.3.1/LICENSE` & `clarifai-9.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/PKG-INFO` & `clarifai-9.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.3.1
+Version: 9.3.2
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.3.1/README.md` & `clarifai-9.3.2/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/auth/helper.py` & `clarifai-9.3.2/clarifai/auth/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/client/abc.py` & `clarifai-9.3.2/clarifai/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/client/stub.py` & `clarifai-9.3.2/clarifai/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/data_upload/datasets/base.py` & `clarifai-9.3.2/clarifai/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/data_upload/datasets/features.py` & `clarifai-9.3.2/clarifai/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/data_upload/datasets/image.py` & `clarifai-9.3.2/clarifai/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/data_upload/datasets/text.py` & `clarifai-9.3.2/clarifai/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.3.2/clarifai/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.3.2/clarifai/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.3.2/clarifai/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/data_upload/examples.py` & `clarifai-9.3.2/clarifai/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/data_upload/upload.py` & `clarifai-9.3.2/clarifai/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/listing/concepts.py` & `clarifai-9.3.2/clarifai/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/listing/datasets.py` & `clarifai-9.3.2/clarifai/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/listing/inputs.py` & `clarifai-9.3.2/clarifai/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/listing/installed_module_versions.py` & `clarifai-9.3.2/clarifai/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/listing/lister.py` & `clarifai-9.3.2/clarifai/listing/lister.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,25 +176,25 @@
 
     Returns:
       gen: a generator that yields a single Module proto at a time.
     """
     page_size = self.default_page_size if page_size is None else page_size
     return modules_generator(self.stub, self.user_id, self.app_id, page_size)
 
-  def list_all_module_versions(self, page_size: int = None):
+  def list_all_module_versions(self, module_id: str, page_size: int = None):
     """
     This lists all the module_versions in an app. Not recommended for large apps.
 
     Returns:
       module_versions: a list of ModuleVersion protos for all the module_versions in the app.
     """
-    return [item for item in self.module_versions_generator(page_size)]
+    return [item for item in self.module_versions_generator(module_id, page_size)]
 
-  def module_versions_generator(self, page_size: int = None):
+  def module_versions_generator(self, module_id: str, page_size: int = None):
     """
     This lists all the module_versions in an app. Not recommended for large apps.
 
     Returns:
       gen: a generator that yields a single ModuleVersion proto at a time.
     """
     page_size = self.default_page_size if page_size is None else page_size
-    return module_versions_generator(self.stub, self.user_id, self.app_id, page_size)
+    return module_versions_generator(self.stub, self.user_id, self.app_id, module_id, page_size)
```

### Comparing `clarifai-9.3.1/clarifai/listing/models.py` & `clarifai-9.3.2/clarifai/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/listing/module_versions.py` & `clarifai-9.3.2/clarifai/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/listing/modules.py` & `clarifai-9.3.2/clarifai/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/modules/css.py` & `clarifai-9.3.2/clarifai/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/modules/pages.py` & `clarifai-9.3.2/clarifai/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/modules/style.css` & `clarifai-9.3.2/clarifai/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai/urls/helper.py` & `clarifai-9.3.2/clarifai/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai.egg-info/PKG-INFO` & `clarifai-9.3.2/clarifai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.3.1
+Version: 9.3.2
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.3.1/clarifai.egg-info/SOURCES.txt` & `clarifai-9.3.2/clarifai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/auth/helper.py` & `clarifai-9.3.2/clarifai_utils/auth/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/client/abc.py` & `clarifai-9.3.2/clarifai_utils/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/client/stub.py` & `clarifai-9.3.2/clarifai_utils/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/data_upload/datasets/base.py` & `clarifai-9.3.2/clarifai_utils/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/data_upload/datasets/features.py` & `clarifai-9.3.2/clarifai_utils/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/data_upload/datasets/image.py` & `clarifai-9.3.2/clarifai_utils/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/data_upload/datasets/text.py` & `clarifai-9.3.2/clarifai_utils/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.3.2/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/data_upload/examples.py` & `clarifai-9.3.2/clarifai_utils/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/data_upload/upload.py` & `clarifai-9.3.2/clarifai_utils/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/listing/concepts.py` & `clarifai-9.3.2/clarifai_utils/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/listing/datasets.py` & `clarifai-9.3.2/clarifai_utils/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/listing/inputs.py` & `clarifai-9.3.2/clarifai_utils/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/listing/installed_module_versions.py` & `clarifai-9.3.2/clarifai_utils/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/listing/lister.py` & `clarifai-9.3.2/clarifai_utils/listing/lister.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,25 +176,25 @@
 
     Returns:
       gen: a generator that yields a single Module proto at a time.
     """
     page_size = self.default_page_size if page_size is None else page_size
     return modules_generator(self.stub, self.user_id, self.app_id, page_size)
 
-  def list_all_module_versions(self, page_size: int = None):
+  def list_all_module_versions(self, module_id: str, page_size: int = None):
     """
     This lists all the module_versions in an app. Not recommended for large apps.
 
     Returns:
       module_versions: a list of ModuleVersion protos for all the module_versions in the app.
     """
-    return [item for item in self.module_versions_generator(page_size)]
+    return [item for item in self.module_versions_generator(module_id, page_size)]
 
-  def module_versions_generator(self, page_size: int = None):
+  def module_versions_generator(self, module_id: str, page_size: int = None):
     """
     This lists all the module_versions in an app. Not recommended for large apps.
 
     Returns:
       gen: a generator that yields a single ModuleVersion proto at a time.
     """
     page_size = self.default_page_size if page_size is None else page_size
-    return module_versions_generator(self.stub, self.user_id, self.app_id, page_size)
+    return module_versions_generator(self.stub, self.user_id, self.app_id, module_id, page_size)
```

### Comparing `clarifai-9.3.1/clarifai_utils/listing/models.py` & `clarifai-9.3.2/clarifai_utils/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/listing/module_versions.py` & `clarifai-9.3.2/clarifai_utils/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/listing/modules.py` & `clarifai-9.3.2/clarifai_utils/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/modules/css.py` & `clarifai-9.3.2/clarifai_utils/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/modules/pages.py` & `clarifai-9.3.2/clarifai_utils/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/modules/style.css` & `clarifai-9.3.2/clarifai_utils/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/clarifai_utils/urls/helper.py` & `clarifai-9.3.2/clarifai_utils/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.1/setup.py` & `clarifai-9.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 packages = setuptools.find_packages(include=["clarifai*"])
 
 setuptools.setup(
     name="clarifai",
-    version="9.3.1",
+    version="9.3.2",
     author="Clarifai",
     author_email="support@clarifai.com",
     description="Clarifai Python Utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Clarifai/clarifai-python-utils",
     packages=packages,
```

