# Comparing `tmp/prefab-0.2.4.tar.gz` & `tmp/prefab-0.2.5.tar.gz`

## Comparing `prefab-0.2.4.tar` & `prefab-0.2.5.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 prefab-0.2.4/.gitattributes
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 prefab-0.2.4/.pylintrc
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 prefab-0.2.4/requirements.txt
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 prefab-0.2.4/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 prefab-0.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    69100 2020-02-02 00:00:00.000000 prefab-0.2.4/assets/logo.png
--rw-r--r--   0        0        0    67819 2020-02-02 00:00:00.000000 prefab-0.2.4/assets/promo_c.png
--rw-r--r--   0        0        0    74174 2020-02-02 00:00:00.000000 prefab-0.2.4/assets/promo_p.png
--rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/circles-inverse_512x512.png
--rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/circles_512x512.png
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/cross-inverse_16x128_256x256.png
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/cross-inverse_32x128_256x256.png
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/cross-inverse_64x128_256x256.png
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/cross_16x128_256x256.png
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/cross_32x128_256x256.png
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/cross_64x128_256x256.png
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/devices.gds
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/grating_16x256_16_512x512.png
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/grating_16x256_32_512x512.png
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/grating_16x256_64_512x512.png
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/grating_32x256_16_512x512.png
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/grating_32x256_32_512x512.png
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/grating_32x256_64_512x512.png
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/grating_64x256_16_512x512.png
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/grating_64x256_32_512x512.png
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/grating_64x256_64_512x512.png
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/pie_128x128_256x256.png
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/rectangle_128x128_256x256.png
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/ring_64x128_256x256.png
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 prefab-0.2.4/devices/star_128x128_256x256.png
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 prefab-0.2.4/docs/models.md
--rw-r--r--   0        0        0   298400 2020-02-02 00:00:00.000000 prefab-0.2.4/examples/example_ECSE596.ipynb
--rw-r--r--   0        0        0   415994 2020-02-02 00:00:00.000000 prefab-0.2.4/examples/example_prediction.ipynb
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 prefab-0.2.4/prefab/__init__.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 prefab-0.2.4/prefab/io.py
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 prefab-0.2.4/prefab/predictor.py
--rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 prefab-0.2.4/prefab/processor.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 prefab-0.2.4/.gitignore
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 prefab-0.2.4/LICENSE
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 prefab-0.2.4/README.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 prefab-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    35326 2020-02-02 00:00:00.000000 prefab-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 prefab-0.2.5/.gitattributes
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 prefab-0.2.5/.pylintrc
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 prefab-0.2.5/requirements.txt
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 prefab-0.2.5/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 prefab-0.2.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    69100 2020-02-02 00:00:00.000000 prefab-0.2.5/assets/logo.png
+-rw-r--r--   0        0        0    67819 2020-02-02 00:00:00.000000 prefab-0.2.5/assets/promo_c.png
+-rw-r--r--   0        0        0    74174 2020-02-02 00:00:00.000000 prefab-0.2.5/assets/promo_p.png
+-rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/circles-inverse_512x512.png
+-rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/circles_512x512.png
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/cross-inverse_16x128_256x256.png
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/cross-inverse_32x128_256x256.png
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/cross-inverse_64x128_256x256.png
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/cross_16x128_256x256.png
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/cross_32x128_256x256.png
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/cross_64x128_256x256.png
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/devices.gds
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_16x256_16_512x512.png
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_16x256_32_512x512.png
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_16x256_64_512x512.png
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_32x256_16_512x512.png
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_32x256_32_512x512.png
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_32x256_64_512x512.png
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_64x256_16_512x512.png
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_64x256_32_512x512.png
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/grating_64x256_64_512x512.png
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/pie_128x128_256x256.png
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/rectangle_128x128_256x256.png
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/ring_64x128_256x256.png
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 prefab-0.2.5/devices/star_128x128_256x256.png
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 prefab-0.2.5/docs/models.md
+-rw-r--r--   0        0        0   281939 2020-02-02 00:00:00.000000 prefab-0.2.5/examples/example_prediction.ipynb
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 prefab-0.2.5/prefab/__init__.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 prefab-0.2.5/prefab/io.py
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 prefab-0.2.5/prefab/predictor.py
+-rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 prefab-0.2.5/prefab/processor.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 prefab-0.2.5/.gitignore
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 prefab-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 prefab-0.2.5/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 prefab-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    35376 2020-02-02 00:00:00.000000 prefab-0.2.5/PKG-INFO
```

### Comparing `prefab-0.2.4/.github/workflows/python-publish.yml` & `prefab-0.2.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/assets/logo.png` & `prefab-0.2.5/assets/logo.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/assets/promo_c.png` & `prefab-0.2.5/assets/promo_c.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/assets/promo_p.png` & `prefab-0.2.5/assets/promo_p.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/circles-inverse_512x512.png` & `prefab-0.2.5/devices/circles-inverse_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/circles_512x512.png` & `prefab-0.2.5/devices/circles_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/cross-inverse_16x128_256x256.png` & `prefab-0.2.5/devices/cross-inverse_16x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/cross-inverse_32x128_256x256.png` & `prefab-0.2.5/devices/cross-inverse_32x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/cross-inverse_64x128_256x256.png` & `prefab-0.2.5/devices/cross-inverse_64x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/cross_16x128_256x256.png` & `prefab-0.2.5/devices/cross_16x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/cross_32x128_256x256.png` & `prefab-0.2.5/devices/cross_32x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/cross_64x128_256x256.png` & `prefab-0.2.5/devices/cross_64x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/grating_16x256_16_512x512.png` & `prefab-0.2.5/devices/grating_16x256_16_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/grating_16x256_32_512x512.png` & `prefab-0.2.5/devices/grating_16x256_32_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/grating_16x256_64_512x512.png` & `prefab-0.2.5/devices/grating_16x256_64_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/grating_32x256_16_512x512.png` & `prefab-0.2.5/devices/grating_32x256_16_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/grating_32x256_32_512x512.png` & `prefab-0.2.5/devices/grating_32x256_32_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/grating_32x256_64_512x512.png` & `prefab-0.2.5/devices/grating_32x256_64_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/grating_64x256_16_512x512.png` & `prefab-0.2.5/devices/grating_64x256_16_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/grating_64x256_32_512x512.png` & `prefab-0.2.5/devices/grating_64x256_32_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/grating_64x256_64_512x512.png` & `prefab-0.2.5/devices/grating_64x256_64_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/pie_128x128_256x256.png` & `prefab-0.2.5/devices/pie_128x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/rectangle_128x128_256x256.png` & `prefab-0.2.5/devices/rectangle_128x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/ring_64x128_256x256.png` & `prefab-0.2.5/devices/ring_64x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/devices/star_128x128_256x256.png` & `prefab-0.2.5/devices/star_128x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/docs/models.md` & `prefab-0.2.5/docs/models.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,9 +6,11 @@
 | --- | ------- | --------------- | --------- | ----- | ---------------- | ---|
 | ANT | NanoSOI | v1 (Nov 4 2022) | Predictor | Alpha | p_ANT_NanoSOI_v1 | Open |
 | ANT | NanoSOI | v1 (Nov 4 2022) | Corrector | Alpha | c_ANT_NanoSOI_v1 | Open |
 | ANT | NanoSOI | v2 (Jan 9 2023) | Predictor | Beta | p_ANT_NanoSOI_v2 | Open |
 | ANT | NanoSOI | v2 (Jan 9 2023) | Corrector | Beta | c_ANT_NanoSOI_v2 | Open |
 | ANT | NanoSOI | v3 (Mar 5 2023) | Predictor | Beta | p_ANT_NanoSOI_v3 | Open |
 | ANT | NanoSOI | v3 (Mar 5 2023) | Corrector | Beta | c_ANT_NanoSOI_v3 | Open |
