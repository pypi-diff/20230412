# Comparing `tmp/pyolaf-0.1.0.tar.gz` & `tmp/pyolaf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyolaf-0.1.0.tar", last modified: Tue Apr 11 19:52:41 2023, max compression
+gzip compressed data, was "pyolaf-0.2.0.tar", last modified: Tue Apr 11 23:49:14 2023, max compression
```

## Comparing `pyolaf-0.1.0.tar` & `pyolaf-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 lili      (1000) lili      (1000)        0 2023-04-11 19:52:41.548221 pyolaf-0.1.0/
--rw-rw-r--   0 lili      (1000) lili      (1000)    11300 2023-04-10 19:39:37.000000 pyolaf-0.1.0/LICENSE
--rw-rw-r--   0 lili      (1000) lili      (1000)     2007 2023-04-11 19:52:41.544221 pyolaf-0.1.0/PKG-INFO
--rw-rw-r--   0 lili      (1000) lili      (1000)     1372 2023-04-11 19:33:26.000000 pyolaf-0.1.0/README.md
-drwxrwxr-x   0 lili      (1000) lili      (1000)        0 2023-04-11 19:52:41.544221 pyolaf-0.1.0/pyolaf/
--rw-rw-r--   0 lili      (1000) lili      (1000)      236 2023-04-11 19:49:09.000000 pyolaf-0.1.0/pyolaf/__init__.py
--rw-rw-r--   0 lili      (1000) lili      (1000)     2905 2023-04-11 19:18:50.000000 pyolaf-0.1.0/pyolaf/aliasing.py
--rw-rw-r--   0 lili      (1000) lili      (1000)     1899 2023-04-11 19:29:52.000000 pyolaf-0.1.0/pyolaf/fftpack.py
--rw-rw-r--   0 lili      (1000) lili      (1000)    34859 2023-04-11 19:15:48.000000 pyolaf-0.1.0/pyolaf/geometry.py
--rw-rw-r--   0 lili      (1000) lili      (1000)    34042 2023-04-11 19:18:59.000000 pyolaf-0.1.0/pyolaf/lf.py
--rw-rw-r--   0 lili      (1000) lili      (1000)    12433 2023-04-11 19:30:31.000000 pyolaf-0.1.0/pyolaf/project.py
--rw-rw-r--   0 lili      (1000) lili      (1000)     2379 2023-04-11 19:20:32.000000 pyolaf-0.1.0/pyolaf/transform.py
-drwxrwxr-x   0 lili      (1000) lili      (1000)        0 2023-04-11 19:52:41.544221 pyolaf-0.1.0/pyolaf.egg-info/
--rw-rw-r--   0 lili      (1000) lili      (1000)     2007 2023-04-11 19:52:41.000000 pyolaf-0.1.0/pyolaf.egg-info/PKG-INFO
--rw-rw-r--   0 lili      (1000) lili      (1000)      301 2023-04-11 19:52:41.000000 pyolaf-0.1.0/pyolaf.egg-info/SOURCES.txt
--rw-rw-r--   0 lili      (1000) lili      (1000)        1 2023-04-11 19:52:41.000000 pyolaf-0.1.0/pyolaf.egg-info/dependency_links.txt
--rw-rw-r--   0 lili      (1000) lili      (1000)       58 2023-04-11 19:52:41.000000 pyolaf-0.1.0/pyolaf.egg-info/requires.txt
--rw-rw-r--   0 lili      (1000) lili      (1000)        7 2023-04-11 19:52:41.000000 pyolaf-0.1.0/pyolaf.egg-info/top_level.txt
--rw-rw-r--   0 lili      (1000) lili      (1000)       38 2023-04-11 19:52:41.548221 pyolaf-0.1.0/setup.cfg
--rw-rw-r--   0 lili      (1000) lili      (1000)     1039 2023-04-11 19:34:30.000000 pyolaf-0.1.0/setup.py
+drwxrwxr-x   0 lili      (1000) lili      (1000)        0 2023-04-11 23:49:14.869633 pyolaf-0.2.0/
+-rw-rw-r--   0 lili      (1000) lili      (1000)    11300 2023-04-10 19:39:37.000000 pyolaf-0.2.0/LICENSE
+-rw-rw-r--   0 lili      (1000) lili      (1000)     2007 2023-04-11 23:49:14.869633 pyolaf-0.2.0/PKG-INFO
+-rw-rw-r--   0 lili      (1000) lili      (1000)     1372 2023-04-11 19:33:26.000000 pyolaf-0.2.0/README.md
+drwxrwxr-x   0 lili      (1000) lili      (1000)        0 2023-04-11 23:49:14.869633 pyolaf-0.2.0/pyolaf/
+-rw-rw-r--   0 lili      (1000) lili      (1000)      236 2023-04-11 23:49:03.000000 pyolaf-0.2.0/pyolaf/__init__.py
+-rw-rw-r--   0 lili      (1000) lili      (1000)     2943 2023-04-11 21:41:27.000000 pyolaf-0.2.0/pyolaf/aliasing.py
+-rw-rw-r--   0 lili      (1000) lili      (1000)     1899 2023-04-11 19:29:52.000000 pyolaf-0.2.0/pyolaf/fftpack.py
+-rw-rw-r--   0 lili      (1000) lili      (1000)    35001 2023-04-11 23:35:03.000000 pyolaf-0.2.0/pyolaf/geometry.py
+-rw-rw-r--   0 lili      (1000) lili      (1000)    34050 2023-04-11 23:45:54.000000 pyolaf-0.2.0/pyolaf/lf.py
+-rw-rw-r--   0 lili      (1000) lili      (1000)    12433 2023-04-11 23:18:28.000000 pyolaf-0.2.0/pyolaf/project.py
+-rw-rw-r--   0 lili      (1000) lili      (1000)     2458 2023-04-11 23:07:15.000000 pyolaf-0.2.0/pyolaf/transform.py
+drwxrwxr-x   0 lili      (1000) lili      (1000)        0 2023-04-11 23:49:14.869633 pyolaf-0.2.0/pyolaf.egg-info/
+-rw-rw-r--   0 lili      (1000) lili      (1000)     2007 2023-04-11 23:49:14.000000 pyolaf-0.2.0/pyolaf.egg-info/PKG-INFO
+-rw-rw-r--   0 lili      (1000) lili      (1000)      301 2023-04-11 23:49:14.000000 pyolaf-0.2.0/pyolaf.egg-info/SOURCES.txt
+-rw-rw-r--   0 lili      (1000) lili      (1000)        1 2023-04-11 23:49:14.000000 pyolaf-0.2.0/pyolaf.egg-info/dependency_links.txt
+-rw-rw-r--   0 lili      (1000) lili      (1000)       69 2023-04-11 23:49:14.000000 pyolaf-0.2.0/pyolaf.egg-info/requires.txt
+-rw-rw-r--   0 lili      (1000) lili      (1000)        7 2023-04-11 23:49:14.000000 pyolaf-0.2.0/pyolaf.egg-info/top_level.txt
+-rw-rw-r--   0 lili      (1000) lili      (1000)       38 2023-04-11 23:49:14.869633 pyolaf-0.2.0/setup.cfg
+-rw-rw-r--   0 lili      (1000) lili      (1000)     1061 2023-04-11 23:48:50.000000 pyolaf-0.2.0/setup.py
```

### Comparing `pyolaf-0.1.0/LICENSE` & `pyolaf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyolaf-0.1.0/PKG-INFO` & `pyolaf-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyolaf
-Version: 0.1.0
+Version: 0.2.0
 Summary: 3D reconstruction framework for light field microscopy
 Home-page: https://github.com/lambdaloop/pyolaf
 Author: Lili Karashchuk
 Author-email: krchtchk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyolaf-0.1.0/README.md` & `pyolaf-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyolaf-0.1.0/pyolaf/aliasing.py` & `pyolaf-0.2.0/pyolaf/aliasing.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,19 +36,19 @@
         lanczos2FFT[:, :, i] = cupy.fft.fft2(lanczos2)
     return lanczos2FFT
 
 def LFM_computeDepthAdaptiveWidth(Camera, Resolution):
 
     ## compute the depth dependent witdth of the anti-aliasing filters
     dz = Resolution["depths"]
