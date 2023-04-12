# Comparing `tmp/metaseg-0.6.0.tar.gz` & `tmp/metaseg-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.6.0.tar", last modified: Wed Apr 12 15:06:21 2023, max compression
+gzip compressed data, was "metaseg-0.6.1.tar", last modified: Wed Apr 12 16:55:23 2023, max compression
```

## Comparing `metaseg-0.6.0.tar` & `metaseg-0.6.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.600587 metaseg-0.6.0/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-12 11:10:24.000000 metaseg-0.6.0/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-12 11:10:24.000000 metaseg-0.6.0/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 15:06:21.600587 metaseg-0.6.0/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2953 2023-04-12 11:10:24.000000 metaseg-0.6.0/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.590587 metaseg-0.6.0/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      631 2023-04-12 15:05:56.000000 metaseg-0.6.0/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.593920 metaseg-0.6.0/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6198 2023-04-12 12:18:37.000000 metaseg-0.6.0/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.597253 metaseg-0.6.0/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3515 2023-04-12 14:10:32.000000 metaseg-0.6.0/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.600587 metaseg-0.6.0/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.600587 metaseg-0.6.0/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8416 2023-04-12 15:06:15.000000 metaseg-0.6.0/metaseg/webapp/app.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2470 2023-04-12 15:06:16.000000 metaseg-0.6.0/metaseg/webapp/demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.590587 metaseg-0.6.0/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 15:06:21.000000 metaseg-0.6.0/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      881 2023-04-12 15:06:21.000000 metaseg-0.6.0/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-12 15:06:21.000000 metaseg-0.6.0/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      230 2023-04-12 15:06:21.000000 metaseg-0.6.0/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-12 15:06:21.000000 metaseg-0.6.0/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-12 11:10:24.000000 metaseg-0.6.0/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      143 2023-04-12 13:57:00.000000 metaseg-0.6.0/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-12 15:06:21.600587 metaseg-0.6.0/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-12 11:10:24.000000 metaseg-0.6.0/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.451956 metaseg-0.6.1/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-12 11:10:24.000000 metaseg-0.6.1/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-12 11:10:24.000000 metaseg-0.6.1/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3531 2023-04-12 16:55:23.451956 metaseg-0.6.1/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3257 2023-04-12 16:55:20.000000 metaseg-0.6.1/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.445290 metaseg-0.6.1/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      631 2023-04-12 16:55:20.000000 metaseg-0.6.1/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.448623 metaseg-0.6.1/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8608 2023-04-12 16:55:20.000000 metaseg-0.6.1/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.448623 metaseg-0.6.1/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3515 2023-04-12 16:41:21.000000 metaseg-0.6.1/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.448623 metaseg-0.6.1/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.451956 metaseg-0.6.1/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.6.1/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8416 2023-04-12 16:41:21.000000 metaseg-0.6.1/metaseg/webapp/app.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2470 2023-04-12 16:41:21.000000 metaseg-0.6.1/metaseg/webapp/demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 16:55:23.445290 metaseg-0.6.1/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3531 2023-04-12 16:55:23.000000 metaseg-0.6.1/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      881 2023-04-12 16:55:23.000000 metaseg-0.6.1/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-12 16:55:23.000000 metaseg-0.6.1/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      230 2023-04-12 16:55:23.000000 metaseg-0.6.1/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-12 16:55:23.000000 metaseg-0.6.1/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-12 11:10:24.000000 metaseg-0.6.1/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      143 2023-04-12 16:41:21.000000 metaseg-0.6.1/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-12 16:55:23.451956 metaseg-0.6.1/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-12 11:10:24.000000 metaseg-0.6.1/setup.py
```

### Comparing `metaseg-0.6.0/LICENSE` & `metaseg-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/PKG-INFO` & `metaseg-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.6.0
+Version: 0.6.1
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -58,25 +58,40 @@
     points_per_batch=64,
     min_area=1000,
     output_path="output.mp4",
 )
 
 # For manuel box and point selection
 
+# For image
 results = SegManualMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
     input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]]
     multimask_output=False,
     random_color=False,
     show=True,
     save=False,
 )
