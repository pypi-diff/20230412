# Comparing `tmp/napari-sam-0.3.0.tar.gz` & `tmp/napari-sam-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.3.0.tar", last modified: Tue Apr 11 20:23:00 2023, max compression
+gzip compressed data, was "napari-sam-0.3.1.tar", last modified: Wed Apr 12 09:57:13 2023, max compression
```

## Comparing `napari-sam-0.3.0.tar` & `napari-sam-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:23:00.561604 napari-sam-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 20:22:37.000000 napari-sam-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 20:22:37.000000 napari-sam-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-04-11 20:23:00.561604 napari-sam-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-04-11 20:22:37.000000 napari-sam-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-11 20:22:37.000000 napari-sam-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-11 20:23:00.561604 napari-sam-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:23:00.561604 napari-sam-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:23:00.561604 napari-sam-0.3.0/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-11 20:22:37.000000 napari-sam-0.3.0/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35840 2023-04-11 20:22:37.000000 napari-sam-0.3.0/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-11 20:22:37.000000 napari-sam-0.3.0/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-11 20:22:37.000000 napari-sam-0.3.0/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:23:00.561604 napari-sam-0.3.0/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-04-11 20:23:00.000000 napari-sam-0.3.0/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 20:23:00.000000 napari-sam-0.3.0/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:23:00.000000 napari-sam-0.3.0/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-11 20:23:00.000000 napari-sam-0.3.0/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-11 20:23:00.000000 napari-sam-0.3.0/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 20:23:00.000000 napari-sam-0.3.0/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:57:13.721663 napari-sam-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 09:56:52.000000 napari-sam-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 09:56:52.000000 napari-sam-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 09:57:13.721663 napari-sam-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-12 09:56:52.000000 napari-sam-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 09:56:52.000000 napari-sam-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-12 09:57:13.721663 napari-sam-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:57:13.717663 napari-sam-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:57:13.721663 napari-sam-0.3.1/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 09:56:52.000000 napari-sam-0.3.1/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36340 2023-04-12 09:56:52.000000 napari-sam-0.3.1/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-12 09:56:52.000000 napari-sam-0.3.1/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-12 09:56:52.000000 napari-sam-0.3.1/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:57:13.721663 napari-sam-0.3.1/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 09:57:13.000000 napari-sam-0.3.1/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 09:57:13.000000 napari-sam-0.3.1/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:57:13.000000 napari-sam-0.3.1/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 09:57:13.000000 napari-sam-0.3.1/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 09:57:13.000000 napari-sam-0.3.1/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 09:57:13.000000 napari-sam-0.3.1/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.3.0/LICENSE` & `napari-sam-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.0/PKG-INFO` & `napari-sam-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.0
+Version: 0.3.1
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
@@ -38,14 +38,16 @@
 
 Segment anything with our **Napari** integration of Meta AI's new **Segment Anything Model (SAM)**!
 
 SAM is the new segmentation system from Meta AI capable of **one-click segmentation of any object**, and now, our plugin neatly integrates this into Napari.
 
 We have already **extended** SAM's click-based foreground separation to full **click-based semantic segmentation and instance segmentation**!
 
