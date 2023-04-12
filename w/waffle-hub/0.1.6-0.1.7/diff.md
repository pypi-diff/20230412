# Comparing `tmp/waffle_hub-0.1.6.tar.gz` & `tmp/waffle_hub-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.1.6.tar", last modified: Mon Apr 10 11:42:10 2023, max compression
+gzip compressed data, was "waffle_hub-0.1.7.tar", last modified: Wed Apr 12 07:56:56 2023, max compression
```

## Comparing `waffle_hub-0.1.6.tar` & `waffle_hub-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.650711 waffle_hub-0.1.6/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-03-20 23:40:26.000000 waffle_hub-0.1.6/LICENSE
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-03-20 23:40:26.000000 waffle_hub-0.1.6/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      885 2023-04-03 23:38:22.000000 waffle_hub-0.1.6/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      213 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-04-10 11:42:10.650711 waffle_hub-0.1.6/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2643 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     6036 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/tests/test_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2500 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/experimental/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/experimental/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/experimental/serve.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/hub/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       63 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/configs/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/configs/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2573 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1793 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8318 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/tx_model_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/hub/adapter/ultralytics/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10931 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    21077 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/hub/base_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/hub/model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/hub/model/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     6340 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/hub/model/wrapper.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1247 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/run.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/schema/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/schema/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      614 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/schema/base_schema.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1257 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/schema/configs.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1170 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/schema/data.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5252 2023-04-10 11:40:54.000000 waffle_hub-0.1.6/waffle_hub/utils/callback.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3385 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/utils/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2239 2023-04-10 11:39:56.000000 waffle_hub-0.1.6/waffle_hub/utils/draw.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:42:10.646711 waffle_hub-0.1.6/waffle_hub.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-10 11:42:10.000000 waffle_hub-0.1.6/waffle_hub.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1119 2023-04-10 11:42:10.000000 waffle_hub-0.1.6/waffle_hub.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-04-10 11:42:10.000000 waffle_hub-0.1.6/waffle_hub.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-04-10 11:42:10.000000 waffle_hub-0.1.6/waffle_hub.egg-info/entry_points.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      172 2023-04-10 11:42:10.000000 waffle_hub-0.1.6/waffle_hub.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-04-10 11:42:10.000000 waffle_hub-0.1.6/waffle_hub.egg-info/top_level.txt
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-03-20 23:40:26.000000 waffle_hub-0.1.7/LICENSE
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-03-20 23:40:26.000000 waffle_hub-0.1.7/MANIFEST.in
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      885 2023-04-03 23:38:22.000000 waffle_hub-0.1.7/README.md
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      213 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/requirements.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/setup.cfg
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2643 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/setup.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/tests/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     6878 2023-04-12 07:56:27.000000 waffle_hub-0.1.7/tests/test_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2500 2023-04-12 07:56:27.000000 waffle_hub-0.1.7/waffle_hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/experimental/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/experimental/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/experimental/serve.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/hub/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       63 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/configs/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/configs/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2573 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1793 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     8318 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/tx_model_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/hub/adapter/ultralytics/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10931 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    21793 2023-04-12 07:56:27.000000 waffle_hub-0.1.7/waffle_hub/hub/base_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/hub/model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/model/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     6340 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/hub/model/wrapper.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1247 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/run.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/schema/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/schema/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      614 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/schema/base_schema.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1257 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/schema/configs.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1170 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/schema/data.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/utils/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5480 2023-04-12 07:56:27.000000 waffle_hub-0.1.7/waffle_hub/utils/callback.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3385 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/utils/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2239 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/utils/draw.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub.egg-info/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-12 07:56:56.000000 waffle_hub-0.1.7/waffle_hub.egg-info/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1119 2023-04-12 07:56:56.000000 waffle_hub-0.1.7/waffle_hub.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-04-12 07:56:56.000000 waffle_hub-0.1.7/waffle_hub.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-04-12 07:56:56.000000 waffle_hub-0.1.7/waffle_hub.egg-info/entry_points.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      172 2023-04-12 07:56:56.000000 waffle_hub-0.1.7/waffle_hub.egg-info/requires.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-04-12 07:56:56.000000 waffle_hub-0.1.7/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.1.6/LICENSE` & `waffle_hub-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/PKG-INFO` & `waffle_hub-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_hub
-Version: 0.1.6
+Version: 0.1.7
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_hub Version: 0.1.6 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle_hub Version: 0.1.7 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.1.6/README.md` & `waffle_hub-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/setup.py` & `waffle_hub-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/tests/test_hub.py` & `waffle_hub-0.1.7/tests/test_hub.py`

 * *Files 16% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     assert len(feature_maps) == 1
 
 
 def test_non_hold(tmpdir: Path, dummy_dataset: Dataset):
 
     export_dir = dummy_dataset.export("yolo_detection")
 
-    name = "test_det"
+    name = "test_det_hold"
 
     hub = UltralyticsHub.new(
         name=name,
         task="object_detection",
         model_type="yolov8",
         model_size="n",
         categories=["1", "2"],
@@ -161,42 +161,73 @@
     )
     hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
     hub: UltralyticsHub = UltralyticsHub.from_model_config(
         name=name,
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
+
+    # fail case
+    try:
+        train_callback: TrainCallback = hub.train(
+            dataset_path="dummy no data",
+            epochs=1,
+            batch_size=4,
+            image_size=32,
+            pretrained_model=None,
+            device="cpu",
+            hold=False,
+        )
+        while not train_callback.is_finished():
+            time.sleep(1)
+    except Exception:
+        pass
+    assert train_callback.is_failed()
+
+    # success case
     train_callback: TrainCallback = hub.train(
         dataset_path=export_dir,
         epochs=1,
         batch_size=4,
         image_size=32,
         pretrained_model=None,
         device="cpu",
         hold=False,
     )
 
     while not train_callback.is_finished():
         time.sleep(1)
+    while not Path(train_callback.best_ckpt_file).exists():
+        time.sleep(1)
+
+    assert not train_callback.is_failed()
 
     assert train_callback.get_progress() == 1
     assert len(train_callback.get_metrics()) == 1
     assert Path(train_callback.best_ckpt_file).exists()
     assert Path(train_callback.last_ckpt_file).exists()
     assert Path(train_callback.metric_file).exists()
     assert Path(train_callback.result_dir).exists()
 
     inference_callback: InferenceCallback = hub.inference(
         source=export_dir, device="cpu", hold=False
     )
     while not inference_callback.is_finished():
         time.sleep(1)
+    while not Path(inference_callback.inference_dir).exists():
+        time.sleep(1)
+
+    assert not inference_callback.is_failed()
 
     assert inference_callback.get_progress() == 1
     assert Path(inference_callback.inference_dir).exists()
 
     export_callback: ExportCallback = hub.export(hold=False)
 
     while not export_callback.is_finished():
         time.sleep(1)
+    while not Path(export_callback.export_file).exists():
+        time.sleep(1)
+
+    assert not export_callback.is_failed()
 
     assert Path(export_callback.export_file).exists()
```

