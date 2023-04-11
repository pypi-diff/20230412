# Comparing `tmp/DataVisual-0.3.8-py3-none-any.whl.zip` & `tmp/DataVisual-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,15 @@
-Zip file size: 6556 bytes, number of entries: 11
--rw-r--r--  2.0 unx       78 b- defN 23-Mar-25 22:16 DataVisual/__init__.py
--rw-r--r--  2.0 unx     6788 b- defN 23-Mar-25 22:16 DataVisual/multi_array.py
--rw-r--r--  2.0 unx     3416 b- defN 23-Mar-25 22:16 DataVisual/tables.py
--rw-r--r--  2.0 unx      148 b- defN 23-Mar-25 22:16 DataVisual/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-25 22:16 DataVisual/tools/__init__.py
--rw-r--r--  2.0 unx      572 b- defN 23-Mar-25 22:16 DataVisual/tools/directories.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Mar-25 22:16 DataVisual-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2262 b- defN 23-Mar-25 22:16 DataVisual-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-25 22:16 DataVisual-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Mar-25 22:16 DataVisual-0.3.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      881 b- defN 23-Mar-25 22:16 DataVisual-0.3.8.dist-info/RECORD
-11 files, 15321 bytes uncompressed, 5060 bytes compressed:  67.0%
+Zip file size: 6922 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        6 b- defN 23-Mar-27 17:58 DataVisual/VERSION
+-rw-r--r--  2.0 unx       78 b- defN 23-Mar-27 17:58 DataVisual/__init__.py
+-rw-r--r--  2.0 unx     6788 b- defN 23-Mar-27 17:58 DataVisual/multi_array.py
+-rw-r--r--  2.0 unx     3416 b- defN 23-Mar-27 17:58 DataVisual/tables.py
+-rw-r--r--  2.0 unx      148 b- defN 23-Mar-27 17:58 DataVisual/utils.py
+-rw-r--r--  2.0 unx       19 b- defN 23-Mar-27 17:58 DataVisual/examples/README.rst
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-27 17:58 DataVisual/tools/__init__.py
+-rw-r--r--  2.0 unx      572 b- defN 23-Mar-27 17:58 DataVisual/tools/directories.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Mar-27 17:58 DataVisual-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2262 b- defN 23-Mar-27 17:58 DataVisual-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-27 17:58 DataVisual-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Mar-27 17:58 DataVisual-0.3.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1038 b- defN 23-Mar-27 17:58 DataVisual-0.3.9.dist-info/RECORD
+13 files, 15503 bytes uncompressed, 5178 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,34 +1,40 @@
+Filename: DataVisual/VERSION
+Comment: 
+
 Filename: DataVisual/__init__.py
 Comment: 
 
 Filename: DataVisual/multi_array.py
 Comment: 
 
 Filename: DataVisual/tables.py
 Comment: 
 
 Filename: DataVisual/utils.py
 Comment: 
 
+Filename: DataVisual/examples/README.rst
+Comment: 
+
 Filename: DataVisual/tools/__init__.py
 Comment: 
 
 Filename: DataVisual/tools/directories.py
 Comment: 
 
-Filename: DataVisual-0.3.8.dist-info/LICENSE
+Filename: DataVisual-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: DataVisual-0.3.8.dist-info/METADATA
+Filename: DataVisual-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: DataVisual-0.3.8.dist-info/WHEEL
+Filename: DataVisual-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: DataVisual-0.3.8.dist-info/top_level.txt
+Filename: DataVisual-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: DataVisual-0.3.8.dist-info/RECORD
+Filename: DataVisual-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## DataVisual/multi_array.py

```diff
@@ -142,16 +142,16 @@
             label_in_box = ""
 
             for _, _, common, _ in iteration:
                 label_in_box += common
 
         return Plots.Text(
             text=label_in_box,
-            position=[0.95, 0.95],
-            font_size=11
+            position=[0.00, 1.00],
+            font_size=12
         )
 
     def _plot_normal_(self, x: Table.Xparameter, y: Table.Xparameter) -> list:
         """
         Method plot the multi-dimensional array with the x key as abscissa.
         args and kwargs can be passed as standard input to matplotlib.pyplot.
```

## Comparing `DataVisual-0.3.8.dist-info/LICENSE` & `DataVisual-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `DataVisual-0.3.8.dist-info/METADATA` & `DataVisual-0.3.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataVisual
-Version: 0.3.8
+Version: 0.3.9
 Summary: A package multidimensional data visualisation.
 Home-page: https://github.com/MartinPdeS/DataVisual
 Author: Martin Poinsinet de Sivry
 Author-email: Martin.poinsinet.de.sivry@gmail.com
 License: MIT
 Platform: unix
 Platform: linux
```

## Comparing `DataVisual-0.3.8.dist-info/RECORD` & `DataVisual-0.3.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+DataVisual/VERSION,sha256=b-bwxo2ag-u9tSnBeCZkxJNPufWmMhWrWtKSUNcv5e0,6
 DataVisual/__init__.py,sha256=0Twe5r7ivbhGBsyCv6kRtemlX7zp8Boqb_ZlEb_8NUE,78
-DataVisual/multi_array.py,sha256=6xb8rIbpWsjxw9aXSt5kAtP9ONbq-ylzRAjEbnaCEL0,6788
+DataVisual/multi_array.py,sha256=kZ3axFni_AJiNYcWwdVlnnWOuh1DB9IiE1ci-8OWZhM,6788
 DataVisual/tables.py,sha256=n_fXRnKz3hnA2RSZR8MibRmz2eIMtfcu1ymbJlb5PHo,3416
 DataVisual/utils.py,sha256=0A5LvRlAmCO5YIpY8INF8QhcIALH0yfxkwGEczW9YHc,148
+DataVisual/examples/README.rst,sha256=WB-wJy7MMO9ETk_nxJ-HmaekQlYJeQFWeZWpFBLIBa4,19
 DataVisual/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 DataVisual/tools/directories.py,sha256=9Cr4SRLV7-S7COFe0MaC8LDala5nNzTGHOjy8gxWVyc,572
-DataVisual-0.3.8.dist-info/LICENSE,sha256=Ke_IyELN_sdt23XyXJ-cK1XuiqyNPaIKjHVkFCcy0uI,1073
-DataVisual-0.3.8.dist-info/METADATA,sha256=Av233U3Ug5AqmkApGsb6dkcjU3iN5RfJXoywyxymb5s,2262
-DataVisual-0.3.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-DataVisual-0.3.8.dist-info/top_level.txt,sha256=noiHFlgpZk0PsyudveLPxwIAClGrpUFDpHoc_HiVXoI,11
-DataVisual-0.3.8.dist-info/RECORD,,
+DataVisual-0.3.9.dist-info/LICENSE,sha256=Ke_IyELN_sdt23XyXJ-cK1XuiqyNPaIKjHVkFCcy0uI,1073
+DataVisual-0.3.9.dist-info/METADATA,sha256=--vKnuKJf-kWQQcwEAsPb8w2GISWJKuGHVJ-2Taw41w,2262
+DataVisual-0.3.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+DataVisual-0.3.9.dist-info/top_level.txt,sha256=noiHFlgpZk0PsyudveLPxwIAClGrpUFDpHoc_HiVXoI,11
+DataVisual-0.3.9.dist-info/RECORD,,
```

