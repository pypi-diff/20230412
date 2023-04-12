# Comparing `tmp/clipcrop-2.1.tar.gz` & `tmp/clipcrop-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcrop-2.1.tar", last modified: Wed Apr 12 11:22:44 2023, max compression
+gzip compressed data, was "clipcrop-2.2.tar", last modified: Wed Apr 12 11:26:52 2023, max compression
```

## Comparing `clipcrop-2.1.tar` & `clipcrop-2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:22:44.709785 clipcrop-2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 11:22:32.000000 clipcrop-2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-12 11:22:44.709785 clipcrop-2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-12 11:22:32.000000 clipcrop-2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:22:44.709785 clipcrop-2.1/clipcrop/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:22:32.000000 clipcrop-2.1/clipcrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-04-12 11:22:32.000000 clipcrop-2.1/clipcrop/clipcrop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:22:44.709785 clipcrop-2.1/clipcrop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-12 11:22:44.000000 clipcrop-2.1/clipcrop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 11:22:44.000000 clipcrop-2.1/clipcrop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:22:44.000000 clipcrop-2.1/clipcrop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:22:44.000000 clipcrop-2.1/clipcrop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 11:22:44.000000 clipcrop-2.1/clipcrop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 11:22:44.000000 clipcrop-2.1/clipcrop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 11:22:44.709785 clipcrop-2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-12 11:22:33.000000 clipcrop-2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:26:52.960560 clipcrop-2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 11:26:44.000000 clipcrop-2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-12 11:26:52.960560 clipcrop-2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-12 11:26:44.000000 clipcrop-2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:26:52.960560 clipcrop-2.2/clipcrop/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:26:44.000000 clipcrop-2.2/clipcrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-04-12 11:26:44.000000 clipcrop-2.2/clipcrop/clipcrop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:26:52.960560 clipcrop-2.2/clipcrop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-12 11:26:52.000000 clipcrop-2.2/clipcrop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 11:26:52.000000 clipcrop-2.2/clipcrop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:26:52.000000 clipcrop-2.2/clipcrop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:26:52.000000 clipcrop-2.2/clipcrop.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 11:26:52.000000 clipcrop-2.2/clipcrop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 11:26:52.000000 clipcrop-2.2/clipcrop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 11:26:52.960560 clipcrop-2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-12 11:26:44.000000 clipcrop-2.2/setup.py
```

### Comparing `clipcrop-2.1/LICENSE` & `clipcrop-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clipcrop-2.1/PKG-INFO` & `clipcrop-2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 2.1
+Version: 2.2
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clipcrop-2.1/README.md` & `clipcrop-2.2/README.md`

 * *Files identical despite different names*

### Comparing `clipcrop-2.1/clipcrop/clipcrop.py` & `clipcrop-2.2/clipcrop/clipcrop.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,16 @@
       
       xmin = int(j[0])
       ymin = int(j[1])
       xmax = int(j[2])
       ymax = int(j[3])
 
       roi = image[ymin:ymax, xmin:xmax]
-      roi_im = Image.fromarray(roi)
-      images_list.append(roi_im[:,:,::-1])
+      roi_im = Image.fromarray(roi[:,:,::-1])
+      images_list.append(roi_im)
 
     inputs = self.CLIPP(text = [self.text], images=images_list , return_tensors="pt", padding=True)
     outputs = self.CLIPM(**inputs)
     logits_per_image = outputs.logits_per_text
     probs = logits_per_image.softmax(-1)
     l_idx = np.argsort(probs[-1].detach().numpy())[::-1][0:self.num]
```

### Comparing `clipcrop-2.1/clipcrop.egg-info/PKG-INFO` & `clipcrop-2.2/clipcrop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 2.1
+Version: 2.2
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clipcrop-2.1/setup.py` & `clipcrop-2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   'numpy',
   'opencv-python'
 ]
 
 
 setuptools.setup(
     name="clipcrop",
-    version="2.1",
+    version="2.2",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/clipcrop/',
     packages=[
```

