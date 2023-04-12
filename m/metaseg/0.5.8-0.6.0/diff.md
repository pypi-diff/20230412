# Comparing `tmp/metaseg-0.5.8.tar.gz` & `tmp/metaseg-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.5.8.tar", last modified: Wed Apr 12 14:11:06 2023, max compression
+gzip compressed data, was "metaseg-0.6.0.tar", last modified: Wed Apr 12 15:06:21 2023, max compression
```

## Comparing `metaseg-0.5.8.tar` & `metaseg-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.720409 metaseg-0.5.8/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-12 11:10:24.000000 metaseg-0.5.8/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-12 11:10:24.000000 metaseg-0.5.8/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 14:11:06.723743 metaseg-0.5.8/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2953 2023-04-12 11:10:24.000000 metaseg-0.5.8/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.710409 metaseg-0.5.8/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      631 2023-04-12 14:10:44.000000 metaseg-0.5.8/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.713743 metaseg-0.5.8/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6198 2023-04-12 12:18:37.000000 metaseg-0.5.8/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.717076 metaseg-0.5.8/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3515 2023-04-12 14:10:32.000000 metaseg-0.5.8/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.720409 metaseg-0.5.8/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.720409 metaseg-0.5.8/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8827 2023-04-12 13:37:18.000000 metaseg-0.5.8/metaseg/webapp/app.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2489 2023-04-12 13:42:49.000000 metaseg-0.5.8/metaseg/webapp/demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.713743 metaseg-0.5.8/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 14:11:06.000000 metaseg-0.5.8/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      881 2023-04-12 14:11:06.000000 metaseg-0.5.8/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-12 14:11:06.000000 metaseg-0.5.8/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      230 2023-04-12 14:11:06.000000 metaseg-0.5.8/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-12 14:11:06.000000 metaseg-0.5.8/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-12 11:10:24.000000 metaseg-0.5.8/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      143 2023-04-12 13:57:00.000000 metaseg-0.5.8/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-12 14:11:06.723743 metaseg-0.5.8/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-12 11:10:24.000000 metaseg-0.5.8/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.600587 metaseg-0.6.0/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-12 11:10:24.000000 metaseg-0.6.0/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-12 11:10:24.000000 metaseg-0.6.0/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 15:06:21.600587 metaseg-0.6.0/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2953 2023-04-12 11:10:24.000000 metaseg-0.6.0/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.590587 metaseg-0.6.0/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      631 2023-04-12 15:05:56.000000 metaseg-0.6.0/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.593920 metaseg-0.6.0/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6198 2023-04-12 12:18:37.000000 metaseg-0.6.0/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.597253 metaseg-0.6.0/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3515 2023-04-12 14:10:32.000000 metaseg-0.6.0/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.600587 metaseg-0.6.0/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.600587 metaseg-0.6.0/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.6.0/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8416 2023-04-12 15:06:15.000000 metaseg-0.6.0/metaseg/webapp/app.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2470 2023-04-12 15:06:16.000000 metaseg-0.6.0/metaseg/webapp/demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 15:06:21.590587 metaseg-0.6.0/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 15:06:21.000000 metaseg-0.6.0/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      881 2023-04-12 15:06:21.000000 metaseg-0.6.0/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-12 15:06:21.000000 metaseg-0.6.0/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      230 2023-04-12 15:06:21.000000 metaseg-0.6.0/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-12 15:06:21.000000 metaseg-0.6.0/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-12 11:10:24.000000 metaseg-0.6.0/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      143 2023-04-12 13:57:00.000000 metaseg-0.6.0/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-12 15:06:21.600587 metaseg-0.6.0/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-12 11:10:24.000000 metaseg-0.6.0/setup.py
```

### Comparing `metaseg-0.5.8/LICENSE` & `metaseg-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/PKG-INFO` & `metaseg-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.5.8
+Version: 0.6.0
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.5.8 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.6.0 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.5.8/README.md` & `metaseg-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/__init__.py` & `metaseg-0.6.0/metaseg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
-__version__ = "0.5.8"
+__version__ = "0.6.0"
```

### Comparing `metaseg-0.5.8/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.6.0/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/generator/build_sam.py` & `metaseg-0.6.0/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/generator/predictor.py` & `metaseg-0.6.0/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/mask_predictor.py` & `metaseg-0.6.0/metaseg/mask_predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/modeling/common.py` & `metaseg-0.6.0/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/modeling/image_encoder.py` & `metaseg-0.6.0/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/modeling/mask_decoder.py` & `metaseg-0.6.0/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/modeling/prompt_encoder.py` & `metaseg-0.6.0/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/modeling/sam.py` & `metaseg-0.6.0/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/modeling/transformer.py` & `metaseg-0.6.0/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/sahi_predict.py` & `metaseg-0.6.0/metaseg/sahi_predict.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/utils/amg.py` & `metaseg-0.6.0/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/utils/data_utils.py` & `metaseg-0.6.0/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/utils/file_utils.py` & `metaseg-0.6.0/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/utils/onnx.py` & `metaseg-0.6.0/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/utils/transforms.py` & `metaseg-0.6.0/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/metaseg/webapp/app.py` & `metaseg-0.6.0/metaseg/webapp/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import gradio as gr
-from demo import automask_image_app, automask_video_app, manual_app, sahi_autoseg_app
+from demo import automask_image_app, automask_video_app, sahi_autoseg_app
 
 
 def image_app():
     with gr.Blocks():
         with gr.Row():
             with gr.Column():
                 seg_automask_image_file = gr.Image(type="filepath").style(height=260)