-    zobj = Camera["fobj"] - dz
+    zobj = (Camera["fobj"] - dz).astype('float')
 
     # avoid division by zero
     for i in range(len(zobj)):
-        if(zobj[i] == Camera["fobj"] or zobj[i] == Camera["dof"]):
+        if(np.isclose(zobj[i], Camera["fobj"]) or np.isclose(zobj[i], Camera["dof"])):
             zobj[i] = zobj[i] + 0.00001*Camera["fobj"]
 
     # z1 -> where the objective will focus
     z1 = (zobj * Camera["fobj"])/(zobj - Camera["fobj"])
 
     # effective radius of the tube lens
     tubeRad = Camera["objRad"] * Camera["Delta_ot"]*np.abs(1./z1 - 1/Camera["Delta_ot"])
```

### Comparing `pyolaf-0.1.0/pyolaf/fftpack.py` & `pyolaf-0.2.0/pyolaf/fftpack.py`

 * *Files identical despite different names*

### Comparing `pyolaf-0.1.0/pyolaf/geometry.py` & `pyolaf-0.2.0/pyolaf/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
 def LFM_processWhiteImage(WhiteImage, spacingPx, gridType, DebugBuildGridModel):
 
     GridModelOptions = {}
     GridModelOptions['ApproxLensletSpacing'] = spacingPx   # lensPitch / pixelPitch;
     GridModelOptions['Orientation'] = 'horz'
     GridModelOptions['FilterDiskRadiusMult'] = 1/3
