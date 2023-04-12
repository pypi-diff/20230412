# Comparing `tmp/napari-sam-0.3.2.tar.gz` & `tmp/napari-sam-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.3.2.tar", last modified: Wed Apr 12 10:04:42 2023, max compression
+gzip compressed data, was "napari-sam-0.3.3.tar", last modified: Wed Apr 12 10:10:14 2023, max compression
```

## Comparing `napari-sam-0.3.2.tar` & `napari-sam-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:04:42.672675 napari-sam-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 10:04:24.000000 napari-sam-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 10:04:24.000000 napari-sam-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 10:04:42.672675 napari-sam-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-12 10:04:24.000000 napari-sam-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 10:04:24.000000 napari-sam-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-12 10:04:42.676675 napari-sam-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:04:42.672675 napari-sam-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:04:42.672675 napari-sam-0.3.2/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 10:04:24.000000 napari-sam-0.3.2/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36420 2023-04-12 10:04:24.000000 napari-sam-0.3.2/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-12 10:04:24.000000 napari-sam-0.3.2/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-12 10:04:24.000000 napari-sam-0.3.2/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:04:42.672675 napari-sam-0.3.2/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 10:04:42.000000 napari-sam-0.3.2/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 10:04:42.000000 napari-sam-0.3.2/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:04:42.000000 napari-sam-0.3.2/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 10:04:42.000000 napari-sam-0.3.2/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 10:04:42.000000 napari-sam-0.3.2/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 10:04:42.000000 napari-sam-0.3.2/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:10:14.540764 napari-sam-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 10:09:51.000000 napari-sam-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 10:09:51.000000 napari-sam-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 10:10:14.540764 napari-sam-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-12 10:09:51.000000 napari-sam-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 10:09:51.000000 napari-sam-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-12 10:10:14.540764 napari-sam-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:10:14.536764 napari-sam-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:10:14.536764 napari-sam-0.3.3/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 10:09:51.000000 napari-sam-0.3.3/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36427 2023-04-12 10:09:51.000000 napari-sam-0.3.3/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-12 10:09:51.000000 napari-sam-0.3.3/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-12 10:09:51.000000 napari-sam-0.3.3/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:10:14.540764 napari-sam-0.3.3/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 10:10:14.000000 napari-sam-0.3.3/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 10:10:14.000000 napari-sam-0.3.3/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:10:14.000000 napari-sam-0.3.3/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 10:10:14.000000 napari-sam-0.3.3/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 10:10:14.000000 napari-sam-0.3.3/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 10:10:14.000000 napari-sam-0.3.3/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.3.2/LICENSE` & `napari-sam-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.2/PKG-INFO` & `napari-sam-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.2
+Version: 0.3.3
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
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.2 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.3 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

### Comparing `napari-sam-0.3.2/README.md` & `napari-sam-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.2/setup.cfg` & `napari-sam-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.2/src/napari_sam/_widget.py` & `napari-sam-0.3.3/src/napari_sam/_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -535,15 +535,15 @@
 
         changed_indices = np.where(prediction == 1)
         index_labels_old = self.label_layer.data[changed_indices]
         self.label_layer.data[self.label_layer.data == point_label] = 0
         if self.segmentation_mode == SegmentationMode.SEMANTIC or point_label == 0:
             self.label_layer.data[prediction == 1] = point_label
         else:
-            self.label_layer.data[prediction & (self.label_layer.data == 0)] = point_label
+            self.label_layer.data[(prediction == 1) & (self.label_layer.data == 0)] = point_label
         index_labels_new = self.label_layer.data[changed_indices]
         self.label_layer_changes = {"indices": changed_indices, "old_values": index_labels_old, "new_values": index_labels_new}
         self.label_layer.data = self.label_layer.data
         # self.label_layer.refresh()
 
     def predict(self, points, labels):
         points = np.asarray(points)
```

### Comparing `napari-sam-0.3.2/src/napari_sam/utils.py` & `napari-sam-0.3.3/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.2/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.3.3/src/napari_sam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.2
+Version: 0.3.3
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
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.2 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.3 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

