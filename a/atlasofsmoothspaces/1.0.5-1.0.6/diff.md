# Comparing `tmp/atlasofsmoothspaces-1.0.5.tar.gz` & `tmp/atlasofsmoothspaces-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlasofsmoothspaces-1.0.5.tar", last modified: Tue Apr 11 08:01:38 2023, max compression
+gzip compressed data, was "atlasofsmoothspaces-1.0.6.tar", last modified: Wed Apr 12 10:22:53 2023, max compression
```

## Comparing `atlasofsmoothspaces-1.0.5.tar` & `atlasofsmoothspaces-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 08:01:38.046491 atlasofsmoothspaces-1.0.5/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 08:01:38.046491 atlasofsmoothspaces-1.0.5/PKG-INFO
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 08:01:38.046491 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       19 2023-04-11 07:32:02.000000 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces/__init__.py
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)     7773 2023-04-11 08:01:20.000000 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces/main.py
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-11 08:01:38.046491 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces.egg-info/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-11 08:01:38.000000 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces.egg-info/PKG-INFO
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-11 08:01:38.000000 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces.egg-info/SOURCES.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-11 08:01:38.000000 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces.egg-info/dependency_links.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-11 08:01:38.000000 atlasofsmoothspaces-1.0.5/atlasofsmoothspaces.egg-info/top_level.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-11 08:01:38.046491 atlasofsmoothspaces-1.0.5/setup.cfg
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-11 08:01:33.000000 atlasofsmoothspaces-1.0.5/setup.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-12 10:22:53.579937 atlasofsmoothspaces-1.0.6/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-12 10:22:53.579937 atlasofsmoothspaces-1.0.6/PKG-INFO
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-12 10:22:53.579937 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       19 2023-04-11 07:32:02.000000 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces/__init__.py
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)    12118 2023-04-12 10:15:05.000000 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces/main.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-12 10:22:53.579937 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces.egg-info/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-12 10:22:53.000000 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces.egg-info/PKG-INFO
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-12 10:22:53.000000 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces.egg-info/SOURCES.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-12 10:22:53.000000 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces.egg-info/dependency_links.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-12 10:22:53.000000 atlasofsmoothspaces-1.0.6/atlasofsmoothspaces.egg-info/top_level.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-12 10:22:53.579937 atlasofsmoothspaces-1.0.6/setup.cfg
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-12 10:22:51.000000 atlasofsmoothspaces-1.0.6/setup.py
```

### Comparing `atlasofsmoothspaces-1.0.5/atlasofsmoothspaces/main.py` & `atlasofsmoothspaces-1.0.6/atlasofsmoothspaces/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,48 @@
 import numpy as np
 import time
 
+MIDI_MAX : int = 127
+
+INITIAL_SIGMOID_CALIBRATION = {
+                    "XMIN": 0,
+                    "XMAX": 0,
+                    "YMIN": 0,
+                    "YMAX": MIDI_MAX,
+                    "BETA": 0.02}
+
+INITIAL_SMOOTHNESS_VALUES = {
+                "raw": 0,
+                "calibration": INITIAL_SIGMOID_CALIBRATION,
+                "calibratedSignal": 0,
+                "isCalibrated" : False}
+
+def sigmoid(x:float, YMAX:float, YMIN:float, XMAX:float, XMIN:float, BETA=0.02):
+    """ Implements a simple sigmoid function
+    """
+    MU = (XMAX - XMIN) / 2
+    ALPHA = np.log((1-BETA) / BETA) / MU
+    return YMIN + (YMAX-  YMIN) / (1 + np.exp((-1)* ALPHA * (x - MU)))
+
 
 class SmoothnessBase():
 
     
     def __init__(self, 
         cacheLength: int,
         derivativeDegree: int,
         alpha: float or list[float]):
 
         self.cacheLength = cacheLength
         self.derivativeDegree = derivativeDegree
         self.smoothness = np.zeros(self.derivativeDegree + 1)
+        self.smoothnessMeasures = {
+            "overall": INITIAL_SMOOTHNESS_VALUES,
+            "relative": INITIAL_SMOOTHNESS_VALUES, 
+            "secondOrder": INITIAL_SMOOTHNESS_VALUES}
         self.derivatives = np.zeros((self.derivativeDegree + 1, self.cacheLength), float)  
         self.deltas = np.zeros(cacheLength, float)
         if isinstance(alpha, list):
             if len(alpha) != self.derivativeDegree + 1:
                 raise Exception("There need to be as many values of alpha as there are degrees of derivatives!")
             self.__alphaIsList = True
             self.alpha = np.array(alpha)
