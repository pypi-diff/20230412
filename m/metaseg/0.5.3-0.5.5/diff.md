# Comparing `tmp/metaseg-0.5.3.tar.gz` & `tmp/metaseg-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.5.3.tar", last modified: Wed Apr 12 12:18:59 2023, max compression
+gzip compressed data, was "metaseg-0.5.5.tar", last modified: Wed Apr 12 13:43:19 2023, max compression
```

## Comparing `metaseg-0.5.3.tar` & `metaseg-0.5.5.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.990048 metaseg-0.5.3/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-12 11:10:24.000000 metaseg-0.5.3/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-12 11:10:24.000000 metaseg-0.5.3/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 12:18:59.990048 metaseg-0.5.3/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2953 2023-04-12 11:10:24.000000 metaseg-0.5.3/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.983381 metaseg-0.5.3/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      631 2023-04-12 12:18:48.000000 metaseg-0.5.3/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.986714 metaseg-0.5.3/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6198 2023-04-12 12:18:37.000000 metaseg-0.5.3/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.986714 metaseg-0.5.3/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3320 2023-04-12 11:34:58.000000 metaseg-0.5.3/metaseg/sahi_predict.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.986714 metaseg-0.5.3/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.986714 metaseg-0.5.3/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-12 11:10:24.000000 metaseg-0.5.3/metaseg/webapp/app.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 12:18:59.983381 metaseg-0.5.3/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 12:18:59.000000 metaseg-0.5.3/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      858 2023-04-12 12:18:59.000000 metaseg-0.5.3/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-12 12:18:59.000000 metaseg-0.5.3/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      231 2023-04-12 12:18:59.000000 metaseg-0.5.3/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-12 12:18:59.000000 metaseg-0.5.3/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-12 11:10:24.000000 metaseg-0.5.3/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      144 2023-04-12 11:10:24.000000 metaseg-0.5.3/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-12 12:18:59.990048 metaseg-0.5.3/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-12 11:10:24.000000 metaseg-0.5.3/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:43:19.366986 metaseg-0.5.5/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-12 11:10:24.000000 metaseg-0.5.5/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-12 11:10:24.000000 metaseg-0.5.5/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 13:43:19.370320 metaseg-0.5.5/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2953 2023-04-12 11:10:24.000000 metaseg-0.5.5/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:43:19.356986 metaseg-0.5.5/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      631 2023-04-12 13:40:03.000000 metaseg-0.5.5/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:43:19.360320 metaseg-0.5.5/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6198 2023-04-12 12:18:37.000000 metaseg-0.5.5/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:43:19.363653 metaseg-0.5.5/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3320 2023-04-12 11:34:58.000000 metaseg-0.5.5/metaseg/sahi_predict.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:43:19.366986 metaseg-0.5.5/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      276 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2327 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:43:19.366986 metaseg-0.5.5/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-12 11:10:24.000000 metaseg-0.5.5/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8827 2023-04-12 13:37:18.000000 metaseg-0.5.5/metaseg/webapp/app.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2489 2023-04-12 13:42:49.000000 metaseg-0.5.5/metaseg/webapp/demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-12 13:43:19.360320 metaseg-0.5.5/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3227 2023-04-12 13:43:19.000000 metaseg-0.5.5/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      881 2023-04-12 13:43:19.000000 metaseg-0.5.5/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-12 13:43:19.000000 metaseg-0.5.5/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      231 2023-04-12 13:43:19.000000 metaseg-0.5.5/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-12 13:43:19.000000 metaseg-0.5.5/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-12 11:10:24.000000 metaseg-0.5.5/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      144 2023-04-12 11:10:24.000000 metaseg-0.5.5/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-12 13:43:19.370320 metaseg-0.5.5/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-12 11:10:24.000000 metaseg-0.5.5/setup.py
```

### Comparing `metaseg-0.5.3/LICENSE` & `metaseg-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/PKG-INFO` & `metaseg-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.5.3
+Version: 0.5.5
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
-Metadata-Version: 2.1 Name: metaseg Version: 0.5.3 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.5.5 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.5.3/README.md` & `metaseg-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/__init__.py` & `metaseg-0.5.5/metaseg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
-__version__ = "0.5.3"
+__version__ = "0.5.5"
```

### Comparing `metaseg-0.5.3/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.5.5/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/generator/build_sam.py` & `metaseg-0.5.5/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/generator/predictor.py` & `metaseg-0.5.5/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/mask_predictor.py` & `metaseg-0.5.5/metaseg/mask_predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/modeling/common.py` & `metaseg-0.5.5/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/modeling/image_encoder.py` & `metaseg-0.5.5/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/modeling/mask_decoder.py` & `metaseg-0.5.5/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/modeling/prompt_encoder.py` & `metaseg-0.5.5/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/modeling/sam.py` & `metaseg-0.5.5/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/modeling/transformer.py` & `metaseg-0.5.5/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/sahi_predict.py` & `metaseg-0.5.5/metaseg/sahi_predict.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/utils/amg.py` & `metaseg-0.5.5/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/utils/data_utils.py` & `metaseg-0.5.5/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/utils/file_utils.py` & `metaseg-0.5.5/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/utils/onnx.py` & `metaseg-0.5.5/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg/utils/transforms.py` & `metaseg-0.5.5/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.5.3/metaseg.egg-info/PKG-INFO` & `metaseg-0.5.5/metaseg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.5.3
+Version: 0.5.5
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
-Metadata-Version: 2.1 Name: metaseg Version: 0.5.3 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.5.5 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.5.3/metaseg.egg-info/SOURCES.txt` & `metaseg-0.5.5/metaseg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,8 +27,9 @@
 metaseg/utils/__init__.py
 metaseg/utils/amg.py
 metaseg/utils/data_utils.py
 metaseg/utils/file_utils.py
 metaseg/utils/onnx.py
 metaseg/utils/transforms.py
 metaseg/webapp/__init__.py
-metaseg/webapp/app.py
+metaseg/webapp/app.py
+metaseg/webapp/demo.py
```

### Comparing `metaseg-0.5.3/setup.py` & `metaseg-0.5.5/setup.py`

 * *Files identical despite different names*