+
+# For video
+
+results = SegManualMaskPredictor().video_predict(
+    source="test.mp4",
+    model_type="vit_l", # vit_l, vit_h, vit_b
+    input_point=[0, 0, 100, 100]
+    input_label=N
+    input_box=None,
+    multimask_output=False,
+    random_color=False,
+    output_path="output.mp4",
+)
+```
 ```
 
 ### SAHI + Segment Anything
 
 ```python
 from metaseg import sahi_sliced_predict, SahiAutoSegmentation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.6.0 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.6.1 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
@@ -11,20 +11,24 @@
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
 points_per_side and points_per_batch. # For image results =
 SegAutoMaskPredictor().image_predict( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0,
 output_path="output.jpg", show=True, save=False, ) # For video results =
 SegAutoMaskPredictor().video_predict( source="video.mp4", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=1000,
-output_path="output.mp4", ) # For manuel box and point selection results =
-SegManualMaskPredictor().image_predict( source="image.jpg", model_type="vit_l",
-# vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]], input_label=[0, 1],
-input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200,
-200]] multimask_output=False, random_color=False, show=True, save=False, ) ```
-### SAHI + Segment Anything ```python from metaseg import sahi_sliced_predict,
+output_path="output.mp4", ) # For manuel box and point selection # For image
+results = SegManualMaskPredictor().image_predict( source="image.jpg",
+model_type="vit_l", # vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]],
+input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200],
+[100, 100, 200, 200]] multimask_output=False, random_color=False, show=True,
+save=False, ) # For video results = SegManualMaskPredictor().video_predict
+( source="test.mp4", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[0,
+0, 100, 100] input_label=N input_box=None, multimask_output=False,
+random_color=False, output_path="output.mp4", ) ``` ``` ### SAHI + Segment
+Anything ```python from metaseg import sahi_sliced_predict,
 SahiAutoSegmentation image_path = "test.jpg" boxes = sahi_sliced_predict
 ( image_path=image_path, detection_model_type="yolov5", #yolov8, detectron2,
 mmdetection, torchvision detection_model_path="yolov5l6.pt", conf_th=0.25,
 image_size=1280, slice_height=256, slice_width=256, overlap_height_ratio=0.2,
 overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
 model_type="vit_b", input_box=boxes, multimask_output=False,
 random_color=False, show=True, save=False, ) ``` [teaser] # Extra Features -
```

### Comparing `metaseg-0.6.0/README.md` & `metaseg-0.6.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -46,25 +46,40 @@
     points_per_batch=64,
     min_area=1000,
     output_path="output.mp4",
 )
 
 # For manuel box and point selection
 
+# For image
 results = SegManualMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
     input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]]
     multimask_output=False,
     random_color=False,
     show=True,
     save=False,
 )
+
+# For video
+
+results = SegManualMaskPredictor().video_predict(
+    source="test.mp4",
+    model_type="vit_l", # vit_l, vit_h, vit_b
+    input_point=[0, 0, 100, 100]
+    input_label=N
+    input_box=None,
+    multimask_output=False,
+    random_color=False,
+    output_path="output.mp4",
+)
+```
 ```
 
 ### SAHI + Segment Anything
 
 ```python
 from metaseg import sahi_sliced_predict, SahiAutoSegmentation
```

#### html2text {}

