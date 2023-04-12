# Comparing `tmp/metaseg-0.5.2.tar.gz` & `tmp/metaseg-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.5.2.tar", last modified: Wed Apr 12 11:35:03 2023, max compression
+gzip compressed data, was "metaseg-0.5.3.tar", last modified: Wed Apr 12 12:18:59 2023, max compression
```

## Comparing `metaseg-0.5.2.tar` & `metaseg-0.5.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:35:03.219906 metaseg-0.5.2/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-12 11:10:24.000000 metaseg-0.5.2/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-12 11:10:24.000000 metaseg-0.5.2/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 11:35:03.219906 metaseg-0.5.2/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2953 2023-04-12 11:10:24.000000 metaseg-0.5.2/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:35:03.209906 metaseg-0.5.2/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      631 2023-04-12 11:34:58.000000 metaseg-0.5.2/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:35:03.209906 metaseg-0.5.2/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6184 2023-04-12 11:34:58.000000 metaseg-0.5.2/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:35:03.213239 metaseg-0.5.2/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3320 2023-04-12 11:34:58.000000 metaseg-0.5.2/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:35:03.216572 metaseg-0.5.2/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:35:03.219906 metaseg-0.5.2/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-12 11:10:24.000000 metaseg-0.5.2/metaseg/webapp/app.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:35:03.209906 metaseg-0.5.2/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 11:35:03.000000 metaseg-0.5.2/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-12 11:35:03.000000 metaseg-0.5.2/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-12 11:35:03.000000 metaseg-0.5.2/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      231 2023-04-12 11:35:03.000000 metaseg-0.5.2/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-12 11:35:03.000000 metaseg-0.5.2/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-12 11:10:24.000000 metaseg-0.5.2/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      144 2023-04-12 11:10:24.000000 metaseg-0.5.2/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-12 11:35:03.219906 metaseg-0.5.2/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-12 11:10:24.000000 metaseg-0.5.2/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.990048 metaseg-0.5.3/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-12 11:10:24.000000 metaseg-0.5.3/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-12 11:10:24.000000 metaseg-0.5.3/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 12:18:59.990048 metaseg-0.5.3/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2953 2023-04-12 11:10:24.000000 metaseg-0.5.3/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.983381 metaseg-0.5.3/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      631 2023-04-12 12:18:48.000000 metaseg-0.5.3/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.986714 metaseg-0.5.3/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6198 2023-04-12 12:18:37.000000 metaseg-0.5.3/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.986714 metaseg-0.5.3/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3320 2023-04-12 11:34:58.000000 metaseg-0.5.3/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.986714 metaseg-0.5.3/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.986714 metaseg-0.5.3/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/webapp/app.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.983381 metaseg-0.5.3/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 12:18:59.000000 metaseg-0.5.3/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-12 12:18:59.000000 metaseg-0.5.3/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-12 12:18:59.000000 metaseg-0.5.3/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      231 2023-04-12 12:18:59.000000 metaseg-0.5.3/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-12 12:18:59.000000 metaseg-0.5.3/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-12 11:10:24.000000 metaseg-0.5.3/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      144 2023-04-12 11:10:24.000000 metaseg-0.5.3/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-12 12:18:59.990048 metaseg-0.5.3/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-12 11:10:24.000000 metaseg-0.5.3/setup.py
```

### Comparing `metaseg-0.5.2/LICENSE` & `metaseg-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/PKG-INFO` & `metaseg-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.5.2
+Version: 0.5.3
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
-Metadata-Version: 2.1 Name: metaseg Version: 0.5.2 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.5.3 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.5.2/README.md` & `metaseg-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/__init__.py` & `metaseg-0.5.3/metaseg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
```

### Comparing `metaseg-0.5.2/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.5.3/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/generator/build_sam.py` & `metaseg-0.5.3/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/generator/predictor.py` & `metaseg-0.5.3/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/mask_predictor.py` & `metaseg-0.5.3/metaseg/mask_predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
         combined_mask = cv2.add(read_image, mask_image)
         self.combined_mask = combined_mask
         if show:
             show_image(combined_mask)
 
         if save:
-            save_image(output_path=output_path, image=combined_mask)
+            save_image(output_path=output_path, output_image=combined_mask)
 
         return masks
 
     def video_predict(self, source, model_type, points_per_side, points_per_batch, min_area, output_path="output.mp4"):
         cap, out = load_video(source, output_path)
         length = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
         colors = np.random.randint(0, 255, size=(256, 3), dtype=np.uint8)
@@ -176,13 +176,13 @@
                 multimask_output=multimask_output,
             )
             mask_image = load_mask(masks, random_color)
             image = load_box(input_box, image)
 
         combined_mask = cv2.add(image, mask_image)
         if save:
-            save_image(output_path=output_path, image=combined_mask)
+            save_image(output_path=output_path, output_image=combined_mask)
 
         if show:
             show_image(combined_mask)
 
         return masks
```

### Comparing `metaseg-0.5.2/metaseg/modeling/common.py` & `metaseg-0.5.3/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/modeling/image_encoder.py` & `metaseg-0.5.3/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/modeling/mask_decoder.py` & `metaseg-0.5.3/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/modeling/prompt_encoder.py` & `metaseg-0.5.3/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/modeling/sam.py` & `metaseg-0.5.3/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/modeling/transformer.py` & `metaseg-0.5.3/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/sahi_predict.py` & `metaseg-0.5.3/metaseg/sahi_predict.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/utils/amg.py` & `metaseg-0.5.3/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/utils/data_utils.py` & `metaseg-0.5.3/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/utils/file_utils.py` & `metaseg-0.5.3/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/utils/onnx.py` & `metaseg-0.5.3/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/utils/transforms.py` & `metaseg-0.5.3/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg/webapp/app.py` & `metaseg-0.5.3/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/metaseg.egg-info/PKG-INFO` & `metaseg-0.5.3/metaseg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.5.2
+Version: 0.5.3
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
-Metadata-Version: 2.1 Name: metaseg Version: 0.5.2 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.5.3 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.5.2/metaseg.egg-info/SOURCES.txt` & `metaseg-0.5.3/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.2/setup.py` & `metaseg-0.5.3/setup.py`

 * *Files identical despite different names*

