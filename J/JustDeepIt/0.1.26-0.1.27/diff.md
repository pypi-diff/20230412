# Comparing `tmp/JustDeepIt-0.1.26.tar.gz` & `tmp/JustDeepIt-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JustDeepIt-0.1.26.tar", last modified: Wed Nov 30 01:32:46 2022, max compression
+gzip compressed data, was "JustDeepIt-0.1.27.tar", last modified: Wed Apr 12 05:40:29 2023, max compression
```

## Comparing `JustDeepIt-0.1.26.tar` & `JustDeepIt-0.1.27.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 01:32:46.419700 JustDeepIt-0.1.26/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 01:32:46.411700 JustDeepIt-0.1.26/JustDeepIt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2022-11-30 01:32:46.000000 JustDeepIt-0.1.26/JustDeepIt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2022-11-30 01:32:46.000000 JustDeepIt-0.1.26/JustDeepIt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 01:32:46.000000 JustDeepIt-0.1.26/JustDeepIt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-30 01:32:46.000000 JustDeepIt-0.1.26/JustDeepIt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      145 2022-11-30 01:32:46.000000 JustDeepIt-0.1.26/JustDeepIt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-11-30 01:32:46.000000 JustDeepIt-0.1.26/JustDeepIt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 01:32:46.000000 JustDeepIt-0.1.26/JustDeepIt.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       98 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2022-11-30 01:32:46.419700 JustDeepIt-0.1.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1451 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 01:32:46.411700 JustDeepIt-0.1.26/justdeepit/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 01:32:46.411700 JustDeepIt-0.1.26/justdeepit/models/
--rw-r--r--   0 runner    (1001) docker     (122)      184 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      270 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)    13213 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/models/instance_segment.py
--rw-r--r--   0 runner    (1001) docker     (122)    14917 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/models/object_detect.py
--rw-r--r--   0 runner    (1001) docker     (122)    12243 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/models/salient_object_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 01:32:46.415700 JustDeepIt-0.1.26/justdeepit/models/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10980 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/models/utils/detectron2base.py
--rw-r--r--   0 runner    (1001) docker     (122)    18103 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/models/utils/mmdetbase.py
--rw-r--r--   0 runner    (1001) docker     (122)    36052 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/models/utils/u2net.py
--rw-r--r--   0 runner    (1001) docker     (122)    10173 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/models/utils/unet.py
--rw-r--r--   0 runner    (1001) docker     (122)    54622 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 01:32:46.415700 JustDeepIt-0.1.26/justdeepit/webapp/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29097 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/app.py
--rw-r--r--   0 runner    (1001) docker     (122)     6491 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/appbase.py
--rw-r--r--   0 runner    (1001) docker     (122)     1378 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/appis.py
--rw-r--r--   0 runner    (1001) docker     (122)     8447 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/appod.py
--rw-r--r--   0 runner    (1001) docker     (122)    22154 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/appsod.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 01:32:46.419700 JustDeepIt-0.1.26/justdeepit/webapp/static/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/static/.Rhistory
--rw-r--r--   0 runner    (1001) docker     (122)    89501 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/static/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   137972 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/static/jquery-3.6.0.min.map
--rw-r--r--   0 runner    (1001) docker     (122)    14309 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/static/styles.css
--rw-r--r--   0 runner    (1001) docker     (122)    58702 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/static/tree.jquery.js
--rw-r--r--   0 runner    (1001) docker     (122)   174878 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/static/tree.jquery.js.map
--rw-r--r--   0 runner    (1001) docker     (122)    23287 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/static/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 01:32:46.419700 JustDeepIt-0.1.26/justdeepit/webapp/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     1198 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (122)    15402 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/templates/module.html
--rw-r--r--   0 runner    (1001) docker     (122)      571 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/justdeepit/webapp/templates/shutdown.html
--rw-r--r--   0 runner    (1001) docker     (122)      151 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-30 01:32:46.423700 JustDeepIt-0.1.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2652 2022-11-30 01:21:12.000000 JustDeepIt-0.1.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.489672 JustDeepIt-0.1.27/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.477672 JustDeepIt-0.1.27/JustDeepIt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:40:29.000000 JustDeepIt-0.1.27/JustDeepIt.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-12 05:40:29.489672 JustDeepIt-0.1.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.477672 JustDeepIt-0.1.27/justdeepit/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.481672 JustDeepIt-0.1.27/justdeepit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/instance_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14917 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/object_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12243 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/salient_object_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.481672 JustDeepIt-0.1.27/justdeepit/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/utils/detectron2base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/utils/mmdetbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36052 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/utils/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/models/utils/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.477672 JustDeepIt-0.1.27/justdeepit/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.485672 JustDeepIt-0.1.27/justdeepit/src/font/
+-rw-r--r--   0 runner    (1001) docker     (123)   555264 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/src/font/NotoSans-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/src/font/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    55796 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.485672 JustDeepIt-0.1.27/justdeepit/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29097 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/appbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/appis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/appod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22154 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/appsod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.489672 JustDeepIt-0.1.27/justdeepit/webapp/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/.Rhistory
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/jquery-3.6.0.min.map
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)    58702 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/tree.jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)   174878 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/tree.jquery.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    23287 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/static/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:40:29.489672 JustDeepIt-0.1.27/justdeepit/webapp/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/templates/module.html
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/justdeepit/webapp/templates/shutdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 05:40:29.489672 JustDeepIt-0.1.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-12 05:38:08.000000 JustDeepIt-0.1.27/setup.py
```

### Comparing `JustDeepIt-0.1.26/JustDeepIt.egg-info/PKG-INFO` & `JustDeepIt-0.1.27/JustDeepIt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.1.26
+Version: 0.1.27
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
 Keywords: object detection,object segmentation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `JustDeepIt-0.1.26/JustDeepIt.egg-info/SOURCES.txt` & `JustDeepIt-0.1.27/JustDeepIt.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 justdeepit/models/object_detect.py
 justdeepit/models/salient_object_detect.py
 justdeepit/models/utils/__init__.py
 justdeepit/models/utils/detectron2base.py
 justdeepit/models/utils/mmdetbase.py
 justdeepit/models/utils/u2net.py
 justdeepit/models/utils/unet.py
+justdeepit/src/font/NotoSans-Medium.ttf
+justdeepit/src/font/OFL.txt
 justdeepit/webapp/__init__.py
 justdeepit/webapp/app.py
 justdeepit/webapp/appbase.py
 justdeepit/webapp/appis.py
 justdeepit/webapp/appod.py
 justdeepit/webapp/appsod.py
 justdeepit/webapp/static/.Rhistory
```