```diff
@@ -7,20 +7,24 @@
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
 points_per_side and points_per_batch. # For image results =
 SegAutoMaskPredictor().image_predict( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0,
 output_path="output.jpg", show=True, save=False, ) # For video results =
 SegAutoMaskPredictor().video_predict( source="video.mp4", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=1000,
-output_path="output.mp4", ) # For manuel box and point selection results =
-SegManualMaskPredictor().image_predict( source="image.jpg", model_type="vit_l",
-# vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]], input_label=[0, 1],
-input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200,
-200]] multimask_output=False, random_color=False, show=True, save=False, ) ```
-### SAHI + Segment Anything ```python from metaseg import sahi_sliced_predict,
+output_path="output.mp4", ) # For manuel box and point selection # For image
+results = SegManualMaskPredictor().image_predict( source="image.jpg",
+model_type="vit_l", # vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]],
+input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200],
+[100, 100, 200, 200]] multimask_output=False, random_color=False, show=True,
+save=False, ) # For video results = SegManualMaskPredictor().video_predict
+( source="test.mp4", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[0,
+0, 100, 100] input_label=N input_box=None, multimask_output=False,
+random_color=False, output_path="output.mp4", ) ``` ``` ### SAHI + Segment
+Anything ```python from metaseg import sahi_sliced_predict,
 SahiAutoSegmentation image_path = "test.jpg" boxes = sahi_sliced_predict
 ( image_path=image_path, detection_model_type="yolov5", #yolov8, detectron2,
 mmdetection, torchvision detection_model_path="yolov5l6.pt", conf_th=0.25,
 image_size=1280, slice_height=256, slice_width=256, overlap_height_ratio=0.2,
 overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
 model_type="vit_b", input_box=boxes, multimask_output=False,
 random_color=False, show=True, save=False, ) ``` [teaser] # Extra Features -
```

### Comparing `metaseg-0.6.0/metaseg/__init__.py` & `metaseg-0.6.1/metaseg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
```

### Comparing `metaseg-0.6.0/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.6.1/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/generator/build_sam.py` & `metaseg-0.6.1/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/generator/predictor.py` & `metaseg-0.6.1/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/mask_predictor.py` & `metaseg-0.6.1/metaseg/mask_predictor.py`

 * *Files 15% similar despite different names*

```diff
@@ -182,7 +182,91 @@
         if save:
             save_image(output_path=output_path, output_image=combined_mask)
 
         if show:
             show_image(combined_mask)
 
         return masks
+
+    def video_predict(
+        self,
+        source,
+        model_type,
+        input_box=None,
+        input_point=None,
+        input_label=None,
+        multimask_output=False,
+        output_path="output.mp4",
+        random_color=False,
+    ):
+        cap, out = load_video(source, output_path)
+        length = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+
+        for _ in tqdm(range(length)):
+            ret, frame = cap.read()
+            if not ret:
+                break
+
+            model = self.load_model(model_type)
+            predictor = SamPredictor(model)
+            predictor.set_image(frame)
+
+            if type(input_box[0]) == list:
+                input_boxes, new_boxes = multi_boxes(input_box, predictor, frame)
+
+                masks, _, _ = predictor.predict_torch(
+                    point_coords=None,
+                    point_labels=None,
+                    boxes=new_boxes,
+                    multimask_output=False,
+                )
+                for mask in masks:
+                    mask_image = load_mask(mask.cpu().numpy(), random_color)
+
+                for box in input_boxes:
+                    frame = load_box(box.cpu().numpy(), frame)
+
+            elif type(input_box[0]) == int:
+                input_boxes = np.array(input_box)[None, :]
+
+                masks, _, _ = predictor.predict(
+                    point_coords=input_point,
+                    point_labels=input_label,
+                    box=input_boxes,
+                    multimask_output=multimask_output,
+                )
+                mask_image = load_mask(masks, random_color)
+                frame = load_box(input_box, frame)
+
+            combined_mask = cv2.add(frame, mask_image)
+            out.write(combined_mask)
+
+        out.release()
+        cap.release()
+        cv2.destroyAllWindows()
+        return output_path
+    
+if __name__ == "__main__":
+    # video
+    source = "test.mp4"
+    model_type = "sam_resnet50d_ade20k"
+    input_box = [0, 0, 100, 100]
+    input_point = None
+    input_label = None
+    multimask_output = False
+    output_path = "output.mp4"
+    random_color = False
+    show = False
+    save = True
+
+    # video
+    predictor = SegManualMaskPredictor()
+    predictor.video_predict(
+        source,
+        model_type,
+        input_box,
+        input_point,
+        input_label,
+        multimask_output,
+        output_path,
+        random_color,
+    )
```

### Comparing `metaseg-0.6.0/metaseg/modeling/common.py` & `metaseg-0.6.1/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/modeling/image_encoder.py` & `metaseg-0.6.1/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/modeling/mask_decoder.py` & `metaseg-0.6.1/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/modeling/prompt_encoder.py` & `metaseg-0.6.1/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/modeling/sam.py` & `metaseg-0.6.1/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/modeling/transformer.py` & `metaseg-0.6.1/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/sahi_predict.py` & `metaseg-0.6.1/metaseg/sahi_predict.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/utils/amg.py` & `metaseg-0.6.1/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/utils/data_utils.py` & `metaseg-0.6.1/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/utils/file_utils.py` & `metaseg-0.6.1/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/utils/onnx.py` & `metaseg-0.6.1/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/utils/transforms.py` & `metaseg-0.6.1/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/webapp/app.py` & `metaseg-0.6.1/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg/webapp/demo.py` & `metaseg-0.6.1/metaseg/webapp/demo.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/metaseg.egg-info/PKG-INFO` & `metaseg-0.6.1/metaseg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.6.0
+Version: 0.6.1
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -58,25 +58,40 @@
     points_per_batch=64,
     min_area=1000,
     output_path="output.mp4",
 )
 
 # For manuel box and point selection
 
