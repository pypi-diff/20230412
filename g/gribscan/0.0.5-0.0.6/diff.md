# Comparing `tmp/gribscan-0.0.5-py3-none-any.whl.zip` & `tmp/gribscan-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 12401 bytes, number of entries: 13
--rw-r--r--  2.0 unx      123 b- defN 22-Sep-02 15:15 gribscan/__init__.py
--rw-r--r--  2.0 unx     5301 b- defN 22-Sep-02 15:15 gribscan/aeccodec.py
--rw-r--r--  2.0 unx    17074 b- defN 22-Sep-02 15:15 gribscan/gribscan.py
--rw-r--r--  2.0 unx     1383 b- defN 22-Sep-02 15:15 gribscan/gridutils.py
--rw-r--r--  2.0 unx     4154 b- defN 22-Sep-02 15:15 gribscan/magician.py
--rw-r--r--  2.0 unx      637 b- defN 22-Sep-02 15:15 gribscan/rawgribcodec.py
--rw-r--r--  2.0 unx     1532 b- defN 22-Sep-02 15:15 gribscan/tools.py
--rw-r--r--  2.0 unx     1078 b- defN 22-Sep-02 15:16 gribscan-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1653 b- defN 22-Sep-02 15:16 gribscan-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Sep-02 15:16 gribscan-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx      261 b- defN 22-Sep-02 15:16 gribscan-0.0.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 22-Sep-02 15:16 gribscan-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1027 b- defN 22-Sep-02 15:16 gribscan-0.0.5.dist-info/RECORD
-13 files, 34324 bytes uncompressed, 10697 bytes compressed:  68.8%
+Zip file size: 12385 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      123 b- defN 23-Apr-12 07:24 gribscan/__init__.py
+-rw-r--r--  2.0 unx     5301 b- defN 23-Apr-12 07:24 gribscan/aeccodec.py
+-rw-r--r--  2.0 unx    17214 b- defN 23-Apr-12 07:24 gribscan/gribscan.py
+-rw-r--r--  2.0 unx     1383 b- defN 23-Apr-12 07:24 gribscan/gridutils.py
+-rw-r--r--  2.0 unx     4154 b- defN 23-Apr-12 07:24 gribscan/magician.py
+-rw-r--r--  2.0 unx      637 b- defN 23-Apr-12 07:24 gribscan/rawgribcodec.py
+-rw-r--r--  2.0 unx     1532 b- defN 23-Apr-12 07:24 gribscan/tools.py
+-rw-r--r--  2.0 unx     1078 b- defN 23-Apr-12 07:24 gribscan-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1653 b- defN 23-Apr-12 07:24 gribscan-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 07:24 gribscan-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx      261 b- defN 23-Apr-12 07:24 gribscan-0.0.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-12 07:24 gribscan-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1027 b- defN 23-Apr-12 07:24 gribscan-0.0.6.dist-info/RECORD
+13 files, 34464 bytes uncompressed, 10681 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: gribscan/rawgribcodec.py
 Comment: 
 
 Filename: gribscan/tools.py
 Comment: 
 
-Filename: gribscan-0.0.5.dist-info/LICENSE
+Filename: gribscan-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: gribscan-0.0.5.dist-info/METADATA
+Filename: gribscan-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: gribscan-0.0.5.dist-info/WHEEL
+Filename: gribscan-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: gribscan-0.0.5.dist-info/entry_points.txt
+Filename: gribscan-0.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: gribscan-0.0.5.dist-info/top_level.txt
+Filename: gribscan-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: gribscan-0.0.5.dist-info/RECORD
+Filename: gribscan-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gribscan/__init__.py

```diff
@@ -1,5 +1,5 @@
 from gribscan.gribscan import *
 from gribscan.aeccodec import *
 from gribscan.rawgribcodec import *
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

## gribscan/gribscan.py

```diff
@@ -210,15 +210,15 @@
     13: 1,  # np.timedelta64(1, "s"),
     #14-191  Reserved
     #192-254 Reserved for local use
     #255 Missing
 }
 
 
-def get_time_offset(gribmessage):
+def get_time_offset(gribmessage, lean_towards="end"):
     offset = 0  # np.timedelta64(0, "s")
     edition = int(gribmessage["editionNumber"])
     if edition == 1:
         timeRangeIndicator = int(gribmessage["timeRangeIndicator"])
         if timeRangeIndicator == 0:
             unit = time_range_units[int(gribmessage.get("indicatorOfUnitOfTimeRange", 255))]
             offset += int(gribmessage["P1"]) * unit
@@ -233,15 +233,17 @@
         try:
             options = production_template_numbers[int(gribmessage["productDefinitionTemplateNumber"])]
         except KeyError:
             return offset
         if options["forcastTime"]:
             unit = time_range_units[int(gribmessage.get("indicatorOfUnitOfTimeRange", 255))]
             offset += gribmessage.get("forecastTime", 0) * unit
-        # TODO: handling of time ranges, see cdo: libcdi/src/gribapi_utilities.c: gribMakeTimeString
+        if options["timeRange"] and lean_towards == "end":
+            unit = time_range_units[int(gribmessage.get("indicatorOfUnitOfTimeRange", 255))]
+            offset += gribmessage.get("lengthOfTimeRange", 0) * unit
     return offset
 
 
 def arrays_to_list(o):
     try:
         return o.tolist()
     except AttributeError:
```

## Comparing `gribscan-0.0.5.dist-info/LICENSE` & `gribscan-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gribscan-0.0.5.dist-info/METADATA` & `gribscan-0.0.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gribscan
-Version: 0.0.5
+Version: 0.0.6
 Summary: create indices for GRIB files and provide an xarray interface
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cfgrib (>=0.9.9.0)
 Requires-Dist: eccodes
 Requires-Dist: numcodecs (>=0.10.0)
 Requires-Dist: numpy
```