### Comparing `JustDeepIt-0.1.26/LICENSE` & `JustDeepIt-0.1.27/LICENSE`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/PKG-INFO` & `JustDeepIt-0.1.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.1.26
+Version: 0.1.27
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
 Keywords: object detection,object segmentation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `JustDeepIt-0.1.26/README.md` & `JustDeepIt-0.1.27/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # JustDeepIt 
 
-Deep learning has been applied to solve various problems, especially in image recognition,
-across many fields including the life sciences and agriculture.
-Many studies have reported the use of deep learning to identify plant and insect species,
-detect flowers and fruits, segment plant individuals from fixed-point observation cameras or drone images,
-and other applications.
-Programming languages such as Python and its libraries including PyTorch, MMDetection, and Detectron2
-have made deep learning easier and more accessible to researchers.
-However, it remains difficult for many researchers without advanced programming skills
-to use deep learning and environments such as the character user interface (CUI) through keyboard input.
-JustDeepIt aims to support researchers by facilitating the use of deep learning for object detection and segmentation
-by providing both graphical user interface (GUI) and CUI operations.
-JustDeepIt can be used for plant detection, pest detection,
-and a variety of tasks in life sciences, agriculture, and other fields.
+Image analysis based on deep learning is becoming mainstream and increasingly accessible
+for solving various scientific problems in diverse fields including plant science.
+Practical applications in plant science include species classification,
+fruit detection, plant disease and pest detection, weed detection,
+leaf segmentation, and plant segmentation.
+Python programming language and its libraries including PyTorch, MMDetection, and Detectron2
+have made deep learning much easier and more accessible to researchers.
+However, deep learning technologies remain challenging for programming beginners
+because they require computer programming skills and a basic familiarity
+with character user interfaces (CUIs).
+JustDeepIt aims to simplify object detection, instance segmentation, and salient object detection
+using deep learning by providing a graphical user interface (GUI).
+In addition, to ensure flexibility and extensibility, JustDeepIt also provides CUI.
+It may be applicable for image analysis in various disciplines beyond plant science.
 
 
 ## Documentation
 
 - https://justdeepit.readthedocs.io/en/latest/index.html
 
 
 ## Citation
 
-Sun J, Cao W and Yamanaka T (2022)
-JustDeepIt: Software tool with graphical and character user interfaces for deep learning-based object detection and segmentation in image analysis.
-Front. Plant Sci. 13:964058.
+Sun J, Cao W, Yamanaka T.
+JustDeepIt: Software tool with graphical and character user interfaces
+for deep learning-based object detection and segmentation in image analysis.
+Front. Plant Sci., 2022, 13:964058.
 doi: [10.3389/fpls.2022.964058](https://doi.org/10.3389/fpls.2022.964058)
```