### Comparing `waffle_hub-0.1.6/waffle_hub/__init__.py` & `waffle_hub-0.1.7/waffle_hub/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 
 import importlib
 import warnings
 from collections import OrderedDict
 
 from tabulate import tabulate
```

### Comparing `waffle_hub-0.1.6/waffle_hub/experimental/serve.py` & `waffle_hub-0.1.7/waffle_hub/experimental/serve.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py` & `waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py` & `waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/waffle_hub/hub/adapter/tx_model/tx_model_hub.py` & `waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/tx_model_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.1.7/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/waffle_hub/hub/base_hub.py` & `waffle_hub-0.1.7/waffle_hub/hub/base_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,48 +395,50 @@
             ValueError: if can not detect appropriate dataset.
             e: something gone wrong with ultralytics
 
         Returns:
             TrainCallback: train callback
         """
 
+        def inner(callback: TrainCallback):
+            try:
+                self.before_train(cfg)
+                self.on_train_start(cfg)
+                self.save_train_config(cfg)
+                self.training(cfg, callback)
+                self.on_train_end(cfg)
+                self.after_train(cfg)
+                callback.force_finish()
+            except Exception as e:
+                if self.artifact_dir.exists():
+                    io.remove_directory(self.artifact_dir)
+                callback.force_finish()
+                callback.set_failed()
+                raise e
+
         cfg = TrainConfig(
             dataset_path=dataset_path,
             epochs=epochs,
             batch_size=batch_size,
             image_size=image_size,
             learning_rate=learning_rate,
             letter_box=letter_box,
             pretrained_model=pretrained_model,
             device=device,
             workers=workers,
             seed=seed,
             verbose=verbose,
         )
-        self.before_train(cfg)
-        self.on_train_start(cfg)
-        self.save_train_config(cfg)
-
-        def inner(callback: TrainCallback):
-            try:
-                self.training(cfg, callback)
-                callback.best_ckpt_file = self.best_ckpt_file
-                callback.last_ckpt_file = self.last_ckpt_file
-                callback.metric_file = self.metric_file
-                callback.result_dir = self.hub_dir
-                self.on_train_end(cfg)
-                self.after_train(cfg)
-                callback.force_finish()
-            except Exception as e:
-                if self.artifact_dir.exists():
-                    io.remove_directory(self.artifact_dir)
-                callback.force_finish()
-                raise e
 
         callback = TrainCallback(cfg.epochs, self.get_metrics)
+        callback.best_ckpt_file = self.best_ckpt_file
+        callback.last_ckpt_file = self.last_ckpt_file
+        callback.metric_file = self.metric_file
+        callback.result_dir = self.hub_dir
+
         if hold:
             inner(callback)
         else:
             thread = threading.Thread(
                 target=inner, args=(callback,), daemon=True
             )
             callback.register_thread(thread)
@@ -546,15 +548,29 @@
         Raises:
             FileNotFoundError: if can not detect appropriate dataset.
             e: something gone wrong with ultralytics
 
         Returns:
             InferenceCallback: inference callback
         """
