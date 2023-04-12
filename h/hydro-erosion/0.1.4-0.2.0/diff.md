# Comparing `tmp/hydro_erosion-0.1.4.tar.gz` & `tmp/hydro_erosion-0.2.0.tar.gz`

## Comparing `hydro_erosion-0.1.4.tar` & `hydro_erosion-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/requirements.txt
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/viewLandscape.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/hydro_erosion/__init__.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/hydro_erosion/__main__.py
--rwxr-xr-x   0        0        0     2279 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/hydro_erosion/erodeLandscape.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/hydro_erosion/generateLandscape.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/hydro_erosion/utilities.py
--rw-r--r--   0        0        0  1339919 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/images/after.png
--rw-r--r--   0        0        0   646229 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/images/after2.png
--rw-r--r--   0        0        0  1209067 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/images/before.png
--rw-r--r--   0        0        0   471648 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/images/before2.png
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/LICENSE
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/README.md
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 hydro_erosion-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/makefile
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/viewLandscape.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/hydro_erosion/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/hydro_erosion/__main__.py
+-rwxr-xr-x   0        0        0     2238 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/hydro_erosion/erodeLandscape.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/hydro_erosion/generateLandscape.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/hydro_erosion/utilities.py
+-rw-r--r--   0        0        0  1339919 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/images/after.png
+-rw-r--r--   0        0        0   646229 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/images/after2.png
+-rw-r--r--   0        0        0  1209067 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/images/before.png
+-rw-r--r--   0        0        0   471648 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/images/before2.png
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/LICENSE
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/README.md
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 hydro_erosion-0.2.0/PKG-INFO
```

### Comparing `hydro_erosion-0.1.4/viewLandscape.py` & `hydro_erosion-0.2.0/viewLandscape.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import plotly.graph_objects as go # https://plot.ly/python/3d-surface-plots/
-from utilities import readCSV, normalizeNoiseMap, dim
+from hydro_erosion.utilities import readCSV, normalizeNoiseMap, dim
 from mayavi import mlab
 
 # Render map
 def viewMap(map):
     viewMapMayavi(map)
 
 def viewMapPlotly(map):
```

### Comparing `hydro_erosion-0.1.4/hydro_erosion/__main__.py` & `hydro_erosion-0.2.0/hydro_erosion/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import sys
 from . utilities import readCSV, writeCSV
 from . erodeLandscape import erodeMap
 
 def main():
     args = sys.argv[1:]
     if len(args) != 4:
-        print("Arguments: [source.csv] [rock.csv] [destination.csv] <#kiterations>")
+        print("Arguments: [source.csv] [rock.csv] [destination.csv] <#iterations>")
         quit()
     source = args[0]
     rock_source = args[1]
     destination = args[2]
-    k_iterations = int(args[3])
-    print(f"Running: ({source}, {rock_source}) #{k_iterations}k => {destination}")
+    iterations = int(args[3])
+    print(f"Running: ({source}, {rock_source}) #{iterations} => {destination}")
     base_map = readCSV(source)
     rock = readCSV(rock_source)
-    height, hydration = erodeMap(base_map, rock, 1000 * k_iterations)
+    height, hydration = erodeMap(base_map, rock, iterations)
     writeCSV(height, destination)
     writeCSV(hydration, "hydrationmap.csv")
     #  viewMap(height)
 
 if __name__ == "__main__":
     main()
```

### Comparing `hydro_erosion-0.1.4/hydro_erosion/generateLandscape.py` & `hydro_erosion-0.2.0/hydro_erosion/generateLandscape.py`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.4/hydro_erosion/utilities.py` & `hydro_erosion-0.2.0/hydro_erosion/utilities.py`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.4/images/after.png` & `hydro_erosion-0.2.0/images/after.png`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.4/images/after2.png` & `hydro_erosion-0.2.0/images/after2.png`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.4/images/before.png` & `hydro_erosion-0.2.0/images/before.png`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.4/images/before2.png` & `hydro_erosion-0.2.0/images/before2.png`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.4/LICENSE` & `hydro_erosion-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.4/README.md` & `hydro_erosion-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hydro_erosion-0.1.4/pyproject.toml` & `hydro_erosion-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hydro_erosion"
-version = "0.1.4"
+version = "0.2.0"
 authors = [
   { name="Mikolaj Figurski", email="miko.f80@gmail.com" },
 ]
 description = "Model of rain eroding a landscape"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `hydro_erosion-0.1.4/PKG-INFO` & `hydro_erosion-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydro_erosion
-Version: 0.1.4
+Version: 0.2.0
 Summary: Model of rain eroding a landscape
 Project-URL: Homepage, https://github.com/mfigurski80/HydroErosion/tree/master
 Project-URL: Bug Tracker, https://github.com/mfigurski80/HydroErosion/issues
 Author-email: Mikolaj Figurski <miko.f80@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

