# Comparing `tmp/vmapper-0.1.0.dev202302040607-py3-none-any.whl.zip` & `tmp/vmapper-0.1.0.dev202304120903-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9871 bytes, number of entries: 7
+Zip file size: 9932 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 vmapper/__init__.py
 -rw-r--r--  2.0 unx     7759 b- defN 80-Jan-01 00:00 vmapper/color.py
 -rw-r--r--  2.0 unx     3395 b- defN 80-Jan-01 00:00 vmapper/meta_func.py
 -rw-r--r--  2.0 unx    29669 b- defN 80-Jan-01 00:00 vmapper/vmapper.py
--rw-r--r--  2.0 unx     1655 b- defN 80-Jan-01 00:00 vmapper-0.1.0.dev202302040607.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 vmapper-0.1.0.dev202302040607.dist-info/WHEEL
-?rw-r--r--  2.0 unx      554 b- defN 16-Jan-01 00:00 vmapper-0.1.0.dev202302040607.dist-info/RECORD
-7 files, 43172 bytes uncompressed, 8893 bytes compressed:  79.4%
+-rw-r--r--  2.0 unx     1809 b- defN 80-Jan-01 00:00 vmapper-0.1.0.dev202304120903.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 vmapper-0.1.0.dev202304120903.dist-info/WHEEL
+?rw-r--r--  2.0 unx      554 b- defN 16-Jan-01 00:00 vmapper-0.1.0.dev202304120903.dist-info/RECORD
+7 files, 43326 bytes uncompressed, 8954 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -6,17 +6,17 @@
 
 Filename: vmapper/meta_func.py
 Comment: 
 
 Filename: vmapper/vmapper.py
 Comment: 
 
-Filename: vmapper-0.1.0.dev202302040607.dist-info/METADATA
+Filename: vmapper-0.1.0.dev202304120903.dist-info/METADATA
 Comment: 
 
-Filename: vmapper-0.1.0.dev202302040607.dist-info/WHEEL
+Filename: vmapper-0.1.0.dev202304120903.dist-info/WHEEL
 Comment: 
 
-Filename: vmapper-0.1.0.dev202302040607.dist-info/RECORD
+Filename: vmapper-0.1.0.dev202304120903.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `vmapper-0.1.0.dev202302040607.dist-info/METADATA` & `vmapper-0.1.0.dev202304120903.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmapper
-Version: 0.1.0.dev202302040607
+Version: 0.1.0.dev202304120903
 Summary: V-Mapper
 Home-page: https://github.com/yusuke-imoto-lab/V-Mapper
 Author: Yusuke Imoto
 Requires-Python: >=3.7,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -16,19 +16,22 @@
 Requires-Dist: scikit-learn (>=0.24)
 Project-URL: Documentation, https://yusuke-imoto-lab.github.io/V-Mapper/
 Project-URL: Repository, https://github.com/yusuke-imoto-lab/V-Mapper
 Description-Content-Type: text/markdown
 
 # V-Mapper - Velocity Mapper
 
-A topological data analysis (TDA) method for high-dimensional data, Mapper, represents a topology of data as a simplicial complex or graph abstraction based on the nerve of clusters \[[Singh et al., 2007](https://doi.org/10.2312/SPBG/SPBG07/091-100)\]. V-Mapper (velocity Mapper) is an extension of Mapper for high-dimensional data with position and velocity. 
-V-Mapper describes a topological structure and flows on it simultaneously as a weighted directed graph (V-Mapper graph) by embedding given velocity data in the edges of the Mapper graph.
-
 <div style="text-align:left"><img style="width:60%; height: auto" src="https://github.com/yusuke-imoto-lab/V-Mapper/blob/main/images/VMapper_Top.jpg"/></div>
 
+V-Mapper (velocity Mapper) is an extension of Mapper, which is a well-known topological data analysis (TDA)  method for extracting high-dimensional topological structures as a graph \[[Singh et al., 2007](https://doi.org/10.2312/SPBG/SPBG07/091-100)\].
+V-Mapper is for high-dimensional data with position and velocity and describes a topological structure and flows on it simultaneously as a weighted directed graph (V-Mapper graph) by embedding given velocity data in the edges of the Mapper graph.
+
+[Y. Imoto and Y. Hiraoka. V-Mapper: topological data analysis for high-dimensional data with velocity, 2023, Nonlinear Theory and Its Applications, IEICE](https://dx.doi.org/10.26508/lsa.202201591). 
+
+
 ## Installation
 To install V-Mapper package, use `pip` as follows:
 
 ```
 $ pip install vmapper
 ```
```

## Comparing `vmapper-0.1.0.dev202302040607.dist-info/RECORD` & `vmapper-0.1.0.dev202304120903.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 vmapper/__init__.py,sha256=gIeqLbDqESlhi9URKoKaz2cbZY_C8SuqyLX99BcqrxE,52
 vmapper/color.py,sha256=JL_d4Z_OU6s92DybdF71hsK7dxn2srmA6uaHja36C8g,7759
 vmapper/meta_func.py,sha256=pvKpf6YltTaLkNQEYP1vPTImfKsIiQwTzrg3CuxOZDY,3395
 vmapper/vmapper.py,sha256=6jW4vi8nolFl7LWHcQLMkapvth7cD36YiR6h3eFNeic,29669
-vmapper-0.1.0.dev202302040607.dist-info/METADATA,sha256=ItHwnCiaqGr5eT4SV0h4zDdwL9qW6xk1aLD7zco7iEo,1655
-vmapper-0.1.0.dev202302040607.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-vmapper-0.1.0.dev202302040607.dist-info/RECORD,,
+vmapper-0.1.0.dev202304120903.dist-info/METADATA,sha256=J2_4NI6iH-o7YSpdU8DAKLUp5Sr_RkaG-ThDxfDMeq4,1809
+vmapper-0.1.0.dev202304120903.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+vmapper-0.1.0.dev202304120903.dist-info/RECORD,,
```

