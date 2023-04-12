# Comparing `tmp/metaseg-0.5.6.tar.gz` & `tmp/metaseg-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.5.6.tar", last modified: Wed Apr 12 13:57:15 2023, max compression
+gzip compressed data, was "metaseg-0.5.8.tar", last modified: Wed Apr 12 14:11:06 2023, max compression
```

## Comparing `metaseg-0.5.6.tar` & `metaseg-0.5.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:57:15.160365 metaseg-0.5.6/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-12 11:10:24.000000 metaseg-0.5.6/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-12 11:10:24.000000 metaseg-0.5.6/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 13:57:15.160365 metaseg-0.5.6/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2953 2023-04-12 11:10:24.000000 metaseg-0.5.6/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:57:15.150365 metaseg-0.5.6/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      631 2023-04-12 13:57:12.000000 metaseg-0.5.6/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:57:15.153698 metaseg-0.5.6/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6198 2023-04-12 12:18:37.000000 metaseg-0.5.6/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:57:15.153698 metaseg-0.5.6/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3342 2023-04-12 13:56:45.000000 metaseg-0.5.6/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:57:15.157031 metaseg-0.5.6/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:57:15.160365 metaseg-0.5.6/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.6/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8827 2023-04-12 13:37:18.000000 metaseg-0.5.6/metaseg/webapp/app.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2489 2023-04-12 13:42:49.000000 metaseg-0.5.6/metaseg/webapp/demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:57:15.150365 metaseg-0.5.6/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 13:57:15.000000 metaseg-0.5.6/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      881 2023-04-12 13:57:15.000000 metaseg-0.5.6/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-12 13:57:15.000000 metaseg-0.5.6/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      230 2023-04-12 13:57:15.000000 metaseg-0.5.6/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-12 13:57:15.000000 metaseg-0.5.6/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-12 11:10:24.000000 metaseg-0.5.6/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      143 2023-04-12 13:57:00.000000 metaseg-0.5.6/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-12 13:57:15.160365 metaseg-0.5.6/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-12 11:10:24.000000 metaseg-0.5.6/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.720409 metaseg-0.5.8/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-12 11:10:24.000000 metaseg-0.5.8/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-12 11:10:24.000000 metaseg-0.5.8/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 14:11:06.723743 metaseg-0.5.8/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2953 2023-04-12 11:10:24.000000 metaseg-0.5.8/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.710409 metaseg-0.5.8/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      631 2023-04-12 14:10:44.000000 metaseg-0.5.8/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.713743 metaseg-0.5.8/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6198 2023-04-12 12:18:37.000000 metaseg-0.5.8/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.717076 metaseg-0.5.8/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3515 2023-04-12 14:10:32.000000 metaseg-0.5.8/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.720409 metaseg-0.5.8/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.720409 metaseg-0.5.8/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.8/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8827 2023-04-12 13:37:18.000000 metaseg-0.5.8/metaseg/webapp/app.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2489 2023-04-12 13:42:49.000000 metaseg-0.5.8/metaseg/webapp/demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 14:11:06.713743 metaseg-0.5.8/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 14:11:06.000000 metaseg-0.5.8/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      881 2023-04-12 14:11:06.000000 metaseg-0.5.8/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-12 14:11:06.000000 metaseg-0.5.8/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      230 2023-04-12 14:11:06.000000 metaseg-0.5.8/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-12 14:11:06.000000 metaseg-0.5.8/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-12 11:10:24.000000 metaseg-0.5.8/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      143 2023-04-12 13:57:00.000000 metaseg-0.5.8/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-12 14:11:06.723743 metaseg-0.5.8/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-12 11:10:24.000000 metaseg-0.5.8/setup.py
```

### Comparing `metaseg-0.5.6/LICENSE` & `metaseg-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/PKG-INFO` & `metaseg-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.5.6
+Version: 0.5.8
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
-Metadata-Version: 2.1 Name: metaseg Version: 0.5.6 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.5.8 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.5.6/README.md` & `metaseg-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/__init__.py` & `metaseg-0.5.8/metaseg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
-__version__ = "0.5.6"
+__version__ = "0.5.8"
```

### Comparing `metaseg-0.5.6/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.5.8/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/generator/build_sam.py` & `metaseg-0.5.8/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/generator/predictor.py` & `metaseg-0.5.8/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/mask_predictor.py` & `metaseg-0.5.8/metaseg/mask_predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/modeling/common.py` & `metaseg-0.5.8/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/modeling/image_encoder.py` & `metaseg-0.5.8/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/modeling/mask_decoder.py` & `metaseg-0.5.8/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/modeling/prompt_encoder.py` & `metaseg-0.5.8/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/modeling/sam.py` & `metaseg-0.5.8/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/modeling/transformer.py` & `metaseg-0.5.8/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/sahi_predict.py` & `metaseg-0.5.8/metaseg/sahi_predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
-import cv2
+from PIL import Image
+
 from metaseg import SamPredictor, sam_model_registry
 from metaseg.utils import download_model, load_image, multi_boxes, plt_load_box, plt_load_mask
 
 
 def sahi_sliced_predict(
     image_path,
     detection_model_type,
@@ -106,12 +108,15 @@
         plt.imshow(read_image)
         for mask in masks:
             plt_load_mask(mask.cpu().numpy(), plt.gca(), random_color=random_color)
         for box in input_boxes:
             plt_load_box(box.cpu().numpy(), plt.gca())
         plt.axis("off")
         if save:
-            cv2.imwrite("output.png", read_image)
+            plt.savefig("output.png", bbox_inches="tight")
+            output_image = cv2.imread("output.png")
+            output_image = Image.fromarray(output_image)
+            return output_image
         if show:
             plt.show()
 
         return masks
```

### Comparing `metaseg-0.5.6/metaseg/utils/amg.py` & `metaseg-0.5.8/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/utils/data_utils.py` & `metaseg-0.5.8/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/utils/file_utils.py` & `metaseg-0.5.8/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/utils/onnx.py` & `metaseg-0.5.8/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/utils/transforms.py` & `metaseg-0.5.8/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/webapp/app.py` & `metaseg-0.5.8/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg/webapp/demo.py` & `metaseg-0.5.8/metaseg/webapp/demo.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/metaseg.egg-info/PKG-INFO` & `metaseg-0.5.8/metaseg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.5.6
+Version: 0.5.8
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
-Metadata-Version: 2.1 Name: metaseg Version: 0.5.6 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.5.8 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.5.6/metaseg.egg-info/SOURCES.txt` & `metaseg-0.5.8/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.6/setup.py` & `metaseg-0.5.8/setup.py`

 * *Files identical despite different names*

