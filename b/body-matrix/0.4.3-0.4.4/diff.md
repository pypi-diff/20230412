# Comparing `tmp/body_matrix-0.4.3.tar.gz` & `tmp/body_matrix-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/troydo42/Desktop/Body_Matrix/dist/.tmp-3dazmxqk/body_matrix-0.4.3.tar", last modified: Wed Apr 12 04:06:52 2023, max compression
+gzip compressed data, was "/Users/troydo42/Desktop/Body_Matrix/dist/.tmp-ud_7jvws/body_matrix-0.4.4.tar", last modified: Wed Apr 12 04:48:05 2023, max compression
```

## Comparing `body_matrix-0.4.3.tar` & `body_matrix-0.4.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-04-12 04:06:52.000000 body_matrix-0.4.3/
--rw-r--r--   0 troydo42   (501) staff       (20)     1069 2023-01-16 08:57:57.000000 body_matrix-0.4.3/LICENSE
--rw-r--r--   0 troydo42   (501) staff       (20)     2696 2023-04-12 04:06:52.000000 body_matrix-0.4.3/PKG-INFO
--rw-r--r--   0 troydo42   (501) staff       (20)     2170 2023-03-30 07:26:33.000000 body_matrix-0.4.3/README.md
--rw-r--r--   0 troydo42   (501) staff       (20)      631 2023-04-12 04:05:52.000000 body_matrix-0.4.3/pyproject.toml
--rw-r--r--   0 troydo42   (501) staff       (20)       38 2023-04-12 04:06:52.000000 body_matrix-0.4.3/setup.cfg
-drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-04-12 04:06:52.000000 body_matrix-0.4.3/src/
-drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-04-12 04:06:52.000000 body_matrix-0.4.3/src/body_matrix/
--rw-r--r--   0 troydo42   (501) staff       (20)        0 2023-01-16 08:47:57.000000 body_matrix-0.4.3/src/body_matrix/__init__.py
--rw-r--r--   0 troydo42   (501) staff       (20)     7892 2023-04-12 03:59:49.000000 body_matrix-0.4.3/src/body_matrix/draw.py
--rw-r--r--   0 troydo42   (501) staff       (20)     5111 2023-04-12 03:58:06.000000 body_matrix-0.4.3/src/body_matrix/export.py
--rw-r--r--   0 troydo42   (501) staff       (20)     4488 2023-04-12 03:59:25.000000 body_matrix-0.4.3/src/body_matrix/infer.py
--rw-r--r--   0 troydo42   (501) staff       (20)     1753 2023-02-24 03:48:47.000000 body_matrix-0.4.3/src/body_matrix/load.py
--rw-r--r--   0 troydo42   (501) staff       (20)     6397 2023-04-12 04:00:23.000000 body_matrix-0.4.3/src/body_matrix/measure.py
--rw-r--r--   0 troydo42   (501) staff       (20)     8453 2023-04-12 04:01:05.000000 body_matrix-0.4.3/src/body_matrix/process.py
--rw-r--r--   0 troydo42   (501) staff       (20)     6748 2023-04-12 04:02:27.000000 body_matrix-0.4.3/src/body_matrix/score.py
-drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-04-12 04:06:52.000000 body_matrix-0.4.3/src/body_matrix.egg-info/
--rw-r--r--   0 troydo42   (501) staff       (20)     2696 2023-04-12 04:06:51.000000 body_matrix-0.4.3/src/body_matrix.egg-info/PKG-INFO
--rw-r--r--   0 troydo42   (501) staff       (20)      394 2023-04-12 04:06:52.000000 body_matrix-0.4.3/src/body_matrix.egg-info/SOURCES.txt
--rw-r--r--   0 troydo42   (501) staff       (20)        1 2023-04-12 04:06:51.000000 body_matrix-0.4.3/src/body_matrix.egg-info/dependency_links.txt
--rw-r--r--   0 troydo42   (501) staff       (20)       19 2023-04-12 04:06:51.000000 body_matrix-0.4.3/src/body_matrix.egg-info/top_level.txt
+drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-04-12 04:48:05.000000 body_matrix-0.4.4/
+-rw-r--r--   0 troydo42   (501) staff       (20)     1069 2023-01-16 08:57:57.000000 body_matrix-0.4.4/LICENSE
+-rw-r--r--   0 troydo42   (501) staff       (20)     2696 2023-04-12 04:48:05.000000 body_matrix-0.4.4/PKG-INFO
+-rw-r--r--   0 troydo42   (501) staff       (20)     2170 2023-03-30 07:26:33.000000 body_matrix-0.4.4/README.md
+-rw-r--r--   0 troydo42   (501) staff       (20)      631 2023-04-12 04:47:00.000000 body_matrix-0.4.4/pyproject.toml
+-rw-r--r--   0 troydo42   (501) staff       (20)       38 2023-04-12 04:48:05.000000 body_matrix-0.4.4/setup.cfg
+drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-04-12 04:48:05.000000 body_matrix-0.4.4/src/
+drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-04-12 04:48:05.000000 body_matrix-0.4.4/src/body_matrix/
+-rw-r--r--   0 troydo42   (501) staff       (20)        0 2023-01-16 08:47:57.000000 body_matrix-0.4.4/src/body_matrix/__init__.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     7892 2023-04-12 03:59:49.000000 body_matrix-0.4.4/src/body_matrix/draw.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     5111 2023-04-12 03:58:06.000000 body_matrix-0.4.4/src/body_matrix/export.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     4488 2023-04-12 03:59:25.000000 body_matrix-0.4.4/src/body_matrix/infer.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     1753 2023-02-24 03:48:47.000000 body_matrix-0.4.4/src/body_matrix/load.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     6438 2023-04-12 04:43:16.000000 body_matrix-0.4.4/src/body_matrix/measure.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     8453 2023-04-12 04:01:05.000000 body_matrix-0.4.4/src/body_matrix/process.py
+-rw-r--r--   0 troydo42   (501) staff       (20)     6748 2023-04-12 04:02:27.000000 body_matrix-0.4.4/src/body_matrix/score.py
+drwxr-xr-x   0 troydo42   (501) staff       (20)        0 2023-04-12 04:48:05.000000 body_matrix-0.4.4/src/body_matrix.egg-info/
+-rw-r--r--   0 troydo42   (501) staff       (20)     2696 2023-04-12 04:48:05.000000 body_matrix-0.4.4/src/body_matrix.egg-info/PKG-INFO
+-rw-r--r--   0 troydo42   (501) staff       (20)      394 2023-04-12 04:48:05.000000 body_matrix-0.4.4/src/body_matrix.egg-info/SOURCES.txt
+-rw-r--r--   0 troydo42   (501) staff       (20)        1 2023-04-12 04:48:05.000000 body_matrix-0.4.4/src/body_matrix.egg-info/dependency_links.txt
+-rw-r--r--   0 troydo42   (501) staff       (20)       19 2023-04-12 04:48:05.000000 body_matrix-0.4.4/src/body_matrix.egg-info/top_level.txt
```

### Comparing `body_matrix-0.4.3/LICENSE` & `body_matrix-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `body_matrix-0.4.3/PKG-INFO` & `body_matrix-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: body_matrix
-Version: 0.4.3
+Version: 0.4.4
 Summary: Package to Calculate Human Body Measurements
 Author-email: Hoang Do <hoang.do.2102@gmail.com>
 Project-URL: Homepage, https://github.com/akando42/body_matrix
 Project-URL: Bug Tracker, https://github.com/akando42/body_matrix/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `body_matrix-0.4.3/README.md` & `body_matrix-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `body_matrix-0.4.3/pyproject.toml` & `body_matrix-0.4.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "av>=8.0", "torchvision>=0.13"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "body_matrix"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="Hoang Do", email="hoang.do.2102@gmail.com" },
 ]
 description = "Package to Calculate Human Body Measurements"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `body_matrix-0.4.3/src/body_matrix/draw.py` & `body_matrix-0.4.4/src/body_matrix/draw.py`

 * *Files identical despite different names*

### Comparing `body_matrix-0.4.3/src/body_matrix/export.py` & `body_matrix-0.4.4/src/body_matrix/export.py`

 * *Files identical despite different names*

### Comparing `body_matrix-0.4.3/src/body_matrix/infer.py` & `body_matrix-0.4.4/src/body_matrix/infer.py`

 * *Files identical despite different names*

### Comparing `body_matrix-0.4.3/src/body_matrix/load.py` & `body_matrix-0.4.4/src/body_matrix/load.py`

 * *Files identical despite different names*

### Comparing `body_matrix-0.4.3/src/body_matrix/measure.py` & `body_matrix-0.4.4/src/body_matrix/measure.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     )
 
     selected_kps = process.keypoints_filter(
         [
             'left_eye', 'right_eye',
             'left_ear', 'right_ear',
             'left_shoulder','right_shoulder',
+            'left_elbow', 'right_elbow',
             'left_wrist','right_wrist',
             'left_hip', 'right_hip',
             'left_ankle', 'right_ankle'
         ],  
         keypoints
     )
```

### Comparing `body_matrix-0.4.3/src/body_matrix/process.py` & `body_matrix-0.4.4/src/body_matrix/process.py`

 * *Files identical despite different names*

### Comparing `body_matrix-0.4.3/src/body_matrix/score.py` & `body_matrix-0.4.4/src/body_matrix/score.py`

 * *Files identical despite different names*

### Comparing `body_matrix-0.4.3/src/body_matrix.egg-info/PKG-INFO` & `body_matrix-0.4.4/src/body_matrix.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: body-matrix
-Version: 0.4.3
+Version: 0.4.4
 Summary: Package to Calculate Human Body Measurements
 Author-email: Hoang Do <hoang.do.2102@gmail.com>
 Project-URL: Homepage, https://github.com/akando42/body_matrix
 Project-URL: Bug Tracker, https://github.com/akando42/body_matrix/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

