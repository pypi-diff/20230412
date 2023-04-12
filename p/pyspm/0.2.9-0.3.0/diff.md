# Comparing `tmp/pySPM-0.2.9.tar.gz` & `tmp/pyspm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pySPM-0.2.9.tar", last modified: Thu Nov  1 16:36:21 2018, max compression
+gzip compressed data, was "pyspm-0.3.0.tar", max compression
```

## Comparing `pySPM-0.2.9.tar` & `pyspm-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,51 @@
-drwxrwxrwx   0        0        0        0 2018-11-01 16:36:21.000000 pySPM-0.2.9/
--rw-rw-rw-   0        0        0     2371 2018-11-01 16:36:21.000000 pySPM-0.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2018-11-01 16:36:21.000000 pySPM-0.2.9/pySPM/
--rw-rw-rw-   0        0        0    10513 2018-09-06 12:33:52.000000 pySPM-0.2.9/pySPM/align.py
--rw-rw-rw-   0        0        0    23405 2018-10-30 09:03:26.000000 pySPM-0.2.9/pySPM/Block.py
--rw-rw-rw-   0        0        0     5329 2018-09-12 14:26:53.000000 pySPM-0.2.9/pySPM/Bruker.py
--rw-rw-rw-   0        0        0     9608 2018-11-01 14:19:01.000000 pySPM-0.2.9/pySPM/collection.py
--rw-rw-rw-   0        0        0     1219 2018-01-16 13:04:44.000000 pySPM-0.2.9/pySPM/GUI.py
--rw-rw-rw-   0        0        0    35260 2018-11-01 15:16:58.000000 pySPM-0.2.9/pySPM/ITA.py
--rw-rw-rw-   0        0        0     7001 2018-01-16 13:04:44.000000 pySPM-0.2.9/pySPM/ITAslicer.py
--rw-rw-rw-   0        0        0     3875 2018-10-01 15:01:39.000000 pySPM-0.2.9/pySPM/ITAX.py
--rw-rw-rw-   0        0        0    41102 2018-11-01 13:58:34.000000 pySPM-0.2.9/pySPM/ITM.py
--rw-rw-rw-   0        0        0      806 2018-01-16 13:04:44.000000 pySPM-0.2.9/pySPM/ITS.py
--rw-rw-rw-   0        0        0     1140 2018-01-16 13:04:44.000000 pySPM-0.2.9/pySPM/mplwidget.py
--rw-rw-rw-   0        0        0     8110 2018-09-12 08:29:30.000000 pySPM-0.2.9/pySPM/nanoscan.py
--rw-rw-rw-   0        0        0     7223 2018-09-06 10:42:00.000000 pySPM-0.2.9/pySPM/PCA.py
--rw-rw-rw-   0        0        0     5203 2017-11-22 10:40:38.000000 pySPM-0.2.9/pySPM/slicer.py
--rw-rw-rw-   0        0        0    69730 2018-11-01 15:44:35.000000 pySPM-0.2.9/pySPM/SPM.py
--rw-rw-rw-   0        0        0     2748 2018-09-12 08:44:14.000000 pySPM-0.2.9/pySPM/SXM.py
--rw-rw-rw-   0        0        0     7804 2018-01-16 13:04:44.000000 pySPM-0.2.9/pySPM/ToF.py
-drwxrwxrwx   0        0        0        0 2018-11-01 16:36:21.000000 pySPM-0.2.9/pySPM/utils/
--rw-rw-rw-   0        0        0      379 2018-11-01 14:30:39.000000 pySPM-0.2.9/pySPM/utils/constants.py
--rw-rw-rw-   0        0        0     7114 2018-10-30 15:39:08.000000 pySPM-0.2.9/pySPM/utils/elts.py
--rw-rw-rw-   0        0        0    10848 2018-04-18 09:32:57.000000 pySPM-0.2.9/pySPM/utils/fit.py
--rw-rw-rw-   0        0        0     1611 2018-10-01 15:01:34.000000 pySPM-0.2.9/pySPM/utils/haar.py
--rw-rw-rw-   0        0        0     8022 2018-08-28 11:47:18.000000 pySPM-0.2.9/pySPM/utils/math.py
--rw-rw-rw-   0        0        0     1043 2018-09-24 11:56:36.000000 pySPM-0.2.9/pySPM/utils/misc.py
--rw-rw-rw-   0        0        0    13588 2018-10-01 15:01:29.000000 pySPM-0.2.9/pySPM/utils/plot.py
--rw-rw-rw-   0        0        0     8853 2018-10-01 15:01:34.000000 pySPM-0.2.9/pySPM/utils/restoration.py
--rw-rw-rw-   0        0        0     6019 2018-06-26 14:10:09.000000 pySPM-0.2.9/pySPM/utils/save.py
--rw-rw-rw-   0        0        0     8597 2018-11-01 16:28:40.000000 pySPM-0.2.9/pySPM/utils/spectra.py
--rw-rw-rw-   0        0        0     6810 2018-10-31 09:13:49.000000 pySPM-0.2.9/pySPM/utils/units.py
--rw-rw-rw-   0        0        0     5942 2018-10-31 08:48:43.000000 pySPM-0.2.9/pySPM/utils/__init__.py
--rw-rw-rw-   0        0        0      721 2018-11-01 16:01:32.000000 pySPM-0.2.9/pySPM/__init__.py
-drwxrwxrwx   0        0        0        0 2018-11-01 16:36:21.000000 pySPM-0.2.9/pySPM.egg-info/
--rw-rw-rw-   0        0        0        1 2018-11-01 16:36:21.000000 pySPM-0.2.9/pySPM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2371 2018-11-01 16:36:21.000000 pySPM-0.2.9/pySPM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       56 2018-11-01 16:36:21.000000 pySPM-0.2.9/pySPM.egg-info/requires.txt
--rw-rw-rw-   0        0        0      695 2018-11-01 16:36:21.000000 pySPM-0.2.9/pySPM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        6 2018-11-01 16:36:21.000000 pySPM-0.2.9/pySPM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3632 2018-10-23 07:53:15.000000 pySPM-0.2.9/README.md
--rw-rw-rw-   0        0        0       42 2018-11-01 16:36:21.000000 pySPM-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1433 2018-09-24 18:18:58.000000 pySPM-0.2.9/setup.py
+-rw-r--r--   0        0        0    11346 2023-04-12 14:13:51.314971 pyspm-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5343 2023-04-12 17:37:24.162737 pyspm-0.3.0/README.md
+-rw-r--r--   0        0        0    33526 2023-04-12 17:36:52.462238 pyspm-0.3.0/pySPM/Block.py
+-rw-r--r--   0        0        0     7145 2023-04-12 17:36:52.462580 pyspm-0.3.0/pySPM/Bruker.py
+-rw-r--r--   0        0        0    42257 2023-04-12 17:36:52.463051 pyspm-0.3.0/pySPM/ITA.py
+-rw-r--r--   0        0        0     3957 2023-04-12 17:36:52.463347 pyspm-0.3.0/pySPM/ITAX.py
+-rw-r--r--   0        0        0     6743 2023-04-12 17:36:52.463628 pyspm-0.3.0/pySPM/ITAslicer.py
+-rw-r--r--   0        0        0    59689 2023-04-12 17:36:52.464199 pyspm-0.3.0/pySPM/ITM.py
+-rw-r--r--   0        0        0      717 2023-04-12 17:36:52.464465 pyspm-0.3.0/pySPM/ITS.py
+-rw-r--r--   0        0        0     8086 2023-04-12 17:36:52.464722 pyspm-0.3.0/pySPM/PCA.py
+-rw-r--r--   0        0        0    71724 2023-04-12 17:36:52.465564 pyspm-0.3.0/pySPM/SPM.py
+-rw-r--r--   0        0        0     2930 2023-04-12 17:36:52.465873 pyspm-0.3.0/pySPM/SXM.py
+-rw-r--r--   0        0        0     7676 2023-04-12 17:36:52.466198 pyspm-0.3.0/pySPM/ToF.py
+-rw-r--r--   0        0        0      523 2023-04-12 17:36:52.466513 pyspm-0.3.0/pySPM/__init__.py
+-rw-r--r--   0        0        0     1719 2023-04-12 17:36:52.466745 pyspm-0.3.0/pySPM/__main__.py
+-rw-r--r--   0        0        0    10604 2023-04-12 17:36:52.466990 pyspm-0.3.0/pySPM/align.py
+-rw-r--r--   0        0        0     9747 2023-04-12 17:36:52.467236 pyspm-0.3.0/pySPM/collection.py
+-rw-r--r--   0        0        0   376832 2023-04-12 14:13:51.414468 pyspm-0.3.0/pySPM/data/elements.db
+-rw-r--r--   0        0        0     1147 2023-04-12 17:36:52.467445 pyspm-0.3.0/pySPM/mplwidget.py
+-rw-r--r--   0        0        0     8486 2023-04-12 17:36:52.467680 pyspm-0.3.0/pySPM/nanoscan.py
+-rw-r--r--   0        0        0     5092 2023-04-12 17:36:52.467906 pyspm-0.3.0/pySPM/slicer.py
+-rw-r--r--   0        0        0        0 2023-04-12 14:13:51.414758 pyspm-0.3.0/pySPM/tools/__init__.py
+-rw-r--r--   0        0        0     1947 2023-04-12 17:36:52.468184 pyspm-0.3.0/pySPM/tools/emission_current_plotter.py
+-rw-r--r--   0        0        0     3028 2023-04-12 17:36:52.468402 pyspm-0.3.0/pySPM/tools/fpanel.py
+-rw-r--r--   0        0        0     1066 2023-04-12 17:36:52.468603 pyspm-0.3.0/pySPM/tools/mplwidget.py
+-rw-r--r--   0        0        0    12108 2023-04-12 17:36:52.468868 pyspm-0.3.0/pySPM/tools/spectra.py
+-rw-r--r--   0        0        0     5605 2023-04-12 17:36:52.469091 pyspm-0.3.0/pySPM/tools/spectraviewer.py
+-rw-r--r--   0        0        0     6760 2023-04-12 17:36:52.469324 pyspm-0.3.0/pySPM/tools/spectraviewer.ui
+-rw-r--r--   0        0        0     2532 2023-04-12 17:36:52.469530 pyspm-0.3.0/pySPM/tools/stability.py
+-rw-r--r--   0        0        0     1969 2023-04-12 17:36:52.469773 pyspm-0.3.0/pySPM/tools/timer_display.py
+-rw-r--r--   0        0        0     1830 2023-04-12 17:36:52.470003 pyspm-0.3.0/pySPM/tools/timer_display.ui
+-rw-r--r--   0        0        0     1793 2023-04-12 17:36:52.470238 pyspm-0.3.0/pySPM/tools/tof_timer.py
+-rw-r--r--   0        0        0     1177 2023-04-12 14:13:51.415480 pyspm-0.3.0/pySPM/tools/values_display.py
+-rw-r--r--   0        0        0     8071 2023-04-12 17:36:52.470567 pyspm-0.3.0/pySPM/tools/win32_helper.py
+-rw-r--r--   0        0        0     7316 2023-04-12 17:36:52.470807 pyspm-0.3.0/pySPM/utils/__init__.py
+-rw-r--r--   0        0        0      260 2023-04-12 17:36:52.470999 pyspm-0.3.0/pySPM/utils/colors.py
+-rw-r--r--   0        0        0      364 2023-04-12 17:36:52.471193 pyspm-0.3.0/pySPM/utils/constants.py
+-rw-r--r--   0        0        0    13816 2023-04-12 17:36:52.471547 pyspm-0.3.0/pySPM/utils/elts.py
+-rw-r--r--   0        0        0    11350 2023-04-12 17:36:52.471840 pyspm-0.3.0/pySPM/utils/fit.py
+-rw-r--r--   0        0        0     2839 2023-04-12 17:36:52.472100 pyspm-0.3.0/pySPM/utils/geometry.py
+-rw-r--r--   0        0        0     1578 2023-04-12 17:36:52.472316 pyspm-0.3.0/pySPM/utils/haar.py
+-rw-r--r--   0        0        0    10108 2023-04-12 17:36:52.472596 pyspm-0.3.0/pySPM/utils/math.py
+-rw-r--r--   0        0        0     5152 2023-04-12 17:36:52.472845 pyspm-0.3.0/pySPM/utils/misc.py
+-rw-r--r--   0        0        0    15083 2023-04-12 17:36:52.473186 pyspm-0.3.0/pySPM/utils/plot.py
+-rw-r--r--   0        0        0      877 2023-04-12 17:36:52.473397 pyspm-0.3.0/pySPM/utils/progressbar.py
+-rw-r--r--   0        0        0     6921 2023-04-12 17:36:52.473642 pyspm-0.3.0/pySPM/utils/restoration.py
+-rw-r--r--   0        0        0     6250 2023-04-12 17:36:52.473876 pyspm-0.3.0/pySPM/utils/save.py
+-rw-r--r--   0        0        0    16421 2023-04-12 17:36:52.474234 pyspm-0.3.0/pySPM/utils/spectra.py
+-rw-r--r--   0        0        0     6834 2023-04-12 17:36:52.474471 pyspm-0.3.0/pySPM/utils/units.py
+-rw-r--r--   0        0        0      936 2023-04-12 17:36:52.474602 pyspm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6649 1970-01-01 00:00:00.000000 pyspm-0.3.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pySPM-0.2.9/pySPM/align.py` & `pyspm-0.3.0/pySPM/align.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,31 +7,32 @@
 Usually one from an SPM and the other from the ToF-SIMS.
 
 This module also gives the ability to perform shift correction on images
 which is used in order to align the different scans from ToF-SIMS images.
 """
 
 from __future__ import print_function
+
 import numpy as np
+from scipy.ndimage import gaussian_filter
 from skimage import transform as tf
-from scipy.ndimage.filters import gaussian_filter
 
 
 class Aligner:
     def __init__(self, fixed, other, prog=True, FFT=True):
         self.fixed = np.copy(fixed)
         self.other = np.copy(other)
         self.size = fixed.shape
-        self. FFT = FFT
+        self.FFT = FFT
         self.trans = [0, 0]
         self.scale = [1, 1]
         self.rotation = 0
 
         self.initIDX = self.getMatchingIndex()
-    
+
     def compute(self, prog=False):
         # Compute the correlation to find the best shift as first guess
         if prog:
             print("Progress [1/4] Improve Shift...", end='\r')
         self.ImproveShift()
         if prog:
             print("Progress [2/6] Improve Scale X...", end='\r')
@@ -49,158 +50,164 @@
             print("Progress [6/6] Improve Scale Y...", end='\r')
         self.ImproveScaleY()
         if prog:
             print("", end='\r')
 
     def ImproveShift(self, verbose=False, **kargs):
         tform = tf.AffineTransform(
-            scale=self.scale, rotation=self.rotation, translation=(0,0))
-        
+            scale=self.scale, rotation=self.rotation, translation=(0, 0))
+
         O = tf.warp(self.other, tform, output_shape=self.other.shape, preserve_range=True)
         if self.FFT:
             Corr = np.real(np.fft.fftshift(np.fft.ifft2(
-                np.conj(np.fft.fft2(self.fixed))*np.fft.fft2(O))))
+                np.conj(np.fft.fft2(self.fixed)) * np.fft.fft2(O))))
             cord = np.unravel_index(np.argmax(Corr), self.fixed.shape)
-            self.trans = [cord[1]-self.size[0]/2, cord[0]-self.size[1]/2]
+            self.trans = [cord[1] - self.size[0] / 2, cord[0] - self.size[1] / 2]
         else:
-            shift, D = AutoShift(self.fixed, O, shift=[-self.trans[0], self.trans[1]],**kargs)
+            shift, D = AutoShift(self.fixed, O, shift=[-self.trans[0], self.trans[1]], **kargs)
             if verbose:
-                print("ImproveShift",shift,D)
+                print("ImproveShift", shift, D)
             self.trans = [-shift[0], shift[1]]
 
     def getTf(self, verbose=False):
         """
         Get the Afdfine transform.
         You can apply it to a pySPM Image (img) with: img.align(this.getTf())
         """
         if verbose:
             print("Transpose: {0[0]}, {0[1]}".format(self.trans))
         return tf.AffineTransform(scale=self.scale, rotation=self.rotation, translation=self.trans)
 
     def getMatchingIndex(self, power=1):
-        img = tf.warp(self.other, self.getTf(), output_shape=self.other.shape, preserve_range=True)[:self.fixed.shape[0],:self.fixed.shape[1]]
-        return np.sum(np.abs(self.fixed-img)**power)
+        img = tf.warp(self.other, self.getTf(), output_shape=self.other.shape, preserve_range=True)[
+              :self.fixed.shape[0], :self.fixed.shape[1]]
+        return np.sum(np.abs(self.fixed - img) ** power)
 
     def ImproveScaleX(self, fact=.1, count=0, verbose=False):
         old = self.scale
         IDX1 = self.getMatchingIndex()
-        self.scale[0] *= 1+fact
+        self.scale[0] *= 1 + fact
         self.ImproveShift()
         IDX2 = self.getMatchingIndex()
-        print("ImproveX",count, IDX1, IDX2)
+        print("ImproveX", count, IDX1, IDX2)
         if IDX2 > IDX1:
-            self.scale[0] = old[0]*(1-fact)
+            self.scale[0] = old[0] * (1 - fact)
             self.ImproveShift()
             IDX2 = self.getMatchingIndex()
             if IDX2 > IDX1:
                 self.scale[0] = old[0]
                 if fact > 1e-3:
                     self.ImproveScaleY(fact)
             elif count <= 11:
-                self.ImproveScaleX(fact, count+1)
+                self.ImproveScaleX(fact, count + 1)
         elif count <= 11:
-            self.ImproveScaleX(fact, count+1)
+            self.ImproveScaleX(fact, count + 1)
 
     def ImproveRotation(self, delta=.1, count=0, prog=False):
         IDX1 = self.getMatchingIndex()
         IDX2 = IDX1
         init = self.rotation
         if prog:
             print("Progress [{i}/4] Improve Rotation. Passes: {count} (max 11)".format(
-                i=prog, count=count+1), end='\r')
+                i=prog, count=count + 1), end='\r')
         while IDX2 <= IDX1:
             IDX1 = IDX2
             count += 1
             self.rotation += delta
             self.ImproveShift()
             IDX2 = self.getMatchingIndex()
         self.rotation -= delta
         if delta > 0:
-            self.ImproveRotation(-delta, count=count+1)
+            self.ImproveRotation(-delta, count=count + 1)
         elif abs(delta) > 1e-5:
-            self.ImproveRotation(abs(delta)/10., count=count+1)
+            self.ImproveRotation(abs(delta) / 10., count=count + 1)
 
     def ImproveScaleY(self, fact=.1, count=0):
         old = self.scale
         IDX1 = self.getMatchingIndex()
-        self.scale[1] *= 1+fact
+        self.scale[1] *= 1 + fact
         self.ImproveShift()
         IDX2 = self.getMatchingIndex()
         if IDX2 > IDX1:
-            self.scale[1] = old[1]*(1-fact)
+            self.scale[1] = old[1] * (1 - fact)
             self.ImproveShift()
             IDX2 = self.getMatchingIndex()
             if IDX2 > IDX1:
                 self.scale[1] = old[1]
                 if fact > 1e-3:
-                    self.ImproveScaleX(fact/10)
+                    self.ImproveScaleX(fact / 10)
             elif count <= 11:
-                self.ImproveScaleY(fact, count+1)
+                self.ImproveScaleY(fact, count + 1)
         elif count <= 11:
-            self.ImproveScaleY(fact, count+1)
+            self.ImproveScaleY(fact, count + 1)
 
     def __repr__(self):
-        return u"Scale: ({scale[0]},{scale[1]})\nRotation: {rot:.6f} deg.\nTranslation: ({trans[0]},{trans[1]})".format(rot=self.rotation, scale=self.scale, trans=self.trans)
+        return u"Scale: ({scale[0]},{scale[1]})\nRotation: {rot:.6f} deg.\nTranslation: ({trans[0]},{trans[1]})".format(
+            rot=self.rotation, scale=self.scale, trans=self.trans)
+
 
 def ApplyShift(Img, shift):
     dx, dy = [-int(x) for x in shift]
-    return np.pad(Img,((max(0,dy),max(0,-dy)),(max(0,-dx),max(0,dx))),
-                mode='constant', constant_values=0)[max(0,-dy):max(0,-dy)+Img.shape[0],
-                                                    max(0,dx):max(0,dx)+Img.shape[1]]
-def ShiftScore(Ref, Img,  shift, gauss = 5, mean=True, norm=False, debug=False, normData=False):
+    return np.pad(Img, ((max(0, dy), max(0, -dy)), (max(0, -dx), max(0, dx))),
+                  mode='constant', constant_values=0)[max(0, -dy):max(0, -dy) + Img.shape[0],
+           max(0, dx):max(0, dx) + Img.shape[1]]
+
+
+def ShiftScore(Ref, Img, shift, gauss=5, mean=True, norm=False, debug=False, normData=False):
     assert Ref.shape[0] <= Img.shape[0]
     assert Ref.shape[1] <= Img.shape[1]
     if mean:
         Ref = Ref - np.mean(Ref)
         Img = Img - np.mean(Img)
     if normData:
-       assert np.std(Ref)>0
-       assert np.std(Img)>0
-       Ref /= np.std(Ref)
-       Img /= np.std(Img)
+        assert np.std(Ref) > 0
+        assert np.std(Img) > 0
+        Ref /= np.std(Ref)
+        Img /= np.std(Img)
     # blur the images for score calculation
-    if gauss in [0,None,False]:
+    if gauss in [0, None, False]:
         im1 = Ref
         im2 = Img
     else:
-        im1 = gaussian_filter( Ref, gauss)
-        im2 = gaussian_filter( Img, gauss)
-        
+        im1 = gaussian_filter(Ref, gauss)
+        im2 = gaussian_filter(Img, gauss)
+
     corr2 = ApplyShift(im2, shift)
     dx, dy = shift
     # Create a copy of the reference and erase parts which are not overlaping with img
     DSX = Img.shape[1] - Ref.shape[1]
     DSY = Img.shape[0] - Ref.shape[0]
     Or = np.copy(im1)
     if dy < 0:
         Or[:-dy, :] = 0
-    elif DSY-dy < 0:
-        Or[DSY-dy:, :] = 0
+    elif DSY - dy < 0:
+        Or[DSY - dy:, :] = 0
     if dx > 0:
         Or[:, :dx] = 0
-    elif DSX+dx < 0:
-        Or[:, dx+DSX:] = 0
-        
-    corr2 = corr2[:Ref.shape[0],:Ref.shape[1]]
+    elif DSX + dx < 0:
+        Or[:, dx + DSX:] = 0
+
+    corr2 = corr2[:Ref.shape[0], :Ref.shape[1]]
     # calculate the score: absolute of the differendces normed by the overlaping area
-    D = np.sum(np.abs( Or - corr2 ))
+    D = np.sum(np.abs(Or - corr2))
     if norm:
-        D /= ((Ref.shape[0]-2*dy)*(Ref.shape[1]-2*dx))
+        D /= ((Ref.shape[0] - 2 * dy) * (Ref.shape[1] - 2 * dx))
     if debug:
         return D, Or, corr2
     return D
 
-def AutoShift(Ref, Img, Delta = 50, shift=(0,0), step=5, gauss=5, mean=True, test=False, norm=False, normData=False):
+
+def AutoShift(Ref, Img, Delta=50, shift=(0, 0), step=5, gauss=5, mean=True, test=False, norm=False, normData=False):
     """Function to find the best shift between two images by using brute force
     It shift the two iumages and calculate a difference score between the two.
     The function will return the shift which gives the lowerst score (least difference)
     The score is the norm of the difference between the two images where all non-overlaping parts of the images
     due to the shifts are set to 0. The score is then normes by the effective area.
     In order to avoid the errors due to shot-noise, the images are gaussian blured.
-  
+
     Delta: shifts between shift[0/1]-Delta and shift[0/1]+Delta will be tested
     step: The step between tested delta values
     gauss: For noisy image it is better to use a gaussian filter in order to improve the score accuracy.
            The value is the gaussian size.
     mean: If True, the mean value of each image are subtracted. This is prefered when the intensities of the two images does not match perfectly.
           Set it to False if you know that the intensities of your two images are identical
     Note: This function was developed as the maximum in FFT correlation does not seems to give very acurate
@@ -211,55 +218,55 @@
     """
     assert Ref.shape[0] <= Img.shape[0]
     assert Ref.shape[1] <= Img.shape[1]
     if mean:
         Ref = Ref - np.mean(Ref)
         Img = Img - np.mean(Img)
     if normData:
-       assert np.std(Ref)>0
-       assert np.std(Img)>0
-       Ref /= np.std(Ref)
-       Img /= np.std(Img)
+        assert np.std(Ref) > 0
+        assert np.std(Img) > 0
+        Ref /= np.std(Ref)
+        Img /= np.std(Img)
     # blur the images for score calculation
-    if gauss in [0,None,False]:
+    if gauss in [0, None, False]:
         im1 = Ref
         im2 = Img
     else:
-        im1 = gaussian_filter( Ref, gauss)
-        im2 = gaussian_filter( Img, gauss)
-        
+        im1 = gaussian_filter(Ref, gauss)
+        im2 = gaussian_filter(Img, gauss)
+
     # the following two variables save the best score
-    best = (0,0)
-    Dbest = Ref.shape[0]*Ref.shape[1]*max(np.max(im2),np.max(im1))
-    
-    tested = np.zeros((int(2*Delta/step)+1,int(2*Delta/step)+1))
+    best = (0, 0)
+    Dbest = Ref.shape[0] * Ref.shape[1] * max(np.max(im2), np.max(im1))
+
+    tested = np.zeros((int(2 * Delta / step) + 1, int(2 * Delta / step) + 1))
     # Sweep through all possible shifts (brute force)
-    for iy,Dy in enumerate(np.arange(shift[1]-Delta, shift[1]+Delta+1, step)):
+    for iy, Dy in enumerate(np.arange(shift[1] - Delta, shift[1] + Delta + 1, step)):
         dy = int(Dy)
-        for ix,Dx in enumerate(np.arange(shift[0]-Delta, shift[0]+Delta+1, step)):
+        for ix, Dx in enumerate(np.arange(shift[0] - Delta, shift[0] + Delta + 1, step)):
             dx = int(Dx)
-            corr2 = ApplyShift(im2, (dx,dy))
+            corr2 = ApplyShift(im2, (dx, dy))
             DSX = Img.shape[1] - Ref.shape[1]
             DSY = Img.shape[0] - Ref.shape[0]
             # Create a copy of the reference and erase parts which are not overlaping with img
             Or = np.copy(im1)
             if dy < 0:
                 Or[:-dy, :] = 0
-            elif DSY-dy < 0:
-                Or[DSY-dy:, :] = 0
+            elif DSY - dy < 0:
+                Or[DSY - dy:, :] = 0
             if dx > 0:
                 Or[:, :dx] = 0
-            elif DSX+dx < 0:
-                Or[:, dx+DSX:] = 0
-            corr2 = corr2[:Ref.shape[0],:Ref.shape[1]]
+            elif DSX + dx < 0:
+                Or[:, dx + DSX:] = 0
+            corr2 = corr2[:Ref.shape[0], :Ref.shape[1]]
             # calculate the score: absolute of the differendces normed by the overlaping area
-            D = np.sum(np.abs( Or - corr2 ))
+            D = np.sum(np.abs(Or - corr2))
             if norm:
-                D /= ((Ref.shape[0]-2*dy)*(Ref.shape[1]-2*dx))
+                D /= ((Ref.shape[0] - 2 * dy) * (Ref.shape[1] - 2 * dx))
             if test:
-                tested[iy,ix] = D
+                tested[iy, ix] = D
             if D < Dbest:
                 Dbest = D
-                best = (dx,dy)
+                best = (dx, dy)
     if test:
         return best, Dbest, tested
     return best, Dbest
```

### Comparing `pySPM-0.2.9/pySPM/Block.py` & `pyspm-0.3.0/pySPM/Block.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,510 +1,771 @@
-# -- coding: utf-8 --
-
-# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
-
-"""
-Module to handle block type used in iontof file formats ITA,ITM,ITS, etc...
-"""
-
-import sys
-import binascii
-import struct
-import os
-
-class MissingBlock(Exception):
-    def __init__(self, parent, name, index):
-        self.block_name = parent.parent+'/'+name
-        self.index = index
-        
-    def __str__(self):
-        return "Missing block \"{name}\" with index {index}".format(name=self.block_name,index=self.index)
-        
-class Block:
-    """
-    Class to handle a iontof-Block
-    One iontof file ITA,ITM,ITS contains a lot of Blocks forming a hierarchical structure.
-    Each Block can have children (sub-Blocks) and values (data).
-    
-    Note: This class was created by reverse engineering on the fileformat of iontof and is most probably not 100% accurate.
-    Nevertheless is works in very good agreement with the developer's data.
-    """
-    def __init__(self, fp, parent=''):
-        """
-        Init the class
-        fp: file pointer (the one created by open(...) of an ITA,ITM,ITS, etc... file pointing at the beginning of a block
-        
-        Each block start with one byte of type followed by 4 bytes that should always be \x19\x00\x00\x00 (all those 5 bytes are saved in self.Type)
-        Note: the value \x19\x00\x00\x00 is the unit32 for 25 which is the pre-header length of the block.
-        
-        Then follows 5 uint32: length, z, u ,x ,y
-            length: The length of the block's name
-            z: Block ID. Start at 0 and is increased monotonically for each blocks of the same name with the same parent. We usually find the ID from the children's list (see below) and this information is never used as it's redundant.
-            u: The number of children / sub-blocks. Might be = 0 even if the block has children. Check the value L (defined below) if so
-            x: The length of the block's value
-            y: Redundant. Seems to be always = x
-        Then follow length-bytes representing the name of the block
-        Then follow x-bytes forming the value of the block
-        
-        Blocks of types \x01\x19\x00\x00\x00 and \x03\x19\x00\x00\x00 are blocks that contains sub-blocks. There is no big difference between the two. I guess that types \x01 is the first one and type \x03 are the continuation blocks
-            Those block have a value which starts with 41-bytes.
-                2 uint32 -> (length, nums).
-                    length: We actually don't need it. It's a redundant information. That is the length of the sub-headers. (It stop just before the sub-blocks names)
-                    nums: The variable u (see above) contains the number of children. If u ==0, then nums will tell the correct number of children
-                5 bytes: type (usually 00 00 00 00 00 or 03 19 00 00 00)
-                5 uint32 -> a,b,L,d,e
-                    a,b,d,e are unknown
-                    L seems to give information on the number of children
-                1 uint64 -> NextBlock
-                    Big blocks can be chunked in several ones. NextBlock tells the position in the file of the next chunk. If = 0, then it's the last chunk
-            Then 33 bytes for each sub-block follows:
-                1 byte: spacing (usually = 0 or 1)
-                3 uint32 -> index, slen, id
-                    index: The position of the sub-block name in the header
-                    slen: The length of the sub-block name (which is store later). So basically the sub-block name is: Block.value[index:index+slen]
-                    id: start at 0 and increase monotonically for sub-blocks having the same name
-                4 unknown padding bytes
-                2 uint64 -> blen, bidx
-                    blen: Block length
-                    bidx: Position of the Block in the file
-            All the names of all sub-blocks follows (concatenated). You need to use their name length (see slen above) in order to chunk them properly
-            You should then go to the position NextBlock in the file and read the block their. It's the continuation of the current one.
-            
-        Blocks of types \x00\x19\x00\x00\s00 have no children and only a value, usually formed by a string (UTF-16), an int or a float.
-        The type of the value was not discovered to be written in the Block. The user should deduce it depending on the block's name and location.
-        
-        Blocks of type \x80\x19\x00\x00\x00 have it's values compressed with zlib (notice the \x78\x5e at the beginning which is typical for zlib encoded data)
-            Once decompressed it usually store an array in binary.
-        """
-        self.f = fp
-        self.parent = parent
-        self.offset = self.f.tell()
-        self.Type = self.f.read(5)
-        if self.Type[1:] != b'\x19\x00\x00\x00':
-            raise ValueError('Wrong block type ({Type}) found @{pos}'\
-                .format(pos=self.offset, Type=binascii.hexlify(self.Type[1:])))
-        if len(self.Type) < 5:
-            raise ValueError('EOF reached. Block cannot be read')
-        self.head = dict(zip(['name_length', 'ID', 'N', 'length1', 'length2'], \
-            struct.unpack('<5I', self.f.read(20))))
-        self.name = self.f.read(self.head['name_length']).decode('ascii')
-        self.value = self.f.read(self.head['length1'])
-        self.List = None
-        self.iterP = 0
-        
-    def DepthFirstSearch(self, callback=None, filter=lambda x: True, func=lambda x: x):
-        """
-        Perform a depth first search on the blocks.
-        pass each block where filter(block) is true to a callback
-        Also apply a function func to the result and create a list for the result
-        """
-        res = []
-        if filter(self):
-            res += [func(self)]
-            if callback is not None:
-                callback(self)
-            if self.Type[0] in [1,3]:
-                for x in self:
-                    res += x.DepthFirstSearch(callback=callback, filter=filter, func=func)
-        return res
-    
-    def getName(self):
-        """
-        Return the name of the Block
-        """
-        return self.name
-
-    def getList(self):
-        """
-        Return the list of the sub-blocks (children) of the current Block.
-        """
-        if not self.Type[0:1] in [b'\x01', b'\x03']:
-            return []
-        if self.List is None:
-            return self.createList()
-        return self.List
-    
-    def gotoFollowingBlock(self):
-        offset = self.offset+25+self.head['name_length']+self.head['length1']
-        if offset < os.fstat(self.f.fileno()).st_size:
-            self.f.seek(offset)
-            return Block(self.f, parent=None)
-        return None
-        
-    def gotoNextBlock(self):
-        offset = self.offset
-        self.f.seek(offset)
-        head = dict(zip(['name_length', 'ID', 'N', 'length1', 'length2'], struct.unpack('<5x5I', self.f.read(25))))
-        name = self.f.read(head['name_length'])
-        length, nums, NextBlock = struct.unpack('<II25xQ', self.f.read(41))
-        self.f.seek(NextBlock)
-        return Block(self.f, parent=self.parent)
-    
-    def getNthChild(self, n=0):
-        L = self.getList()
-        assert len(L)>n
-        return self.gotoItem(L[n]['name'],L[n]['id'])
-        
-    def createList(self, limit=None, debug=False):
-        """
-        Generate a list (self.List) containing all the children (sub-blocks) of the current Block
-        """
-        length, nums, NextBlock = struct.unpack('<II25xQ', self.value[:41])
-        self.nums = nums
-        offset = self.offset
-        self.List = []
-        while True:
-            self.f.seek(offset)
-            head = dict(zip(['name_length', 'ID', 'N', 'length1', 'length2'], \
-                struct.unpack('<5x5I', self.f.read(25))))
-            name = self.f.read(head['name_length'])
-            data = self.f.tell()
-            length, nums, NextBlock = \
-                struct.unpack('<II25xQ', self.f.read(41))
-            N = head['N']
-            ## The following is commented as believed to be erroneous
-            #if N == 0:
-            #    N = nums
-            for i in range(N):                
-                self.f.seek(data+42+33*i)
-                S = dict(\
-                    zip(['index', 'slen', 'id', 'blen', 'bidx'],\
-                    struct.unpack('<III4xQQ', self.f.read(32))))
-                self.f.seek(data+S['index'])
-                S['name'] = self.f.read(S['slen']).decode('ascii')
-                self.List.append(S)
-            if NextBlock == 0:
-                break
-            offset = NextBlock
-        return self.List
-            
-    def getString(self):
-        """
-        Decode the value of the Block to UTF-16 (standard for all strings in this fileformat)
-        """
-        return self.value.decode('utf16')
-
-    def dictList(self):
-        """
-        Return a dictionary of the value decoded with various formats (raw, long, float, utf16)
-        As the type of the data is not known, this function is very helpful for debugging purpose
-        """
-        d = {}
-        for i, l in enumerate(self.getList()):
-            self.f.seek(l['bidx'])
-            child = Block(self.f, parent=[self.parent+'/'+self.name,'/'][self.parent==''])
-            if child.Type[0:1] == b'\x00':
-                value = binascii.hexlify(child.value)
-                d[child.name] = {'raw':value}
-                if len(child.value) == 4:
-                    d[child.name]['long'] = child.getLong()
-                elif len(child.value) == 8:
-                    d[child.name]['float'] = child.getDouble()
-                    d[child.name]['long'] = child.getLongLong()
-                if len(child.value)%2 == 0:
-                    d[child.name]['utf16'] = child.value.decode('utf16', "ignore")
-            del child
-        return d
-
-    def showList(self):
-        """
-        Show a list of all the children (sub-blocks) of the current Block.
-        It will also display the value/data of all the children (if any)
-        """
-        print('List of', len(self.getList()))
-        for i, l in enumerate(self.List):
-            self.f.seek(l['bidx'])
-            other = ''
-            try:
-                child = Block(self.f, parent=[self.parent+'/'+self.name,'/'][self.parent==''])
-                if child.Type[0:1] == b'\x00':
-                    if len(child.value) == 4:
-                        vL = child.getLong()
-                        Dtype = 'long'
-                    elif len(child.value) == 8:
-                        vL = child.getDouble()
-                        Dtype = 'double'
-                        other += ' = '+str(child.getLongLong())+" (long64)"
-                    elif len(child.value) == 2:
-                        vL = child.getShort()
-                        Dtype = 'short'
-                    elif len(child.value) == 1:
-                        vL = child.getByte()
-                        Dtype = 'byte'
-                    else:
-                        vL = '???'
-                        Dtype = '???'
-                    
-                    value = binascii.hexlify(child.value)
-                    if len(value) > 16:
-                        value = value[:16]+b'...'
-                    if len(child.value)%2 == 0:
-                        vS = child.value.decode('utf16', "ignore")
-                        if len(vS) > 20:
-                            vS = vS[:20]+'...'
-                        print(u"{name} ({id}) <{blen}> @{bidx}, value = {value} (hex) = \"{vS}\" (UTF-16)= {vL} ({Dtype}){other}"\
-                            .format(value=value, vL=vL, Dtype=Dtype, other=other, vS=vS, **l))
-                    else:
-                        print(u"{name} ({id}) <{blen}> @{bidx}, value = {value} (hex) = {vL} ({Dtype}){other}"\
-                            .format(value=value, vL=vL, Dtype=Dtype, other=other, **l))
-                else:
-                    print("{name} ({id}) [{T}] <{blen}> @{bidx}".format(T=child.Type[0], **l))
-                del child
-            except ValueError:
-                pass
-
-    def __iter__(self):
-        """
-        Return an iterator over all the children of the current block)
-        """
-        self.pointer = 0
-        return self
-
-    def __next__(self):
-        L = self.getList()
-        if self.pointer >= len(L):
-            raise StopIteration
-        it = L[self.pointer]
-        self.pointer += 1
-        return self.gotoItem(it['name'], it['id'])
-
-    def gotoItem(self, name, idx=0, lazy=False):
-        """
-        Return a new Block instance of a child of the current Block
-        name: name of the children's block
-        """
-        Idx = self.getIndex(name, idx, lazy=lazy)
-        self.f.seek(Idx)
-        return Block(self.f, parent=[self.parent+'/'+self.name,'/'][self.parent==''])
-
-    def getIndex(self, name, idx=0, lazy=False):
-        """
-        Get the index of the children having a name=name.
-        This function is more intended for internal usage.
-        You are encouraged to use the function _goto_ instead
-        
-        If more than one children have the same name,
-        the second one can by retrieved by idx=1, the third with idx=2, etc.
-        
-        Sometimes the id does not start with 0, but with random high values.
-        Instead of looking at the correct id, you can sue lazy=True with idx=0 in order to fetch the first one saved.
-        """
-        if type(name) is bytes:
-            name = name.decode('ascii')
-        i=0
-        if name is '*':
-            return self.getList()[idx]['bidx']
-        for l in self.getList():
-            if l['name'] == name:
-                if (lazy and i==idx) or (not lazy and l['id'] == idx):
-                    return l['bidx']
-                i+=1
-        raise MissingBlock(self, name, idx)
-
-    def goto(self, path, lazy=False):
-        """
-        Return a sub Block having a specific path
-        path: path is similar to filepath.
-        The block X contained in B which is itself contained in A,
-        can be retrieved with the path: A/B/X
-        if the block B has several children having the same name,
-        A/B/X[n] will return the n-th child (note that 0 is the first child)$
-        
-        As the id sometimes start at weird values and we just want the first ones
-        saved whatever its id is, we can use the lazy=True argument.
-        """
-        if path == '':
-            return self
-        self.f.seek(self.offset)
-        s = Block(self.f)
-        for p in path.split('/'):
-            idx = 0
-            if '[' in p and p[-1] == ']':
-                i = p.index('[')
-                idx = int(p[i+1:-1])
-                p = p[:i]
-            if p is '*':
-                e = s.getList()[idx]
-                p = e['name']
-                idx = e['id']
-            s = s.gotoItem(p, idx, lazy=lazy)
-        return s
-
-    def getLongLong(self):
-        """
-        Decode the value as an 64-Integer
-        """
-        return struct.unpack('<q', self.value)[0]
-
-    def getDouble(self):
-        """
-        Decode the value as a 64-float (Double)
-        """
-        return struct.unpack('<d', self.value)[0]
-
-    def getShort(self):
-        """
-        Decode the value as an 16-Integer (Short)
-        """
-        return struct.unpack('<h', self.value)[0]
-
-    def getByte(self):
-        """
-        Decode the value as a 1-Byte
-        """
-        return struct.unpack('<B', self.value)[0]
-
-    def getULong(self):
-        """
-        Decode the value as an unsigned 32-Integer (Long)
-        """
-        return struct.unpack('<I', self.value)[0]
-
-    def getLong(self):
-        """
-        Decode the value as an 32-Integer (Long)
-        """
-        return struct.unpack('<i', self.value)[0]
-    
-    def unpickle(self):
-        import pickle
-        return pickle.loads(self.value)
-        
-    def getKeyValue(self, offset=16):
-        """
-        Return a dictionnary of key/values pairs of the data
-        Note that the function has no idea if the data are stored as so.
-        """
-        L = struct.unpack("<I", self.value[offset:offset+4])[0]
-        Key = self.value[offset+4:offset+4+L].decode('utf16', 'ignore')
-        int_value, float_value = struct.unpack("<2xqd", self.value[offset+4+L:offset+22+L])
-        L2 = struct.unpack("<I", self.value[offset+22+L:offset+26+L])[0]
-        SVal = self.value[offset+26+L:offset+26+L+L2].decode('utf16', 'ignore')
-        return {'key':Key, 'float':float_value, 'int':int_value,'string':SVal}
-
-    def show(self, maxlevel=3, level=0, All=False, out=sys.stdout, digraph=False, parent=None, ex=None):
-        """
-        Display the children of the current Block (recursively if maxlevel > 1)
-        Very useful for debugging purpose and looking for the path of valuable data.
-        out: file instance to write the results (default terminal)
-        digraph: if True return a digraph (http://www.graphviz.org/) representation of the children
-        level: internal variable used to call the function recursively.
-        ex: execute function
-        """
-        if not ex is None:
-            ex(self)
-        if parent == None:
-            parent = self.name
-        if digraph and level == 0:
-            out.write('digraph {{\n graph [nodesep=.1 rankdir=LR size="10,120"]\n'.format(root=parent))
-        for l in self.getList():
-            if l['id'] == 0 or All:
-                if digraph:
-                    out.write('"{parent}-{name}" [label="{name}"]\n"{parent}" -> "{parent}-{name}"\n'\
-                        .format(parent=parent, name=l['name'].decode('utf8')))
-                else:
-                    if ex is None:
-                        out.write("{tab}{name} ({id}) @{bidx}\n".format(tab="\t"*level, **l))
-                if level < maxlevel:
-                    try:
-                        self.gotoItem(l['name'], l['id'])\
-                            .show(maxlevel, level+1, All=All, out=out, digraph=digraph\
-                            , parent=parent+'-'+l['name'], ex=ex)
-                    except:
-                        pass
-        if digraph and level == 0:
-            out.write('}')
-
-    def getIndexes(self, key, debug=False):
-        if type(key) is str:
-            key = key.encode('utf8')
-        r = []
-        for x in self.getList():
-            if debug:
-                print(x['name'],key)
-            if x['name'] == key:
-                r.append(x['id'])
-        return r
-
-    def decompress(self):
-        import zlib
-        return zlib.decompress(self.value)
-
-    def getData(self, fmt="I"):
-        raw = self.decompress()
-        L = len(raw)//struct.calcsize(fmt)
-        return struct.unpack("<"+str(L)+fmt, raw)
-        
-    def modify_block_and_export(self, path, new_data, output, debug=False, prog=False, lazy=False):
-        assert not os.path.exists(output) # Avoid to erase an existing file. Erase it outside the library if needed.
-        out = open(output,'wb')
-        out.write(b'ITStrF01')
-        block = self.goto(path, lazy=lazy)
-        block_offset = block.offset
-        length_diff = len(new_data)-len(block.value)
-        self.f.seek(8)
-        FILE_SIZE =  os.fstat(self.f.fileno()).st_size
-        if prog:
-            try:
-                from tqdm import tqdm_notebook as tqdm
-            except:
-                from tqdm import tqdm as tqdm
-            T = tqdm(total=FILE_SIZE)
-        debug_msg = ["FileSize: "+str(FILE_SIZE)]
-        if debug:
-            print("File Size",FILE_SIZE)
-        curr = 8
-        if prog:
-            T.update(8)
-        while self.f.tell() < FILE_SIZE:
-            debug_msg = debug_msg[-30:]
-            if prog:
-                ncurr = self.f.tell()
-                T.update(ncurr-curr)
-                curr = ncurr
-            debug_msg.append("Current position: @"+str(self.f.tell()))
-            try:
-                current = Block(self.f) # Here we don't care about the parent argument. It is used only for debug purpose anyway.
-            except Exception as ex:
-                print("Error found! Debug info")
-                for x in debug_msg:
-                    print("\t"+x)
-                raise ex
-            self.f.seek(current.offset)
-            curr_block_length = current.head['length1'] + current.head['name_length'] + 25
-            debug_msg.append('Block Name: "{}" / length: {}'.format(current.name, curr_block_length))
-            if current.offset == block_offset: # Found the block to change
-                debug_msg.append("Block to change FOUND!")
-                out.write(self.f.read(5)) # Write block type
-                out.write(struct.pack("<5I",block.head['name_length'],block.head['ID'],block.head['N'], length_diff+block.head['length1'], length_diff+block.head['length2']))
-                self.f.read(20) # Skip header
-                out.write(self.f.read(block.head['name_length'])) # copy block name
-                self.f.read(block.head['length1']) # skip data in source
-                out.write(new_data) # write new_data
-            elif current.Type[0] in [1,3]: # found a container, check for references to block after the modified block
-                debug_msg.append("Block container found. Checking children...")
-                out.write(self.f.read(25)) # copy header
-                out.write(self.f.read(current.head['name_length'])) # copy block name
-                SubHeader = list(struct.unpack('<2I5s5IQ', self.f.read(41) )) # read sub-block header
-                if SubHeader[8] > block_offset: # Is the nextbloxk after the modified block? Yes => Adjust the offset position
-                    SubHeader[8] += length_diff
-                out.write(struct.pack('<2I5s5IQ', *SubHeader )) # write sub-block header
-                N = current.head['N']
-                #if N == 0:
-                #    N = SubHeader[1]
-                for i in range(N):
-                    X, index, slen, id,Y, blen, bidx = struct.unpack('<B4I2Q', self.f.read(33))
-                    if bidx == block_offset: # If the children block is the modified block, adjust length
-                        blen = len(new_data)
-                    elif bidx > block_offset: # If the children is after the modifien block, adjust its offset
-                        bidx += length_diff
-                    out.write(struct.pack('<B4I2Q',X, index, slen, id, Y,blen, bidx)) # write child info
-                # Write the extra bytes used by iontof which seems to be useless as well as the childrens' name
-                delta = curr_block_length - (self.f.tell() - current.offset) # number of bytes remaining till the end of the block
-                out.write(self.f.read(delta))
-            else:
-                debug_msg.append("Data Block found. Copy data without check...")
-                out.write(self.f.read(curr_block_length))
-        if prog:
-            T.update(FILE_SIZE-curr)
-            T.close()
-        out.close()
+# -- coding: utf-8 --
+
+# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
+
+"""
+Module to handle block type used in iontof file formats ITA,ITM,ITS, etc...
+"""
+
+from __future__ import absolute_import
+
+import binascii
+import os
+import struct
+import sys
+
+from .utils import dec_debug, do_debug
+from .utils.misc import deprecated, aliased
+
+
+class MissingBlock(Exception):
+    def __init__(self, parent, name, index):
+        self.block_name = parent.path + parent.name + '/' + name
+        self.index = index
+
+    def __str__(self):
+        return "Missing block \"{name}\" with index {index}".format(name=self.block_name, index=self.index)
+
+
+@aliased
+class Block:
+    """
+    Class to handle a iontof-Block
+    One iontof file ITA,ITM,ITS contains a lot of Blocks forming a hierarchical structure.
+    Each Block can have children (sub-Blocks) and values (data).
+    
+    Note: This class was created by reverse engineering on the fileformat of iontof and is most probably not 100% accurate.
+    Nevertheless is works in very good agreement with the developer's data.
+    """
+
+    def __init__(self, fp, parent=None):
+        """
+        Init the class
+        fp: file pointer (the one created by open(...) of an ITA,ITM,ITS, etc... file pointing at the beginning of a block
+        
+        Each block start with one byte of type followed by 4 bytes that should always be \x19\x00\x00\x00 (all those 5 bytes are saved in self.Type)
+        Note: the value \x19\x00\x00\x00 is the unit32 for 25 which is the pre-header length of the block.
+        
+        Then follows 5 uint32: slen, ID, N ,length1, length2
+            slen: The length of the block's name
+            ID: Block ID. Start at 0 and is increased monotonically for each blocks of the same name with the same parent. We usually find the ID from the children's list (see below) and this information is never used as it's redundant.
+            N: The number of children / sub-blocks
+            length1: The length of the block's value
+            length2: Redundant. Seems to be always = x. We suspect that length2 is the length till the next following block in the file. Length1 and length2 might be different in case a long block is modified with a smaller content. Length1 should thus math the new data length and length2 remain as large as the old data.
+        Then follow slen-bytes representing the name of the block
+        Then follow length1-bytes forming the value of the block
+        
+        Blocks of types \x01\x19\x00\x00\x00 and \x03\x19\x00\x00\x00 are blocks that contains sub-blocks. There is no big difference between the two. Types \x01 are the first one and type \x03 are the continuation blocks (see NextBlock information below)
+            Those block have a value which starts with 41-bytes.
+                2 uint32 -> (length, nums).
+                    length: We actually don't need it. It's a redundant information. That is the length of the sub-headers. (It stop just before the sub-blocks names)
+                    nums: nums is an indication on the number of children the block can contains. It was found that the block size is = 53*nums
+                5 bytes: type of the NextBlock (usually 00 00 00 00 00 or 03 19 00 00 00)
+                5 uint32 -> a,b,c,d,e
+                    a,b,c,d,e are the NextBlock header (a=slen, b=ID, ...)
+                1 uint64 -> NextBlock
+                    Big blocks can be chunked in several ones. NextBlock tells the position in the file of the next chunk. If = 0, then it's the last chunk
+            Then 33 bytes for each sub-block follows:
+                1 byte: Type of the child
+                3 uint32 -> index, slen, id
+                    index: The position of the sub-block name in the header
+                    slen: The length of the sub-block name (which is store later). So basically the sub-block name is: Block.value[index:index+slen]
+                    id: start at 0 and increase monotonically for sub-blocks having the same name
+                1 uint32: 1 if the child contains data (we believe)?
+                2 uint64 -> blen, bidx
+                    blen: Block length
+                    bidx: Position of the Block in the file
+            All the names of all sub-blocks follows (concatenated). You need to use their name length (see slen above) in order to chunk them properly
+            You should then go to the position NextBlock in the file and read the block their. It's the continuation of the current one.
+            
+        Blocks of types \x00\x19\x00\x00\s00 have no children and only a value, usually formed by a string (UTF-16), an int or a float.
+        The type of the value was not discovered to be written in the Block. The user should deduce it depending on the block's name and location.
+        
+        Blocks of type \x80\x19\x00\x00\x00 have it's values compressed with zlib (notice the \x78\x5e at the beginning which is typical for zlib encoded data)
+            Once decompressed it usually store an array in binary.
+        """
+        self.f = fp
+        self.parent = parent
+        self.path = ''
+        if parent is not None:
+            if parent.parent is None:
+                self.path = '/'
+            else:
+                self.path = parent.path + parent.name + '/'
+        self.offset = self.f.tell()
+        self.Type = self.f.read(5)
+        if self.Type[1:] != b'\x19\x00\x00\x00':
+            raise ValueError('Wrong block type ({Type}) found @{pos}' \
+                             .format(pos=self.offset, Type=binascii.hexlify(self.Type[1:])))
+        if len(self.Type) < 5:
+            raise ValueError('EOF reached. Block cannot be read')
+        self.head = dict(zip(['name_length', 'ID', 'N', 'length1', 'length2'], \
+                             struct.unpack('<5I', self.f.read(20))))
+        self.name = self.f.read(self.head['name_length']).decode('ascii')
+        self.value = self.f.read(self.head['length1'])
+        self.List = None
+        self.iterP = 0
+
+    def inc(self):
+        """
+        Increment the value (interpreted as unsigned in32) of a block by one and write the changes to the file
+        """
+        self.rewrite(struct.pack("<I", self.getLong() + 1))
+
+    def add_child(self, blk):
+        """
+        Add a new child to a given block. /!\ will overwrite the ITA/ITM file.
+        """
+        assert self.Type[0] in [1, 3]
+
+        length, nums, NextBlock = struct.unpack('<II25xQ', self.value[:41])
+        if NextBlock != 0:
+            return self.goto_next_block().add_child(blk)
+
+        # Check the available size of the block
+        header_length = 41 + 33 * self.head['N']
+
+        children_names_length = 0
+        last_id = None
+        lowest_index = struct.unpack("<I", self.value[:4])[0]
+        children_names_length = self.head['length1'] - lowest_index
+        free_space = lowest_index - header_length
+        new_name = blk.name not in self
+
+        new_subblock = False
+        if new_name:
+            if free_space < 33 + len(blk.name):
+                new_subblock = True
+            index = lowest_index - len(blk.name)
+        else:
+            if free_space < 33:
+                new_subblock = True
+            else:
+                index = 0
+                for i in range(self.head['N']):
+                    self.f.seek(self.offset + 25 + len(self.name) + 41 + 33 * i)
+                    s = struct.unpack("<B4I2Q", self.f.read(33))
+                    if s[2] == len(blk.name):
+                        self.f.seek(self.offset + 25 + len(self.name) + s[1])
+                        if blk.name == self.f.read(s[2]).decode('utf8'):
+                            index = s[1]
+                            break
+                assert index > 0
+        if new_subblock:
+            raise Exception("Block is too small to fit the data.")
+        self.f.seek(self.offset + 25 + len(self.name) + header_length)
+        self.f.write(
+            struct.pack("<B4I2Q", blk.Type[0], index, len(blk.name), blk.head['ID'], [0, 1][blk.Type[0] in [0, 128]],
+                        blk.head['length1'], blk.offset))
+        self.f.seek(self.offset + 25 + len(self.name) + index)
+        self.f.write(blk.name.encode('utf8'))
+        self.f.seek(self.offset + 13)
+        self.head['N'] += 1
+        self.f.write(struct.pack("<I", self.head['N']))
+        self.f.seek(self.offset + 25 + len(self.name))
+        if new_name:
+            self.f.write(struct.pack("<I", struct.unpack("<I", self.value[:4])[0] - len(blk.name)))
+
+        self.refresh()
+        return blk
+
+    def refresh(self):
+        """
+        Reload self.value from the file.
+        This function is useful in case a block was overwritten
+        """
+        self.List = None
+        self.f.seek(self.offset + self.head['name_length'] + 25)
+        self.value = self.f.read(self.head['length1'])
+
+    def edit_child(self, old_block, new_block, debug=False):
+        """
+        Edit the children list of a given block.
+        """
+        if not self.Type[0] in [1, 3]:
+            raise Exception("The current block should be of type 01 or 03 (folder)")
+
+        header_length = 41 + 33 * self.head['N']
+        children_names_length = 0
+        last_id = None
+        lowest_index = struct.unpack("<I", self.value[:4])[0]
+        children_names_length = self.head['length1'] - lowest_index
+        found = False
+        for i in range(self.head['N']):
+            self.f.seek(self.offset + 25 + len(self.name) + 41 + 33 * i)
+            entry = list(struct.unpack("<B4I2Q", self.f.read(33)))
+            if entry[6] == old_block.offset:
+                found = True
+                self.f.seek(self.offset + 25 + len(self.name) + 41 + 33 * i)
+                entry[6] = new_block.offset
+                entry[5] = new_block.head['length1']
+                if do_debug(debug):
+                    print("Update inode")
+                self.f.write(struct.pack("<B4I2Q", *entry))
+                break
+        if not found:
+            raise Exception('Child {} not found in {}'.format(old_block.name, self.name))
+        self.refresh()
+
+    def create_dir(self, name, children=[], nums=100, assign=True, id=0):
+        """
+        Create a directory in the ITStr format.
+        
+        Parameters
+        ----------
+        name: string
+            name of the directory
+        children: list of blocks
+            list of the childrens' block which are added
+        nums: int
+            this number will give the approximate number of children one can create. The size of the block will be 53*nums
+        assign: bool
+            If True, will add the created dir as a child of self
+        id: int
+            Blocks having the same name should have a different id.
+        """
+        size = 53 * nums
+        value = struct.pack("<2IB6IQ{}x".format(size - 41), size, nums, 0, 0, 0, 0, 0, 0, 0, 0)
+        blk = self.create_block(name, value, _type=1, id=id)
+        for x in children:
+            blk.add_child(x)
+        if assign:
+            self.add_child(blk)
+        return blk
+
+    def edit_block(self, path, name, value, id=0, _type=0, force=False, debug=False):
+        """
+        This function will go to a given path and create all necessary "folder" (block of type 1).
+        It will then either create a new child with a given name and value if it does not exists and if so it will edit it.
+        Please note that for safety the new value should be of the exact same length than the existing one.
+        If this is not the case, you should consider using the modify_block_and_export() method.
+        You can also use the force=True parameter to force to edit a block when its content is not the same. Be careful, because this will actually keep the old data in the file (but won't be accessible or seen anymore). This means that the size of your ita can grow quickly if you perform a lot of edits...
+        """
+        self.f.seek(self.offset)
+        parent = self
+        if path != '':
+            for p in path.split('/'):
+                idx = 0
+                if '[' in p and p[-1] == ']':
+                    i = p.index('[')
+                    idx = int(p[i + 1:-1])
+                    p = p[:i]
+                if p == '*':
+                    e = parent.get_list()[idx]
+                    p = e['name']
+                    idx = e['id']
+                try:
+                    parent = parent.goto_item(p, idx)
+                except MissingBlock:
+                    parent = parent.create_dir(p, children=[], id=idx)
+        try:
+            if do_debug(debug):
+                print("Accessing block \"{}\"[{}]".format(name, id))
+            child = parent.goto_item(name, id)
+            if child.head['length1'] == len(value):
+                if do_debug(debug):
+                    print("rewrite block")
+                child.rewrite(value, debug=dec_debug(debug))
+                return child
+            elif force:
+                blk = parent.create_block(name, value, id=id, _type=_type, debug=dec_debug(debug))
+                parent.edit_child(child, blk, debug=dec_debug(debug))
+            else:
+                raise Exception(
+                    "Use the force=True parameter if you wish to replace an existing block with another data size")
+        except MissingBlock:
+            if do_debug(debug):
+                print("create new block")
+            return parent.add_child(parent.create_block(name, value, id=id, _type=_type))
+
+    def create_block(self, name, value, id=0, _type=0, debug=False):
+        """
+        Create a new block and write it at the end of the file
+        """
+        if do_debug(debug):
+            print("Creating new block \"{}\" of size {}".format(name, len(value)))
+        if type(name) is str:
+            name = name.encode('utf8')
+        self.f.seek(0, 2)  # goto end of file
+        offset = self.f.tell()
+        size = len(value)
+        slen = len(name)
+        self.f.write(struct.pack("<B6I", _type, 25, slen, id, 0, size, size))
+        self.f.write(name)
+        self.f.write(value)
+        self.f.seek(offset)
+        return Block(self.f)
+
+    @deprecated("DepthFirstSearch")
+    def depth_first_search(self, callback=None, filter=lambda x: True, func=lambda x: x):
+        """
+        Perform a depth first search on the blocks.
+        pass each block where filter(block) is true to a callback
+        Also apply a function func to the result and create a list for the result
+        """
+        res = []
+        if filter(self):
+            res += [func(self)]
+            if callback is not None:
+                callback(self)
+        if self.Type[0] in [1, 3]:
+            for x in self:
+                res += x.depth_first_search(callback=callback, filter=filter, func=func)
+        return res
+
+    @deprecated("getName")
+    def get_name(self):
+        """
+        Return the name of the Block
+        """
+        return self.name
+
+    @deprecated("getList")
+    def get_list(self):
+        """
+        Return the list of the sub-blocks (children) of the current Block.
+        """
+        if not self.Type[0:1] in [b'\x01', b'\x03']:
+            return []
+        if self.List is None:
+            return self.create_list()
+        return self.List
+
+    @deprecated("gotoFollowingBlock")
+    def goto_following_block(self):
+        offset = self.offset + 25 + self.head['name_length'] + self.head['length1']
+        if offset < os.fstat(self.f.fileno()).st_size:
+            self.f.seek(offset)
+            return Block(self.f, parent=None)
+        return None
+
+    # deprecated("gotoNextBlock")
+    def goto_next_block(self):
+        offset = self.offset
+        self.f.seek(offset)
+        head = dict(zip(['name_length', 'ID', 'N', 'length1', 'length2'], struct.unpack('<5x5I', self.f.read(25))))
+        name = self.f.read(head['name_length'])
+        length, nums, NextBlock = struct.unpack('<II25xQ', self.f.read(41))
+        if NextBlock == 0:
+            return None
+        self.f.seek(NextBlock)
+        return Block(self.f, parent=self.parent)
+
+    def getNthChild(self, n=0):
+        L = self.get_list()
+        assert len(L) > n
+        return self.goto_item(L[n]['name'], L[n]['id'])
+
+    @deprecated("createList")
+    def create_list(self, limit=None, debug=False):
+        """
+        Generate a list (self.List) containing all the children (sub-blocks) of the current Block
+        """
+        length, nums, next_block = struct.unpack('<II25xQ', self.value[:41])
+        self.nums = nums
+        offset = self.offset
+        self.List = []
+        while True:
+            self.f.seek(offset)
+            data = self.f.read(25)
+            if len(data) < 25:
+                raise Exception('Children of {} @{} cannot be read. Data might be corrupted!'.format(self.name, offset))
+            head = dict(zip(['name_length', 'ID', 'N', 'length1', 'length2'], \
+                            struct.unpack('<5x5I', data)))
+            name = self.f.read(head['name_length'])
+            data = self.f.tell()
+            length, nums, next_block = \
+                struct.unpack('<II25xQ', self.f.read(41))
+            N = head['N']
+            ## The following is commented as believed to be erroneous
+            # if N == 0:
+            #    N = nums
+            for i in range(N):
+                self.f.seek(data + 42 + 33 * i)
+                S = dict( \
+                    zip(['index', 'slen', 'id', 'blen', 'bidx'], \
+                        struct.unpack('<III4xQQ', self.f.read(32))))
+                self.f.seek(data + S['index'])
+                S['name'] = self.f.read(S['slen']).decode('ascii')
+                self.List.append(S)
+            if next_block == 0:
+                break
+            offset = next_block
+        return self.List
+
+    @deprecated("getString")
+    def get_string(self):
+        """
+        Decode the value of the Block to UTF-16 (standard for all strings in this fileformat)
+        """
+        return self.value.decode('utf16')
+
+    @deprecated("dictList")
+    def dict_list(self):
+        """
+        Return a dictionary of the value decoded with various formats (raw, long, float, utf16)
+        As the type of the data is not known, this function is very helpful for debugging purpose
+        """
+        d = {}
+        for i, l in enumerate(self.get_list()):
+            self.f.seek(l['bidx'])
+            child = Block(self.f, parent=self)
+            if child.Type[0:1] == b'\x00':
+                value = binascii.hexlify(child.value)
+                d[child.name] = {'raw': value}
+                if len(child.value) == 4:
+                    d[child.name]['long'] = child.get_long()
+                    d[child.name]['ulong'] = child.get_ulong()
+                elif len(child.value) == 8:
+                    d[child.name]['float'] = child.get_double()
+                    d[child.name]['long'] = child.get_longlong()
+                if len(child.value) % 2 == 0:
+                    d[child.name]['utf16'] = child.value.decode('utf16', "ignore")
+            del child
+        return d
+
+    @deprecated("showList")
+    def show_list(self):
+        """
+        Show a list of all the children (sub-blocks) of the current Block.
+        It will also display the value/data of all the children (if any)
+        """
+        print('List of', len(self.get_list()))
+        for i, l in enumerate(self.List):
+            self.f.seek(l['bidx'])
+            other = ''
+            try:
+                child = Block(self.f, parent=self)
+                if child.Type[0:1] == b'\x00':
+                    if len(child.value) == 4:
+                        vL = child.get_long()
+                        Dtype = 'long'
+                    elif len(child.value) == 8:
+                        vL = child.get_double()
+                        Dtype = 'double'
+                        other += ' = ' + str(child.get_longlong()) + " (long64)"
+                    elif len(child.value) == 2:
+                        vL = child.get_short()
+                        Dtype = 'short'
+                    elif len(child.value) == 1:
+                        vL = child.get_byte()
+                        Dtype = 'byte'
+                    else:
+                        vL = '???'
+                        Dtype = '???'
+
+                    value = binascii.hexlify(child.value)
+                    if len(value) > 16:
+                        value = value[:16] + b'...'
+                    if len(child.value) % 2 == 0:
+                        vS = child.value.decode('utf16', "ignore")
+                        if len(vS) > 20:
+                            vS = vS[:20] + '...'
+                        print(
+                            u"{name} ({id}) <{blen}> @{bidx}, value = {value} (hex) = \"{vS}\" (UTF-16)= {vL} ({Dtype}){other}" \
+                                .format(value=value, vL=vL, Dtype=Dtype, other=other, vS=vS, **l))
+                    else:
+                        print(u"{name} ({id}) <{blen}> @{bidx}, value = {value} (hex) = {vL} ({Dtype}){other}" \
+                              .format(value=value, vL=vL, Dtype=Dtype, other=other, **l))
+                else:
+                    print("{name} ({id}) [{T}] <{blen}> @{bidx}".format(T=child.Type[0], **l))
+                del child
+            except ValueError:
+                pass
+
+    def __iter__(self):
+        """
+        Return an iterator over all the children of the current block)
+        """
+        self.pointer = 0
+        return self
+
+    def __next__(self):
+        L = self.get_list()
+        if self.pointer >= len(L):
+            raise StopIteration
+        it = L[self.pointer]
+        self.pointer += 1
+        return self.goto_item(it['name'], it['id'])
+
+    @deprecated("gotoItem")
+    def goto_item(self, name, idx=0, lazy=False):
+        """
+        Return a new Block instance of a child of the current Block
+        name: name of the children's block
+        """
+        Idx = self.get_index(name, idx, lazy=lazy)
+        self.f.seek(Idx)
+        return Block(self.f, parent=self)
+
+    @deprecated("getIndex")
+    def get_index(self, name, idx=0, lazy=False):
+        """
+        Get the index (here to understand the offset in bytes from the beginning of the file till the block of interest) of the children having a name=name.
+        This function is more intended for internal usage.
+        You are encouraged to use the function _goto_ instead
+        
+        If more than one children have the same name,
+        the second one can by retrieved by idx=1, the third with idx=2, etc.
+        
+        Sometimes the id does not start with 0, but with random high values.
+        Instead of looking at the correct id, you can use lazy=True with idx=0 in order to fetch the first one saved.
+        """
+        if type(name) is bytes:
+            name = name.decode('ascii')
+        i = 0
+        if name == '*':
+            return self.get_list()[idx]['bidx']
+        for l in self.get_list():
+            if l['name'] == name:
+                if (lazy and i == idx) or (not lazy and l['id'] == idx):
+                    return l['bidx']
+                i += 1
+        raise MissingBlock(self, name, idx)
+
+    def goto(self, path, lazy=False):
+        """
+        Return a sub Block having a specific path
+        path: path is similar to filepath.
+        The block X contained in B which is itself contained in A,
+        can be retrieved with the path: A/B/X
+        if the block B has several children having the same name,
+        A/B/X[n] will return the n-th child (note that 0 is the first child)$
+        
+        As the id sometimes start at weird values and we just want the first ones
+        saved whatever its id is, we can use the lazy=True argument.
+        """
+        if path.startswith('/'):
+            path = path[1:]
+        if path == '':
+            return self
+        self.f.seek(self.offset)
+        s = Block(self.f)
+        for p in path.split('/'):
+            idx = 0
+            if '[' in p and p[-1] == ']':
+                i = p.index('[')
+                idx = int(p[i + 1:-1])
+                p = p[:i]
+            if p == '*':
+                e = s.get_list()[idx]
+                p = e['name']
+                idx = e['id']
+            s = s.goto_item(p, idx, lazy=lazy)
+        return s
+
+    @deprecated("getLongLong")
+    def get_longlong(self):
+        """
+        Decode the value as an 64-Integer
+        """
+        return struct.unpack('<q', self.value)[0]
+
+    @deprecated("getDouble")
+    def get_double(self):
+        """
+        Decode the value as a 64-float (Double)
+        """
+        return struct.unpack('<d', self.value)[0]
+
+    @deprecated("getShort")
+    def get_short(self):
+        """
+        Decode the value as an 16-Integer (Short)
+        """
+        return struct.unpack('<h', self.value)[0]
+
+    @deprecated("getByte")
+    def get_byte(self):
+        """
+        Decode the value as a 1-Byte
+        """
+        return struct.unpack('<B', self.value)[0]
+
+    def get_bytes(self):
+        """
+        Decode the values as unsigned bytes
+        """
+        return struct.unpack('<{}B'.format(len(self.value)), self.value)
+
+    @deprecated("getULong")
+    def get_ulong(self):
+        """
+        Decode the value as an unsigned 32-Integer (Long)
+        """
+        return struct.unpack('<I', self.value)[0]
+
+    @deprecated("getLong")
+    def get_long(self):
+        """
+        Decode the value as an 32-Integer (Long)
+        """
+        return struct.unpack('<i', self.value)[0]
+
+    def unpickle(self):
+        import pickle
+        return pickle.loads(self.value)
+
+    @deprecated("getKeyValue")
+    def get_key_value(self, offset=16):
+        """
+        Return a dictionnary of key/values pairs of the data
+        Note that the function has no idea if the data are stored as so.
+        """
+        L = struct.unpack("<I", self.value[offset:offset + 4])[0]
+        Key = self.value[offset + 4:offset + 4 + L].decode('utf16', 'ignore')
+        int_value, float_value = struct.unpack("<2xqd", self.value[offset + 4 + L:offset + 22 + L])
+        L2 = struct.unpack("<I", self.value[offset + 22 + L:offset + 26 + L])[0]
+        SVal = self.value[offset + 26 + L:offset + 26 + L + L2].decode('utf16', 'ignore')
+        return {'key': Key, 'float': float_value, 'int': int_value, 'string': SVal}
+
+    def __contains__(self, name):
+        return name in [x['name'] for x in self.get_list()]
+
+    def show(self, maxlevel=3, level=0, all=False, out=sys.stdout, digraph=False, parent=None, ex=None, **kargs):
+        """
+        Display the children of the current Block (recursively if maxlevel > 1)
+        Very useful for debugging purpose and looking for the path of valuable data.
+        out: file instance to write the results (default terminal)
+        digraph: if True return a digraph (http://www.graphviz.org/) representation of the children
+        level: internal variable used to call the function recursively.
+        ex: execute function
+        """
+        if 'All' in kargs:
+            all = kargs.pop("All")
+
+        if not ex is None:
+            ex(self)
+        if parent == None:
+            parent = self.name
+        if digraph and level == 0:
+            out.write('digraph {{\n graph [nodesep=.1 rankdir=LR size="10,120"]\n'.format(root=parent))
+        for l in self.get_list():
+            if l['id'] == 0 or all:
+                if digraph:
+                    out.write('"{parent}-{name}" [label="{name}"]\n"{parent}" -> "{parent}-{name}"\n' \
+                              .format(parent=parent, name=l['name'].decode('utf8')))
+                else:
+                    if ex is None:
+                        out.write("{tab}{name} ({id}) @{bidx}\n".format(tab="\t" * level, **l))
+                if level < maxlevel:
+                    try:
+                        self.goto_item(l['name'], l['id']) \
+                            .show(maxlevel, level + 1, all=all, out=out, digraph=digraph \
+                                  , parent=parent + '-' + l['name'], ex=ex)
+                    except:
+                        pass
+        if digraph and level == 0:
+            out.write('}')
+
+    @deprecated("getIndexes")
+    def get_indexes(self, key, debug=False):
+        if type(key) is str:
+            key = key.encode('utf8')
+        r = []
+        for x in self.get_list():
+            if debug:
+                print(x['name'], key)
+            if x['name'] == key:
+                r.append(x['id'])
+        return r
+
+    def decompress(self):
+        import zlib
+        return zlib.decompress(self.value)
+
+    @deprecated("getData")
+    def get_data(self, fmt="I", decompress=True):
+        if decompress:
+            raw = self.decompress()
+        else:
+            raw = self.value
+        L = len(raw) // int(struct.calcsize(fmt))
+        return struct.unpack("<" + str(L) + fmt, raw)
+
+    def rewrite(self, content, debug=False):
+        assert (len(content)) == self.head['length1']
+        if do_debug(debug):
+            print("Rewriting block \"{}\"".format(self.name))
+        # set pointer at beginning of data
+        self.f.seek(self.offset + 25 + self.head['name_length'])
+        self.f.write(content)
+        self.refresh()
+
+    def modify_block_and_export(self, path, new_data, output, debug=False, prog=False, lazy=False):
+        assert not os.path.exists(output)  # Avoid to erase an existing file. Erase it outside the library if needed.
+        out = open(output, 'wb')
+        out.write(b'ITStrF01')
+        block = self.goto(path, lazy=lazy)
+        block_offset = block.offset
+        length_diff = len(new_data) - len(block.value)
+        self.f.seek(8)
+        FILE_SIZE = os.fstat(self.f.fileno()).st_size
+        if prog:
+            try:
+                from tqdm import tqdm_notebook as tqdm
+            except:
+                from tqdm import tqdm as tqdm
+            T = tqdm(total=FILE_SIZE)
+        debug_msg = ["FileSize: " + str(FILE_SIZE)]
+        if debug:
+            print("File Size", FILE_SIZE)
+        curr = 8
+        if prog:
+            T.update(8)
+        while self.f.tell() < FILE_SIZE:
+            debug_msg = debug_msg[-30:]
+            if prog:
+                ncurr = self.f.tell()
+                T.update(ncurr - curr)
+                curr = ncurr
+            debug_msg.append("Current position: @" + str(self.f.tell()))
+            try:
+                current = Block(
+                    self.f)  # Here we don't care about the parent argument. It is used only for debug purpose anyway.
+            except Exception as ex:
+                print("Error found! Debug info")
+                for x in debug_msg:
+                    print("\t" + x)
+                raise ex
+            self.f.seek(current.offset)
+            curr_block_length = current.head['length1'] + current.head['name_length'] + 25
+            debug_msg.append('Block Name: "{}" / length: {}'.format(current.name, curr_block_length))
+            if current.offset == block_offset:  # Found the block to change
+                debug_msg.append("Block to change FOUND!")
+                out.write(self.f.read(5))  # Write block type
+                out.write(struct.pack("<5I", block.head['name_length'], block.head['ID'], block.head['N'],
+                                      length_diff + block.head['length1'], length_diff + block.head['length2']))
+                self.f.read(20)  # Skip header
+                out.write(self.f.read(block.head['name_length']))  # copy block name
+                self.f.read(block.head['length1'])  # skip data in source
+                out.write(new_data)  # write new_data
+            elif current.Type[0] in [1, 3]:  # found a container, check for references to block after the modified block
+                debug_msg.append("Block container found. Checking children...")
+                out.write(self.f.read(25))  # copy header
+                out.write(self.f.read(current.head['name_length']))  # copy block name
+                SubHeader = list(struct.unpack('<2I5s5IQ', self.f.read(41)))  # read sub-block header
+                if SubHeader[
+                    8] > block_offset:  # Is the nextbloxk after the modified block? Yes => Adjust the offset position
+                    SubHeader[8] += length_diff
+                out.write(struct.pack('<2I5s5IQ', *SubHeader))  # write sub-block header
+                N = current.head['N']
+                # if N == 0:
+                #    N = SubHeader[1]
+                for i in range(N):
+                    X, index, slen, id, Y, blen, bidx = struct.unpack('<B4I2Q', self.f.read(33))
+                    if bidx == block_offset:  # If the children block is the modified block, adjust length
+                        blen = len(new_data)
+                    elif bidx > block_offset:  # If the children is after the modifien block, adjust its offset
+                        bidx += length_diff
+                    out.write(struct.pack('<B4I2Q', X, index, slen, id, Y, blen, bidx))  # write child info
+                # Write the extra bytes used by iontof which seems to be useless as well as the childrens' name
+                delta = curr_block_length - (
+                        self.f.tell() - current.offset)  # number of bytes remaining till the end of the block
+                out.write(self.f.read(delta))
+            else:
+                debug_msg.append("Data Block found. Copy data without check...")
+                out.write(self.f.read(curr_block_length))
+        if prog:
+            T.update(FILE_SIZE - curr)
+            T.close()
+        out.close()
```

### Comparing `pySPM-0.2.9/pySPM/Bruker.py` & `pyspm-0.3.0/pySPM/Bruker.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 # Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
 
 """
 Module to handle SPM images recorded by a Bruker AFM
 """
 
-import struct
 import re
+import struct
+
 import numpy as np
+
 import pySPM
-import warnings
 
 
 class Bruker:
     """
     Class to handle SPM images recorded by a Bruker AFM
     """
 
@@ -38,91 +39,130 @@
                     if mode == 'Image':
                         self.layers[-1][args[0]] = args[1:]
                     elif mode == 'Scanner':
                         self.scanners[-1][args[0]] = args[1:]
                 if line == b"*File list end":
                     break
 
-    def _get_raw_layer(self, i):
+    def _get_bpp(self, i):
+        off = int(self.layers[i][b'Data offset'][0])
+        cols = int(self.layers[i][b'Number of lines'][0])
+        rows = int(self.layers[i][b'Samps/line'][0])
+        byte_length = int(self.layers[i][b'Data length'][0])
+        length = rows * cols
+        bpp = byte_length // length
+        return bpp
+
+    def _get_raw_layer(self, i, debug=False):
         """
         Internal function to retrieve raw data of a layer
         """
         off = int(self.layers[i][b'Data offset'][0])
+        if debug:
+            print("RAW offset: ", off)
         cols = int(self.layers[i][b'Number of lines'][0])
         rows = int(self.layers[i][b'Samps/line'][0])
         byte_length = int(self.layers[i][b'Data length'][0])
-        length = rows*cols
+        length = rows * cols
         bpp = byte_length // length
         byte_length = length * bpp
-        
+
         self.file.seek(off)
         return np.array(
-            struct.unpack("<"+str(length)+{2:'h',4:'i',8:'q'}[bpp], self.file.read(byte_length)),
+            struct.unpack("<" + str(length) + {2: 'h', 4: 'i', 8: 'q'}[bpp], self.file.read(byte_length)),
             dtype='float64').reshape((cols, rows))
 
     def list_channels(self, encoding='latin1'):
         print("Channels")
         print("========")
         for x in [z[b'@2:Image Data'][0] for z in self.layers]:
-            print("\t"+x.decode(encoding))
+            print("\t" + x.decode(encoding))
 
-    def get_channel(self, channel="Height Sensor", backward=False, corr=None, debug=False, encoding='latin1', lazy=True):
+    def get_channel(self, channel="Height Sensor", backward=False, corr=None, debug=False, encoding='latin1',
+                    lazy=True):
         """
         Load the SPM image contained in a channel
         """
         for i in range(len(self.layers)):
             layer_name = self.layers[i][b'@2:Image Data'][0].decode(encoding)
             result = re.match(
                 r'([^ ]+) \[([^\]]*)\] "([^"]*)"', layer_name).groups()
             if result[2] == channel:
                 if debug:
-                    print("channel "+channel+" Found!")
+                    print("channel " + channel + " Found!")
                 bck = False
                 if self.layers[i][b'Line Direction'][0] == b'Retrace':
                     bck = True
                 if bck == backward:
                     if debug:
                         print("Direction found")
                     var = self.layers[i][b'@2:Z scale'][0].decode(encoding)
+                    if debug:
+                        print("@2:Z scale", var)
                     if '[' in var:
-                        result = re.match(r'[A-Z]+\s+\[([^\]]+)\]\s+\(-?[0-9\.]+ .*?\)\s+(-?[0-9\.]+)\s+(.*?)$', var).groups()
+                        result = re.match(r'[A-Z]+\s+\[([^\]]+)\]\s+\(-?[0-9\.]+ .*?\)\s+(-?[0-9\.]+)\s+(.*?)$',
+                                          var).groups()
                         if debug:
                             print(result)
-                        scale = float(result[1])/65536.0
-                        result2 = self.scanners[0][b'@'+result[0].encode(encoding)][0].split()
-                        scale2 = float(result[1])
-                        if len(result2)>2:
+                        bpp = int(self.layers[i][b'Bytes/pixel'][0])
+                        if debug:
+                            print("BPP", bpp)
+                        # scale = float(result[1])
+                        scale = float(result[1]) / 256 ** bpp
+
+                        result2 = self.scanners[0][b'@' + result[0].encode(encoding)][0].split()
+                        if debug:
+                            print("result2", result2)
+                        scale2 = float(result2[1])
+                        if len(result2) > 2:
                             zscale = result2[2]
                         else:
                             zscale = result2[0]
                         if b'/V' in zscale:
-                            zscale = zscale.replace(b'/V',b'')
+                            zscale = zscale.replace(b'/V', b'')
+                        if debug:
+                            print("scale: {:.3e}".format(scale))
+                            print("scale2: {:.3e}".format(scale2))
+                            print("zscale: " + str(zscale))
                         var = self.layers[i][b'@2:Z offset'][0].decode(encoding)
-                        result = re.match(r'[A-Z]+\s+\[[^\]]+\]\s+\(-?[0-9\.]+ .*?\)\s+(-?[0-9\.]+)\s+.*?$', var).groups()
+                        result = re.match(r'[A-Z]+\s+\[[^\]]+\]\s+\(-?[0-9\.]+ .*?\)\s+(-?[0-9\.]+)\s+.*?$',
+                                          var).groups()
                         offset = float(result[0])
                     else:
+                        if debug:
+                            print("mode 2")
                         result = re.match(r'[A-Z]+ \(-?[0-9\.]+ [^\)]+\)\s+(-?[0-9\.]+) [\w]+', var).groups()
-                        scale = float(result[0])/65536.0
+                        scale = float(result[0]) / 65536.0
                         scale2 = 1
                         zscale = b'V'
-                        result = re.match(r'[A-Z]+ \(-?[0-9\.]+ .*?\)\s+(-?[0-9\.]+) .*?', self.layers[i][b'@2:Z offset'][0].decode(encoding)).groups()
+                        result = re.match(r'[A-Z]+ \(-?[0-9\.]+ .*?\)\s+(-?[0-9\.]+) .*?',
+                                          self.layers[i][b'@2:Z offset'][0].decode(encoding)).groups()
                         offset = float(result[0])
-                    data = self._get_raw_layer(i)*scale*scale2
-
+                    if debug:
+                        print("Offset:", offset)
+                    data = self._get_raw_layer(i, debug=debug) * scale * scale2
+                    xres = int(self.layers[i][b"Samps/line"][0])
+                    yres = int(self.layers[i][b"Number of lines"][0])
+                    if debug:
+                        print("xres/yres", xres, yres)
                     scan_size = self.layers[i][b'Scan Size'][0].split()
+                    aspect_ratio = [int(x) for x in self.layers[i][b'Aspect Ratio'][0].split(b":")]
+                    if debug:
+                        print("aspect ratio", aspect_ratio)
                     if scan_size[2][0] == 126:
-                        scan_size[2] = b'u'+scan_size[2][1:]
+                        scan_size[2] = b'u' + scan_size[2][1:]
                     size = {
-                        'x': float(scan_size[0]),
-                        'y': float(scan_size[1]),
+                        'x': float(scan_size[0]) / aspect_ratio[1],
+                        'y': float(scan_size[1]) / aspect_ratio[0],
                         'unit': scan_size[2].decode(encoding)}
                     image = pySPM.SPM_image(
-                        channel=[channel,'Topography'][channel=='Height Sensor'],
+                        channel=[channel, 'Topography'][channel == 'Height Sensor'],
                         BIN=data,
                         real=size,
                         _type='Bruker AFM',
                         zscale=zscale.decode(encoding),
                         corr=corr)
                     return image
         if lazy:
-            return self.get_channel(channel=channel,backward=not backward, corr=corr, debug=debug, encoding=encoding, lazy=False)
+            return self.get_channel(channel=channel, backward=not backward, corr=corr, debug=debug, encoding=encoding,
+                                    lazy=False)
         raise Exception("Channel {} not found".format(channel))
```

### Comparing `pySPM-0.2.9/pySPM/collection.py` & `pyspm-0.3.0/pySPM/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 """
 collection is a module to handle collection of images.
 This is specially useful for SPM data which store several channels for the same measurement
 """
 
 import copy
 import re
-import numpy as np
+
 import matplotlib.pyplot as plt
-from .SPM import SPM_image
+import numpy as np
+
 from . import SPM
+from .SPM import SPM_image
 
 
 def atoi(text):
     """
     Convert string to integer
     """
     return int(text) if text.isdigit() else text
@@ -69,31 +71,31 @@
                 self.size['x'] = len(Img[0])
                 self.size['y'] = len(Img)
         if name in self.channels:
             if force:
                 del self.channels[name]
             else:
                 raise KeyError('The channel {} is already present in '
-                           'the collection. Please delete it before')
+                               'the collection. Please delete it before')
                 return
         self.channels[name] = Img
-        
+
     def create_image(self, img, key=None):
         return SPM_image(img, _type=self.name, real=self.size, channel=key)
 
     def __len__(self):
         return len(self.channels)
-        
+
     def __getitem__(self, key):
         if key not in self.channels:
             return None
         if isinstance(self.channels[key], SPM_image):
             return self.channels[key]
         return self.create_image(self.channels[key], key=key)
-        
+
     def __delitem__(self, key):
         del self.channels[key]
 
     def __iter__(self):
         self.iterator = iter(self.channels)
         return self
 
@@ -117,28 +119,28 @@
         """
         if channels is None:
             channels = list(self.channels.keys())
         channels_number = len(channels)
         assert channels_number > 0
         channels.sort(key=natural_keys)
         if ax is None:
-            if channels_number == 4:
+            if channels_number == 4 and ncols == 3:
                 fig, ax = plt.subplots(2, 2, figsize=(width,
                                                       self[channels[0]].pixels.shape[
-                                                          0]*width
+                                                          0] * width
                                                       / self[channels[0]].pixels.shape[1]))
             else:
-                Ny = (channels_number-1)//ncols+1
+                Ny = (channels_number - 1) // ncols + 1
                 Nx = min(ncols, channels_number)
                 fig, ax = plt.subplots(Ny, Nx,
-                                       figsize=(width, ((channels_number-1)//ncols+1)*width/Nx))
+                                       figsize=(width, ((channels_number - 1) // ncols + 1) * width / Nx))
         if type(ax) is not list:
-            ax = np.array(ax)
+            ax = np.array(ax).ravel()
         for i, x in enumerate(channels):
-            self[x].show(ax=ax.ravel()[i], cmap=cmap, **kargs)
+            self[x].show(ax=ax[i], cmap=cmap, **kargs)
         plt.tight_layout()
 
     def get_multivariate(self, channels=None):
         """
         Create and return a (pandas) DataFrame of the collection
         channels: List of the channels to use (default: None => all channels)
 
@@ -151,32 +153,32 @@
             data = pd.DataFrame(
                 {k: self.channels[k].pixels.ravel() for k in channels})
         else:
             data = pd.DataFrame(
                 {k: self.channels[k].ravel() for k in channels})
         return data
 
-    def overlay(self, channel_names, colors=[[1, 0, 0], [0,1,0],[0,0,1]],
+    def overlay(self, channel_names, colors=[[1, 0, 0], [0, 1, 0], [0, 0, 1]],
                 sig=None, vmin=None, vmax=None, **kargs):
         """
         Create an overlay (in color) of several channels.
         channel_names: a list of the channels to select for the overlay
         colors: List of [Red,Green,Blue] color to use.
             (Its length should be identical to channel_names)
         """
         assert len(channel_names) >= 2
         assert len(colors) >= len(channel_names)
         data = [SPM.normalize(
             self[ch].pixels, sig=sig, vmin=vmin, vmax=vmax)
             for ch in channel_names]
-        layers = [np.stack([data[i]*colors[i][j] for j in range(3)], axis=2)
+        layers = [np.stack([data[i] * colors[i][j] for j in range(3)], axis=2)
                   for i in range(len(channel_names))]
         overlay = np.clip(np.sum(layers, axis=0), 0, 1)
         o = self.create_image(overlay, key="overlay")
-        ch = [self.create_image(x, key=self[channel_names[i]].channel) for i,x in enumerate(layers)]
+        ch = [self.create_image(x, key=self[channel_names[i]].channel) for i, x in enumerate(layers)]
         if 'ax' in kargs:
             o.show(**kargs)
         return o, ch
 
     def stitch_correction(self, channel, stitches):
         """
         Function to correct for anomalies seen in stitched image.
@@ -187,26 +189,26 @@
             (take one with homogeneous intensities in the whole image)
         stitches: a tuple/list containing the number of stitches in the image (x,y)
         """
         result = copy.deepcopy(self)
         del result.channels
         result.channels = {}
         size = list(self.channels.values())[0]
-        S = np.zeros((size[0]/stitches[0], size[1]/stitches[1]))
+        S = np.zeros((size[0] / stitches[0], size[1] / stitches[1]))
         for i in range(stitches[0]):
             for j in range(stitches[1]):
-                S += self.channels[channel][sy*i:sy*(i+1), sx*j:sx*(j+1)]
+                S += self.channels[channel][sy * i:sy * (i + 1), sx * j:sx * (j + 1)]
         S[S == 0] = 1
         sy, sx = S.shape
         for x in self.channels:
             F = np.zeros(size)
             for i in range(stitches[0]):
                 for j in range(stitches[1]):
-                    F[sy*i:sy*(i+1), sx*j:sx*(j+1)] \
-                        = self.channels[x][sy*i:sy*(i+1), sx*j:sx*(j+1)]/S
+                    F[sy * i:sy * (i + 1), sx * j:sx * (j + 1)] \
+                        = self.channels[x][sy * i:sy * (i + 1), sx * j:sx * (j + 1)] / S
             result.add(F, x)
         return result
 
 
 def __Tsign(p1, p2, p3):
     return (p1[0] - p3[0]) * (p2[1] - p3[1]) - (p2[0] - p3[0]) * (p1[1] - p3[1])
 
@@ -218,15 +220,16 @@
     """
     b1 = __Tsign(pt, v1, v2) < 0
     b2 = __Tsign(pt, v2, v3) < 0
     b3 = __Tsign(pt, v3, v1) < 0
     return (b1 == b2) * (b2 == b3)
 
 
-def overlay_triangle(channel_names, colors=[[1,0,0],[0,1,0],[0,0,1]], radius=.8,proportion = .8,ax=None, size=512, bgcolor=[0,0,0], textcolor='white',fontsize=20):
+def overlay_triangle(channel_names, colors=[[1, 0, 0], [0, 1, 0], [0, 0, 1]], radius=.8, proportion=.8, ax=None,
+                     size=512, bgcolor=[0, 0, 0], textcolor='white', fontsize=20):
     """
     Create the image of a triangle, where the color is a gradient between three colors
     (one for each vertex).
 
     channel_names: a list of 3 channels
     colors: a list of 3 [R,G,B] list color
     ax: the matplotlib axis to plot in (if none use plt.gca())
@@ -234,29 +237,29 @@
         As there are in RGB no more than 256 values,
         the default value of 512 should be good in most of the cases.
     """
     assert len(channel_names) == 3
     assert len(colors) == 3
     if ax is None:
         ax = plt.gca()
-    RGB = [bgcolor[i]*np.ones((size, size)) for i in range(3)]
-    distance = 2*radius*proportion*np.sin(np.radians(120))
+    RGB = [bgcolor[i] * np.ones((size, size)) for i in range(3)]
+    distance = 2 * radius * proportion * np.sin(np.radians(120))
 
     x = np.linspace(-.7, 1.1, size)
     y = np.linspace(-1, 1, size)
     X, Y = np.meshgrid(x, y)
-    centers = [(radius*proportion*np.cos(np.radians(120*i)), radius *
-                proportion*np.sin(np.radians(120*i))) for i in range(3)]
-    dist = [np.sqrt((X-centers[i][0])**2+(Y-centers[i][1])**2)
+    centers = [(radius * proportion * np.cos(np.radians(120 * i)), radius *
+                proportion * np.sin(np.radians(120 * i))) for i in range(3)]
+    dist = [np.sqrt((X - centers[i][0]) ** 2 + (Y - centers[i][1]) ** 2)
             for i in range(3)]
 
     for j in range(3):
         RGB[j] = sum(
-            [colors[i][j]*np.maximum((distance-dist[i])/distance, 0) for i in range(3)])
-        ax.annotate(channel_names[j], (radius*np.cos(np.radians(120*j)), radius*np.sin(np.radians(120*j))),
+            [colors[i][j] * np.maximum((distance - dist[i]) / distance, 0) for i in range(3)])
+        ax.annotate(channel_names[j], (radius * np.cos(np.radians(120 * j)), radius * np.sin(np.radians(120 * j))),
                     color=textcolor,
                     fontsize=fontsize,
                     va="center",
                     ha="center")
         RGB[j][PointInTriangle([X, Y], *centers) == 0] = bgcolor[j]
     image = np.stack(RGB, axis=2)
     ax.imshow(image, extent=[x[0], x[-1], y[-1], y[0]])
```

### Comparing `pySPM-0.2.9/pySPM/ITA.py` & `pyspm-0.3.0/pySPM/ITA.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,97 +2,116 @@
 
 # Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
 
 """
 This module gives the ability to ready and parse the ToF-SIMS ITA files from iontof.
 You can mainly retrieve images and spectra for each channel and scan.
 """
+from __future__ import absolute_import
 
-import numpy as np
-import struct
 import os.path
-import zlib
 import re
-import copy
+import struct
+import zlib
+
+import numpy as np
 
+from .Block import MissingBlock
 from .ITM import ITM
 from .collection import Collection
-from .SPM import SPM_image
-from .Block import MissingBlock
-from .utils import in_ipynb
-import warnings
+from .utils.misc import deprecated, aliased, alias, PB
+
 
+@aliased
 class ITA(ITM):
-    def __init__(self, filename):
+    def __init__(self, filename, *args, **kargs):
         """
         Open an ITA file.
-        
+
         Parameters
         ----------
         filename : string
             the path of the ita file
-        
+
         Returns
         -------
         Class<ITA>
             ITA Object
 
         Examples
         --------
         >>> import pySPM
         >>> filename = "myfile.ita"
         >>> A = pySPM.ITA(filename)
         """
-        ITM.__init__(self, filename)
+        ITM.__init__(self, filename, *args, **kargs)
         try:
             self.sx = self.root.goto(
-                'filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScans/Image.XSize').getLong()
+                'filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScans/Image.XSize').get_ulong()
             self.sy = self.root.goto(
-                'filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScans/Image.YSize').getLong()
+                'filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScans/Image.YSize').get_ulong()
         except MissingBlock:
             self.sx = self.size['pixels']['x']
             self.sy = self.size['pixels']['y']
         try:
             # self.Nscan = int(self.root.goto('filterdata/TofCorrection/ImageStack/Reduced Data'\
             #    '/ImageStackScans/Image.NumberOfScans').getLong())
             self.Nimg = int(self.root.goto('filterdata/TofCorrection/ImageStack/Reduced Data'
-                                           '/ImageStackScans/Image.NumberOfImages').getLong())
+                                           '/ImageStackScans/Image.NumberOfImages').get_ulong())
         except:
-            try:
-                self.Nimg = self.root.goto('propend/Measurement.ScanNumber').getKeyValue()['int']
-            except:
-                raise TypeError(
-                    "Invalid file format. Maybe the file is corrupted?")
-        
-        self.img = self.getIntensity()
-        
+            self.Nimg = 0
+        self.img = self.get_intensity()
+
         try:
-            self.fov = self.root.goto('Meta/SI Image[0]/fieldofview').getDouble()
+            self.fov = self.root.goto('Meta/SI Image[0]/fieldofview').get_double()
         except MissingBlock:
-            self.fov = self.getValue("Registration.Raster.FieldOfView")['float']
+            self.fov = self.get_value("Registration.Raster.FieldOfView")['float']
+
+    @alias("getIntensity")
+    def get_intensity(self):
+        """
+        Retrieve the total Ion image
+        """
+        try:
+            X, Y = self.size['pixels']['x'], self.size['pixels']['y']
+            img = self.image(np.flipud(
+                np.array(self.root.goto('Meta/SI Image/intensdata').get_data("f"), dtype=np.float32).reshape((Y, X))),
+                channel="SI count")
+        except Exception as e:
+            try:
+                img = self.get_added_image(0).pixels
+            except:
+                try:
+                    img = self.get_added_image_by_SN(self.get_channel_SN("total"))
+                except:
+                    import warnings
+                    warnings.warn("SI image cannot be retrieved")
+                    return None
+        return img
 
     def get_channel_SN(self, channel):
         """
         New ITA fileformat assign a serial number (SN) in the form of a UUID for each channel.
         The SN corresponding to a given channel name can be retrieved by this function.
 
         Parameters
         ----------
         channel : string
             The channel name assigned to a given peak
         """
-        for x in  self.root.goto("MassIntervalList"):
+        for x in self.root.goto("MassIntervalList"):
             if x.name == 'mi':
-                l = x.dictList()
+                l = x.dict_list()
                 if l['assign']['utf16'] == channel or l['desc']['utf16'] == channel:
                     return l['SN']['utf16']
 
         raise Exception("Channel name \"{channel}\" not found".format(channel=channel))
 
-    def getChannelsByName(self, name, strict=False):
+    @alias("getChannelsByName")
+    def get_channels_by_name(self, name, strict=False):
         """
         Retrieve the channels for a given assignment name in the form of a list of dictionaries.
         The output can be formatted in a human readable way with the pySPM.ITA.showChannels function (see examples).
 
         Parameters
         ----------
         name : string or list of strings
@@ -112,15 +131,15 @@
                   of the rest 1 and the first peak is 2, ... )
                 - SN : an utf16 serial number which is useless for the end-used
                 - assign : a utf16 string with the element assignment of the
                   peak (e.g.: CH-, Na+, ...)
                 - lmass : a long value indicating the lower mass of the peak (in u)
                 - umass : a long value indicating the upper mass of the peak (in u)
                 - cmass : a long value indicating the center mass of the peak
-   
+
         Examples
         --------
         >>> A = pySPM.ITA("myfile.ita")
         >>> ch = A.getChannelsByName("C")
         >>> A.showChannels(ch)
         	CH- (), mass: 12.99 - 13.03
             C_2- (), mass: 23.97 - 24.03
@@ -143,28 +162,29 @@
         >>> ch = A.getChannelsByName("CH", True) # Only CH channel and not CHNO and CHO_2
         >>> A.showChannels(ch)
         	CH- (), mass: 12.99 - 13.03
         """
         res = []
         if strict:
             if type(name) in [list, tuple]:
-                name = ['^'+n+'[+-]?$' for n in name]
+                name = ['^' + n + '[+-]?$' for n in name]
             else:
-                name = '^'+name+'[+-]?$'
+                name = '^' + name + '[+-]?$'
         if type(name) is not list:
             name = [name]
         for n in name:
             for P in self.peaks:
                 p = self.peaks[P]
                 ma = re.compile(n, re.U)
                 if ma.match(p['assign']['utf16']) or ma.match(p['desc']['utf16']):
                     res.append(p)
         return res
 
-    def showChannels(self, ch):
+    @deprecated("showChannels")
+    def show_channels(self, ch):
         """
         Format a list of channels where each channel is represented by a dictionary (like the ones produced by pySPM.ITA.getChannelsByName) to a human readable output.
 
         Parameters
         ----------
         ch : list
             A list of dictionaries representing the channels
@@ -175,15 +195,16 @@
             It will print a list of channels with the assignment, the description in parenthesis followed by the lower - upper mass range.
         """
         for z in ch:
             print("\t{name} ({desc}), mass: {lower:.2f} - {upper:.2f}"
                   .format(desc=z['desc']['utf16'], name=z['assign']['utf16'],
                           lower=z['lmass']['float'], upper=z['umass']['float']))
 
-    def getChannelByMass(self, mass, full=False):
+    @alias("getChannelByMass")
+    def get_channel_by_mass(self, mass, full=False):
         """
         Retrieves the first channel ID which has a mass range containing a given mass.
 
         Parameters
         ---------
         mass : int, float
             The mass. If zero, the channel 0 will be returned and correspond to the Total count channel.
@@ -195,22 +216,23 @@
         int
             The first channel ID containing the mass given in argument. If a mass 0 is given, the output will be 0 which corresponds to the total count channel.
         """
         if mass == 0:
             return 0
         for P in self.peaks:
             p = self.peaks[P]
-            
+
             if p['id']['long'] > 1 and p['lmass']['float'] <= mass and mass <= p['umass']['float']:
                 if full:
                     return p
                 return p['id']['long']
         raise ValueError('Mass {:.2f} Not Found'.format(mass))
 
-    def getShiftCorrectedImageByName(self, names, **kargs):
+    @alias("getShiftCorrectedImageByName")
+    def get_shift_corrected_image_by_name(self, names, **kargs):
         """
         Retrieve the drift corrected (or shift corrected) image for the sum of all channels matching a given name. The shift correction applied is the one saved in the ITA file.
 
         Parameters
         ---------
         names : string or list of strings
             A channel name of a list of channel names to be summed up
@@ -219,57 +241,59 @@
         -------
         pySPM.SPM.SPM_image
             The image of the sum of all the selected channels
         list of dictionaries
             The list of all the channels selected. This list can be displayed in a human readable form by the pySPM.ITA.showChannels function
 
         """
-        return self.getSumImageByName(names, Shifts=[(-x,-y) for x,y in self.getSavedShift()],**kargs)
-        
-    def __getSumImage(self, scans, channels, **kargs):
+        return self.get_sum_image_by_name(names, shifts=[(-x, -y) for x, y in self.get_saved_shift()], **kargs)
+
+    def __get_sum_image(self, scans, channels, **kargs):
         """
         An internal function to retrieve the sum of several scans for several channel ID.
         """
         Z = np.zeros((self.sy, self.sx))
-        if 'Shifts' in kargs:
-            Shifts = kargs['Shifts']
+        if 'shifts' in kargs:
+            shifts = kargs['shifts']
+        elif 'Shifts' in kargs:
+            shifts = kargs['Shifts']
         else:
-            Shifts = [(-x,-y) for x,y in self.getSavedShift()]            
+            shifts = [(-x, -y) for x, y in self.get_saved_shift()]
         for ch in channels:
             ID = ch['id']['long']
-            Z += self.fastGetImage(ID, scans, Shifts)
+            Z += self.fast_get_image(ID, scans, shifts)
         return Z
 
-    def getSumImageBySN(self, SN, scans=None, prog=False, raw=False, **kargs):
+    @alias("getSumImageBySN")
+    def get_sum_image_by_sn(self, SN, scans=None, prog=False, raw=False, **kargs):
         """
         Retrieve the image for the sum of several scans for a given channel SN.
         """
         if scans is None:
             scans = range(self.Nscan)
         if type(scans) == int:
             scans = [scans]
         if prog:
-            try:
-                from tqdm import tqdm_notebook as tqdm
-            except:
-                from tqdm import tqdm
-            scans= tqdm(scans)
+            scans = PB(scans)
 
         Z = np.zeros((self.sy, self.sx))
         for s in scans:
-            node = self.root.goto("filterdata/TofCorrection/ImageStack/Reduced Data/Images/{SN}/ScanData/EDROff/{scan}".format(SN=SN, scan=s))
+            node = self.root.goto(
+                "filterdata/TofCorrection/ImageStack/Reduced Data/Images/{SN}/ScanData/EDROff/{scan}".format(SN=SN,
+                                                                                                             scan=s))
             dat = node.decompress()
-            data = struct.unpack("<{}I".format(len(dat)//4), dat)
-            Z += np.array(data, dtype=np.float).reshape((self.sy, self.sx))
+            data = struct.unpack("<{}I".format(len(dat) // 4), dat)
+            Z += np.array(data, dtype=np.float64).reshape((self.sy, self.sx))
         if raw:
             return Z
-        channel = self.getChannelBySN(SN)
+        channel = self.get_channel_by_sn(SN)
         return self.image(np.flipud(Z), channel=channel)
 
-    def getSumImageByName(self, names, scans=None, strict=False, prog=False, raw=False, **kargs):
+    @alias("getSumImageByName")
+    def get_sum_image_by_name(self, names, scans=None, strict=False, prog=False, raw=False, **kargs):
         """
         Retrieve the image for the sum of several scans and channels selected by their channel name.
 
         Parameters
         ----------
         names : string or list of strings
             Similar as for pySPM.ITA.getChannelsByName
@@ -282,23 +306,19 @@
         raw : bool
             If True a numpy array will be returned instead of a pySPM.SPM.SPM_image
         """
         if scans is None:
             scans = range(self.Nscan)
         if type(scans) == int:
             scans = [scans]
-        
-        channels = self.getChannelsByName(names, strict)
+
+        channels = self.get_added_image_by_name(names, strict)
         if prog:
-            try:
-                from tqdm import tqdm_notebook as tqdm
-            except:
-                from tqdm import tqdm
-            scans = tqdm(scans)
-        Z = self.__getSumImage(scans, channels)
+            scans = PB(scans)
+        Z = self.__get_sum_image(scans, channels)
         if raw:
             return Z, channels
         channel_title = ",".join([z['assign']['utf16'] for z in channels])
         return self.image(np.flipud(Z), channel=channel_title), channels
 
     def show(self, ax=None):
         """
@@ -312,45 +332,46 @@
         Returns
         -------
         None
         """
         import matplotlib.pyplot as plt
         if ax is None:
             fig, ax = plt.subplots(1, 1, figsize=(5, 5))
-        ax.imshow(self.img, extent=(0, self.fov*1e6, 0, self.fov*1e6))
+        ax.imshow(self.img, extent=(0, self.fov * 1e6, 0, self.fov * 1e6))
         ax.set_title("Total SI")
         ax.set_xlabel("x [$\mu$m]")
         ax.set_ylabel("y [$\mu$m]")
 
-    def getShiftsByMass(self, masses, centered=True, prog=False, Filter=None):
+    @alias("getShiftsByMass")
+    def get_shifts_by_mass(self, masses, centered=True, prog=False, Filter=None):
         """
         Deprecated. A relic function that the developer is not even sure what it was supposed to do ;)
         """
         Shifts = [(0, 0)]
         if Filter is None:
             Filter = lambda z: z
-        S0 = Filter(self.getSumImageByMass(masses, 0))
+        S0 = Filter(self.get_added_image_by_mass(masses, 0))
         Y = range(1, self.Nscan)
         if prog:
-            from tqdm import tqdm
-            Y = tqdm(Y)
+            Y = PB(Y)
         for i in Y:
-            S = Filter(self.getSumImageByMass(masses, i))
+            S = Filter(self.get_sum_image_by_mass(masses, i))
             Shift = np.real(np.fft.fftshift(np.fft.ifft2(
                 np.conj(np.fft.fft2(S0)) * np.fft.fft2(S))))
             cord = np.unravel_index(np.argmax(Shift), S0.shape)
-            trans = (cord[1]-S0.shape[1]/2, cord[0]-S0.shape[0]/2)
+            trans = (cord[1] - S0.shape[1] / 2, cord[0] - S0.shape[0] / 2)
             Shifts.append(trans)
         if centered:
             avSx = np.round(np.mean([z[0] for z in Shifts]))
             avSy = np.round(np.mean([z[1] for z in Shifts]))
-            Shifts = [(z[0]-avSx, z[1]-avSy) for z in Shifts]
+            Shifts = [(z[0] - avSx, z[1] - avSy) for z in Shifts]
         return Shifts
 
-    def getXsectionByMass(self, x1, y1, x2, y2, masses, N=None, prog=False, ax=None, flip=False, col='w-', **kargs):
+    @alias("getXsectionByMass")
+    def get_xsection_by_mass(self, x1, y1, x2, y2, masses, N=None, prog=False, ax=None, flip=False, col='w-', **kargs):
         """
         Retrieves a Cross-Section for a given mass along the profile determined by coordinates (x1,y1) and (x2,y2).
         The output is a 2D image where the x-axis correspond to the position along the profile and the y-axis the scan number.
 
         Parameters
         ----------
         x1 : int
@@ -375,39 +396,36 @@
             All supplementary arguments are passed to the pySPM.ITA.getSumImageByMass
 
         Returns
         -------
         np.ndarray
             2D numpy array containing the sum of all channels. The values are the count number
         """
-        y1 = self.sy-1-y1
-        y2 = self.sy-1-y2           
+        y1 = self.sy - 1 - y1
+        y2 = self.sy - 1 - y2
         if N is None:
-            N = int(np.sqrt((x2-x1)**2+(y2-y1)**2))+1
+            N = int(np.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2)) + 1
         x = np.linspace(x1, x2, N)
         y = np.linspace(y1, y2, N)
         out = np.zeros((self.Nscan, N))
         Y = range(self.Nscan)
         if ax is not None:
             if not flip:
-                ax.plot([x1, x2], [self.sy-1-y1, self.sy-1-y2], col)
+                ax.plot([x1, x2], [self.sy - 1 - y1, self.sy - 1 - y2], col)
         if prog:
-            try:
-                from tqdm import tqdm_notebook as tqdm
-            except:
-                from tqdm import tqdm as tqdm
-            Y = tqdm(Y)
+            Y = PB(Y)
         from scipy.ndimage import map_coordinates
         for s in Y:
-            Z = self.getSumImageByMass(masses, s, **kargs)
+            Z = self.get_sum_image_by_mass(masses, s, **kargs)
             P = map_coordinates(Z.pixels, np.vstack((y, x)))
             out[s, :] = P
         return out
 
-    def getAddedImageByName(self, names, strict=False, raw=False, **kargs):
+    @alias("getAddedImageByName")
+    def get_added_image_by_name(self, names, strict=False, raw=False, **kargs):
         """
         Retrieve the image for the sum of all scan (precomputed by iontof, but not shift-corrected) for given names
 
         Parameters
         ----------
         names : string or list of strings
             name of the channel (see pySPM.ITA.getChannelsByName)
@@ -423,76 +441,74 @@
         pySPM.SPM.SPM_image
             Image of the result
         list of dictionaries
             List of all selected peaks used to compute the image.
             Note: Pass this list to pySPM.ITA.showChannels in order to print a human readable representation of it.
         """
         Z = np.zeros((self.sy, self.sx))
-        channels = self.getChannelsByName(names, strict)
+        channels = self.get_channels_by_name(names, strict)
         for ch in channels:
             ID = ch['id']['long']
-            Z += self.getAddedImage(ID, **kargs)
+            Z += self.get_added_image(ID, **kargs)
         ch = self.get_masses(channels)
         if raw:
             return Z, ch
         return self.image(np.flipud(Z), channel=",".join([z['assign'] for z in ch])), ch
 
-    def getSavedShift(self):
+    @alias("getSavedShift")
+    def get_saved_shift(self):
         """
         getSavedShift returns the shifts saved with the file. Usually this is the shift correction you perform with the IonToF software.
 
         Returns
         -------
         List of tuples
             each tuple is a (Δx,Δy) in pixels (one for each scan).
         """
         try:
             X = zlib.decompress(self.root.goto('filterdata/TofCorrection/ImageStack/Reduced Data'
-                                           '/ImageStackScans/ShiftCoordinates/ImageStack.ShiftCoordinates').value)
+                                               '/ImageStackScans/ShiftCoordinates/ImageStack.ShiftCoordinates').value)
         except:
-            return [(0,0) for x in range(self.Nscan)]
-        D = struct.unpack('<'+str(len(X)//4)+'i', X)
+            return [(0, 0) for x in range(self.Nscan)]
+        D = struct.unpack('<' + str(len(X) // 4) + 'i', X)
         dx = D[::2]
         dy = D[1::2]
         return list(zip(dx, dy))
-        
-    def getShiftCorrectedImageByMass(self, masses, **kargs):
+
+    @alias("getShiftCorrectedImageByMass")
+    def get_shift_corrected_image_by_mass(self, masses, **kargs):
         """
-        Shortcut function for pySPM.ITA.getSumImageByMass using the saved shift corrections.
+        Shortcut function for pySPM.ITA.get_sum_image_by_mass using the saved shift corrections.
         """
-        return self.getSumImageByMass(masses, Shifts=[(-x,-y) for x,y in self.getSavedShift()], **kargs)
-        
-    def getSumImageByMass(self, masses, scans=None, prog=False, raw=False, **kargs):
+        return self.get_sum_image_by_mass(masses, shifts=[(-x, -y) for x, y in self.get_saved_shift()], **kargs)
+
+    @alias("getSumImageByMass")
+    def get_sum_image_by_mass(self, masses, scans=None, prog=False, raw=False, **kargs):
         """
         Similar to pySPM.ITA.getSumImageByName but instead of the names, the mass or list of mass is provided
         see pySPM.ITA.getSumImageByName for more details
         """
         if scans is None:
             scans = range(self.Nscan)
         if type(scans) is int:
             scans = [scans]
         if type(masses) is int or type(masses) is float:
             masses = [masses]
         if prog:
-            if in_ipynb():
-                try:
-                    from tqdm import tqdm_notebook as tqdm
-                except:
-                    from tqdm import tqdm
-            else:
-                from tqdm import tqdm
-            scans = tqdm(scans, leave=False)
-        channels = [self.getChannelByMass(m, full=True) for m in masses]
-        Z = self.__getSumImage(scans, channels, **kargs)
+            scans = PB(scans, leave=False)
+        channels = [self.get_channel_by_mass(m, full=True) for m in masses]
+        Z = self.__get_sum_image(scans, channels, **kargs)
         if raw:
             return Z, channels
-        channels_name = [["{:.2f}u".format(m['cmass']['float']),m['assign']['utf16']][m['assign']['utf16']!=''] for m in channels]
-        return self.image(np.flipud(Z), channel="Masses: "+",".join(channels_name))
+        channels_name = [["{:.2f}u".format(m['cmass']['float']), m['assign']['utf16']][m['assign']['utf16'] != ''] for m
+                         in channels]
+        return self.image(np.flipud(Z), channel="Masses: " + ",".join(channels_name))
 
-    def getAddedImageByMass(self, masses, raw=False, **kargs):
+    @alias("getAddedImageByMass")
+    def get_added_image_by_mass(self, masses, raw=False, **kargs):
         """
         Retrieve the image for the sum of all scan (precomputed by iontof, but not shift-corrected) for (a) given masse(s)
 
         Parameters
         ----------
         masses : float or list of float
             mass of the channels to be used
@@ -511,72 +527,76 @@
             Note: Pass this list to pySPM.ITA.showChannels in order to print a human readable representation of it.
         """
         if type(masses) is int or type(masses) is float:
             masses = [masses]
         Z = np.zeros((self.sy, self.sx))
         channels = []
         for m in masses:
-            ch = self.getChannelByMass(m)
+            ch = self.get_channel_by_mass(m)
             m = self.get_masses()[ch]
             if m['assign'] != '':
                 channels.append(m['assign'])
             else:
                 channels.append("{cmass:.2f}u".format(**m))
-            Z += self.getAddedImage(ch, **kargs)
+            Z += self.get_added_image(ch, **kargs)
         if raw:
             return Z, channels
         return self.image(np.flipud(Z), channel=",".join(channels))
 
-    def getChannelBySN(self, SN):
+    @alias("get_channel_by_sn", "getChannelBySN")
+    def get_channel_by_SN(self, SN):
         for node in self.root.goto("MassIntervalList"):
             if node.name == "mi":
-                l = node.dictList()
-                if l['SN']['utf16']==SN:
+                l = node.dict_list()
+                if l['SN']['utf16'] == SN:
                     name = l['assign']['utf16']
                     if not name:
                         name = l['desc']['utf16']
                     if not name:
                         name = '{:.2f}u'.format(l['cmass']['float'])
                     return name
 
-    def getAddedImageBySN(self, SN, raw=False):
+    @alias("get_added_image_by_sn", "getAddedImageBySN")
+    def get_added_image_by_SN(self, SN, raw=False):
         """
         New ITA fileformat save images with their respective serial number (SN).
         This function return the image for a given SN.
 
         Parameters
         ----------
 
         SN: Serial Number of the channel
         """
-        node = self.root.goto("filterdata/TofCorrection/ImageStack/Reduced Data/Images/{SN}/SumImage/EDROff".format(SN=SN))
+        node = self.root.goto(
+            "filterdata/TofCorrection/ImageStack/Reduced Data/Images/{SN}/SumImage/EDROff".format(SN=SN))
         dat = node.decompress()
-        data = struct.unpack("<{}I".format(len(dat)//4), dat)
-        img = np.array(data, dtype=np.float).reshape((self.sy, self.sx))
+        data = struct.unpack("<{}I".format(len(dat) // 4), dat)
+        img = np.array(data, dtype=np.float64).reshape((self.sy, self.sx))
         if raw:
             return img
-        channel = self.getChannelBySN(SN)
+        channel = self.get_channel_by_SN(SN)
         return self.image(np.flipud(img), channel=channel)
 
-
-    def getAddedImage(self, channel, **kargs):
+    @alias("getAddedImage")
+    def get_added_image(self, channel, **kargs):
         """
         Retrieve the numpy 2D array of a given channel ID for the sum of all scan (precomputed by iontof, but not shift-corrected)
         Note: It is preferable to use the pySPM.ITA.getAddedImageByMass or pySPM.ITA.getAddedImageByName
         """
         assert type(channel) is int
         assert channel >= 0 and channel < self.Nimg
         c = self.root.goto('filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScansAdded'
-                           '/Image['+str(channel)+']/ImageArray.Long')
+                           '/Image[' + str(channel) + ']/ImageArray.Long')
         D = zlib.decompress(c.value)
-        V = np.array(struct.unpack('<'+str(self.sx*self.sy)+'I', D),
-                     dtype=np.float).reshape((self.sy, self.sx))
+        V = np.array(struct.unpack('<' + str(self.sx * self.sy) + 'I', D),
+                     dtype=np.float64).reshape((self.sy, self.sx))
         return V
-    
-    def fastGetImage(self, channel, scans, Shifts=False, prog=False):
+
+    @alias("fastGetImage")
+    def fast_get_image(self, channel, scans, shifts=False, prog=False, **kargs):
         """
         Retieve a 2D numpy array corresponding to a given channel ID for given scan(s) and return their sum.
 
         Parameters
         ----------
         channel : int
             The channel ID
@@ -589,42 +609,39 @@
             Display a progressbar ?
 
         Returns
         -------
         2D numpy array
             array data of the image
         """
+        # Old parameter name compatibility
+        if 'Shifts' in kargs:
+            shifts = kargs.pop("Shifts")
+
         Z = np.zeros((self.sy, self.sx))
         if prog:
-            try:
-                from tqdm import tqdm_notebook as tqdm
-                scans = tqdm(scans)
-            except:
-                warning.warn("tqdm_notebook not available")
-                try:
-                    from tqdm import tqdm
-                    scans = tqdm(scans)
-                except:
-                    warning.warn("cannot load tqdm library")
-            
-        im_root =  self.root.goto('filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScans/Image['+str(channel)+']')
+            scans = PB(scans)
+
+        im_root = self.root.goto(
+            'filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScans/Image[' + str(channel) + ']')
         for scan in scans:
-            c = im_root.goto('ImageArray.Long['+str(scan)+']')
-            V = np.array(c.getData('I'), dtype=np.float).reshape((self.sy, self.sx))
-            if Shifts:
-                r = [int(z) for z in Shifts[scan]]
+            c = im_root.goto('ImageArray.Long[' + str(scan) + ']')
+            V = np.array(c.get_data('I'), dtype=np.float64).reshape((self.sy, self.sx))
+            if shifts:
+                r = [int(z) for z in shifts[scan]]
                 V = np.roll(np.roll(V, -r[0], axis=1), -r[1], axis=0)
-                rx = [max(0,-r[0]), self.sx-max(1,r[0])]
-                ry = [max(0,-r[1]), self.sy-max(1,r[1])]
-                Z[ry[0]:ry[1],rx[0]:rx[1]] += V[ry[0]:ry[1],rx[0]:rx[1]]
+                rx = [max(0, -r[0]), self.sx - max(1, r[0])]
+                ry = [max(0, -r[1]), self.sy - max(1, r[1])]
+                Z[ry[0]:ry[1], rx[0]:rx[1]] += V[ry[0]:ry[1], rx[0]:rx[1]]
             else:
                 Z += V
         return Z
-        
-    def getImage(self, channel, scan, Shifts=None, ShiftMode='roll', const=0):
+
+    @alias("getImage")
+    def get_image(self, channel, scan, shifts=None, shift_mode='roll', const=0, **kargs):
         """
         getImage retrieve the image of a specific channel (ID) and a specific scan.
 
         Parameters
         ----------
         channel : int
             channel ID
@@ -636,66 +653,178 @@
         ShiftMode :  string
             roll : roll the data over. easy but non-physical
             const : replace missing values by a constant (given by argument const)
             NaN : the same as const but with const=numpy.NaN
         const : float
             if ShiftMode is 'const' then this parameter defines the constant used (default 0)
         """
+        # Compatibility with old parameter names
+        if 'Shifts' in kargs:
+            shifts = kargs.pop("Shifts")
+        if 'ShiftMode' in kargs:
+            shift_mode = kargs.pop("ShiftMode")
+
         assert type(channel) is int
         assert type(scan) is int
         assert channel >= 0 and channel < self.Nimg
         assert scan >= 0 and scan < self.Nscan
         c = self.root.goto('filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScans'
-                           '/Image['+str(channel)+']/ImageArray.Long['+str(scan)+']')
-        V = np.array(c.getData(self.sx*self.sy), dtype=np.float).reshape((self.sy, self.sx))
-        if not Shifts is None:
-            r = [int(z) for z in Shifts[scan]]
+                           '/Image[' + str(channel) + ']/ImageArray.Long[' + str(scan) + ']')
+        V = np.array(c.get_data(), dtype=np.float64).reshape((self.sy, self.sx))
+        if not shifts is None:
+            r = [int(z) for z in shifts[scan]]
             V = np.roll(np.roll(V, -r[0], axis=1), -r[1], axis=0)
-            if ShiftMode == 'const' or ShiftMode == 'NaN':
-                if ShiftMode == 'NaN':
+            if shift_mode == 'const' or shift_mode == 'NaN':
+                if shift_mode == 'NaN':
                     const = np.nan
                 if r[1] < 0:
                     V[:-r[1], :] = const
                 elif r[1] > 0:
                     V[-r[1]:, :] = const
                 if r[0] < 0:
                     V[:, :-r[0]] = const
                 elif r[0] > 0:
                     V[:, -r[0]:] = const
         return V
-        
-    def showSpectrumAround(self, m0, delta=0.15, sf=None, k0=None, **kargs):
+
+    @alias("getOperation")
+    def get_opertion(self, OpID):
+        """
+        Test function to retrieve the operations used in the Worksheet.
         """
-        Display the Spectrum around a given mass.
+        Nop = self.root.goto('Presentation/Imaging Worksheet/Worksheet/OPERATIONS/OpCount').get_ulong()
+        for i in range(Nop):
+            blk = self.root.goto('Presentation/Imaging Worksheet/Worksheet/OPERATIONS/Operation[{}]'.format(i))
+            if blk.goto_item('OpID').get_ulong() == OpID:
+                return blk
+        return None
+
+    @alias("showWorksheet")
+    def show_worksheet(self, page=0):
+        """
+        In Dev. function to display the worksheet
+        """
+        import matplotlib as mpl
+        from .utils import sp
+        num_pages = self.root.goto('Presentation/Imaging Worksheet/Worksheet/PAGES/COUNT').get_ulong()
+        assert page < num_pages
+        Nitems = self.root.goto(
+            'Presentation/Imaging Worksheet/Worksheet/PAGES/Page[{}]/ItemCount'.format(page)).get_ulong()
+        sett = self.root.goto(
+            'Presentation/Imaging Worksheet/Worksheet/PAGES/Page[{}]/SETTINGS'.format(page)).dict_list()
+        Nx = sett['Xsize']['ulong']
+        Ny = sett['Ysize']['ulong']
+        items = self.root.goto('Presentation/Imaging Worksheet/Worksheet/PAGES/Page[{}]/Items'.format(page)).get_data()
+        ax = sp(len(items))
+        IntV = {}
+        for x in self.root.goto("MassIntervalList"):
+            if x.name == 'mi':
+                d = x.dict_list()
+                IntV[d['id']['long']] = d['desc']['utf16'] + d['assign']['utf16']
+        for i, it in enumerate(items):
+            blk = self.get_operation(it)
+            OPTYPE = blk.goto_item('OPTYPE').get_ulong()
+            while OPTYPE != 3:
+                OPTYPE = blk.goto_item('OPTYPE').get_ulong()
+                if OPTYPE == 4:
+                    blk = self.getOperation(blk.goto_item('ArgOpIDs').get_ulong())
+                elif OPTYPE == 3:
+                    palette = np.array(blk.goto_item('BMP-Palette').get_data('B')).reshape((256, 4))
+                    B, G, R = palette[:, 0], palette[:, 1], palette[:, 2]
+                    dimx = blk.goto('Cache/IImage-Cache-DimX').get_ulong()
+                    dimy = blk.goto('Cache/IImage-Cache-DimY').get_ulong()
+                    img = np.array(blk.goto('Cache/IImage-Cache-Intensities').get_data('d')).reshape((dimy, dimx))
+                    RGB = np.hstack([R[:, None], G[:, None], B[:, None]]) / 256
+                    cm = mpl.colors.ListedColormap(RGB)
+                    ax[i].imshow(img, cmap=cm)
+
+    def add_new_images(self, miblock, scans=None, added=None, prog=False, **kargs):
+        # Compatibility with old parameter names
+        if 'Scans' in kargs:
+            scans = kargs.pop("Scans")
+        if 'Added' in kargs:
+            added = kargs.pop("Added")
+
+        assert scans is not None or added is not None
+        lvl = 3  # zlib encoding level
+        sy, sx = self.size['pixels']['y'], self.size['pixels']['x']
+        SN = miblock.goto("SN").get_string()
+        if added is None:
+            added_img = np.zeros((sy, sx), dtype=np.uint32)
+        chID = miblock.goto("id").get_ulong()
+        if scans is not None:
+            N = self.root.goto(
+                "filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScans/Image.NumberOfImages").get_ulong()
+        AN = self.root.goto(
+            "filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScansAdded/Image.NumberOfImages").get_ulong()
+        self.root.edit_block(
+            "filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScansAdded/Image[{}]".format(AN),
+            "Image.MassIntervalSN", SN.encode('utf8'))
+        self.root.edit_block(
+            "filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScansAdded/Image[{}]".format(AN), "Image.XSize",
+            struct.pack("<I", sx))
+        self.root.edit_block(
+            "filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScansAdded/Image[{}]".format(AN), "Image.YSize",
+            struct.pack("<I", sy))
+        if scans is not None:
+            RS = range(self.Nscan)
+            if prog:
+                RS = PB(RS)
+            for i in RS:
+                img = np.flipud(scans[i].astype(np.uint32, casting='unsafe'))
+                data = zlib.compress(struct.pack("<{}I".format(sx * sy), *np.ravel(img)), level=lvl)
+                self.root.edit_block(
+                    "filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScans/Image[{}]".format(N),
+                    "ImageArray.Long", data, id=i, _type=128)
+                if added is None:
+                    added_img += img
 
-        Parameters
-        ----------
-        m0 : float
-            The central mass around which the spectrum will be plotted (in u)
-        delta : float
-            The spectrum will be plotted between m0-delta and m0+delta
-        sf : float or None
-        k0 : float or None
-            sf and k0 are the mass calibration parameters. If None values saved with the file will be used.
-        **kargs : supplementary arguments
-            Passed to pySPM.utils.showPeak
-        """
-        polarity = '+'
-        if self.getValue('Instrument.Analyzer_Polarity_Switch')['string'] == 'Negative':
-            polarity = '-'
-        from . import utils
-        m, D = self.getSpectrum(sf=sf, k0=k0)
-        return utils.showPeak(m, D, m0, delta, polarity=polarity, **kargs)
+        if added is None:
+            added = added_img
+        else:
+            added = np.flipud(added)
+        data = zlib.compress(struct.pack("<{}I".format(sx * sy), *np.ravel(added.astype(np.uint32, casting='unsafe'))),
+                             level=lvl)
+        self.root.edit_block(
+            "filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScansAdded/Image[{}]".format(AN),
+            "ImageArray.Long", data, _type=128)
+
+        self.root.edit_block(
+            "filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScansAdded/Image[{}]".format(AN),
+            "Image.PulsesPerPixel", struct.pack("<I", self.spp * self.Nscan))
+        self.root.edit_block(
+            "filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScansAdded/Image[{}]".format(AN),
+            "Image.MaxCountsPerPixel", struct.pack("<I", int(np.max(added))))
+        self.root.edit_block(
+            "filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScansAdded/Image[{}]".format(AN),
+            "Image.MinCountsPerPixel", struct.pack("<I", int(np.min(added))))
+        self.root.edit_block(
+            "filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScansAdded/Image[{}]".format(AN),
+            "Image.TotalCountsDbl", struct.pack("<d", np.sum(added)))
+        self.root.edit_block(
+            "filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScansAdded/Image[{}]".format(AN),
+            "Image.TotalCounts", struct.pack("<I", int(np.sum(added))))
+
+        if scans is not None:
+            self.root.edit_block("filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScans",
+                                 "Image.NumberOfImages", struct.pack("<I", N + 1))
+        self.root.edit_block("filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScansAdded",
+                             "Image.NumberOfImages", struct.pack("<I", AN + 1))
+        self.Nimg += 1
 
+
+@aliased
 class ITA_collection(Collection):
     """
     ITA_collection is a super class containing a collection of tof-sims images.
     for details on Collection see pySPM.collection.Collection
     """
-    def __init__(self, filename, channels1=None, channels2=None, name=None, mass=False, strict=False):
+
+    def __init__(self, filename, channels1=None, channels2=None, name=None, mass=False, strict
+    =False):
         """
         Opening a ToF-SIMS ITA file as an image collection
 
         Parameters
         ----------
         filename : string
             The filename
@@ -715,15 +844,15 @@
         """
         self.ita = ITA(filename)
         self.filename = filename
         self.PCA = None
         if name is None:
             name = os.path.basename(filename)
         self.name = name
-        Collection.__init__(self, sx=self.ita.fov, sy=self.ita.fov*self.ita.sy/self.ita.sx,
+        Collection.__init__(self, sx=self.ita.fov, sy=self.ita.fov * self.ita.sy / self.ita.sx,
                             unit='m', name=name)
         self.msg = ""
         if channels1 is None:
             mass = True
             masses = self.ita.get_masses()
             channels1 = [x['cmass'] for x in masses if x['id'] > 1]
         CHS = [channels1]
@@ -732,40 +861,40 @@
         for channels in CHS:
             if channels is channels2:
                 strict = False
             if type(channels) is list:
                 for x in channels:
                     if mass:
                         try:
-                            I = self.ita.getAddedImageByMass(x)
-                            m = masses[2+channels1.index(x)]
+                            I = self.ita.get_added_image_by_mass(x)
+                            m = masses[2 + channels1.index(x)]
                             if m['assign'] != '':
                                 self.add(I, m['assign'])
                             else:
                                 self.add(I, "{cmass:.2f}u".format(cmass=x))
                         except:
                             pass
                     else:
-                        Z, ch = self.ita.getAddedImageByName(x, strict)
+                        Z, ch = self.ita.get_added_image_by_name(x, strict)
                         self.msg += "{0}\n".format(x)
                         for z in ch:
-                            self.msg += "\t{name} ({desc}), mass: {lower:.2f} - {upper:.2f}\n"\
+                            self.msg += "\t{name} ({desc}), mass: {lower:.2f} - {upper:.2f}\n" \
                                 .format(desc=z['desc'], name=z['assign'],
                                         lower=z['lmass'], upper=z['umass'])
                         self.add(Z, x)
             elif type(channels) is dict:
                 for x in channels:
                     if mass:
-                        self.add(self.ita.getAddedImageByMass(channels[x]), x)
+                        self.add(self.ita.get_added_image_by_mass(channels[x]), x)
                     else:
-                        Z, ch = self.ita.getAddedImageByName(
+                        Z, ch = self.ita.get_added_image_by_name(
                             channels[x], strict)
                         self.msg += "{0}\n".format(x)
                         for z in ch:
-                            self.msg += "\t{name} ({desc}), mass: {lower:.2f} - {upper:.2f}\n"\
+                            self.msg += "\t{name} ({desc}), mass: {lower:.2f} - {upper:.2f}\n" \
                                 .format(desc=z['desc'], name=z['assign'],
                                         lower=z['lmass'], upper=z['umass'])
                         self.add(Z, x)
             else:
                 raise TypeError(
                     "Channels should be a list or a dictionnary. Got {}".format(type(channels)))
 
@@ -779,50 +908,52 @@
         >>> A['Au-']
         <pySPM.SPM.SPM_image at 0x????????>
         """
         if key not in self.channels:
             return None
         return self.channels[key]
 
-    def runPCA(self, channels=None):
+    @alias("runPCA")
+    def run_pca(self, channels=None):
         """
         Perform a Principle Component Analysis (PCA) on the channels
 
         Parameters
         ----------
         channels : None or list of strings
             List of channels to use for the PCA. If None all channels will be used.
         """
-        from pySPM import PCA
+        from .PCA import ITA_PCA
         if channels is None:
             channels = self.channels.keys()
-        self.PCA = PCA.ITA_PCA(self, channels)
+        self.PCA = ITA_PCA(self, channels)
 
-    def showPCA(self, num=None, **kargs):
+    @alias("showPCA")
+    def show_pca(self, num=None, loadings=True, **kargs):
         """
         Run PCA if not already done and display the PCA images.
 
         Parameters
         ----------
         num : int or None
             The number of PC component to display. If None display all PAs
         **kargs : additional parameters
             passed to pySPM.PCA.showPCA
-        
+
         Returns
         -------
         None
             Plot num PCA into a 1×num subplots
 
         """
         if self.PCA is None:
-            self.runPCA()
-        self.PCA.showPCA(num=num, **kargs)
+            self.run_pca()
+        self.PCA.show_pca(num=num, loadings=loadings, **kargs)
 
-    def loadings(self, num=None):
+    def loadings(self, num=None, ax=None):
         """
         Return a pandas DataFrame with the num first loadings
 
         Parameters
         ----------
         num : int or None
             The number of PC to use. If None use all PCs
@@ -833,20 +964,28 @@
         >>> col = pySPM.ITA_collection("myfile.ita")
         >>> L = col.loadings(3)
         >>> col.PCA.hincton(matrix=L)
         Display a hinton plot with num lines representing the strength of each loading. Blue means negative loadings and Red means positive ones.
         The size of each square is proportional to the absolute value of each loading.
         """
         if self.PCA is None:
-            self.runPCA()
+            self.run_pca()
         if num is None:
-            return self.PCA.loadings()
-        return self.PCA.loadings()[:num]
+            L = self.PCA.loadings()
+        else:
+            L = self.PCA.loadings()[:num]
+        if ax is not None:
+            if ax is True:
+                self.PCA.hinton(matrix=L)
+            else:
+                self.PCA.hinton(matrix=L, ax=ax)
+        return L
 
-    def StitchCorrection(self, channel, stitches, gauss=0, debug=False):
+    @deprecated("StitchCorrection")
+    def stitch_correction(self, channel, stitches, gauss=0, debug=False):
         """
         When an image is created by stitching of several images (while moving the stage during the measurement) the resulting image can have several artifacts due to charging.
         The goal of this function is the try to suppress this stitching artifacts by givings a channel name which is known to be homogeneous everywhere
 
         Parameters
         ----------
         channel : string
@@ -864,27 +1003,27 @@
             A new collection with corrected data
 
         """
         import copy
         from scipy.ndimage.filters import gaussian_filter
         N = ITA_collection(self.filename, [], name=self.name)
         size = list(self.channels.values())[0].pixels.shape
-        S = np.zeros((int(size[0]/stitches[0]), int(size[1]/stitches[1])))
+        S = np.zeros((int(size[0] / stitches[0]), int(size[1] / stitches[1])))
         sy, sx = S.shape
         for i in range(stitches[0]):
             for j in range(stitches[1]):
-                S += self.channels[channel].pixels[sy*i:sy*(i+1), sx*j:sx*(j+1)]
+                S += self.channels[channel].pixels[sy * i:sy * (i + 1), sx * j:sx * (j + 1)]
         S[S == 0] = 1
-        if gauss>0:
+        if gauss > 0:
             S = gaussian_filter(S, gauss)
         for x in self.channels:
             F = np.zeros(size)
             for i in range(stitches[0]):
                 for j in range(stitches[1]):
-                    F[sy*i:sy*(i+1), sx*j:sx*(j+1)] = \
-                        self.channels[x].pixels[sy*i:sy*(i+1), sx*j:sx*(j+1)]/S
+                    F[sy * i:sy * (i + 1), sx * j:sx * (j + 1)] = \
+                        self.channels[x].pixels[sy * i:sy * (i + 1), sx * j:sx * (j + 1)] / S
             new_channel = copy.deepcopy(self[x])
             new_channel.pixels = F
             N.add(new_channel, x)
         if debug:
             return N, S
         return N
```

### Comparing `pySPM-0.2.9/pySPM/ITAslicer.py` & `pyspm-0.3.0/pySPM/ITAslicer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,175 +1,177 @@
-# -- coding: utf-8 --
-
-# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
-
-"""
-This is a standalone script which allows the user to perfome cross-section on ToF-SIMS images on different channels
-"""
-
-import sys
-from PyQt5.QtWidgets import QApplication, QMainWindow, QTableWidgetItem, QFileDialog, QWidget, QAction, QProgressBar, QStatusBar
-from PyQt5.QtGui import QPixmap
-from PyQt5.QtCore import Qt, QCoreApplication
-from slicer import Ui_slicer
-import os
-import re
-import pySPM
-import numpy as np
-from pySPM.utils import CDF
-from scipy import optimize as opt
-
-class SlicerApp(QWidget):
-    def __init__(self, filename=None):
-        super(QWidget, self).__init__()
-        self.ui = Ui_slicer()
-        self.ui.setupUi(self)
-        
-        self.canvas = self.ui.mpl.canvas
-        self.fig = self.ui.mpl.canvas.fig
-        self.initPlotLayout()
-        self.level = None
-        if filename is None:
-            if len(sys.argv) < 2:
-                self.path, _ = QFileDialog.getOpenFileName(self,"ITA Image", "","(*.ITA)")
-            else:
-                # If an argument is sent to the script, the first argument will be used as a Path. Very usefull for debugging the script without having to selectr the folder each time with window dialog
-                self.path = sys.argv[1]
-        else:
-            self.path = filename
-        if not os.path.exists(self.path):
-            raise Exception("File \"{}\" is not found".format(self.path))
-        if os.path.exists(self.path+".level.npy"):
-            self.level = np.load(self.path+".level.npy")
-        self.curs = [0,0,0]
-        self.volume = None
-        self.ITA = pySPM.ITA(self.path) 
-        for i,x in enumerate(self.ITA.get_masses()):
-            self.ui.peakList.setRowCount(i+1)
-            self.ui.peakList.setItem(i, 0, QTableWidgetItem(x['assign']))
-            self.ui.peakList.setItem(i, 1, QTableWidgetItem("{:.2f}u".format((x['cmass']))))
-            self.ui.peakList.setItem(i, 2, QTableWidgetItem("{:.2f}u".format(x['umass'] - x['lmass'])))
-        self.ui.peakList.show()
-        self.ui.cmap.currentIndexChanged.connect(self.plot)
-        self.ui.prof1daxis.currentIndexChanged.connect(self.plot)
-        self.ui.peakList.cellClicked.connect(self.load_channel)
-        self.canvas.mpl_connect('button_press_event', self.on_pick)
-        self.flatAction = QAction("Flatten substrate from this channel")
-        self.flatAction.triggered.connect(self.flatten)
-        self.ui.correction.stateChanged.connect(self.plot)
-        self.ui.peakList.addAction(self.flatAction)
-        self.ui.status.setText("IDLE")
-    
-    def flatline(self, y):
-        for x in range(self.volume.shape[1]):
-            popt, pcov = opt.curve_fit(CDF, np.arange(self.volume.shape[2]), self.volume[y,x,:], (10, self.volume.shape[2]/2, 1))
-            self.level[y, x] = popt[1]
-         
-    def flatten(self):
-        from scipy import optimize as opt
-        self.ui.status.setText("Start the flattening...")
-        self.level = np.zeros(self.volume.shape[:2])
-        self.ui.pb.setMaximum(self.volume.shape[0])
-        for y in range(self.volume.shape[0]):
-            self.ui.pb.setValue(y)
-            self.flatline(y)
-            QCoreApplication.processEvents()
-            self.ax.clear()
-            self.ax.imshow(self.level)
-            self.canvas.draw()
-        self.ui.pb.setValue(0)
-        self.ui.status.setText("Flattening finished")
-        np.save(self.path+".level", self.level)
-        
-    def load_channel(self, row, col):
-        self.ui.status.setText("Loading channel...")
-        id = row
-        vol = []
-        for i in range(self.ITA.Nscan):
-            x = self.ITA.getImage(id, i)
-            vol.append(x)
-        self.volume = np.stack([x for x in vol], axis=2)
-        if not self.level is None:
-            self.corrected = np.zeros(self.volume.shape)
-            z = np.arange(self.ITA.Nscan)
-            self.ui.pb.setMaximum(self.level.shape[0])
-            for y in np.arange(self.level.shape[0]):
-                self.ui.pb.setValue(y)
-                for x in np.arange(self.level.shape[1]):
-                    dz = int(-self.level[y,x] + np.max(self.level))
-                    self.corrected[y,x,dz:] = self.volume[y,x,:self.volume.shape[2]-dz]
-            self.ui.pb.setValue(0)
-        self.plot()
-        self.ui.status.setText("IDLE")
-        
-    def plot(self):
-        if self.ui.correction.isChecked():
-            A = self.corrected
-        else:
-            A = self.volume
-        cmap = self.ui.cmap.currentText()
-        self.axXY.clear()
-        self.axXZ.clear()
-        self.axYZ.clear()
-        self.ax.clear()
-        if self.volume is None:
-            return
-        self.axXY.imshow(A[:,:,self.curs[2]],cmap=cmap)
-        self.axXZ.imshow(A[self.curs[1],:,:].T,cmap=cmap)
-        self.axYZ.imshow(A[:,self.curs[0],:].T,cmap=cmap)
-        self.axXY.axhline(self.curs[1])
-        self.axXY.axvline(self.curs[0])
-        self.axXZ.axhline(self.curs[2])
-        self.axXZ.axvline(self.curs[0])
-        self.axYZ.axhline(self.curs[2])
-        self.axYZ.axvline(self.curs[1])
-        self.axXY.set_title("XY")
-        self.axXZ.set_title("XZ")
-        self.axYZ.set_title("YZ")
-        if self.ui.prof1daxis.currentText() in 'XYZ':
-            i = 'XYZ'.index(self.ui.prof1daxis.currentText())
-            self.ax.set_xlabel("XYZ"[i])
-            if i==0:
-                self.ax.plot(A[:,self.curs[0],self.curs[2]])
-            elif i==1:
-                self.ax.plot(A[self.curs[1],:,self.curs[2]])
-            elif i==2:
-                self.ax.plot(A[self.curs[1],self.curs[0],:])
-        self.canvas.draw()
-        
-    def on_pick(self, event):
-        if not event.inaxes in [self.axYZ,self.axXZ,self.axXY]:
-            return
-        x = event.xdata
-        y = event.ydata
-        axis = [self.axYZ,self.axXZ,self.axXY].index(event.inaxes)
-        xdata = int(x)
-        ydata = int(y)
-        
-        if event.inaxes == self.axXY:
-            self.curs[0] = xdata
-            self.curs[1] = ydata
-        elif event.inaxes == self.axYZ:
-            self.curs[1] = xdata
-            self.curs[2] = ydata
-        elif event.inaxes == self.axXZ:
-            self.curs[0] = xdata
-            self.curs[2] = ydata
-        else:
-            print("Click event not handled")
-        self.curs = [np.clip(0,self.curs[i],self.volume.shape[i]-1) for i in range(3)]
-        self.plot()
-        
-    def initPlotLayout(self):
-        """
-        Setup the plotting layout.
-        """
-        self.axXY = self.fig.add_subplot(2,2,1)
-        self.axYZ = self.fig.add_subplot(2,2,2)
-        self.axXZ = self.fig.add_subplot(2,2,3)
-        self.ax = self.fig.add_subplot(2,2,4)
-        self.fig.tight_layout()
-
-app = QApplication(sys.argv)
-window = SlicerApp()
-window.show()
-sys.exit(app.exec_())
+# -- coding: utf-8 --
+
+# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
+
+"""
+This is a standalone script which allows the user to perfome cross-section on ToF-SIMS images on different channels
+"""
+
+import os
+import sys
+
+import numpy as np
+from PyQt5.QtCore import QCoreApplication
+from PyQt5.QtWidgets import QApplication, QTableWidgetItem, QFileDialog, QWidget, QAction
+from scipy import optimize as opt
+
+import pySPM
+from pySPM.utils import CDF
+from slicer import Ui_slicer
+
+
+class SlicerApp(QWidget):
+    def __init__(self, filename=None):
+        super(QWidget, self).__init__()
+        self.ui = Ui_slicer()
+        self.ui.setupUi(self)
+
+        self.canvas = self.ui.mpl.canvas
+        self.fig = self.ui.mpl.canvas.fig
+        self.initPlotLayout()
+        self.level = None
+        if filename is None:
+            if len(sys.argv) < 2:
+                self.path, _ = QFileDialog.getOpenFileName(self, "ITA Image", "", "(*.ITA)")
+            else:
+                # If an argument is sent to the script, the first argument will be used as a Path. Very usefull for debugging the script without having to selectr the folder each time with window dialog
+                self.path = sys.argv[1]
+        else:
+            self.path = filename
+        if not os.path.exists(self.path):
+            raise Exception("File \"{}\" is not found".format(self.path))
+        if os.path.exists(self.path + ".level.npy"):
+            self.level = np.load(self.path + ".level.npy")
+        self.curs = [0, 0, 0]
+        self.volume = None
+        self.ITA = pySPM.ITA(self.path)
+        for i, x in enumerate(self.ITA.get_masses()):
+            self.ui.peakList.setRowCount(i + 1)
+            self.ui.peakList.setItem(i, 0, QTableWidgetItem(x['assign']))
+            self.ui.peakList.setItem(i, 1, QTableWidgetItem("{:.2f}u".format((x['cmass']))))
+            self.ui.peakList.setItem(i, 2, QTableWidgetItem("{:.2f}u".format(x['umass'] - x['lmass'])))
+        self.ui.peakList.show()
+        self.ui.cmap.currentIndexChanged.connect(self.plot)
+        self.ui.prof1daxis.currentIndexChanged.connect(self.plot)
+        self.ui.peakList.cellClicked.connect(self.load_channel)
+        self.canvas.mpl_connect('button_press_event', self.on_pick)
+        self.flatAction = QAction("Flatten substrate from this channel")
+        self.flatAction.triggered.connect(self.flatten)
+        self.ui.correction.stateChanged.connect(self.plot)
+        self.ui.peakList.addAction(self.flatAction)
+        self.ui.status.setText("IDLE")
+
+    def flatline(self, y):
+        for x in range(self.volume.shape[1]):
+            popt, pcov = opt.curve_fit(CDF, np.arange(self.volume.shape[2]), self.volume[y, x, :],
+                                       (10, self.volume.shape[2] / 2, 1))
+            self.level[y, x] = popt[1]
+
+    def flatten(self):
+        self.ui.status.setText("Start the flattening...")
+        self.level = np.zeros(self.volume.shape[:2])
+        self.ui.pb.setMaximum(self.volume.shape[0])
+        for y in range(self.volume.shape[0]):
+            self.ui.pb.setValue(y)
+            self.flatline(y)
+            QCoreApplication.processEvents()
+            self.ax.clear()
+            self.ax.imshow(self.level)
+            self.canvas.draw()
+        self.ui.pb.setValue(0)
+        self.ui.status.setText("Flattening finished")
+        np.save(self.path + ".level", self.level)
+
+    def load_channel(self, row, col):
+        self.ui.status.setText("Loading channel...")
+        id = row
+        vol = []
+        for i in range(self.ITA.Nscan):
+            x = self.ITA.getImage(id, i)
+            vol.append(x)
+        self.volume = np.stack([x for x in vol], axis=2)
+        if not self.level is None:
+            self.corrected = np.zeros(self.volume.shape)
+            z = np.arange(self.ITA.Nscan)
+            self.ui.pb.setMaximum(self.level.shape[0])
+            for y in np.arange(self.level.shape[0]):
+                self.ui.pb.setValue(y)
+                for x in np.arange(self.level.shape[1]):
+                    dz = int(-self.level[y, x] + np.max(self.level))
+                    self.corrected[y, x, dz:] = self.volume[y, x, :self.volume.shape[2] - dz]
+            self.ui.pb.setValue(0)
+        self.plot()
+        self.ui.status.setText("IDLE")
+
+    def plot(self):
+        if self.ui.correction.isChecked():
+            A = self.corrected
+        else:
+            A = self.volume
+        cmap = self.ui.cmap.currentText()
+        self.axXY.clear()
+        self.axXZ.clear()
+        self.axYZ.clear()
+        self.ax.clear()
+        if self.volume is None:
+            return
+        self.axXY.imshow(A[:, :, self.curs[2]], cmap=cmap)
+        self.axXZ.imshow(A[self.curs[1], :, :].T, cmap=cmap)
+        self.axYZ.imshow(A[:, self.curs[0], :].T, cmap=cmap)
+        self.axXY.axhline(self.curs[1])
+        self.axXY.axvline(self.curs[0])
+        self.axXZ.axhline(self.curs[2])
+        self.axXZ.axvline(self.curs[0])
+        self.axYZ.axhline(self.curs[2])
+        self.axYZ.axvline(self.curs[1])
+        self.axXY.set_title("XY")
+        self.axXZ.set_title("XZ")
+        self.axYZ.set_title("YZ")
+        if self.ui.prof1daxis.currentText() in 'XYZ':
+            i = 'XYZ'.index(self.ui.prof1daxis.currentText())
+            self.ax.set_xlabel("XYZ"[i])
+            if i == 0:
+                self.ax.plot(A[:, self.curs[0], self.curs[2]])
+            elif i == 1:
+                self.ax.plot(A[self.curs[1], :, self.curs[2]])
+            elif i == 2:
+                self.ax.plot(A[self.curs[1], self.curs[0], :])
+        self.canvas.draw()
+
+    def on_pick(self, event):
+        if not event.inaxes in [self.axYZ, self.axXZ, self.axXY]:
+            return
+        x = event.xdata
+        y = event.ydata
+        axis = [self.axYZ, self.axXZ, self.axXY].index(event.inaxes)
+        xdata = int(x)
+        ydata = int(y)
+
+        if event.inaxes == self.axXY:
+            self.curs[0] = xdata
+            self.curs[1] = ydata
+        elif event.inaxes == self.axYZ:
+            self.curs[1] = xdata
+            self.curs[2] = ydata
+        elif event.inaxes == self.axXZ:
+            self.curs[0] = xdata
+            self.curs[2] = ydata
+        else:
+            print("Click event not handled")
+        self.curs = [np.clip(0, self.curs[i], self.volume.shape[i] - 1) for i in range(3)]
+        self.plot()
+
+    def initPlotLayout(self):
+        """
+        Setup the plotting layout.
+        """
+        self.axXY = self.fig.add_subplot(2, 2, 1)
+        self.axYZ = self.fig.add_subplot(2, 2, 2)
+        self.axXZ = self.fig.add_subplot(2, 2, 3)
+        self.ax = self.fig.add_subplot(2, 2, 4)
+        self.fig.tight_layout()
+
+
+app = QApplication(sys.argv)
+window = SlicerApp()
+window.show()
+sys.exit(app.exec_())
```

### Comparing `pySPM-0.2.9/pySPM/ITAX.py` & `pyspm-0.3.0/pySPM/ITAX.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,94 @@
-import zlib
-import struct
-import numpy as np
-from .Block import Block
-from . import utils
-
-class ITAX:
-    def __init__(self, filename):
-        self.f = open(filename, 'rb')
-        self.f.read(8)
-        self.root = Block(self.f)
-        mo = self.root.goto('CommonDataObjects/MeasurementOptions').getList()[0]
-        self.meas_options = self.root.goto('CommonDataObjects/MeasurementOptions/{name}[{id}]/pickle'.format(**mo)).unpickle()
-        self.size = {'pixels':dict(x=self.meas_options['raster_resolution'], y=self.meas_options['raster_resolution']), 'real':dict(x=self.meas_options['raster_fov'], y=self.meas_options['raster_fov'], unit='m')}
-
-    def getSnapshots(self):
-        """
-        Retrieve teh RGB images of the camera which are captured
-        Return a list of array for all the snapshots
-        """
-        snapshots = []
-        for x in self.root.goto('CommonDataObjects/Attachments'):
-            for y in x.getList():
-                if y['name'] == 'Video Snapshot':
-                    self.f.seek(y['bidx'])
-                    blk = Block(self.f)
-                    sx = blk.goto('res_x').getLong()
-                    sy = blk.goto('res_y').getLong()
-                    raw = blk.goto("imagedata").value
-                    data = zlib.decompress(raw)
-                    I = np.flipud(np.array(struct.unpack("<"+str(3*sx*sy)+"B", data)).reshape((sy, sx, 3)))
-                    snapshots.append(I)
-                    del blk
-        return snapshots
-    
-    def showSnapshots(self):
-        """
-        Retrieve and plot all recorded snapshots (camera images)
-        """
-        from .utils import sp
-        s = self.getSnapshots()
-        ax = sp(len(s))
-        for i, S in enumerate(s):
-            ax[i].imshow(S)
-            
-    def get_mass_cal(self):
-        k0 = self.root.goto("CommonDataObjects/DataViewCollection/*/properties/Context.MassScale.K0", lazy=True).getKeyValue()['float']
-        sf = self.root.goto("CommonDataObjects/DataViewCollection/*/properties/Context.MassScale.SF", lazy=True).getKeyValue()['float']
-        return sf, k0
-
-    def getSpectrum(self, sf=None, k0=None, time=False, **kargs):
-        """
-        Retrieve the spectrum in a similar way as for ITA file
-        """
-        slen = self.root.goto("CommonDataObjects/DataViewCollection/*/sizeSpectrum").getLong()
-        raw = self.root.goto("CommonDataObjects/DataViewCollection/*/dataSource/simsDataCache/spectrum/correctedData").value
-        spectrum = np.array(struct.unpack("<"+str(slen)+"d", raw))
-        CH = 2*np.arange(slen)        
-        if time:
-            return CH, spectrum
-        if sf is None:
-            sf = self.root.goto("CommonDataObjects/DataViewCollection/*/properties/Context.MassScale.SF", lazy=True).getKeyValue()['float']
-        if k0 is None:
-            k0 = self.root.goto("CommonDataObjects/DataViewCollection/*/properties/Context.MassScale.K0", lazy=True).getKeyValue()['float']
-        m = utils.time2mass(CH, sf, k0)
-        return m, spectrum
-    
-    def getProfile(self, name):
-        """
-        retrieve the depth profile for a given channel name
-        """
-        SN = None
-        for x in self.root.goto("CommonDataObjects/MeasurementOptions/*/massintervals"):
-            if x.name == 'mi':
-                v = x.dictList()
-                lab = v['assign']['utf16'] or v['desc']['utf16']
-                if lab == name:
-                    SN = v['SN']['utf16']
-                    break
-        if SN is None:
-            raise Exception("Profile \"{}\" not found".format(name))
-        path = "CommonDataObjects/DataViewCollection/*/dataSource/simsDataCache/{SN}/profile".format(SN=SN)
-        raw = self.root.goto(path, lazy=True).decompress()
-        return struct.unpack("<"+str(len(raw)//8)+"d", raw)
+import struct
+import zlib
+
+import numpy as np
+
+from . import utils
+from .Block import Block
+
+
+class ITAX:
+    def __init__(self, filename):
+        self.f = open(filename, 'rb')
+        self.f.read(8)
+        self.root = Block(self.f)
+        mo = self.root.goto('CommonDataObjects/MeasurementOptions').getList()[0]
+        self.meas_options = self.root.goto(
+            'CommonDataObjects/MeasurementOptions/{name}[{id}]/pickle'.format(**mo)).unpickle()
+        self.size = {'pixels': dict(x=self.meas_options['raster_resolution'], y=self.meas_options['raster_resolution']),
+                     'real': dict(x=self.meas_options['raster_fov'], y=self.meas_options['raster_fov'], unit='m')}
+
+    def getSnapshots(self):
+        """
+        Retrieve teh RGB images of the camera which are captured
+        Return a list of array for all the snapshots
+        """
+        snapshots = []
+        for x in self.root.goto('CommonDataObjects/Attachments'):
+            for y in x.getList():
+                if y['name'] == 'Video Snapshot':
+                    self.f.seek(y['bidx'])
+                    blk = Block(self.f)
+                    sx = blk.goto('res_x').getLong()
+                    sy = blk.goto('res_y').getLong()
+                    raw = blk.goto("imagedata").value
+                    data = zlib.decompress(raw)
+                    I = np.flipud(np.array(struct.unpack("<" + str(3 * sx * sy) + "B", data)).reshape((sy, sx, 3)))
+                    snapshots.append(I)
+                    del blk
+        return snapshots
+
+    def showSnapshots(self):
+        """
+        Retrieve and plot all recorded snapshots (camera images)
+        """
+        from .utils import sp
+        s = self.getSnapshots()
+        ax = sp(len(s))
+        for i, S in enumerate(s):
+            ax[i].imshow(S)
+
+    def get_mass_cal(self):
+        k0 = self.root.goto("CommonDataObjects/DataViewCollection/*/properties/Context.MassScale.K0",
+                            lazy=True).getKeyValue()['float']
+        sf = self.root.goto("CommonDataObjects/DataViewCollection/*/properties/Context.MassScale.SF",
+                            lazy=True).getKeyValue()['float']
+        return sf, k0
+
+    def getSpectrum(self, sf=None, k0=None, time=False, **kargs):
+        """
+        Retrieve the spectrum in a similar way as for ITA file
+        """
+        slen = self.root.goto("CommonDataObjects/DataViewCollection/*/sizeSpectrum").getLong()
+        raw = self.root.goto(
+            "CommonDataObjects/DataViewCollection/*/dataSource/simsDataCache/spectrum/correctedData").value
+        spectrum = np.array(struct.unpack("<" + str(slen) + "d", raw))
+        CH = 2 * np.arange(slen)
+        if time:
+            return CH, spectrum
+        if sf is None:
+            sf = self.root.goto("CommonDataObjects/DataViewCollection/*/properties/Context.MassScale.SF",
+                                lazy=True).getKeyValue()['float']
+        if k0 is None:
+            k0 = self.root.goto("CommonDataObjects/DataViewCollection/*/properties/Context.MassScale.K0",
+                                lazy=True).getKeyValue()['float']
+        m = utils.time2mass(CH, sf, k0)
+        return m, spectrum
+
+    def getProfile(self, name):
+        """
+        retrieve the depth profile for a given channel name
+        """
+        SN = None
+        for x in self.root.goto("CommonDataObjects/MeasurementOptions/*/massintervals"):
+            if x.name == 'mi':
+                v = x.dictList()
+                lab = v['assign']['utf16'] or v['desc']['utf16']
+                if lab == name:
+                    SN = v['SN']['utf16']
+                    break
+        if SN is None:
+            raise Exception("Profile \"{}\" not found".format(name))
+        path = "CommonDataObjects/DataViewCollection/*/dataSource/simsDataCache/{SN}/profile".format(SN=SN)
+        raw = self.root.goto(path, lazy=True).decompress()
+        return struct.unpack("<" + str(len(raw) // 8) + "d", raw)
```

### Comparing `pySPM-0.2.9/pySPM/ITM.py` & `pyspm-0.3.0/pySPM/ITM.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 # -- coding: utf-8 --
 
 # Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
 
-from . import Block
-import numpy as np
-import struct
+from __future__ import absolute_import
+
+import os
 import os.path
+import struct
 import zlib
-import re
+from warnings import warn
+
+import numpy as np
+
+from . import Block
+from .utils.misc import deprecated, aliased, alias, PB
+
 
 class InvalidRAWdataformat(Exception):
     def __init__(self, block, msg):
         self.block = block
         self.msg = msg
-        
+
     def __str__(self):
-        return "Invalid RAW dataformat seen in block "+self.block.parent+'/'+self.block.name+' : '+self.msg
+        return "Invalid RAW dataformat seen in block " + self.block.path + self.block.name + ' : ' + self.msg
+
 
+@aliased
 class ITM:
-    def __init__(self, filename, debug=False):
+    def __init__(self, filename, debug=False, readonly=True, precond=False, label=None):
         """
         Create the ITM object out of the filename.  Note that this works for
         all .ITA,.ITM, .ITS files as they have the same structure
         
         The ITM has the specialty to contain the "rawdata" block. Which
         contains a lot of sub-blocks all having a name which consists of spaces
         followed by numbers.
@@ -43,233 +52,268 @@
         coordinates of the pixel location (just replace the \xC0 byte by 0 and
         read it as a uint32) The second uint32 terminating by\cD0 tells the y
         coord.  of the pixel. The third terminating by \x40 tells the pixel
         number (increasing monotonically. I know iontof like to write 10 times
         the same information everywhere). The rest are the detected peaks
         measured in channel unit for that specific pixel. In order to get the
         mass see the channel2mass function
+        
+        Parameters
+        ----------
+        filename : string
+            Path of the ITA/ITM/ITS file
+        debug : bool
+            if True display some debug message.
+        readonly : bool
+            The pySPM library can now EDIT ITM/ITA files. In case you want to avoid that, please set readonly=True.
+            This might be also useful in case the file is open by another program which locks the file.
+        precond : bool
+            If True will run the preconditioner (adjust k0 so that H peak is correct and adjust scaling factor on the H peak)
         """
         self.filename = filename
+        if label is None:
+            self.label = os.path.basename(filename)
+        else:
+            self.label = label
         if not os.path.exists(filename):
             print("ERROR: File \"{}\" not found".format(filename))
             raise FileNotFoundError
-        self.f = open(self.filename, 'rb')
+        if readonly:
+            self.f = open(self.filename, 'rb')
+        else:
+            self.f = open(self.filename, 'r+b')
         self.Type = self.f.read(8)
         assert self.Type == b'ITStrF01'
         self.root = Block.Block(self.f)
         try:
-            d = self.root.goto('Meta/SI Image').dictList()
+            d = self.root.goto('Meta/SI Image').dict_list()
             self.size = {
                 'pixels': {
                     'x': d['res_x']['long'],
                     'y': d['res_y']['long']},
                 'real': {
                     'x': d['fieldofview']['float'],
-                    'y': d['fieldofview']['float']*d['res_y']['long']/d['res_x']['long'],
+                    'y': d['fieldofview']['float'] * d['res_y']['long'] / d['res_x']['long'],
                     'unit': 'm'}}
         except:
-            s = self.getValue('Registration.Raster.Resolution')['int']
-            fov = self.getValue("Registration.Raster.FieldOfView")['float']
-            self.size = {'pixels':dict(x=s,y=s),'real':dict(x=fov,y=fov,unit='m')}
+            s = self.get_value('Registration.Raster.Resolution')['int']
+            fov = self.get_value("Registration.Raster.FieldOfView")['float']
+            self.size = {'pixels': dict(x=s, y=s), 'real': dict(x=fov, y=fov, unit='m')}
         try:
             self.size['Scans'] = \
                 self.root.goto(
-                    'filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScans/Image.NumberOfScans').getULong()
+                    'filterdata/TofCorrection/ImageStack/Reduced Data/ImageStackScans/Image.NumberOfScans').get_ulong()
         except:
             pass
-        self.polarity = self.getValue("Instrument.Analyzer_Polarity_Switch")['string']
+        self.polarity = self.get_value("Instrument.Analyzer_Polarity_Switch")['string']
         self.peaks = {}
-        self.MeasData = {}
+        self.meas_data = {}
         self.rawlist = None
         try:
-            self.Nscan = self.root.goto('propend/Measurement.ScanNumber').getKeyValue()['int']
+            self.Nscan = self.root.goto("filterdata/TofCorrection/ImageStack/Reduced Data/NumberOfScans").getLong()
         except:
-            self.Nscan = None
-            
+            try:
+                self.Nscan = self.root.goto('propend/Measurement.ScanNumber').get_key_value()['int']
+            except:
+                self.Nscan = None
+        self.spp = self.root.goto("propend/Registration.Raster.ShotsPerPixel").get_key_value()['int']
         try:
-            R = [z for z in self.root.goto('MassIntervalList').getList() if z[
-                'name'] == 'mi']
+            R = [z for z in self.root.goto('MassIntervalList').get_list() if z['name'] == 'mi']
             N = len(R)
             for x in R:
                 try:
-                    X = self.root.goto('MassIntervalList/mi['+str(x['id'])+']')
-                    d = X.dictList()
+                    X = self.root.goto('MassIntervalList/mi[' + str(x['id']) + ']')
+                    d = X.dict_list()
                     self.peaks[d['id']['long']] = d
                 except ValueError:
                     pass
         except Exception as e:
             if debug:
                 raise e
-    
-    def getPeakList(self, name):
+        self.sf, self.k0 = self.get_mass_cal()
+        self.scale = 1
+        if precond:
+            self.precond()
+
+    @alias("getPeakList")
+    def get_peak_list(self, name):
         """
         Retrieve extra MassIntervalList (MIL) by it's name. Those are saved and visible in iontof software in the spectrum window.
         """
         PeakList = []
         for x in self.root.goto('filterdata/TofCorrection/Spectrum/Reduced Data/ExtraMILs'):
-            if x.goto('Name').getString() == name:
-                for y in [z for z in x.getList() if z['name'].decode() == 'mi']:
-                    d = x.goto('mi[{}]'.format(y['id'])).dictList()
-                    PeakList.append({key.decode('utf8'):d[key] for key in d})
+            if x.goto('Name').get_string() == name:
+                for y in [z for z in x.get_list() if z['name'].decode() == 'mi']:
+                    d = x.goto('mi[{}]'.format(y['id'])).dict_list()
+                    PeakList.append({key.decode('utf8'): d[key] for key in d})
                 return PeakList
         return None
-        
-    def showPeakList(self, name):
-        for m in self.getPeakList(name):
-            print("{id[long]}: ({desc[utf16]}) [{assign[utf16]}] {lmass[float]:.2f}u - {umass[float]:.2f}u (center: {cmass[float]:.2f}u)".format(**m))
-    
-    def getPropertyTrend(self, name):
+
+    @alias("showPeakList")
+    def show_peak_list(self, name):
+        for m in self.get_peak_list(name):
+            print(
+                "{id[long]}: ({desc[utf16]}) [{assign[utf16]}] {lmass[float]:.2f}u - {umass[float]:.2f}u (center: {cmass[float]:.2f}u)".format(
+                    **m))
+
+    @alias("getPropertyTrend")
+    def get_property_trend(self, name):
         """
         Sometimes values might be saved in ITA files under PropertyTrend.
         You can recover them here
         """
         for x in self.root.goto("PropertyTrends"):
-            if (x.name=='PropertyTrend' and x.goto("Trend.Name").getString() == name) or x.name == name:
-                N = x.goto('Trend.Data.NumberEntries').getLong()
+            if (x.name == 'PropertyTrend' and x.goto("Trend.Name").get_string() == name) or x.name == name:
+                N = x.goto('Trend.Data.NumberEntries').get_long()
                 data = x.goto("Trend.Data").value
-                dat = np.array([struct.unpack('<4d',data[32*i:32*(i+1)])[2:4] for i in range(N)])
+                dat = np.array([struct.unpack('<4d', data[32 * i:32 * (i + 1)])[2:4] for i in range(N)])
                 return dat
         return None
-        
+
     def get_summary(self, numeric=False):
         """
         Retrieve a summary of the important data concerning the measurement
         """
         from .utils import time2hms, funit
         def Get(k, default='Unknown', numeric=numeric):
             try:
                 v = self.getValue(k)
-                if len(v['string'].split())==1:
+                if len(v['string'].split()) == 1:
                     return v['string']
                 unit = v['string'].split()[-1]
                 if unit[0] in 'afpnumkMGE':
                     unit = unit[1:]
                 if not numeric:
-                    if unit == 's' and v['float']>60:
+                    if unit == 's' and v['float'] > 60:
                         return time2hms(v['float'])
                     r = funit(v['float'], unit)
-                    if int(r['value'])==r['value']:
+                    if int(r['value']) == r['value']:
                         return "{value:.0f} {unit}".format(**r)
                     return "{value:.2f} {unit}".format(**r)
-                
+
                 return v['string']
             except:
                 return default
-            
+
         return {
             'pixels': self.size['pixels'],
-            'fov': self.root.goto('Meta/SI Image[0]/fieldofview').getDouble(),
+            'fov': self.root.goto('Meta/SI Image[0]/fieldofview').get_double(),
+            'Floodgun': Get("Instrument.Timing.Floodgun"),
             'LMIG': {
                 'Extractor': Get("Instrument.LMIG.Extractor"),
                 'Lens_Source': Get("Instrument.LMIG.Lens_Source")},
             'ExtractionDelay': Get("Instrument.Analyzer.ExtractionDelay"),
-            'SputterSpecies': Get('Instrument.SputterGun.Species','Off'),
-            'SputterEnergy': Get('Instrument.SputterGun.Energy','Off'),
+            'SputterSpecies': Get('Instrument.SputterGun.Species', 'Off'),
+            'SputterEnergy': Get('Instrument.SputterGun.Energy', 'Off'),
             'AnalysisTime': Get("Analysis.AcquisitionTime"),
             'SputterTime': Get("Analysis.SputterTime"),
-            'Scans':  Get("Analysis.TotalScans",self.Nscan),
-            'TotalTime':  Get( "Analysis.TotalTime"),
+            'Scans': Get("Analysis.TotalScans", self.Nscan),
+            'TotalTime': Get("Analysis.TotalTime"),
             'peaks': self.get_masses(),
             'polarity': Get("Instrument.Analyzer_Polarity_Switch"),
-            'CycleTime': Get( "Measurement.CycleTime"),
-            'UpperMass': Get( "Measurement.UpperMass"),
-            'LMIGDropouts': Get( "Measurement.LMIGDropouts"),
-            'ShotsPerPixel' : Get( "Registration.Raster.ShotsPerPixel"),
+            'CycleTime': Get("Measurement.CycleTime"),
+            'UpperMass': Get("Measurement.UpperMass"),
+            'LMIGDropouts': Get("Measurement.LMIGDropouts"),
+            'ShotsPerPixel': Get("Registration.Raster.ShotsPerPixel"),
             'RasterMode': Get("Registration.Raster.Mode")
-            }
+        }
 
     def show_summary(self, fig=None, plot=True, **kargs):
         from . import funit
         s = self.get_summary(numeric=False)
         print("""
         Analysis time: {AnalysisTime}
         Delayed extraction: {ExtractionDelay}
+        Floodgun: {Floodgun}
         LMIG's Lens source: {LMIG[Lens_Source]}
         Sputter species: {SputterSpecies} @ {SputterEnergy}
         Field of View: {Fov[value]:.2f} {Fov[unit]}
         Pixel size: {pixels[x]} × {pixels[y]}
         Polarity: {polarity}
         Pixel Size: {pxs[value]:.2f} {pxs[unit]}
         Shots per pixel: {ShotsPerPixel}
         Raster mode: {RasterMode}
-        Cycle time: {CycleTime} (Upper mass: {UpperMass})""".format(Fov=funit(s['fov'],'m'), pxs=funit(s['fov']/s['pixels']['x'], 'm'), **s))
+        Number of scans: {Nscan}
+        Cycle time: {CycleTime} (Upper mass: {UpperMass})""".format(Nscan=self.Nscan, Fov=funit(s['fov'], 'm'),
+                                                                    pxs=funit(s['fov'] / s['pixels']['x'], 'm'), **s))
         print("Peaks:")
         for x in s['peaks']:
             if x['assign']:
                 print("\t▸ {assign} ({lmass:.3f} - {umass:.3f}u)".format(**x))
             elif x['desc']:
                 print("\t▸ {desc} ({lmass:.3f} - {umass:.3f}u)".format(**x))
             else:
                 print("\t▸ {cmass:.2f}u ({lmass:.3f} - {umass:.3f}u)".format(**x))
         if plot:
             import matplotlib.pyplot as plt
             import matplotlib as mpl
             if fig is None:
-                fig = plt.figure(figsize=kargs.get("figsize",(21,10)))
-            
-            SI = self.getIntensity()
-            Snapshot = self.getSnapshot()
-            EC = self.getPropertyTrend("Instrument.LMIG.Emission_Current")
-            Supp = self.getPropertyTrend("Instrument.LMIG.Suppressor")
-            Press = self.getPropertyTrend("Instrument.VCU.Pressure.Main")
-            N = (SI is not None)+(Snapshot is not None)+1+(EC is not None or Supp is not None or Press is not None)
+                fig = plt.figure(figsize=kargs.get("figsize", (21, 10)))
+
+            SI = self.get_intensity()
+            Snapshot = self.get_snapshot()
+            EC = self.get_property_trend("Instrument.LMIG.Emission_Current")
+            Supp = self.get_property_trend("Instrument.LMIG.Suppressor")
+            Press = self.get_property_trend("Instrument.VCU.Pressure.Main")
+            N = (SI is not None) + (Snapshot is not None) + 1 + (
+                    EC is not None or Supp is not None or Press is not None)
             gs = mpl.gridspec.GridSpec(2, N)
-            
+
             index = 0
             if SI is not None:
                 ax = plt.subplot(gs[0, index])
-                desc = self.root.goto('Meta/SI Image/description').getString()
-                SI.show(ax=ax, **{k:kargs[k] for k in kargs if k not in ['high', 'low']})
+                desc = self.root.goto('Meta/SI Image/description').get_string()
+                SI.show(ax=ax, **{k: kargs[k] for k in kargs if k not in ['high', 'low']})
                 index += 1
             if Snapshot is not None:
                 ax = plt.subplot(gs[0, index])
                 desc = self.root.goto('Meta/Video Snapshot/description').getString()
                 ax.imshow(Snapshot)
                 ax.set_title(desc)
                 index += 1
-            axStage = plt.subplot(gs[0, index+1])
-            axSpectra = plt.subplot(gs[1,:])
+            axStage = plt.subplot(gs[0, index + 1])
+            axSpectra = plt.subplot(gs[1, :])
             if EC is not None or Supp is not None or Press is not None:
                 ax = plt.subplot(gs[0, index])
                 from mpl_toolkits.axes_grid1 import make_axes_locatable
                 divider = make_axes_locatable(ax)
                 index2 = 0
-                from .utils import  s2hms
+                from .utils import s2hms
                 if Press is not None:
-                   t, tunit = s2hms(Press[:,0])
-                   ax.plot(t, Press[:,1]*1e6, 'C2')
-                   ax.set_xlabel("Time [{}]".format(tunit))
-                   ax.set_ylabel("Pressure ($\cdot 10^{-8}$) [mbar]")
-                   index2 += 1
-                   if index2%2 == 0:
-                    ax.yaxis.set_label_position("right")
+                    t, tunit = s2hms(Press[:, 0])
+                    ax.plot(t, Press[:, 1] * 1e6, 'C2')
+                    ax.set_xlabel("Time [{}]".format(tunit))
+                    ax.set_ylabel("Pressure ($\cdot 10^{-8}$) [mbar]")
+                    index2 += 1
+                    if index2 % 2 == 0:
+                        ax.yaxis.set_label_position("right")
                 if EC is not None:
-                   axc = divider.append_axes("bottom", size=1.2, sharex=ax)
-                   t, tunit = s2hms(EC[:,0])
-                   axc.plot(t, EC[:,1]*1e6, 'C0')
-                   axc.set_xlabel("Time [{}]".format(tunit))
-                   axc.set_ylabel("Emission Current [$\mu$A]")
-                   index2 += 1
-                   if index2%2 == 0:
-                    axc.yaxis.set_label_position("right")
+                    axc = divider.append_axes("bottom", size=1.2, sharex=ax)
+                    t, tunit = s2hms(EC[:, 0])
+                    axc.plot(t, EC[:, 1] * 1e6, 'C0')
+                    axc.set_xlabel("Time [{}]".format(tunit))
+                    axc.set_ylabel("Emission Current [$\mu$A]")
+                    index2 += 1
+                    if index2 % 2 == 0:
+                        axc.yaxis.set_label_position("right")
 
                 if Supp is not None:
-                   axb = divider.append_axes("bottom", size=1.2, sharex=ax)
-                   t, tunit = s2hms(Supp[:,0])
-                   axb.plot(t, Supp[:,1], 'C1')
-                   axb.set_xlabel("Time [{}]".format(tunit))
-                   axb.set_ylabel("LMIG Suppressor [V]")
-                   index2 += 1
-                   if index2%2 == 0:
-                    axb.yaxis.set_label_position("right")
+                    axb = divider.append_axes("bottom", size=1.2, sharex=ax)
+                    t, tunit = s2hms(Supp[:, 0])
+                    axb.plot(t, Supp[:, 1], 'C1')
+                    axb.set_xlabel("Time [{}]".format(tunit))
+                    axb.set_ylabel("LMIG Suppressor [V]")
+                    index2 += 1
+                    if index2 % 2 == 0:
+                        axb.yaxis.set_label_position("right")
                 index += 1
-            
-            self.showStage(ax=axStage, markers=True)
-            self.showSpectrum(low=kargs.get('low',0), high=kargs.get('high', None), ax=axSpectra)
-            
+
+            self.show_stage(ax=axStage, markers=True)
+            self.show_spectrum(low=kargs.get('low', 0), high=kargs.get('high', None), ax=axSpectra)
+
     def image(self, I, channel="Unknown", zscale="Counts"):
         """
         Create a pySPM.SPM.SPM_image for a given numpy array with the same real size information as the tof-sims data.
 
         Parameters
         ----------
         I : numpy 2D array
@@ -287,329 +331,612 @@
         Example
         -------
         >>> A = pySPM.ITA("myfile.ita")
         >>> Au,_ = A.getAddedImageByName("Au") # retrieve the gold channel (total counts)
         >>> Au_tofcorr = A.image(-np.log(1-np.fmin(.999, Au.pixels(A.Nscan))), "Au", zscale="yield") # Create a new image with the tof-corrected data
         """
         from .SPM import SPM_image
-        return SPM_image(I, real=self.size['real'], _type="TOF", zscale=zscale, channel=channel)     
-        
-    def getIntensity(self):
+        return SPM_image(I, real=self.size['real'], _type="TOF", zscale=zscale, channel=channel)
+
+    @alias("getIntensity")
+    def get_intensity(self):
         """
-        Retieve the total Ion image
+        Retrieve the total Ion image
         """
-        try:
-            X, Y = self.size['pixels']['x'], self.size['pixels']['y']
-            img = self.image(np.flipud(np.array(self.root.goto('Meta/SI Image/intensdata').getData("f")).reshape((Y, X))), channel="SI count")
-        except Exception as e:
-            try:
-                img = self.getAddedImage(0).pixels
-            except:
-                try:
-                    img = self.getAddedImageBySN(self.get_channel_SN("total"))
-                except:
-                    import warnings
-                    warn.warnings("SI image cannot be retrieved")
-                    return None
+        X, Y = self.size['pixels']['x'], self.size['pixels']['y']
+        img = self.image(np.flipud(
+            np.array(self.root.goto('Meta/SI Image/intensdata').get_data("f"), dtype=np.float32).reshape((Y, X))),
+            channel="SI count")
         return img
 
     def get_LMIG_info(self):
-        rs = self.getValues(start=True)
-        re = self.getValues()
+        rs = self.get_values(start=True)
+        re = self.get_values()
         Val = [["Parameter name", "Value at start", "Value at end"]]
         for i, x in enumerate(rs):
             Val.append([x, rs[x], re[x]])
 
-    def getValue(self, name, end=True):
-        return self.root.goto('prop{}/{name}'.format(['start','end'][end],name=name)).getKeyValue()
-    
-    def getValues(self, pb=False, start=False,end=True,names=[], startsWith="", nest=False, hidePrefix=True, numeric=False):
+    @alias("getValue")
+    def get_value(self, name, end=True):
+        return self.root.goto('prop{}/{name}'.format(['start', 'end'][end], name=name)).get_key_value()
+
+    @alias("getValues")
+    def get_values(self, prog=False, start=False, end=True, names=[], startsWith="", nest=False, hidePrefix=True,
+                   numeric=False):
         """
         Beta function: Retrieve a list of the values
         """
         Vals = {}
         startEnd = []
         if start:
             startEnd.append(True)
         if end:
             startEnd.append(False)
         for start in startEnd:
-            List = self.root.goto(['propend', 'propstart'][start]).getList()
-            if pb:
-                import tqdm
-                List = tqdm.tqdm(List)
+            List = self.root.goto(['propend', 'propstart'][start]).get_list()
+            if prog:
+                List = PB(List)
             for l in List:
                 Node = self.root.goto(['propend', 'propstart'][
-                                      start]).gotoItem(l['name'], l['id'])
-                r = Node.getKeyValue()
+                                          start]).goto_item(l['name'], l['id'])
+                r = Node.get_key_value()
                 del Node
                 S = Vals
                 if numeric:
                     value = r['float']
                 else:
                     value = r['string']
-                if r['key'] in names or ( names==[] and r['key'].startswith(startsWith) ):
+                if r['key'] in names or (names == [] and r['key'].startswith(startsWith)):
                     if hidePrefix:
                         key_name = r['key'][len(startsWith):]
                     else:
                         key_name = r['key']
                     if nest:
                         K = key_name.split('.')
                         for k in K:
                             if k not in S:
                                 S[k] = {}
                             S = S[k]
-                        S['value @'+['end', 'start'][start]] = value
+                        S['value @' + ['end', 'start'][start]] = value
                     else:
                         if key_name in Vals:
                             Vals[key_name].append(value)
                         else:
                             Vals[key_name] = [value]
-                            
         return Vals
 
-    def autoMassCal(self, t=None, S=None, pos=True, debug=False, Range=5000, FittingPeaks = ['C','CH','CH2','CH3','Na'], sf=None, k0=None):
-        """
-        perform an auto callibration for positive spectrum. (in test, might be unreliable)
-        """
-        from .utils import get_mass, time2mass, fitSpectrum, mass2time
-        from scipy.optimize import curve_fit
-        TimeWidth = 1e10*self.root.goto('propend/Instrument.LMIG.Chopper.Width').getKeyValue()['float']
+    @alias("autoMassCal")
+    def auto_mass_cal(self, t=None, S=None, pos=True, debug=False, error=False, Range=5000,
+                      fitting_peaks=['C', 'CH', 'CH2', 'CH3', 'Na'], apply=False, **kargs):
+        """
+        perform an auto calibration for spectrum. (in test, might be unreliable)
+        """
+        # old parameter name compatibility
+        if 'FittingPeaks' in kargs:
+            fitting_peaks = kargs['FittingPeaks']
+        if type(fitting_peaks) is str:
+            fitting_peaks = fitting_peaks.split(",")
+        negative = self.polarity == 'Negative'
+        fitting_peaks = [x + [['+', '-'][negative], '']['+' in x or '-' in x] for x in fitting_peaks]
+        from .utils import get_mass, time2mass, fit_spectrum, mass2time
+        time_width = 1e10 * self.root.goto('propend/Instrument.LMIG.Chopper.Width').get_key_value()['float']
         if t is None or S is None:
-            t, S = self.getSpectrum(time=True)
+            t, S = self.get_spectrum(time=True)
         N = np.prod(list(self.size['pixels'].values())) * self.Nscan
-        mask = S > N*0.01/TimeWidth
-        times_start = t[1:][np.nonzero(mask[1:]*(~mask[:-1]))]
-        times_end = t[np.nonzero(mask[:-1]*(~mask[1:]))]
-        times = (times_start + times_end)/2
+        mask = S > N * 0.01 / time_width
+        times_start = t[1:][np.nonzero(mask[1:] * (~mask[:-1]))]
+        times_end = t[np.nonzero(mask[:-1] * (~mask[1:]))]
+        times = (times_start + times_end) / 2
         tH = times[0]
-        mask = (t>=tH-TimeWidth)*(t<=tH+TimeWidth)
+        mask = (t >= tH - time_width) * (t <= tH + time_width)
         tH = t[mask][np.argmax(S[mask])]
+        if not 'sf' in kargs:
+            sf = self.sf
+        else:
+            sf = kargs.pop('sf')
+        if not 'k0' in kargs:
+            k0 = self.k0
+        else:
+            k0 = kargs.pop('k0')
+
         if sf is None or k0 is None:
-            sf=1e5
+            sf = 72000
             for i in range(3):
-                k0 = tH-sf*np.sqrt(get_mass('H+'))
+                k0 = tH - sf * np.sqrt(get_mass('H' + ['+', '-'][self.polarity == 'Negative']))
                 m = time2mass(t, sf=sf, k0=k0)
                 mP = time2mass(times, sf=sf, k0=k0)
-                t0 = times[np.argmin(np.abs(mP-12))]
-                t1 = times[np.argmin(np.abs(mP-12))+1]
-                sf = np.sqrt((t1-k0)**2 - (t0-k0)**2)
-                k0 = tH-sf*np.sqrt(get_mass('H+'))
+                t0 = times[np.argmin(np.abs(mP - 12))]
+                t1 = times[np.argmin(np.abs(mP - 12)) + 1]
+                sf = np.sqrt((t1 - k0) ** 2 - (t0 - k0) ** 2)
+                k0 = tH - sf * np.sqrt(get_mass('H'))
         ts = []
-        for x in [mass2time(get_mass(x+'+'), sf=sf, k0=k0) for x in FittingPeaks]:
-            mask = (t>=(x-Range))*(t<=(x+Range))
+        for x in [mass2time(get_mass(x), sf=sf, k0=k0) for x in fitting_peaks]:
+            mask = (t >= (x - Range)) * (t <= (x + Range))
             t_peak = t[mask][np.argmax(S[mask])]
             ts.append(t_peak)
-        ms = [get_mass(x+'+') for x in FittingPeaks]
+        ms = [get_mass(x) for x in fitting_peaks]
+        sf, k0, dsf, dk0 = fit_spectrum(ts, ms, error=True)
+        if apply:
+            self.set_sf(sf)
+            self.set_k0(k0)
+        self.sf = sf
+        self.k0 = k0
         if debug:
-            return fitSpectrum(ts, ms, error=True), ts, ms
-        return fitSpectrum(ts, ms)
-    
-    def showValues(self, pb=False, gui=False, **kargs):
+            return sf, k0, dsf, dk0, ts, ms
+        if error:
+            return sf, k0, dsf, dk0
+        return sf, k0
+
+    @alias("showValues")
+    def show_values(self, pb=False, gui=False, **kargs):
         from .utils import html_table, aa_table
         html = True
         if 'html' in kargs:
             html = kargs['html']
             del kargs['html']
         if gui:
-            from pySPM import GUI
-            Vals = self.getValues(pb, nest=True, **kargs)
-            GUI.ShowValues(Vals)
+            from pySPM.tools import values_display
+            Vals = self.get_values(pb, nest=True, **kargs)
+            values_display.show_values(Vals)
         else:
-            Vals = self.getValues(pb, **kargs)
+            Vals = self.get_values(pb, **kargs)
             Table = [["Parameter Name", "Value @start", "Value @end"]]
             for x in Vals:
-                Table.append(tuple([x]+Vals[x]))
+                Table.append(tuple([x] + Vals[x]))
             if not html:
                 print(aa_table(Table, header=True))
             else:
                 from IPython.core.display import display, HTML
                 res = html_table(Table, header=True)
                 display(HTML(res))
-                
+
+    def reset_mass_cal(self, alt=False):
+        self.sf, self.k0 = self.get_mass_cal(alt=alt)
+
     def get_mass_cal(self, alt=False):
         try:
-            assert not alt
-            V = self.root.goto('filterdata/TofCorrection/Spectrum/Reduced Data/IMassScaleSFK0')
-            sf = V.goto('sf',lazy=True).getDouble()
-            k0 = V.goto('k0',lazy=True).getDouble()
+            if not alt:
+                V = self.root.goto('filterdata/TofCorrection/Spectrum/Reduced Data/IMassScaleSFK0')
+                sf = V.goto('sf', lazy=True).get_double()
+                k0 = V.goto('k0', lazy=True).get_double()
+            else:
+                sf = self.root.goto('MassScale/sf').get_double()
+                k0 = self.root.goto('MassScale/k0').get_double()
         except:
             import warnings
             warnings.warn("Failed to get sf,k0, find alternative")
-            sf = self.root.goto('MassScale/sf').getDouble()
-            k0 = self.root.goto('MassScale/k0').getDouble()
-            
+            if not alt:
+                sf = self.root.goto('MassScale/sf').get_double()
+                k0 = self.root.goto('MassScale/k0').get_double()
+            else:
+                V = self.root.goto('filterdata/TofCorrection/Spectrum/Reduced Data/IMassScaleSFK0')
+                sf = V.goto('sf', lazy=True).get_double()
+                k0 = V.goto('k0', lazy=True).get_double()
         return sf, k0
 
     def channel2mass(self, channels, sf=None, k0=None, binning=1):
         """
         Calculate the mass from the time of flight
         The parameters sf and k0 will be read from the file (calibration used by iontof) in case they are None
         The binning just multiply the channels in order to get the correct answer (used for the ITA files for the moment)
         default values for uncalibrated spectrum are sf = 100'000 &  k0 = 0
         The time can be retrieved by knowing the channel width (typically 100ps). So time = channel * channelWidth
         The mass = (2*q*U/L**2)*(channel*channelWidth)**2
         L is the path length, thus twice the columns length and is about 2m I think
         For an extractor of 2keV and L=2m, 1u = (time[s]*310620.843175[u**.5/s])**2 = [channel/sf]**2 => sf is about 32000 for k0 = 0
         Caution. If data are binned, the channel number should be multiplied by the binning factor in order to use the same sf and k0 factor!
         
-        For information the channel width is 50ps and is strangely not saved in the file.
+        For information the channel width is 50ps and can be retrieved by pySPM.ITM.get_value("Registration.TimeResolution")
         """
         if sf is None or k0 is None:
-            sf0, k00 = self.get_mass_cal()
+            sf0, k00 = self.sf, self.k0
         if sf is None:
             sf = sf0
         if k0 is None:
             k0 = k00
-        return ((binning*channels-k0)/(sf))**2
+        return ((binning * channels - k0) / (sf)) ** 2
+
+    def shift_sf(self, dsf):
+        """
+        This function adjust the value of sf by adding the value given as parameter and recalculate k0 such that the H peak does not move.
+        """
+        from .utils import get_mass
+        self.k0 = self.k0 - dsf * np.sqrt(get_mass("H+"))
+        self.sf += dsf
+
+    def rescale(self, elt, amp=10000, delta=.02):
+        from .utils.fit import peak_fit
+        m, s = self.get_spectrum(scale=1)
+        p0 = peak_fit(m, s, elt, delta=delta)
+        self.scale = amp / p0[2]
+        return p0
+
+    def adjust_sf(self, elt, delta=0.02):
+        from .utils import get_mass
+        from .utils.fit import peak_fit
+        m, s = self.get_spectrum()
+        mH = get_mass("H" + "+-"[self.polarity == 'Negative'])
+        p0 = peak_fit(m, s, mH, delta=.02)
+        tH = 2 * np.argmin(abs(m - p0[0]))
+
+        mX = get_mass(elt)
+        p0 = peak_fit(m, s, mX, delta=delta)
+        tX = 2 * np.argmin(abs(m - p0[0]))
+        self.sf = (tX - tH) / (np.sqrt(mX) - np.sqrt(mH))
+        self.k0 = tH - self.sf * np.sqrt(mH)
+
+    def precond(self, amp=10000, do_mass_cal=False):
+        """
+        This is a pre-conditioner function which adjust k0 so that the H peak is exactly centered on the correct mass and it adjusts the scale factor so that the H peak is exactly equivalent to amp (10'000 by default).
+        
+        This function is useful in case people want to compare several measurements together.
+        
+        Parameters
+        ----------
+        amp : float, int
+            The amplitude of the H peak after scaling
+        apply : bool
+            Appy the changes of k0 and sf to the file
+        """
+        from .utils import get_mass
+        from .utils.fit import peak_fit
+
+        m, s = self.getSpectrum()
+        mask = (m > .5) * (m < 1.5)
+        amp0 = np.max(s[mask])
+        mH = get_mass("H" + "+-"[self.polarity == 'Negative'])
+        if do_mass_cal or amp0 < max(100, .05 * self.Nscan * self.size['pixels']['x'] * self.size['pixels']['y']):
+            warn("the initial mass calibration seems to be wrong, let's try to perform it from scratch")
+            self.sf, self.k0 = self.auto_mass_cal(sf=72000, k0=0)
+            m, s = self.getSpectrum()
+            mask = (m > .98) * (m < 1.02)
+            amp0 = np.max(s[mask])
+        try:
+            p0 = peak_fit(m, s, mH)
+        except:
+            if not do_mass_cal:
+                return self.precond(amp=amp, do_mass_cal=True)
+        tH = 2 * np.argmin(abs(m - p0[0]))
+        self.k0 = tH - self.sf * np.sqrt(mH)
+        if amp is not None:
+            self.scale = amp / p0[2]
 
-    def getSpectrum(self, sf=None, k0=None, time=False, error=False, **kargs):
+    @alias("getSpectrum")
+    def get_spectrum(self, sf=None, k0=None, scale=None, time=False, error=False, **kargs):
         """
         Retieve a mass,spectrum array
         This only works for .ita and .its files.
         For this reason it is implemented in the itm class.
         """
         RAW = zlib.decompress(self.root.goto(
-            'filterdata/TofCorrection/Spectrum/Reduced Data/IITFSpecArray/'+['CorrectedData','Data'][kargs.get('uncorrected',False)]).value)
-        D = np.array(struct.unpack("<{0}f".format(len(RAW)//4), RAW))
-        ch = 2*np.arange(len(D))
+            'filterdata/TofCorrection/Spectrum/Reduced Data/IITFSpecArray/' + ['CorrectedData', 'Data'][
+                kargs.get('uncorrected', False)]).value)
+        if scale is None:
+            scale = self.scale
+        D = scale * np.array(struct.unpack("<{0}f".format(len(RAW) // 4), RAW))
+        ch = 2 * np.arange(len(D))  # We multiply by two because the channels are binned.
         if time:
             return ch, D
         m = self.channel2mass(ch, sf=sf, k0=k0)
         if error:
-            Dm = 2*np.sqrt(m)*np.sqrt(Dk0**2+m*Dsf**2)/sf
+            # TODO: parameters Dk0 and Dsf are undefined
+            Dm = 2 * np.sqrt(m) * np.sqrt(Dk0 ** 2 + m * Dsf ** 2) / sf
             return m, D, Dm
         return m, D
-    
-    def getMeasData(self, name='Instrument.LMIG.Emission_Current', prog=False, debug=False):
+
+    @alias("getMeasData")
+    def get_meas_data(self, name='Instrument.LMIG.Emission_Current', prog=False, debug=False):
         """
         Allows to recover the data saved during the measurements.
         This function is like getValues, but instead of giving the values at the beginning and at the end, 
         it track the changes of them during the measurement.
         """
-        if name in self.MeasData:
-            return self.MeasData[name]
+        if name in self.meas_data:
+            return self.meas_data[name]
         self.rawdata = self.root.goto('rawdata')
-        L = self.rawdata.getList()
+        L = self.rawdata.get_list()
         i = 1
-        while L[-i]['name'] !=  '  20':
+        while L[-i]['name'] != '  20':
             i += 1
         max_index = L[-i]['id']
         if prog:
-            try:
-                from tqdm import tqdm_notebook as tqdm
-            except:
-                from tqdm import tqdm as tqdm
-            if prog is True:
-                T = tqdm(L)
-            else:
-                T = prog(L)
+            T = PB(L)
         else:
-            T=L
-        for i,elt in enumerate(T):
+            T = L
+        for i, elt in enumerate(T):
             if elt['name'] != '  20':
                 continue
             idx = elt['bidx']
             self.f.seek(idx)
             child = Block.Block(self.f)
-            r = child.getKeyValue(0)
-            if not r['key'] in self.MeasData:
-                self.MeasData[r['key']] = []
-            self.MeasData[r['key']].append((idx,r['float']))
-        if name in self.MeasData:
-            return self.MeasData[name]
+            r = child.get_key_value(0)
+            if not r['key'] in self.meas_data:
+                self.meas_data[r['key']] = []
+            self.meas_data[r['key']].append((idx, r['float']))
+        if name in self.meas_data:
+            return self.meas_data[name]
         else:
             raise KeyError(name)
-    
+
     def show_stability(self, ax=None, prog=False):
-        from .utils.plot import DualPlot
+        from .utils.plot import dual_plot
         if ax is None:
             import matplotlib.pyplot as plt
             ax = plt.gca()
-        self.showMeasData(ax=ax, scans=3, mul=1e6, prog=prog);
-        axb = DualPlot(ax)
-        self.showMeasData("Instrument.LMIG.Suppressor", ax=axb, color='orange', scans=False, prog=prog);
-        
-    def showMeasData(self, name='Instrument.LMIG.Emission_Current', prog=False, ax=None, mul=1, scans=2, **kargs):
-        t = self.getMeasData('Measurement.AcquisitionTime')
-        S = self.getMeasData("Measurement.ScanNumber")
+        self.show_meas_data(ax=ax, scans=3, mul=1e6, prog=prog);
+        axb = dual_plot(ax)
+        self.show_meas_data("Instrument.LMIG.Suppressor", ax=axb, color='orange', scans=False, prog=prog);
+
+    def show_meas_data(self, name='Instrument.LMIG.Emission_Current', prog=False, ax=None, mul=1, scans=2, **kargs):
+        t = self.get_meas_data('Measurement.AcquisitionTime')
+        S = self.get_meas_data("Measurement.ScanNumber")
         idx = [x[0] for x in t]
         time = [x[1] for x in t]
         ScanData = [x[1] for x in S]
         ScanIdx = [x[0] for x in S]
-        s = np.interp(ScanIdx,idx,time)
-        
-        Meas = self.getMeasData(name,prog=prog)
-        
+        s = np.interp(ScanIdx, idx, time)
+
+        Meas = self.get_meas_data(name, prog=prog)
+
         MeasData = [x[1] for x in Meas]
         MeasIdx = [x[0] for x in Meas]
-        t = np.interp(MeasIdx,idx, time)
+        t = np.interp(MeasIdx, idx, time)
         if ax is None:
             import matplotlib.pyplot as plt
             ax = plt.gca()
-        p = ax.plot(t, np.array(MeasData)*mul, **kargs)
+        p = ax.plot(t, np.array(MeasData) * mul, **kargs)
         ax.set_xlabel("Time [s]");
         ax.set_ylabel(name)
         if scans:
             assert type(scans) is int
             lim = ax.get_ylim()
             axs = ax.twiny()
-            axs.set_xticks(.5*s[:-1:scans]+.5*s[1::scans])
-            axs.set_xticklabels([str(i+1) for i in range(0,self.Nscan,scans)])
-            colors = [i%2 for i in range(0,self.Nscan,scans)]
-            for i,tick in enumerate(axs.xaxis.get_ticklabels()):
-                tick.set_color(["black","green"][colors[i]])
+            axs.set_xticks(.5 * s[:-1:scans] + .5 * s[1::scans])
+            axs.set_xticklabels([str(i + 1) for i in range(0, self.Nscan, scans)])
+            colors = [i % 2 for i in range(0, self.Nscan, scans)]
+            for i, tick in enumerate(axs.xaxis.get_ticklabels()):
+                tick.set_color(["black", "green"][colors[i]])
             axs.set_xlim(ax.get_xlim())
-            for i in range(1,self.Nscan-1,2):
-                ax.fill_between([s[i],s[i+1]],*lim,color='green',alpha=.1)
+            for i in range(1, self.Nscan - 1, 2):
+                ax.fill_between([s[i], s[i + 1]], *lim, color='green', alpha=.1)
             axs.set_xlabel("Scan number")
             axs.set_xlim(ax.get_xlim())
             axs.set_ylim(*lim)
         return p
 
-    def showSpectrum(self, low=0, high=None, sf=None, k0=None, ax=None, log=False, showPeaks=True, **kargs):
+    @alias("showSpectrumAround")
+    def show_spectrum_around(self, m0, delta=None, amp_scale=1, sf=None, k0=None, **kargs):
+        """
+        Display the Spectrum around a given mass.
+
+        Parameters
+        ----------
+        m0 : float
+            The central mass around which the spectrum will be plotted (in u)
+        delta : float
+            The spectrum will be plotted between m0-delta and m0+delta
+        sf : float or None
+        k0 : float or None
+            sf and k0 are the mass calibration parameters. If None values saved with the file will be used.
+        **kargs : supplementary arguments
+            Passed to pySPM.utils.showPeak
+        """
+        polarity = '+'
+        if self.get_value('Instrument.Analyzer_Polarity_Switch')['string'] == 'Negative':
+            polarity = '-'
+        from . import utils
+        m, D = self.get_spectrum(sf=sf, k0=k0)
+        if 'label' not in kargs:
+            kargs['label'] = self.label
+        return utils.show_peak(m, D * amp_scale, m0, delta, polarity=polarity, sf=sf, k0=k0, **kargs)
+
+    @deprecated("SpectraPerPixel")
+    def spectra_per_pixel(self, pixel_aggregation=None, peak_lim=0, scans=None, prog=False, safe=True, FOVcorr=True,
+                          smooth=False):
+        """
+        This function return a 2D array representing the spectra per pixel. The first axis correspond to each aggregated pixel and the second axis the spectral time.
+        In order to keep the 2D array small enough the spectra are filtered in order to keep only strictly positive values (or larger than peak_lim).
+        
+        Parameters
+        ----------
+        pixel_aggregation: int
+            the number of pixels aggregation. pixel_aggregation 
+        
+        """
+        if pixel_aggregation is None:
+            pixel_aggregation = max(1, int(self.size['pixels']['x'] // 64))
+
+        from .utils import get_mass, constants as const, closest_arg
+        gun = self.root.goto('propend/Instrument.PrimaryGun.Species').get_key_value()[
+            'string']  # Primary Gun Species (Bi1,Bi3,Bi3++)
+
+        # if the + is missing in the name, add it
+        if gun[-1] != '+':
+            gun += '+'
+
+        Q = gun.count('+')  # number of charge
+
+        nrj = self.root.goto('propend/Instrument.PrimaryGun.Energy').get_key_value()[
+            'float']  # Primary ion energy (in eV)
+        dx = self.size['real']['x'] / self.size['pixels']['x']  # distance per pixel
+
+        # Calculate the mass of the primary ion
+        mp = get_mass(gun)
+
+        if FOVcorr:
+            DT = dx * (1 / 5e-11) * .5 * np.sqrt(2) * np.sqrt((1e-3 * mp / const.NA) / (
+                    Q * 2 * nrj * const.qe))  # delta time in channel per pixel. The 5e-11 is the channelwidth (50ps)
+            # sqrt(2)/2 is from the sin(45°), nrj=E=.5*mp*v^2
+        else:
+            DT = 0
+
+        if peak_lim is None:
+            peak_lim = 0
+
+        if prog:
+            pb = PB(total=3, postfix={'task': "Calculating total spectrum"})
+            IT = lambda x: PB(x, leave=False)
+        else:
+            IT = lambda x: x
+
+        pixel_size = ((self.size['pixels']['x'] + pixel_aggregation - 1) // pixel_aggregation) * (
+                (self.size['pixels']['y'] + pixel_aggregation - 1) // pixel_aggregation)
+        channels = round(
+            self.get_value("Measurement.CycleTime")['float'] / self.get_value("Registration.TimeResolution")['float'])
+
+        # calculate total spectra
+        m = np.zeros(channels)
+
+        if scans is None:
+            scans = range(self.Nscan)
+        dts = DT * (self.size['pixels']['x'] / 2 - np.arange(
+            self.size['pixels']['x']))  # time correction for the given x coordinate (in channel number)
+        for scan in IT(scans):
+            raw = self.get_raw_raw_data(scan)
+            rawv = struct.unpack('<{}I'.format(len(raw) // 4), raw)
+            i = 0
+            while i < len(rawv):
+                b = rawv[i]
+                if b & 0xc0000000:
+                    x = b & 0x0fffffff
+                    dt = dts[x]
+                    # fp = dt%1
+                    ip = int(dt)
+                    i += 3
+                else:
+                    m[b - ip] += 1  # (1-fp)
+                    # m[b-ip-1] += fp
+                    i += 1
+
+        # calculate the extreme cases
+        max_time = np.nonzero(m)[0][-1]
+        max_count = np.max(m)
+
+        if prog:
+            pb.update(1)
+            pb.set_postfix({'task': "calculating aggregated spectrum"})
+
+        # Select the peaks which are higher that peak_lim counts
+        t = np.arange(channels)
+        tx = t[m > peak_lim]  # reduced time vector
+        mx = m[m > peak_lim]  # reduced mass vector
+        rev = {x: -1 for x in range(max_time + 1)}
+        for k in range(len(tx)):
+            rev[tx[k]] = k
+
+        if safe:
+            import psutil
+            free_ram = psutil.virtual_memory().free
+            if pixel_size * tx.size * 4 >= free_ram:
+                raise Exception("""You don't have sufficient free RAM to perform this operation.
+                Free RAM: {ram:.1f}Mb
+                Number of pixels: {Npix}
+                Spectrum size [value>{peak_lim}] : {tx} elements
+                Array size: {N} elements = {ss}Mb
+                It is advised that you clean up memory or use a higher pixel_aggregation value.
+                You can force the execution of this command by using the argument safe=False.
+                """.format(ram=free_ram / 1024 ** 2, peak_lim=peak_lim, Npix=pixel_size, tx=tx.size,
+                           N=pixel_size * tx.size, ss=pixel_size * tx.size * 4 / 1024 ** 2))
+
+        size = (pixel_size, tx.size)
+        spec = np.zeros(size, dtype='float32')
+        for scan in IT(scans):
+            raw = self.get_raw_raw_data(scan)
+            rawv = struct.unpack('<{}I'.format(len(raw) // 4), raw)
+            k = 0
+            while k < len(rawv):
+                b = rawv[k]
+                if b & 0xc0000000:
+                    x = b & 0x0fffffff
+                    y = rawv[k + 1] & 0x0fffffff
+                    dt = dts[x]
+                    # fp = dt%1
+                    ip = int(dt)
+                    k += 3
+                    i = (self.size['pixels']['x'] // pixel_aggregation) * (
+                            y // pixel_aggregation) + x // pixel_aggregation
+                else:
+                    j1 = rev[b - ip]
+                    if j1 < 0:
+                        j1 = closest_arg(tx, b - ip)
+                    # j2 = closest_arg(tx, b-ip-1)
+                    spec[i][j1] += 1
+                    # if j2>0:
+                    #    spec[i][j2] += fp
+                    k += 1
+        if prog:
+            pb.update(1)
+            pb.set_postfix({'task': 'smooth spectra'})
+
+        if smooth:
+            if smooth is True:
+                smooth = (51, 3)
+            from scipy.signal import savgol_filter
+            for i in IT(range(pixel_size)):
+                s = np.zeros(channels)
+                s[m > peak_lim] = spec[i]
+                s = savgol_filter(s, *smooth)
+                spec[i] = s[m > peak_lim]
+
+        if prog:
+            pb.update(1)
+            pb.set_postfix({'task': 'done'})
+
+        return m > peak_lim, spec
+
+    @alias("showSpectrum")
+    def show_spectrum(self, low=0, high=None, sf=None, k0=None, ax=None, log=False, show_peaks=False, **kargs):
         """
         Plot the (summed) spectrum
         low and high: mass boundary of the plotted data
         ax: matplotlib axis
         log: plot the log of the intensity if True
         """
-        m, s = self.getSpectrum(sf=sf,k0=k0,**kargs)
+        # old notation compatibility
+        if 'showPeaks' in kargs:
+            warn("The parameter showPeaks is deprecated. Please use show_peaks")
+            show_peaks = kargs.pop("showPeaks")
+
+        m, s = self.get_spectrum(sf=sf, k0=k0, **kargs)
         if ax is None:
             import matplotlib.pyplot as plt
             ax = plt.gca()
         if high is None:
             high = m[-1]
         mask = np.logical_and(m >= low, m <= high)
         M = m[mask]
         S = s[mask]
         if log:
-            S = np.log(S)
-        ax.plot(M, S)
+            ax.log = True
+            S[S >= 1] = np.log10(S[S >= 1])
+            S[S < 1] = 0
+        if 'label' not in kargs:
+            kargs['label'] = self.label
+        ax.plot(M, S, **kargs)
         self.get_masses()
-        if showPeaks:
+        if show_peaks:
             ymax = ax.get_ylim()[1]
             labels = []
             pos = []
             index = 0
-            for P in [x for x in self.peaks if self.peaks[x]['desc']['utf16'] not in ['total','sum of rest']]:
+            for P in [x for x in self.peaks if self.peaks[x]['desc']['utf16'] not in ['total', 'sum of rest']]:
                 p = self.peaks[P]
                 c = p['cmass']['float']
-                mask = (m >= p['lmass']['float'])*(m <= p['umass']['float'])
+                mask = (m >= p['lmass']['float']) * (m <= p['umass']['float'])
                 if c >= low and c <= high:
-                    i = np.argmin(abs(m-c))
+                    i = np.argmin(abs(m - c))
                     pos.append(m[i])
-                    #ax.fill_between(m[mask], 0, ymax, color=['red','green','blue'][index%3], alpha=.2)
+                    # ax.fill_between(m[mask], 0, ymax, color=['red','green','blue'][index%3], alpha=.2)
                     index += 1
                     labels.append(p['assign']['utf16'])
             from .utils import put_Xlabels
             put_Xlabels(ax, pos, labels);
             ax.set_xlabel("Mass [u]")
             ax.set_ylabel("Total counts [-]");
-            
+
     def get_masses(self, mass_list=None):
         """
         retrieve the peak list as a dictionnary
         """
         if mass_list is None:
             masses = self.peaks
         else:
@@ -622,18 +949,20 @@
                 p = P
             result.append({
                 'id': p['id']['long'],
                 'desc': p['desc']['utf16'],
                 'assign': p['assign']['utf16'],
                 'lmass': p['lmass']['float'],
                 'cmass': p['cmass']['float'],
-                'umass': p['umass']['float']})
+                'umass': p['umass']['float'],
+                'SN': p['SN']['utf16']})
         return result
 
-    def getRawSpectrum(self, scans=None, ROI=None, FOVcorr=True, deadTimeCorr=True, **kargs):
+    @alias("getRawSpectrum")
+    def get_raw_spectrum(self, scans=None, ROI=None, FOVcorr=True, deadTimeCorr=True, **kargs):
         """
         Reconstruct the spectrum from RAW data.
         scans: List of scans to use. if None all scans are used (default)
         ROI: Region Of Interest. It can be:
             1) None: All pixels are used
             2) A list of images. The pixels will be added to the spectrum i if the value of the i-th image is True for that pixel
             3) An image with integer value. The current pixels will be added to the i-th spectrum if the value of ROI at that pixel is i.
@@ -652,262 +981,303 @@
         
         see Ref. T. Stephan, J. Zehnpfenning and A. Benninghoven, J. vac. Sci. A 12 (2), 1994
  
         """
         from .utils import get_mass, constants as const
         if ROI is None and 'roi' in kargs:
             ROI = kargs['roi']
-            
-        gun = self.root.goto('propend/Instrument.PrimaryGun.Species').getKeyValue()['string'] # Primary Gun Species (Bi1,Bi3,Bi3++)
-        
+
+        gun = self.root.goto('propend/Instrument.PrimaryGun.Species').get_key_value()[
+            'string']  # Primary Gun Species (Bi1,Bi3,Bi3++)
+
         # if the + is missing in the name, add it
-        if gun[-1]!='+':
+        if gun[-1] != '+':
             gun += '+'
-            
-        Q = gun.count('+') # number of charge
-        
-        nrj = self.root.goto('propend/Instrument.PrimaryGun.Energy').getKeyValue()['float'] # Primary ion energy (in eV)
-        dx = self.size['real']['x']/self.size['pixels']['x'] # distance per pixel
-        
+
+        Q = gun.count('+')  # number of charge
+
+        nrj = self.root.goto('propend/Instrument.PrimaryGun.Energy').get_key_value()[
+            'float']  # Primary ion energy (in eV)
+        dx = self.size['real']['x'] / self.size['pixels']['x']  # distance per pixel
+
         # Calculate the mass of the primary ion
         mp = get_mass(gun)
-            
+
         # Perform the time of flight correction?
         if FOVcorr:
-            DT = dx*(1/5e-11)*.5*np.sqrt(2)*np.sqrt((1e-3*mp/const.NA)/(Q*2*nrj*const.qe)) # delta time in channel per pixel. The 5e-11 is the channelwidth (50ps)
+            DT = dx * (1 / 5e-11) * .5 * np.sqrt(2) * np.sqrt((1e-3 * mp / const.NA) / (
+                    Q * 2 * nrj * const.qe))  # delta time in channel per pixel. The 5e-11 is the channelwidth (50ps)
             # sqrt(2)/2 is from the sin(45°), nrj=E=.5*mp*v^2
         else:
             DT = 0
-            
+
         if scans is None:
             scans = range(self.Nscan)
-            
+
         assert hasattr(scans, '__iter__')
-        
+
         # Allocate vector for the spectrum
-        number_channels = int(round(self.root.goto('propend/Measurement.CycleTime').getKeyValue()['float']\
-            / self.root.goto('propend/Registration.TimeResolution').getKeyValue()['float']))
-        
-        if kargs.get('prog',False):
-            try:
-                from tqdm import tqdm_notebook as tqdm
-            except:
-                from tqdm import tqdm as tqdm
-            T = tqdm(scans)
+        number_channels = int(round(self.root.goto('propend/Measurement.CycleTime').get_key_value()['float'] \
+                                    / self.root.goto('propend/Registration.TimeResolution').get_key_value()['float']))
+
+        if kargs.get('prog', False):
+            T = PB(scans)
         else:
             T = scans
-            
+        if kargs.get('debug', False):
+            import time
+            t0 = time.time()
+        dts = DT * (self.size['pixels']['x'] / 2 - np.arange(
+            self.size['pixels']['x']))  # time correction for the given x coordinate (in channel number)
         if ROI is None:
             Spectrum = np.zeros(number_channels, dtype=np.float32)
             for s in T:
-                Data = self.getRawData(s)[2]
-                if kargs.get('prog', False):
-                    LData = tqdm(Data, leave=False)
-                else:
-                    LData = Data
-                for xy in LData:
-                    dt = DT*(self.size['pixels']['x']/2-xy[0]) # time correction for the given x coordinate (in channel number)
-                    ip = int(dt)
-                    fp = dt%1
-                    for x in Data[xy]:
-                        Spectrum[x-ip] += (1-fp)
-                        Spectrum[x-ip-1] += fp
+                raw = self.get_raw_raw_data(s)
+                rawv = struct.unpack('<{}I'.format(len(raw) // 4), raw)
+                i = 0
+                while i < len(rawv):
+                    b = rawv[i]
+                    if b & 0xc0000000:
+                        x = b & 0x0fffffff
+                        dt = dts[x]
+                        ip = int(dt)
+                        fp = dt % 1
+                        i += 3
+                    else:
+                        Spectrum[b - ip] += (1 - fp)
+                        Spectrum[b - ip - 1] += fp
+                        i += 1
         elif type(ROI) is np.ndarray:
-            assert np.min(ROI)>=0
-            Spectrum = np.zeros((number_channels,np.max(ROI)+1), dtype=np.float32)
+            assert np.min(ROI) >= 0
+            Spectrum = np.zeros((number_channels, np.max(ROI) + 1), dtype=np.float32)
             for s in T:
-                Data = self.getRawData(s)[2]
-                if kargs.get('prog', False):
-                    LData = tqdm(Data, leave=False)
-                else:
-                    LData = Data
-                for xy in LData:
-                    dt = DT*(self.size['pixels']['x']/2-xy[0]) # time correction for the given x coordinate (in channel number)
-                    ip = int(dt)
-                    fp = dt%1
-                    id = ROI[xy[1],xy[0]]
-                    for x in Data[xy]:
-                        Spectrum[x-ip, id] += (1-fp)
-                        Spectrum[x-ip-1, id] += fp
-        elif type(ROI) in [list,tuple]:
+                raw = self.get_raw_raw_data(s)
+                rawv = struct.unpack('<{}I'.format(len(raw) // 4), raw)
+                i = 0
+                while i < len(rawv):
+                    b = rawv[i]
+                    if b & 0xc0000000:
+                        x = b & 0x0fffffff
+                        y = rawv[i + 1] & 0x0fffffff
+                        dt = dts[x]
+                        fp = dt % 1
+                        ip = int(dt)
+                        id = ROI[y, x]
+                        i += 3
+                    else:
+                        Spectrum[b - ip, id] += (1 - fp)
+                        Spectrum[b - ip - 1, id] += fp
+                        i += 1
+        elif type(ROI) in [list, tuple]:
             multi_roi = True
-            Spectrum = np.zeros((number_channels,len(ROI)), dtype=np.float32)
+            Spectrum = np.zeros((number_channels, len(ROI)), dtype=np.float32)
             for s in T:
-                Data = self.getRawData(s)[2]
-                for xy in Data:
-                    dt = DT*(self.size['pixels']['x']/2-xy[0]) # time correction for the given x coordinate (in channel number)
-                    ip = int(dt)
-                    fp = dt%1
-                    li = []
-                    for k,R in enumerate(ROI):
-                        if R[xy[1],xy[0]]:
-                            li.append(k)
-                    for x in Data[xy]:
+                raw = self.get_raw_raw_data(s)
+                rawv = struct.unpack('<{}I'.format(len(raw) // 4), raw)
+                i = 0
+                li = []
+                while i < len(rawv):
+                    b = rawv[i]
+                    if b & 0xc000000000:
+                        x = b & 0x0fffffff
+                        y = rawv[i + 1] & 0x0fffffff
+                        dt = dts[x]
+                        fp = dt % 1
+                        ip = int(dt)
+                        li = []
+                        for k, R in enumerate(ROI):
+                            if R[y, x]:
+                                li.append(k)
+                        i += 3
+                    else:
                         for k in li:
-                            Spectrum[x-ip,k] += (1-fp)
-                            Spectrum[x-ip-1,k] += fp
-        sf = kargs.get('sf',self.root.goto('MassScale/sf').getDouble())
-        k0 = kargs.get('k0',self.root.goto('MassScale/k0').getDouble())
-        masses = self.channel2mass(np.arange(number_channels),sf=sf,k0=k0)
+                            Spectrum[b - ip, k] += (1 - fp)
+                            Spectrum[b - ip - 1, k] += fp
+                        i += 1
+        if kargs.get('debug', False):
+            t1 = time.time()
+            print("Sepctra calc. time: ", t1 - t0)
+            t0 = t1
+        sf = kargs.get('sf', self.root.goto('MassScale/sf').get_double())
+        k0 = kargs.get('k0', self.root.goto('MassScale/k0').get_double())
+        masses = self.channel2mass(np.arange(number_channels), sf=sf, k0=k0)
         if deadTimeCorr:
-            dt = 1300 # 65ns*(1ch/50ps) = 1300 channels
-            N = self.Nscan*self.size['pixels']['x']*self.size['pixels']['y'] # total of count events
+            dt = 1300  # 65ns*(1ch/50ps) = 1300 channels
+            N = self.Nscan * self.size['pixels']['x'] * self.size['pixels']['y']  # total of count events
             Np = np.zeros(Spectrum.shape)
-            if Spectrum.ndim>1:
+            if Spectrum.ndim > 1:
                 for i in range(Spectrum.shape[1]):
-                    Np[:,i] = N-np.convolve(Spectrum[:,i], np.ones(dt-1,dtype=int), 'full')[:-dt+2]
+                    Np[:, i] = N - np.convolve(Spectrum[:, i], np.ones(dt - 1, dtype=int), 'full')[:-dt + 2]
             else:
-                Np = N-np.convolve(Spectrum, np.ones(dt-1,dtype=int), 'full')[:-dt+2]
-            Np[Np==0] = 1
-            Spectrum = -N*np.log(1-Spectrum/Np)
-        if kargs.get('time',False):
+                Np = N - np.convolve(Spectrum, np.ones(dt - 1, dtype=int), 'full')[:-dt + 2]
+            Np[Np == 0] = 1
+            Spectrum = -N * np.log(1 - Spectrum / Np)
+        if kargs.get('debug', False):
+            t1 = time.time()
+            print("Dead time correction time: ", t1 - t0)
+            t0 = t1
+        if kargs.get('time', False):
             return np.arange(number_channels), Spectrum
         return masses, Spectrum
 
-    def getRawRawData(self, scan=0):
+    @alias("getRawRawData")
+    def get_raw_raw_data(self, scan=0):
         assert scan < self.Nscan
         found = False
         RAW = b''
         if self.rawlist is None:
-            self.rawlist = self.root.goto('rawdata').getList()
+            self.rawlist = self.root.goto('rawdata').get_list()
         startFound = False
         for x in self.rawlist:
             if x['name'] == '   6':
                 if not startFound:
                     startFound = x['id'] == scan
                 else:
                     break
             elif startFound and x['name'] == '  14':
                 self.root.f.seek(x['bidx'])
                 child = Block.Block(self.root.f)
                 RAW += zlib.decompress(child.value)
         if type(RAW) is str:
             return bytearray(RAW)
         return RAW
-        
-    def getRawData(self, scan=0):
+
+    def get_pixel_order(self, scan=0):
+        raw = self.get_raw_raw_data(scan)
+        rawv = struct.unpack('<{}I'.format(len(raw) // 4), raw)
+        pixel_order = np.zeros((self.size['pixels']['y'], self.size['pixels']['x']))
+        i = 0
+        while i < len(rawv):
+            b = rawv[i]
+            if b & 0xc0000000:
+                x = b & 0x0fffffff
+                y = rawv[i + 1] & 0x0fffffff
+                id = rawv[i + 2] & 0x3fffffff
+                pixel_order[y, x] = id
+                i += 3
+            else:
+                i += 1
+        return pixel_order
+
+    @alias("getRawData")
+    def get_raw_data(self, scan=0):
         """
         Function which allows you to read and parse the raw data.
-        With this you are able to reconstruct the data.
-        Somehow the number of channel is double in the raw data compared
-        to the compressed version saved in the ITA files.
-        scan: The scan number. Start at 0
-        """
-        RAW = self.getRawRawData(scan)
-        Blocks = {}
-        _Block = []
-        PixelList = []
-        PixelOrder = np.zeros((self.size['pixels']['y'], self.size['pixels']['x']))
+        It return a dictionary of list where each key is the pixel position (x,y) and the value is the list of all times (channel number).
+        """
+        raw = self.get_raw_raw_data(scan)
+        rawv = struct.unpack('<{}I'.format(len(raw) // 4), raw)
+        blocks = {}
         i = 0
-        while i < len(RAW):
-            b = RAW[i:i+4]
-            if b[3:4] == b'\xc0':
-                if len(_Block):
-                    Blocks[(x, y)] = _Block
-                b = b[:3] + b'\x00'
-                x = struct.unpack('<I', b)[0]
-                i += 4
-                b = RAW[i:i+4]
-                if b[3:4] != b'\xd0':
-                    raise TypeError("Expecting a D0 block at {}".format(i+3))
-                b = b[:3] + b'\x00'
-                y = struct.unpack('<I', b)[0]
-                i += 4
-                b = bytearray(RAW[i:i+4])
-                if b[3] < 64:
-                    raise TypeError("Expecting a 40 or higher block at {}, got {:02x}".format(i+3,b[3]))
-                b = b[:3] + bytearray([b[3]&16])
-                _Block = []
-                id = struct.unpack('<I', b)[0]
-                PixelOrder[y, x] = id
-                PixelList.append((x,y))
+        _block = []
+        x, y = -1, -1
+        while i < len(rawv):
+            b = rawv[i]
+            if b & 0xc0000000:
+                blocks[(x,
+                        y)] = _block  # Somehow it's faster to append the data to a list first and then attribute it to the dict
+                x = b & 0x0fffffff
+                y = rawv[i + 1] & 0x0fffffff
+                _block = []
+                i += 3
             else:
-                _Block.append(struct.unpack('<I', b)[0])
-            i += 4
-        return PixelList, PixelOrder, Blocks
+                _block.append(b)
+                i += 1
+        del blocks[(-1, -1)]
+        return blocks
 
     def show_masses(self, mass_list=None):
         """
         Display the peak list (assignment name with lower, center and upper mass)
         """
         for m in self.get_masses():
             if mass_list is None or m['id'] in [z['id'] for z in mass_list]:
                 print(
                     "{id}: ({desc}) [{assign}] {lmass:.2f}u - {umass:.2f}u (center: {cmass:.2f}u)".format(**m))
 
-    def showStage(self, ax=None, markers=False, plist=False):
+    @alias("showStage")
+    def show_stage(self, ax=None, markers=False, plist=False):
         """
         Display an image of the stage used
         ax: maplotlib axis to be ploted in. If None the current one (or new) will be used
         markers: If True will display on the map the Position List items.
         """
         import pickle
         import matplotlib as mpl
-        W = self.root.goto('SampleHolderInfo/bitmap/res_x').getLong()
-        H = self.root.goto('SampleHolderInfo/bitmap/res_y').getLong()
+        W = self.root.goto('SampleHolderInfo/bitmap/res_x').get_ulong()
+        H = self.root.goto('SampleHolderInfo/bitmap/res_y').get_ulong()
 
         if ax is None:
             import matplotlib.pyplot as plt
-            fig, ax = plt.subplots(1, 1, figsize=(W*10/H, 10))
+            fig, ax = plt.subplots(1, 1, figsize=(W * 10 / H, 10))
 
         Dat = zlib.decompress(self.root.goto(
             'SampleHolderInfo/bitmap/imagedata').value)
-        I = np.array(struct.unpack("<"+str(W*H*3)+"B", Dat)
-                         ).reshape((H, W, 3))
+        I = np.array(struct.unpack("<" + str(W * H * 3) + "B", Dat), dtype=np.uint8).reshape((H, W, 3))
         ax.imshow(I)
         if markers:
-            X = self.root.goto('Meta/SI Image[0]/stageposition_x').getDouble()
-            Y = self.root.goto('Meta/SI Image[0]/stageposition_y').getDouble()
+            X = self.root.goto('Meta/SI Image[0]/stageposition_x').get_double()
+            Y = self.root.goto('Meta/SI Image[0]/stageposition_y').get_double()
 
             def toXY(xy, W, H):
                 sx = 23
                 sy = 23
-                return (913+sx*xy[0], 1145+sy*xy[1])
+                return (913 + sx * xy[0], 1145 + sy * xy[1])
+
             if plist:
                 for x in self.root.goto('SampleHolderInfo/positionlist'):
                     if x.name == 'shpos':
                         y = pickle.loads(x.goto('pickle').value)
                         pos = toXY((y['stage_x'], y['stage_y']), W, H)
                         if pos[0] >= 0 and pos[0] < W and pos[1] >= 0 and pos[1] < H:
                             ax.annotate(y['name'], xy=pos, xytext=(-15, -25), textcoords='offset points',
                                         arrowprops=dict(arrowstyle='->', facecolor='black'))
             pos = toXY((X, Y), W, H)
             ax.plot(pos[0], pos[1], 'xr')
-            ll = toXY((X-self.fov*5e2, Y-self.fov*5e3), W, H)
-            ur = toXY((X+self.fov*5e2, Y+self.fov*5e3), W, H)
-            ax.add_patch(mpl.patches.Rectangle(ll, ur[0]-ll[0], ur[1]-ll[1], ec='lime', fill=False))
+            ll = toXY((X - self.fov * 5e2, Y - self.fov * 5e3), W, H)
+            ur = toXY((X + self.fov * 5e2, Y + self.fov * 5e3), W, H)
+            ax.add_patch(mpl.patches.Rectangle(ll, ur[0] - ll[0], ur[1] - ll[1], ec='lime', fill=False))
         ax.set_xlim((0, W))
         ax.set_ylim((0, H))
         ax.set_xticks([])
         ax.set_yticks([])
 
-    def getSnapshot(self):
+    @alias("getSnapshot")
+    def get_snapshot(self):
         """
         Return the video snapshot
         """
         try:
-            dl = self.root.goto('Meta/Video Snapshot').dictList()
-            sx = dl['res_x']['long']
-            sy = dl['res_y']['long']
-            img = np.array(self.root.goto('Meta/Video Snapshot/imagedata').getData('B')).reshape((sy, sx, 3))
-            return  img
+            dl = self.root.goto('Meta/Video Snapshot').dict_list()
+            sx = dl['res_x']['ulong']
+            sy = dl['res_y']['ulong']
+            img = np.array(self.root.goto('Meta/Video Snapshot/imagedata').get_data('B')).reshape((sy, sx, 3))
+            return img
         except Exception as e:
             return None
 
-    def showPeaks(self):
+    @alias("showPeaks")
+    def show_peaks(self):
         for p in self.peaks:
             P = self.peaks[p]
             label = P['assign']['utf16']
             if label:
                 print("{0}) {peaklabel}".format(p, peaklabel=label))
             else:
-                print("{0}) {cmass:.2f}u [{lmass:.2f}u-{umass:.2f}u]".format(p, cmass=P['cmass']['float'],lmass=P['lmass']['float'],umass=P['umass']['float']))
-            
-    def modify_block_and_export(self, path, new_data, output, **kargs):
+                print("{0}) {cmass:.2f}u [{lmass:.2f}u-{umass:.2f}u]".format(p, cmass=P['cmass']['float'],
+                                                                             lmass=P['lmass']['float'],
+                                                                             umass=P['umass']['float']))
+
+    def modify_block_and_export(self, path, new_data, output, reload=True, **kargs):
         self.root.modify_block_and_export(path, new_data, output, **kargs)
+        if reload:
+            self.f.close()
+            self.f.open(path, "rb+")
+            self.f.read(8)
+            self.root = Block.Block(self.f)
 
     def reconstruct(self, channels, scans=None, sf=None, k0=None, prog=False, time=False):
         """
         Reconstruct an Image from a raw spectra by defining the lower and upper mass
         channels: list of (lower_mass, upper_mass)
         upper_mass: upper mass of the peak
         scans: The list of the scans to take into account (if None, all scans are taken)
@@ -917,36 +1287,122 @@
         """
         from .utils import mass2time
         from . import SPM_image
         assert hasattr(channels, '__iter__')
         if not hasattr(channels[0], '__iter__'):
             channels = [channels]
         for c in channels:
-            assert len(c)==2
+            assert len(c) == 2
         if scans is None:
             scans = range(self.Nscan)
         if prog:
-            try:
-                from tqdm import tqdm_notebook as tqdm
-            except:
-                from tqdm import tqdm as tqdm
-            scans = tqdm(scans)
+            scans = PB(scans)
         left = np.array([x[0] for x in channels])
         right = np.array([x[1] for x in channels])
         if not time:
             if sf is None or k0 is None:
                 sf, k0 = self.get_mass_cal()
             left = mass2time(left, sf=sf, k0=k0)
             right = mass2time(right, sf=sf, k0=k0)
-        Counts = [np.zeros((self.size['pixels']['x'],self.size['pixels']['y'])) for x in channels]
+        Counts = [np.zeros((self.size['pixels']['x'], self.size['pixels']['y'])) for x in channels]
         for s in scans:
-            PixelList, PixelOrder, Data = self.getRawData(s)
+            Data = self.get_raw_data(s)
             for xy in Data:
-                for i,ch in enumerate(channels):
-                    Counts[i][xy[1],xy[0]] += np.sum((Data[xy]>=left[i])*(Data[xy]<=right[i]))
-        res = [SPM_image(C, real=self.size['real'], _type='TOF', channel="{0[0]:.2f}{unit}-{0[1]:.2f}{unit}".format(channels[i],unit=["u","s"][time]), zscale="Counts") for i,C in enumerate(Counts)]
+                for i, ch in enumerate(channels):
+                    Counts[i][xy[1], xy[0]] += np.sum((Data[xy] >= left[i]) * (Data[xy] <= right[i]))
+        res = [SPM_image(C, real=self.size['real'], _type='TOF',
+                         channel="{0[0]:.2f}{unit}-{0[1]:.2f}{unit}".format(channels[i], unit=["u", "s"][time]),
+                         zscale="Counts") for i, C in enumerate(Counts)]
         if len(res) == 1:
             return res[0]
+            return res[0]
         return res
-    
+
+    def create_new_miblock(self, assign, lmass=None, umass=None, cmass=None, desc="", _uuid=None, **kargs):
+        import uuid
+        if _uuid is None:
+            _uuid = str(uuid.uuid4())
+        if _uuid[0] != '{':
+            _uuid = '{' + _uuid + '}'
+        _uuid = _uuid.upper()
+        if lmass is None:
+            lmass = self.channel2mass(0)
+        if umass is None:
+            up = int(np.round(
+                self.get_value("Measurement.CycleTime")['float'] / self.get_value("Registration.TimeResolution")[
+                    'float'], 0))
+            umass = self.channel2mass(up)
+        new_index = max([x.head['ID'] for x in self.root.goto("MassIntervalList") if x.name == 'mi']) + 1
+        new_index2 = self.root.goto("Measurement Options/massintervals/NextId").get_ulong()
+        new_id = max([x.goto("id").get_ulong() for x in self.root.goto("MassIntervalList") if x.name == 'mi']) + 1
+        new_id2 = max([x.goto("id").get_ulong() for x in self.root.goto("Measurement Options/massintervals") if
+                       x.name == 'mi']) + 1
+        NID = self.root.goto("MassIntervalList/NextId", lazy=True)
+        NID.rewrite(struct.pack("<I", NID.get_ulong() + 1))
+        defaults = {
+            'clsid': ('raw', b'\x85\x1b\xa9\xe4hZ\xc8M\x93\xe0\x7f\xc0\xf8\xe2\xbb\xd9'),
+            'color': ('raw', b'\xff\x00\x00\x00'),
+            'symbolID': ('I', 8),
+            'RSF': ('d', 0),
+            'label': ('B', 1),
+            'peaklabel': ('I', 0),
+            'edrfl': ('I', 0),
+            'attr.ConsiderBurstMode': ('B', 1),
+            'attr.Normalized': ('B', 0),
+            'attr.PoissonCorrectable': ('B', 1),
+            'attr.Sticky': ('B', 0),
+            'attr.Visible': ('B', 1)
+        }
+        p = dict(new_index=new_index, new_index2=new_index2)
+        self.root.edit_block("Measurement Options/massintervals/mi[{new_index2}]".format(**p), "id",
+                             struct.pack("<I", new_id))
+        self.root.edit_block("MassIntervalList/mi[{new_index}]".format(**p), "id", struct.pack("<I", new_id))
+        for path in ["Measurement Options/massintervals/mi[{new_index2}]", "MassIntervalList/mi[{new_index}]"]:
+            self.root.edit_block(path.format(**p), "desc", desc.encode('utf16')[2:])
+            self.root.edit_block(path.format(**p), "SN", _uuid.encode('utf16')[2:])
+            self.root.edit_block(path.format(**p), "assign", assign.encode('utf16')[2:])
+            self.root.edit_block(path.format(**p), "lmass", struct.pack("<d", lmass))
+            self.root.edit_block(path.format(**p), "umass", struct.pack("<d", umass))
+            if cmass is None:
+                cmass = (lmass + umass) / 2
+            self.root.edit_block(path.format(**p), "cmass", struct.pack("<d", cmass))
+            self.root.edit_block(path.format(**p), "desc", desc.encode('utf16')[2:])
+            for key in defaults:
+                data = kargs.get(key, defaults[key][1])
+                fmt = defaults[key][0]
+                if fmt == 'utf16':
+                    data = data.encode('utf16')[2:]
+                elif fmt == 'raw':
+                    pass
+                else:
+                    data = struct.pack("<" + fmt, data)
+                self.root.edit_block(path.format(**p), key, data)
+        blk = self.root.goto("MassIntervalList/mi[{new_index}]".format(**p))
+        d = blk.dict_list()
+        self.peaks[d['id']['long']] = d
+        return blk
+
     def __del__(self):
+        if self.f.writable():
+            self.f.flush()
+            os.fsync(self.f)
         self.f.close()
+
+    @alias("setK0")
+    def set_k0(self, k0):
+        import struct
+        try:
+            b = self.root.goto('filterdata/TofCorrection/Spectrum/Reduced Data/IMassScaleSFK0/k0')
+        except:
+            b = self.root.goto("MassScale/k0")
+        buffer = struct.pack("<d", k0)
+        b.rewrite(buffer);
+
+    @alias("setSF")
+    def set_sf(self, sf):
+        import struct
+        try:
+            b = self.root.goto('filterdata/TofCorrection/Spectrum/Reduced Data/IMassScaleSFK0/sf')
+        except:
+            b = self.root.goto("MassScale/sf")
+        buffer = struct.pack("<d", sf)
+        b.rewrite(buffer);
```

### Comparing `pySPM-0.2.9/pySPM/nanoscan.py` & `pyspm-0.3.0/pySPM/nanoscan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # -- coding: utf-8 --
 
 # Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
 
-import os
 import base64
-import xml.etree.ElementTree as ET
+import os
 import struct
+import xml.etree.ElementTree as ET
+
 import numpy as np
+
 import pySPM.SPM
 from pySPM.SPM import SPM_image, funit
+from .utils.misc import aliased, alias, deprecated
 
 
-def getCurve(filename, channel='Normal Deflection', backward=False):
+@deprecated("getCurve")
+def get_curve(filename, channel='Normal Deflection', backward=False):
     """
     function to retrieve data which are not in the form of images.
     This is typically used for 1D channel where the normal deflection is recorded while z is swept.
     """
     tree = ET.parse(filename)
     root = tree.getroot()
     namespace = {'spm': 'http://www.nanoscan.ch/SPM'}
@@ -28,21 +32,21 @@
                                "spm:contents/spm:start/spm:vector/spm:v", namespace)[0].text)
     stop = float(root.findall("spm:vector/spm:contents/spm:axis/spm:vector/"
                               "spm:contents/spm:stop/spm:vector/spm:v", namespace)[0].text)
     unit = root.findall("spm:vector/spm:contents/spm:axis/spm:vector/spm:contents"
                         "/spm:unit/spm:v", namespace)[0].text
     BIN = base64.b64decode(RAW)
     N = len(BIN)
-    vals = np.array(struct.unpack("<"+str(N//4)+"f", BIN))
+    vals = np.array(struct.unpack("<" + str(N // 4) + "f", BIN))
     x = np.linspace(start, stop, len(vals))
     return x, vals
 
 
+@aliased
 class Nanoscan():
-
     def __init__(self, filename=None):
         if not os.path.exists(filename):
             raise IOError('File "{0}" Not Found'.format(filename))
         if filename[-4:] != '.xml':
             raise TypeError("Nanoscan files should be xml files")
         self.filename = filename
         tree = ET.parse(filename)
@@ -57,18 +61,18 @@
             uval = float(self.__grab(
                 ".//spm:area//spm:contents/spm:size/spm:contents/spm:fast_axis/spm:v"))
             udispu = self.__grab(
                 ".//spm:area//spm:contents/spm:display_unit/spm:v")
             udisps = float(self.__grab(
                 ".//spm:area/spm:contents/spm:display_scale/spm:v"))
             uname = self.__grab(".//spm:area/spm:contents/spm:unit/spm:v")
-            x = funit(uval*udisps, udispu)
+            x = funit(uval * udisps, udispu)
             uval = float(self.__grab(
                 ".//spm:area//spm:contents/spm:size/spm:contents/spm:slow_axis/spm:v"))
-            y = funit(uval*udisps, udispu)
+            y = funit(uval * udisps, udispu)
             self.size = {
                 'unit': x['unit'],
                 'x': x['value'],
                 'y': y['value']}
             try:
                 self.feedback = {'channel': self.__grab(
                     '{0}/spm:z_feedback_channel/spm:v'.format(self.fbPath))}
@@ -80,68 +84,75 @@
                     'unit': self.__grab('{0}/spm:integral_z_time_unit/spm:v'.format(self.fbPath))}
                 if self.feedback['channel'] == 'df':
                     self.feedback['channel'] = u'Δf'
             except:
                 self.feedback = {}
             self.scan_speed = {
                 z: {
-                    'value': float(self.__grab("spm:vector//spm:direction/spm:vector/spm:contents/spm:name[spm:v='{dir}']/../spm:point_interval/spm:v".format(dir=z))) * self.pixel_size[0],
-                    'unit': self.__grab("spm:vector//spm:direction/spm:vector/spm:contents/spm:name[spm:v='{dir}']/../spm:point_interval_unit/spm:v".format(dir=z))} for z in ['forward', 'backward']}
+                    'value': float(self.__grab(
+                        "spm:vector//spm:direction/spm:vector/spm:contents/spm:name[spm:v='{dir}']/../spm:point_interval/spm:v".format(
+                            dir=z))) * self.pixel_size[0],
+                    'unit': self.__grab(
+                        "spm:vector//spm:direction/spm:vector/spm:contents/spm:name[spm:v='{dir}']/../spm:point_interval_unit/spm:v".format(
+                            dir=z))} for z in ['forward', 'backward']}
         else:
             raise TypeError(
                 "Unknown or wrong data type. Expecting a valid Nanoscan xml")
-    
+
     def list_channels(self):
         """
         Printout the list of stored channels
         """
-        for d in ['forward','backward']:
+        for d in ['forward', 'backward']:
             print(d)
-            print("="*len(d))
-            for z in self.root.findall("spm:vector//spm:direction/spm:vector/spm:contents/spm:name[spm:v='{}']/../spm:channel//spm:contents/spm:name/spm:v".format(d), self.namespaces):
-                print("  - "+z.text)
+            print("=" * len(d))
+            for z in self.root.findall(
+                    "spm:vector//spm:direction/spm:vector/spm:contents/spm:name[spm:v='{}']/../spm:channel//spm:contents/spm:name/spm:v".format(
+                        d), self.namespaces):
+                print("  - " + z.text)
             print()
 
     def get_channel(self, channel='Topography', backward=False, corr=None):
         try:
             RAW = self.__grab("spm:vector//spm:direction/spm:vector/spm:contents"
                               "/spm:name[spm:v='{direction}']/../spm:channel//spm:contents/spm:name[spm:v='{channel}']"
                               "/../spm:data/spm:v".format(direction=["forward", "backward"][backward], channel=channel))
         except:
             raise 'Channel {0} in {1} scan not found'.format(
-                channel, direction)
+                channel, "backward" if backward else "forward")
             return None
 
         BIN = base64.b64decode(RAW)
-        recorded_length = len(BIN)/4
+        recorded_length = len(BIN) / 4
 
-        py = int(recorded_length/self.pixel_size[0])
+        py = int(recorded_length / self.pixel_size[0])
         recorded_size = {
             'x': self.size['x'],
-            'y': self.size['y']*py/float(self.pixel_size[1]),
+            'y': self.size['y'] * py / float(self.pixel_size[1]),
             'unit': self.size['unit']}
 
         image_array = np.array(struct.unpack("<%if" % (recorded_length), BIN)).reshape(
             (py, self.pixel_size[0]))
         return SPM_image(image_array, channel=channel, _type=self.type, real=recorded_size, corr=corr)
 
     def __grab(self, path):
         result = [z.text for z in self.root.findall(path, self.namespaces)]
         if len(result) == 1:
             result = result[0]
         return result
 
-    def arraySummary(self):
-        from pySPM.utils import htmlTable
+    @deprecated("arraySummary")
+    def array_summary(self):
         res = [y.format(**self.__dict__) for y in
                ["{filename}", "{pixel_size[0]}×{pixel_size[1]}", "{size[x][value]}×{size[y][value]} {size[x][unit]}",
                 "{scan_speed[forward][value]} {scan_speed[forward][unit]}",
                 "{feedback[channel]}", "{P[value]:.2f} {P[unit]}", "{I[value]:.2f} {I[unit]}"]]
 
-    def getSummary(self):
+    @alias("getSummary")
+    def get_summary(self):
         x = funit(self.size['x'], self.size['unit'])
         y = funit(self.size['y'], self.size['unit'])
         P = funit(self.feedback['P'])
         I = funit(self.feedback['I'])
         return u"""Feedback: {feedback[channel]} : P:{P[value]}{P[unit]} : I:{I[value]}{I[unit]}
 Size: {pixel_size[0]}×{pixel_size[1]} pixels = {x[value]:.3} {x[unit]}×{y[value]:.3} {y[unit]}
 Scan Speed: {scanSpeed[value]}{scanSpeed[unit]}/line""".format(
@@ -152,14 +163,16 @@
     @staticmethod
     def show_dir_summary(path):
         from pySPM.utils import htmlTable
         res = [["Filename", "pixel size", "real size",
                 "scan_speed", "feedback", "P", "I"]]
         for x in os.listdir(path):
             try:
-                A = pySPM.Nanoscan(path+x)
+                A = pySPM.Nanoscan(path + x)
                 res.append([y.format(f=os.path.basename(A.filename), **A.__dict__) for y in
-                        ["{f}", "{pixel_size[0]}×{pixel_size[1]}", "{size[x]}×{size[y]} {size[unit]}", "{scan_speed[forward][value]} {scan_speed[forward][unit]}",
-                         "{feedback[channel]}", "{feedback[P][value]:.2f} {feedback[P][unit]}", "{feedback[I][value]:.2f} {feedback[I][unit]}"]])
+                            ["{f}", "{pixel_size[0]}×{pixel_size[1]}", "{size[x]}×{size[y]} {size[unit]}",
+                             "{scan_speed[forward][value]} {scan_speed[forward][unit]}",
+                             "{feedback[channel]}", "{feedback[P][value]:.2f} {feedback[P][unit]}",
+                             "{feedback[I][value]:.2f} {feedback[I][unit]}"]])
             except:
-                print("Cannot read image \""+x+"\" skipping it")
+                print("Cannot read image \"" + x + "\" skipping it")
         htmlTable(res, header=True)
```

### Comparing `pySPM-0.2.9/pySPM/PCA.py` & `pyspm-0.3.0/pySPM/PCA.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,55 +2,58 @@
 
 # Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
 
 """
 This module performs the PCS with the help of the scikit library and gives the user various function for quick plotting.
 """
 
-import pandas as pd
-import numpy as np
-from sklearn.preprocessing import scale
-from sklearn.decomposition import PCA as PCA1
-from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
-from scipy import stats
+from __future__ import absolute_import
+
+import re
+
 import matplotlib.pyplot as plt
-from pySPM.SPM import SPM_image
-import matplotlib as mpl
+import numpy as np
+import pandas as pd
 from matplotlib import cm
+from sklearn.decomposition import PCA as PCA1
+from sklearn.preprocessing import scale
+
 from pySPM import collection
-import re
+from .utils.misc import aliased, alias
 
-class PCA:
 
+@aliased
+class PCA:
     def __init__(self, data):
         self.data = data
         self.pca = None
         self.standX = None
 
     def scatter(self, **kargs):
         pd.tools.plotting.scatter_matrix(self.data, diagonal="kde", **kargs)
         plt.tight_layout()
 
     def corr(self):
         corrmat = self.data.corr()
         return corrmat
 
-    def corrShow(self):
+    @alias("corrShow")
+    def show_corr(self):
         import seaborn as sns
         corrmat = self.corr()
         sns.heatmap(corrmat).xaxis.tick_top()
 
-    def hinton(self, max_weight=None, ax=None, matrix = None, xlabel=None, ylabel=None):
+    def hinton(self, max_weight=None, ax=None, matrix=None, xlabel=None, ylabel=None):
         """Draw Hinton diagram for visualizing a weight matrix."""
         if matrix is None:
             matrix = self.corr()
         ax = ax if ax is not None else plt.gca()
 
         if not max_weight:
-            max_weight = 2**np.ceil(np.log(np.abs(matrix).max())/np.log(2))
+            max_weight = 2 ** np.ceil(np.log(np.abs(matrix).max()) / np.log(2))
 
         ax.patch.set_facecolor('lightgray')
         ax.set_aspect('equal', 'box')
         ax.xaxis.set_major_locator(plt.NullLocator())
         ax.yaxis.set_major_locator(plt.NullLocator())
 
         for (x, y), w in np.ndenumerate(matrix):
@@ -61,19 +64,19 @@
             ax.add_patch(rect)
 
         nxticks = matrix.shape[1]
         nyticks = matrix.shape[0]
         if xlabel is None:
             xlabel = []
             for x in list(matrix.columns):
-                x = re.sub(r'\^([0-9]+)',r'^{\1}', x)
-                x = re.sub(r'_([0-9]+)',r'_{\1}', x)
-                if x[-1] in ['+','-']:
-                    x = x[:-1]+'^'+x[-1]
-                xlabel.append('$'+x+'$')
+                x = re.sub(r'\^([0-9]+)', r'^{\1}', x)
+                x = re.sub(r'_([0-9]+)', r'_{\1}', x)
+                if x[-1] in ['+', '-']:
+                    x = x[:-1] + '^' + x[-1]
+                xlabel.append('$' + x + '$')
         if ylabel is None:
             ylabel = list(matrix.index)
         ax.xaxis.tick_top()
         ax.set_xticks(range(nxticks))
         ax.set_xticklabels(xlabel, rotation=90)
         ax.set_yticks(range(nyticks))
         ax.set_yticklabels(ylabel)
@@ -83,123 +86,143 @@
         ax.invert_yaxis()
 
     def standardized(self, meanCentering=True):
         self.standX = pd.DataFrame(
             scale(self.data, with_mean=meanCentering), index=self.data.index, columns=self.data.columns)
         return self.standX
 
-    def runPCA(self, meanCentering=True):
+    @alias("runPCA")
+    def run_pca(self, meanCentering=True):
         if self.standX is None:
             self.standardized(meanCentering=meanCentering)
         self.pca = PCA1().fit(self.standX)
 
     def pca_summary(self):
         if self.pca is None:
-            self.runPCA()
-        names = ["PC"+str(i)
-                 for i in range(1, len(self.pca.explained_variance_ratio_)+1)]
+            self.run_pca()
+        names = ["PC" + str(i)
+                 for i in range(1, len(self.pca.explained_variance_ratio_) + 1)]
         a = list(np.std(self.pca.transform(self.standX), axis=0))
         b = list(self.pca.explained_variance_ratio_)
         c = [np.sum(self.pca.explained_variance_ratio_[:i])
-             for i in range(1, len(self.pca.explained_variance_ratio_)+1)]
+             for i in range(1, len(self.pca.explained_variance_ratio_) + 1)]
         columns = pd.MultiIndex.from_tuples([("sdev", "Standard deviation"), (
             "varprop", "Proportion of Variance"), ("cumprop", "Cumulative Proportion")])
         Z = zip(a, b, c)
         summary = pd.DataFrame(list(Z), index=names, columns=columns)
         return summary
 
     def screeplot(self, ax=None, num=None):
         if self.pca is None:
-            self.runPCA()
+            self.run_pca()
         ax = ax if ax is not None else plt.gca()
-        
-        y = np.std(self.pca.transform(self.standX), axis=0)**2
+
+        y = np.std(self.pca.transform(self.standX), axis=0) ** 2
         if num is None:
             num = len(y)
         x = np.arange(len(y)) + 1
         ax.grid(True)
         ax.plot(x[:num], y[:num], "o-")
         ax.set_xticks(x[:num])
-        ax.set_xticklabels(["PC"+str(i) for i in x[:num]], rotation=60)
+        ax.set_xticklabels(["PC" + str(i) for i in x[:num]], rotation=60)
         ax.set_ylabel("Variance")
 
     def pc(self, id=0):
         # find the number of samples in the data set and the number of
         # variables
         if self.pca is None:
-            self.runPCA()
+            self.run_pca()
         pc = np.matmul(self.standX.values, self.pca.components_[id].T)
         return pc
 
     def loadings(self, id=None):
         if self.pca is None:
-            self.runPCA()
+            self.run_pca()
         if id is not None:
             return pd.DataFrame(self.pca.components_[id, None], columns=self.data.columns)
-        return pd.DataFrame(self.pca.components_, columns=self.data.columns, index=["PC{0}".format(i+1) for i in range(len(self.pca.components_))])
+        return pd.DataFrame(self.pca.components_, columns=self.data.columns,
+                            index=["PC{0}".format(i + 1) for i in range(len(self.pca.components_))])
 
-    def getPCAtransf(self):
+    @alias("getPCAtransf")
+    def get_pca_transf(self):
         if self.pca is None:
-            self.runPCA()
+            self.run_pca()
         return self.pca.transform(self.standX)
 
-    def showStand(self):
+    @alias("showStand")
+    def show_stand(self):
         return pd.DataFrame([self.standX.apply(np.mean), self.standX.apply(np.std)], index=['Mean', 'Std'])
 
     def pca_scatter(self, classifs=None, light=False):
         import seaborn as sns
-        foo = self.getPCAtransf()
+        foo = self.get_pca_transf()
         if classifs is None:
             if light:
                 plt.scatter(foo[:, 0], foo[:, 1])
             else:
                 bar = pd.DataFrame(
                     list(zip(foo[:, 0], foo[:, 1])), columns=["PC1", "PC2"])
                 sns.lmplot("PC1", "PC2", bar, fit_reg=False)
         else:
             if light:
                 plt.scatter(foo[:, 0], foo[:, 1], color=cm.Scalar)
             else:
                 bar = pd.DataFrame(list(zip(foo[:, 0], foo[:, 1], classifs)), columns=[
-                                   "PC1", "PC2", "Class"])
+                    "PC1", "PC2", "Class"])
                 sns.lmplot("PC1", "PC2", bar, hue="Class", fit_reg=False)
 
 
 class ITA_PCA(PCA):
     def __init__(self, c, channels=None):
         """Init a PCA class from a collection"""
         self.col = c
         if channels is None:
             channels = c.channels.keys()
         mul = self.col.get_multivariate(channels)
         PCA.__init__(self, mul)
 
-    def showPCA(self, num=None, ax=None, pn=False, cmap=None, symmetric=True, **kargs):
-        c = self.getPCAcol(num, pn)
+    @alias("showPCA")
+    def show_pca(self, num=None, ax=None, pn=False, cmap=None, symmetric=True, loadings=True, **kargs):
+        c = self.get_pca_col(num, pn)
         if cmap is None:
             if pn:
                 cmap = 'viridis'
                 symmetric = False
             else:
                 cmap = 'bwr'
+        L = self.loadings()[:num]
+        if loadings:
+            N = len(c)
+            ncols = kargs.get('ncols', 4)
+            width = kargs.get('width', 21)
+            Ny = (N - 1) // ncols + 2
+            Nx = min(ncols, N)
+            from matplotlib.gridspec import GridSpec
+            fig = plt.figure(figsize=(width, (Ny - 1) * width / Nx + width * N / len(L.columns)))
+            gs = GridSpec(Ny, Nx, height_ratios=[width / Nx for i in range(Ny - 1)] + [width * N / len(L.columns)])
+            ax = [plt.subplot(gs[i, j]) for i in range(Ny - 1) for j in range(Nx)]
+            axh = plt.subplot(gs[-1, :])
+            self.hinton(matrix=L, ax=axh)
         c.show(ax=ax, cmap=cmap, symmetric=symmetric, **kargs)
+        return L
 
-
-    def getPCAcol(self, num=None, pn=False):
+    @alias("getPCAcol")
+    def get_pca_col(self, num=None, pn=False):
         if num is None:
             num = self.data.shape[1]
         assert num <= self.data.shape[1]
         PCA_col = collection.Collection(
-            cls=self.col, name=self.col.name+"[PCA]")
+            cls=self.col, name=self.col.name + "[PCA]")
         for i in range(num):
-            PC = self.getPCA(i)
+            PC = self.get_pca(i)
             if pn:
-                PCA_col.add(PC*(PC>=0), 'PC{0}+'.format(i+1))
-                PCA_col.add(-PC*(PC<=0), 'PC{0}-'.format(i+1))
+                PCA_col.add(PC * (PC >= 0), 'PC{0}+'.format(i + 1))
+                PCA_col.add(-PC * (PC <= 0), 'PC{0}-'.format(i + 1))
             else:
-                PCA_col.add(PC, 'PC{0}'.format(i+1))
+                PCA_col.add(PC, 'PC{0}'.format(i + 1))
         return PCA_col
 
-    def getPCA(self, id=0):
+    @alias("getPCA")
+    def get_pca(self, id=0):
         s = list(self.col.channels.values())[0].pixels.shape
         PC = self.pc(id).reshape(s)
         return PC
```

### Comparing `pySPM-0.2.9/pySPM/slicer.py` & `pyspm-0.3.0/pySPM/slicer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,106 +1,108 @@
-# -*- coding: utf-8 -*-
-
-# Form implementation generated from reading ui file 'C:\Users\ols\Dropbox\Python\pySPM\slicer.ui'
-#
-# Created by: PyQt5 UI code generator 5.6
-#
-# WARNING! All changes made in this file will be lost!
-
-from PyQt5 import QtCore, QtGui, QtWidgets
-
-class Ui_slicer(object):
-    def setupUi(self, slicer):
-        slicer.setObjectName("slicer")
-        slicer.resize(802, 547)
-        self.gridLayout = QtWidgets.QGridLayout(slicer)
-        self.gridLayout.setObjectName("gridLayout")
-        self.peakList = QtWidgets.QTableWidget(slicer)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.peakList.sizePolicy().hasHeightForWidth())
-        self.peakList.setSizePolicy(sizePolicy)
-        self.peakList.setContextMenuPolicy(QtCore.Qt.ActionsContextMenu)
-        self.peakList.setObjectName("peakList")
-        self.peakList.setColumnCount(3)
-        self.peakList.setRowCount(0)
-        item = QtWidgets.QTableWidgetItem()
-        self.peakList.setHorizontalHeaderItem(0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.peakList.setHorizontalHeaderItem(1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.peakList.setHorizontalHeaderItem(2, item)
-        self.gridLayout.addWidget(self.peakList, 0, 0, 1, 1)
-        self.mpl = MplWidget(slicer)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.mpl.sizePolicy().hasHeightForWidth())
-        self.mpl.setSizePolicy(sizePolicy)
-        self.mpl.setMinimumSize(QtCore.QSize(500, 500))
-        self.mpl.setObjectName("mpl")
-        self.gridLayout.addWidget(self.mpl, 0, 1, 1, 1)
-        self.horizontalLayout = QtWidgets.QHBoxLayout()
-        self.horizontalLayout.setObjectName("horizontalLayout")
-        self.status = QtWidgets.QLabel(slicer)
-        self.status.setObjectName("status")
-        self.horizontalLayout.addWidget(self.status)
-        self.correction = QtWidgets.QCheckBox(slicer)
-        self.correction.setLayoutDirection(QtCore.Qt.RightToLeft)
-        self.correction.setObjectName("correction")
-        self.horizontalLayout.addWidget(self.correction)
-        self.gridLayout.addLayout(self.horizontalLayout, 1, 0, 1, 1)
-        self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
-        self.horizontalLayout_2.setObjectName("horizontalLayout_2")
-        self.pb = QtWidgets.QProgressBar(slicer)
-        self.pb.setEnabled(True)
-        self.pb.setProperty("value", 0)
-        self.pb.setInvertedAppearance(False)
-        self.pb.setObjectName("pb")
-        self.horizontalLayout_2.addWidget(self.pb)
-        self.label_2 = QtWidgets.QLabel(slicer)
-        self.label_2.setObjectName("label_2")
-        self.horizontalLayout_2.addWidget(self.label_2)
-        self.prof1daxis = QtWidgets.QComboBox(slicer)
-        self.prof1daxis.setObjectName("prof1daxis")
-        self.prof1daxis.addItem("")
-        self.prof1daxis.addItem("")
-        self.prof1daxis.addItem("")
-        self.horizontalLayout_2.addWidget(self.prof1daxis)
-        self.label = QtWidgets.QLabel(slicer)
-        self.label.setObjectName("label")
-        self.horizontalLayout_2.addWidget(self.label)
-        self.cmap = QtWidgets.QComboBox(slicer)
-        self.cmap.setObjectName("cmap")
-        self.cmap.addItem("")
-        self.cmap.addItem("")
-        self.cmap.addItem("")
-        self.cmap.addItem("")
-        self.horizontalLayout_2.addWidget(self.cmap)
-        self.gridLayout.addLayout(self.horizontalLayout_2, 1, 1, 1, 1)
-
-        self.retranslateUi(slicer)
-        QtCore.QMetaObject.connectSlotsByName(slicer)
-
-    def retranslateUi(self, slicer):
-        _translate = QtCore.QCoreApplication.translate
-        slicer.setWindowTitle(_translate("slicer", "Slicer"))
-        item = self.peakList.horizontalHeaderItem(0)
-        item.setText(_translate("slicer", "Name"))
-        item = self.peakList.horizontalHeaderItem(1)
-        item.setText(_translate("slicer", "center mass"))
-        item = self.peakList.horizontalHeaderItem(2)
-        item.setText(_translate("slicer", "Δ mass"))
-        self.status.setText(_translate("slicer", "Loading..."))
-        self.correction.setText(_translate("slicer", "Apply Correction"))
-        self.label_2.setText(_translate("slicer", "1D plot on"))
-        self.prof1daxis.setItemText(0, _translate("slicer", "X"))
-        self.prof1daxis.setItemText(1, _translate("slicer", "Y"))
-        self.prof1daxis.setItemText(2, _translate("slicer", "Z"))
-        self.label.setText(_translate("slicer", "Colormap"))
-        self.cmap.setItemText(0, _translate("slicer", "viridis"))
-        self.cmap.setItemText(1, _translate("slicer", "gray"))
-        self.cmap.setItemText(2, _translate("slicer", "hot"))
-        self.cmap.setItemText(3, _translate("slicer", "jet"))
-
-from mplwidget import MplWidget
+# -*- coding: utf-8 -*-
+
+# Form implementation generated from reading ui file 'C:\Users\ols\Dropbox\Python\pySPM\slicer.ui'
+#
+# Created by: PyQt5 UI code generator 5.6
+#
+# WARNING! All changes made in this file will be lost!
+
+from PyQt5 import QtCore, QtWidgets
+
+
+class Ui_slicer(object):
+    def setupUi(self, slicer):
+        slicer.setObjectName("slicer")
+        slicer.resize(802, 547)
+        self.gridLayout = QtWidgets.QGridLayout(slicer)
+        self.gridLayout.setObjectName("gridLayout")
+        self.peakList = QtWidgets.QTableWidget(slicer)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.peakList.sizePolicy().hasHeightForWidth())
+        self.peakList.setSizePolicy(sizePolicy)
+        self.peakList.setContextMenuPolicy(QtCore.Qt.ActionsContextMenu)
+        self.peakList.setObjectName("peakList")
+        self.peakList.setColumnCount(3)
+        self.peakList.setRowCount(0)
+        item = QtWidgets.QTableWidgetItem()
+        self.peakList.setHorizontalHeaderItem(0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.peakList.setHorizontalHeaderItem(1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.peakList.setHorizontalHeaderItem(2, item)
+        self.gridLayout.addWidget(self.peakList, 0, 0, 1, 1)
+        self.mpl = MplWidget(slicer)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.mpl.sizePolicy().hasHeightForWidth())
+        self.mpl.setSizePolicy(sizePolicy)
+        self.mpl.setMinimumSize(QtCore.QSize(500, 500))
+        self.mpl.setObjectName("mpl")
+        self.gridLayout.addWidget(self.mpl, 0, 1, 1, 1)
+        self.horizontalLayout = QtWidgets.QHBoxLayout()
+        self.horizontalLayout.setObjectName("horizontalLayout")
+        self.status = QtWidgets.QLabel(slicer)
+        self.status.setObjectName("status")
+        self.horizontalLayout.addWidget(self.status)
+        self.correction = QtWidgets.QCheckBox(slicer)
+        self.correction.setLayoutDirection(QtCore.Qt.RightToLeft)
+        self.correction.setObjectName("correction")
+        self.horizontalLayout.addWidget(self.correction)
+        self.gridLayout.addLayout(self.horizontalLayout, 1, 0, 1, 1)
+        self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_2.setObjectName("horizontalLayout_2")
+        self.pb = QtWidgets.QProgressBar(slicer)
+        self.pb.setEnabled(True)
+        self.pb.setProperty("value", 0)
+        self.pb.setInvertedAppearance(False)
+        self.pb.setObjectName("pb")
+        self.horizontalLayout_2.addWidget(self.pb)
+        self.label_2 = QtWidgets.QLabel(slicer)
+        self.label_2.setObjectName("label_2")
+        self.horizontalLayout_2.addWidget(self.label_2)
+        self.prof1daxis = QtWidgets.QComboBox(slicer)
+        self.prof1daxis.setObjectName("prof1daxis")
+        self.prof1daxis.addItem("")
+        self.prof1daxis.addItem("")
+        self.prof1daxis.addItem("")
+        self.horizontalLayout_2.addWidget(self.prof1daxis)
+        self.label = QtWidgets.QLabel(slicer)
+        self.label.setObjectName("label")
+        self.horizontalLayout_2.addWidget(self.label)
+        self.cmap = QtWidgets.QComboBox(slicer)
+        self.cmap.setObjectName("cmap")
+        self.cmap.addItem("")
+        self.cmap.addItem("")
+        self.cmap.addItem("")
+        self.cmap.addItem("")
+        self.horizontalLayout_2.addWidget(self.cmap)
+        self.gridLayout.addLayout(self.horizontalLayout_2, 1, 1, 1, 1)
+
+        self.retranslateUi(slicer)
+        QtCore.QMetaObject.connectSlotsByName(slicer)
+
+    def retranslateUi(self, slicer):
+        _translate = QtCore.QCoreApplication.translate
+        slicer.setWindowTitle(_translate("slicer", "Slicer"))
+        item = self.peakList.horizontalHeaderItem(0)
+        item.setText(_translate("slicer", "Name"))
+        item = self.peakList.horizontalHeaderItem(1)
+        item.setText(_translate("slicer", "center mass"))
+        item = self.peakList.horizontalHeaderItem(2)
+        item.setText(_translate("slicer", "Δ mass"))
+        self.status.setText(_translate("slicer", "Loading..."))
+        self.correction.setText(_translate("slicer", "Apply Correction"))
+        self.label_2.setText(_translate("slicer", "1D plot on"))
+        self.prof1daxis.setItemText(0, _translate("slicer", "X"))
+        self.prof1daxis.setItemText(1, _translate("slicer", "Y"))
+        self.prof1daxis.setItemText(2, _translate("slicer", "Z"))
+        self.label.setText(_translate("slicer", "Colormap"))
+        self.cmap.setItemText(0, _translate("slicer", "viridis"))
+        self.cmap.setItemText(1, _translate("slicer", "gray"))
+        self.cmap.setItemText(2, _translate("slicer", "hot"))
+        self.cmap.setItemText(3, _translate("slicer", "jet"))
+
+
+from mplwidget import MplWidget
```

### Comparing `pySPM-0.2.9/pySPM/SPM.py` & `pyspm-0.3.0/pySPM/SPM.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,1813 +1,1877 @@
-# -- coding: utf-8 --
-
-# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
-
-"""
-Library to handle SPM data.
-This is the core module of all images retrieved by SPM and ToF-SIMS.
-"""
-
-import numpy as np
-import matplotlib.pyplot as plt
-import scipy
-import scipy.ndimage
-import scipy.optimize
-import skimage
-import skimage.exposure
-import skimage.filters
-import scipy.interpolate
-from skimage import transform as tf
-import copy
-from .utils import CDF, funit
-import sys
-
-try:
-    from tqdm import tqdm_notebook as tqdm
-except:
-    try:
-        from tqdm import tqdm
-    except:
-        tqdm = lambda x: x
-        
-import matplotlib as mpl
-import warnings
-
-try:
-    from skimage.filters import threshold_local
-except:
-    # For compatibility with old versions of skimage
-    from skimage.filters import threshold_adaptive as threshold_local
-   
-class SPM_image:
-    """
-    Main class to handle SPM images.
-    This class contains the pixels data of the images as well as it's real size.
-    It also provides a lot of tools to correct and perform various analysis and tasks on the image.
-    """
-    
-    def __init__(self, BIN, channel='Topography',
-                 corr=None, real=None, zscale='?', _type='Unknown'):
-        """
-        Create a new SPM_image
-
-        Parameters
-        ----------
-        BIN : 2D numpy array
-            The pixel values of the image as a 2D numpy array
-        channel : string
-            The name of the channel. What does the image represents?
-        corr : string or None
-            'slope' : correct the SPM image for its slope (see pySPM.SPM.SPM_image.correct_slope)
-            'lines' : correct the SPM image for its lines (see pySPM.SPM.SPM_image.correct_lines)
-            'plane' : correct the SPM image by plane fitting (see pySPM.SPM.SPM_image.correct_plane)
-        real : None or dictionary
-            Information about the real size of the image {'x':width,'y':height,'unit':unit_name}
-        zscale : string
-            Unit used to describe the z-scale. (units of the data of BIN)
-        _type : string
-            represent the type of measurement
-        """
-        self.channel = channel
-        self.direction = 'Unknown'
-        self.size = {'pixels': {'x': BIN.shape[1], 'y': BIN.shape[0]}}
-        if not real is None:
-            self.size['real'] = real
-        else:
-            self.size['real'] = {'unit': 'pixels',
-                                 'x': BIN.shape[1], 'y': BIN.shape[0]}
-        if not 'unit' in self.size['real']:
-            self.size['real']['unit'] = 'px'
-        self.pixels = BIN
-        self.type = _type
-        self.zscale = zscale
-        if corr is not None:
-            if corr.lower() == 'slope':
-                self.correct_slope()
-            elif corr.lower() == 'lines':
-                self.correct_lines()
-            elif corr.lower() == 'plane':
-                self.correct_plane()
-            
-    def __add__(self, b):
-        """
-        Add up two images. This is a low level function and no check is performed to proof that both images have the same size.
-        """
-        New = copy.deepcopy(self)
-        New.pixels += b.pixels
-        New.channel += " + "+b.channel
-        return New
-    
-    def pxs(self):
-        """
-        Return the pixel size
-        """
-        fxy = {xy: funit(self.size['real'][xy], self.size['real']['unit']) for xy in 'xy'}
-        return [(fxy[xy]['value']/self.size['pixels'][xy], fxy[xy]['unit']) for xy in 'xy']
-        
-    def add_scale(self, length, ax=None, height=20, color='w', loc=4, text=True, pixels=True, fontsize=20):
-        """
-        Display a scale marker on an existing image
-
-        Parameters
-        ----------
-
-        length : float
-            The length of the scale in real units
-        ax : matplotlib axis
-            if None the current axis will be taken (plt.gca())
-        height : int
-            The height of the scale bar in pixels
-        color : string
-            The color used to display the scale bar
-        loc : int
-            The location of the scale bar.
-            1 : top right
-            2 : top left
-            3 : bottom left
-            4 : bottom right
-        text : bool
-            display the size of the scale on top of it?
-        pixels : bool
-            Is the image plotted in ax with a x/y scale in pixels?
-        fontsize : float
-            The fontsize used to display the text
-
-        Example
-        -------
-        >>> img = pySPM.SPM_image()
-        >>> img.show()
-        >>> img.add_scale(50e-6, pixels=False);
-        Add a scale of 50 μm on an image displayed with real units
-
-        >>> img = pySPM.SPM_image()
-        >>> img.show(pixels=True)
-        >>> img.add_scale(50e-6);
-        Add a scale of 50 μm on an image displayed in pixels
-        """
-        import matplotlib.patches
-        L = length*self.size['pixels']['x']/self.size['real']['x']
-        ref = [height, height]
-        if loc == 1 or loc == 4:
-            ref[0] = self.size['pixels']['x'] - ref[0] - L
-        if loc == 3 or loc == 4:
-            ref[1] = self.size['pixels']['y'] - ref[1] - height
-        if ax is None:
-            ax = plt.gca()
-        if text and loc in [1,2]:
-            ref[1] += fontsize + height
-        if not pixels:
-            x,y = self.px2real(ref[0]+L,ref[1]+height)
-            ref = self.px2real(*ref)
-            L = x-ref[0]
-            height = y-ref[1]
-        ax.add_patch(matplotlib.patches.Rectangle(
-            ref, width=L, height=height, color=color))
-        if text:
-            r = funit(length, self.size['real']['unit'])
-            if r['unit'][0] == 'u':
-                r['unit'] = '$\\mu$' + r['unit'][1:]
-            ax.annotate("{value:.01f} {unit}".format(**r),
-                        (ref[0]+L/2, ref[1]), color=color,
-                        fontsize=fontsize, va="bottom", ha="center")
-
-    def offset(self, profiles, width=1, ax=None, col='w', inline=True, **kargs):
-        """
-        Correct an image by offsetting each row individually in order that the lines passed as argument in "profiles" becomes flat.
-
-        Parameters
-        ----------
-        profiles: list of list
-            each sublist represent a line as [x1, y1, x2, y2] in pixels known to be flat
-        width : int, float
-            the line width in pixels used for better statistics
-        ax : matplotlib axis or None
-            If not None, axis in which the profiles will be plotted in
-        inline : bool
-            If True perform the correction on the current object, otherwise return a new image
-        col : string
-            matrplotlib color used to plot the profiles (if ax is not None)
-        labels : bool
-            display a label number with each profile
-        **kargs: arguments passed further to get_row_profile.
-            axPixels: set to True if you axis "ax" have the data plotted in pixel instead of real distance
-
-        Example
-        -------
-        Exampel if the data are plotted in pixels:
-        >>> topo = pySPM.SPM_image(...)
-        >>> fig, ax = plt.subplots(1, 2, figsize=(10, 5))
-        >>> topoC = topo.offset([[150, 0, 220, 255]], inline=False,axPixels=True)
-        >>> topo.show(pixels=True, ax=ax[0])
-        >>> topoC.show(ax=ax[1]);
-
-        Example if the data are plotted with real units
-        >>> topo = pySPM.SPM_image(...)
-        >>> fig, ax = plt.subplots(1, 2, figsize=(10, 5))
-        >>> topoC = topo.offset([[150, 0, 220, 255]], inline=False)
-        >>> topo.show(ax=ax[0])
-        >>> topoC.show(ax=ax[1]);
-        """
-        offset = np.zeros(self.pixels.shape[0])
-        counts = np.zeros(self.pixels.shape[0])
-        for i, p in enumerate(profiles):
-            if kargs.get('labels', False):            
-                y, D = self.get_row_profile(*p, width=width, ax=ax, col=col, label=str(i), **kargs)
-            else:  
-                y, D = self.get_row_profile(*p, width=width, ax=ax, col=col, **kargs)
-            counts[y] += 1
-            offset[y[1:]] += np.diff(D)
-        counts[counts == 0] = 1
-        offset = offset/counts
-        offset = np.cumsum(offset)
-        offset = offset.reshape((self.pixels.shape[0], 1))
-        if inline:
-            self.pixels = self.pixels - \
-                np.flipud(np.repeat(offset, self.pixels.shape[1], axis=1))
-            return self
-        else:
-            C = copy.deepcopy(self)
-            C.pixels = self.pixels - \
-                np.flipud(np.repeat(offset, self.pixels.shape[1], axis=1))
-            return C
-            
-    def pxRect2Real(self, xy, width, height):
-        """
-        Transform a xy, width, height data in pixels to an equivalentz one with real units
-        """
-        ll = self.px2real(xy[0],xy[1])
-        ur = self.px2real(xy[0]+width,xy[1]+height)
-        return ll,ur[0]-ll[0],ur[1]-ll[1]
-    
-    def get_row_profile(self, x1, y1, x2, y2, width=1, col='C1', ax=None, alpha=0, **kargs):
-        """
-        Get a profile per row along a given line. This function is mainly useful for the function offset.
-        
-        x1, y1, x2, y2: int
-            coordinates of the line.
-        width : int
-            the width of the line used for statistics (in pixels)
-        col: string
-            color used to plot the line position
-        ax : matplotlib axis
-            axis in which the lines position will plotted
-        alpha : float
-            The alpha channel of the line color (≥0 and ≤1)
-        **kargs:
-            line style arguments: linewidth, color and linestyle
-            axis units: axPixels set to True if ax has the image plotted in pixels.
-            
-        Returns
-        -------
-        Y coordinates : 1D numpy array
-            distance along the profile starting at 0
-        Z coordinates : 1D numpy array
-            profile
-        """
-        plotargs = { key: kargs[key] for key in ['linewidth', 'color', 'linestyle'] if key in kargs }
-        if y2 < y1:
-            x1, y1, x2, y2 = x2, y2, x1, y1
-        if ax is not None:
-            d = np.sqrt((x2-x1)**2+(y2-y1)**2)
-            dx = -width/2*(y2-y1)/d
-            dy = width/2*(x2-x1)/d
-            if kargs.get('axPixels', False):
-                ax.plot([x1-dx, x1+dx], [y1-dy, y1+dy], col)
-                ax.plot([x2-dx, x2+dx], [y2-dy, y2+dy], col)
-                ax.plot((x1, x2), (y1, y2), col, **plotargs)
-                if kargs.get('label', False):
-                    ax.annotate(kargs.get('label'), (.5*(x1+x2),.5*(y1+y2)), color=col)
-                if alpha>0:
-                    import matplotlib.patches
-                    ax.add_patch(matplotlib.patches.Rectangle((x1+dx,y1+dy),width, d, -np.degrees(np.arctan2(x2-x1,y2-y1)), color=col, alpha=alpha))
-            else:
-                h = self.pixels.shape[0]
-                pxs = self.size['real']['x'] / self.pixels.shape[1]
-                pys = self.size['real']['y'] / h
-                ax.plot([(x1-dx)*pxs, (x1+dx)*pxs], [(h-(y1-dy))*pys, (h-(y1+dy))*pys], col)
-                ax.plot([(x2-dx)*pxs, (x2+dx)*pxs], [(h-(y2-dy))*pys, (h-(y2+dy))*pys], col)                
-                ax.plot((x1*pxs, x2*pxs), ((h-y1)*pys, (h-y2)*pys), col, **plotargs)
-                if kargs.get('label', False):
-                    ax.annotate(kargs.get('label'), (.5*(x1+x2)*pxs,.5*(2*h-y1-y2)*pys), color=col)
-                if alpha>0:
-                    import matplotlib.patches
-                    W = np.sqrt((2*dx*pxs)**2+(2*dy*pys)**2)
-                    L = np.sqrt(((x2-x1)*pxs)**2+((y2-y1)*pys)**2)
-                    ax.add_patch(matplotlib.patches.Rectangle(((x1+dx)*pxs,(y1+dy)*pys), W, L, -np.degrees(np.arctan2((x2-x1)*pxs,(y2-y1)*pys)), color=col, alpha=alpha))
-
-        x = np.arange(self.pixels.shape[1])
-        y = np.arange(self.pixels.shape[0])
-        I = scipy.interpolate.interp2d(x, y, np.flipud(self.pixels))
-
-        Y = np.arange(y1, y2+1)
-        V = np.zeros(len(Y))
-        for w in np.arange(width):
-            xl = np.linspace(x1-(width-1)/2.+w, x2-(width-1)/2.+w, len(Y))
-            for i in range(len(Y)):
-                Z = I(xl[i], Y[i])
-                V[i] += Z
-        return Y, V/width
-
-    def correct_median_diff(self, inline=True):
-        """
-        Correct the image with the median difference
-        """
-        N = self.pixels
-        # Difference of the pixel between two consecutive row
-        N2 = np.vstack([N[1:, :], N[-1:, :]])-N
-        # Take the median of the difference and cumsum them
-        C = np.cumsum(np.median(N2, axis=1))
-        # Extend the vector to a matrix (row copy)
-        D = np.tile(C, (N.shape[0], 1)).T
-        if inline:
-            self.pixels = N-D
-        else:
-            New = copy.deepcopy(self)
-            New.pixels = N-D
-            return New
-
-    def correct_slope(self, inline=True):
-        """
-        Correct the image by subtracting a fitted slope along the y-axis
-        """
-        s = np.mean(self.pixels, axis=1)
-        i = np.arange(len(s))
-        fit = np.polyfit(i, s, 1)
-        if inline:
-            self.pixels -= np.tile(np.polyval(fit, i).reshape(len(i), 1), len(i))
-            return self
-        else:
-            New = copy.deepcopy(self)
-            New.pixels -= np.tile(np.polyval(fit, i).reshape(len(i), 1), len(i))
-            return New
-
-    def correct_plane(self, inline=True, mask=None):
-        """
-        Correct the image by subtracting a fitted 2D-plane on the data
-
-        Parameters
-        ----------
-        inline : bool
-            If True the data of the current image will be updated otherwise a new image is created
-        mask : None or 2D numpy array
-            If not None define on which pixels the data should be taken.
-        """
-        x = np.arange(self.pixels.shape[1])
-        y = np.arange(self.pixels.shape[0])
-        X0, Y0 = np.meshgrid(x, y)
-        Z0 = self.pixels
-        if mask is not None:
-            X = X0[mask]
-            Y = Y0[mask]
-            Z = Z0[mask]
-        else:
-            X = X0
-            Y = Y0
-            Z = Z0
-        A = np.column_stack((np.ones(Z.ravel().size), X.ravel(), Y.ravel()))
-        c, resid, rank, sigma = np.linalg.lstsq(A, Z.ravel(), rcond=-1)
-        if inline:
-            self.pixels -= c[0] * \
-                np.ones(self.pixels.shape) + c[1] * X0 + c[2] * Y0
-            return self
-        else:
-            New = copy.deepcopy(self)
-            New.pixels -= c[0]*np.ones(self.pixels.shape) + c[1] * X0 + c[2] * Y0
-            return New
-
-    def correct_lines(self, inline=True):
-        """
-        Subtract the average of each line for the image.
-
-        if inline is True the current data are updated otherwise a new image with the corrected data is returned
-        """
-        if inline:
-            self.pixels -= np.tile(np.mean(self.pixels, axis=1).T, (self.pixels.shape[0], 1)).T
-            return self
-        else:
-            New = copy.deepcopy(self)
-            New.pixels -= np.tile(np.mean(self.pixels, axis=1).T, (self.pixels.shape[0], 1)).T
-            return New
-
-    def dist_v2(self, pixel=False):
-        """
-        Return a 2D array with the distance between each pixel and the closest border.
-        Might be usefull for FFT filtering
-        """
-        if pixel:
-            dx = 1
-            dy = 1
-        else:
-            dx = self.size['real']['x']/self.size['pixels']['x']
-            dy = self.size['real']['y']/self.size['pixels']['y']
-        x2 = np.arange(self.size['pixels']['x'])
-        x2 = (np.minimum(x2, self.size['pixels']['x']-x2) * dx)**2
-        y2 = np.arange(self.size['pixels']['y'])
-        y2 = (np.minimum(y2, self.size['pixels']['y'] - y2) * dy)**2
-        X, Y = np.meshgrid(x2, y2)
-        return np.sqrt(X+Y)
-    
-    def inv_calc_flat(self, d, l=0.1):
-        """
-        Function used for inverse MFM calculation (inspired from http://qmfm.empa.ch/qmfm/)
-        The function is in its early devlopment stage as not used by the developed.
-
-        Parameters
-        ----------
-        d : float
-            Height distance in the input data
-        l : float
-            Tikhonov parameter for the deconvolution
-        """
-        work_image = self.pixels
-        ny, nx = self.pixels.shape
-        dx = self.size['real']['x']/self.size['pixels']['x']
-        dy = self.size['real']['y']/self.size['pixels']['y']
-
-        k = self.dist_v2()
-        k[0, 0] = 1e-10
-
-        tf = np.exp(-d*k)
-        tf[0, 0] = np.mean(tf)
-        tf /= 2
-        tf *= 1-np.exp(-d * k)
-
-        recon_tf = np.ones(tf.shape) / (tf+l*np.ones(tf.shape) / np.conj(tf))
-        tf *= recon_tf
-        return np.real(np.fft.ifft2(np.fft.fft2(work_image)*recon_tf))
-
-    def get_extent(self):
-        """
-        Get the image extent in real data
-        """
-        W = self.size['recorded']['real']['x']
-        H = self.size['recorded']['real']['y']
-        return (0, W, 0, H)
-
-    def show(self, ax=None, sig=None, cmap=None, title=None,
-             adaptive=False, dmin=0, dmax=0, pixels=False, flip=False, wrap=None, mul=1, symmetric=False, **kargs):
-        """
-        Function to display the image with a lot of parametrization
-
-        Parameters
-        ----------
-        ax : matplotlib axis or None
-            matplotlib axis if given otherwise current axis will be used (plt.gca())
-        sig : float
-            sigma values to adjust the contrast range around the mean ±sig times the standard-deviation
-        cmap : string
-            colormap name used. By default a gray map is used. If the zscale of the data are in 'meter' (i.e. topography data) the 'hot' colormap is used
-        title : string
-            The title of the plot. By default is the channel name
-        adaptive : bool
-            The color scale used is linear. If adaptive is True a non linear color scale is used in order that each color is used with the same amount.
-        dmin : float
-            minimum value adjustment used for the colorscale
-        dmax: float
-            maximum value adjustment used for the colorscale
-        pixels : bool
-            Display the image with x/y-labels with real unit. If pixels is True, the axes are in pixels
-        flip : bool
-            Flip the image upside-down
-        wrap : Nont or int
-            wrap the title to a width of wrap chars
-        symmetric : bool
-            If True will place the middle of the colorscale to the value 0.
-            This is specially usefull for diverging colormaps such as : BrBG, bwr, coolwarm, seismiv, spectral, etc.
-        level : float
-            level should be ≥0 and <50. Adjust the lower and upper colorscale to level% and (100-level)% of the data range.
-            e.g. if level=1, the colorscale will display 1-99% of the data range
-        vmin : float
-            Minimum value used for the colorscale
-        vmax : flaot
-            Maximum value used for the colorscale
-
-
-        Returns
-        -------
-        matplotlib.image.AxesImage
-            matplolib axis instance returned by imshow
-
-        Examples
-        --------
-        >>> topo = pySPM.SPM_image(...)
-        >>> fig, (ax, ax2) = plt.subplots(2, 3, figsize=(15, 10))
-        >>> topo.show(ax=ax[0], cmap='gray', title="color map=\"gray\"")
-        >>> topo.show(ax=ax[1], sig=2, title="standard deviation=2")
-        >>> topo.show(ax=ax[2], adaptive=True, title="Adaptive colormap")
-        >>> topo.show(ax=ax2[0], dmin=4e-8, cmap='gray', title="raise the lowest value for the colormap of +40nm")
-        >>> topo.show(ax=ax2[1], dmin=3e-8, dmax=-3e-8, cmap='gray',title="raise lower of +30nm and highest of -30nm")
-        >>> topo.show(ax=ax2[2], pixels=True, title="Set axis value in pixels");
-        """
-        mpl.rc('axes', grid=False)
-        
-        if ax is None:
-            ax = plt.gca()
-        ax.src = self
-        if title == None:
-            title = u"{0} - {1}".format(self.type, self.channel)
-        if wrap is not None:
-            title = "\n".join([title[i*wrap:(i+1)*wrap]
-                               for i in range(int(len(title)/wrap)+1)])
-        unit = self.size['real']['unit']
-        sunit = 'afpnum kMGTPE'
-        if len(unit) == 1 or unit in ['pixels']:
-            isunit = 6
-        elif unit[0] in sunit:
-            isunit = sunit.find(unit[0])
-            unit = unit[1:]
-        else:
-            isunit = 6
-        W = self.size['real']['x']
-        H = self.size['real']['y']
-        fact = int(np.floor(np.log(W)/np.log(10)/3))
-        isunit += fact
-        W, H = W/10**(fact*3), H/10**(fact*3)
-        if cmap == None:
-            cmap = 'gray'
-            if unit == 'm' and self.channel == "Topography":
-                cmap = 'hot'
-        mi, ma = np.nanmin(self.pixels), np.nanmax(self.pixels)            
-        if adaptive:
-            img = np.asarray(256**2*(self.pixels-mi)/(ma-mi), dtype=np.uint16)
-            mi, ma = 0, 1
-            img = skimage.exposure.equalize_adapthist(img, clip_limit=0.03)
-        else:
-            img = mul*self.pixels
-            mi *= mul
-            ma *= mul
-        
-        if sig == None:
-            vmin = mi+dmin
-            vmax = ma+dmax
-        else:
-            std = np.nanstd(img)
-            avg = np.nanmean(img)
-            vmin = avg - sig * std
-            vmax = avg + sig * std
-        if 'level' in kargs:
-            if kargs['level'] < 0 or kargs['level']>=50:
-                raise ValueError("The level shoud have a value in [0,50)")
-            vmax = np.percentile(img, 100-kargs['level'])
-            vmin = np.percentile(img, kargs['level'])
-            del kargs['level']
-        if 'vmin' in kargs:
-            vmin = kargs['vmin']
-            del kargs['vmin']
-        if 'vmax' in kargs:
-            vmax = kargs['vmax']
-            del kargs['vmax']
-        if symmetric:
-            vmax = abs(max(vmin,vmax))
-            vmin = -vmax
-        if not flip:
-            ax.flipped = False
-            if pixels:
-                ax.isPixel = True
-                r = ax.imshow(np.flipud(img), extent=[0,img.shape[1],img.shape[0],0], cmap=cmap, vmin=vmin, vmax=vmax, **kargs)
-            else:
-                ax.isPixel = False
-                r = ax.imshow(np.flipud(img), extent=[0, W, 0, H], cmap=cmap, vmin=vmin, vmax=vmax, **kargs)
-        else:
-            ax.flipped = True
-            if pixels:
-                ax.isPixel = True
-                r = ax.imshow(np.flipud(img), extent=[0,img.shape[1],img.shape[0],0], cmap=cmap, vmin=vmin, vmax=vmax, **kargs)
-            else:
-                ax.isPixel = False
-                r = ax.imshow(np.flipud(img), cmap=cmap, extent=[0, W, 0, H], vmin=vmin, vmax=vmax, **kargs)
-        if pixels:
-            ax.set_xlim((0, self.pixels.shape[1]))
-            if flip:
-                ax.set_ylim((0, self.pixels.shape[0]))
-            else:
-                ax.set_ylim((self.pixels.shape[0], 0))
-        else:
-            ax.set_xlim((0,W))
-            if flip:
-                ax.set_ylim((H,0))
-            else:
-                ax.set_ylim((0,H))
-
-        if not pixels:
-            if isunit != 6:
-                u = sunit[isunit]
-                if u == 'u':
-                    u = '$\\mu$'
-                ax.set_xlabel(u'x [{0}{1}]'.format(u, unit))
-                ax.set_ylabel(u'y [{0}{1}]'.format(u, unit))
-            else:
-                ax.set_xlabel(u'x [{0}]'.format(unit))
-                ax.set_ylabel(u'y [{0}]'.format(unit))
-        if title != None:
-            ax.set_title(title)
-        return r
-        
-    def real2px(self, x, y):
-        """
-        Transform a real (x,y) value in pixels
-        Units should be the same as the one plotted by pySPM.SPM_image.show
-        """
-        return self.real2pixels(x,y)
-        
-    def real2pixels(self, x, y, float=False):
-        """
-        Transform a real (x,y) value in pixels
-        Units should be the same as the one plotted by pySPM.SPM_image.show
-        """
-        W = self.size['real']['x']
-        fact = int(np.floor(np.log(W)/np.log(10)/3))*3
-        if not float:
-            px = np.digitize(x, np.linspace(0,self.size['real']['x']/(10**fact),self.pixels.shape[1]), right=True)
-            py = np.digitize(y, np.linspace(0,self.size['real']['y']/(10**fact),self.pixels.shape[0]), right=False)
-        else:
-            px = x*(self.pixels.shape[1]-1)/(self.size['real']['x']/(10**fact))
-            py = y*(self.pixels.shape[0]-1)/(self.size['real']['y']/(10**fact))
-        return px, py
-        
-    def px2real(self, x, y):
-        """
-        Transform  a (x,y) value from pixels to real
-        Units are the same as the one plotted by pySPM.SPM_image.show
-        """
-        W = self.size['real']['x']
-        fact = int(np.floor(np.log(W)/np.log(10)/3))*3
-        rx = x*self.size['real']['x']/(10**fact)/self.pixels.shape[1]
-        ry = (self.pixels.shape[0]-y)*self.size['real']['y']/(10**fact)/self.pixels.shape[0]
-        return rx, ry
-    
-    def circular_profile(self, x0, y0, Ra=1, Rn=0, width=1, N=20, A=0, B=360,\
-        cmap='jet', axImg=None, axPolar=None, axProfile=None, plotProfileEvery=1,\
-        xtransf=lambda x: x*1e9, ytransf=lambda x:x*1e9,\
-        ToFcorr=False, fit=lambda x, *p: p[3]+p[2]*CDF(x, *p[:2]), p0=None, errors=False, bounds=(-np.inf, np.inf), fakefit=False, **kargs):
-        """
-        Create radial profiles from point x0,y0 with length Ra (outer radius) and Rn (negative Radius).
-        Start from angle A° to angle B° with N profiles.
-        If you want to apply the ToF-correction, please set ToFcorr to the number of scans used to record the ToF-SIMS image.
-        Return the fitting uncertainty on sigma if errors is set to True
-        The fitting function can be adjusted by fit and the default parameters by p0 which is an array of function where the first parameter passed will be the x-values and the second the y-values.
-        """
-        from matplotlib import colors, cm
-        
-        # Create a colormap for each profile
-        CM =  plt.get_cmap(cmap) 
-        cNorm  = colors.Normalize(vmin=0, vmax=N)
-        scalarMap = cm.ScalarMappable(norm=cNorm, cmap=CM)
-        res = []
-        cov = []
-        angles = []
-        assert A<B        
-        for i, angle in enumerate(np.linspace(A, B, N)):
-            a = np.radians(angle)
-            angles.append(a)
-            l, p = self.get_profile(
-                x0-Rn*np.cos(a),
-                y0+Rn*np.sin(a),
-                x0+Ra*np.cos(a),
-                y0-Ra*np.sin(a),
-                ax=axImg, width=width, color=scalarMap.to_rgba(i), **kargs)
-            if width==0:
-                profile = p
-            else:
-                profile = np.mean(p, axis=1)
-            if ToFcorr:
-                profile = -np.log(1.001-profile/ToFcorr)
-            if p0 is None:
-                AC = np.mean(profile[:len(l)//2])
-                AE = np.mean(profile[len(l)//2:])
-                if AC<AE:
-                    p0 = [l[len(l)//2], 5*(l[1]-l[0]), np.max(profile)-np.min(profile), np.min(profile) ]
-                else:
-                    p0 = [l[len(l)//2], 5*(l[1]-l[0]), -np.max(profile)+np.min(profile), np.max(profile) ]
-            else:
-                for j,p in enumerate(p0):
-                    if callable(p):
-                        p0[j] = p(l,profile)
-            if kargs.get('debug',False):
-                print("calculate fit parameters are", p0)
-            if not fakefit:
-                p0, pcov = scipy.optimize.curve_fit(fit, l , profile, p0)
-            else:
-                pcov = np.zeros((len(p0),len(p0)))
-            res.append(p0)
-            cov.append([np.sqrt(abs(pcov[i,i])) for i in range(len(p0))])
-            if axProfile and i%plotProfileEvery == 0:
-                axProfile.plot(xtransf(l-p0[0]), profile, color=scalarMap.to_rgba(i), linestyle=':')
-                axProfile.plot(xtransf(l-p0[0]), fit(l,*p0), color=scalarMap.to_rgba(i))
-        # close loop
-        if A%360 == B%360:
-            angles.append(angles[0])
-            res.append(res[0])
-            cov.append(cov[0])
-        
-        # Plot polar
-        angles = np.array(angles)
-        res = np.array(res)
-        cov = np.array(cov)
-        fact = 2*np.sqrt(2*np.log(2))
-        if axPolar:
-            axPolar.plot(angles, ytransf(res[:,1]), color=kargs.get('sig_color','C0'), label="$\\sigma$")
-            axPolar.plot(angles, ytransf(fact*res[:,1]), color=kargs.get('fwhm_color','C1'), label="FWHM")
-            if errors:
-                axPolar.fill_between(angles, ytransf(res[:,1]-cov[:,1]),ytransf(res[:,1]+cov[:,1]), color=kargs.get('sig_color','C0'), alpha=kargs.get('fillalpha',.5))
-                axPolar.fill_between(angles, fact*ytransf(res[:, 1]-cov[:, 1]), ytransf(res[:, 1]+cov[:, 1]), color=kargs.get('fwhm_color', 'C1'), alpha=kargs.get('fillalpha',.5))
-            
-        return angles, res, cov
-        
-    def get_profile(self, x1, y1, x2, y2, width=0, ax=None, pixels=True, color='w', axPixels=None, **kargs):
-        """
-        retrieve the profile of the image between pixel x1,y1 and x2,y2
-
-        Parameters
-        ----------
-        x1, y1, x2, y2 : ints
-            coordinates for the profile
-        ax : matplotlib axis
-            defines the matplotlib axis on which the position of the profile should be drawn (in not None)
-        width : int
-            the width of the profile (for averaging/statistics) in pixels
-        color : string
-            color used to plot the profiles lines
-        axPixels : bool
-            If True the image plotted in the ax axis is displayed in pixels
-        
-        Returns
-        -------
-        x data : 1D numpy array
-        profile : 1D numpy array
-        """
-        if kargs.get('debug',False):
-            print("get_profile input coordinates:", x1, y1, x2, y2)
-        if ax is not None and axPixels is None:
-            if hasattr(ax, 'isPixel'):
-                axPixels = ax.isPixel
-        if axPixels is None:
-            axPixels = pixels
-        W = self.size['real']['x']
-        fact = int(np.floor(np.log(W)/np.log(10)/3))*3
-        if not pixels:
-            if kargs.get('debug', False):
-                print("Image range (real scale):", self.size['real']['x']/(10**fact), self.size['real']['y']/(10**fact))
-            x1, y1 = self.real2pixels(x1, y1, float=True)
-            x2, y2 = self.real2pixels(x2, y2, float=True)
-            y1 = self.pixels.shape[0]-y1
-            y2 = self.pixels.shape[0]-y2
-            if kargs.get('debug', False):
-                print("Pixel coordinates:", x1, y1, x2, y2)
-            if not axPixels:
-                xvalues, p = get_profile(np.flipud(self.pixels), x1, y1, x2, y2, ax=ax, width=width, color=color,\
-                    transx = lambda x: x*(self.size['real']['x']/(10**fact))/self.pixels.shape[1],\
-                    transy = lambda x: (self.pixels.shape[0]-x)*(self.size['real']['y']/(10**fact))/self.pixels.shape[0],\
-                    **kargs)
-            else:
-                values, p = get_profile(np.flipud(self.pixels), x1, y1, x2, y2, ax=ax, width=width, color=color, **kargs)
-        else:
-            if axPixels:
-                values, p = get_profile(np.flipud(self.pixels), x1, y1, x2, y2, ax=ax, width=width, color=color, **kargs)
-            else:
-                values, p = get_profile(np.flipud(self.pixels), x1, y1, x2, y2, ax=ax, width=width, color=color,\
-                    transx = lambda x: x*(self.size['real']['x']/(10**fact))/self.pixels.shape[1],\
-                    transy = lambda x: (self.pixels.shape[0]-x)*(self.size['real']['y']/(10**fact))/self.pixels.shape[0],\
-                    **kargs)
-
-        dx = (x2-x1)*self.size['real']['x']/self.size['pixels']['x']
-        dy = (y2-y1)*self.size['real']['y']/self.size['pixels']['y']
-        rd = np.sqrt(dx**2+dy**2)
-        xvalues = np.linspace(0, rd, len(p))
-        return xvalues, p
-
-    def plot_profile(self, x1, y1, x2, y2, width=0, ax=None, pixels=True, img=None, imgColor='w', ztransf=lambda x: x, zunit=None, **kargs):
-        """
-        Retrieve and plot a profile from an image
-
-        Parameters
-        ----------
-        x1, y1, x2, y2 : int
-            coordinate of the profile in real size or in pixels (if pixels is True)
-        width : float
-            the width of the profiles in pixels for better statistics
-        ax : matplotlib axis
-            The axis in which the profile will be plotted
-        pixels : bool
-            If True the coordinates are given in pixels and not in real units
-        img : matplotlib axis
-            The axis in which the profile position will be drawn
-        imgColor : string
-            The color used to display the profile positions
-        ztransf : function
-            function to transform the profile data. This can be used to scale the data.
-            Most profiles are retrieved in 'm' and a 'nm' value can be used by using ztransf=lambda x: x*1e9
-        zunit : string
-            the zunit name used if ztransft is used
-        color : string
-            The color of the profile
-        col : string
-            can be used instead of color
-        stdplot : bool
-            If True display the ±nσ plots where n is given by the sig parameter
-        sig : int
-            The number of sigmas used in stdplot
-        label : string
-            The label used for plotting the profile (useful if you perform a ax.legend() afterwards)
-
-        Returns
-        -------
-        dictionary : {'plot': matplotlib_plot_instance, 'l': profile_xaxis, 'z': profile_yaxis}
-
-        Examples
-        --------
-        >>> topo = pySPM.SPM_image(...)
-        >>> fig, ax = plt.subplots(1, 2, figsize=(10, 5))
-        >>> topo.plot_profile(70, 100, 170, 200, ax=ax[1], img=ax[0], ztransf=lambda x:x*1e9, zunit='nm');
-        >>> topo.show(ax=ax[0], pixels=True);
-        """
-        col = kargs.get('color',kargs.get('col','C0'))
-        W = self.size['real']['x']
-        fact = int(np.floor(np.log(W)/np.log(10)/3))*3
-        if ax == None:
-            ax = plt.gca()
-        xvalues, p = self.get_profile(x1, y1, x2, y2, width=width, color=imgColor, ax=img, pixels=pixels, **kargs)
-        d = np.sqrt((x2-x1)**2+(y2-y1)**2)
-        dx = (x2-x1)
-        dy = (y2-y1)
-        if pixels:
-            rd = d
-            u = ''
-            unit = 'px'
-        else:
-            unit = self.size['real']['unit']
-            sunit = 'afpnum kMGTPE'
-            if len(unit) == 1:
-                isunit = 6
-            elif unit[0] in sunit:
-                isunit = sunit.find(unit[0])
-                unit = unit[1:]
-            else:
-                isunit = 6
-            isunit += fact//3
-            if isunit != 6:
-                u = sunit[isunit]
-            else:
-                u=''
-            if u == 'u':
-                u = '$\\mu$'
-            rd = np.sqrt(dx**2+dy**2)
-        xvalues = np.linspace(0, rd, len(p))
-        lab = kargs.get("label", "")
-        if width < 2:
-            profile = ztransf(p)
-        else:
-            profile = ztransf(np.mean(p, axis=1))
-            s = np.std(p)
-            if kargs.get('stdplot', False):
-                for ns in range(1, kargs.get('sig', 2)+1):
-                    ax.fill_between(xvalues, profile-ns*s, profile+ns*s, color=col, alpha=.2, label=[lab+' ($\\sigma,\ldots {}\\sigma$)'.format(kargs.get('sig',2)),None][ns>1])
-        
-        Plot = ax.plot(xvalues, profile, color=col, linewidth=kargs.get('linewidth',1),linestyle=kargs.get('linestyle','-'), label=lab+[' (mean)',''][width<2])
-        if kargs.get('min',False):
-            minStyle = kargs.get('minStyle', kargs.get('minmaxStyle', '--'))
-            minColor = kargs.get('minColor', kargs.get('minmaxColor', col))
-            minMarker = kargs.get('minMarker', kargs.get('minmaxMarker', ''))
-            ax.plot(xvalues, np.min(p, axis=1), color=minColor, linewidth=kargs.get('linewidth',1),linestyle=minStyle, marker=minMarker, label=lab+' (min)')
-        if kargs.get('max', False):
-            maxStyle = kargs.get('maxStyle',kargs.get('minmaxStyle','--'))
-            maxColor = kargs.get('maxColor',kargs.get('minmaxColor',col))
-            maxMarker = kargs.get('maxMarker',kargs.get('minmaxMarker',''))
-            ax.plot(xvalues, np.max(p, axis=1), color=maxColor, linestyle=maxStyle, linewidth=kargs.get('linewidth',1), marker=maxMarker, label=lab+' (max)')
-            
-        ax.set_xlabel("Distance [{1}{0}]".format(unit, u))
-        if zunit is not None:
-            ax.set_ylabel("{1} [{0}]".format(zunit, self.channel))
-        else:
-            ax.set_ylabel("{1} [{0}]".format(self.zscale, self.channel))
-       
-        return {'plot': Plot, 'l': xvalues, 'z': profile}
-
-    def get_bin_threshold(self, percent, high=True, adaptive=False, binary=True, img=False):
-        """
-        Threshold the image into binary values
-        
-        Parameters
-        ----------
-        percent : float
-            The percentage where the thresholding is made
-        high : bool
-            If high a value of 1 is returned for values > percent
-        adaptive : bool
-            If True, performs an adaptive thresholding (see skimage.filters.threshold_adaptive)
-        binary : bool
-            If True return bool data (True/False) otherwise  numeric (0/1)
-        img : bool
-            If True return a SPM_image otherwise a numpy array
-        """
-        if adaptive:
-            if binary:
-                return self.pixels > threshold_local(self.pixels, percent)
-            return threshold_local(self.pixels, percent)
-        mi = np.min(self.pixels)
-        norm = (self.pixels-mi)/(np.max(self.pixels)-mi)
-        if high:
-            r = norm > percent
-        else:
-            r = norm < percent
-        if not img:
-            if binary:
-                return r
-            return np.ones(self.pixels.shape)*r
-        else:
-            I = copy.deepcopy(self)
-            I.channel = "Threshold from "+I.channel
-            if binary:
-                I.pixels = r
-            else:
-                I.pixels = np.ones(self.pixels.shape)*r
-            return I
-
-    def spline_offset(self, X, Y, Z=None, inline=True, ax=None, output='img', **kargs):
-        """
-        subtract a spline interpolated by points corrdinates.
-        if Z is None, the image values will be used (default)
-        """
-        if ax is not None:
-            if 'num' in kargs and kargs['num']:
-                text_color = 'k'
-                if 'text_color' in kargs:
-                    text_color = kargs['text_color']
-                    del kargs['text_color']
-                for i in range(len(X)):
-                    l = self.pixels.shape[1]-X[i] < 20
-                    ax.annotate(str(i), (X[i], Y[i]), ([
-                                5, -5][l], 0), textcoords='offset pixels', va="center", ha=["left", "right"][l], color=text_color)
-                del kargs['num']
-            ax.plot(X, Y, 'o', **kargs)
-        import scipy.interpolate
-        T = np.flipud(self.pixels) - np.min(self.pixels)
-        if Z is None:
-            Z = [T[Y[i], X[i]] for i in range(len(X))]
-        x = np.arange(self.pixels.shape[1])
-        y = np.arange(self.pixels.shape[0])
-        xx, yy = np.meshgrid(x, y)
-        I = scipy.interpolate.SmoothBivariateSpline(X, Y, Z)
-        z = I.ev(xx, yy)
-        if inline:
-            self.pixels -= z
-            return z
-        else:
-            if output == 'img':
-                New = copy.deepcopy(self)
-                New.pixels -= z
-                return New
-            elif output == 'spline':
-                return z
-            else:
-                raise ValueError(
-                    "The output parameter should be either 'img' or 'spline'")
-
-    def get_shadow_mask(self, angle, BIN=None, pb=False):
-        """
-        If an image is recorded with a beam incident with a certain angle, the topography will shadow the data.
-        This function generates the shadow mask for a given topography and a given incident angle.
-
-        Parameters
-        ----------
-        angle : float
-            The incidence angle in degrees
-        BIN : numpy array
-            Data. If given will move the recorded pixels at the correct x,y positions
-        pb : bool
-            display a progressbar ?
-
-        Note
-        ----
-        This function is old, might not be optimized or working properly
-        """
-        if BIN is not None:
-            BIN = BIN*1.0
-        slope = np.tan(np.radians(angle))
-        neg = False
-        if slope < 0:
-            neg = True
-            slope = -slope
-            topo = np.fliplr(self.pixels)
-            if BIN is not None:
-                BIN = np.fliplr(BIN)
-        else:
-            topo = self.pixels
-        x = np.linspace(0, self.size['real']['x'], self.pixels.shape[1])
-        if self.size['real']['unit'] == 'um':
-            x *= 1e-6
-        elif self.size['real']['unit'] == 'nm':
-            x *= 1e-9
-        mask = np.zeros(self.pixels.shape)
-        AFM_bin_shadow = np.zeros(self.pixels.shape)
-        Y = range(self.pixels.shape[0])
-        if pb:
-            Y = tqdm(Y)
-        for yi in Y:
-            for xi in range(self.pixels.shape[1]):
-                cut = self.pixels.shape[1]-2
-                y_ray = slope*(x-x[xi]) + topo[yi, xi]
-                while cut > xi and y_ray[cut] > topo[yi, cut]:
-                    cut -= 1
-                if xi == cut:
-                    if BIN is not None:
-                        AFM_bin_shadow[yi, xi] = BIN[yi, xi]
-                    continue
-                # Cut has been found
-                if BIN is not None:
-                    x1 = x[cut]
-                    x2 = x[cut+1]
-                    y1 = topo[yi, cut]
-                    y2 = topo[yi, cut+1]
-                    x0 = x[xi]
-                    y0 = topo[yi, xi]
-                    if y2 == y1:
-                        x_cut = (y1+slope*x0-y0)/slope
-                        y_cut = y1
-                    else:
-                        numerator = x1/(x2-x1)+(y0-slope*x0-y1)/(y2-y1)
-                        denominator = 1/(x2-x1)-slope/(y2-y1)
-                        x_cut = numerator / denominator
-                        y_cut = slope*(x_cut-x0)+y0
-                    if x_cut >= x1 and x_cut <= x2:
-                        y1 = BIN[yi, cut]
-                        y2 = BIN[yi, cut+1]
-                        yint = (((y2-y1)/(x2-x1))*(x_cut-x1))+y1
-                    else:
-                        yint = BIN[yi, xi]
-                    AFM_bin_shadow[yi, xi] = yint
-                mask[yi, xi] = 1
-        if neg:
-            mask = np.fliplr(mask)
-            AFM_bin_shadow = np.fliplr(AFM_bin_shadow)
-        if BIN is not None:
-            return (mask, AFM_bin_shadow)
-        return mask
-
-    def adjust_position(self, fixed):
-        """
-        Shift the current pixels to match a fixed image.
-        The shift is determined by position where the cross-correlation is maximized.
-        """
-        adj = copy.deepcopy(self)
-        cor = np.fft.fft2(fixed.pixels)
-        cor = np.abs(np.fft.ifft2(np.conj(cor) * np.fft.fft2(self.pixels)))
-        cor = cor / fixed.pixels.size
-        ypeak, xpeak = np.unravel_index(cor.argmax(), cor.shape)
-        shift = [-(ypeak-1), -(xpeak-1)]
-        adj.pixels = np.roll(self.pixels, shift[0], axis=0)
-        adj.pixels = np.roll(adj.pixels, shift[1], axis=1)
-        return adj
-
-    def align(self, tform, cut=True):
-        """
-        Apply an Affine transform on the data
-
-        Parameters
-        ----------
-        tform : skimage.transform
-            the affine transform to perform
-        cut : bool
-            If True cut the data
-        """
-        New = copy.deepcopy(self)
-        New.pixels = tf.warp(self.pixels, tform, preserve_range=True)
-        if not cut:
-            return New
-        cut = [0, 0] + list(self.pixels.shape)
-        if tform.translation[0] >= 0:
-            cut[2] -= tform.translation[0]
-        elif tform.translation[0] < 0:
-            cut[0] -= tform.translation[0]
-        if tform.translation[1] >= 0:
-            cut[1] += tform.translation[1]
-        elif tform.translation[1] < 0:
-            cut[3] += tform.translation[1]
-        cut = [int(x) for x in cut]
-        New.cut(cut, inplace=True)
-        return New, cut
-
-    def get_fft(self):
-        """
-        return the FFT2 transform opf the image
-        """
-        return np.fft.fftshift(np.fft.fft2(self.pixels))
-
-    def corr_fit2d(self, nx=2, ny=1, poly=False, inline=True, mask=None):
-        """
-        Subtract a fitted 2D-polynom of nx and ny order from the data
-
-        Parameters
-        ----------
-        nx : int
-            the polynom order for the x-axis
-        ny : int
-            the polynom order for the y-axis
-        poly : bool
-            if True the polynom is returned as output
-        inline : bool
-            create a new object?
-        mask : 2D numpy array
-            mask where the fitting should be performed
-        """
-        r, z = fit2d(self.pixels, nx, ny, mask=mask)
-        if inline:
-            self.pixels -= z
-        else:
-            N = copy.deepcopy(self)
-            N.pixels -= z
-            if poly:
-                return N, z
-            return N
-        if poly:
-            return z
-        return self
-
-    def zero_min(self, inline=True):
-        """
-        Shift the values so that the minimum becomes zero.
-        """
-        if inline:
-            self.pixels -= np.min(self.pixels)
-            return self
-        else:
-            N = copy.deepcopy(self)
-            N.pixels -= np.min(N.pixels)
-            return N
-
-    def filter_lowpass(self, p, inline=True):
-        """
-        Execute a lowpass filter on the data
-        """
-        F = self.get_fft()
-        mask = self.getRmask() < p
-        if inline:
-            self.pixels = np.real(np.fft.ifft2(np.fft.fftshift(F*mask)))
-        else:
-            C = copy.deepcopy(self)
-            C.pixels = np.real(np.fft.ifft2(np.fft.fftshift(F*mask)))
-            return C
-
-    def _resize_infos(self):
-        """
-        Internal to recalculate the real size when the image is cropped or cut
-        """
-        self.size['real']['x'] *= self.pixels.shape[1]/self.size['pixels']['x']
-        self.size['real']['y'] *= self.pixels.shape[0]/self.size['pixels']['y']
-        self.size['pixels']['x'] = int(self.pixels.shape[1])
-        self.size['pixels']['y'] = int(self.pixels.shape[0])
-        if 'recorded' in self.size:
-            self.size['recorded']['real']['x'] \
-                *= (self.pixels.shape[1]/self.size['pixels']['x'])
-            self.size['recorded']['real']['y'] \
-                *= (self.pixels.shape[0]/self.size['pixels']['y'])
-            self.size['recorded']['pixels']['x'] = int(self.pixels.shape[1])
-            self.size['recorded']['pixels']['y'] = int(self.pixels.shape[0])
-        
-    def filter_scars_removal(self, thresh=.5, inline=True):
-        """
-        Filter function to remove scars from images.
-        """
-        if not inline:
-            C = copy.deepcopy(self)
-        else:
-            C = self
-        for y in range(1, self.pixels.shape[0]-1):
-            b = self.pixels[y-1, :]
-            c = self.pixels[y, :]
-            a = self.pixels[y+1, :]
-            mask = np.abs(b-a) < thresh*(np.abs(c-a))
-            C.pixels[y, mask] = b[mask]
-        if not inline:
-            return C
-        return self
-
-    def cut(self, c, inline=False, pixels=True, **kargs):
-        """
-        Clip/Crop the image
-
-        Parameters
-        ----------
-        c : list [llx,lly,urx,ury]
-            list of the lowe-left (ll) and upper-right (ur) coordinates
-        inline: bool
-            perform the transformation inline or produce a new SPM_image?
-        pixels : bool
-            Are the coordinates given in pixels?
-
-        Returns
-        -------
-        self if inplace, clipped SPM_image otherwises2 = pySPM.Nanoscan("%s/CyI5b_PCB_ns.xml"%(Path))
-        """
-        if 'inplace' in kargs:
-            inline=kargs['inplace']
-        if kargs.get('debug',False):
-            print("cut) Input coordinates:", c)
-        if not pixels:
-            c = [z for s in zip(*self.real2pixels(c[0::2], c[1::2])) for z in s]
-            if kargs.get('debug',False):
-                print("cut) pixel coordinates:", c)
-        if not inline:
-            new = copy.deepcopy(self)
-            new.pixels = cut(self.pixels, c, **kargs)
-            new._resize_infos()
-            return new
-        else:
-            self.pixels = cut(self.pixels, c, **kargs)
-            self._resize_infos()
-            return self
-    
-    def zoom(self, zoom_factor, inplace=False, order=3):
-        """
-        Resize the image to a new pixel size (but keep the real size) by pixel interpolation.
-
-        Parameters
-        ----------
-        zoom_factor : float
-            > 1: up sampling
-            < 1: down sampling
-        order : int
-            The spline interpolation order to use. (default: 3). Use 0 for binary or very sharp images.
-        inplace : bool
-            create a new image?
-        """
-        from scipy.ndimage.interpolation import zoom
-        if not inplace:        
-            new = copy.deepcopy(self)
-            new.pixels = zoom(new.pixels, zoom_factor, order=order)
-            new.size['pixels']['x'] = new.pixels.shape[1]
-            new.size['pixels']['y'] = new.pixels.shape[0]
-            return new
-        else:
-            self.pixels = zoom(self.pixels, zoom_factor, order=order)
-            self.size['pixels']['x'] = self.pixels.shape[1]
-            self.size['pixels']['y'] = self.pixels.shape[0]
-            return self
-
-# Note: The following functions are not part of the SPM_image class.
-# All following functions are performed on numpy arrays
-
-def cut(img, c, **kargs):
-    """
-    Clip / Crop a numpy array
-
-    Parameters
-    ----------
-    img : 2D numpy array
-        The input image array
-    c : list [llx, lly, urx, ury]
-        the lower-left (ll) and upper-right (ur) coordinates used for the clippings2 = pySPM.Nanoscan("%s/CyI5b_PCB_ns.xml"%(Path))
-    """
-    if kargs.get('debug',False):
-        print("cut in x", c[0], "->", c[2], " - in y", c[1], "->", c[3])
-    if c[3] < c[1]:
-        c = [c[0],c[3],c[2],c[1]]
-    if c[2] < c[0]:
-        c = [c[2],c[1],c[0],c[3]]
-    if c[2]-c[0] == img.shape[1] and c[3]-c[1] == img.shape[0]:
-        raise Exception("Reshaping the same array again?")
-    return img[c[1]:c[3], c[0]:c[2]]
-
-
-def normalize(data, sig=None, vmin=None, vmax=None):
-    """
-    Normalize the input data. Minimum_value -> 0 and maximum_value -> 1
-
-    Parameters
-    ----------
-    data : numpy array
-        input data
-    sig : float or None
-        if not None:
-            mean(data)-sig*standard_deviation(data) -> 0
-            mean(data)+sig*standard_deviation(data) -> 1
-    vmin : float or None
-        if not None, define the lower bound i.e.  vmin -> 0
-    vmax : float or None
-        if not None, defines the upper bound i.e. vmax -> 0
-
-    Note
-    ----
-    All values below the lower bound will be = 0
-    and all values above the upper bound will be = 1
-
-
-    """
-    if sig is None:
-        mi = np.min(data)
-        ma = np.max(data)
-    else:
-        s = sig*np.std(data)
-        mi = np.mean(data)-s
-        ma = np.mean(data)+s
-    if vmin is not None:
-        mi = vmin
-    if vmax is not None:
-        ma = vmax
-    N = (data-mi)/(ma-mi)
-    N[N < 0] = 0
-    N[N > 1] = 1
-    return N
-
-
-def imshow_sig(img, sig=1, ax=None, **kargs):
-    """
-    Shortcut to plot a numpy array around it's mean with bounds ±sig sigmas
-
-    Parameters
-    ----------
-    img : 2D numpy array
-        input image to display
-    sig : float
-        The number of standard-deviation to plot
-    ax : matplotlib axis
-        matplotlib axis to use. If None, the current axis (plt.gca() will be used).
-    **kargs : additional parameters
-        will be passed to the imshow function of matplotls2 = pySPM.Nanoscan("%s/CyI5b_PCB_ns.xml"%(Path))ib
-    """
-    if ax == None:
-        fig, ax = plt.subplots(1, 1)
-    std = np.std(img)
-    avg = np.mean(img)
-    vmin = avg - sig * std
-    vmax = avg + sig * std
-    ax.imshow(img, vmin=vmin, vmax=vmax, **kargs)
-
-
-def adjust_position(fixed, to_adjust, shift=False):
-    """ Shift the current pixels to match a fixed image by rolling the data"""
-    adj = copy.deepcopy(to_adjust)
-    cor = np.fft.fft2(fixed)
-    cor = np.abs(np.fft.ifft2(np.conj(cor) * np.fft.fft2(to_adjust)))
-    cor = cor / to_adjust.size
-    ypeak, xpeak = np.unravel_index(cor.argmax(), cor.shape)
-    shift = [-(ypeak-1), -(xpeak-1)]
-    adj = np.roll(to_adjust, shift[0], axis=0)
-    adj = np.roll(adj, shift[1], axis=1)
-    if shift:
-        return adj, shift
-    return adj
-
-
-def tukeyfy(A, alpha, type='default'):
-    """
-    Apply a Tukey window on the current image
-
-    Parameters
-    ----------
-    A : 2D numpy array
-        input array
-    alpha : float
-        Size of the Tukey windows in percent of the image (≥0 and ≤1)
-    type : string
-        if not "default" perform a mean centering (data will blend down to its mean instead of 0)
-    """
-    tuky = tukeywin(A.shape[0], alpha)
-    tukx = tukeywin(A.shape[1], alpha)
-    tuk = np.multiply(tukx[:, None].T, tuky[:, None])
-    if type is 'default':
-        return A * tuk
-    avg = np.mean(A)
-    return avg+(A-avg) * tuk
-
-
-def tukeywin(window_length, alpha=0.5):
-    '''The Tukey window, also known as the tapered cosine window, can be regarded as a cosine lobe of width \alpha * N / 2
-    that is convolved with a rectangle window of width (1 - \alpha / 2). At \alpha = 1 it becomes rectangular, and
-    at \alpha = 0 it becomes a Hann window.
-
-    We use the same reference as MATLAB to provide the same results in case users compare a MATLAB output to this function
-    output
-
-    Reference
-    ---------
-    http://www.mathworks.com/access/helpdesk/help/toolbox/signal/tukeywin.html
-
-    '''
-    # Special cases
-    if alpha <= 0:
-        return np.ones(window_length)  # rectangular window
-    elif alpha >= 1:
-        return np.hanning(window_length)
-
-    # Normal case
-    x = np.linspace(0, 1, window_length)
-    w = np.ones(x.shape)
-
-    # first condition 0 <= x < alpha/2
-    first_condition = x < alpha/2
-    w[first_condition] = 0.5 * \
-        (1 + np.cos(2*np.pi/alpha * (x[first_condition] - alpha/2)))
-
-    # second condition already taken care of
-
-    # third condition 1 - alpha / 2 <= x <= 1
-    third_condition = x >= (1 - alpha/2)
-    w[third_condition] = 0.5 * \
-        (1 + np.cos(2*np.pi/alpha * (x[third_condition] - 1 + alpha/2)))
-    return w
-
-
-def overlay(ax, mask, color, **kargs):
-    """
-    Plot an overlay on an existing axis
-
-    Parameters
-    ----------
-    ax : matplotlib axis
-        input axis
-    mask : 2D numpy array
-        Binary array where a mask should be plotted
-    color : string
-        The color of the mask to  plot
-    **kargs: additional parameters
-        passed to the imshow function of matploltib
-    """
-    m = ma.masked_array(mask, ~mask)
-    col = np.array(colors.colorConverter.to_rgba(color))
-    I = col[:, None, None].T*m[:, :, None]
-    ax.imshow(I, **kargs)
-
-
-def normP(x, p, trunk=True):
-    """
-    Normalize the input data accroding to its percentile value.
-
-    Parameters
-    ----------
-    x : 2D numpy array
-        input data
-    p : float
-        percentile to normalize the data.
-        lower bound = p percentile
-        upper bound = (100-p) percentile
-    trunk : bool
-        If True the data are truncated between 0 and 1
-    """
-    thresh_high = np.percentile(x, 100-p)
-    thresh_low = np.percentile(x, p)
-    if thresh_low == thresh_high:
-        thresh_high = np.max(x)
-        thresh_low = np.min(x)
-    if thresh_low == thresh_high:
-        thresh_high = thresh_low+1
-    r = (x-thresh_low)/(thresh_high-thresh_low)
-    if trunk:
-        r[r < 0] = 0
-        r[r > 1] = 1
-    return r
-
-def beam_profile(target, source, mu=1e-6, tukey=0, meanCorr=False, source_tukey=None, real=np.abs, **kargs):
-    """
-    Calculate the PSF by deconvolution of the target
-    with the source using a Tikhonov regularization of factor mu.
-    """
-    if source_tukey is None:
-        source_tukey = tukey
-    if kargs.get('source_centering', False):
-        source = 2*source-1
-    if meanCorr:
-        target = target-np.mean(target)
-    if tukey>0:
-        target = tukeyfy(target, tukey)
-    if source_tukey>0:
-        source = tukeyfy(source, tukey)
-    tf = np.fft.fft2(source)
-    tf /= np.size(tf)
-    recon_tf = np.conj(tf) / (np.abs(tf)**2 + mu)
-    return np.fft.fftshift(real(np.fft.ifft2(np.fft.fft2(target) * recon_tf)))/np.size(target)
-
-
-def beam_profile1d(target, source, mu=1e-6, real=np.abs):
-    source = source
-    tf = np.fft.fft(source)
-    tf /= np.size(tf)
-    recon_tf = np.conj(tf) / (np.abs(tf)**2 + mu)
-    F = np.fft.fft(target) * recon_tf
-    return np.fft.fftshift(real(np.fft.ifft(F))), F
-
-
-def zoom_center(img, sx, sy=None):
-    """
-    Zoom by taking the sx × sy central pixels
-
-    Parameters
-    ----------
-    img : 2D numpy array
-        The input data
-    sx : int
-        The number of pixels along the x-axis to take
-
-    sy : int or None
-        The number of pixels alongs the y-axis to take.
-        If None take the same value as for sx
-    """
-    if sy is None:
-        sy = sx
-    assert type(sx) is int
-    assert type(sy) is int
-    return img[
-        img.shape[0]//2-sy//2: img.shape[0]//2 + sy//2,
-        img.shape[1]//2-sx//2: img.shape[1]//2 + sx//2]
-
-def px2real(x, y, size, ext):
-    rx = ext[0]+(x/size[1])*(ext[1]-ext[0])
-    ry = ext[2]+(y/size[0])*(ext[3]-ext[2])
-    return rx, ry
-
-
-def real2px(x, y, size, ext):
-    px = size[1]*(x-ext[0])/(ext[1]-ext[0])
-    py = size[0]*(y-ext[2])/(ext[3]-ext[2])
-    return px, py
-
-
-def gaussian(x, mu, sig, A=1):
-    """
-    Deprecated, please use pySPM.utils.Gauss
-    Will be removed in the next revision
-    """
-    from warnings import warn
-    warn("Function pySPM.SPM.gaussian is deprecated. Please use pySPM.utils.Gauss instead")
-    return A*np.exp(-np.power(x - mu, 2.) / (2 * np.power(sig, 2.)))
-
-def stat(x):
-    """
-    Quick function to display the min/max, mean and standard-deviation of a given data.
-
-    Note
-    ----
-    Please use the more adavanced function pySPM.utils.stat_info which also provide information about the quartile and also plot the distribution
-    """
-    print("Min: {mi:.3f}, Max: {ma:.3f}, Mean: {mean:.3f}, Std: {std:.3f}".format(mi=np.min(x), ma=np.max(x), mean=np.mean(x), std=np.std(x)))
-
-
-def fit2d(Z0, dx=2, dy=1, mask=None):
-    """
-    Fit the input data with a 2D polynom of order dx × dy
-
-    Parameters
-    ----------
-    Z0 : 2D numpy array
-        input data
-    dx : int
-        order of the polynom for the x-axis
-    dy : int
-        order of the polynom for the y-xis
-    mask : 2D numpy array
-        Give a mask where True values only will be used to perform the fitting
-
-    Returns
-    -------
-    numpy array
-        fitting parameters
-    2D numpy array
-        result of the polynom
-    """
-    x = np.arange(Z0.shape[1], dtype=np.float)
-    y = np.arange(Z0.shape[0], dtype=np.float)
-    X0, Y0 = np.meshgrid(x, y)
-    if mask is not None:
-        X = X0[mask]
-        Y = Y0[mask]
-        Z = Z0[mask]
-    else:
-        X = X0
-        Y = Y0
-        Z = Z0
-    x2 = X.ravel()
-    y2 = Y.ravel()
-    A = np.vstack([x2**i for i in range(dx+1)])
-    A = np.vstack([A]+[y2**i for i in range(1, dy+1)])
-    res = scipy.optimize.lsq_linear(A.T, Z.ravel())
-    r = res['x']
-    Z2 = r[0]*np.ones(Z0.shape)
-    for i in range(1, dx+1):
-        Z2 += r[i]*(X0**i)
-    for i in range(1, dy+1):
-        Z2 += r[dx+i]*(Y0**i)
-    return r, Z2
-
-
-def warp_and_cut(img, tform, cut=True):
-    """
-    Perform an Affine transform on the input data and cut them if cut=True
-
-    Parameters
-    ----------
-    img : 2D numpy array
-        input data
-    tform : skimage.transform
-        An Affine fransform to perform on the data
-    cut : bool
-        Should the data be cutted?
-    """
-    New = tf.warp(img, tform, preserve_range=True)
-    Cut = [0, 0] + list(img.shape)
-    if tform.translation[0] >= 0:
-        Cut[2] -= tform.translation[0]
-    elif tform.translation[0] < 0:
-        Cut[0] -= tform.translation[0]
-    if tform.translation[1] >= 0:
-        Cut[1] += tform.translation[1]
-    elif tform.translation[1] < 0:
-        Cut[3] += tform.translation[1]
-    Cut = [int(x) for x in Cut]
-    if cut:
-        New = cut(New, Cut)
-    return New, Cut
-
-
-def get_profile(I, x1, y1, x2, y2, width=0, ax=None, color='w', alpha=0, N=None,\
-        transx=lambda x: x, transy=lambda x: x, interp_order=1, **kargs):
-    """
-    Get a profile from an input matrix.
-    Low-level function. Doc will come laters2 = pySPM.Nanoscan("%s/CyI5b_PCB_ns.xml"%(Path))
-    """
-    d = np.sqrt((x2-x1)**2+(y2-y1)**2)
-    if N is None:
-        N = int(d)+1
-    P = []
-    dx = -width/2*(y2-y1)/d
-    dy = width/2*(x2-x1)/d
-    for w in np.linspace(-width/2, width/2, max(1,width)):
-        dx = -w*(y2-y1)/d
-        dy = w*(x2-x1)/d
-        x = np.linspace(x1+dx, x2+dx, N)
-        y = np.linspace(y1+dy, y2+dy, N)
-        M = scipy.ndimage.interpolation.map_coordinates(I, np.vstack((y, x)), order=interp_order)
-        P.append(M)
-    if kargs.get('debug',False):
-        print("get_profile input coordinates:",x1,y1,x2,y2)
-    if not ax is None:
-        x1 = transx(x1)
-        x2 = transx(x2)
-        y1 = transy(y1)
-        y2 = transy(y2)
-        if kargs.get('debug',False):
-            print("Drawing coordinates:",x1,y1,x2,y2)
-        dx = -width/2*(y2-y1)/d
-        dy = width/2*(x2-x1)/d
-        if type(color) in [tuple, list]:
-            ax.plot([x1, x2], [y1, y2], color=color, alpha=kargs.get('linealpha',1))
-            ax.plot([x1-dx, x1+dx], [y1-dy, y1+dy], color=color, alpha=kargs.get('linealpha',1))
-            ax.plot([x2-dx, x2+dx], [y2-dy, y2+dy], color=color, alpha=kargs.get('linealpha',1))
-        else:
-            ax.plot([x1, x2], [y1, y2], color, alpha=kargs.get('linealpha',1))
-            ax.plot([x1-dx, x1+dx], [y1-dy, y1+dy], color, alpha=kargs.get('linealpha',1))
-            ax.plot([x2-dx, x2+dx], [y2-dy, y2+dy], color, alpha=kargs.get('linealpha',1))
-        if alpha>0:
-            import matplotlib.patches
-            ax.add_patch(matplotlib.patches.Rectangle(
-                (x1+dx,y1+dy), 
-                2*np.sqrt(dx**2+dy**2),
-                np.sqrt((x2-x1)**2+(y2-y1)**2),
-                -np.degrees(np.arctan2(x2-x1,y2-y1)), color=color, alpha=alpha))
-    if len(P)==1:
-        return np.linspace(0, d, N), P[0]
-    return np.linspace(0, d, N), np.vstack(P).T
-
-
-def dist_v2(img, dx=1, dy=1):
-    """
-    Return a 2D array with the distance in pixel with the clothest corner of the array.
-    """
-    x2 = np.arange(img.shape[1])
-    x2 = (np.minimum(x2, img.shape[1]-x2) * dx)**2
-    y2 = np.arange(img.shape[0])
-    y2 = (np.minimum(y2, img.shape[0] - y2) * dy)**2
-    X, Y = np.meshgrid(x2, y2)
-    return np.sqrt(X+Y)
-
-def generate_k_matrices(A, dx, dy):
-    """
-    GENERATE_K_MATRICES k-Matrix generation (helper function).
-    generates k-matrices for the 2D-channel CHANNEL.
-   
-    K is a matrix of the same size as the pixel matrix A, containing the real-life frequency distance of each 
-    pixel position to the nearest corner of an matrix that is one pixel
-    wider/higher.
-    KX is of the same size as K and contains the real-life  difference in x-direction of each pixel position to the nearest corner 
-    of a matrix that is one pixel wider/higher.
-    Similarly, KY is of the  same size as K, containing the real-life difference in y-direction of  each pixel position to the nearest corner of an matrix that is one 
-    pixel wider/higher.
-    """
-    ny, nx = A.shape
-    dkx = 2*np.pi/(nx*dx)
-    dky = 2*np.pi/(ny*dy)
-    
-    ky = np.arange(0, ny);
-    ky = (np.mod(ky+ny/2, ny) - ny/2) * dky
-    
-    kx = np.arange(0, nx);
-    kx = (np.mod(kx+nx/2, nx) - nx/2) * dkx
-    
-    kx, ky = np.meshgrid(kx, ky)
-    k = dist_v2(A, dkx, dky)
-    k[0, 0] = 1.0 # Prevent division by zero error and illegal operand errors. This may be improved...
-    return k, kx, ky
-        
-def mfm_tf(nx, dx, ny, dy, tf_in, derivative=0, transform=0, z=0, A=0, theta=None, phi=None, d=None, delta_w=None):
-    """
-    Draft for the MFM tf function
-    """
-    k, kx, ky = generate_k_matrices(tf_in, dx, dy)
-    # Distance loss
-    tf_out = np.exp(-z*k)
-    if d is not None:
-        tf_out = tf_out / 2.0
-        if not np.isinf(d):
-            if d == 0:
-                tf_out *= k
-            else:
-                tf_out *= 1 - np.exp(-d*k)
-    if A == 0:
-        if transform != 0:
-            assert theta is not None
-            assert phi is not None
-            tf_out *= ((np.cos(theta)+1j*(np.cos(phi)*np.sin(-theta)*kx+np.sin(phi)*np.sin(-theta)*ky)) / k)**transform
-        if derivative == 1:
-            tf_out *= k
-    else:
-        pass # TODO
-    return tf_out * tf_in
-
-def mfm_inv_calc_flat(img, z, tf_in, thickness=None, delta_w=None, amplitude=0, derivative=0, transform=0, mu=1e-8):
-    """
-    MFM inv calc function
-    """
-    theta = np.radians(12)
-    phi = np.radians(-90)
-    ny, nx = img.shape
-    tf = mfm_tf(nx, 1, ny, 1, tf_in, derivative, transform, z, amplitude, theta, phi, thickness, delta_w)
-    tf[0,0] = np.real(np.mean(tf))
-    recon_tf = np.conj(tf) / (mu+np.abs(tf)**2)
-    work_img = np.abs(np.fft.ifft2(np.fft.fft2(img) * recon_tf ))
-    return work_img
-
-def getTikTf(Img, mu, tukey=0, source_tukey=0, debug=False, d=200, real=np.real):
-    import scipy
-    def fit(x, a ,A, bg, x0):
-        return bg+(A-bg)*np.exp(-abs(x-x0)/a)
-    
-    x = np.arange(Img.shape[1])
-    y = np.arange(Img.shape[0])
-    X, Y = np.meshgrid(x, y)
-    x0 = Img.shape[1]/2
-    y0 = Img.shape[0]/2
-    R = np.sqrt((X-x0)**2+(Y-y0)**2)
-    
-    Z = beam_profile(Img, Img, mu=mu, tukey=tukey, source_tukey=source_tukey, real=real)
-    zoom = zoom_center(Z, d)
-    P = zoom[zoom.shape[0]//2, :]
-    p0 = (1,np.max(zoom), 0, len(P)/2)
-    popt, pcov = scipy.optimize.curve_fit(fit, np.arange(len(P)), P, p0, bounds=((0,0,-np.inf,0),np.inf))
-    bg = popt[2]
-    a = popt[0]
-    if debug:
-        return bg+np.exp(-np.abs(R)/a), Z, p0, popt
-    return bg+np.exp(-np.abs(R)/a)
-    
-DEPRECATED_METHODS = {
-    'getRowProfile': 'get_row_profile',
-    'plotProfile':   'plot_profile',
-    'getProfile':    'get_profile',
-    'getShadowMask': 'get_shadow_mask',
-    'addScale':      'add_scale',
-    'getExtent':     'get_extent',
-    'getBinThreshold':'get_bin_threshold',
-    'corrFit2d':      'corrr_fit2d',
-    'getFFT':         'get_fft',
-    'filterLowPass':  'filter_lowpass',
-    'ResizeInfos':    '_resize_infos'
-    }
-
-def method_alias(old_name, new_name):
-    def _alias_meth(self, *args, **kargs):
-        from warnings import warn
-        warn("Function {name} is deprecated. Please use \"{new_name}\" instead".format(name=old_name, new_name=new_name))
-        return getattr(SPM_image, new_name)(self, *args, **kargs)
-    return _alias_meth
-        
-def fun_alias(old_name, new_name):
-    def _alias_fun(*args, **kargs):
-        from warnings import warn
-        warn("Function {name} is deprecated. Please use \"{new_name}\" instead".format(name=old_name, new_name=new_name))
-        return getattr(SPM, new_name)(*args, **kargs)
-    return _alias_fun
-        
-DEPRECATED_FUNCTIONS = {
-        'NormP':'normP',
-        'getProfile':'get_profile',
-        'BeamProfile':'beam_profile',
-        'BeamProfile1D':'beam_profile1d',
-        'Normalize':'normalize',
-        'Align':'align',
-        'ZoomCenter':'zoom_center',
-    }
-    
-for x in DEPRECATED_METHODS:
-    setattr(SPM_image, x, method_alias(x, DEPRECATED_METHODS[x]))
-
-thisModule = sys.modules[__name__]
-for x in DEPRECATED_FUNCTIONS:
-    setattr(thisModule, x, fun_alias(x, DEPRECATED_FUNCTIONS[x]))    
+# -- coding: utf-8 --
+
+# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
+
+"""
+Library to handle SPM data.
+This is the core module of all images retrieved by SPM and ToF-SIMS.
+"""
+
+import copy
+
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+import numpy as np
+import scipy
+import scipy.interpolate
+import scipy.ndimage
+import scipy.optimize
+import skimage
+import skimage.exposure
+import skimage.filters
+from skimage import transform as tf
+from skimage.draw import disk
+
+from .utils import CDF, funit
+from .utils.misc import PB
+
+try:
+    from skimage.filters import threshold_local
+except:
+    # For compatibility with old versions of skimage
+    from skimage.filters import threshold_adaptive as threshold_local
+
+
+class SPM_image:
+    """
+    Main class to handle SPM images.
+    This class contains the pixels data of the images as well as it's real size.
+    It also provides a lot of tools to correct and perform various analysis and tasks on the image.
+    """
+
+    def __init__(self, BIN, channel='Topography',
+                 corr=None, real=None, zscale='?', _type='Unknown'):
+        """
+        Create a new SPM_image
+
+        Parameters
+        ----------
+        BIN : 2D numpy array
+            The pixel values of the image as a 2D numpy array
+        channel : string
+            The name of the channel. What does the image represents?
+        corr : string or None
+            'slope' : correct the SPM image for its slope (see pySPM.SPM.SPM_image.correct_slope)
+            'lines' : correct the SPM image for its lines (see pySPM.SPM.SPM_image.correct_lines)
+            'plane' : correct the SPM image by plane fitting (see pySPM.SPM.SPM_image.correct_plane)
+        real : None or dictionary
+            Information about the real size of the image {'x':width,'y':height,'unit':unit_name}
+        zscale : string
+            Unit used to describe the z-scale. (units of the data of BIN)
+        _type : string
+            represent the type of measurement
+        """
+        self.channel = channel
+        self.direction = 'Unknown'
+        self.size = {'pixels': {'x': BIN.shape[1], 'y': BIN.shape[0]}}
+        if not real is None:
+            self.size['real'] = real
+        else:
+            self.size['real'] = {'unit': 'pixels',
+                                 'x': BIN.shape[1], 'y': BIN.shape[0]}
+        if not 'unit' in self.size['real']:
+            self.size['real']['unit'] = 'px'
+        self.pixels = BIN
+        self.type = _type
+        self.zscale = zscale
+        if corr is not None:
+            if corr.lower() == 'slope':
+                self.correct_slope()
+            elif corr.lower() == 'lines':
+                self.correct_lines()
+            elif corr.lower() == 'plane':
+                self.correct_plane()
+
+    def __add__(self, b):
+        """
+        Add up two images. This is a low level function and no check is performed to proof that both images have the same size.
+        """
+        New = copy.deepcopy(self)
+        if isinstance(b, SPM_image):
+            New.pixels += b.pixels
+            New.channel += " + " + b.channel
+        elif type(b) in [int, float]:
+            New.pixels += b
+            New.channels += " + {:.2f}".format(b)
+        return New
+
+    def __sub__(self, b):
+        """
+        Subtract two images. This is a low level function and no check is performed to proof that both images have the same size.
+        """
+        New = copy.deepcopy(self)
+        if isinstance(b, SPM_image):
+            New.pixels -= b.pixels
+            New.channel += " - " + b.channel
+        elif type(b) in [int, float]:
+            New.pixels -= b
+            New.channels += " - {:.2f}".format(b)
+        return New
+
+    def __mul__(self, b):
+        New = copy.deepcopy(self)
+        if isinstance(b, SPM_image):
+            New.pixels *= b.pixels
+            New.channel = "({})*{}".format(New.channel, b.channel)
+        elif type(b) in [int, float]:
+            New.pixels *= b
+            New.channels = "({})*{:.2f}".format(New.channel, b)
+        return New
+
+    def __div__(self, b):
+        New = copy.deepcopy(self)
+        if isinstance(b, SPM_image):
+            New.pixels /= b.pixels
+            New.channel = "({})/{}".format(New.channel, b.channel)
+        elif type(b) in [int, float]:
+            New.pixels /= b
+            New.channels = "({})/{:.2f}".format(New.channel, b)
+        return New
+
+    def pxs(self):
+        """
+        Return the pixel size
+        """
+        fxy = {xy: funit(self.size['real'][xy], self.size['real']['unit']) for xy in 'xy'}
+        return [(fxy[xy]['value'] / self.size['pixels'][xy], fxy[xy]['unit']) for xy in 'xy']
+
+    def add_scale(self, length, ax=None, height=20, margin=5, color='w', loc=4, text=True, pixels=None, fontsize=20,
+                  edge_color='k', edge_width=3):
+        """
+        Display a scale marker on an existing image
+
+        Parameters
+        ----------
+
+        length : float
+            The length of the scale in real units
+        ax : matplotlib axis
+            if None the current axis will be taken (plt.gca())
+        height : int
+            The height of the scale bar in pixels
+        color : string
+            The color used to display the scale bar
+        loc : int
+            The location of the scale bar.
+            1 : top right
+            2 : top left
+            3 : bottom left
+            4 : bottom right
+        text : bool
+            display the size of the scale on top of it?
+        pixels : bool
+            Is the image plotted in ax with a x/y scale in pixels?
+        fontsize : float
+            The fontsize used to display the text
+
+        Example
+        -------
+        >>> img = pySPM.SPM_image()
+        >>> img.show()
+        >>> img.add_scale(50e-6, pixels=False);
+        Add a scale of 50 μm on an image displayed with real units
+
+        >>> img = pySPM.SPM_image()
+        >>> img.show(pixels=True)
+        >>> img.add_scale(50e-6);
+        Add a scale of 50 μm on an image displayed in pixels
+        """
+
+        import matplotlib.patches
+        import matplotlib.patheffects as PathEffects
+
+        fL = length / self.size['real']['x']
+        L = self.size['pixels']['x'] * fL
+        fH = height / self.size['pixels']['y']
+        if ax is None:
+            ax = plt.gca()
+        if pixels is None:
+            if hasattr(ax, 'isPixel'):
+                pixels = ax.isPixel
+            else:
+                pixels = False
+        flipped = False
+        if hasattr(ax, 'flipped'):
+            flipped = ax.flipped
+        if type(loc) is int:
+            assert loc in [1, 2, 3, 4]
+            ref = ax.transAxes.transform({1: (1 - fL, 0), 2: (0, 0), 3: (0, 1 - fH), 4: (1 - fL, 1 - fH)}[loc])
+            if loc in [2, 3]:
+                ref[0] += margin
+            else:
+                ref[0] -= margin
+            if loc in [1, 2]:
+                ref[1] += margin
+            else:
+                ref[1] -= margin
+        else:
+            assert type(loc) in [tuple, list]
+            assert len(loc) == 2
+            ref = ax.transData.transform(loc) + ax.transAxes.transform((-fL / 2, -fH / 2)) - ax.transAxes.transform(
+                (0, 0))
+        inv = ax.transData.inverted()
+        ref = inv.transform(ref)
+        WH = inv.transform(ax.transAxes.transform((fL, fH))) - inv.transform(ax.transAxes.transform((0, 0)))
+        rect = ax.add_patch(matplotlib.patches.Rectangle(ref, width=WH[0], height=WH[1], color=color))
+
+        if text:
+            r = funit(length, self.size['real']['unit'])
+            if r['unit'][0] == 'u':
+                r['unit'] = 'µ' + r['unit'][1:]
+            if loc in [3, 4]:
+                label_ref = [ref[0] + WH[0] / 2, ref[1]]
+                ann = ax.annotate("{value:.01f} {unit}".format(**r),
+                                  label_ref, color=color,
+                                  fontsize=fontsize, va="top", ha="center")
+            else:
+                label_ref = [ref[0] + WH[0] / 2, ref[1] + WH[1]]
+                ann = ax.annotate("{value:.01f} {unit}".format(**r),
+                                  label_ref, color=color,
+                                  fontsize=fontsize, va="bottom", ha="center")
+            ann.set_path_effects([PathEffects.withStroke(linewidth=edge_width, foreground=edge_color)])
+
+    def offset(self, profiles, width=1, ax=None, col='w', inline=True, **kargs):
+        """
+        Correct an image by offsetting each row individually in order that the lines passed as argument in "profiles" becomes flat.
+
+        Parameters
+        ----------
+        profiles: list of list
+            each sublist represent a line as [x1, y1, x2, y2] in pixels known to be flat
+        width : int, float
+            the line width in pixels used for better statistics
+        ax : matplotlib axis or None
+            If not None, axis in which the profiles will be plotted in
+        inline : bool
+            If True perform the correction on the current object, otherwise return a new image
+        col : string
+            matrplotlib color used to plot the profiles (if ax is not None)
+        labels : bool
+            display a label number with each profile
+        **kargs: arguments passed further to get_row_profile.
+            axPixels: set to True if you axis "ax" have the data plotted in pixel instead of real distance
+
+        Example
+        -------
+        Exampel if the data are plotted in pixels:
+        >>> topo = pySPM.SPM_image(...)
+        >>> fig, ax = plt.subplots(1, 2, figsize=(10, 5))
+        >>> topoC = topo.offset([[150, 0, 220, 255]], inline=False,axPixels=True)
+        >>> topo.show(pixels=True, ax=ax[0])
+        >>> topoC.show(ax=ax[1]);
+
+        Example if the data are plotted with real units
+        >>> topo = pySPM.SPM_image(...)
+        >>> fig, ax = plt.subplots(1, 2, figsize=(10, 5))
+        >>> topoC = topo.offset([[150, 0, 220, 255]], inline=False)
+        >>> topo.show(ax=ax[0])
+        >>> topoC.show(ax=ax[1]);
+        """
+        offset = np.zeros(self.pixels.shape[0])
+        counts = np.zeros(self.pixels.shape[0])
+        for i, p in enumerate(profiles):
+            if kargs.get('labels', False):
+                y, D = self.get_row_profile(*p, width=width, ax=ax, col=col, label=str(i), **kargs)
+            else:
+                y, D = self.get_row_profile(*p, width=width, ax=ax, col=col, **kargs)
+            counts[y] += 1
+            offset[y[1:]] += np.diff(D)
+        counts[counts == 0] = 1
+        offset = offset / counts
+        offset = np.cumsum(offset)
+        offset = offset.reshape((self.pixels.shape[0], 1))
+        if inline:
+            self.pixels = self.pixels - \
+                          np.flipud(np.repeat(offset, self.pixels.shape[1], axis=1))
+            return self
+        else:
+            C = copy.deepcopy(self)
+            C.pixels = self.pixels - \
+                       np.flipud(np.repeat(offset, self.pixels.shape[1], axis=1))
+            return C
+
+    def pxRect2Real(self, xy, width, height):
+        """
+        Transform a xy, width, height data in pixels to an equivalentz one with real units
+        """
+        ll = self.px2real(xy[0], xy[1])
+        ur = self.px2real(xy[0] + width, xy[1] + height)
+        return ll, ur[0] - ll[0], ur[1] - ll[1]
+
+    def get_row_profile(self, x1, y1, x2, y2, width=1, col='C1', ax=None, alpha=0, **kargs):
+        """
+        Get a profile per row along a given line. This function is mainly useful for the function offset.
+        
+        x1, y1, x2, y2: int
+            coordinates of the line.
+        width : int
+            the width of the line used for statistics (in pixels)
+        col: string
+            color used to plot the line position
+        ax : matplotlib axis
+            axis in which the lines position will plotted
+        alpha : float
+            The alpha channel of the line color (≥0 and ≤1)
+        **kargs:
+            line style arguments: linewidth, color and linestyle
+            axis units: axPixels set to True if ax has the image plotted in pixels.
+            
+        Returns
+        -------
+        Y coordinates : 1D numpy array
+            distance along the profile starting at 0
+        Z coordinates : 1D numpy array
+            profile
+        """
+        plotargs = {key: kargs[key] for key in ['linewidth', 'color', 'linestyle'] if key in kargs}
+        if y2 < y1:
+            x1, y1, x2, y2 = x2, y2, x1, y1
+        if ax is not None:
+            d = np.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2)
+            dx = -width / 2 * (y2 - y1) / d
+            dy = width / 2 * (x2 - x1) / d
+            if kargs.get('axPixels', False):
+                ax.plot([x1 - dx, x1 + dx], [y1 - dy, y1 + dy], col)
+                ax.plot([x2 - dx, x2 + dx], [y2 - dy, y2 + dy], col)
+                ax.plot((x1, x2), (y1, y2), col, **plotargs)
+                if kargs.get('label', False):
+                    ax.annotate(kargs.get('label'), (.5 * (x1 + x2), .5 * (y1 + y2)), color=col)
+                if alpha > 0:
+                    import matplotlib.patches
+                    ax.add_patch(matplotlib.patches.Rectangle((x1 + dx, y1 + dy), width, d,
+                                                              -np.degrees(np.arctan2(x2 - x1, y2 - y1)), color=col,
+                                                              alpha=alpha))
+            else:
+                h = self.pixels.shape[0]
+                pxs = self.size['real']['x'] / self.pixels.shape[1]
+                pys = self.size['real']['y'] / h
+                ax.plot([(x1 - dx) * pxs, (x1 + dx) * pxs], [(h - (y1 - dy)) * pys, (h - (y1 + dy)) * pys], col)
+                ax.plot([(x2 - dx) * pxs, (x2 + dx) * pxs], [(h - (y2 - dy)) * pys, (h - (y2 + dy)) * pys], col)
+                ax.plot((x1 * pxs, x2 * pxs), ((h - y1) * pys, (h - y2) * pys), col, **plotargs)
+                if kargs.get('label', False):
+                    ax.annotate(kargs.get('label'), (.5 * (x1 + x2) * pxs, .5 * (2 * h - y1 - y2) * pys), color=col)
+                if alpha > 0:
+                    import matplotlib.patches
+                    W = np.sqrt((2 * dx * pxs) ** 2 + (2 * dy * pys) ** 2)
+                    L = np.sqrt(((x2 - x1) * pxs) ** 2 + ((y2 - y1) * pys) ** 2)
+                    ax.add_patch(matplotlib.patches.Rectangle(((x1 + dx) * pxs, (y1 + dy) * pys), W, L,
+                                                              -np.degrees(np.arctan2((x2 - x1) * pxs, (y2 - y1) * pys)),
+                                                              color=col, alpha=alpha))
+
+        x = np.arange(self.pixels.shape[1])
+        y = np.arange(self.pixels.shape[0])
+        I = scipy.interpolate.interp2d(x, y, np.flipud(self.pixels))
+
+        Y = np.arange(y1, y2 + 1)
+        V = np.zeros(len(Y))
+        for w in np.arange(width):
+            xl = np.linspace(x1 - (width - 1) / 2. + w, x2 - (width - 1) / 2. + w, len(Y))
+            for i in range(len(Y)):
+                Z = I(xl[i], Y[i])
+                V[i] += Z
+        return Y, V / width
+
+    def correct_median_diff(self, inline=True):
+        """
+        Correct the image with the median difference
+        """
+        N = self.pixels
+        # Difference of the pixel between two consecutive row
+        N2 = N - np.vstack([N[:1, :], N[:-1, :]])
+        # Take the median of the difference and cumsum them
+        C = np.cumsum(np.median(N2, axis=1))
+        # Extend the vector to a matrix (row copy)
+        D = np.tile(C, (N.shape[0], 1)).T
+        if inline:
+            self.pixels = N - D
+        else:
+            New = copy.deepcopy(self)
+            New.pixels = N - D
+            return New
+
+    def correct_slope(self, inline=True):
+        """
+        Correct the image by subtracting a fitted slope along the y-axis
+        """
+        s = np.mean(self.pixels, axis=1)
+        i = np.arange(s.shape[0])
+        fit = np.polyfit(i, s, 1)
+        if inline:
+            self.pixels -= np.tile(np.polyval(fit, i).reshape(self.pixels.shape[0], 1), self.pixels.shape[1])
+            return self
+        else:
+            New = copy.deepcopy(self)
+            New.pixels -= np.tile(np.polyval(fit, i).reshape(self.pixels.shape[0], 1), self.pixels.shape[1])
+            return New
+
+    def correct_plane(self, inline=True, mask=None):
+        """
+        Correct the image by subtracting a fitted 2D-plane on the data
+
+        Parameters
+        ----------
+        inline : bool
+            If True the data of the current image will be updated otherwise a new image is created
+        mask : None or 2D numpy array
+            If not None define on which pixels the data should be taken.
+        """
+        x = np.arange(self.pixels.shape[1])
+        y = np.arange(self.pixels.shape[0])
+        X0, Y0 = np.meshgrid(x, y)
+        Z0 = self.pixels
+        if mask is not None:
+            X = X0[mask]
+            Y = Y0[mask]
+            Z = Z0[mask]
+        else:
+            X = X0
+            Y = Y0
+            Z = Z0
+        A = np.column_stack((np.ones(Z.ravel().size), X.ravel(), Y.ravel()))
+        c, resid, rank, sigma = np.linalg.lstsq(A, Z.ravel(), rcond=-1)
+        if inline:
+            self.pixels -= c[0] * \
+                           np.ones(self.pixels.shape) + c[1] * X0 + c[2] * Y0
+            return self
+        else:
+            New = copy.deepcopy(self)
+            New.pixels -= c[0] * np.ones(self.pixels.shape) + c[1] * X0 + c[2] * Y0
+            return New
+
+    def correct_lines(self, inline=True):
+        """
+        Subtract the average of each line for the image.
+
+        if inline is True the current data are updated otherwise a new image with the corrected data is returned
+        """
+        if inline:
+            self.pixels -= np.tile(np.mean(self.pixels, axis=1).T, (self.pixels.shape[1], 1)).T
+            return self
+        else:
+            New = copy.deepcopy(self)
+            New.pixels -= np.tile(np.mean(self.pixels, axis=1).T, (self.pixels.shape[1], 1)).T
+            return New
+
+    def dist_v2(self, pixel=False):
+        """
+        Return a 2D array with the distance between each pixel and the closest border.
+        Might be usefull for FFT filtering
+        """
+        if pixel:
+            dx = 1
+            dy = 1
+        else:
+            dx = self.size['real']['x'] / self.size['pixels']['x']
+            dy = self.size['real']['y'] / self.size['pixels']['y']
+        x2 = np.arange(self.size['pixels']['x'])
+        x2 = (np.minimum(x2, self.size['pixels']['x'] - x2) * dx) ** 2
+        y2 = np.arange(self.size['pixels']['y'])
+        y2 = (np.minimum(y2, self.size['pixels']['y'] - y2) * dy) ** 2
+        X, Y = np.meshgrid(x2, y2)
+        return np.sqrt(X + Y)
+
+    def inv_calc_flat(self, d, l=0.1):
+        """
+        Function used for inverse MFM calculation (inspired from http://qmfm.empa.ch/qmfm/)
+        The function is in its early devlopment stage as not used by the developed.
+
+        Parameters
+        ----------
+        d : float
+            Height distance in the input data
+        l : float
+            Tikhonov parameter for the deconvolution
+        """
+        work_image = self.pixels
+        ny, nx = self.pixels.shape
+        dx = self.size['real']['x'] / self.size['pixels']['x']
+        dy = self.size['real']['y'] / self.size['pixels']['y']
+
+        k = self.dist_v2()
+        k[0, 0] = 1e-10
+
+        tf = np.exp(-d * k)
+        tf[0, 0] = np.mean(tf)
+        tf /= 2
+        tf *= 1 - np.exp(-d * k)
+
+        recon_tf = np.ones(tf.shape) / (tf + l * np.ones(tf.shape) / np.conj(tf))
+        tf *= recon_tf
+        return np.real(np.fft.ifft2(np.fft.fft2(work_image) * recon_tf))
+
+    def get_extent(self):
+        """
+        Get the image extent in real data
+        """
+        if 'recorded' in self.size:
+            W = self.size['recorded']['real']['x']
+            H = self.size['recorded']['real']['y']
+        else:
+            W = self.size['real']['x']
+            H = self.size['real']['y']
+        return (0, W, 0, H)
+
+    def show(self, ax=None, sig=None, cmap=None, title=None,
+             adaptive=False, dmin=0, dmax=0, pixels=False, flip=False, wrap=None, mul=1, symmetric=False, **kargs):
+        """
+        Function to display the image with a lot of parametrization
+
+        Parameters
+        ----------
+        ax : matplotlib axis or None
+            matplotlib axis if given otherwise current axis will be used (plt.gca())
+        sig : float
+            sigma values to adjust the contrast range around the mean ±sig times the standard-deviation
+        cmap : string
+            colormap name used. By default a gray map is used. If the zscale of the data are in 'meter' (i.e. topography data) the 'hot' colormap is used
+        title : string
+            The title of the plot. By default is the channel name
+        adaptive : bool
+            The color scale used is linear. If adaptive is True a non linear color scale is used in order that each color is used with the same amount.
+        dmin : float
+            minimum value adjustment used for the colorscale
+        dmax: float
+            maximum value adjustment used for the colorscale
+        pixels : bool
+            Display the image with x/y-labels with real unit. If pixels is True, the axes are in pixels
+        flip : bool
+            Flip the image upside-down
+        wrap : Nont or int
+            wrap the title to a width of wrap chars
+        symmetric : bool
+            If True will place the middle of the colorscale to the value 0.
+            This is specially usefull for diverging colormaps such as : BrBG, bwr, coolwarm, seismiv, spectral, etc.
+        level : float
+            level should be ≥0 and <50. Adjust the lower and upper colorscale to level% and (100-level)% of the data range.
+            e.g. if level=1, the colorscale will display 1-99% of the data range
+        vmin : float
+            Minimum value used for the colorscale
+        vmax : flaot
+            Maximum value used for the colorscale
+
+
+        Returns
+        -------
+        matplotlib.image.AxesImage
+            matplolib axis instance returned by imshow
+
+        Examples
+        --------
+        >>> topo = pySPM.SPM_image(...)
+        >>> fig, (ax, ax2) = plt.subplots(2, 3, figsize=(15, 10))
+        >>> topo.show(ax=ax[0], cmap='gray', title="color map=\"gray\"")
+        >>> topo.show(ax=ax[1], sig=2, title="standard deviation=2")
+        >>> topo.show(ax=ax[2], adaptive=True, title="Adaptive colormap")
+        >>> topo.show(ax=ax2[0], dmin=4e-8, cmap='gray', title="raise the lowest value for the colormap of +40nm")
+        >>> topo.show(ax=ax2[1], dmin=3e-8, dmax=-3e-8, cmap='gray',title="raise lower of +30nm and highest of -30nm")
+        >>> topo.show(ax=ax2[2], pixels=True, title="Set axis value in pixels");
+        """
+        mpl.rc('axes', grid=False)
+
+        if ax is None:
+            ax = plt.gca()
+        ax.src = self
+        if title == None:
+            title = u"{0} - {1}".format(self.type, self.channel)
+        if wrap is not None:
+            title = "\n".join([title[i * wrap:(i + 1) * wrap]
+                               for i in range(int(len(title) / wrap) + 1)])
+        unit = self.size['real']['unit']
+        sunit = 'afpnum kMGTPE'
+        if len(unit) == 1 or unit in ['pixels']:
+            isunit = 6
+        elif unit[0] in sunit:
+            isunit = sunit.find(unit[0])
+            unit = unit[1:]
+        else:
+            isunit = 6
+        W = self.size['real']['x']
+        H = self.size['real']['y']
+        fact = int(np.floor(np.log(W) / np.log(10) / 3))
+        isunit += fact
+        W, H = W / 10 ** (fact * 3), H / 10 ** (fact * 3)
+        if cmap == None:
+            cmap = 'gray'
+            if unit == 'm' and self.channel == "Topography":
+                cmap = 'hot'
+        mi, ma = np.nanmin(self.pixels), np.nanmax(self.pixels)
+        if adaptive:
+            img = np.asarray(256 ** 2 * (self.pixels - mi) / (ma - mi), dtype=np.uint16)
+            mi, ma = 0, 1
+            img = skimage.exposure.equalize_adapthist(img, clip_limit=0.03)
+        else:
+            img = mul * self.pixels
+            mi *= mul
+            ma *= mul
+
+        if sig == None:
+            vmin = mi + dmin
+            vmax = ma + dmax
+        else:
+            std = np.nanstd(img)
+            avg = np.nanmean(img)
+            vmin = avg - sig * std
+            vmax = avg + sig * std
+        if 'level' in kargs:
+            if kargs['level'] < 0 or kargs['level'] >= 50:
+                raise ValueError("The level shoud have a value in [0,50)")
+            vmax = np.percentile(img, 100 - kargs['level'])
+            vmin = np.percentile(img, kargs['level'])
+            del kargs['level']
+        if 'vmin' in kargs:
+            vmin = kargs['vmin']
+            del kargs['vmin']
+        if 'vmax' in kargs:
+            vmax = kargs['vmax']
+            del kargs['vmax']
+        if symmetric:
+            vmax = abs(max(vmin, vmax))
+            vmin = -vmax
+        if not flip:
+            ax.flipped = False
+            if pixels:
+                ax.isPixel = True
+                r = ax.imshow(np.flipud(img), extent=[0, img.shape[1], img.shape[0], 0], cmap=cmap, vmin=vmin,
+                              vmax=vmax, **kargs)
+            else:
+                ax.isPixel = False
+                r = ax.imshow(np.flipud(img), extent=[0, W, 0, H], cmap=cmap, vmin=vmin, vmax=vmax, **kargs)
+        else:
+            ax.flipped = True
+            if pixels:
+                ax.isPixel = True
+                r = ax.imshow(np.flipud(img), extent=[0, img.shape[1], img.shape[0], 0], cmap=cmap, vmin=vmin,
+                              vmax=vmax, **kargs)
+            else:
+                ax.isPixel = False
+                r = ax.imshow(np.flipud(img), cmap=cmap, extent=[0, W, 0, H], vmin=vmin, vmax=vmax, **kargs)
+        if pixels:
+            ax.set_xlim((0, self.pixels.shape[1]))
+            if flip:
+                ax.set_ylim((0, self.pixels.shape[0]))
+            else:
+                ax.set_ylim((self.pixels.shape[0], 0))
+        else:
+            ax.set_xlim((0, W))
+            if flip:
+                ax.set_ylim((H, 0))
+            else:
+                ax.set_ylim((0, H))
+
+        if not pixels:
+            if isunit != 6:
+                u = sunit[isunit]
+                if u == 'u':
+                    u = 'µ'
+                ax.set_xlabel(u'x [{0}{1}]'.format(u, unit))
+                ax.set_ylabel(u'y [{0}{1}]'.format(u, unit))
+            else:
+                ax.set_xlabel(u'x [{0}]'.format(unit))
+                ax.set_ylabel(u'y [{0}]'.format(unit))
+        if title != None:
+            ax.set_title(title)
+        return r
+
+    def real2px(self, x, y):
+        """
+        Transform a real (x,y) value in pixels
+        Units should be the same as the one plotted by pySPM.SPM_image.show
+        """
+        return self.real2pixels(x, y)
+
+    def real2pixels(self, x, y, float=False):
+        """
+        Transform a real (x,y) value in pixels
+        Units should be the same as the one plotted by pySPM.SPM_image.show
+        """
+        W = self.size['real']['x']
+        fact = int(np.floor(np.log(W) / np.log(10) / 3)) * 3
+        if not float:
+            px = np.digitize(x, np.linspace(0, self.size['real']['x'] / (10 ** fact), self.pixels.shape[1]), right=True)
+            py = np.digitize(y, np.linspace(0, self.size['real']['y'] / (10 ** fact), self.pixels.shape[0]),
+                             right=False)
+        else:
+            px = x * (self.pixels.shape[1] - 1) / (self.size['real']['x'] / (10 ** fact))
+            py = y * (self.pixels.shape[0] - 1) / (self.size['real']['y'] / (10 ** fact))
+        return px, py
+
+    def px2real(self, x, y):
+        """
+        Transform  a (x,y) value from pixels to real
+        Units are the same as the one plotted by pySPM.SPM_image.show
+        """
+        W = self.size['real']['x']
+        fact = int(np.floor(np.log(W) / np.log(10) / 3)) * 3
+        rx = x * self.size['real']['x'] / (10 ** fact) / self.pixels.shape[1]
+        ry = (self.pixels.shape[0] - y) * self.size['real']['y'] / (10 ** fact) / self.pixels.shape[0]
+        return rx, ry
+
+    def circular_profile(self, x0, y0, Ra=1, Rn=0, width=1, N=20, A=0, B=360, \
+                         cmap='jet', axImg=None, axPolar=None, axProfile=None, plotProfileEvery=1, \
+                         xtransf=lambda x: x * 1e9, ytransf=lambda x: x * 1e9, \
+                         ToFcorr=False, fit=lambda x, *p: p[3] + p[2] * CDF(x, *p[:2]), p0=None, errors=False,
+                         bounds=(-np.inf, np.inf), fakefit=False, **kargs):
+        """
+        Create radial profiles from point x0,y0 with length Ra (outer radius) and Rn (negative Radius).
+        Start from angle A° to angle B° with N profiles.
+        If you want to apply the ToF-correction, please set ToFcorr to the number of scans used to record the ToF-SIMS image.
+        Return the fitting uncertainty on sigma if errors is set to True
+        The fitting function can be adjusted by fit and the default parameters by p0 which is an array of function where the first parameter passed will be the x-values and the second the y-values.
+        """
+        from matplotlib import colors, cm
+
+        # Create a colormap for each profile
+        CM = plt.get_cmap(cmap)
+        cNorm = colors.Normalize(vmin=0, vmax=N)
+        scalarMap = cm.ScalarMappable(norm=cNorm, cmap=CM)
+        res = []
+        cov = []
+        angles = []
+        assert A < B
+        for i, angle in enumerate(np.linspace(A, B, N)):
+            a = np.radians(angle)
+            angles.append(a)
+            l, p = self.get_profile(
+                x0 - Rn * np.cos(a),
+                y0 + Rn * np.sin(a),
+                x0 + Ra * np.cos(a),
+                y0 - Ra * np.sin(a),
+                ax=axImg, width=width, color=scalarMap.to_rgba(i), **kargs)
+            if width == 0:
+                profile = p
+            else:
+                profile = np.mean(p, axis=1)
+            if ToFcorr:
+                profile = -np.log(1.001 - profile / ToFcorr)
+            if p0 is None:
+                AC = np.mean(profile[:len(l) // 2])
+                AE = np.mean(profile[len(l) // 2:])
+                if AC < AE:
+                    p0 = [l[len(l) // 2], 5 * (l[1] - l[0]), np.max(profile) - np.min(profile), np.min(profile)]
+                else:
+                    p0 = [l[len(l) // 2], 5 * (l[1] - l[0]), -np.max(profile) + np.min(profile), np.max(profile)]
+            else:
+                for j, p in enumerate(p0):
+                    if callable(p):
+                        p0[j] = p(l, profile)
+            if kargs.get('debug', False):
+                print("calculate fit parameters are", p0)
+            if not fakefit:
+                p0, pcov = scipy.optimize.curve_fit(fit, l, profile, p0)
+            else:
+                pcov = np.zeros((len(p0), len(p0)))
+            res.append(p0)
+            cov.append([np.sqrt(abs(pcov[i, i])) for i in range(len(p0))])
+            if axProfile and i % plotProfileEvery == 0:
+                axProfile.plot(xtransf(l - p0[0]), profile, color=scalarMap.to_rgba(i), linestyle=':')
+                axProfile.plot(xtransf(l - p0[0]), fit(l, *p0), color=scalarMap.to_rgba(i))
+        # close loop
+        if A % 360 == B % 360:
+            angles.append(angles[0])
+            res.append(res[0])
+            cov.append(cov[0])
+
+        # Plot polar
+        angles = np.array(angles)
+        res = np.array(res)
+        cov = np.array(cov)
+        fact = 2 * np.sqrt(2 * np.log(2))
+        if axPolar:
+            axPolar.plot(angles, ytransf(res[:, 1]), color=kargs.get('sig_color', 'C0'), label="$\\sigma$")
+            axPolar.plot(angles, ytransf(fact * res[:, 1]), color=kargs.get('fwhm_color', 'C1'), label="FWHM")
+            if errors:
+                axPolar.fill_between(angles, ytransf(res[:, 1] - cov[:, 1]), ytransf(res[:, 1] + cov[:, 1]),
+                                     color=kargs.get('sig_color', 'C0'), alpha=kargs.get('fillalpha', .5))
+                axPolar.fill_between(angles, fact * ytransf(res[:, 1] - cov[:, 1]), ytransf(res[:, 1] + cov[:, 1]),
+                                     color=kargs.get('fwhm_color', 'C1'), alpha=kargs.get('fillalpha', .5))
+
+        return angles, res, cov
+
+    def get_profile(self, x1, y1, x2, y2, width=0, ax=None, pixels=True, color='w', axPixels=None, **kargs):
+        """
+        retrieve the profile of the image between pixel x1,y1 and x2,y2
+
+        Parameters
+        ----------
+        x1, y1, x2, y2 : ints
+            coordinates for the profile
+        ax : matplotlib axis
+            defines the matplotlib axis on which the position of the profile should be drawn (in not None)
+        width : int
+            the width of the profile (for averaging/statistics) in pixels
+        color : string
+            color used to plot the profiles lines
+        axPixels : bool
+            If True the image plotted in the ax axis is displayed in pixels
+        
+        Returns
+        -------
+        x data : 1D numpy array
+        profile : 1D numpy array
+        """
+        if kargs.get('debug', False):
+            print("get_profile input coordinates:", x1, y1, x2, y2)
+        if ax is not None and axPixels is None:
+            if hasattr(ax, 'isPixel'):
+                axPixels = ax.isPixel
+        if axPixels is None:
+            axPixels = pixels
+        W = self.size['real']['x']
+        fact = int(np.floor(np.log(W) / np.log(10) / 3)) * 3
+        if not pixels:
+            if kargs.get('debug', False):
+                print("Image range (real scale):", self.size['real']['x'] / (10 ** fact),
+                      self.size['real']['y'] / (10 ** fact))
+            x1, y1 = self.real2pixels(x1, y1, float=True)
+            x2, y2 = self.real2pixels(x2, y2, float=True)
+            y1 = self.pixels.shape[0] - y1
+            y2 = self.pixels.shape[0] - y2
+            if kargs.get('debug', False):
+                print("Pixel coordinates:", x1, y1, x2, y2)
+            if not axPixels:
+                xvalues, p = get_profile(np.flipud(self.pixels), x1, y1, x2, y2, ax=ax, width=width, color=color, \
+                                         transx=lambda x: x * (self.size['real']['x'] / (10 ** fact)) /
+                                                          self.pixels.shape[1], \
+                                         transy=lambda x: (self.pixels.shape[0] - x) * (
+                                                 self.size['real']['y'] / (10 ** fact)) / self.pixels.shape[0], \
+                                         **kargs)
+            else:
+                values, p = get_profile(np.flipud(self.pixels), x1, y1, x2, y2, ax=ax, width=width, color=color,
+                                        **kargs)
+        else:
+            if axPixels:
+                values, p = get_profile(np.flipud(self.pixels), x1, y1, x2, y2, ax=ax, width=width, color=color,
+                                        **kargs)
+            else:
+                values, p = get_profile(np.flipud(self.pixels), x1, y1, x2, y2, ax=ax, width=width, color=color, \
+                                        transx=lambda x: x * (self.size['real']['x'] / (10 ** fact)) /
+                                                         self.pixels.shape[1], \
+                                        transy=lambda x: (self.pixels.shape[0] - x) * (
+                                                self.size['real']['y'] / (10 ** fact)) / self.pixels.shape[0], \
+                                        **kargs)
+
+        dx = (x2 - x1) * self.size['real']['x'] / self.size['pixels']['x']
+        dy = (y2 - y1) * self.size['real']['y'] / self.size['pixels']['y']
+        rd = np.sqrt(dx ** 2 + dy ** 2)
+        xvalues = np.linspace(0, rd, len(p))
+        return xvalues, p
+
+    def plot_profile(self, x1, y1, x2, y2, width=0, ax=None, pixels=True, img=None, imgColor='w', ztransf=lambda x: x,
+                     zunit=None, **kargs):
+        """
+        Retrieve and plot a profile from an image
+
+        Parameters
+        ----------
+        x1, y1, x2, y2 : int
+            coordinate of the profile in real size or in pixels (if pixels is True)
+        width : float
+            the width of the profiles in pixels for better statistics
+        ax : matplotlib axis
+            The axis in which the profile will be plotted
+        pixels : bool
+            If True the coordinates are given in pixels and not in real units
+        img : matplotlib axis
+            The axis in which the profile position will be drawn
+        imgColor : string
+            The color used to display the profile positions
+        ztransf : function
+            function to transform the profile data. This can be used to scale the data.
+            Most profiles are retrieved in 'm' and a 'nm' value can be used by using ztransf=lambda x: x*1e9
+        zunit : string
+            the zunit name used if ztransft is used
+        color : string
+            The color of the profile
+        col : string
+            can be used instead of color
+        stdplot : bool
+            If True display the ±nσ plots where n is given by the sig parameter
+        sig : int
+            The number of sigmas used in stdplot
+        label : string
+            The label used for plotting the profile (useful if you perform a ax.legend() afterwards)
+
+        Returns
+        -------
+        dictionary : {'plot': matplotlib_plot_instance, 'l': profile_xaxis, 'z': profile_yaxis}
+
+        Examples
+        --------
+        >>> topo = pySPM.SPM_image(...)
+        >>> fig, ax = plt.subplots(1, 2, figsize=(10, 5))
+        >>> topo.plot_profile(70, 100, 170, 200, ax=ax[1], img=ax[0], ztransf=lambda x:x*1e9, zunit='nm');
+        >>> topo.show(ax=ax[0], pixels=True);
+        """
+        col = kargs.get('color', kargs.get('col', 'C0'))
+        W = self.size['real']['x']
+        fact = int(np.floor(np.log(W) / np.log(10) / 3)) * 3
+        if ax == None:
+            ax = plt.gca()
+        xvalues, p = self.get_profile(x1, y1, x2, y2, width=width, color=imgColor, ax=img, pixels=pixels, **kargs)
+        d = np.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2)
+        dx = (x2 - x1)
+        dy = (y2 - y1)
+        if pixels:
+            rd = d
+            u = ''
+            unit = 'px'
+        else:
+            unit = self.size['real']['unit']
+            sunit = 'afpnum kMGTPE'
+            if len(unit) == 1:
+                isunit = 6
+            elif unit[0] in sunit:
+                isunit = sunit.find(unit[0])
+                unit = unit[1:]
+            else:
+                isunit = 6
+            isunit += fact // 3
+            if isunit != 6:
+                u = sunit[isunit]
+            else:
+                u = ''
+            if u == 'u':
+                u = 'µ'
+            rd = np.sqrt(dx ** 2 + dy ** 2)
+        xvalues = np.linspace(0, rd, len(p))
+        lab = kargs.get("label", "")
+        if width < 2:
+            profile = ztransf(p)
+        else:
+            profile = ztransf(np.mean(p, axis=1))
+            s = np.std(p)
+            if kargs.get('stdplot', False):
+                for ns in range(1, kargs.get('sig', 2) + 1):
+                    ax.fill_between(xvalues, profile - ns * s, profile + ns * s, color=col, alpha=.2,
+                                    label=[lab + ' ($\\sigma,\ldots {}\\sigma$)'.format(kargs.get('sig', 2)), None][
+                                        ns > 1])
+
+        Plot = ax.plot(xvalues, profile, color=col, linewidth=kargs.get('linewidth', 1),
+                       linestyle=kargs.get('linestyle', '-'), label=lab + [' (mean)', ''][width < 2])
+        if kargs.get('min', False):
+            minStyle = kargs.get('minStyle', kargs.get('minmaxStyle', '--'))
+            minColor = kargs.get('minColor', kargs.get('minmaxColor', col))
+            minMarker = kargs.get('minMarker', kargs.get('minmaxMarker', ''))
+            ax.plot(xvalues, np.min(p, axis=1), color=minColor, linewidth=kargs.get('linewidth', 1), linestyle=minStyle,
+                    marker=minMarker, label=lab + ' (min)')
+        if kargs.get('max', False):
+            maxStyle = kargs.get('maxStyle', kargs.get('minmaxStyle', '--'))
+            maxColor = kargs.get('maxColor', kargs.get('minmaxColor', col))
+            maxMarker = kargs.get('maxMarker', kargs.get('minmaxMarker', ''))
+            ax.plot(xvalues, np.max(p, axis=1), color=maxColor, linestyle=maxStyle, linewidth=kargs.get('linewidth', 1),
+                    marker=maxMarker, label=lab + ' (max)')
+
+        ax.set_xlabel("Distance [{1}{0}]".format(unit, u))
+        if zunit is not None:
+            ax.set_ylabel("{1} [{0}]".format(zunit, self.channel))
+        else:
+            ax.set_ylabel("{1} [{0}]".format(self.zscale, self.channel))
+
+        return {'plot': Plot, 'l': xvalues, 'z': profile}
+
+    def get_bin_threshold(self, percent, high=True, adaptive=False, binary=True, img=False):
+        """
+        Threshold the image into binary values
+        
+        Parameters
+        ----------
+        percent : float
+            The percentage where the thresholding is made
+        high : bool
+            If high a value of 1 is returned for values > percent
+        adaptive : bool
+            If True, performs an adaptive thresholding (see skimage.filters.threshold_adaptive)
+        binary : bool
+            If True return bool data (True/False) otherwise  numeric (0/1)
+        img : bool
+            If True return a SPM_image otherwise a numpy array
+        """
+        if adaptive:
+            if binary:
+                return self.pixels > threshold_local(self.pixels, percent)
+            return threshold_local(self.pixels, percent)
+        mi = np.min(self.pixels)
+        norm = (self.pixels - mi) / (np.max(self.pixels) - mi)
+        if high:
+            r = norm > percent
+        else:
+            r = norm < percent
+        if not img:
+            if binary:
+                return r
+            return np.ones(self.pixels.shape) * r
+        else:
+            I = copy.deepcopy(self)
+            I.channel = "Threshold from " + I.channel
+            if binary:
+                I.pixels = r
+            else:
+                I.pixels = np.ones(self.pixels.shape) * r
+            return I
+
+    def spline_offset(self, X, Y, Z=None, inline=True, ax=None, output='img', **kargs):
+        """
+        subtract a spline interpolated by points corrdinates.
+        if Z is None, the image values will be used (default)
+        """
+        if ax is not None:
+            if 'num' in kargs and kargs['num']:
+                text_color = 'k'
+                if 'text_color' in kargs:
+                    text_color = kargs['text_color']
+                    del kargs['text_color']
+                for i in range(len(X)):
+                    l = self.pixels.shape[1] - X[i] < 20
+                    ax.annotate(str(i), (X[i], Y[i]), ([
+                                                           5, -5][l], 0), textcoords='offset pixels', va="center",
+                                ha=["left", "right"][l], color=text_color)
+                del kargs['num']
+            ax.plot(X, Y, 'o', **kargs)
+        import scipy.interpolate
+        T = np.flipud(self.pixels) - np.min(self.pixels)
+        if Z is None:
+            Z = [T[Y[i], X[i]] for i in range(len(X))]
+        x = np.arange(self.pixels.shape[1])
+        y = np.arange(self.pixels.shape[0])
+        xx, yy = np.meshgrid(x, y)
+        I = scipy.interpolate.SmoothBivariateSpline(X, Y, Z)
+        z = I.ev(xx, yy)
+        if inline:
+            self.pixels -= z
+            return z
+        else:
+            if output == 'img':
+                New = copy.deepcopy(self)
+                New.pixels -= z
+                return New
+            elif output == 'spline':
+                return z
+            else:
+                raise ValueError(
+                    "The output parameter should be either 'img' or 'spline'")
+
+    def get_shadow_mask(self, angle, BIN=None, prog=False):
+        """
+        If an image is recorded with a beam incident with a certain angle, the topography will shadow the data.
+        This function generates the shadow mask for a given topography and a given incident angle.
+
+        Parameters
+        ----------
+        angle : float
+            The incidence angle in degrees
+        BIN : numpy array
+            Data. If given will move the recorded pixels at the correct x,y positions
+        prog : bool
+            display a progressbar ?
+
+        Note
+        ----
+        This function is old, might not be optimized or working properly
+        """
+        if BIN is not None:
+            BIN = BIN * 1.0
+        slope = np.tan(np.radians(angle))
+        neg = False
+        if slope < 0:
+            neg = True
+            slope = -slope
+            topo = np.fliplr(self.pixels)
+            if BIN is not None:
+                BIN = np.fliplr(BIN)
+        else:
+            topo = self.pixels
+        x = np.linspace(0, self.size['real']['x'], self.pixels.shape[1])
+        if self.size['real']['unit'] == 'um':
+            x *= 1e-6
+        elif self.size['real']['unit'] == 'nm':
+            x *= 1e-9
+        mask = np.zeros(self.pixels.shape)
+        AFM_bin_shadow = np.zeros(self.pixels.shape)
+        Y = range(self.pixels.shape[0])
+        if prog:
+            Y = PB(Y)
+        for yi in Y:
+            for xi in range(self.pixels.shape[1]):
+                cut = self.pixels.shape[1] - 2
+                y_ray = slope * (x - x[xi]) + topo[yi, xi]
+                while cut > xi and y_ray[cut] > topo[yi, cut]:
+                    cut -= 1
+                if xi == cut:
+                    if BIN is not None:
+                        AFM_bin_shadow[yi, xi] = BIN[yi, xi]
+                    continue
+                # Cut has been found
+                if BIN is not None:
+                    x1 = x[cut]
+                    x2 = x[cut + 1]
+                    y1 = topo[yi, cut]
+                    y2 = topo[yi, cut + 1]
+                    x0 = x[xi]
+                    y0 = topo[yi, xi]
+                    if y2 == y1:
+                        x_cut = (y1 + slope * x0 - y0) / slope
+                        y_cut = y1
+                    else:
+                        numerator = x1 / (x2 - x1) + (y0 - slope * x0 - y1) / (y2 - y1)
+                        denominator = 1 / (x2 - x1) - slope / (y2 - y1)
+                        x_cut = numerator / denominator
+                        y_cut = slope * (x_cut - x0) + y0
+                    if x_cut >= x1 and x_cut <= x2:
+                        y1 = BIN[yi, cut]
+                        y2 = BIN[yi, cut + 1]
+                        yint = (((y2 - y1) / (x2 - x1)) * (x_cut - x1)) + y1
+                    else:
+                        yint = BIN[yi, xi]
+                    AFM_bin_shadow[yi, xi] = yint
+                mask[yi, xi] = 1
+        if neg:
+            mask = np.fliplr(mask)
+            AFM_bin_shadow = np.fliplr(AFM_bin_shadow)
+        if BIN is not None:
+            return (mask, AFM_bin_shadow)
+        return mask
+
+    def adjust_position(self, fixed):
+        """
+        Shift the current pixels to match a fixed image.
+        The shift is determined by position where the cross-correlation is maximized.
+        """
+        adj = copy.deepcopy(self)
+        cor = np.fft.fft2(fixed.pixels)
+        cor = np.abs(np.fft.ifft2(np.conj(cor) * np.fft.fft2(self.pixels)))
+        cor = cor / fixed.pixels.size
+        ypeak, xpeak = np.unravel_index(cor.argmax(), cor.shape)
+        shift = [-(ypeak - 1), -(xpeak - 1)]
+        adj.pixels = np.roll(self.pixels, shift[0], axis=0)
+        adj.pixels = np.roll(adj.pixels, shift[1], axis=1)
+        return adj
+
+    def align(self, tform, cut=True):
+        """
+        Apply an Affine transform on the data
+
+        Parameters
+        ----------
+        tform : skimage.transform
+            the affine transform to perform
+        cut : bool
+            If True cut the data
+        """
+        New = copy.deepcopy(self)
+        New.pixels = tf.warp(self.pixels, tform, preserve_range=True)
+        if not cut:
+            return New
+        cut = [0, 0] + list(self.pixels.shape)
+        if tform.translation[0] >= 0:
+            cut[2] -= tform.translation[0]
+        elif tform.translation[0] < 0:
+            cut[0] -= tform.translation[0]
+        if tform.translation[1] >= 0:
+            cut[1] += tform.translation[1]
+        elif tform.translation[1] < 0:
+            cut[3] += tform.translation[1]
+        cut = [int(x) for x in cut]
+        New.cut(cut, inplace=True)
+        return New, cut
+
+    def get_fft(self):
+        """
+        return the FFT2 transform opf the image
+        """
+        return np.fft.fftshift(np.fft.fft2(self.pixels))
+
+    def corr_fit2d(self, nx=2, ny=1, poly=False, inline=True, mask=None):
+        """
+        Subtract a fitted 2D-polynom of nx and ny order from the data
+
+        Parameters
+        ----------
+        nx : int
+            the polynom order for the x-axis
+        ny : int
+            the polynom order for the y-axis
+        poly : bool
+            if True the polynom is returned as output
+        inline : bool
+            create a new object?
+        mask : 2D numpy array
+            mask where the fitting should be performed
+        """
+        r, z = fit2d(self.pixels, nx, ny, mask=mask)
+        if inline:
+            self.pixels -= z
+        else:
+            N = copy.deepcopy(self)
+            N.pixels -= z
+            if poly:
+                return N, z
+            return N
+        if poly:
+            return z
+        return self
+
+    def zero_min(self, inline=True):
+        """
+        Shift the values so that the minimum becomes zero.
+        """
+        if inline:
+            self.pixels -= np.min(self.pixels)
+            return self
+        else:
+            N = copy.deepcopy(self)
+            N.pixels -= np.min(N.pixels)
+            return N
+
+    def get_radius_mask_from_center(self, radius):
+        mask = np.zeros(self.pixels.shape, dtype=np.uint8)
+        rr, cc = disk(center=(self.pixels.shape[0] // 2, self.pixels.shape[1] // 2), radius=radius)
+        mask[rr, cc] = 1
+        return mask
+
+    def filter_lowpass(self, fft_radius, inline=True):
+        """
+        Execute a lowpass filter on the data
+        """
+        F = self.get_fft()
+        mask = self.get_radius_mask_from_center(radius=fft_radius)
+        if inline:
+            self.pixels = np.real(np.fft.ifft2(np.fft.fftshift(F * mask)))
+        else:
+            C = copy.deepcopy(self)
+            C.pixels = np.real(np.fft.ifft2(np.fft.fftshift(F * mask)))
+            return C
+
+    def filter_gaussian(self, sigma, inline=True, **kwargs):
+        """
+        Execute a gaussian filter on the data
+        """
+        if inline:
+            self.pixels = scipy.ndimage.gaussian_filter(self.pixels, sigma=sigma, **kwargs)
+        else:
+            C = copy.deepcopy(self)
+            C.pixels = scipy.ndimage.gaussian_filter(C.pixels, sigma=sigma, **kwargs)
+            return C
+
+    def filter_percentile(self, percentile, size, inline=True, **kwargs):
+        """
+        Execute a percentile filter on the data
+        """
+        if inline:
+            self.pixels = scipy.ndimage.percentile_filter(self.pixels, percentile=percentile, size=size, **kwargs)
+        else:
+            C = copy.deepcopy(self)
+            C.pixels = scipy.ndimage.percentile_filter(C.pixels, percentile=percentile, size=size, **kwargs)
+            return C
+
+    def _resize_infos(self):
+        """
+        Internal to recalculate the real size when the image is cropped or cut
+        """
+        self.size['real']['x'] *= self.pixels.shape[1] / self.size['pixels']['x']
+        self.size['real']['y'] *= self.pixels.shape[0] / self.size['pixels']['y']
+        self.size['pixels']['x'] = int(self.pixels.shape[1])
+        self.size['pixels']['y'] = int(self.pixels.shape[0])
+        if 'recorded' in self.size:
+            self.size['recorded']['real']['x'] \
+                *= (self.pixels.shape[1] / self.size['pixels']['x'])
+            self.size['recorded']['real']['y'] \
+                *= (self.pixels.shape[0] / self.size['pixels']['y'])
+            self.size['recorded']['pixels']['x'] = int(self.pixels.shape[1])
+            self.size['recorded']['pixels']['y'] = int(self.pixels.shape[0])
+
+    def filter_scars_removal(self, thresh=.5, inline=True):
+        """
+        Filter function to remove scars from images.
+        """
+        if not inline:
+            C = copy.deepcopy(self)
+        else:
+            C = self
+        for y in range(1, self.pixels.shape[0] - 1):
+            b = self.pixels[y - 1, :]
+            c = self.pixels[y, :]
+            a = self.pixels[y + 1, :]
+            mask = np.abs(b - a) < thresh * (np.abs(c - a))
+            C.pixels[y, mask] = b[mask]
+        if not inline:
+            return C
+        return self
+
+    def cut(self, c, inline=False, pixels=True, **kargs):
+        """
+        Clip/Crop the image
+
+        Parameters
+        ----------
+        c : list [llx,lly,urx,ury]
+            list of the lowe-left (ll) and upper-right (ur) coordinates
+        inline: bool
+            perform the transformation inline or produce a new SPM_image?
+        pixels : bool
+            Are the coordinates given in pixels?
+
+        Returns
+        -------
+        self if inplace, clipped SPM_image otherwises2 = pySPM.Nanoscan("%s/CyI5b_PCB_ns.xml"%(Path))
+        """
+        if 'inplace' in kargs:
+            inline = kargs['inplace']
+        if kargs.get('debug', False):
+            print("cut) Input coordinates:", c)
+        if not pixels:
+            c = [z for s in zip(*self.real2pixels(c[0::2], c[1::2])) for z in s]
+            if kargs.get('debug', False):
+                print("cut) pixel coordinates:", c)
+        if not inline:
+            new = copy.deepcopy(self)
+            new.pixels = cut(self.pixels, c, **kargs)
+            new._resize_infos()
+            return new
+        else:
+            self.pixels = cut(self.pixels, c, **kargs)
+            self._resize_infos()
+            return self
+
+    def zoom(self, zoom_factor, inplace=False, order=3):
+        """
+        Resize the image to a new pixel size (but keep the real size) by pixel interpolation.
+
+        Parameters
+        ----------
+        zoom_factor : float
+            > 1: up sampling
+            < 1: down sampling
+        order : int
+            The spline interpolation order to use. (default: 3). Use 0 for binary or very sharp images.
+        inplace : bool
+            create a new image?
+        """
+        from scipy.ndimage.interpolation import zoom
+        if not inplace:
+            new = copy.deepcopy(self)
+            new.pixels = zoom(new.pixels, zoom_factor, order=order)
+            new.size['pixels']['x'] = new.pixels.shape[1]
+            new.size['pixels']['y'] = new.pixels.shape[0]
+            return new
+        else:
+            self.pixels = zoom(self.pixels, zoom_factor, order=order)
+            self.size['pixels']['x'] = self.pixels.shape[1]
+            self.size['pixels']['y'] = self.pixels.shape[0]
+            return self
+
+
+# Note: The following functions are not part of the SPM_image class.
+# All following functions are performed on numpy arrays
+
+def cut(img, c, **kargs):
+    """
+    Clip / Crop a numpy array
+
+    Parameters
+    ----------
+    img : 2D numpy array
+        The input image array
+    c : list [llx, lly, urx, ury]
+        the lower-left (ll) and upper-right (ur) coordinates used for the cropping
+    """
+    from .utils.geometry import Bbox
+    if kargs.get('debug', False):
+        print("cut in x", c[0], "->", c[2], " - in y", c[1], "->", c[3])
+    if isinstance(c, Bbox):
+        c = [c.left, c.bottom, c.right, c.top]
+    if c[3] < c[1]:
+        c = [c[0], c[3], c[2], c[1]]
+    if c[2] < c[0]:
+        c = [c[2], c[1], c[0], c[3]]
+    if c[2] - c[0] == img.shape[1] and c[3] - c[1] == img.shape[0]:
+        raise Exception("Reshaping the same array again?")
+    return img[c[1]:c[3], c[0]:c[2]]
+
+
+def normalize(data, sig=None, vmin=None, vmax=None):
+    """
+    Normalize the input data. Minimum_value -> 0 and maximum_value -> 1
+
+    Parameters
+    ----------
+    data : numpy array
+        input data
+    sig : float or None
+        if not None:
+            mean(data)-sig*standard_deviation(data) -> 0
+            mean(data)+sig*standard_deviation(data) -> 1
+    vmin : float or None
+        if not None, define the lower bound i.e.  vmin -> 0
+    vmax : float or None
+        if not None, defines the upper bound i.e. vmax -> 0
+
+    Note
+    ----
+    All values below the lower bound will be = 0
+    and all values above the upper bound will be = 1
+
+
+    """
+    if sig is None:
+        mi = np.min(data)
+        ma = np.max(data)
+    else:
+        s = sig * np.std(data)
+        mi = np.mean(data) - s
+        ma = np.mean(data) + s
+    if vmin is not None:
+        mi = vmin
+    if vmax is not None:
+        ma = vmax
+    N = (data - mi) / (ma - mi)
+    N[N < 0] = 0
+    N[N > 1] = 1
+    return N
+
+
+def imshow_sig(img, sig=1, ax=None, **kargs):
+    """
+    Shortcut to plot a numpy array around it's mean with bounds ±sig sigmas
+
+    Parameters
+    ----------
+    img : 2D numpy array
+        input image to display
+    sig : float
+        The number of standard-deviation to plot
+    ax : matplotlib axis
+        matplotlib axis to use. If None, the current axis (plt.gca() will be used).
+    **kargs : additional parameters
+        will be passed to the imshow function of matplotls2 = pySPM.Nanoscan("%s/CyI5b_PCB_ns.xml"%(Path))ib
+    """
+    if ax == None:
+        fig, ax = plt.subplots(1, 1)
+    std = np.std(img)
+    avg = np.mean(img)
+    vmin = avg - sig * std
+    vmax = avg + sig * std
+    ax.imshow(img, vmin=vmin, vmax=vmax, **kargs)
+
+
+def adjust_position(fixed, to_adjust, shift=False):
+    """ Shift the current pixels to match a fixed image by rolling the data"""
+    adj = copy.deepcopy(to_adjust)
+    cor = np.fft.fft2(fixed)
+    cor = np.abs(np.fft.ifft2(np.conj(cor) * np.fft.fft2(to_adjust)))
+    cor = cor / to_adjust.size
+    ypeak, xpeak = np.unravel_index(cor.argmax(), cor.shape)
+    shift = [-(ypeak - 1), -(xpeak - 1)]
+    adj = np.roll(to_adjust, shift[0], axis=0)
+    adj = np.roll(adj, shift[1], axis=1)
+    if shift:
+        return adj, shift
+    return adj
+
+
+def tukeyfy(A, alpha, type='default'):
+    """
+    Apply a Tukey window on the current image
+
+    Parameters
+    ----------
+    A : 2D numpy array
+        input array
+    alpha : float
+        Size of the Tukey windows in percent of the image (≥0 and ≤1)
+    type : string
+        if not "default" perform a mean centering (data will blend down to its mean instead of 0)
+    """
+    tuky = tukeywin(A.shape[0], alpha)
+    tukx = tukeywin(A.shape[1], alpha)
+    tuk = np.multiply(tukx[:, None].T, tuky[:, None])
+    if type == 'default':
+        return A * tuk
+    avg = np.mean(A)
+    return avg + (A - avg) * tuk
+
+
+def tukeywin(window_length, alpha=0.5):
+    '''The Tukey window, also known as the tapered cosine window, can be regarded as a cosine lobe of width \alpha * N / 2
+    that is convolved with a rectangle window of width (1 - \alpha / 2). At \alpha = 1 it becomes rectangular, and
+    at \alpha = 0 it becomes a Hann window.
+
+    We use the same reference as MATLAB to provide the same results in case users compare a MATLAB output to this function
+    output
+
+    Reference
+    ---------
+    http://www.mathworks.com/access/helpdesk/help/toolbox/signal/tukeywin.html
+
+    '''
+    # Special cases
+    if alpha <= 0:
+        return np.ones(window_length)  # rectangular window
+    elif alpha >= 1:
+        return np.hanning(window_length)
+
+    # Normal case
+    x = np.linspace(0, 1, window_length)
+    w = np.ones(x.shape)
+
+    # first condition 0 <= x < alpha/2
+    first_condition = x < alpha / 2
+    w[first_condition] = 0.5 * \
+                         (1 + np.cos(2 * np.pi / alpha * (x[first_condition] - alpha / 2)))
+
+    # second condition already taken care of
+
+    # third condition 1 - alpha / 2 <= x <= 1
+    third_condition = x >= (1 - alpha / 2)
+    w[third_condition] = 0.5 * \
+                         (1 + np.cos(2 * np.pi / alpha * (x[third_condition] - 1 + alpha / 2)))
+    return w
+
+
+def overlay(ax, mask, color, **kargs):
+    """
+    Plot an overlay on an existing axis
+
+    Parameters
+    ----------
+    ax : matplotlib axis
+        input axis
+    mask : 2D numpy array
+        Binary array where a mask should be plotted
+    color : string
+        The color of the mask to  plot
+    **kargs: additional parameters
+        passed to the imshow function of matploltib
+    """
+    m = np.ma.masked_array(mask, ~mask)
+    col = np.array(mpl.colors.colorConverter.to_rgba(color))
+    I = col[:, None, None].T * m[:, :, None]
+    ax.imshow(I, **kargs)
+
+
+def normP(x, p, trunk=True):
+    """
+    Normalize the input data accroding to its percentile value.
+
+    Parameters
+    ----------
+    x : 2D numpy array
+        input data
+    p : float
+        percentile to normalize the data.
+        lower bound = p percentile
+        upper bound = (100-p) percentile
+    trunk : bool
+        If True the data are truncated between 0 and 1
+    """
+    thresh_high = np.percentile(x, 100 - p)
+    thresh_low = np.percentile(x, p)
+    if thresh_low == thresh_high:
+        thresh_high = np.max(x)
+        thresh_low = np.min(x)
+    if thresh_low == thresh_high:
+        thresh_high = thresh_low + 1
+    r = (x - thresh_low) / (thresh_high - thresh_low)
+    if trunk:
+        r[r < 0] = 0
+        r[r > 1] = 1
+    return r
+
+
+def beam_profile(target, source, mu=1e-6, tukey=0, meanCorr=False, source_tukey=None, real=np.abs, **kargs):
+    """
+    Calculate the PSF by deconvolution of the target
+    with the source using a Tikhonov regularization of factor mu.
+    """
+    if source_tukey is None:
+        source_tukey = tukey
+    if kargs.get('source_centering', False):
+        source = 2 * source - 1
+    if meanCorr:
+        target = target - np.mean(target)
+    if tukey > 0:
+        target = tukeyfy(target, tukey)
+    if source_tukey > 0:
+        source = tukeyfy(source, tukey)
+    tf = np.fft.fft2(source)
+    tf /= np.size(tf)
+    recon_tf = np.conj(tf) / (np.abs(tf) ** 2 + mu)
+    return np.fft.fftshift(real(np.fft.ifft2(np.fft.fft2(target) * recon_tf))) / np.size(target)
+
+
+def beam_profile1d(target, source, mu=1e-6, real=np.abs):
+    source = source
+    tf = np.fft.fft(source)
+    tf /= np.size(tf)
+    recon_tf = np.conj(tf) / (np.abs(tf) ** 2 + mu)
+    F = np.fft.fft(target) * recon_tf
+    return np.fft.fftshift(real(np.fft.ifft(F))), F
+
+
+def zoom_center(img, sx, sy=None):
+    """
+    Zoom by taking the sx × sy central pixels
+
+    Parameters
+    ----------
+    img : 2D numpy array
+        The input data
+    sx : int
+        The number of pixels along the x-axis to take
+
+    sy : int or None
+        The number of pixels alongs the y-axis to take.
+        If None take the same value as for sx
+    """
+    if sy is None:
+        sy = sx
+    assert type(sx) is int
+    assert type(sy) is int
+    return img[
+           img.shape[0] // 2 - sy // 2: img.shape[0] // 2 + sy // 2,
+           img.shape[1] // 2 - sx // 2: img.shape[1] // 2 + sx // 2]
+
+
+def px2real(x, y, size, ext):
+    rx = ext[0] + (x / size[1]) * (ext[1] - ext[0])
+    ry = ext[2] + (y / size[0]) * (ext[3] - ext[2])
+    return rx, ry
+
+
+def real2px(x, y, size, ext):
+    px = size[1] * (x - ext[0]) / (ext[1] - ext[0])
+    py = size[0] * (y - ext[2]) / (ext[3] - ext[2])
+    return px, py
+
+
+def fit2d(Z0, dx=2, dy=1, mask=None):
+    """
+    Fit the input data with a 2D polynom of order dx × dy
+
+    Parameters
+    ----------
+    Z0 : 2D numpy array
+        input data
+    dx : int
+        order of the polynom for the x-axis
+    dy : int
+        order of the polynom for the y-xis
+    mask : 2D numpy array
+        Give a mask where True values only will be used to perform the fitting
+
+    Returns
+    -------
+    numpy array
+        fitting parameters
+    2D numpy array
+        result of the polynom
+    """
+    x = np.arange(Z0.shape[1], dtype=float)
+    y = np.arange(Z0.shape[0], dtype=float)
+    X0, Y0 = np.meshgrid(x, y)
+    if mask is not None:
+        X = X0[mask]
+        Y = Y0[mask]
+        Z = Z0[mask]
+    else:
+        X = X0
+        Y = Y0
+        Z = Z0
+    x2 = X.ravel()
+    y2 = Y.ravel()
+    A = np.vstack([x2 ** i for i in range(dx + 1)])
+    A = np.vstack([A] + [y2 ** i for i in range(1, dy + 1)])
+    res = scipy.optimize.lsq_linear(A.T, Z.ravel())
+    r = res['x']
+    Z2 = r[0] * np.ones(Z0.shape)
+    for i in range(1, dx + 1):
+        Z2 += r[i] * (X0 ** i)
+    for i in range(1, dy + 1):
+        Z2 += r[dx + i] * (Y0 ** i)
+    return r, Z2
+
+
+def warp_and_cut(img, tform, cut=True):
+    """
+    Perform an Affine transform on the input data and cut them if cut=True
+
+    Parameters
+    ----------
+    img : 2D numpy array
+        input data
+    tform : skimage.transform
+        An Affine fransform to perform on the data
+    cut : bool
+        Should the data be cutted?
+    """
+    New = tf.warp(img, tform, preserve_range=True)
+    Cut = [0, 0] + list(img.shape)
+    if tform.translation[0] >= 0:
+        Cut[2] -= tform.translation[0]
+    elif tform.translation[0] < 0:
+        Cut[0] -= tform.translation[0]
+    if tform.translation[1] >= 0:
+        Cut[1] += tform.translation[1]
+    elif tform.translation[1] < 0:
+        Cut[3] += tform.translation[1]
+    Cut = [int(x) for x in Cut]
+    if cut:
+        New = cut(New, Cut)
+    return New, Cut
+
+
+def get_profile(I, x1, y1, x2, y2, width=0, ax=None, color='w', alpha=0, N=None, \
+                transx=lambda x: x, transy=lambda x: x, interp_order=1, **kargs):
+    """
+    Get a profile from an input matrix.
+    Low-level function. Doc will come laters2 = pySPM.Nanoscan("%s/CyI5b_PCB_ns.xml"%(Path))
+    """
+    d = np.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2)
+    if N is None:
+        N = int(d) + 1
+    P = []
+    dx = -width / 2 * (y2 - y1) / d
+    dy = width / 2 * (x2 - x1) / d
+    for w in np.linspace(-width / 2, width / 2, max(1, width)):
+        dx = -w * (y2 - y1) / d
+        dy = w * (x2 - x1) / d
+        x = np.linspace(x1 + dx, x2 + dx, N)
+        y = np.linspace(y1 + dy, y2 + dy, N)
+        M = scipy.ndimage.interpolation.map_coordinates(I, np.vstack((y, x)), order=interp_order)
+        P.append(M)
+    if kargs.get('debug', False):
+        print("get_profile input coordinates:", x1, y1, x2, y2)
+    if not ax is None:
+        x1 = transx(x1)
+        x2 = transx(x2)
+        y1 = transy(y1)
+        y2 = transy(y2)
+        if kargs.get('debug', False):
+            print("Drawing coordinates:", x1, y1, x2, y2)
+        dx = -width / 2 * (y2 - y1) / d
+        dy = width / 2 * (x2 - x1) / d
+        if type(color) in [tuple, list]:
+            ax.plot([x1, x2], [y1, y2], color=color, alpha=kargs.get('linealpha', 1),
+                    linestyle=kargs.get("linestyle", "-"))
+            ax.plot([x1 - dx, x1 + dx], [y1 - dy, y1 + dy], color=color, alpha=kargs.get('linealpha', 1))
+            ax.plot([x2 - dx, x2 + dx], [y2 - dy, y2 + dy], color=color, alpha=kargs.get('linealpha', 1))
+        else:
+            ax.plot([x1, x2], [y1, y2], color, alpha=kargs.get('linealpha', 1), lw=kargs.get('lw', 1),
+                    linestyle=kargs.get("linestyle", "-"))
+            ax.plot([x1 - dx, x1 + dx], [y1 - dy, y1 + dy], color, alpha=kargs.get('linealpha', 1))
+            ax.plot([x2 - dx, x2 + dx], [y2 - dy, y2 + dy], color, alpha=kargs.get('linealpha', 1))
+        if alpha > 0:
+            import matplotlib.patches
+            ax.add_patch(matplotlib.patches.Rectangle(
+                (x1 + dx, y1 + dy),
+                2 * np.sqrt(dx ** 2 + dy ** 2),
+                np.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2),
+                -np.degrees(np.arctan2(x2 - x1, y2 - y1)), color=color, alpha=alpha))
+    if len(P) == 1:
+        return np.linspace(0, d, N), P[0]
+    return np.linspace(0, d, N), np.vstack(P).T
+
+
+def dist_v2(img, dx=1, dy=1):
+    """
+    Return a 2D array with the distance in pixel with the clothest corner of the array.
+    """
+    x2 = np.arange(img.shape[1])
+    x2 = (np.minimum(x2, img.shape[1] - x2) * dx) ** 2
+    y2 = np.arange(img.shape[0])
+    y2 = (np.minimum(y2, img.shape[0] - y2) * dy) ** 2
+    X, Y = np.meshgrid(x2, y2)
+    return np.sqrt(X + Y)
+
+
+def generate_k_matrices(A, dx, dy):
+    """
+    GENERATE_K_MATRICES k-Matrix generation (helper function).
+    generates k-matrices for the 2D-channel CHANNEL.
+   
+    K is a matrix of the same size as the pixel matrix A, containing the real-life frequency distance of each 
+    pixel position to the nearest corner of an matrix that is one pixel
+    wider/higher.
+    KX is of the same size as K and contains the real-life  difference in x-direction of each pixel position to the nearest corner 
+    of a matrix that is one pixel wider/higher.
+    Similarly, KY is of the  same size as K, containing the real-life difference in y-direction of  each pixel position to the nearest corner of an matrix that is one 
+    pixel wider/higher.
+    """
+    ny, nx = A.shape
+    dkx = 2 * np.pi / (nx * dx)
+    dky = 2 * np.pi / (ny * dy)
+
+    ky = np.arange(0, ny);
+    ky = (np.mod(ky + ny / 2, ny) - ny / 2) * dky
+
+    kx = np.arange(0, nx);
+    kx = (np.mod(kx + nx / 2, nx) - nx / 2) * dkx
+
+    kx, ky = np.meshgrid(kx, ky)
+    k = dist_v2(A, dkx, dky)
+    k[0, 0] = 1.0  # Prevent division by zero error and illegal operand errors. This may be improved...
+    return k, kx, ky
+
+
+def mfm_tf(nx, dx, ny, dy, tf_in, derivative=0, transform=0, z=0, A=0, theta=None, phi=None, d=None, delta_w=None):
+    """
+    Draft for the MFM tf function
+    """
+    k, kx, ky = generate_k_matrices(tf_in, dx, dy)
+    # Distance loss
+    tf_out = np.exp(-z * k)
+    if d is not None:
+        tf_out = tf_out / 2.0
+        if not np.isinf(d):
+            if d == 0:
+                tf_out *= k
+            else:
+                tf_out *= 1 - np.exp(-d * k)
+    if A == 0:
+        if transform != 0:
+            assert theta is not None
+            assert phi is not None
+            tf_out *= ((np.cos(theta) + 1j * (
+                    np.cos(phi) * np.sin(-theta) * kx + np.sin(phi) * np.sin(-theta) * ky)) / k) ** transform
+        if derivative == 1:
+            tf_out *= k
+    else:
+        pass  # TODO
+    return tf_out * tf_in
+
+
+def mfm_inv_calc_flat(img, z, tf_in, thickness=None, delta_w=None, amplitude=0, derivative=0, transform=0, mu=1e-8):
+    """
+    MFM inv calc function
+    """
+    theta = np.radians(12)
+    phi = np.radians(-90)
+    ny, nx = img.shape
+    tf = mfm_tf(nx, 1, ny, 1, tf_in, derivative, transform, z, amplitude, theta, phi, thickness, delta_w)
+    tf[0, 0] = np.real(np.mean(tf))
+    recon_tf = np.conj(tf) / (mu + np.abs(tf) ** 2)
+    work_img = np.abs(np.fft.ifft2(np.fft.fft2(img) * recon_tf))
+    return work_img
+
+
+def get_tik_tf(Img, mu, tukey=0, source_tukey=0, debug=False, d=200, real=np.real):
+    import scipy
+    def fit(x, a, A, bg, x0):
+        return bg + (A - bg) * np.exp(-abs(x - x0) / a)
+
+    x = np.arange(Img.shape[1])
+    y = np.arange(Img.shape[0])
+    X, Y = np.meshgrid(x, y)
+    x0 = Img.shape[1] / 2
+    y0 = Img.shape[0] / 2
+    R = np.sqrt((X - x0) ** 2 + (Y - y0) ** 2)
+
+    Z = beam_profile(Img, Img, mu=mu, tukey=tukey, source_tukey=source_tukey, real=real)
+    zoom = zoom_center(Z, d)
+    P = zoom[zoom.shape[0] // 2, :]
+    p0 = (1, np.max(zoom), 0, len(P) / 2)
+    popt, pcov = scipy.optimize.curve_fit(fit, np.arange(len(P)), P, p0, bounds=((0, 0, -np.inf, 0), np.inf))
+    bg = popt[2]
+    a = popt[0]
+    if debug:
+        return bg + np.exp(-np.abs(R) / a), Z, p0, popt
+    return bg + np.exp(-np.abs(R) / a)
```

### Comparing `pySPM-0.2.9/pySPM/SXM.py` & `pyspm-0.3.0/pySPM/SXM.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,79 +3,88 @@
 # Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
 
 """
 This module handle sxm file format used by Nanonis instruments
 """
 
 import os
-# -- coding: utf-8 --
-
-# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
-
 import struct
+
 import numpy as np
+
 from .SPM import SPM_image
 
+
+# -- coding: utf-8 --
+# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
+
+
 class SXM:
     def __init__(self, filename):
         self.filename = filename
         assert os.path.exists(self.filename)
         self.f = open(self.filename, 'rb')
         l = ''
         key = ''
         self.header = {}
-        while l!=b':SCANIT_END:':
+        while l != b':SCANIT_END:':
             l = self.f.readline().rstrip()
-            if l[:1]==b':':
+            if l[:1] == b':':
                 key = l.split(b':')[1].decode('ascii')
                 self.header[key] = []
             else:
-                if l: # remove empty lines
+                if l:  # remove empty lines
                     self.header[key].append(l.decode('ascii').split())
-        while self.f.read(1)!=b'\x1a':
+        while self.f.read(1) != b'\x1a':
             pass
-        assert self.f.read(1)==b'\x04'
-        assert self.header['SCANIT_TYPE'][0][0] in ['FLOAT','INT','UINT','DOUBLE']
+        assert self.f.read(1) == b'\x04'
+        assert self.header['SCANIT_TYPE'][0][0] in ['FLOAT', 'INT', 'UINT', 'DOUBLE']
         self.data_offset = self.f.tell()
+        self.f.close()
         self.size = dict(pixels={
-                'x': int(self.header['SCAN_PIXELS'][0][0]),
-                'y': int(self.header['SCAN_PIXELS'][0][1])
-            },real={
-                'x': float(self.header['SCAN_RANGE'][0][0]),
-                'y': float(self.header['SCAN_RANGE'][0][1]),
-                'unit': 'm'
-            })
+            'x': int(self.header['SCAN_PIXELS'][0][0]),
+            'y': int(self.header['SCAN_PIXELS'][0][1])
+        }, real={
+            'x': float(self.header['SCAN_RANGE'][0][0]),
+            'y': float(self.header['SCAN_RANGE'][0][1]),
+            'unit': 'm'
+        })
 
     def list_channels(self):
         print("Channels")
         print("========")
         h = self.header['DATA_INFO'][0]
         i = h.index('Name')
         for z in self.header['DATA_INFO'][1:]:
-            print("  - "+z[i])
+            print("  - " + z[i])
 
-    def get_channel(self, name, direction='forward',corr=None):
+    def get_channel(self, name, direction='forward', corr=None):
         chID = 0
         zscale = ''
         for x in self.header['DATA_INFO'][1:]:
-            if x[1]==name:
-                if x[3]=='both' and direction=='backward':
+            if x[1] == name:
+                if x[3] == 'both' and direction == 'backward':
                     chID += 1
-                if x[3]== 'both' or direction == x[3]:
+                if x[3] == 'both' or direction == x[3]:
                     break
                 return None
                 zscale = x[2]
             elif x[3] == 'both':
                 chID += 2
             else:
                 chID += 1
-                    
-        size = self.size['pixels']['x']*self.size['pixels']['y']
-        self.f.seek(self.data_offset+chID*size*4)
-        data = np.array(struct.unpack('<>'['MSBFIRST'==self.header['SCANIT_TYPE'][0][1]]+str(size)+{'FLOAT':'f','INT':'i','UINT':'I','DOUBLE':'d'}[self.header['SCANIT_TYPE'][0][0]],self.f.read(4*size))).reshape((self.size['pixels']['y'],self.size['pixels']['x']))
+
+        size = self.size['pixels']['x'] * self.size['pixels']['y']
+        self.f = open(self.filename, 'rb')
+        self.f.seek(self.data_offset + chID * size * 4)
+        data = np.array(struct.unpack('<>'['MSBFIRST' == self.header['SCANIT_TYPE'][0][1]] + str(size) +
+                                      {'FLOAT': 'f', 'INT': 'i', 'UINT': 'I', 'DOUBLE': 'd'}[
+                                          self.header['SCANIT_TYPE'][0][0]], self.f.read(4 * size))).reshape(
+            (self.size['pixels']['y'], self.size['pixels']['x']))
+        self.f.close()
         return SPM_image(
             channel=name,
             BIN=data,
             real=self.size['real'],
-            _type = 'Nanonis SXM',
-            zscale = zscale,
+            _type='Nanonis SXM',
+            zscale=zscale,
             corr=corr)
```

### Comparing `pySPM-0.2.9/pySPM/ToF.py` & `pyspm-0.3.0/pySPM/ToF.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,228 +1,231 @@
-# -- coding: utf-8 --
-
-# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
-
-"""
-This is an old module which is deprecated now. It is kept in the project as it can be used to read BIF6 and BIF3D images.
-"""
-
-import numpy as np
-import struct
-import os
-import re
-import matplotlib.pyplot as plt
-import pySPM
-
-Elements = {
-    'H': {1: (1.00782503223, .999885), 2: (2.01410177812, .000115)},
-    'Li': {6: (6.0151228874, .0759), 7: (7.0160034366, .9241)},
-    'Be': {9: (9.012183065, 1)},
-    'B': {10: (10.01293695, .199), 11: (11.00930536, .801)},
-    'C': {12: (12, .9893), 13: (13.00335483507, .01107)},
-    'N': {14: (14.00307400443, .99636), 15: (15.00010889888, .00364)},
-    'O': {16: (15.99491461957, .99757), 17: (16.99913175650, .00038), 18: (17.99915961286, .00205)},
-    'F': {19: (18.9984036273, 1)},
-    'Ag': {107: (106.9050916, .51839), 109: (108.9047553, .48161)},
-    'Au': {197: (196.96656879, 1)},
-    'Si': {28: (27.97692653465, .92223), 29: (28.97649466490, .04685), 30: (29.973770136, 0.3092)},
-    'Ti': {46: (45.95262772, .0825), 47: (46.95175879, 0.0744), 48: (47.94794198, .7372), 49: (48.94786568, .0541), 50: (49.94478689, .0518)},
-}
-
-
-def getSpecElt(Elts):
-    if len(Elts) == 1:
-        return Elements[Elts[0]]
-    tm = {}
-    r1 = Elements[Elts[0]]
-    r2 = getSpecElt(Elts[1:])
-    for x in r1:
-        for y in r2:
-            if x+y not in tm:
-                tm[x+y] = [r1[x][0]+r2[y][0], r1[x][1]*r2[y][1]]
-            else:
-                tm[x+y][1] += r1[x][1]*r2[y][1]
-    return tm
-
-
-def SplitElts(elt):
-    elts = []
-    for x, i in re.findall('([A-Z][a-z]?)([0-9]*)', elt):
-        if i == '':
-            i = 1
-        else:
-            i = int(i)
-        elts += [x for k in range(i)]
-    return elts
-
-
-def showElts(Elts):
-    r = getSpecElt(Elts)
-    plt.bar(r.keys(), [z[1] for z in r.values()])
-    plt.show()
-
-
-class BIF6:
-    def __init__(self, filename):
-        self.f = open(filename, 'rb')
-        self.header = struct.unpack('xx4s5H', self.f.read(16))
-        self.size = (self.header[2], self.header[3])
-        self.N = self.size[0]*self.size[1]
-        self.cat = []
-        for i in range(self.header[1]):
-            self.f.seek(16+i*(4*self.N+16))
-            self.cat.append(struct.unpack('4f', self.f.read(16)))
-
-    def getImgID(self, ID):
-        assert ID >= 0 and ID <= self.header[1]
-        self.f.seek(32+ID*(4*self.N+16))
-        return np.array(struct.unpack(str(self.N)+'I', self.f.read(4*self.N))).reshape(self.size)
-
-    def getImgMass(self, masses, raw=False):
-        if type(masses)is float or type(masses) is int:
-            masses = [masses]
-        SUM = None
-        for i, x in enumerate(self.cat):
-            for m in masses:
-                if m >= x[0]-.5 and m <= x[1]+.5:
-                    if SUM is None:
-                        SUM = self.getImgID(i)
-                    else:
-                        SUM += self.getImgID(i)
-        if raw:
-            return SUM
-        if SUM is None:
-            return None
-        return pySPM.SPM_image(np.flipud(SUM))
-
-    def getImgElt(self, elt):
-        r = {}
-        A = getSpecElt(SplitElts(elt))
-        for k in A:
-            I = self.getImgMass(k)
-            if I is not None:
-                r[k] = {
-                    'data': I,
-                    'mass': A[k][0],
-                    'abund': A[k][1]}
-        return r
-
-    def showImgElt(self, elt, size=10, abundCorr=False, tot=True):
-        A = self.getImgElt(elt)
-        ks = [z for z in A if A[z]['data'] != None]
-        fig, ax = plt.subplots((len(ks)+1)//4+1, 4,
-                               figsize=(10*((len(ks)+1)//4+1), 10))
-        mi = np.min(A[ks[0]]['data'].pixels)
-        ma = np.max(A[ks[0]]['data'].pixels)
-        A[ks[0]]['CT'] = ma
-        for i, k in enumerate(ks[1:]):
-            M = np.min(A[k]['data'].pixels)
-            mi = min(mi, M)
-            A[k]['minCT'] = M
-            M = np.max(A[k]['data'].pixels)
-            ma = max(ma, M)
-            A[k]['CT'] = M
-        ks.sort()
-        di = 0
-        if tot:
-            SUM = sum([A[k]['data'].pixels for k in ks])
-            ax[0][0].imshow(SUM, vmin=0)
-            ax[0][0].set_title("Total")
-            di = 1
-        for i, k in enumerate(ks):
-            if abundCorr:
-                ax[(i+di)//4][(i+di) % 4].imshow(A[k]
-                                                 ['data'].pixels/A[k]['abund'], vmin=0, vmax=ma)
-            else:
-                A[k]['data'].show(ax=ax[(i+di)//4][(i+di) %
-                                                   4], vmin=0, vmax=ma)
-            ax[(i+di)//4][(i+di) % 4].set_title(
-                'mass: {mass:.3} - abundancy: {abund:.3f} - CT: {CT}'.format(**A[k]))
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        self.f.close()
-
-
-class BIF3D:
-
-    def __init__(self, path):
-        self.Peaks = {}
-        self.RPeaks = {}
-        self.Path = os.path.dirname(path)
-        self.Basename = os.path.basename(path)
-        self.size = None
-        for x in os.listdir(self.Path):
-            if x[:len(self.Basename)] == self.Basename:
-                if x[-6:] == ".BIF3D":
-                    s = self.Basename+r' \(([0-9]+)\)(?: - (.*?))?\.BIF3D'
-                    r = re.search(s, x)
-                    ID = int(r.group(1))
-                    self.Peaks[ID] = r.group(2)
-                    if r.group(2) != None:
-                        self.RPeaks[r.group(2)] = ID
-        self.data = {}
-
-    def getIDs(self, channels):
-        assert type(channels) in [str, int, list, tuple]
-        if type(channels) == int:
-            return channels
-        if type(channels) == str:
-            assert channels in self.RPeaks.keys()
-            return self.RPeaks[channels]
-        if type(channels) == list or type(channels) == tuple:
-            ID = []
-            for x in channels:
-                ID.append(self.getIDs(x))
-            return ID
-
-    def getChannel(self, channel):
-        k = self.getIDs(channel)
-        if k in self.data:
-            return self.data[k]
-        v = self.Peaks[k]
-        if v != None:
-            path = '{path}{sep}{basename} ({ID}) - {Peak}.BIF3D'
-        else:
-            path = '{path}{sep}{basename} ({ID}).BIF3D'
-        f = open(path.format(path=self.Path, sep=os.sep,
-                             basename=self.Basename, ID=k, Peak=v), 'rb')
-        A = f.read()
-        f.close()
-        size = struct.unpack("II", A[32:40])
-        if self.size == None:
-            self.size = size
-        else:
-            assert self.size == size
-        return np.array(struct.unpack("{0}d".format(self.size[0]*self.size[1]), A[640:])).reshape(self.size)
-
-    def loadChannel(self, channel):
-        k = self.getIDs(channel)
-        if not k in self.data:
-            self.data[k] = self.getChannel(channel)
-
-    def loadChannels(self, channels):
-        if not type(channels) in [list, tuple]:
-            self.loadChannel(channels)
-        else:
-            for x in channels:
-                self.loadChannel(x)
-
-    def getChannels(self, *channels):
-        k = self.getIDs(channels)
-        self.loadChannels(k)
-        if type(k) == int:
-            return self.data[k]
-        D = np.zeros(self.size)
-        for x in k:
-            D += self.data[x]
-        return D
-
-    def listChannels(self):
-        return self.Peaks
-
-    def show(self, ax, *channels):
-        D = self.getChannels(*channels)
-        ax.imshow(D)
-        if len(channels) > 1:
-            ax.set_title(','.join([str(z) for z in channels]))
-        else:
-            ax.set_title(str(channels[0]))
+# -- coding: utf-8 --
+
+# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
+
+"""
+This is an old module which is deprecated now. It is kept in the project as it can be used to read BIF6 and BIF3D images.
+"""
+
+import os
+import re
+import struct
+
+import matplotlib.pyplot as plt
+import numpy as np
+
+import pySPM
+
+Elements = {
+    'H': {1: (1.00782503223, .999885), 2: (2.01410177812, .000115)},
+    'Li': {6: (6.0151228874, .0759), 7: (7.0160034366, .9241)},
+    'Be': {9: (9.012183065, 1)},
+    'B': {10: (10.01293695, .199), 11: (11.00930536, .801)},
+    'C': {12: (12, .9893), 13: (13.00335483507, .01107)},
+    'N': {14: (14.00307400443, .99636), 15: (15.00010889888, .00364)},
+    'O': {16: (15.99491461957, .99757), 17: (16.99913175650, .00038), 18: (17.99915961286, .00205)},
+    'F': {19: (18.9984036273, 1)},
+    'Ag': {107: (106.9050916, .51839), 109: (108.9047553, .48161)},
+    'Au': {197: (196.96656879, 1)},
+    'Si': {28: (27.97692653465, .92223), 29: (28.97649466490, .04685), 30: (29.973770136, 0.3092)},
+    'Ti': {46: (45.95262772, .0825), 47: (46.95175879, 0.0744), 48: (47.94794198, .7372), 49: (48.94786568, .0541),
+           50: (49.94478689, .0518)},
+}
+
+
+def getSpecElt(Elts):
+    if len(Elts) == 1:
+        return Elements[Elts[0]]
+    tm = {}
+    r1 = Elements[Elts[0]]
+    r2 = getSpecElt(Elts[1:])
+    for x in r1:
+        for y in r2:
+            if x + y not in tm:
+                tm[x + y] = [r1[x][0] + r2[y][0], r1[x][1] * r2[y][1]]
+            else:
+                tm[x + y][1] += r1[x][1] * r2[y][1]
+    return tm
+
+
+def SplitElts(elt):
+    elts = []
+    for x, i in re.findall('([A-Z][a-z]?)([0-9]*)', elt):
+        if i == '':
+            i = 1
+        else:
+            i = int(i)
+        elts += [x for k in range(i)]
+    return elts
+
+
+def showElts(Elts):
+    r = getSpecElt(Elts)
+    plt.bar(r.keys(), [z[1] for z in r.values()])
+    plt.show()
+
+
+class BIF6:
+    def __init__(self, filename):
+        self.f = open(filename, 'rb')
+        self.header = struct.unpack('xx4s5H', self.f.read(16))
+        self.size = (self.header[2], self.header[3])
+        self.N = self.size[0] * self.size[1]
+        self.cat = []
+        for i in range(self.header[1]):
+            self.f.seek(16 + i * (4 * self.N + 16))
+            self.cat.append(struct.unpack('4f', self.f.read(16)))
+
+    def getImgID(self, ID):
+        assert ID >= 0 and ID <= self.header[1]
+        self.f.seek(32 + ID * (4 * self.N + 16))
+        return np.array(struct.unpack(str(self.N) + 'I', self.f.read(4 * self.N))).reshape(self.size)
+
+    def getImgMass(self, masses, raw=False):
+        if type(masses) is float or type(masses) is int:
+            masses = [masses]
+        SUM = None
+        for i, x in enumerate(self.cat):
+            for m in masses:
+                if m >= x[0] - .5 and m <= x[1] + .5:
+                    if SUM is None:
+                        SUM = self.getImgID(i)
+                    else:
+                        SUM += self.getImgID(i)
+        if raw:
+            return SUM
+        if SUM is None:
+            return None
+        return pySPM.SPM_image(np.flipud(SUM))
+
+    def getImgElt(self, elt):
+        r = {}
+        A = getSpecElt(SplitElts(elt))
+        for k in A:
+            I = self.getImgMass(k)
+            if I is not None:
+                r[k] = {
+                    'data': I,
+                    'mass': A[k][0],
+                    'abund': A[k][1]}
+        return r
+
+    def showImgElt(self, elt, size=10, abundCorr=False, tot=True):
+        A = self.getImgElt(elt)
+        ks = [z for z in A if A[z]['data'] != None]
+        fig, ax = plt.subplots((len(ks) + 1) // 4 + 1, 4,
+                               figsize=(10 * ((len(ks) + 1) // 4 + 1), 10))
+        mi = np.min(A[ks[0]]['data'].pixels)
+        ma = np.max(A[ks[0]]['data'].pixels)
+        A[ks[0]]['CT'] = ma
+        for i, k in enumerate(ks[1:]):
+            M = np.min(A[k]['data'].pixels)
+            mi = min(mi, M)
+            A[k]['minCT'] = M
+            M = np.max(A[k]['data'].pixels)
+            ma = max(ma, M)
+            A[k]['CT'] = M
+        ks.sort()
+        di = 0
+        if tot:
+            SUM = sum([A[k]['data'].pixels for k in ks])
+            ax[0][0].imshow(SUM, vmin=0)
+            ax[0][0].set_title("Total")
+            di = 1
+        for i, k in enumerate(ks):
+            if abundCorr:
+                ax[(i + di) // 4][(i + di) % 4].imshow(A[k]
+                                                       ['data'].pixels / A[k]['abund'], vmin=0, vmax=ma)
+            else:
+                A[k]['data'].show(ax=ax[(i + di) // 4][(i + di) %
+                                                       4], vmin=0, vmax=ma)
+            ax[(i + di) // 4][(i + di) % 4].set_title(
+                'mass: {mass:.3} - abundancy: {abund:.3f} - CT: {CT}'.format(**A[k]))
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.f.close()
+
+
+class BIF3D:
+
+    def __init__(self, path):
+        self.Peaks = {}
+        self.RPeaks = {}
+        self.Path = os.path.dirname(path)
+        self.Basename = os.path.basename(path)
+        self.size = None
+        for x in os.listdir(self.Path):
+            if x[:len(self.Basename)] == self.Basename:
+                if x[-6:] == ".BIF3D":
+                    s = self.Basename + r' \(([0-9]+)\)(?: - (.*?))?\.BIF3D'
+                    r = re.search(s, x)
+                    ID = int(r.group(1))
+                    self.Peaks[ID] = r.group(2)
+                    if r.group(2) != None:
+                        self.RPeaks[r.group(2)] = ID
+        self.data = {}
+
+    def getIDs(self, channels):
+        assert type(channels) in [str, int, list, tuple]
+        if type(channels) == int:
+            return channels
+        if type(channels) == str:
+            assert channels in self.RPeaks.keys()
+            return self.RPeaks[channels]
+        if type(channels) == list or type(channels) == tuple:
+            ID = []
+            for x in channels:
+                ID.append(self.getIDs(x))
+            return ID
+
+    def getChannel(self, channel):
+        k = self.getIDs(channel)
+        if k in self.data:
+            return self.data[k]
+        v = self.Peaks[k]
+        if v != None:
+            path = '{path}{sep}{basename} ({ID}) - {Peak}.BIF3D'
+        else:
+            path = '{path}{sep}{basename} ({ID}).BIF3D'
+        f = open(path.format(path=self.Path, sep=os.sep,
+                             basename=self.Basename, ID=k, Peak=v), 'rb')
+        A = f.read()
+        f.close()
+        size = struct.unpack("II", A[32:40])
+        if self.size == None:
+            self.size = size
+        else:
+            assert self.size == size
+        return np.array(struct.unpack("{0}d".format(self.size[0] * self.size[1]), A[640:])).reshape(self.size)
+
+    def loadChannel(self, channel):
+        k = self.getIDs(channel)
+        if not k in self.data:
+            self.data[k] = self.getChannel(channel)
+
+    def loadChannels(self, channels):
+        if not type(channels) in [list, tuple]:
+            self.loadChannel(channels)
+        else:
+            for x in channels:
+                self.loadChannel(x)
+
+    def getChannels(self, *channels):
+        k = self.getIDs(channels)
+        self.loadChannels(k)
+        if type(k) == int:
+            return self.data[k]
+        D = np.zeros(self.size)
+        for x in k:
+            D += self.data[x]
+        return D
+
+    def listChannels(self):
+        return self.Peaks
+
+    def show(self, ax, *channels):
+        D = self.getChannels(*channels)
+        ax.imshow(D)
+        if len(channels) > 1:
+            ax.set_title(','.join([str(z) for z in channels]))
+        else:
+            ax.set_title(str(channels[0]))
```

### Comparing `pySPM-0.2.9/pySPM/utils/fit.py` & `pyspm-0.3.0/pySPM/utils/fit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,299 +1,328 @@
-# -- coding: utf-8 --
-
-# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
-
-"""
-Provides useful functions for fitting with scipy.optimize.curve_fit
-"""
-
-from . import math
-import numpy as np
-
-def CDF(x, bg, *args, **kargs):
-    """
-    Return the sum of several CDFs.
-    x: values used to evaluate the function
-    bg: background (value on the very left)
-    args: suits of one or several Ai, xi, si describing each a CDF
-        Ai: Amplitude
-        xi: position
-        si: sigma of CDF
-                     _  
-    ex: step edge: _| |_ between 0.2 and 0.7 in y and -1 and 1 in x with sigma=5
-        CDF(x, 0.2, 0.5, -1, 5, -0.5, 1, 5)
-    """
-    if 'A' in kargs and 'x0' in kargs and 'sig' in kargs:
-        args = [x for y in zip(kargs['A'], kargs['x0'], kargs['sig']) for x in y]
-        
-    r = bg * np.ones(x.shape)
-    if len(args)%3 != 0:
-        raise Exception("Invalid number of arguments. see help.")
-        return
-        
-    for i in range(len(args)//3):
-        r += args[3*i]*math.CDF(x, args[3*i+1], args[3*i+2])
-    return r
-
-def lgCDF(x, bg, lg=0, *args, **kargs):
-    """
-    Return the sum of several CDFs.
-    x: values used to evaluate the function
-    bg: background (value on the very left)
-    lg: Lorentz-Gauss factor (0=Gauss, 1=Lorentz, in-between = mix)
-    args: suits of one or several Ai, xi, si describing each a CDF
-        Ai: Amplitude
-        xi: position
-        si: sigma of CDF
-                     _  
-    ex: step edge: _| |_ between 0.2 and 0.7 in y and -1 and 1 in x with sigma=5
-        lgCDF(x, lg, 0.2, 0.5, -1, 5, -0.5, 1, 5)
-    """
-    
-    if 'A' in kargs and 'x0' in kargs and 'sig' in kargs:
-        args = [x for y in zip(kargs['A'], kargs['x0'], kargs['sig']) for x in y]
-    
-    r = bg * np.ones(x.shape)
-    if len(args)%3 != 0:
-        raise Exception("Invalid number of arguments. see help.")
-        return
-        
-    for i in range(len(args)//3):
-        r += args[3*i]*math.CDF(x, args[3*i+1], args[3*i+2], lg=lg)
-    return r
-
-def lgCDF_fit(x,y, p0, dic=False):
-    import scipy.optimize as opt
-    n = (len(p0)-2)//3
-    bounds=[
-        [0,0]+[-np.inf,-np.inf,0]*n,
-        [np.inf,1]+[np.inf,np.inf,np.inf]*n]
-    popt, pcov = opt.curve_fit(lgCDF, x, y, p0, bounds=bounds)
-    if dic:
-        d = np.diag(pcov)
-        return dict(bg=popt[0],lg=popt[1],A=popt[2::3],x0=popt[3::3],sig=popt[4::3]), dict(bg=d[0],lg=d[1],A=d[2::3],x0=d[3::3],sig=d[4::3])
-    return popt, pcov
-
-def CDF_fit(x,y, p0, dic=False):
-    import scipy.optimize as opt
-    n = (len(p0)-1)//3
-    bounds=[
-        [0]+[-np.inf,-np.inf,0]*n,
-        [np.inf]+[np.inf,np.inf,np.inf]*n]
-    popt, pcov = opt.curve_fit(CDF, x, y, p0, bounds=bounds)
-    if dic:
-        d = np.diag(pcov)
-        return dict(bg=popt[0], A=popt[1::3],x0=popt[2::3],sig=popt[3::3]), dict(bg=d[0],A=d[2::3],x0=d[3::3],sig=d[4::3])
-    return popt, pcov
-
-def LG2Dr(A, ratio=np.sqrt(2), Rweight=None, sigma=None, dic=False, **kargs):
-    """
-    Perform a 2D Lorentz-Gauss fitting on a 2D array A with a fix ration between σx and σy
-    dic: if True return the solution as a dictionary
-    
-    output: list of popt and pcov array.
-    The parameter order is:
-    Amplitude, Angle, Sigma_x, Sigma_y, Center_x, Center_y, LGx, LGy
-    """
-    from scipy.optimize import curve_fit
-    params = ['amplitude', 'angle', 'sig_y', 'x0', 'y0', 'LG_x', 'LG_y','bg']
-    def fit(XY, *args):
-        # Add default parameters to the argument list at the right position
-        j = 0
-        a = []
-        for x in params:
-            if x in kargs:
-                a.append(kargs[x])
-            else:
-                a.append(args[j])
-                j += 1
-        a = a[:2]+[ratio*a[2]]+a[2:] # insert sig_x
-        # Calculate the 2D Lorentz-Gauss
-        return a[-1]+math.LG2D(XY, *a[:-1]).ravel()
-        
-    # First guess for parameters
-    Amplitude = np.max(A)
-    Center = np.unravel_index(np.argmax(A), A.shape)
-    p0_def = [Amplitude, 0, 10, Center[1], Center[0], 0, 0, 0]
-    bounds_def = [
-        [0     , np.radians(-45),       0, -np.inf, -np.inf, 0, 0, 0],
-        [np.inf, np.radians(45) , +np.inf,  np.inf,  np.inf, 1, 1, np.inf]
-        ]
-    p0 = [p0_def[i] for i,x in enumerate(params) if x not in kargs]
-    bounds = [
-        [bounds_def[0][i] for i,x in enumerate(params) if x not in kargs],
-        [bounds_def[1][i] for i,x in enumerate(params) if x not in kargs]
-        ]
-    # Kick out arguments for the given default parameters
-
-    x = np.arange(A.shape[1])
-    y = np.arange(A.shape[0])
-    X, Y = np.meshgrid(x, y)
-    R = np.sqrt((X-Center[1])**2+(Y-Center[0])**2)
-    if Rweight is not None:
-        if Rweight is 'R':
-            sigma = 0.001+R
-        else:
-            sigma = Rweight(R)
-    if sigma is not None:
-        sigma = np.ravel(sigma)
-    pfit = curve_fit(fit, (X, Y), np.ravel(A), p0=p0, sigma = sigma, bounds=bounds)        
-    
-    # Re-add default parameters to the output
-    pout = []
-    dpout = []
-    j = 0
-    for i,x in enumerate(params):
-        if x in kargs:
-            pout.append(kargs[x])
-            dpout.append(0)
-        else:
-            pout.append(pfit[0][j])
-            dpout.append(np.sqrt(pfit[1][j,j]))
-            j += 1
-    pout = pout[:2]+[ratio*pout[2]]+pout[2:]
-    dpout = dpout[:2]+[ratio*dpout[2]]+dpout[2:]
-    if dic:
-        params2 = params[:2]+['sig_x']+params[2:]
-        return dict(zip(params2, pout)), dict(zip(params2, dpout))
-    return pout, dpout
-
-def LG2D(A, Rweight=None, sigma=None, dic=False, **kargs):
-    """
-    Perform a 2D Lorentz-Gauss fitting on a 2D array A
-    dic: if True return the solution as a dictionary
-    
-    output: list of popt and pcov array.
-    The parameter order is:
-    Amplitude, Angle, Sigma_x, Sigma_y, Center_x, Center_y, LGx, LGy
-    """
-    from scipy.optimize import curve_fit
-    params = ['amplitude', 'angle', 'sig_x', 'sig_y', 'x0', 'y0', 'LG_x', 'LG_y', 'assym_x', 'assym_y', 'bg']
-    def fit(XY, *args):
-        # Add default parameters to the argument list at the right position
-        j = 0
-        a = []
-        for x in params:
-            if x in kargs:
-                a.append(kargs[x])
-            else:
-                a.append(args[j])
-                j += 1
-        # Calculate the 2D Lorentz-Gauss
-        return a[-1]+math.LG2D(XY, *a[:-1]).ravel()
-        
-    # First guess for parameters
-    Amplitude = np.max(A)
-    Center = np.unravel_index(np.argmax(A), A.shape)
-    p0_def = [Amplitude, 0, 10, 10, Center[1], Center[0], 0, 0, 1, 1, 0]
-    bounds_def = [
-        [0     , np.radians(-45),       0,       0, -np.inf, -np.inf, 0, 0, 0, 0, -np.inf],
-        [np.inf, np.radians(45) , +np.inf, +np.inf,  np.inf,  np.inf, 1, 1, np.inf, np.inf, np.inf]
-        ]
-    p0 = [p0_def[i] for i,x in enumerate(params) if x not in kargs]
-    bounds = [
-        [bounds_def[0][i] for i,x in enumerate(params) if x not in kargs],
-        [bounds_def[1][i] for i,x in enumerate(params) if x not in kargs]
-        ]
-    # Kick out arguments for the given default parameters
-
-    x = np.arange(A.shape[1])
-    y = np.arange(A.shape[0])
-    X, Y = np.meshgrid(x, y)
-    R = np.sqrt((X-Center[1])**2+(Y-Center[0])**2)
-    if Rweight is not None:
-        if Rweight is 'R':
-            sigma = 0.001+R
-        else:
-            sigma = Rweight(R)
-    if sigma is not None:
-        sigma = np.ravel(sigma)
-    pfit = curve_fit(fit, (X, Y), np.ravel(A), p0=p0, sigma = sigma, bounds=bounds)        
-    
-    # Re-add default parameters to the output
-    pout = []
-    dpout = []
-    j = 0
-    for i,x in enumerate(params):
-        if x in kargs:
-            pout.append(kargs[x])
-            dpout.append(0)
-        else:
-            pout.append(pfit[0][j])
-            dpout.append(np.sqrt(pfit[1][j,j]))
-            j += 1
-            
-    if dic:
-       return dict(zip(params, pout)), dict(zip(params, dpout))
-    return pout, dpout
-
-def LG2Da(A, Rweight=None, sigma=None, dic=False, **kargs):
-    """
-    Perform a 2D Lorentz-Gauss fitting on a 2D array A
-    dic: if True return the solution as a dictionary
-    
-    output: list of popt and pcov array.
-    The parameter order is:
-    Amplitude, Angle, Sigma_x, Sigma_y, Center_x, Center_y, LGx, LGy
-    """
-    from scipy.optimize import curve_fit
-    params = ['amplitude', 'angle', 'sigN', 'sigS', 'sigE','sigW','x0', 'y0', 'LGN', 'LGS','LGE','LGW','bg']
-    def fit(XY, *args):
-        # Add default parameters to the argument list at the right position
-        j = 0
-        a = []
-        for x in params:
-            if x in kargs:
-                a.append(kargs[x])
-            else:
-                a.append(args[j])
-                j += 1
-        # Calculate the 2D Lorentz-Gauss
-        return a[-1]+math.LG2Da(XY, *a[:-1]).ravel()
-        
-    # First guess for parameters
-    Amplitude = np.max(A)
-    Center = np.unravel_index(np.argmax(A), A.shape)
-    #   Amplitude,           angle,    sigN,    sigS,    sigE,    sigW,        x0,        y0, LGN, LGS, LGE, LGW, bg
-    p0_def = [
-        Amplitude,               0,      10,      10,      10,      10, Center[1], Center[0], 0, 0, 0, 0, 0]
-    bounds_def = [
-        [0       , np.radians(-45),       0,       0,       0,       0,   -np.inf,   -np.inf, 0, 0, 0, 0, -np.inf],
-        [  np.inf,  np.radians(45), +np.inf, +np.inf, +np.inf, +np.inf,   +np.inf,    np.inf, 1, 1, 1, 1, np.inf]
-        ]
-    p0 = [p0_def[i] for i,x in enumerate(params) if x not in kargs]
-    bounds = [
-        [bounds_def[0][i] for i,x in enumerate(params) if x not in kargs],
-        [bounds_def[1][i] for i,x in enumerate(params) if x not in kargs]
-        ]
-    # Kick out arguments for the given default parameters
-
-    x = np.arange(A.shape[1])
-    y = np.arange(A.shape[0])
-    X, Y = np.meshgrid(x, y)
-    R = np.sqrt((X-Center[1])**2+(Y-Center[0])**2)
-    if Rweight is not None:
-        if Rweight is 'R':
-            sigma = 0.001+R
-        else:
-            sigma = Rweight(R)
-    if sigma is not None:
-        sigma = np.ravel(sigma)
-    pfit = curve_fit(fit, (X, Y), np.ravel(A), p0=p0, sigma = sigma, bounds=bounds)        
-    
-    # Re-add default parameters to the output
-    pout = []
-    dpout = []
-    j = 0
-    for i,x in enumerate(params):
-        if x in kargs:
-            pout.append(kargs[x])
-            dpout.append(0)
-        else:
-            pout.append(pfit[0][j])
-            dpout.append(np.sqrt(pfit[1][j,j]))
-            j += 1
-            
-    if dic:
-       return dict(zip(params, pout)), dict(zip(params, dpout))
-    return pout, dpout
-    
+# -- coding: utf-8 --
+
+# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
+
+"""
+Provides useful functions for fitting with scipy.optimize.curve_fit
+"""
+
+import numpy as np
+
+from . import math
+
+
+def peak_fit(m, s, m0, delta=0.02):
+    from scipy.optimize import curve_fit
+    from . import LG, get_mass
+    assert len(m) == len(s)
+    if type(m0) is str:
+        m0 = get_mass(m0)
+    assert m0 < m[-1] and m0 > m[0]
+    assert delta > 0
+    mask = (m >= (m0 - delta)) * (m <= (m0 + delta))
+    amp0 = np.max(s[mask])
+    sig = abs(m[mask][np.argmin(abs(s[mask] - amp0 / 2))] - m0) / np.sqrt(2 * np.log(2))
+    p00 = (m[mask][np.argmax(s[mask])], sig, amp0, .3, 1)
+    p0, _ = curve_fit(LG, m[mask], s[mask], p00, bounds=((-np.inf, 0, 0, 0, 0), (np.inf, np.inf, np.inf, 1, np.inf)))
+    return p0
+
+
+def CDF(x, bg, *args, **kargs):
+    """
+    Return the sum of several CDFs.
+    x: values used to evaluate the function
+    bg: background (value on the very left)
+    args: suits of one or several Ai, xi, si describing each a CDF
+        Ai: Amplitude
+        xi: position
+        si: sigma of CDF
+                     _  
+    ex: step edge: _| |_ between 0.2 and 0.7 in y and -1 and 1 in x with sigma=5
+        CDF(x, 0.2, 0.5, -1, 5, -0.5, 1, 5)
+    """
+    if 'A' in kargs and 'x0' in kargs and 'sig' in kargs:
+        args = [x for y in zip(kargs['A'], kargs['x0'], kargs['sig']) for x in y]
+
+    r = bg * np.ones(x.shape)
+    if len(args) % 3 != 0:
+        raise Exception("Invalid number of arguments. see help.")
+        return
+
+    for i in range(len(args) // 3):
+        r += args[3 * i] * math.CDF(x, args[3 * i + 1], args[3 * i + 2])
+    return r
+
+
+def lgCDF(x, bg, lg=0, *args, **kargs):
+    """
+    Return the sum of several CDFs.
+    x: values used to evaluate the function
+    bg: background (value on the very left)
+    lg: Lorentz-Gauss factor (0=Gauss, 1=Lorentz, in-between = mix)
+    args: suits of one or several Ai, xi, si describing each a CDF
+        Ai: Amplitude
+        xi: position
+        si: sigma of CDF
+                     _  
+    ex: step edge: _| |_ between 0.2 and 0.7 in y and -1 and 1 in x with sigma=5
+        lgCDF(x, lg, 0.2, 0.5, -1, 5, -0.5, 1, 5)
+    """
+
+    if 'A' in kargs and 'x0' in kargs and 'sig' in kargs:
+        args = [x for y in zip(kargs['A'], kargs['x0'], kargs['sig']) for x in y]
+
+    r = bg * np.ones(x.shape)
+    if len(args) % 3 != 0:
+        raise Exception("Invalid number of arguments. see help.")
+        return
+
+    for i in range(len(args) // 3):
+        r += args[3 * i] * math.CDF(x, args[3 * i + 1], args[3 * i + 2], lg=lg)
+    return r
+
+
+def lgCDF_fit(x, y, p0, dic=False):
+    import scipy.optimize as opt
+    n = (len(p0) - 2) // 3
+    bounds = [
+        [0, 0] + [-np.inf, -np.inf, 0] * n,
+        [np.inf, 1] + [np.inf, np.inf, np.inf] * n]
+    popt, pcov = opt.curve_fit(lgCDF, x, y, p0, bounds=bounds)
+    if dic:
+        d = np.diag(pcov)
+        return dict(bg=popt[0], lg=popt[1], A=popt[2::3], x0=popt[3::3], sig=popt[4::3]), dict(bg=d[0], lg=d[1],
+                                                                                               A=d[2::3], x0=d[3::3],
+                                                                                               sig=d[4::3])
+    return popt, pcov
+
+
+def CDF_fit(x, y, p0, dic=False):
+    import scipy.optimize as opt
+    n = (len(p0) - 1) // 3
+    bounds = [
+        [0] + [-np.inf, -np.inf, 0] * n,
+        [np.inf] + [np.inf, np.inf, np.inf] * n]
+    popt, pcov = opt.curve_fit(CDF, x, y, p0, bounds=bounds)
+    if dic:
+        d = np.diag(pcov)
+        return dict(bg=popt[0], A=popt[1::3], x0=popt[2::3], sig=popt[3::3]), dict(bg=d[0], A=d[2::3], x0=d[3::3],
+                                                                                   sig=d[4::3])
+    return popt, pcov
+
+
+def LG2Dr(A, ratio=np.sqrt(2), Rweight=None, sigma=None, dic=False, **kargs):
+    """
+    Perform a 2D Lorentz-Gauss fitting on a 2D array A with a fix ration between σx and σy
+    dic: if True return the solution as a dictionary
+    
+    output: list of popt and pcov array.
+    The parameter order is:
+    Amplitude, Angle, Sigma_x, Sigma_y, Center_x, Center_y, LGx, LGy
+    """
+    from scipy.optimize import curve_fit
+    params = ['amplitude', 'angle', 'sig_y', 'x0', 'y0', 'LG_x', 'LG_y', 'bg']
+
+    def fit(XY, *args):
+        # Add default parameters to the argument list at the right position
+        j = 0
+        a = []
+        for x in params:
+            if x in kargs:
+                a.append(kargs[x])
+            else:
+                a.append(args[j])
+                j += 1
+        a = a[:2] + [ratio * a[2]] + a[2:]  # insert sig_x
+        # Calculate the 2D Lorentz-Gauss
+        return a[-1] + math.LG2D(XY, *a[:-1]).ravel()
+
+    # First guess for parameters
+    Amplitude = np.max(A)
+    Center = np.unravel_index(np.argmax(A), A.shape)
+    p0_def = [Amplitude, 0, 10, Center[1], Center[0], 0, 0, 0]
+    bounds_def = [
+        [0, np.radians(-45), 0, -np.inf, -np.inf, 0, 0, 0],
+        [np.inf, np.radians(45), +np.inf, np.inf, np.inf, 1, 1, np.inf]
+    ]
+    p0 = [p0_def[i] for i, x in enumerate(params) if x not in kargs]
+    bounds = [
+        [bounds_def[0][i] for i, x in enumerate(params) if x not in kargs],
+        [bounds_def[1][i] for i, x in enumerate(params) if x not in kargs]
+    ]
+    # Kick out arguments for the given default parameters
+
+    x = np.arange(A.shape[1])
+    y = np.arange(A.shape[0])
+    X, Y = np.meshgrid(x, y)
+    R = np.sqrt((X - Center[1]) ** 2 + (Y - Center[0]) ** 2)
+    if Rweight is not None:
+        if Rweight == 'R':
+            sigma = 0.001 + R
+        else:
+            sigma = Rweight(R)
+    if sigma is not None:
+        sigma = np.ravel(sigma)
+    pfit = curve_fit(fit, (X, Y), np.ravel(A), p0=p0, sigma=sigma, bounds=bounds)
+
+    # Re-add default parameters to the output
+    pout = []
+    dpout = []
+    j = 0
+    for i, x in enumerate(params):
+        if x in kargs:
+            pout.append(kargs[x])
+            dpout.append(0)
+        else:
+            pout.append(pfit[0][j])
+            dpout.append(np.sqrt(pfit[1][j, j]))
+            j += 1
+    pout = pout[:2] + [ratio * pout[2]] + pout[2:]
+    dpout = dpout[:2] + [ratio * dpout[2]] + dpout[2:]
+    if dic:
+        params2 = params[:2] + ['sig_x'] + params[2:]
+        return dict(zip(params2, pout)), dict(zip(params2, dpout))
+    return pout, dpout
+
+
+def LG2D(A, Rweight=None, sigma=None, dic=False, **kargs):
+    """
+    Perform a 2D Lorentz-Gauss fitting on a 2D array A
+    dic: if True return the solution as a dictionary
+    
+    output: list of popt and pcov array.
+    The parameter order is:
+    Amplitude, Angle, Sigma_x, Sigma_y, Center_x, Center_y, LGx, LGy
+    """
+    from scipy.optimize import curve_fit
+    params = ['amplitude', 'angle', 'sig_x', 'sig_y', 'x0', 'y0', 'LG_x', 'LG_y', 'assym_x', 'assym_y', 'bg']
+
+    def fit(XY, *args):
+        # Add default parameters to the argument list at the right position
+        j = 0
+        a = []
+        for x in params:
+            if x in kargs:
+                a.append(kargs[x])
+            else:
+                a.append(args[j])
+                j += 1
+        # Calculate the 2D Lorentz-Gauss
+        return a[-1] + math.LG2D(XY, *a[:-1]).ravel()
+
+    # First guess for parameters
+    Amplitude = np.max(A)
+    Center = np.unravel_index(np.argmax(A), A.shape)
+    p0_def = [Amplitude, 0, 10, 10, Center[1], Center[0], 0, 0, 1, 1, 0]
+    bounds_def = [
+        [0, np.radians(-45), 0, 0, -np.inf, -np.inf, 0, 0, 0, 0, -np.inf],
+        [np.inf, np.radians(45), +np.inf, +np.inf, np.inf, np.inf, 1, 1, np.inf, np.inf, np.inf]
+    ]
+    p0 = [p0_def[i] for i, x in enumerate(params) if x not in kargs]
+    bounds = [
+        [bounds_def[0][i] for i, x in enumerate(params) if x not in kargs],
+        [bounds_def[1][i] for i, x in enumerate(params) if x not in kargs]
+    ]
+    # Kick out arguments for the given default parameters
+
+    x = np.arange(A.shape[1])
+    y = np.arange(A.shape[0])
+    X, Y = np.meshgrid(x, y)
+    R = np.sqrt((X - Center[1]) ** 2 + (Y - Center[0]) ** 2)
+    if Rweight is not None:
+        if Rweight == 'R':
+            sigma = 0.001 + R
+        else:
+            sigma = Rweight(R)
+    if sigma is not None:
+        sigma = np.ravel(sigma)
+    pfit = curve_fit(fit, (X, Y), np.ravel(A), p0=p0, sigma=sigma, bounds=bounds)
+
+    # Re-add default parameters to the output
+    pout = []
+    dpout = []
+    j = 0
+    for i, x in enumerate(params):
+        if x in kargs:
+            pout.append(kargs[x])
+            dpout.append(0)
+        else:
+            pout.append(pfit[0][j])
+            dpout.append(np.sqrt(pfit[1][j, j]))
+            j += 1
+
+    if dic:
+        return dict(zip(params, pout)), dict(zip(params, dpout))
+    return pout, dpout
+
+
+def LG2Da(A, Rweight=None, sigma=None, dic=False, **kargs):
+    """
+    Perform a 2D Lorentz-Gauss fitting on a 2D array A
+    dic: if True return the solution as a dictionary
+    
+    output: list of popt and pcov array.
+    The parameter order is:
+    Amplitude, Angle, Sigma_x, Sigma_y, Center_x, Center_y, LGx, LGy
+    """
+    from scipy.optimize import curve_fit
+    params = ['amplitude', 'angle', 'sigN', 'sigS', 'sigE', 'sigW', 'x0', 'y0', 'LGN', 'LGS', 'LGE', 'LGW', 'bg']
+
+    def fit(XY, *args):
+        # Add default parameters to the argument list at the right position
+        j = 0
+        a = []
+        for x in params:
+            if x in kargs:
+                a.append(kargs[x])
+            else:
+                a.append(args[j])
+                j += 1
+        # Calculate the 2D Lorentz-Gauss
+        return a[-1] + math.LG2Da(XY, *a[:-1]).ravel()
+
+    # First guess for parameters
+    Amplitude = np.max(A)
+    Center = np.unravel_index(np.argmax(A), A.shape)
+    #   Amplitude,           angle,    sigN,    sigS,    sigE,    sigW,        x0,        y0, LGN, LGS, LGE, LGW, bg
+    p0_def = [
+        Amplitude, 0, 10, 10, 10, 10, Center[1], Center[0], 0, 0, 0, 0, 0]
+    bounds_def = [
+        [0, np.radians(-45), 0, 0, 0, 0, -np.inf, -np.inf, 0, 0, 0, 0, -np.inf],
+        [np.inf, np.radians(45), +np.inf, +np.inf, +np.inf, +np.inf, +np.inf, np.inf, 1, 1, 1, 1, np.inf]
+    ]
+    p0 = [p0_def[i] for i, x in enumerate(params) if x not in kargs]
+    bounds = [
+        [bounds_def[0][i] for i, x in enumerate(params) if x not in kargs],
+        [bounds_def[1][i] for i, x in enumerate(params) if x not in kargs]
+    ]
+    # Kick out arguments for the given default parameters
+
+    x = np.arange(A.shape[1])
+    y = np.arange(A.shape[0])
+    X, Y = np.meshgrid(x, y)
+    R = np.sqrt((X - Center[1]) ** 2 + (Y - Center[0]) ** 2)
+    if Rweight is not None:
+        if Rweight == 'R':
+            sigma = 0.001 + R
+        else:
+            sigma = Rweight(R)
+    if sigma is not None:
+        sigma = np.ravel(sigma)
+    pfit = curve_fit(fit, (X, Y), np.ravel(A), p0=p0, sigma=sigma, bounds=bounds)
+
+    # Re-add default parameters to the output
+    pout = []
+    dpout = []
+    j = 0
+    for i, x in enumerate(params):
+        if x in kargs:
+            pout.append(kargs[x])
+            dpout.append(0)
+        else:
+            pout.append(pfit[0][j])
+            dpout.append(np.sqrt(pfit[1][j, j]))
+            j += 1
+
+    if dic:
+        return dict(zip(params, pout)), dict(zip(params, dpout))
+    return pout, dpout
```

### Comparing `pySPM-0.2.9/pySPM/utils/haar.py` & `pyspm-0.3.0/pySPM/utils/haar.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-import numpy as np
-import copy
-import pywt
-
-
-def sign(abs_var, sign_var):
-    return abs(abs_var) * (1 - np.where(sign_var < 0, 2*sign_var, sign_var))
-    
-def hfilter(diff_image, var_image, threshold=1, ndamp=10):
-    """:ta  
-    This code was inspired from: https://github.com/spacetelescope/sprint_notebooks/blob/master/lucy_damped_haar.ipynb
-    I believe it was initially written by Justin Ely: https://github.com/justincely
-    It was buggy and not working properly with every image sizes.
-    I have thus exchanged it by using pyWavelet (pywt) and a custom function htrans
-    to calculate the matrix for the var_image.
-    """
-    him, coeff_slices = pywt.coeffs_to_array(pywt.wavedec2(diff_image.astype(np.float), 'haar'), padding=0)
-    dvarim = htrans(var_image.astype(np.float))
-    
-    sqhim = ((him/threshold)**2)/dvarim
-    index = np.where(sqhim < 1)
-    
-    if len(index[0]) == 0:
-        return diff_image
-    
-    # Eq. 8 of White is derived leading to N*x^(N-1)-(N-1)*x^N  :DOI: 10.1117/12.176819
-    sqhim = sqhim[index] * (ndamp * sqhim[index]**(ndamp-1) - (ndamp-1)*sqhim[index]**ndamp)
-    him[index] = sign(threshold*np.sqrt(dvarim[index] * sqhim), him[index])
-    
-    return pywt.waverec2(pywt.array_to_coeffs(him, coeff_slices, output_format='wavedec2'), 'haar')[:diff_image.shape[0],:diff_image.shape[1]]
-
-def htrans(A):
-    h0 = A
-    res = []
-    while h0.shape[0]>1 and h0.shape[1]>1:
-        h0, (hx, hy, hc) = pywt.dwt2(h0, 'haar')
-        res = [(h0, h0, h0)]+res
-    out, _ = pywt.coeffs_to_array([h0]+res, padding=1)
-    return out
+import numpy as np
+import pywt
+
+
+def sign(abs_var, sign_var):
+    return abs(abs_var) * (1 - np.where(sign_var < 0, 2 * sign_var, sign_var))
+
+
+def hfilter(diff_image, var_image, threshold=1, ndamp=10):
+    """
+    This code was inspired from: https://github.com/spacetelescope/sprint_notebooks/blob/master/lucy_damped_haar.ipynb
+    I believe it was initially written by Justin Ely: https://github.com/justincely
+    It was buggy and not working properly with every image sizes.
+    I have thus exchanged it by using pyWavelet (pywt) and a custom function htrans
+    to calculate the matrix for the var_image.
+    """
+    him, coeff_slices = pywt.coeffs_to_array(pywt.wavedec2(diff_image.astype(np.float), 'haar'), padding=0)
+    dvarim = htrans(var_image.astype(np.float))
+
+    sqhim = ((him / threshold) ** 2) / dvarim
+    index = np.where(sqhim < 1)
+
+    if len(index[0]) == 0:
+        return diff_image
+
+    # Eq. 8 of White is derived leading to N*x^(N-1)-(N-1)*x^N  :DOI: 10.1117/12.176819
+    sqhim = sqhim[index] * (ndamp * sqhim[index] ** (ndamp - 1) - (ndamp - 1) * sqhim[index] ** ndamp)
+    him[index] = sign(threshold * np.sqrt(dvarim[index] * sqhim), him[index])
+
+    return pywt.waverec2(pywt.array_to_coeffs(him, coeff_slices, output_format='wavedec2'), 'haar')[
+           :diff_image.shape[0], :diff_image.shape[1]]
+
+
+def htrans(A):
+    h0 = A
+    res = []
+    while h0.shape[0] > 1 and h0.shape[1] > 1:
+        h0, (hx, hy, hc) = pywt.dwt2(h0, 'haar')
+        res = [(h0, h0, h0)] + res
+    out, _ = pywt.coeffs_to_array([h0] + res, padding=1)
+    return out
```

### Comparing `pySPM-0.2.9/pySPM/utils/plot.py` & `pyspm-0.3.0/pySPM/utils/plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,318 +1,395 @@
-# -- coding: utf-8 --
-# -- coding: utf-8 --
-
-# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
-
-"""
-Various helper function for plotting data with matplotlib
-"""
-
-import numpy as np
-import matplotlib.pyplot as plt
-import matplotlib as mpl
-from .misc import dec_debug, do_debug
-
-def plotMask(ax, mask, color, **kargs):
-    """
-    Create an overlay of a given color where mask is True.
-    The transparency and other parameters can be adjusted with **kargs. see help(plt.imshow)
-    
-    ax: matplotlib axis
-    mask: An array with value True where the mask should be plotted
-    color: color of the mask
-    **kargs: dictionnary of arguments which can be passed to imshow. Useful is mainly: alpha
-    """
-    import copy
-    m = np.ma.masked_array(mask, ~mask)
-    palette = copy.copy(plt.cm.gray)
-    palette.set_over(color, 1.0)
-    ax.imshow(m, cmap=palette, vmin=0, vmax=0.5, **kargs)
-
-def offset_coord(xy, offset=(0,0), ax=None, fig=None, unit='px'):
-    if ax is None:
-        ax = plt.gca()
-
-    if fig is None:
-        fig = plt.gcf()
-
-    tr = ax.transData
-    tri = tr.inverted()
-
-    if unit is 'px':
-        offset = np.array(offset)
-    elif unit is 'ax':
-        offset = ax.transAxes.transform(offset)
-    elif unit is 'fig':
-        offset = fig.transFigure.transform(offset)
-    return tri.transform(tr.transform(xy)+offset)
-
-def Xdist(ax,left, right, y, color='r', linestyle=':', fmt="{dist:.1f}{unit}", xtransf=lambda x: x, va='bottom', ha='center', offset=(0,2), **kargs):
-    """
-    Show the distance between to x-values
-    
-    ax: matplotlib axis
-    left: x-value of the left mark
-    right: x-value of the right mark
-    y: height of the label
-    color: color of the lines / labels
-    linestyle: linestyle of the vertical lines
-    fmt: Format string to parse the distance
-    xtransf: a function can be passed to display the distance in an other unit that the x axis.
-        example: xtransf=lambda x: x*1e3 to display the distance in nm on an axis that uses micro-meters.
-    va: vertical alignment of the distance label
-    ha: horizontal alignment of the distance label
-    offset: (x,y) offset of the label in pixels
-    **kargs: additional arguments.
-        arguments starting with amn_ will be sent to the annotation
-        arguments starting with arr_ will be sent to the arrow
-        for example arr_color='r', ann_color='b' will display a red arrow with the distance in blue
-    """
-    
-    ax.axvline(left, color=color, linestyle=linestyle)
-    ax.axvline(right, color=color, linestyle=linestyle)
-    ann = dict(va=va, ha=ha, color=color)
-    ann.update({k[3:]:kargs[k] for k in kargs if k.startswith('an_')})
-    ax.annotate(fmt.format(dist=xtransf(right-left),unit=kargs.get('unit','')), ({'center':.5*(left+right),'left':right,'right':left}[ann['ha']], y), offset, textcoords='offset pixels', **ann)
-    arr = dict(arrowstyle='<->',color=color)
-    arr.update({k[4:]:kargs[k] for k in kargs if k.startswith('arr_')})
-    ax.annotate("", (left, y), (right, y), arrowprops=arr)
-
-def Ydist(ax, down, up, x, color='r', linestyle=':', fmt="{dist:.2f}{unit}", ytransf=lambda y: y, rotation=90, va='center', ha='right', offset=(-2,0), **kargs):
-    """
-    Show the distance between to x-values
-    
-    ax: matplotlib axis
-    down: y-value of the bottom mark
-    up: y-value of the top mark
-    x: gorizontal position of the label
-    color: color of the lines / labels
-    linestyle: linestyle of the vertical lines
-    fmt: Format string to parse the distance
-    xtransf: a function can be passed to display the distance in an other unit that the x axis.
-        example: xtransf=lambda x: x*1e3 to display the distance in nm on an axis that uses micro-meters.
-    va: vertical alignment of the distance label
-    ha: horizontal alignment of the distance label
-    offset: (x,y) offset of the label in pixels
-    **kargs: additional arguments.
-        arguments starting with amn_ will be sent to the annotation
-        arguments starting with arr_ will be sent to the arrow
-        for example arr_color='r', ann_color='b' will display a red arrow with the distance in blue
-    """
-    
-    ax.axhline(down, color=color, linestyle=linestyle)
-    ax.axhline(up, color=color, linestyle=linestyle)
-    ann = dict(va=va, ha=ha, color=color)
-    ann.update({k[3:]:kargs[k] for k in kargs if k.startswith('an_')})
-    ax.annotate(fmt.format(dist=ytransf(up-down),unit=kargs.get('unit','')), (x,{'center':.5*(down+up),'top':up,'bottom':down}[ann['va']]), offset, textcoords='offset pixels', rotation=rotation, **ann)
-    arr = dict(arrowstyle='<->',color=color)
-    arr.update({k[4:]:kargs[k] for k in kargs if k.startswith('arr_')})
-    ax.annotate("", (x, down), (x, up), arrowprops=arr)
-    
-def DualPlot(ax, col1='C0',col2='C1'):
-    """
-    Create a dual axis from ax and tune the color of the left/right axes to col1, col2 resp.
-    """
-    axb = ax.twinx()
-    axb.spines['left'].set_color(col1)
-    axb.spines['right'].set_color(col2)
-    ax.yaxis.label.set_color(col1)
-    axb.yaxis.label.set_color(col2)
-    ax.tick_params(axis='y', colors=col1)
-    axb.tick_params(axis='y', colors=col2)
-    return axb
-
-def sp(M, N=1, W=21, ravel=True, fig=False):
-    """
-    Shortcut for creating subplots with max width = W (default 21,
-        which seems to correspond to 100% of the width in jupyter).
-    Height is calculated in order to have square subplots.
-    The layout is given by M columns and N lines.
-    If N is negative, abs(N) is interpreted as the number of elements and the number of line will be calculated automatically in function of M.
-    """
-    if N < 0:
-        tot = -N
-        N = 1+(tot-1)//M
-    f, ax = plt.subplots(N, M, figsize=(W, N*W/M))
-    if ravel:
-        if fig:
-            return np.ravel(ax), f
-        return np.ravel(ax)
-    if fig:
-        return ax, f
-    return ax
-    
-def get_rect(img, bottom, top, left, right, ax, color='r'):
-    """
-    return a sub-area on a 2D-array img and display the boundaries on a matplotlib axis ax
-    """
-    ax.axhline(bottom, color=color)
-    ax.axhline(top, color=color)
-    ax.axvline(left, color=color)
-    ax.axvline(right, color=color)
-    return img[bottom:top, left:right]
-    
-def sublegend(*ax, **kargs):
-    labels   = kargs.get('labels', None)
-    color    = kargs.get('color', 'white')
-    margin   = kargs.get('margin', 9)
-    titles   = kargs.get('titles', None)
-    fontsize = kargs.get('fontsize',14)
-    """
-    ax: list of axes
-    labels: If None, the will be a, b, c, d, ...
-    color: background color of the rectangle
-    margin: margin in pixel from the axis border
-    titles: set to False to remove all titles. (Useful to keep the set_title info in the code to remember what is plotted)
-    fontsize: The font size of the labels
-    """
-    props = dict(boxstyle='round', facecolor=color, alpha=1)  
-    if not hasattr(margin, "__getitem__") and not hasattr(margin, "__iter__"):
-        margin = (margin, margin)
-
-    if labels is None:
-        labels = [chr(ord('a')+i) for i,_ in enumerate(np.ravel(ax))]
-    for i,a in enumerate(np.ravel(ax)):
-        if titles is False:
-            a.set_title("")
-        a.annotate(labels[i],(0, 1),xytext=(margin[0],-margin[1]),fontsize=fontsize,verticalalignment='top', bbox=props, xycoords='axes fraction',textcoords='offset pixels');
-
-def formula(x):
-    import re
-    x = re.sub('_([0-9]+)',r'$_{\1}$',x)
-    x = re.sub(r'\^([0-9\+\-]+)',r'$^{\1}$',x)
-    return x
-
-def __points_in_bbox(x,y,bbox):
-    x_in = np.logical_and(x>=bbox.xmin, x<=bbox.xmax)
-    y_in = np.logical_and(y>=bbox.ymin, y<=bbox.ymax)
-    mask = x_in & y_in
-    return np.any(mask), mask
-
-def __bbox_overlap(bbox1, bbox2):
-    x_overlap = (bbox1.xmax >= bbox2.xmin) and (bbox1.xmin <= bbox2.xmax)
-    y_overlap = (bbox1.ymax >= bbox2.ymin) and (bbox1.ymin <= bbox2.ymax)
-    return x_overlap and y_overlap
-
-__cached_points = {}
-__cached_pointsd = {}
-
-def __overlap(ax, obj, objs, debug=False):
-    global __cached_points
-    fig = ax.get_figure()
-    renderer = fig.canvas.get_renderer()
-    tr = ax.transData
-#    tri = tr.inverted()
-    r = obj.get_window_extent(renderer) # got object bbox
-    for o in objs:
-        if type(o) is mpl.lines.Line2D:
-            if o in __cached_points:
-                xy = __cached_points[o]
-                xyd = __cached_pointsd[o]
-            else:
-                xyd = np.vstack(o.get_data()).T # retriev data in data coordinates
-                xy = tr.transform(xyd) # retrieve data in pixel coordinates
-                __cached_points[o] = xy
-                __cached_pointsd[o] = xyd
-            isin, ins = __points_in_bbox(xy[:,0],xy[:,1],r)
-            if isin:
-                if debug: ax.plot(xyd[:,0][ins],xyd[:,1][ins],'rx')
-                return o
-        else:
-            ro = o.get_window_extent(renderer)
-            if __bbox_overlap(r,ro):
-                return o
-    return False
-
-def color_frame(ax, color, sx = 0.01, sy=None, lw = 5, **kargs):
-    if sy is None:
-        sy = sx
-    import matplotlib as mpl
-    fig = plt.gcf()
-    fig.patches.append(mpl.patches.Rectangle((-sx,-sy), 1+2*sx,1+2*sy, transform=ax.transAxes, ec=color, fill=False, lw=lw, zorder=0, **kargs))
-
-def __get_yextend_of_curve(ax, bbox, curve):
-    tri = ax.transData.inverted()
-    rd = bbox.transformed(tri) # bbox in data coordinates
-    x, y = curve.get_data()
-    mask = (x>=rd.xmin)*(x<=rd.xmax)
-    if len(y[mask])==0:
-        return (0,0)
-    return (np.min(y[mask]), np.max(y[mask]))
-
-
-def put_Xlabels(ax, pos, labels, colors='rgb', debug=False, save=False, bbox=False, **kargs):
-    fig = ax.get_figure()
-    renderer = fig.canvas.get_renderer()
-    P = list(zip(pos, labels))
-    P.sort(key=lambda x: x[0]) # sort labels by ascending x
-    labs = []
-    ax.draw(renderer) # make sure to draw the new object
-    ylim = ax.get_ylim()
-    objs = [o for o in ax.get_children() if type(o) not in [mpl.patches.Rectangle]]
-    coli = [None, None]
-    for i, (x, lab) in enumerate(P):
-        col = colors[i%len(colors)]
-        pos = offset_coord((x, ylim[0]), (3, 0), ax=ax)
-        labs.append(ax.text(pos[0], pos[1], lab, va='bottom', ha='left', rotation=90, color=col))
-        ax.axvline(x, color=col, linestyle=kargs.get('linestyle','-'), alpha=kargs.get('line_alpha',.5))
-        ax.draw(renderer) # make sure to draw the new object
-        r = labs[-1].get_window_extent(renderer) # get the Bbox of the last label
-        ov = __overlap(ax, labs[-1], objs+labs[:-1])
-        if save:
-            if ov:
-                r1 = r.transformed(ax.transData.inverted())
-                r2 = ov.get_window_extent(renderer).transformed(ax.transData.inverted())
-                print(repr(ov), r2.ymin, r2.ymax)
-                coli[0] = mpl.patches.Rectangle((r1.xmin, r1.ymin), r1.xmax-r1.xmin, r1.ymax-r1.ymin, ec='b', fill=False)                
-                coli[1] = mpl.patches.Rectangle((r2.xmin, r2.ymin), r2.xmax-r2.xmin, r2.ymax-r2.ymin, ec='r', fill=False)
-
-                ax.add_patch(coli[0])
-                ax.add_patch(coli[1])
-            fig.savefig("put_Xlabels_{:03d}_000.png".format(i))
-            if ov:
-                coli[0].remove()
-                coli[1].remove()
-        last_ov = ov
-        y_offset = 0
-        it = 0
-        while ov:
-            it += 1
-            if debug: print("Label \"{}\" overlap with {}".format(labs[-1].get_text(), repr(ov)))
-            if type(ov) is mpl.lines.Line2D:
-                new_y = __get_yextend_of_curve(ax, r, ov)[1]
-            else:
-                rov = ov.get_window_extent(renderer).transformed(ax.transData.inverted())
-                new_y = rov.ymax
-            if ov == last_ov:
-                y_offset += kargs.get('offset_step', 5)
-                if y_offset > kargs.get('offset_step', 5)*kargs.get('max_iteration', 6):
-                    break
-            else:
-                y_offset = kargs.get('offset_step', 5)
-            last_ov = ov
-            new_xy_px = ax.transData.transform((x,new_y))+np.array([3,y_offset])
-            new_xy = ax.transData.inverted().transform(new_xy_px) # Offset the new_y of 5 pixels
-            labs[-1].set_position(new_xy)
-            ax.draw(renderer)
-            ov = __overlap(ax, labs[-1], objs+labs[:-1], debug=debug)
-            if save:
-                ax.draw(renderer)
-                fig.savefig("put_Xlabels_{:03d}_{:03d}.png".format(i,it))
-                if ov:
-                    r2 = ov.get_window_extent(renderer) # get the Bbox of the last label
-                    mpl.patches.draw_bbox(r, renderer, color='r')
-                    mpl.patches.draw_bbox(r2, renderer, color='r')
-    if bbox:
-        ax.draw(renderer)
-        for o in objs:
-            if type(o) is not mpl.lines.Line2D:
-                r = o.get_window_extent(renderer).transformed(ax.transData.inverted())
-                ax.add_patch(
-                        mpl.patches.Rectangle((r.xmin,r.ymin), r.xmax-r.xmin, r.ymax-r.ymin, ec='r', fill=False)
-                        )
-
-        for l in labs:
-            r = l.get_window_extent(renderer).transformed(ax.transData.inverted())
-            ax.add_patch(
-                    mpl.patches.Rectangle((r.xmin,r.ymin), r.xmax-r.xmin, r.ymax-r.ymin, ec='b', fill=False)
-                    )
+# -- coding: utf-8 --
+# -- coding: utf-8 --
+
+# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
+
+"""
+Various helper function for plotting data with matplotlib
+"""
+
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+import numpy as np
+
+from .misc import alias
+
+
+@alias("plot_mask")
+def plotMask(ax, mask, color, **kargs):
+    """
+    Create an overlay of a given color where mask is True.
+    The transparency and other parameters can be adjusted with **kargs. see help(plt.imshow)
+    
+    ax: matplotlib axis
+    mask: An array with value True where the mask should be plotted
+    color: color of the mask
+    **kargs: dictionnary of arguments which can be passed to imshow. Useful is mainly: alpha
+    """
+    import copy
+    m = np.ma.masked_array(mask, ~mask)
+    palette = copy.copy(plt.cm.gray)
+    palette.set_over(color, 1.0)
+    ax.imshow(m, cmap=palette, vmin=0, vmax=0.5, **kargs)
+
+
+def offset_coord(xy, offset=(0, 0), ax=None, fig=None, unit='px'):
+    if ax is None:
+        ax = plt.gca()
+
+    if fig is None:
+        fig = plt.gcf()
+
+    tr = ax.transData
+    tri = tr.inverted()
+
+    if unit == 'px':
+        offset = np.array(offset)
+    elif unit == 'ax':
+        offset = ax.transAxes.transform(offset)
+    elif unit == 'fig':
+        offset = fig.transFigure.transform(offset)
+    return tri.transform(tr.transform(xy) + offset)
+
+
+def Xdist(ax, left, right, y, color='r', linestyle=':', fmt="{dist:.1f}{unit}", xtransf=lambda x: x, va='bottom',
+          ha='center', offset=(0, 2), **kargs):
+    """
+    Show the distance between to x-values
+    
+    ax: matplotlib axis
+    left: x-value of the left mark
+    right: x-value of the right mark
+    y: height of the label
+    color: color of the lines / labels
+    linestyle: linestyle of the vertical lines
+    fmt: Format string to parse the distance
+    xtransf: a function can be passed to display the distance in an other unit that the x axis.
+        example: xtransf=lambda x: x*1e3 to display the distance in nm on an axis that uses micro-meters.
+    va: vertical alignment of the distance label
+    ha: horizontal alignment of the distance label
+    offset: (x,y) offset of the label in pixels
+    **kargs: additional arguments.
+        arguments starting with amn_ will be sent to the annotation
+        arguments starting with arr_ will be sent to the arrow
+        for example arr_color='r', ann_color='b' will display a red arrow with the distance in blue
+    """
+
+    ax.axvline(left, color=color, linestyle=linestyle)
+    ax.axvline(right, color=color, linestyle=linestyle)
+    ann = dict(va=va, ha=ha, color=color)
+    ann.update({k[3:]: kargs[k] for k in kargs if k.startswith('an_')})
+    ax.annotate(fmt.format(dist=xtransf(right - left), unit=kargs.get('unit', '')),
+                ({'center': .5 * (left + right), 'left': right, 'right': left}[ann['ha']], y), offset,
+                textcoords='offset pixels', **ann)
+    arr = dict(arrowstyle='<->', color=color)
+    arr.update({k[4:]: kargs[k] for k in kargs if k.startswith('arr_')})
+    ax.annotate("", (left, y), (right, y), arrowprops=arr)
+
+
+def Ydist(ax, down, up, x, color='r', linestyle=':', fmt="{dist:.2f}{unit}", ytransf=lambda y: y, rotation=90,
+          va='center', ha='right', offset=(-2, 0), **kargs):
+    """
+    Show the distance between to x-values
+    
+    ax: matplotlib axis
+    down: y-value of the bottom mark
+    up: y-value of the top mark
+    x: gorizontal position of the label
+    color: color of the lines / labels
+    linestyle: linestyle of the vertical lines
+    fmt: Format string to parse the distance
+    xtransf: a function can be passed to display the distance in an other unit that the x axis.
+        example: xtransf=lambda x: x*1e3 to display the distance in nm on an axis that uses micro-meters.
+    va: vertical alignment of the distance label
+    ha: horizontal alignment of the distance label
+    offset: (x,y) offset of the label in pixels
+    **kargs: additional arguments.
+        arguments starting with amn_ will be sent to the annotation
+        arguments starting with arr_ will be sent to the arrow
+        for example arr_color='r', ann_color='b' will display a red arrow with the distance in blue
+    """
+
+    ax.axhline(down, color=color, linestyle=linestyle)
+    ax.axhline(up, color=color, linestyle=linestyle)
+    ann = dict(va=va, ha=ha, color=color)
+    ann.update({k[3:]: kargs[k] for k in kargs if k.startswith('an_')})
+    ax.annotate(fmt.format(dist=ytransf(up - down), unit=kargs.get('unit', '')),
+                (x, {'center': .5 * (down + up), 'top': up, 'bottom': down}[ann['va']]), offset,
+                textcoords='offset pixels', rotation=rotation, **ann)
+    arr = dict(arrowstyle='<->', color=color)
+    arr.update({k[4:]: kargs[k] for k in kargs if k.startswith('arr_')})
+    ax.annotate("", (x, down), (x, up), arrowprops=arr)
+
+
+@alias("DualPlot")
+def dual_plot(ax, col1='C0', col2='C1'):
+    """
+    Create a dual axis from ax and tune the color of the left/right axes to col1, col2 resp.
+    """
+    axb = ax.twinx()
+    axb.spines['left'].set_color(col1)
+    axb.spines['right'].set_color(col2)
+    ax.yaxis.label.set_color(col1)
+    axb.yaxis.label.set_color(col2)
+    ax.tick_params(axis='y', colors=col1)
+    axb.tick_params(axis='y', colors=col2)
+    return axb
+
+
+def sp(M, N=1, W=21, ravel=True, fig=False):
+    """
+    Shortcut for creating subplots with max width = W (default 21,
+        which seems to correspond to 100% of the width in jupyter).
+    Height is calculated in order to have square subplots.
+    The layout is given by M columns and N lines.
+    If N is negative, abs(N) is interpreted as the number of elements and the number of line will be calculated automatically in function of M.
+    """
+    if N < 0:
+        tot = -N
+        N = 1 + (tot - 1) // M
+    f, ax = plt.subplots(N, M, figsize=(W, N * W / M))
+    if ravel:
+        if fig:
+            return np.ravel(ax), f
+        return np.ravel(ax)
+    if fig:
+        return ax, f
+    return ax
+
+
+def get_rect(img, bottom, top, left, right, ax, color='r'):
+    """
+    return a sub-area on a 2D-array img and display the boundaries on a matplotlib axis ax
+    """
+    ax.axhline(bottom, color=color)
+    ax.axhline(top, color=color)
+    ax.axvline(left, color=color)
+    ax.axvline(right, color=color)
+    return img[bottom:top, left:right]
+
+
+def sublegend(*ax, **kargs):
+    labels = kargs.get('labels', None)
+    color = kargs.get('color', 'white')
+    margin = kargs.get('margin', 9)
+    titles = kargs.get('titles', None)
+    fontsize = kargs.get('fontsize', 14)
+    """
+    ax: list of axes
+    labels: If None, the will be a, b, c, d, ...
+    color: background color of the rectangle
+    margin: margin in pixel from the axis border
+    titles: set to False to remove all titles. (Useful to keep the set_title info in the code to remember what is plotted)
+    fontsize: The font size of the labels
+    """
+    props = dict(boxstyle='round', facecolor=color, alpha=1)
+    if not hasattr(margin, "__getitem__") and not hasattr(margin, "__iter__"):
+        margin = (margin, margin)
+
+    if labels is None:
+        labels = [chr(ord('a') + i) for i, _ in enumerate(np.ravel(ax))]
+    for i, a in enumerate(np.ravel(ax)):
+        if titles is False:
+            a.set_title("")
+        a.annotate(labels[i], (0, 1), xytext=(margin[0], -margin[1]), fontsize=fontsize, verticalalignment='top',
+                   bbox=props, xycoords='axes fraction', textcoords='offset pixels');
+
+
+def formula(x):
+    import re
+    x = re.sub('_([0-9]+)', r'$_{\1}$', x)
+    x = re.sub(r'\^([0-9\+\-]+)', r'$^{\1}$', x)
+    return x
+
+
+def _points_in_bbox(x, y, bbox):
+    x_in = np.logical_and(x >= bbox.xmin, x <= bbox.xmax)
+    y_in = np.logical_and(y >= bbox.ymin, y <= bbox.ymax)
+    mask = x_in & y_in
+    return np.any(mask), mask
+
+
+def _bbox_overlap(bbox1, bbox2):
+    x_overlap = (bbox1.xmax >= bbox2.xmin) and (bbox1.xmin <= bbox2.xmax)
+    y_overlap = (bbox1.ymax >= bbox2.ymin) and (bbox1.ymin <= bbox2.ymax)
+    return x_overlap and y_overlap
+
+
+_cached_points = {}
+_cached_pointsd = {}
+
+
+def _overlap(ax, obj, objs, debug=False):
+    global _cached_points
+    fig = ax.get_figure()
+    renderer = fig.canvas.get_renderer()
+    tr = ax.transData
+    #    tri = tr.inverted()
+    r = obj.get_window_extent(renderer)  # got object bbox
+    for o in objs:
+        if type(o) is mpl.lines.Line2D:
+            if o in _cached_points:
+                xy = _cached_points[o]
+                xyd = _cached_pointsd[o]
+            else:
+                xyd = np.vstack(o.get_data()).T  # retriev data in data coordinates
+                xy = tr.transform(xyd)  # retrieve data in pixel coordinates
+                _cached_points[o] = xy
+                _cached_pointsd[o] = xyd
+            isin, ins = _points_in_bbox(xy[:, 0], xy[:, 1], r)
+            if isin:
+                if debug: ax.plot(xyd[:, 0][ins], xyd[:, 1][ins], 'rx')
+                return o
+        else:
+            ro = o.get_window_extent(renderer)
+            if _bbox_overlap(r, ro):
+                return o
+    return False
+
+
+def color_frame(ax, color, sx=0.01, sy=None, lw=5, **kargs):
+    if sy is None:
+        sy = sx
+    import matplotlib as mpl
+    fig = plt.gcf()
+    fig.patches.append(
+        mpl.patches.Rectangle((-sx, -sy), 1 + 2 * sx, 1 + 2 * sy, transform=ax.transAxes, ec=color, fill=False, lw=lw,
+                              zorder=0, **kargs))
+
+
+def _get_yextend_of_curve(ax, bbox, curve):
+    tri = ax.transData.inverted()
+    rd = bbox.transformed(tri)  # bbox in data coordinates
+    x, y = curve.get_data()
+    mask = (x >= rd.xmin) * (x <= rd.xmax)
+    if len(y[mask]) == 0:
+        return (0, 0)
+    return (np.min(y[mask]), np.max(y[mask]))
+
+
+def put_Xlabels(ax, pos, labels, colors='rgb', debug=False, save=False, bbox=False, **kargs):
+    fig = ax.get_figure()
+    renderer = fig.canvas.get_renderer()
+    P = list(zip(pos, labels))
+    P.sort(key=lambda x: x[0])  # sort labels by ascending x
+    labs = []
+    ax.draw(renderer)  # make sure to draw the new object
+    ylim = ax.get_ylim()
+    objs = [o for o in ax.get_children() if type(o) not in [mpl.patches.Rectangle]]
+    coli = [None, None]
+    for i, (x, lab) in enumerate(P):
+        col = colors[i % len(colors)]
+        pos = offset_coord((x, ylim[0]), (3, 0), ax=ax)
+        labs.append(ax.text(pos[0], pos[1], lab, va='bottom', ha='left', rotation=90, color=col))
+        ax.axvline(x, color=col, linestyle=kargs.get('linestyle', '-'), alpha=kargs.get('line_alpha', .5))
+        ax.draw(renderer)  # make sure to draw the new object
+        r = labs[-1].get_window_extent(renderer)  # get the Bbox of the last label
+        ov = _overlap(ax, labs[-1], objs + labs[:-1])
+        if save:
+            if ov:
+                r1 = r.transformed(ax.transData.inverted())
+                r2 = ov.get_window_extent(renderer).transformed(ax.transData.inverted())
+                print(repr(ov), r2.ymin, r2.ymax)
+                coli[0] = mpl.patches.Rectangle((r1.xmin, r1.ymin), r1.xmax - r1.xmin, r1.ymax - r1.ymin, ec='b',
+                                                fill=False)
+                coli[1] = mpl.patches.Rectangle((r2.xmin, r2.ymin), r2.xmax - r2.xmin, r2.ymax - r2.ymin, ec='r',
+                                                fill=False)
+
+                ax.add_patch(coli[0])
+                ax.add_patch(coli[1])
+            fig.savefig("put_Xlabels_{:03d}_000.png".format(i))
+            if ov:
+                coli[0].remove()
+                coli[1].remove()
+        last_ov = ov
+        y_offset = 0
+        it = 0
+        while ov:
+            it += 1
+            if debug: print("Label \"{}\" overlap with {}".format(labs[-1].get_text(), repr(ov)))
+            if type(ov) is mpl.lines.Line2D:
+                new_y = _get_yextend_of_curve(ax, r, ov)[1]
+            else:
+                rov = ov.get_window_extent(renderer).transformed(ax.transData.inverted())
+                new_y = rov.ymax
+            if ov == last_ov:
+                y_offset += kargs.get('offset_step', 5)
+                if y_offset > kargs.get('offset_step', 5) * kargs.get('max_iteration', 6):
+                    break
+            else:
+                y_offset = kargs.get('offset_step', 5)
+            last_ov = ov
+            new_xy_px = ax.transData.transform((x, new_y)) + np.array([3, y_offset])
+            new_xy = ax.transData.inverted().transform(new_xy_px)  # Offset the new_y of 5 pixels
+            labs[-1].set_position(new_xy)
+            ax.draw(renderer)
+            ov = _overlap(ax, labs[-1], objs + labs[:-1], debug=debug)
+            if save:
+                ax.draw(renderer)
+                fig.savefig("put_Xlabels_{:03d}_{:03d}.png".format(i, it))
+                if ov:
+                    r2 = ov.get_window_extent(renderer)  # get the Bbox of the last label
+                    mpl.patches.draw_bbox(r, renderer, color='r')
+                    mpl.patches.draw_bbox(r2, renderer, color='r')
+    if bbox:
+        ax.draw(renderer)
+        for o in objs:
+            if type(o) is not mpl.lines.Line2D:
+                r = o.get_window_extent(renderer).transformed(ax.transData.inverted())
+                ax.add_patch(
+                    mpl.patches.Rectangle((r.xmin, r.ymin), r.xmax - r.xmin, r.ymax - r.ymin, ec='r', fill=False)
+                )
+
+        for l in labs:
+            r = l.get_window_extent(renderer).transformed(ax.transData.inverted())
+            ax.add_patch(
+                mpl.patches.Rectangle((r.xmin, r.ymin), r.xmax - r.xmin, r.ymax - r.ymin, ec='b', fill=False)
+            )
+
+
+def stdplot(x, y, Nsig=2, ax=None, color='b', axis=1, **kargs):
+    """
+    Plot the mean / standard-deviation for a signal
+    
+    x: 1D numpy.ndarrayx
+        x values
+    y: 2D numpy.ndarray
+        y values. One of the two axis is used for the statistics
+    Nsig: int
+        The number of standard-deviations to display
+    axis: int
+        which axis is used to calculate mean/std
+    ax: matplotlib axis
+        maplotlib axis to plot in
+    color: string
+        color of the line
+    **kargs: arguments passed to plot
+    
+    """
+    if ax is None:
+        ax = plt.gca()
+    dy = np.std(y, axis=axis)
+    mean = np.mean(y, axis=axis)
+    ax.plot(x, mean, color=color, **kargs)
+    for i in range(1, Nsig + 1):
+        ax.fill_between(x, mean - i * dy, mean + i * dy, color=color, alpha=.2)
+
+
+def pixel2img(xy, ax=None):
+    """
+    Plot create by SPM.show can be either in pixels or real unit.
+    This function return the input in case the plot is in pixels
+    or calculate and return the real unit coordinate of the corresponding pixel.
+    """
+    import matplotlib.pyplot as plt
+    if ax is None:
+        ax = plt.gca()
+
+    if hasattr(ax, 'isPixel'):
+        if not ax.isPixel:
+            pixel_shape = ax.images[0].get_array().shape
+            extent = ax.images[0].get_extent()
+            eW = extent[1] - extent[0]
+            eH = extent[3] - extent[2]
+            return (xy[0] * eW / pixel_shape[1], xy[1] * eH / pixel_shape[0])
+    return xy
```

### Comparing `pySPM-0.2.9/pySPM/utils/save.py` & `pyspm-0.3.0/pySPM/utils/save.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,185 +1,209 @@
-# -- coding: utf-8 --
-
-# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
-
-import pickle
-import zipfile
-import os
-import shutil
-import tempfile
-
-"""
-This small utility can save and load python objects to a single file.
-It uses ZIP DEFLATE compression method in order to keep the file small.
-It works in a similar way as numpy.savez_compressed and numpy.load, but
-just work with any python objects and thus do not generate a numpy.array
-for every object. Several objects can be added to the same file with either one call of save or several.
-The new data will just be appended to your file. It also support the update of the file (in this case the data file is copied in a new one).
-
-the default file extension is pkz (for Pickle Zip)
-"""
-
-data_path = '.'
-
-def set_datapath(path):
-    global data_path
-    data_path = path
-
-def findPKZ(filename):
-    if os.path.splitext(filename)[1]=='':
-        filename += '.pkz'
-    p2 = os.path.join(data_path, filename)
-    if os.path.exists(p2):
-        return p2
-    if os.path.exists(filename):
-        return filename
-    if not os.path.exists(filename):
-        raise IOError("File \"{}\" not found".format(filename))
-    return filename
-        
-        
-def save(filename, *objs, **obj):
-    """
-    save python objects to file
-    """
-    if os.path.splitext(filename)[1]=='':
-        filename += '.pkz'
-    filename = os.path.join(data_path, filename)
-    out = zipfile.ZipFile(filename, 'a', zipfile.ZIP_DEFLATED)
-    file_list = out.namelist()
-    update = []
-    for i,o in enumerate(objs):
-        obj[i] = o
-        
-    # List objects which are already present in the file (so which will be updated)
-    for k in obj:
-        if k in file_list:
-            update.append(k)
-            
-    if len(update) == 0 : # No files are updated, just append the new data to the file
-        for k in obj:
-            out.writestr(k, pickle.dumps(obj[k], pickle.HIGHEST_PROTOCOL))
-    else:
-        # close the current file, copy it to a temp file and reopen the original file in write mode (will thus override all data)
-        out.close()
-        ft, temp = tempfile.mkstemp()
-        shutil.copy(filename, temp)
-        out = zipfile.ZipFile(filename , 'w', zipfile.ZIP_DEFLATED)
-        
-        # Copy all old data which are not updated and clean tempfile
-        old = zipfile.ZipFile(temp, 'r')
-        for k in [x for x in file_list if x not in update]:
-            out.writestr(k, old.read(k))
-        old.close()
-        os.fdopen(ft).close()
-        os.remove(temp)
-        
-        # Write all new objects
-        for k in obj:
-            out.writestr(k, pickle.dumps(obj[k], pickle.HIGHEST_PROTOCOL))
-    out.close()
-    
-def load(filename, *keys):
-    """
-    load python objects from saved pkz files
-    """
-    filename = findPKZ(filename)
-    if len(keys) == 0:
-        keys = ['0']
-    elif len(keys) == 1 and ',' in keys[0]:
-        keys = keys[0].split(',')
-    f = zipfile.ZipFile(filename, 'r')
-    res = []
-    for key in keys:
-        if type(key) is int:
-            key = str(key)
-        res.append(pickle.loads(f.read(key)))
-    f.close()
-    if len(keys)==1:
-        return res[0]
-    return res
-    
-class loader:
-    """
-    This class act as a dictionary and read default value for compressed pkz files.
-    Values can be set to new values without changing the content of the saved data.
-    Only retrieved data are kept in memory and not all the data.
-    """
-    def __init__(self, filename):
-        self.filename = findPKZ(filename)
-        self.local = {}
-    
-    def __iter__(self):
-        f = zipfile.ZipFile(self.filename, 'r')
-        self.keys = set(f.namelist()+list(self.local.keys()))
-        f.close()
-        return self
-        
-    def __next__(self):
-        if len(self.keys) == 0:
-            raise StopIteration()
-        else:
-            return self.keys.pop()
-        
-    def __getitem__(self, key):
-        if not key in self.local:
-            f = zipfile.ZipFile(self.filename, 'r')
-            self.local[key] = pickle.loads(f.read(key))
-            f.close()
-        return self.local[key]
-    
-    def __setitem__(self, key, value):
-        self.local[key] = value
-        
-    def __delitem__(self, key):
-        delf.local.delitem(key)
-        
-class BidirData:
-    """
-    This class act as a dictionary and read default value for compressed pkz files.
-    Values can be set to new values without changing the content of the saved data.
-    Only retrieved data are kept in memory and not all the data.
-    """
-    def __init__(self, filename):
-        try:
-            self.filename = findPKZ(filename)
-        except IOError:
-            if os.path.splitext(filename)[1]=='':
-                filename += '.pkz'
-            self.filename = os.path.join(data_path, filename)
-            out = zipfile.ZipFile(filename, 'a', zipfile.ZIP_DEFLATED)
-            out.close()
-        self.local = {}
-    
-    def __iter__(self):
-        f = zipfile.ZipFile(self.filename, 'r')
-        self.keys = set(f.namelist()+list(self.local.keys()))
-        f.close()
-        return self
-        
-    def __next__(self):
-        if len(self.keys) == 0:
-            raise StopIteration()
-        else:
-            return self.keys.pop()
-        
-    def __getitem__(self, key):
-        if not key in self.local:
-            f = zipfile.ZipFile(self.filename, 'r')
-            self.local[key] = pickle.loads(f.read(key))
-            f.close()
-        return self.local[key]
-    
-    def __setitem__(self, key, value):
-        self.local[key] = value
-        save(self.filename, **{key:value})
-        
-    def __delitem__(self, key):
-        delf.local.delitem(key)
-        
-    def keys(self):
-        f = zipfile.ZipFile(self.filename, 'r')
-        keys = f.filelist
-        f.close()
-        return [x.filename for x in keys]
-        
+# -- coding: utf-8 --
+
+# Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
+
+import os
+import pickle
+import shutil
+import tempfile
+import zipfile
+
+"""
+This small utility can save and load python objects to a single file.
+It uses ZIP DEFLATE compression method in order to keep the file small.
+It works in a similar way as numpy.savez_compressed and numpy.load, but
+just work with any python objects and thus do not generate a numpy.array
+for every object. Several objects can be added to the same file with either one call of save or several.
+The new data will just be appended to your file. It also support the update of the file (in this case the data file is copied in a new one).
+
+the default file extension is pkz (for Pickle Zip)
+"""
+
+data_path = '.'
+
+
+def set_datapath(path):
+    global data_path
+    data_path = path
+
+
+def findPKZ(filename):
+    if os.path.splitext(filename)[1] == '':
+        filename += '.pkz'
+    p2 = os.path.join(data_path, filename)
+    if os.path.exists(p2):
+        return p2
+    if os.path.exists(filename):
+        return filename
+    if not os.path.exists(filename):
+        raise IOError("File \"{}\" not found".format(filename))
+    return filename
+
+
+def inarxiv(filename, obj):
+    if os.path.splitext(filename)[1] == '':
+        filename += '.pkz'
+    filename = os.path.join(data_path, filename)
+    out = zipfile.ZipFile(filename, 'a', zipfile.ZIP_DEFLATED)
+    file_list = out.namelist()
+    return obj in file_list
+
+
+def save(filename, *objs, **obj):
+    """
+    save python objects to file
+    """
+    if os.path.splitext(filename)[1] == '':
+        filename += '.pkz'
+    filename = os.path.join(data_path, filename)
+    out = zipfile.ZipFile(filename, 'a', zipfile.ZIP_DEFLATED)
+    file_list = out.namelist()
+    update = []
+    for i, o in enumerate(objs):
+        obj[i] = o
+
+    # List objects which are already present in the file (so which will be updated)
+    for k in obj:
+        if k in file_list:
+            update.append(k)
+
+    if len(update) == 0:  # No files are updated, just append the new data to the file
+        for k in obj:
+            out.writestr(k, pickle.dumps(obj[k], pickle.HIGHEST_PROTOCOL))
+    else:
+        # close the current file, copy it to a temp file and reopen the original file in write mode (will thus override all data)
+        out.close()
+        ft, temp = tempfile.mkstemp()
+        shutil.copy(filename, temp)
+        out = zipfile.ZipFile(filename, 'w', zipfile.ZIP_DEFLATED)
+
+        # Copy all old data which are not updated and clean tempfile
+        old = zipfile.ZipFile(temp, 'r')
+        for k in [x for x in file_list if x not in update]:
+            out.writestr(k, old.read(k))
+        old.close()
+        os.fdopen(ft).close()
+        os.remove(temp)
+
+        # Write all new objects
+        for k in obj:
+            out.writestr(k, pickle.dumps(obj[k], pickle.HIGHEST_PROTOCOL))
+    out.close()
+
+
+def load(filename, *keys):
+    """
+    load python objects from saved pkz files
+    """
+    filename = findPKZ(filename)
+    if len(keys) == 0:
+        keys = ['0']
+    elif len(keys) == 1 and ',' in keys[0]:
+        keys = keys[0].split(',')
+    f = zipfile.ZipFile(filename, 'r')
+
+    res = []
+    for key in keys:
+        if type(key) is int:
+            key = str(key)
+        try:
+            raw = f.read(key)
+        except Exception as e:
+            raise KeyError("There is no key {} found in the data {}".format(key, filename))
+        try:
+            res.append(pickle.loads(raw))
+        except:
+            raise Exception("Cannot pickle recorded data for key {}".format(key))
+
+    f.close()
+    if len(keys) == 1:
+        return res[0]
+    return res
+
+
+class loader:
+    """
+    This class act as a dictionary and read default value for compressed pkz files.
+    Values can be set to new values without changing the content of the saved data.
+    Only retrieved data are kept in memory and not all the data.
+    """
+
+    def __init__(self, filename):
+        self.filename = findPKZ(filename)
+        self.local = {}
+
+    def __iter__(self):
+        f = zipfile.ZipFile(self.filename, 'r')
+        self.keys = set(f.namelist() + list(self.local.keys()))
+        f.close()
+        return self
+
+    def __next__(self):
+        if len(self.keys) == 0:
+            raise StopIteration()
+        else:
+            return self.keys.pop()
+
+    def __getitem__(self, key):
+        if not key in self.local:
+            f = zipfile.ZipFile(self.filename, 'r')
+            self.local[key] = pickle.loads(f.read(key))
+            f.close()
+        return self.local[key]
+
+    def __setitem__(self, key, value):
+        self.local[key] = value
+
+    def __delitem__(self, key):
+        del self.local[key]
+
+
+class BidirData:
+    """
+    This class act as a dictionary and read default value for compressed pkz files.
+    Values can be set to new values without changing the content of the saved data.
+    Only retrieved data are kept in memory and not all the data.
+    """
+
+    def __init__(self, filename):
+        try:
+            self.filename = findPKZ(filename)
+        except IOError:
+            if os.path.splitext(filename)[1] == '':
+                filename += '.pkz'
+            self.filename = os.path.join(data_path, filename)
+            out = zipfile.ZipFile(filename, 'a', zipfile.ZIP_DEFLATED)
+            out.close()
+        self.local = {}
+
+    def __iter__(self):
+        f = zipfile.ZipFile(self.filename, 'r')
+        self.keys = set(f.namelist() + list(self.local.keys()))
+        f.close()
+        return self
+
+    def __next__(self):
+        if len(self.keys) == 0:
+            raise StopIteration()
+        else:
+            return self.keys.pop()
+
+    def __getitem__(self, key):
+        if not key in self.local:
+            f = zipfile.ZipFile(self.filename, 'r')
+            self.local[key] = pickle.loads(f.read(key))
+            f.close()
+        return self.local[key]
+
+    def __setitem__(self, key, value):
+        self.local[key] = value
+        save(self.filename, **{key: value})
+
+    def __delitem__(self, key):
+        delf.local.delitem(key)
+
+    def keys(self):
+        f = zipfile.ZipFile(self.filename, 'r')
+        keys = f.filelist
+        f.close()
+        return [x.filename for x in keys]
```

### Comparing `pySPM-0.2.9/pySPM/utils/__init__.py` & `pyspm-0.3.0/pySPM/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # -- coding: utf-8 --
 
 # Copyright 2018 Olivier Scholder <o.scholder@gmail.com>
 
-import numpy as np
-from scipy import stats, optimize as opt
-import re
-import sqlite3
-from .math import *
-from .elts import *
+from . import fit, misc, colors
 from .constants import *
-from .spectra import *
+from .elts import *
+from .math import *
+from .misc import alias, PB
 from .plot import *
-from . import fit
-from .save import *
 from .restoration import *
+from .save import *
+from .spectra import *
+
 
 def funit(value, unit=None):
     """
     Convert a value and unit to proper value
     e.g. 0.01m will be converted to 10mm
     e.g. 1000A will be converted to 1kA
     etc.
@@ -45,174 +43,214 @@
     """
     if unit == None:
         unit = value['unit']
         value = value['value']
     import math
     if value == 0:
         return {'value': value, 'unit': unit}
-    shift = int(math.floor(math.log10(value)/3.0))  # base10 exponent
+    shift = int(math.floor(math.log10(value) / 3.0))  # base10 exponent
     mag = u'afpnum1kMGTPE'
     index_mag = mag.index('1')
     # Test if unit has a scale factor (n,m,k,M,G, etc.)
     if len(unit) > 1 and unit[0] in mag and unit[1:] and index_mag:
         index_mag = mag.index(unit[0])
         unit = unit[1:]
-    value /= 10**(3*shift)
+    value /= 10 ** (3 * shift)
     index_mag += shift
     if index_mag < 0:
-        value *= 10**(index_mag*3)
+        value *= 10 ** (index_mag * 3)
         index_mag = 0
     elif index_mag >= len(mag):
-        value *= 10**((index_mag-len(mag)+1)*3)
-        index_mag = len(mag)-1
+        value *= 10 ** ((index_mag - len(mag) + 1) * 3)
+        index_mag = len(mag) - 1
     unit_prefix = mag[index_mag]
     if unit_prefix == '1':
         unit_prefix = ''
     return {'value': value, 'unit': u'{mag}{unit}'.format(mag=unit_prefix, unit=unit)}
+
+
+def get_shifts_bbox(shifts, shape):
+    """
+    Return the bounding-box of the overlapping area of scans which have a thermal drift given by shifts.
+    Return: dictionary with the top, left, right, bottom position
     
+    Parameters
+    ----------
+    shifts: list of tuple [(dx0, dy0), (dx1, dy1), ..., (dxN, dyN)]
+        list of tuple given the shift for each scan in pixel in the x- and y-direction.
+        The number of element should equal the number of scans (so N=Nscan-1)
+    shape: tuple (Height, Width)
+        shape of the image.
+    """
+    from .geometry import Bbox
+    right = shape[1] + min(0, np.min([x[0] for x in shifts]))
+    left = np.max([x[0] for x in shifts])
+    top = shape[0] + min(0, np.min([x[1] for x in shifts]))
+    bottom = np.max([x[1] for x in shifts])
+    return Bbox(right=right, left=left, top=top, bottom=bottom)
+
+
 def s2hms(s):
     """Convert seconds to hour, minutes or seconds"""
     M = np.max(s)
-    if M>120*60:
-        return s/(60*60), 'h'
-    if M>300:
-        return s/60, 'min'
+    if M > 120 * 60:
+        return s / (60 * 60), 'h'
+    if M > 300:
+        return s / 60, 'min'
     return s, 's'
 
+
 def time2hms(s, string=True):
-    h = int(s//3600)
-    s -= h*3600
-    m = int(s//60)
-    s -= m*60
+    h = int(s // 3600)
+    s -= h * 3600
+    m = int(s // 60)
+    s -= m * 60
     if string:
-        return "{:02d}:{:02d}:{:02.2f}".format(h,m,s)
-    return (h,m,s)
-    
-def fitSpectrum(t, m, error=False):
+        return "{:02d}:{:02d}:{:02.2f}".format(h, m, s)
+    return (h, m, s)
+
+
+@alias("fitSpectrum")
+def fit_spectrum(t, m, error=False):
     """
     fit and return the sf and k0 parameters for given known times t and masses m
     """
     M = np.sqrt(np.array(m))
-    T = np.hstack([np.array(t)[:,None],np.ones((len(t),1))])
-    x = np.linalg.lstsq(T,M,rcond=-1)[0]
-    sf = 1/x[0]
-    k0 = -sf*x[1]
+    T = np.hstack([np.array(t)[:, None], np.ones((len(t), 1))])
+    x = np.linalg.lstsq(T, M, rcond=-1)[0]
+    sf = 1 / x[0]
+    k0 = -sf * x[1]
     res = [sf, k0]
     if error:
         mfit = np.dot(T, x)
         mresid = M - mfit
         X = np.dot(T.T, T)
         epsvar = np.var(mresid, ddof=2)
-        xvar = np.linalg.inv(X) * epsvar # correlation matrix
-        D = np.sqrt(np.diag(xvar)) # error vector
-        Dsf = D[0]/x[0]**2
-        Dk0 = np.sqrt((D[1]/x[0])**2+(x[1]*D[0]/x[0]**2)**2)
-        res.append(Dsf, Dk0)
+        xvar = np.linalg.inv(X) * epsvar  # correlation matrix
+        D = np.sqrt(np.diag(xvar))  # error vector
+        Dsf = np.abs(D[0] / x[0] ** 2)
+        Dk0 = np.sqrt((D[1] / x[0]) ** 2 + (x[1] * Dsf) ** 2)
+        res += [Dsf, Dk0]
     return res
 
+
 def chunks(l, n):
     """Yield successive n-sized chunks from l."""
     for i in range(0, len(l), n):
         yield l[i:i + n]
 
+
 def mass2time(m, sf, k0):
-    return sf*np.sqrt(m)+k0
+    """
+    Here the time is actually the number of channels.
+    To convert it to real time, you should multiply the answer by the Time Resolution which can be obtained by pySPM.ITM.get_value("Registration.TimeResolution")
+    """
+    r = m * 0 + k0
+    if not hasattr(r, '__setitem__'):
+        if m < 0:
+            return r
+        return sf * np.sqrt(m) + k0
+    r[m >= 0] = sf * np.sqrt(m[m >= 0]) + k0
+    return r
+
 
 def time2mass(t, sf, k0):
-    return ((t-k0)/sf)**2
+    """
+    Here the time t is actually the number of channels.
+    To convert a real time to the number of channel t, you should divide the real time by the Time Resolution which can be obtained by pySPM.ITM.get_value("Registration.TimeResolution")
+    """
+    return ((t - k0) / sf) ** 2
+
 
 def show_table(t):
     from IPython.core.display import display, HTML
     display(HTML(html_table(t)))
 
+
 def html_table(t, header=False):
     S = "<table>"
     if header:
-        S += "<tr>"+"".join(["<th>{0}</th>".format(x) for x in t[0]])+"</tr>"
+        S += "<tr>" + "".join(["<th>{0}</th>".format(x) for x in t[0]]) + "</tr>"
         t = t[1:]
     for x in t:
-        S += "<tr>"+"".join(["<td>{0}</td>".format(y) for y in x])+"</tr>"
+        S += "<tr>" + "".join(["<td>{0}</td>".format(y) for y in x]) + "</tr>"
     S += "</table>"
     return S
 
+
 def aa_table(t, header=False):
     """
     print a list of list in a nice ascii-art
     """
     Ncols = len(t[0])
-    Lcol = [0]*Ncols
+    Lcol = [0] * Ncols
     for x in t:
         for i in range(Ncols):
             Lcol[i] = max(Lcol[i], len(repr(x[i])))
     if header:
         print(
-            "  ".join([u"{: <"+str(Lcol[i]+4)+"}" for i in range(Ncols)]).format(*t[0]))
-        print("="*sum(Lcol))
+            "  ".join([u"{: <" + str(Lcol[i] + 4) + "}" for i in range(Ncols)]).format(*t[0]))
+        print("=" * sum(Lcol))
         t = t[1:]
     for j, x in enumerate(t):
-        print("  ".join([u"{:"+['.', '_'][j % 2]+"<" +
-                         str(Lcol[i]+4)+"}" for i in range(Ncols)]).format(*x))
+        print("  ".join([u"{:" + ['.', '_'][j % 2] + "<" +
+                         str(Lcol[i] + 4) + "}" for i in range(Ncols)]).format(*x))
+
 
 def dict_update(d, u):
     import collections
     for k, v in u.items():
         if isinstance(v, collections.Mapping):
             r = dict_update(d.get(k, {}), v)
             d[k] = r
         else:
             d[k] = u[k]
     return d
 
+
 def htmlTable(t, show=True, header=False):
     import html
     s = "<table><tr>"
     if header:
-        s += "<th>"+"</th><th>".join([html.escape(str(y))
-                                      for y in t[0]])+"</th></tr><tr>"
+        s += "<th>" + "</th><th>".join([html.escape(str(y))
+                                        for y in t[0]]) + "</th></tr><tr>"
         t = t[1:]
     s += "".join([
-        "<tr><td>"+"</td><td>".join([
-            html.escape(str(y)) for y in x]) + "</td></tr>" for x in t])+"</table>"
+        "<tr><td>" + "</td><td>".join([
+            html.escape(str(y)) for y in x]) + "</td></tr>" for x in t]) + "</table>"
     if show:
         from IPython.display import display, HTML
         display(HTML(s))
     else:
         return s
 
+
 def zfit_level(A, processes=4):
     import multiprocessing as mp
-    level = np.array(mp.Pool(processes).map(fitCDF1line, (A[:,i,:] for i in range(A.shape[1]))))
+    level = np.array(mp.Pool(processes).map(fitCDF1line, (A[:, i, :] for i in range(A.shape[1]))))
     return level
 
-def in_ipynb():
-    try:
-        cfg = get_ipython().config 
-        if 'IPKernelApp' in cfg:
-            return True
-        else:
-            return False
-    except NameError:
-        return False
 
 def getToFimg(I, N=100, prog=False):
     """
     Simulate obtained counts for N scans from an image
     """
     R = np.zeros(I.shape)
     L = range(N)
     if prog:
-        from tqdm import tqdm_notebook as tqdm
-        L = tqdm(L)
+        L = PB(L)
     for i in L:
-        R += (np.random.rand(*I.shape)<(1-np.exp(-I)))
+        R += (np.random.rand(*I.shape) < (1 - np.exp(-I)))
     return R
 
+
 def getToFsimg(I, N=[10, 50, 100, 300, 500], prog=False):
-    Ns = np.insert(np.diff(N),0,N[0])
+    Ns = np.insert(np.diff(N), 0, N[0])
     T = [getToFimg(I, n) for n in Ns]
-    return dict(zip(N,np.cumsum(T, axis=0)))
+    return dict(zip(N, np.cumsum(T, axis=0)))
+
 
 def centered_meshgrid(A):
     w = A.shape[1]
     h = A.shape[0]
-    Y, X = np.mgrid[-h//2:h//2,-w//2:w//2]
-    return Y,X
+    Y, X = np.mgrid[-h // 2:h // 2, -w // 2:w // 2]
+    return Y, X
```