-    GridModelOptions['CropAmt'] = 30 # changed from 30, gives better results
+    GridModelOptions['CropAmt'] = 15 # changed from 30, gives better results
     GridModelOptions['SkipStep'] = 10
     GridModelOptions['Precision'] = 'single'
 
     # Find grid params
     LensletGridModel, gridCoords = LFM_BuildLensletGridModel(
         WhiteImage, gridType, GridModelOptions, DebugBuildGridModel )
 
@@ -274,21 +274,27 @@
     if DebugDisplay:
         plt.show(block=False)
 
     #--Trim ends to wipe out alignment, initial estimate artefacts--
     RecPtsY = RecPtsY[3:-3]
     RecPtsX = RecPtsX[3:-3]
 
-    #--Estimate angle--
-    SlopeX = np.mean(LineFitX, axis=0)[0]
-    SlopeY = np.mean(LineFitY, axis=0)[0]
-
-    AngleX = np.arctan2(-SlopeX, 1)
-    AngleY = np.arctan2(SlopeY, 1)
-    EstAngle = np.mean([AngleX, AngleY])
+    #--Estimate angle-
+    possible = []
+    if len(LineFitX) > 0:
+        SlopeX = np.mean(LineFitX, axis=0)[0]
+        AngleX = np.arctan2(-SlopeX, 1)
+        possible.append(AngleX)
+
+    if len(LineFitY) > 0:
+        SlopeY = np.mean(LineFitY, axis=0)[0]
+        AngleY = np.arctan2(SlopeY, 1)
+        possible.append(AngleY)
+
+    EstAngle = np.mean(possible)
 
     #--Estimate spacing, assuming approx zero angle--
     # t = RecPtsY[:,:,1]
     # YSpacing = np.mean(np.diff(t, axis=1))/2 / (np.sqrt(3)/2)
     YSpacing = np.mean([np.mean(np.diff(row[:,1]))
                         for row in RecPtsY]) /2 / (np.sqrt(3)/2)