-        self.check_train_sanity()
+
+        def inner(callback):
+            try:
+                self.before_inference(cfg)
+                self.on_inference_start(cfg)
+                self.inferencing(cfg, callback)
+                self.on_inference_end(cfg)
+                self.after_inference(cfg)
+                callback.force_finish()
+            except Exception as e:
+                if self.inference_dir.exists():
+                    io.remove_directory(self.inference_dir)
+                callback.force_finish()
+                callback.set_failed()
+                raise e
 
         cfg = InferenceConfig(
             source=source,
             batch_size=batch_size,
             recursive=recursive,
             image_size=image_size,
             letter_box=letter_box,
@@ -562,70 +578,43 @@
             iou_threshold=iou_threshold,
             half=half,
             workers=workers,
             device="cpu" if device == "cpu" else f"cuda:{device}",
             draw=draw,
         )
 
-        self.before_inference(cfg)
-        self.on_inference_start(cfg)
-
-        def inner(callback):
-            try:
-                self.inferencing(cfg, callback)
-                callback.inference_dir = self.inference_dir
-                callback.draw_dir = self.draw_dir if cfg.draw else None
-                self.on_inference_end(cfg)
-                self.after_inference(cfg)
-                callback.force_finish()
-            except Exception as e:
-                if self.inference_dir.exists():
-                    io.remove_directory(self.inference_dir)
-                callback.force_finish()
-                raise e
-
         callback = InferenceCallback(0)
+        callback.inference_dir = self.inference_dir
+        callback.draw_dir = self.draw_dir if cfg.draw else None
 
         if hold:
             inner(callback)
         else:
             thread = threading.Thread(
                 target=inner, args=(callback,), daemon=True
             )
             callback.register_thread(thread)
             callback.start()
 
         return callback
 
     # Export Hook
-    def export(
-        self,
-        image_size: Union[int, list[int]] = None,
-        batch_size: int = 16,
-        opset_version: int = 11,
-        hold: bool = True,
-    ) -> ExportCallback:
-        """Export Model
-
-        Args:
-            image_size (Union[int, list[int]], optional): inference image size. None for same with train_config (recommended).
-            batch_size (int, optional): dynamic batch size. Defaults to 16.
-            opset_version (int, optional): onnx opset version. Defaults to 11.
-            hold (bool, optional): hold or not.
-                If True then it holds until task finished.
-                If False then return Inferece Callback and run in background. Defaults to True.
-
-        Returns:
-            ExportCallback: export callback
-        """
+    def before_export(self, cfg: ExportConfig):
         self.check_train_sanity()
 
+        # overwrite training config
         train_config = self.get_train_config()
+        if cfg.image_size is None:
+            cfg.image_size = train_config.image_size
 
-        image_size = image_size if image_size else train_config.image_size
+    def on_export_start(self, cfg: ExportConfig):
+        pass
+
+    def exporting(self, cfg: ExportConfig, callback: ExportCallback) -> str:
+        image_size = cfg.image_size
         image_size = (
             [image_size, image_size]
             if isinstance(image_size, int)
             else image_size
         )
 
         model = self.get_model()
@@ -636,39 +625,78 @@
         elif self.task == "classification":
             output_names = ["predictions"]
         else:
             raise NotImplementedError(
                 f"{self.task} does not support export yet."
             )
 
