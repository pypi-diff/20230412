# Comparing `tmp/hydro_erosion-0.1.3.tar.gz` & `tmp/hydro_erosion-0.1.4.tar.gz`

## Comparing `hydro_erosion-0.1.3.tar` & `hydro_erosion-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/requirements.txt
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/viewLandscape.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/hydro_erosion/__init__.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/hydro_erosion/__main__.py
--rwxr-xr-x   0        0        0     2277 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/hydro_erosion/erodeLandscape.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/hydro_erosion/generateLandscape.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/hydro_erosion/utilities.py
--rw-r--r--   0        0        0  1339919 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/images/after.png
--rw-r--r--   0        0        0   646229 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/images/after2.png
--rw-r--r--   0        0        0  1209067 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/images/before.png
--rw-r--r--   0        0        0   471648 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/images/before2.png
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/LICENSE
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/README.md
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 hydro_erosion-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/requirements.txt
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/viewLandscape.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/hydro_erosion/__init__.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/hydro_erosion/__main__.py
+-rwxr-xr-x   0        0        0     2279 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/hydro_erosion/erodeLandscape.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/hydro_erosion/generateLandscape.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/hydro_erosion/utilities.py
+-rw-r--r--   0        0        0  1339919 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/images/after.png
+-rw-r--r--   0        0        0   646229 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/images/after2.png
+-rw-r--r--   0        0        0  1209067 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/images/before.png
+-rw-r--r--   0        0        0   471648 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/images/before2.png
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/LICENSE
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/README.md
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/PKG-INFO
```

### Comparing `hydro_erosion-0.1.3/viewLandscape.py` & `hydro_erosion-0.1.4/viewLandscape.py`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.3/hydro_erosion/__main__.py` & `hydro_erosion-0.1.4/hydro_erosion/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import sys
-from utilities import readCSV, writeCSV
-from erodeLandscape import erodeMap
+from . utilities import readCSV, writeCSV
+from . erodeLandscape import erodeMap
 
 def main():
     args = sys.argv[1:]
     if len(args) != 4:
         print("Arguments: [source.csv] [rock.csv] [destination.csv] <#kiterations>")
         quit()
     source = args[0]
```

### Comparing `hydro_erosion-0.1.3/hydro_erosion/erodeLandscape.py` & `hydro_erosion-0.1.4/hydro_erosion/erodeLandscape.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /home/miko/python/HydroErosion/env/bin/python3
 
 import random
-from utilities import mean
+from . utilities import mean
 
 #  from viewLandscape import viewMap
 
 def getDeltaHeight(map, x, y):
     deltaHeight = []
     for i in [-1, 0, 1]:
         deltaHeight.append([])
```

### Comparing `hydro_erosion-0.1.3/hydro_erosion/generateLandscape.py` & `hydro_erosion-0.1.4/hydro_erosion/generateLandscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import noise
-from utilities import writeCSV, normalizeNoiseMap
+from . utilities import writeCSV, normalizeNoiseMap
 
 def generateNoiseMap(length, width, scale=190, roughness=5, shift=2.0):
     octaves = roughness
     persistence = .5
     lacunarity = shift
     map = [[noise.pnoise2(i/scale, j/scale,
         octaves=octaves,
```

### Comparing `hydro_erosion-0.1.3/hydro_erosion/utilities.py` & `hydro_erosion-0.1.4/hydro_erosion/utilities.py`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.3/images/after.png` & `hydro_erosion-0.1.4/images/after.png`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.3/images/after2.png` & `hydro_erosion-0.1.4/images/after2.png`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.3/images/before.png` & `hydro_erosion-0.1.4/images/before.png`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.3/images/before2.png` & `hydro_erosion-0.1.4/images/before2.png`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.3/LICENSE` & `hydro_erosion-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.3/README.md` & `hydro_erosion-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.3/pyproject.toml` & `hydro_erosion-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hydro_erosion"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Mikolaj Figurski", email="miko.f80@gmail.com" },
 ]
 description = "Model of rain eroding a landscape"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `hydro_erosion-0.1.3/PKG-INFO` & `hydro_erosion-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydro_erosion
-Version: 0.1.3
+Version: 0.1.4
 Summary: Model of rain eroding a landscape
 Project-URL: Homepage, https://github.com/mfigurski80/HydroErosion/tree/master
 Project-URL: Bug Tracker, https://github.com/mfigurski80/HydroErosion/issues
 Author-email: Mikolaj Figurski <miko.f80@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