```

### Comparing `pyolaf-0.1.0/pyolaf/lf.py` & `pyolaf-0.2.0/pyolaf/lf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 import numpy as np
 import time
+from tqdm import trange
 
 def LFM_computePSFsize(maxDepth, Camera):
     ## geometric blur radius at the MLA
     maxDepth = maxDepth - Camera["offsetFobj"]
     zobj = Camera["fobj"] - maxDepth
     # avoid division by zero
     if(zobj == Camera["fobj"] or zobj == Camera["dof"]):
@@ -362,17 +363,16 @@
 
     Nnum_half_coord = Resolution['TexNnum_half'] // Resolution['texScaleFactor']
     sensorRes = Resolution['sensorRes']
 
     # Resolution['texScaleFactor(1/2)'] is actually (Resolution['texRes(1/2)'] * M / Resolution['sensorRes(1/2)'])^-1
     H = np.empty((coordsRange[0], coordsRange[1], len(Resolution['depths'])),
                  dtype='object')
-    for c in range(len(Resolution['depths'])):
-        print('Forward Patterns, depth:', c+1, '/', len(Resolution['depths']))
-
+    for c in trange(len(Resolution['depths']), ncols=70, desc=' forward patterns'):
+        # print('Forward Patterns, depth:', c+1, '/', len(Resolution['depths']))
         psfREF = psfWaveStack[:,:,c]
         for i in range(coordsRange[0]):
             for j in range(coordsRange[1]):
                 aa_tex = i+1
                 aa_sensor = aa_tex / Resolution['texScaleFactor'][0]
                 bb_tex = j+1
                 bb_sensor = bb_tex / Resolution['texScaleFactor'][1]
@@ -439,37 +439,33 @@
 
     # compute backprojection patterns for all the pixels in coordsRange
     Ht = np.empty((coordsRange[0], coordsRange[1], nDepths), dtype='object')  # container for back projection patterns
 
     # Iterate through every pixel behind the central micro-lens and compute
     # which part of the texture (object) affects it.
 
-    for aa_sensor in range(coordsRange[0]):
-        print('Backward patterns, x: {}/{}'.format(aa_sensor+1, coordsRange[0]))
+    for aa_sensor in trange(coordsRange[0], ncols=70, desc='backward patterns'):
+        # print('Backward patterns, x: {}/{}'.format(aa_sensor+1, coordsRange[0]))
         aa_tex = np.ceil((1+aa_sensor) * Resolution["texScaleFactor"][0]).astype(int)  # compute the corresponding coord of "aa_sensor" pixel in real world space
         for bb_sensor in range(coordsRange[1]):
             bb_tex = np.ceil((1+bb_sensor) * Resolution["texScaleFactor"][1]).astype(int)  # compute the corresponding coord of "bb_sensor" pixel in real world space
 
             # backproject the activated sensor pixel
             currentPixel = [aa_sensor + offsetImg[0] - Resolution["Nnum_half"][0],
                             bb_sensor + offsetImg[1] - Resolution["Nnum_half"][1]]  # position of the current active pixel in the image
             tempback = LFM_backwardProjectSinglePoint(H, Resolution, imgSize, texSize, currentPixel, lensletCenters, crange, lensOrder)
 
             # bring the backprojection to center (the operator assumes the bproj patterns are centered when applying them)
-            tempbackShift = [None]*nDepths
             for cc in range(nDepths):
                 backShiftX = np.round(Resolution["TexNnum_half"][0]-aa_tex).astype(int)
                 backShiftY = np.round(Resolution["TexNnum_half"][1]-bb_tex).astype(int)
                 shifted = imShift2(tempback[:,:,cc], backShiftX, backShiftY)
-                tempbackShift[cc] = csr_matrix(shifted)
                 # store the pattern
                 Ht[(aa_sensor,bb_sensor, cc)] = csr_matrix(shifted)
 