-        dummy_input = torch.randn(batch_size, 3, *image_size)
+        dummy_input = torch.randn(cfg.batch_size, 3, *image_size)
+
+        torch.onnx.export(
+            model,
+            dummy_input,
+            str(self.onnx_file),
+            input_names=input_name,
+            output_names=output_names,
+            opset_version=cfg.opset_version,
+            dynamic_axes={
+                name: {0: "batch_size"} for name in input_name + output_names
+            },
+        )
+
+    def on_export_end(self, cfg: ExportConfig):
+        pass
+
+    def after_export(self, cfg: ExportConfig):
+        pass
+
+    def export(
+        self,
+        image_size: Union[int, list[int]] = None,
+        batch_size: int = 16,
+        opset_version: int = 11,
+        hold: bool = True,
+    ) -> ExportCallback:
+        """Export Model
+
+        Args:
+            image_size (Union[int, list[int]], optional): inference image size. None for same with train_config (recommended).
+            batch_size (int, optional): dynamic batch size. Defaults to 16.
+            opset_version (int, optional): onnx opset version. Defaults to 11.
+            hold (bool, optional): hold or not.
+                If True then it holds until task finished.
+                If False then return Inferece Callback and run in background. Defaults to True.
+
+        Returns:
+            ExportCallback: export callback
+        """
 
         def inner(callback):
             try:
-                torch.onnx.export(
-                    model,
-                    dummy_input,
-                    str(self.onnx_file),
-                    input_names=input_name,
-                    output_names=output_names,
-                    opset_version=opset_version,
-                    dynamic_axes={
-                        name: {0: "batch_size"}
-                        for name in input_name + output_names
-                    },
-                )
-                callback.export_file = self.onnx_file
+                self.before_export(cfg)
+                self.on_export_start(cfg)
+                self.exporting(cfg, callback)
+                self.on_export_end(cfg)
+                self.after_export(cfg)
                 callback.force_finish()
             except Exception as e:
                 if self.onnx_file.exists():
                     io.remove_file(self.onnx_file)
                 callback.force_finish()
+                callback.set_failed()
                 raise e
 
+        cfg = ExportConfig(
+            image_size=image_size,
+            batch_size=batch_size,
+            opset_version=opset_version,
+        )
+
         callback = ExportCallback(1)
+        callback.export_file = self.onnx_file
 
         if hold:
             inner(callback)
         else:
             thread = threading.Thread(
                 target=inner, args=(callback,), daemon=True
             )
```

### Comparing `waffle_hub-0.1.6/waffle_hub/hub/model/wrapper.py` & `waffle_hub-0.1.7/waffle_hub/hub/model/wrapper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/waffle_hub/run.py` & `waffle_hub-0.1.7/waffle_hub/run.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/waffle_hub/schema/base_schema.py` & `waffle_hub-0.1.7/waffle_hub/schema/base_schema.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/waffle_hub/schema/configs.py` & `waffle_hub-0.1.7/waffle_hub/schema/configs.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/waffle_hub/schema/data.py` & `waffle_hub-0.1.7/waffle_hub/schema/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/waffle_hub/utils/callback.py` & `waffle_hub-0.1.7/waffle_hub/utils/callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,25 +43,34 @@
 
 class ThreadProgressCallback:
     def __init__(self, total_steps: int):
         self._total_steps = total_steps
 
         self._thread = None
         self._finished = False
+        self._failed = False
         self._progress = 0
         self._start_time = time.time()
 
     def get_progress(self) -> float:
         """Get the progress of the task. (0 ~ 1)"""
         return self._progress
 
     def is_finished(self) -> bool:
         """Check if the task has finished."""
         return self._finished
 
+    def is_failed(self) -> bool:
+        """Check if the task has failed."""
+        return self._failed
+
+    def set_failed(self):
+        """Set the task as failed."""
+        self._failed = True
+
     def get_remaining_time(self) -> float:
         """Get the remaining time of the task. (seconds)"""
         elapsed = time.time() - self._start_time
         if self._progress == 0:
             return float("inf")
         return (elapsed / self._progress) - elapsed
```

### Comparing `waffle_hub-0.1.6/waffle_hub/utils/data.py` & `waffle_hub-0.1.7/waffle_hub/utils/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/waffle_hub/utils/draw.py` & `waffle_hub-0.1.7/waffle_hub/utils/draw.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.6/waffle_hub.egg-info/PKG-INFO` & `waffle_hub-0.1.7/waffle_hub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-hub
-Version: 0.1.6
+Version: 0.1.7
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-hub Version: 0.1.6 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle-hub Version: 0.1.7 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.1.6/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.1.7/waffle_hub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