-
                 with gr.Row():
                     with gr.Column():
                         seg_automask_image_model_type = gr.Dropdown(
                             choices=[
                                 "vit_h",
                                 "vit_l",
                                 "vit_b",
                             ],
                             value="vit_l",
                             label="Model Type",
                         )
 
-                        seg_automask_image_points_per_side = gr.Slider(
-                            minimum=0,
-                            maximum=32,
-                            step=2,
-                            value=16,
-                            label="Points per Side",
-                        )
-
-                        seg_automask_image_points_per_batch = gr.Slider(
-                            minimum=0,
-                            maximum=64,
-                            step=2,
-                            value=64,
-                            label="Points per Batch",
-                        )
-
                         seg_automask_image_min_area = gr.Number(
                             value=0,
                             label="Min Area",
                         )
+                    with gr.Row():
+                        with gr.Column():
+                            seg_automask_image_points_per_side = gr.Slider(
+                                minimum=0,
+                                maximum=32,
+                                step=2,
+                                value=16,
+                                label="Points per Side",
+                            )
+
+                            seg_automask_image_points_per_batch = gr.Slider(
+                                minimum=0,
+                                maximum=64,
+                                step=2,
+                                value=64,
+                                label="Points per Batch",
+                            )
 
                 seg_automask_image_predict = gr.Button(value="Generator")
 
             with gr.Column():
                 output_image = gr.Image()
 
         seg_automask_image_predict.click(
@@ -60,47 +60,47 @@
 
 
 def video_app():
     with gr.Blocks():
         with gr.Row():
             with gr.Column():
                 seg_automask_video_file = gr.Video().style(height=260)
-
                 with gr.Row():
                     with gr.Column():
                         seg_automask_video_model_type = gr.Dropdown(
                             choices=[
                                 "vit_h",
                                 "vit_l",
                                 "vit_b",
                             ],
                             value="vit_l",
                             label="Model Type",
                         )
-
-                        seg_automask_video_points_per_side = gr.Slider(
-                            minimum=0,
-                            maximum=32,
-                            step=2,
-                            value=16,
-                            label="Points per Side",
+                        seg_automask_video_min_area = gr.Number(
+                            value=1000,
+                            label="Min Area",
                         )
-                        seg_automask_video_points_per_batch = gr.Slider(
-                            minimum=0,
-                            maximum=64,
-                            step=2,
-                            value=64,
-                            label="Points per Batch",
-                        )
-                        with gr.Row():
-                            with gr.Column():
-                                seg_automask_video_min_area = gr.Number(
-                                    value=1000,
-                                    label="Min Area",
-                                )
+
+                    with gr.Row():
+                        with gr.Column():
+                            seg_automask_video_points_per_side = gr.Slider(
+                                minimum=0,
+                                maximum=32,
+                                step=2,
+                                value=16,
+                                label="Points per Side",
+                            )
+
+                            seg_automask_video_points_per_batch = gr.Slider(
+                                minimum=0,
+                                maximum=64,
+                                step=2,
+                                value=64,
+                                label="Points per Batch",
+                            )
 
                 seg_automask_video_predict = gr.Button(value="Generator")
             with gr.Column():
                 output_video = gr.Video()
 
         seg_automask_video_predict.click(
             fn=automask_video_app,
@@ -116,86 +116,87 @@
 
 
 def sahi_app():
     with gr.Blocks():
         with gr.Row():
             with gr.Column():
                 sahi_image_file = gr.Image(type="filepath").style(height=260)
+                sahi_autoseg_model_type = gr.Dropdown(
+                    choices=[
+                        "vit_h",
+                        "vit_l",
+                        "vit_b",
+                    ],
+                    value="vit_l",
+                    label="Sam Model Type",
+                )
+
                 with gr.Row():
                     with gr.Column():
-                        sahi_autoseg_model_type = gr.Dropdown(
+                        sahi_model_type = gr.Dropdown(
                             choices=[
-                                "vit_h",
-                                "vit_l",
-                                "vit_b",
+                                "yolov5",
+                                "yolov8",
                             ],
-                            value="vit_l",
-                            label="Sam Model Type",
+                            value="yolov5",
+                            label="Detector Model Type",
                         )
                         sahi_image_size = gr.Slider(
                             minimum=0,
                             maximum=1600,
                             step=32,
                             value=640,
                             label="Image Size",
                         )
-                        sahi_conf_th = gr.Slider(
+
+                        sahi_overlap_width = gr.Slider(
                             minimum=0,
                             maximum=1,
                             step=0.1,
                             value=0.2,
-                            label="Confidence Threshold",
+                            label="Overlap Width",
                         )
+
                         sahi_slice_width = gr.Slider(
                             minimum=0,
                             maximum=640,
                             step=32,
                             value=256,
                             label="Slice Width",
                         )
 
-                        sahi_overlap_height = gr.Slider(
-                            minimum=0,
-                            maximum=1,
-                            step=0.1,
-                            value=0.2,
-                            label="Overlap Height",
-                        )
                     with gr.Row():
                         with gr.Column():
-                            sahi_model_type = gr.Dropdown(
-                                choices=[
-                                    "yolov5",
-                                    "yolov8",
-                                ],
-                                value="yolov5",
-                                label="Detector Model Type",
-                            )
-
                             sahi_model_path = gr.Dropdown(
                                 choices=["yolov5l.pt", "yolov5l6.pt", "yolov8l.pt", "yolov8x.pt"],
-                                value="yolov5m",
+                                value="yolov5l6.pt",
                                 label="Detector Model Path",
                             )
-                            sahi_slice_height = gr.Slider(
+
+                            sahi_conf_th = gr.Slider(
                                 minimum=0,
-                                maximum=640,
-                                step=32,
-                                value=256,
-                                label="Slice Height",
+                                maximum=1,
+                                step=0.1,
+                                value=0.2,
+                                label="Confidence Threshold",
                             )
-
-                            sahi_overlap_width = gr.Slider(
+                            sahi_overlap_height = gr.Slider(
                                 minimum=0,
                                 maximum=1,
                                 step=0.1,
                                 value=0.2,
-                                label="Overlap Width",
+                                label="Overlap Height",
+                            )
+                            sahi_slice_height = gr.Slider(
+                                minimum=0,
+                                maximum=640,
+                                step=32,
+                                value=256,
+                                label="Slice Height",
                             )
-
                 sahi_image_predict = gr.Button(value="Generator")
 
             with gr.Column():
                 output_image = gr.Image()
 
         sahi_image_predict.click(
             fn=sahi_autoseg_app,
@@ -214,24 +215,14 @@
             outputs=[output_image],
         )
 
 
 def metaseg_app():
     app = gr.Blocks()
     with app:
-        gr.Markdown("# **<h2 align='center'>Segment Anything + Video + SAHI</h2>**")
-        gr.Markdown(
-            """
-            <h5 style='text-align: center'>
-            Follow me for more! 
-            <a href='https://twitter.com/kadirnar_ai' target='_blank'>Twitter</a> | <a href='https://github.com/kadirnar' target='_blank'>Github</a> | <a href='https://www.linkedin.com/in/kadir-nar/' target='_blank'>Linkedin</a> |
-            </h5>
-            """
-        )
-
         with gr.Row():
             with gr.Column():
                 with gr.Tab("Image"):
                     image_app()
                 with gr.Tab("Video"):
                     video_app()
                 with gr.Tab("SAHI"):
```

### Comparing `metaseg-0.5.8/metaseg/webapp/demo.py` & `metaseg-0.6.0/metaseg/webapp/demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     SegAutoMaskPredictor().video_predict(
         source=video_path,
         model_type=model_type,  # vit_l, vit_h, vit_b
         points_per_side=points_per_side,
         points_per_batch=points_per_batch,
         min_area=min_area,
         output_path="output.mp4",
-        save=True,
     )
     return "output.mp4"
 
 
 # For manuel box and point selection
```

### Comparing `metaseg-0.5.8/metaseg.egg-info/PKG-INFO` & `metaseg-0.6.0/metaseg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.5.8
+Version: 0.6.0
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.5.8 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.6.0 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.5.8/metaseg.egg-info/SOURCES.txt` & `metaseg-0.6.0/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.8/setup.py` & `metaseg-0.6.0/setup.py`

 * *Files identical despite different names*