@@ -47,31 +73,66 @@
 
     def _addNewDelta(self, newDelta: float):    
         self.deltas = np.append(self.deltas[1:], newDelta)
 
     def _addNewSmoothness(self, newDerivatives: np.ndarray):
         self.smoothness = (1 - self.alpha) * self.smoothness + self.alpha * newDerivatives
 
+    def _updateSmoothnessMeasures(self):
+        ## update all the smoothness measures
+        self.smoothnessMeasures["overall"]["raw"] = np.sqrt(np.sum(self.smoothness[1:]**2))
+        self.smoothnessMeasures["relative"]["raw"] = np.abs(self.smoothness[2] - self.smoothness[1]**2)
+        self.smoothnessMeasures["secondOrder"]["raw"] = np.abs(self.smoothness[2])
+        for measure in ["overall", "relative", "secondOrder"] :
+            if (self.smoothnessMeasures[measure]["isCalibrated"]):
+                self.smoothnessMeasures[measure]["calibratedSignal"] = sigmoid(
+                    x=self.smoothnessMeasures[measure]["raw"], 
+                    **self.smoothnessMeasures[measure]["calibration"])
+        
+        
+
     def addNewValue(self, newValue: float, newDelta: float=None):
         
         newTime = time.time()*1000.0
         if newDelta is None:
             newDelta = newTime - self.lastUpdateTime
             
         self._addNewDelta(newDelta)
         newDerivatives = self._addNewDerivative(newValue, newDelta)
         self._addNewSmoothness(newDerivatives)
+        self._updateSmoothnessMeasures()
 
         self.lastUpdateTime = newTime
 
 
+    def getSmoothness(self, smoothnessMeasure="overall"):
+        return {
+            "raw": self.smoothnessMeasures[smoothnessMeasure]["raw"],
+            "calibratedSignal": self.smoothnessMeasures[smoothnessMeasure]["calibratedSignal"]
+        }
+    
+    def calibrateSignal(self, XMAX:float, XMIN:float, BETA:float=0.02, YMIN:float=0, YMAX:float=MIDI_MAX, smoothnessMeasure: str="overall"):
+        self.smoothnessMeasures[smoothnessMeasure]["calibration"] = {
+            "XMAX": XMAX, 
+            "XMIN": XMIN, 
+            "YMIN": YMIN,
+            "YMAX": YMAX,
+            "BETA": BETA}
+        self.smoothnessMeasures[smoothnessMeasure]["isCalibrated"] = True 
+
+    
+    def decalibrateSignal(self, smoothnessMeasure: str="overall"):
+        self.smoothnessMeasures[smoothnessMeasure]["isCalibrated"] = False 
+
 
-class Smoothness():
 