+# For image
 results = SegManualMaskPredictor().image_predict(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     input_point=[[100, 100], [200, 200]],
     input_label=[0, 1],
     input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200, 200]]
     multimask_output=False,
     random_color=False,
     show=True,
     save=False,
 )
+
+# For video
+
+results = SegManualMaskPredictor().video_predict(
+    source="test.mp4",
+    model_type="vit_l", # vit_l, vit_h, vit_b
+    input_point=[0, 0, 100, 100]
+    input_label=N
+    input_box=None,
+    multimask_output=False,
+    random_color=False,
+    output_path="output.mp4",
+)
+```
 ```
 
 ### SAHI + Segment Anything
 
 ```python
 from metaseg import sahi_sliced_predict, SahiAutoSegmentation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.6.0 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.6.1 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
@@ -11,20 +11,24 @@
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
 points_per_side and points_per_batch. # For image results =
 SegAutoMaskPredictor().image_predict( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0,
 output_path="output.jpg", show=True, save=False, ) # For video results =
 SegAutoMaskPredictor().video_predict( source="video.mp4", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=1000,
-output_path="output.mp4", ) # For manuel box and point selection results =
-SegManualMaskPredictor().image_predict( source="image.jpg", model_type="vit_l",
-# vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]], input_label=[0, 1],
-input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200], [100, 100, 200,
-200]] multimask_output=False, random_color=False, show=True, save=False, ) ```
-### SAHI + Segment Anything ```python from metaseg import sahi_sliced_predict,
+output_path="output.mp4", ) # For manuel box and point selection # For image
+results = SegManualMaskPredictor().image_predict( source="image.jpg",
+model_type="vit_l", # vit_l, vit_h, vit_b input_point=[[100, 100], [200, 200]],
+input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100, 200, 200],
+[100, 100, 200, 200]] multimask_output=False, random_color=False, show=True,
+save=False, ) # For video results = SegManualMaskPredictor().video_predict
+( source="test.mp4", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[0,
+0, 100, 100] input_label=N input_box=None, multimask_output=False,
+random_color=False, output_path="output.mp4", ) ``` ``` ### SAHI + Segment
+Anything ```python from metaseg import sahi_sliced_predict,
 SahiAutoSegmentation image_path = "test.jpg" boxes = sahi_sliced_predict
 ( image_path=image_path, detection_model_type="yolov5", #yolov8, detectron2,
 mmdetection, torchvision detection_model_path="yolov5l6.pt", conf_th=0.25,
 image_size=1280, slice_height=256, slice_width=256, overlap_height_ratio=0.2,
 overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
 model_type="vit_b", input_box=boxes, multimask_output=False,
 random_color=False, show=True, save=False, ) ``` [teaser] # Extra Features -
```

### Comparing `metaseg-0.6.0/metaseg.egg-info/SOURCES.txt` & `metaseg-0.6.1/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.6.0/setup.py` & `metaseg-0.6.1/setup.py`

 * *Files identical despite different names*