### Comparing `JustDeepIt-0.1.26/justdeepit/models/instance_segment.py` & `JustDeepIt-0.1.27/justdeepit/models/instance_segment.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/models/object_detect.py` & `JustDeepIt-0.1.27/justdeepit/models/object_detect.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/models/salient_object_detect.py` & `JustDeepIt-0.1.27/justdeepit/models/salient_object_detect.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/models/utils/detectron2base.py` & `JustDeepIt-0.1.27/justdeepit/models/utils/detectron2base.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/models/utils/mmdetbase.py` & `JustDeepIt-0.1.27/justdeepit/models/utils/mmdetbase.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/models/utils/u2net.py` & `JustDeepIt-0.1.27/justdeepit/models/utils/u2net.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/models/utils/unet.py` & `JustDeepIt-0.1.27/justdeepit/models/utils/unet.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/utils.py` & `JustDeepIt-0.1.27/justdeepit/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import re
 import gzip
 import json
 import base64
 import hashlib
 import random
 import string
+import pkg_resources
 import xml.etree.ElementTree as ET
 import numpy as np
 import cv2
 import skimage
 import skimage.io
 import skimage.color
 import skimage.measure
@@ -815,25 +816,55 @@
         if file_path is None:
             return img
         else:
             skimage.io.imsave(file_path, img.astype(np.uint8), check_contrast=False)
         
     
     
-    def __put_text(self, img, text, pos=(0, 0),
+    def __put_text_cv(self, img, text, pos=(0, 0),
                    font=cv2.FONT_HERSHEY_SIMPLEX, font_scale=1, font_thickness=2,
                    color=(0, 255, 0), bg_color=(0, 0, 0)):
+        '''
+        Write a text into image with OpenCV methods.
+        '''
         x, y = pos
         text_size, _ = cv2.getTextSize(text, font, font_scale, font_thickness)
         text_w, text_h = text_size
         cv2.rectangle(img, pos, (x + text_w + 10, y + text_h + 10), bg_color, -1)
         cv2.putText(img, text, (x + 5, y + text_h + font_scale + 5), font, font_scale, color, font_thickness)
         return img
 
     
+    def __pil2cv(self, img):
+        img_cv_rgb = np.array(img, dtype = np.uint8)
+        img_cv_bgr = np.array(img)[:, :, ::-1]
+        return img_cv_bgr
+    
+    
+    def __cv2pil(self, img):
+        return PIL.Image.fromarray(img[:, :, ::-1])
+    
+    
+    def __put_text(self, img, text, pos=(0, 0),
+                         font=None, font_scale=28, font_thickness=1,
+                         color=(0, 255, 0), bg_color=(0, 0, 0)):
+        x, y = pos
+        x = x + 5
+        y = y - font_scale - 5
+        if font is None:
+            font = pkg_resources.resource_filename('justdeepit', 'src/font/NotoSans-Medium.ttf')
+        img_pil = self.__cv2pil(img)
+        font = PIL.ImageFont.truetype(font=font, size=font_scale)
+        draw = PIL.ImageDraw.Draw(img_pil)
+        l_, t_, r_, b_ = draw.textbbox((x, y), text, font=font)
+        draw.rectangle((l_ - 5, t_ - 5, r_ + 5, b_ + 5),
+                       fill=color[::-1], outline=color[::-1], width=5)
+        draw.text((x, y), text, font=font, fill=bg_color[::-1])
+        return self.__pil2cv(img_pil)
+    
 
     def __get_bg_color(self, col):
         lbg = 0.2126 * col[0] + 0.7152 * col[1] + 0.0722 * col[2]
         lw = 1
         lb = 0
         cw = (lw + 0.05) / (lbg + 0.05)
         cb = (lbg + 0.05) / (lb + 0.05)
```

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/app.py` & `JustDeepIt-0.1.27/justdeepit/webapp/app.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/appbase.py` & `JustDeepIt-0.1.27/justdeepit/webapp/appbase.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/appis.py` & `JustDeepIt-0.1.27/justdeepit/webapp/appis.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/appod.py` & `JustDeepIt-0.1.27/justdeepit/webapp/appod.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/appsod.py` & `JustDeepIt-0.1.27/justdeepit/webapp/appsod.py`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/static/jquery-3.6.0.min.js` & `JustDeepIt-0.1.27/justdeepit/webapp/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/static/jquery-3.6.0.min.map` & `JustDeepIt-0.1.27/justdeepit/webapp/static/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/static/styles.css` & `JustDeepIt-0.1.27/justdeepit/webapp/static/styles.css`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/static/tree.jquery.js` & `JustDeepIt-0.1.27/justdeepit/webapp/static/tree.jquery.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/static/tree.jquery.js.map` & `JustDeepIt-0.1.27/justdeepit/webapp/static/tree.jquery.js.map`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/static/utils.js` & `JustDeepIt-0.1.27/justdeepit/webapp/static/utils.js`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/templates/index.html` & `JustDeepIt-0.1.27/justdeepit/webapp/templates/index.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/templates/module.html` & `JustDeepIt-0.1.27/justdeepit/webapp/templates/module.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/justdeepit/webapp/templates/shutdown.html` & `JustDeepIt-0.1.27/justdeepit/webapp/templates/shutdown.html`

 * *Files identical despite different names*

### Comparing `JustDeepIt-0.1.26/setup.py` & `JustDeepIt-0.1.27/setup.py`

 * *Files identical despite different names*