-    MIDI_MAX : int = 127
+
+
+
+class Smoothness():
 
     CHANNELS = {
         "CC16_1": "gyro x left",
         "CC16_2": "gyro x right",
         "CC17_1": "gyro y left",
         "CC17_2": "gyro y right",
         "CC18_1": "gyro z left",
@@ -114,26 +175,29 @@
         
         if isNotAdmissibleSmoothnessType:
             raise Smoothness.NotAdmissibleType
         
         if customMidiMax is not None:
             self.midiMax = customMidiMax
         else:
-            self.midiMax = Smoothness.MIDI_MAX
+            self.midiMax = MIDI_MAX
 
         if isinstance(smoothnessTypes, list):
             self.smoothnessTypes = smoothnessTypes
         else :
             self.smoothnessTypes = [smoothnessTypes]
         
+        self.currentDefaultSmoothnessMeasure = "overall"
+
         self.data : dict[str, SmoothnessBase] = {}
         self.cacheLengths : dict[str, int] = {}
         self.derivativeDegrees : dict[str, int] = {}
         self.alphas : dict[str, float or list[float]] = {}
 
+
         if (cacheLengths is not None) and (derivativeDegrees is not None) and (alphas is not None): 
             if isinstance(cacheLengths,int):
                 cacheLengths = [cacheLengths]*len(self.smoothnessTypes)
             if isinstance(derivativeDegrees, int):
                 derivativeDegrees = [derivativeDegrees]*len(self.smoothnessTypes)
             if isinstance(alphas, float):
                 alphas = [alphas] * len(self.smoothnessTypes)
@@ -165,31 +229,65 @@
         for smoothnessType in self.data.keys():
             newValue = self.conversion(smoothnessType, channelData)
             self.data[smoothnessType].addNewValue(newValue)
         if returnSmoothness:
             return self.getSmoothnessMeasure()
         
 
-    def getSmoothnessMeasure(self):
-        return {t:np.sum(v.smoothness**2) for t, v in self.data.items()}
+    def getSmoothnessMeasure(self, smoothnessMeasure=None):
+        smoothnessMeasure = (self.currentDefaultSmoothnessMeasure if smoothnessMeasure is None else smoothnessMeasure)
+        return  { 
+            smoothnessType: (
+                {
+                    "raw": smoothnessObject.smoothnessMeasures[smoothnessMeasure]["raw"],
+                    "calibratedSignal": smoothnessObject.smoothnessMeasures[smoothnessMeasure]["calibratedSignal"]
+                }
+                if smoothnessObject.smoothnessMeasures[smoothnessMeasure]["isCalibrated"]
+                else {"raw": smoothnessObject.smoothnessMeasures[smoothnessMeasure]["raw"]})
+            for smoothnessType, smoothnessObject in self.data.items()}
         
 
+    def calibrateSmoothness(self, smoothnessTypes: str or list[str], minsAndMaxs: list[int] or list[list[int]], smoothnessMeasure: str="overall"):
+        if isinstance(smoothnessTypes, str):
+            self.data[smoothnessTypes].calibrateSignal(XMIN=minsAndMaxs[0], XMAX=minsAndMaxs[1], smoothnessMeasure=smoothnessMeasure)
+        else:
+            if len(smoothnessTypes)!=len(minsAndMaxs):
+                raise Exception("arrays should be of equal lengths")
+            for sT, minMAx in zip(smoothnessTypes, minsAndMaxs):
+                self.data[sT].calibrateSignal(XMIN=minMAx[0], XMAX=minMAx[1], smoothnessMeasure=smoothnessMeasure)
+
+
+    def changeCurrentDefaultSmoothnessMeasure(self, newSmoothnessMeasure="overall"):
+        self.currentDefaultSmoothnessMeasure = newSmoothnessMeasure
 
 
     def conversion(self, smoothnessType: str, data: dict[int, float]):
         if (smoothnessType=="GYRO_LEFT"):
+
             theta = data["CC16_1"] * 2 * np.pi / self.midiMax
             phi = data["CC17_1"] * 2 * np.pi / self.midiMax
             psi = data["CC18_1"] * 2 * np.pi / self.midiMax
-            return np.sqrt(theta**2 + phi**2 + psi**2)
+            # y = np.sin(theta)
+            # z = np.cos(theta)
+            # x = np.cos(phi)
+            # z = np.sin(phi)
+            # x = np.sin(psi)
+            # y = np.cos(psi)
+            x = np.cos(phi) + np.sin(psi)
+            y = np.sin(theta) + np.cos(psi)
+            z = np.cos(theta) + np.sin(phi)
+            return np.sqrt(x**2 + y**2 + z**2)
         elif (smoothnessType=="GYRO_RIGHT"):
             theta = data["CC16_2"] * 2 * np.pi / self.midiMax
             phi = data["CC17_2"] * 2 * np.pi / self.midiMax
             psi = data["CC18_2"] * 2 * np.pi / self.midiMax
-            return np.sqrt(theta**2 + phi**2 + psi**2)
+            x = np.cos(phi) + np.sin(psi)
+            y = np.sin(theta) + np.cos(psi)
+            z = np.cos(theta) + np.sin(phi)
+            return np.sqrt(x**2 + y**2 + z**2)
         elif (smoothnessType=="VEL_LEFT"):
             return data["CC22_1"] / self.midiMax
         elif (smoothnessType=="VEL_RIGHT"):
             return data["CC22_2"] / self.midiMax
         elif (smoothnessType=="VEL_AVG"):
             return (data["CC22_1"] + data["CC22_2"] ) / (2 * self.midiMax)
         if (smoothnessType=="ACCEL_LEFT"):
```

### Comparing `atlasofsmoothspaces-1.0.5/setup.py` & `atlasofsmoothspaces-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.5' 
+VERSION = '1.0.6' 
 DESCRIPTION = 'Calculating Smoothness from Input Stream'
 LONG_DESCRIPTION = 'Smoothness is calculated from an input stream. The input data format is midi.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="atlasofsmoothspaces",
```