-            # store the pattern
-            # Ht[(aa_sensor,bb_sensor, cc)] = csr_matrix(tempbackShift)
 
 
     return Ht
 
 
 
 
@@ -630,22 +626,25 @@
 
 def normalizeHt(Ht):
     # Ht_sizes = np.max(list(Ht.keys()), axis=0) + 1
     Ht_sizes = Ht.shape
 
     for aa in range(Ht_sizes[0]):
         for bb in range(Ht_sizes[1]):
-            temp = np.concatenate(
-                [Ht[aa, bb, cc].todense() for cc in range(Ht_sizes[2])],
-                axis=1)
-            sum_temp = np.sum(temp)
+            sum_temp = 0
+            for c in range(Ht_sizes[2]):
+                sum_temp += Ht[aa, bb, c].sum()
+            # temp = np.concatenate(
+            #     [Ht[aa, bb, cc].toarray() for cc in range(Ht_sizes[2])],
+            #     axis=1)
+            # sum_temp = np.sum(temp)
             if np.isclose(sum_temp, 0):
                 continue
             for c in range(Ht_sizes[2]):
-                Ht[aa, bb, c] = csr_matrix(Ht[aa, bb, c] / sum_temp)
+                Ht[aa, bb, c] = Ht[aa, bb, c] / sum_temp
 
     return Ht
 
 def ignoreSmallVals(H, tol):
     for a in range(H.shape[0]):
         for b in range(H.shape[1]):
             for c in range(H.shape[2]):
```

### Comparing `pyolaf-0.1.0/pyolaf/project.py` & `pyolaf-0.2.0/pyolaf/project.py`

 * *Files identical despite different names*

### Comparing `pyolaf-0.1.0/pyolaf/transform.py` & `pyolaf-0.2.0/pyolaf/transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,18 @@
 
 
 def transform_img(img, ttnew, lens_offset):
     scale = np.diag(ttnew)[:2]
     new_shape = np.floor(np.round(img.shape / scale) / 2) * 2 + 1
     new_shape = new_shape.astype('int32')
     offset = np.ceil(new_shape / 2) - lens_offset
+    # this transformation has some discrepancy to matlab code
+    # it's the biggest discrepancy across the pipeline
     new = affine_transform(img, cupy.asarray(ttnew[:2, :2]),
-                           offset=ttnew[:2,2] / 3.0, # smaller error if divide by 3?
+                           offset=ttnew[:2,2],
                            output_shape=tuple(new_shape),
                            order=1, prefilter=False)
     # new = affine_transform(new, cupy.eye(2), offset=[-offset[0], -offset[1]], order=1)
     new = shift(new, [offset[0], offset[1]], order=1, prefilter=False)
     new[new < np.mean(new)] = np.mean(new)
     return new
```

### Comparing `pyolaf-0.1.0/pyolaf.egg-info/PKG-INFO` & `pyolaf-0.2.0/pyolaf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyolaf
-Version: 0.1.0
+Version: 0.2.0
 Summary: 3D reconstruction framework for light field microscopy
 Home-page: https://github.com/lambdaloop/pyolaf
 Author: Lili Karashchuk
 Author-email: krchtchk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyolaf-0.1.0/setup.py` & `pyolaf-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyolaf",
-    version="0.1.0",
+    version="0.2.0",
     author="Lili Karashchuk",
     author_email="krchtchk@gmail.com",
     description="3D reconstruction framework for light field microscopy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lambdaloop/pyolaf",
     packages=setuptools.find_packages(),
@@ -25,14 +25,15 @@
     ],
     install_requires=[
         'pyyaml',
         'numpy',
         'scipy',
         'tqdm',
         'tifffile',
-        'scikit-image'
+        'scikit-image',
+        'matplotlib'
     ],
     extras_require={
         'gpu':  ["cupy"]
     }
 
 )
```