+| ANT | NanoSOI | v4 (Apr 12 2023) | Predictor | Beta | p_ANT_NanoSOI_v4 | Open |
+| ANT | NanoSOI | v4 (Apr 12 2023) | Corrector | Beta | c_ANT_NanoSOI_v4 | Open |
 
 *This list will update over time. Usage is subject to change. Please contact us or create an issue if you would like to see a new foundry and process modelled.*
```

### Comparing `prefab-0.2.4/prefab/__init__.py` & `prefab-0.2.5/prefab/__init__.py`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/prefab/io.py` & `prefab-0.2.5/prefab/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,17 @@
     contours = []
     for polygon in polygons:
         contour = []
         for vertex in polygon:
             contour.append([[int(1000*vertex[0] - bounds[0][0]),
                              int(1000*vertex[1] - bounds[0][1])]])
         contours.append(np.array(contour))
-    cv2.drawContours(device, contours, -1, (1, 1, 1), -1)
+
+    for contour in contours:
+        cv2.fillPoly(img=device, pts=[contour], color=(1, 1, 1))
 
     if coords is not None:
         device = device[int(coords[0][1] - bounds[0][1]):
                         int(coords[1][1] - bounds[0][1]),
                         int(coords[0][0] - bounds[0][0]):
                         int(coords[1][0] - bounds[0][0])]
```

