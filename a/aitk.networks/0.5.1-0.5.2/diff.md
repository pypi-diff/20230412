# Comparing `tmp/aitk.networks-0.5.1-py3-none-any.whl.zip` & `tmp/aitk.networks-0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 30469 bytes, number of entries: 10
+Zip file size: 30473 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      411 b- defN 21-Feb-18 23:19 aitk/networks/__init__.py
--rw-rw-r--  2.0 unx      392 b- defN 21-Sep-22 04:07 aitk/networks/_version.py
+-rw-rw-r--  2.0 unx      392 b- defN 23-Apr-12 16:20 aitk/networks/_version.py
 -rw-rw-r--  2.0 unx     4294 b- defN 21-Apr-03 15:39 aitk/networks/callbacks.py
--rw-rw-r--  2.0 unx   105208 b- defN 21-Sep-19 16:26 aitk/networks/network.py
--rw-rw-r--  2.0 unx    14268 b- defN 21-Aug-22 19:42 aitk/networks/utils.py
+-rw-rw-r--  2.0 unx   105211 b- defN 23-Apr-12 16:14 aitk/networks/network.py
+-rw-rw-r--  2.0 unx    14268 b- defN 21-Sep-25 03:35 aitk/networks/utils.py
 -rw-rw-r--  2.0 unx     7235 b- defN 21-Aug-14 17:34 aitk/networks/watchers.py
--rw-rw-r--  2.0 unx     1158 b- defN 21-Sep-22 04:07 aitk.networks-0.5.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 21-Sep-22 04:07 aitk.networks-0.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 21-Sep-22 04:07 aitk.networks-0.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      811 b- defN 21-Sep-22 04:07 aitk.networks-0.5.1.dist-info/RECORD
-10 files, 133874 bytes uncompressed, 29089 bytes compressed:  78.3%
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Apr-12 16:27 aitk.networks-0.5.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 16:27 aitk.networks-0.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-12 16:27 aitk.networks-0.5.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      811 b- defN 23-Apr-12 16:27 aitk.networks-0.5.2.dist-info/RECORD
+10 files, 133877 bytes uncompressed, 29093 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: aitk/networks/utils.py
 Comment: 
 
 Filename: aitk/networks/watchers.py
 Comment: 
 
-Filename: aitk.networks-0.5.1.dist-info/METADATA
+Filename: aitk.networks-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: aitk.networks-0.5.1.dist-info/WHEEL
+Filename: aitk.networks-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: aitk.networks-0.5.1.dist-info/top_level.txt
+Filename: aitk.networks-0.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: aitk.networks-0.5.1.dist-info/RECORD
+Filename: aitk.networks-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aitk/networks/_version.py

```diff
@@ -4,9 +4,9 @@
 #
 # Copyright (c) 2021 AITK Developers
 #
 # https://github.com/ArtificialIntelligenceToolkit/aitk.networks
 #
 # **************************************************************
 
-version_info = (0, 5, 1)
+version_info = (0, 5, 2)
 __version__ = ".".join(map(str, version_info))
```

## aitk/networks/network.py

```diff
@@ -1081,25 +1081,25 @@
             if channel is None:
                 channel = self._get_feature(layer_name)
             select = tuple([slice(None) for i in range(len(vector.shape) - 1)] + [slice(channel, channel+1)])
             vector = vector[select]
         else:
             pass # let's try it as is
 
+        # If vshape is given, then resize the vector:
+        vshape = self.vshape(layer_name)
+        if vshape and vshape != vector.shape:
+            vector = vector.reshape(vshape)
+
         try:
             image = array_to_image(vector, minmax=self._layer_minmax(layer_name))
         except Exception:
             # Error: make a red image
             image = array_to_image([[[255, 0, 0]], [[255, 0, 0]]])
 
-        # If vshape is given, then resize the image:
-        vshape = self.vshape(layer_name)
-        if vshape and vshape != image.size:
-            image = image.resize(vshape, 0)
-
         return image
 
     def _make_color(self, item):
         if isinstance(item, numbers.Number):
             return (item, item, item)
         else:
             return tuple(item)
```

## Comparing `aitk.networks-0.5.1.dist-info/METADATA` & `aitk.networks-0.5.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitk.networks
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Keras model wrapper with visualizations
 Home-page: https://github.com/ArtificialIntelligenceToolkit/aitk.networks
 Author: Douglas Blank
 License: BSD-3-Clause
 Keywords: robot,simulator,jupyter,python
 Platform: Linux
 Platform: Mac OS X
```

## Comparing `aitk.networks-0.5.1.dist-info/RECORD` & `aitk.networks-0.5.2.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 aitk/networks/__init__.py,sha256=-hk9H0DAOP8Lt62hxF1wj2wZUB2zwmpEOuhfWO1zzo8,411
-aitk/networks/_version.py,sha256=dK40DuPA1CE8bXDJxLcXPP1VHywxqZQcugUugFFdnj4,392
+aitk/networks/_version.py,sha256=RhdQvBs-Z-ukZPyAfUt0JwF7XoJT7K49Dzfn_SP_t4w,392
 aitk/networks/callbacks.py,sha256=jH0yuZVWSET6tV80tY9WNng7mfN-miHGhYSDcmlCYY4,4294
-aitk/networks/network.py,sha256=UQqwSWL9TS9vRUEyk7FZ_dgheGjUmrUwdmEuwJsyi74,105208
+aitk/networks/network.py,sha256=UCUnxJ35nagbwEzVXjhUhlUjH4y8JS_A23FkO8AS0wo,105211
 aitk/networks/utils.py,sha256=9Bc00Dq4gQGHhxQpiasgpc0m8koDzpF3_879QT9ddoo,14268
 aitk/networks/watchers.py,sha256=fKa9Q2Si6dmKcaTJcFxUHcD0DuYSBF5uVWBF62CvnBs,7235
-aitk.networks-0.5.1.dist-info/METADATA,sha256=Utb0u3M3jWftARkmJbmoKMGlzoQnVZG7budbVxPI8pw,1158
-aitk.networks-0.5.1.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-aitk.networks-0.5.1.dist-info/top_level.txt,sha256=Nd1TXMWwE1VIGABpa4lX9EdmidaqlayqBFLVnVNuCvM,5
-aitk.networks-0.5.1.dist-info/RECORD,,
+aitk.networks-0.5.2.dist-info/METADATA,sha256=aCz17ZM1XijxdRLFd6u7HwWsh2-WHU16WjnnI8wjUiM,1158
+aitk.networks-0.5.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+aitk.networks-0.5.2.dist-info/top_level.txt,sha256=Nd1TXMWwE1VIGABpa4lX9EdmidaqlayqBFLVnVNuCvM,5
+aitk.networks-0.5.2.dist-info/RECORD,,
```

