# Comparing `tmp/napari-sam-0.3.1.tar.gz` & `tmp/napari-sam-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.3.1.tar", last modified: Wed Apr 12 09:57:13 2023, max compression
+gzip compressed data, was "napari-sam-0.3.2.tar", last modified: Wed Apr 12 10:04:42 2023, max compression
```

## Comparing `napari-sam-0.3.1.tar` & `napari-sam-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:57:13.721663 napari-sam-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 09:56:52.000000 napari-sam-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 09:56:52.000000 napari-sam-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 09:57:13.721663 napari-sam-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-12 09:56:52.000000 napari-sam-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 09:56:52.000000 napari-sam-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-12 09:57:13.721663 napari-sam-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:57:13.717663 napari-sam-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:57:13.721663 napari-sam-0.3.1/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 09:56:52.000000 napari-sam-0.3.1/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36340 2023-04-12 09:56:52.000000 napari-sam-0.3.1/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-12 09:56:52.000000 napari-sam-0.3.1/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-12 09:56:52.000000 napari-sam-0.3.1/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:57:13.721663 napari-sam-0.3.1/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 09:57:13.000000 napari-sam-0.3.1/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 09:57:13.000000 napari-sam-0.3.1/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:57:13.000000 napari-sam-0.3.1/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 09:57:13.000000 napari-sam-0.3.1/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 09:57:13.000000 napari-sam-0.3.1/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 09:57:13.000000 napari-sam-0.3.1/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:04:42.672675 napari-sam-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 10:04:24.000000 napari-sam-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 10:04:24.000000 napari-sam-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 10:04:42.672675 napari-sam-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-12 10:04:24.000000 napari-sam-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 10:04:24.000000 napari-sam-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-12 10:04:42.676675 napari-sam-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:04:42.672675 napari-sam-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:04:42.672675 napari-sam-0.3.2/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 10:04:24.000000 napari-sam-0.3.2/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36420 2023-04-12 10:04:24.000000 napari-sam-0.3.2/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-12 10:04:24.000000 napari-sam-0.3.2/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-12 10:04:24.000000 napari-sam-0.3.2/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:04:42.672675 napari-sam-0.3.2/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 10:04:42.000000 napari-sam-0.3.2/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 10:04:42.000000 napari-sam-0.3.2/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:04:42.000000 napari-sam-0.3.2/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 10:04:42.000000 napari-sam-0.3.2/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 10:04:42.000000 napari-sam-0.3.2/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 10:04:42.000000 napari-sam-0.3.2/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.3.1/LICENSE` & `napari-sam-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.1/PKG-INFO` & `napari-sam-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.1
+Version: 0.3.2
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.1 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.2 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

### Comparing `napari-sam-0.3.1/README.md` & `napari-sam-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.1/setup.cfg` & `napari-sam-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.1/src/napari_sam/_widget.py` & `napari-sam-0.3.2/src/napari_sam/_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,24 +191,24 @@
             self.rb_semantic.setStyleSheet("color: gray")
             self.rb_instance.setChecked(True)
         else:
             self.rb_semantic.setEnabled(True)
             self.rb_semantic.setStyleSheet("")
 
     def on_image_change(self):
-        if self.viewer.layers[self.cb_image_layers.currentText()].ndim > 2:
+        image_name = self.cb_image_layers.currentText()
+        if image_name != "" and self.viewer.layers[image_name].ndim > 2:
             self.rb_auto.setEnabled(False)
             self.rb_auto.setChecked(False)
             self.rb_click.setChecked(True)
             self.rb_auto.setStyleSheet("color: gray")
         else:
             self.rb_auto.setEnabled(True)
             self.rb_auto.setStyleSheet("")
 
-
     def init_model_type_combobox(self):
         model_types = list(sam_model_registry.keys())
         cached_weight_types = get_cached_weight_types(model_types)
         entries = []
         for name, is_cached in cached_weight_types.items():
             if is_cached:
                 entries.append("{} (Cached)".format(name))
@@ -440,16 +440,16 @@
                 yield
             elif event.button == 1 and self.points_layer is not None and len(self.points_layer.data) > 0:
                 # Find the closest point to the mouse click
                 distances = np.linalg.norm(self.points_layer.data - coords, axis=1)
                 closest_point_idx = np.argmin(distances)
                 closest_point_distance = distances[closest_point_idx]
 
-                # Select the closest point if it's within 5 pixels of the click
-                if closest_point_distance <= 5:
+                # Select the closest point if it's within self.point_size pixels of the click
+                if closest_point_distance <= self.point_size:
                     self.points_layer.selected_data = {closest_point_idx}
                 else:
                     self.points_layer.selected_data = set()
 
     def on_delete(self, layer):
         selected_points = list(self.points_layer.selected_data)
         if len(selected_points) > 0:
```

### Comparing `napari-sam-0.3.1/src/napari_sam/utils.py` & `napari-sam-0.3.2/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.1/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.3.2/src/napari_sam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.1
+Version: 0.3.2
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.1 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.2 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