### Comparing `prefab-0.2.4/prefab/predictor.py` & `prefab-0.2.5/prefab/predictor.py`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/prefab/processor.py` & `prefab-0.2.5/prefab/processor.py`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/LICENSE` & `prefab-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prefab-0.2.4/README.md` & `prefab-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,30 +18,38 @@
 
 ## Models
 
 Each photonic foundry requires its own *predictor* and *corrector* models. These models are updated regularly based on data from recent fabrication runs. The following models are currently available:
 
 | Foundry | Process | Latest Version (Date) | Type | Status | Name | Usage|
 | --- | ------- | --------------- | --------- | ----- | ---------------- | ---|
-| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v3 (Mar 5 2023) | Predictor | Beta | p_ANT_NanoSOI_v3 | Open |
-| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v3 (Mar 5 2023) | Corrector | Beta | c_ANT_NanoSOI_v3 | Open |
+| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v4 (Apr 12 2023) | Predictor | Beta | p_ANT_NanoSOI_v4 | Open |
+| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v4 (Apr 12 2023) | Corrector | Beta | c_ANT_NanoSOI_v4 | Open |
 
 *This list will update over time. Usage is subject to change. Please contact us or create an issue if you would like to see a new foundry and process modelled.*
 
 ## Installation
 
 ### Local
 
 Install the latest version of `PreFab` locally using:
 
 ```sh
 pip install prefab
 ```
 
-Alternatively, you can clone this repository and then install in development mode using the command `pip install -e .` in its directory. This will allow any changes made to the source code to be reflected in your Python module.
+Alternatively, you can clone this repository and then install in development mode using:
+
+```sh
+git clone https://github.com/PreFab-Photonics/PreFab.git
+cd PreFab
+pip install -e .
+```
+
+This will allow any changes made to the source code to be reflected in your Python module.
 
 ### Online
 
 You can also run the latest version of `PreFab` online by following:
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?machine=basicLinux32gb&repo=608330448&ref=main&devcontainer_path=.devcontainer%2Fdevcontainer.json&location=EastUs)
```

### Comparing `prefab-0.2.4/pyproject.toml` & `prefab-0.2.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "prefab"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
     {name = "Dusan Gostimirovic", email="dusan@prefabphotonics.com"},
 ]
 keywords = ["photonics", "nanofabrication", "machine learning", "layout"]
 description = "Machine learning based prediction of photonic device fabrication"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `prefab-0.2.4/PKG-INFO` & `prefab-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefab
-Version: 0.2.4
+Version: 0.2.5
 Summary: Machine learning based prediction of photonic device fabrication
 Project-URL: Homepage, https://github.com/PreFab-Photonics/PreFab
 Author-email: Dusan Gostimirovic <dusan@prefabphotonics.com>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
@@ -541,30 +541,38 @@
 
 ## Models
 
 Each photonic foundry requires its own *predictor* and *corrector* models. These models are updated regularly based on data from recent fabrication runs. The following models are currently available:
 
 | Foundry | Process | Latest Version (Date) | Type | Status | Name | Usage|
 | --- | ------- | --------------- | --------- | ----- | ---------------- | ---|
-| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v3 (Mar 5 2023) | Predictor | Beta | p_ANT_NanoSOI_v3 | Open |
-| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v3 (Mar 5 2023) | Corrector | Beta | c_ANT_NanoSOI_v3 | Open |
+| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v4 (Apr 12 2023) | Predictor | Beta | p_ANT_NanoSOI_v4 | Open |
+| ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v4 (Apr 12 2023) | Corrector | Beta | c_ANT_NanoSOI_v4 | Open |
 
 *This list will update over time. Usage is subject to change. Please contact us or create an issue if you would like to see a new foundry and process modelled.*
 
 ## Installation
 
 ### Local
 
 Install the latest version of `PreFab` locally using:
 
 ```sh
 pip install prefab
 ```
 
-Alternatively, you can clone this repository and then install in development mode using the command `pip install -e .` in its directory. This will allow any changes made to the source code to be reflected in your Python module.
+Alternatively, you can clone this repository and then install in development mode using:
+
+```sh
+git clone https://github.com/PreFab-Photonics/PreFab.git
+cd PreFab
+pip install -e .
+```
+
+This will allow any changes made to the source code to be reflected in your Python module.
 
 ### Online
 
 You can also run the latest version of `PreFab` online by following:
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?machine=basicLinux32gb&repo=608330448&ref=main&devcontainer_path=.devcontainer%2Fdevcontainer.json&location=EastUs)
```

