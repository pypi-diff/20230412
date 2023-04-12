# Comparing `tmp/cellmap-1.0.1.dev202304120838-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304120839-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 751469 bytes, number of entries: 9
+Zip file size: 751471 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
 -rw-r--r--  2.0 unx    43472 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
 -rw-r--r--  2.0 unx   203706 b- defN 80-Jan-01 00:00 cellmap/figures/CellMap_Endocrine_1_RNA_velocity.png
 -rw-r--r--  2.0 unx   194405 b- defN 80-Jan-01 00:00 cellmap/figures/CellMap_Endocrine_2_Potential_flow.png
 -rw-r--r--  2.0 unx   192764 b- defN 80-Jan-01 00:00 cellmap/figures/CellMap_Endocrine_3_Rotational_flow.png
 -rw-r--r--  2.0 unx   152250 b- defN 80-Jan-01 00:00 cellmap/figures/CellMap_Endocrine_4_Potential.png
--rw-r--r--  2.0 unx     1742 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304120838.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304120838.dist-info/WHEEL
-?rw-r--r--  2.0 unx      850 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304120838.dist-info/RECORD
-9 files, 789329 bytes uncompressed, 749991 bytes compressed:  5.0%
+-rw-r--r--  2.0 unx     1752 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304120839.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304120839.dist-info/WHEEL
+?rw-r--r--  2.0 unx      850 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304120839.dist-info/RECORD
+9 files, 789339 bytes uncompressed, 749993 bytes compressed:  5.0%
```

## zipnote {}

```diff
@@ -12,17 +12,17 @@
 
 Filename: cellmap/figures/CellMap_Endocrine_3_Rotational_flow.png
 Comment: 
 
 Filename: cellmap/figures/CellMap_Endocrine_4_Potential.png
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304120838.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304120839.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304120838.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304120839.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304120838.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304120839.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cellmap-1.0.1.dev202304120838.dist-info/METADATA` & `cellmap-1.0.1.dev202304120839.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304120838
+Version: 1.0.1.dev202304120839
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,15 +16,15 @@
 Requires-Dist: scipy (>=1.8.1,<2.0.0)
 Project-URL: Documentation, https://github.com/yusuke-imoto-lab/CellMap/
 Project-URL: Repository, https://github.com/yusuke-imoto-lab/CellMap
 Description-Content-Type: text/markdown
 
 # CellMap - RNA landscape inference method
 
-<div style="text-align:left"><img style="width:100%; height: auto" src="https://github.com/yusuke-imoto-lab/CellMap/figures/CellMap_Overview.jpg"/></div>
+<div style="text-align:left"><img style="width:100%; height: auto" src="https://github.com/yusuke-imoto-lab/CellMap/blob/main/figures/CellMap_Overview.jpg"/></div>
 
 The CellMap is a RNA landscape inference method based on the graph Hodge decomposition. 
 
 ## Installation
 
 To install CellMap package, use `pip` as follows:
```

## Comparing `cellmap-1.0.1.dev202304120838.dist-info/RECORD` & `cellmap-1.0.1.dev202304120839.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cellmap/__init__.py,sha256=iMIk5quffcAyDvWQc2u06lLTm1_dxOkW_L6t6JbQKi0,52
 cellmap/cellmap.py,sha256=9v3vqp1CQHgAaywlRxJ2moXyA00fcSlViqsUJv2xNZY,43472
 cellmap/figures/CellMap_Endocrine_1_RNA_velocity.png,sha256=HTVrJ9-mS8N8Uhhhe34zV0ePfWqqOlzgFw65KcyBv1U,203706
 cellmap/figures/CellMap_Endocrine_2_Potential_flow.png,sha256=nnyMqovV9m4UZGa1DV1c6PooQqr6RZeVDVuKaEBS5nU,194405
 cellmap/figures/CellMap_Endocrine_3_Rotational_flow.png,sha256=_C7NQt2wFHl1d8TQPuTB2iIjwRkIx2HhXTo34pS_OxQ,192764
 cellmap/figures/CellMap_Endocrine_4_Potential.png,sha256=I5qGkVzlbySNmJKtR4-SwMB4HXhTQl1vMT84gigsJwU,152250
-cellmap-1.0.1.dev202304120838.dist-info/METADATA,sha256=c9kEPsCDY5TFOmdjGd0jfwiGjjcDxlGI4OcxA0ODUgE,1742
-cellmap-1.0.1.dev202304120838.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-cellmap-1.0.1.dev202304120838.dist-info/RECORD,,
+cellmap-1.0.1.dev202304120839.dist-info/METADATA,sha256=0kZZvEZd70ehCJaTXu-B63bd5BkdZdApWoVOMk8e8xo,1752
+cellmap-1.0.1.dev202304120839.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+cellmap-1.0.1.dev202304120839.dist-info/RECORD,,
```