+At last, our SAM integration supports both **2D and 3D images**!
+
 ----------------------------------
 
 Everything mode             |  Click-based semantic segmentation mode |  Click-based instance segmentation mode
 :-------------------------:|:-------------------------:|:-------------------------:
 ![](cats_everything.png)  |  ![](cats_semantic.png)  |  ![](cats_instance.png)
 
 ----------------------------------
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.0 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.1 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
@@ -25,18 +25,19 @@
 badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam) [![napari hub](https://
 img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sam)]
 (https://napari-hub.org/plugins/napari-sam) Segment anything with our
 **Napari** integration of Meta AI's new **Segment Anything Model (SAM)**! SAM
 is the new segmentation system from Meta AI capable of **one-click segmentation
 of any object**, and now, our plugin neatly integrates this into Napari. We
 have already **extended** SAM's click-based foreground separation to full
-**click-based semantic segmentation and instance segmentation**! --------------
--------------------- Everything mode | Click-based semantic segmentation mode |
-Click-based instance segmentation mode :-------------------------:|:-----------
---------------:|:-------------------------: ![](cats_everything.png) | ![]
+**click-based semantic segmentation and instance segmentation**! At last, our
+SAM integration supports both **2D and 3D images**! ---------------------------
+------- Everything mode | Click-based semantic segmentation mode | Click-based
+instance segmentation mode :-------------------------:|:-----------------------
+--:|:-------------------------: ![](cats_everything.png) | ![]
 (cats_semantic.png) | ![](cats_instance.png) ----------------------------------
                         ***** SAM in Napari demo *****
                             Click to play the video
                                   [SAM_Demo]
 ---------------------------------- ## Installation The plugin requires
 `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow
 the instructions here to install both PyTorch and TorchVision dependencies.
```

### Comparing `napari-sam-0.3.0/README.md` & `napari-sam-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 Segment anything with our **Napari** integration of Meta AI's new **Segment Anything Model (SAM)**!
 
 SAM is the new segmentation system from Meta AI capable of **one-click segmentation of any object**, and now, our plugin neatly integrates this into Napari.
 
 We have already **extended** SAM's click-based foreground separation to full **click-based semantic segmentation and instance segmentation**!
 
+At last, our SAM integration supports both **2D and 3D images**!
+
 ----------------------------------
 
 Everything mode             |  Click-based semantic segmentation mode |  Click-based instance segmentation mode
 :-------------------------:|:-------------------------:|:-------------------------:
 ![](cats_everything.png)  |  ![](cats_semantic.png)  |  ![](cats_instance.png)
 
 ----------------------------------
```

#### html2text {}

```diff
@@ -9,18 +9,19 @@
 graph/badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam) [![napari hub]
 (https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-
 sam)](https://napari-hub.org/plugins/napari-sam) Segment anything with our
 **Napari** integration of Meta AI's new **Segment Anything Model (SAM)**! SAM
 is the new segmentation system from Meta AI capable of **one-click segmentation
 of any object**, and now, our plugin neatly integrates this into Napari. We
 have already **extended** SAM's click-based foreground separation to full
-**click-based semantic segmentation and instance segmentation**! --------------
--------------------- Everything mode | Click-based semantic segmentation mode |
-Click-based instance segmentation mode :-------------------------:|:-----------
---------------:|:-------------------------: ![](cats_everything.png) | ![]
+**click-based semantic segmentation and instance segmentation**! At last, our
+SAM integration supports both **2D and 3D images**! ---------------------------
+------- Everything mode | Click-based semantic segmentation mode | Click-based
+instance segmentation mode :-------------------------:|:-----------------------
+--:|:-------------------------: ![](cats_everything.png) | ![]
 (cats_semantic.png) | ![](cats_instance.png) ----------------------------------
                         ***** SAM in Napari demo *****
                             Click to play the video
                                   [SAM_Demo]
 ---------------------------------- ## Installation The plugin requires
 `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow
 the instructions here to install both PyTorch and TorchVision dependencies.
```

### Comparing `napari-sam-0.3.0/setup.cfg` & `napari-sam-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.0/src/napari_sam/_widget.py` & `napari-sam-0.3.1/src/napari_sam/_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         self.init_model_type_combobox()
 
         l_image_layer = QLabel("Select input image layer:")
         self.layout().addWidget(l_image_layer)
 
         self.cb_image_layers = QComboBox()
         self.cb_image_layers.addItems(self.get_layer_names("image"))
+        self.cb_image_layers.currentTextChanged.connect(self.on_image_change)
         self.layout().addWidget(self.cb_image_layers)
 
         l_label_layer = QLabel("Select output labels layer:")
         self.layout().addWidget(l_label_layer)
 
         self.cb_label_layers = QComboBox()
         self.cb_label_layers.addItems(self.get_layer_names("labels"))
@@ -189,14 +190,25 @@
             self.rb_semantic.setChecked(False)
             self.rb_semantic.setStyleSheet("color: gray")
             self.rb_instance.setChecked(True)
         else:
             self.rb_semantic.setEnabled(True)
             self.rb_semantic.setStyleSheet("")
 
+    def on_image_change(self):
+        if self.viewer.layers[self.cb_image_layers.currentText()].ndim > 2:
+            self.rb_auto.setEnabled(False)
+            self.rb_auto.setChecked(False)
+            self.rb_click.setChecked(True)
+            self.rb_auto.setStyleSheet("color: gray")
+        else:
+            self.rb_auto.setEnabled(True)
+            self.rb_auto.setStyleSheet("")
+
+
     def init_model_type_combobox(self):
         model_types = list(sam_model_registry.keys())
         cached_weight_types = get_cached_weight_types(model_types)
         entries = []
         for name, is_cached in cached_weight_types.items():
             if is_cached:
                 entries.append("{} (Cached)".format(name))
@@ -270,14 +282,15 @@
         for layer in layers:
             if (type == "all" or isinstance(layer, self.layer_types[type])) and ((not exclude_hidden) or (exclude_hidden and "<hidden>" not in layer.name)):
                 filtered_layers.append(layer.name)
         return filtered_layers
 
     def _init_comboboxes_callback(self):
         self._check_activate_btn()
+        self.on_image_change()
 
     def _on_layers_changed_callback(self):
         self._check_activate_btn()
         if (self.image_layer is not None and self.image_layer not in self.viewer.layers) or (self.label_layer is not None and self.label_layer not in self.viewer.layers):
             self._deactivate()
 
     def _check_activate_btn(self):
```

### Comparing `napari-sam-0.3.0/src/napari_sam/utils.py` & `napari-sam-0.3.1/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.0/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.3.1/src/napari_sam.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.0
+Version: 0.3.1
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
@@ -38,14 +38,16 @@
 
 Segment anything with our **Napari** integration of Meta AI's new **Segment Anything Model (SAM)**!
 
 SAM is the new segmentation system from Meta AI capable of **one-click segmentation of any object**, and now, our plugin neatly integrates this into Napari.
 
 We have already **extended** SAM's click-based foreground separation to full **click-based semantic segmentation and instance segmentation**!
 
+At last, our SAM integration supports both **2D and 3D images**!
+
 ----------------------------------
 
 Everything mode             |  Click-based semantic segmentation mode |  Click-based instance segmentation mode
 :-------------------------:|:-------------------------:|:-------------------------:
 ![](cats_everything.png)  |  ![](cats_semantic.png)  |  ![](cats_instance.png)
 
 ----------------------------------
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.0 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.1 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
@@ -25,18 +25,19 @@
 badge.svg)](https://codecov.io/gh/MIC-DKFZ/napari-sam) [![napari hub](https://
 img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sam)]
 (https://napari-hub.org/plugins/napari-sam) Segment anything with our
 **Napari** integration of Meta AI's new **Segment Anything Model (SAM)**! SAM
 is the new segmentation system from Meta AI capable of **one-click segmentation
 of any object**, and now, our plugin neatly integrates this into Napari. We
 have already **extended** SAM's click-based foreground separation to full
-**click-based semantic segmentation and instance segmentation**! --------------
--------------------- Everything mode | Click-based semantic segmentation mode |
-Click-based instance segmentation mode :-------------------------:|:-----------
---------------:|:-------------------------: ![](cats_everything.png) | ![]
+**click-based semantic segmentation and instance segmentation**! At last, our
+SAM integration supports both **2D and 3D images**! ---------------------------
+------- Everything mode | Click-based semantic segmentation mode | Click-based
+instance segmentation mode :-------------------------:|:-----------------------
+--:|:-------------------------: ![](cats_everything.png) | ![]
 (cats_semantic.png) | ![](cats_instance.png) ----------------------------------
                         ***** SAM in Napari demo *****
                             Click to play the video
                                   [SAM_Demo]
 ---------------------------------- ## Installation The plugin requires
 `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow
 the instructions here to install both PyTorch and TorchVision dependencies.
```

