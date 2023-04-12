# Comparing `tmp/metaseg-0.5.0.tar.gz` & `tmp/metaseg-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.5.0.tar", last modified: Tue Apr 11 22:23:13 2023, max compression
+gzip compressed data, was "metaseg-0.5.1.tar", last modified: Wed Apr 12 11:20:39 2023, max compression
```

## Comparing `metaseg-0.5.0.tar` & `metaseg-0.5.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.637373 metaseg-0.5.0/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.5.0/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.5.0/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-11 22:23:13.637373 metaseg-0.5.0/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2953 2023-04-11 22:22:18.000000 metaseg-0.5.0/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.630706 metaseg-0.5.0/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-11 22:22:31.000000 metaseg-0.5.0/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.634040 metaseg-0.5.0/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6236 2023-04-11 22:22:49.000000 metaseg-0.5.0/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.634040 metaseg-0.5.0/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.5.0/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.5.0/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.5.0/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.5.0/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.5.0/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.5.0/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.5.0/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3297 2023-04-11 22:22:49.000000 metaseg-0.5.0/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.637373 metaseg-0.5.0/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-11 18:48:27.000000 metaseg-0.5.0/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.5.0/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-11 22:22:49.000000 metaseg-0.5.0/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.5.0/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.5.0/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.637373 metaseg-0.5.0/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-10 18:01:14.000000 metaseg-0.5.0/metaseg/webapp/app.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-11 22:23:13.630706 metaseg-0.5.0/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-11 22:23:13.000000 metaseg-0.5.0/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-11 22:23:13.000000 metaseg-0.5.0/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-11 22:23:13.000000 metaseg-0.5.0/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      231 2023-04-11 22:23:13.000000 metaseg-0.5.0/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-11 22:23:13.000000 metaseg-0.5.0/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.5.0/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      144 2023-04-10 19:54:00.000000 metaseg-0.5.0/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-11 22:23:13.637373 metaseg-0.5.0/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.5.0/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:20:39.103193 metaseg-0.5.1/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-12 11:10:24.000000 metaseg-0.5.1/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-12 11:10:24.000000 metaseg-0.5.1/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 11:20:39.103193 metaseg-0.5.1/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2953 2023-04-12 11:10:24.000000 metaseg-0.5.1/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:20:39.096526 metaseg-0.5.1/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      631 2023-04-12 11:17:11.000000 metaseg-0.5.1/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:20:39.099860 metaseg-0.5.1/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6182 2023-04-12 11:11:25.000000 metaseg-0.5.1/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:20:39.099860 metaseg-0.5.1/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3319 2023-04-12 11:19:56.000000 metaseg-0.5.1/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:20:39.103193 metaseg-0.5.1/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:20:39.103193 metaseg-0.5.1/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-12 11:10:24.000000 metaseg-0.5.1/metaseg/webapp/app.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:20:39.099860 metaseg-0.5.1/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 11:20:39.000000 metaseg-0.5.1/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-12 11:20:39.000000 metaseg-0.5.1/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-12 11:20:39.000000 metaseg-0.5.1/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      231 2023-04-12 11:20:39.000000 metaseg-0.5.1/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-12 11:20:39.000000 metaseg-0.5.1/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-12 11:10:24.000000 metaseg-0.5.1/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      144 2023-04-12 11:10:24.000000 metaseg-0.5.1/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-12 11:20:39.103193 metaseg-0.5.1/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-12 11:10:24.000000 metaseg-0.5.1/setup.py
```

### Comparing `metaseg-0.5.0/LICENSE` & `metaseg-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/PKG-INFO` & `metaseg-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.5.0
+Version: 0.5.1
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
-Metadata-Version: 2.1 Name: metaseg Version: 0.5.0 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.5.1 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.5.0/README.md` & `metaseg-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.5.1/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/generator/build_sam.py` & `metaseg-0.5.1/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/generator/predictor.py` & `metaseg-0.5.1/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/mask_predictor.py` & `metaseg-0.5.1/metaseg/mask_predictor.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         source,
         model_type,
         points_per_side,
         points_per_batch,
         min_area,
         output_path="output.png",
         show=False,
-        save=False,
+        save=True,
     ):
         read_image = load_image(source)
         model = self.load_model(model_type)
         mask_generator = SamAutomaticMaskGenerator(
             model, points_per_side=points_per_side, points_per_batch=points_per_batch, min_mask_region_area=min_area
         )
 
@@ -120,16 +120,14 @@
         return output_path
 
 
 class SegManualMaskPredictor:
     def __init__(self):
         self.model = None
         self.device = "cuda" if torch.cuda.is_available() else "cpu"
-        self.save = False
-        self.show = False
 
     def load_model(self, model_type):
         if self.model is None:
             self.model_path = download_model(model_type)
             self.model = sam_model_registry[model_type](checkpoint=self.model_path)
             self.model.to(device=self.device)
 
@@ -142,15 +140,15 @@
         input_box=None,
         input_point=None,
         input_label=None,
         multimask_output=False,
         output_path="output.png",
         random_color=False,
         show=False,
-        save=False,
+        save=True,
     ):
         image = load_image(source)
         model = self.load_model(model_type)
         predictor = SamPredictor(model)
         predictor.set_image(image)
 
         if type(input_box[0]) == list:
```

### Comparing `metaseg-0.5.0/metaseg/modeling/common.py` & `metaseg-0.5.1/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/modeling/image_encoder.py` & `metaseg-0.5.1/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/modeling/mask_decoder.py` & `metaseg-0.5.1/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/modeling/prompt_encoder.py` & `metaseg-0.5.1/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/modeling/sam.py` & `metaseg-0.5.1/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/modeling/transformer.py` & `metaseg-0.5.1/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/sahi_predict.py` & `metaseg-0.5.1/metaseg/sahi_predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,16 @@
         source,
         model_type,
         input_box=None,
         input_point=None,
         input_label=None,
         multimask_output=False,
         random_color=False,
-        save=False,
-        show=True,
+        show=False,
+        save=True,
     ):
 
         read_image = load_image(source)
         model = self.load_model(model_type)
         predictor = SamPredictor(model)
         predictor.set_image(read_image)
 
@@ -109,7 +109,9 @@
         for box in input_boxes:
             plt_load_box(box.cpu().numpy(), plt.gca())
         plt.axis("off")
         if save:
             plt.savefig("output.png")
         if show:
             plt.show()
+
+        return masks
```

### Comparing `metaseg-0.5.0/metaseg/utils/amg.py` & `metaseg-0.5.1/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/utils/data_utils.py` & `metaseg-0.5.1/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/utils/file_utils.py` & `metaseg-0.5.1/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/utils/onnx.py` & `metaseg-0.5.1/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/utils/transforms.py` & `metaseg-0.5.1/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg/webapp/app.py` & `metaseg-0.5.1/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/metaseg.egg-info/PKG-INFO` & `metaseg-0.5.1/metaseg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.5.0
+Version: 0.5.1
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
-Metadata-Version: 2.1 Name: metaseg Version: 0.5.0 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.5.1 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.5.0/metaseg.egg-info/SOURCES.txt` & `metaseg-0.5.1/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.0/setup.py` & `metaseg-0.5.1/setup.py`

 * *Files identical despite different names*

