# Comparing `tmp/eptlsoot-0.0.4-cp39-cp39-win_amd64.whl.zip` & `tmp/eptlsoot-0.0.5-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 1613496 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat      471 b- defN 23-Apr-05 21:45 eptlsoot/__init__.py
+Zip file size: 1628730 bytes, number of entries: 20
+-rw-rw-rw-  2.0 fat      468 b- defN 23-Apr-08 22:08 eptlsoot/__init__.py
 -rw-rw-rw-  2.0 fat  1465856 b- defN 23-Apr-05 21:26 eptlsoot/_eptlsoot.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat     6093 b- defN 23-Apr-05 21:43 eptlsoot/cpfr.py
 -rw-rw-rw-  2.0 fat      679 b- defN 23-Apr-05 21:38 eptlsoot/eptlsoot.py
 -rw-rw-rw-  2.0 fat      644 b- defN 23-Apr-05 21:43 eptlsoot/psr.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-05 04:38 eptlsoot/apps/__init__.py
--rw-rw-rw-  2.0 fat      412 b- defN 23-Apr-05 21:49 eptlsoot/apps/flame.py
--rw-rw-rw-  2.0 fat     1413 b- defN 23-Apr-06 23:35 eptlsoot/apps/pahgrowth.py
+-rw-rw-rw-  2.0 fat      580 b- defN 23-Apr-08 22:09 eptlsoot/apps/flame.py
+-rw-rw-rw-  2.0 fat     1628 b- defN 23-Apr-12 01:01 eptlsoot/apps/pahgrowth.py
 -rw-rw-rw-  2.0 fat     4680 b- defN 23-Apr-06 17:33 eptlsoot/apps/reactors.py
 -rw-rw-rw-  2.0 fat      265 b- defN 23-Apr-05 04:46 eptlsoot/apps/solutionarray.py
 -rw-rw-rw-  2.0 fat     3082 b- defN 23-Apr-06 04:32 eptlsoot/apps/sootgas.py
 -rw-rw-rw-  2.0 fat      950 b- defN 23-Apr-05 21:55 eptlsoot/apps/sootmodels.py
--rw-rw-rw-  2.0 fat     5968 b- defN 23-Apr-06 02:51 eptlsoot/apps/sootwrappers.py
+-rw-rw-rw-  2.0 fat     5993 b- defN 23-Apr-08 23:53 eptlsoot/apps/sootwrappers.py
 -rw-rw-rw-  2.0 fat      239 b- defN 23-Apr-05 21:52 eptlsoot/apps/surfacereactions.py
--rw-rw-rw-  2.0 fat  1432576 b- defN 23-Apr-07 06:03 eptlsoot/lib/_eptlsoot.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  1482752 b- defN 23-Apr-12 01:11 eptlsoot/lib/_eptlsoot.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat  1468928 b- defN 23-Apr-05 21:11 eptlsoot2/_eptlsoot2.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      734 b- defN 23-Apr-07 06:03 eptlsoot-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-07 06:03 eptlsoot-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-07 06:03 eptlsoot-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1641 b- defN 23-Apr-07 06:03 eptlsoot-0.0.4.dist-info/RECORD
-20 files, 4394740 bytes uncompressed, 1610832 bytes compressed:  63.4%
+-rw-rw-rw-  2.0 fat      734 b- defN 23-Apr-12 01:11 eptlsoot-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-12 01:11 eptlsoot-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-12 01:11 eptlsoot-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1641 b- defN 23-Apr-12 01:11 eptlsoot-0.0.5.dist-info/RECORD
+20 files, 4445321 bytes uncompressed, 1626066 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: eptlsoot/lib/_eptlsoot.cp39-win_amd64.pyd
 Comment: 
 
 Filename: eptlsoot2/_eptlsoot2.cp39-win_amd64.pyd
 Comment: 
 
-Filename: eptlsoot-0.0.4.dist-info/METADATA
+Filename: eptlsoot-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: eptlsoot-0.0.4.dist-info/WHEEL
+Filename: eptlsoot-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: eptlsoot-0.0.4.dist-info/top_level.txt
+Filename: eptlsoot-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: eptlsoot-0.0.4.dist-info/RECORD
+Filename: eptlsoot-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## eptlsoot/__init__.py

```diff
@@ -1,9 +1,9 @@
 from .eptlsoot import SootModel, Reactor, ReactorSoot, FlameSolver, FlameSolverOpt
 from .cpfr import CPFR
 from .apps.sootgas import SootGas
 from .apps.sootmodels import MonodisperseSootModel
 from .apps.reactors import PlugFlowReactor, ConstantVolumeReactor, Inlet
 from .apps.pahgrowth import ReactDim, DimerCoal
-from .apps.flame import TempFlameSolver, TempFlameSolverVector
+from .apps.flame import TempFlameSolver, TempFlameSolverOpt
 from .apps.sootwrappers import SootWrapper
 from .apps.solutionarray import SolutionArray
```

## eptlsoot/apps/flame.py

```diff
@@ -1,10 +1,15 @@
-from ..lib._eptlsoot import CTempFlameSolver, CTempFlameSolverVector
+from ..lib._eptlsoot import CTempFlameSolver, CTempFlameSolverOpt
 
 class TempFlameSolver(CTempFlameSolver):
     def __init__(self, soot_gas, flame, grid, soot_model):
         super().__init__(soot_gas, flame, grid, soot_model)
 
 
-class TempFlameSolverVector(CTempFlameSolverVector):
-    def __init__(self, soot_gas, flame, grid, soot_model):
-        super().__init__(soot_gas, flame, grid, soot_model)
+# class TempFlameSolverVector(CTempFlameSolverVector):
+#     def __init__(self, soot_gas, flame, grid, soot_model):
+#         super().__init__(soot_gas, flame, grid, soot_model)
+
+
+class TempFlameSolverOpt(CTempFlameSolverOpt):
+    def __init__(self, soot_gas, flame, grid, soot):
+        super().__init__(soot_gas, flame, grid, soot)
```

## eptlsoot/apps/pahgrowth.py

```diff
@@ -1,8 +1,8 @@
-from ..lib._eptlsoot import CReactDim, CDimerCoal, CCrossLink
+from ..lib._eptlsoot import CReactDim, CDimerCoal, CDimerCoalMod, CCrossLink
 
 class PAHGrowthAbstract:
     def __init__(self, soot_wrapper):
         super().__init__(soot_wrapper);
 
 
     def set_precursor_names(self, precursor_list):
@@ -27,13 +27,19 @@
 
 
 class DimerCoal(PAHGrowthAbstract, CDimerCoal):
     serialized_name = "DimerCoalescence"
     def __init__(self, soot_wrapper):
         super().__init__(soot_wrapper);
 
+
+class DimerCoalMod(PAHGrowthAbstract, CDimerCoal):
+    serialized_name = "DimerCoalescenceModified"
+    def __init__(self, soot_wrapper):
+        super().__init__(soot_wrapper);
+
 class CrossLink(PAHGrowthAbstract, CCrossLink):
     serialized_name = "CrossLinking"
     def __init__(self, soot_wrapper):
         super().__init__(soot_wrapper);
 
-PAH_GROWTH_MODELS = [ReactDim, DimerCoal, CrossLink]
+PAH_GROWTH_MODELS = [ReactDim, DimerCoal, CrossLink, DimerCoalMod]
```

## eptlsoot/apps/sootwrappers.py

```diff
@@ -112,8 +112,8 @@
         current_surface_reactions_model = self._get_or_create_surface_reactions_model(model_type);
         self.set_surface_reactions_model(current_surface_reactions_model);
 
     def __getattr__(self, name):
         if name in self.soot_model.soot_att:
             return self.soot_model.det_soot_att(name);
         else:
-            raise ValueError("Attirbute not found")
+            raise ValueError(f"{name} is an attirbute of SootWrapper class")
```

## Comparing `eptlsoot-0.0.4.dist-info/METADATA` & `eptlsoot-0.0.5.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eptlsoot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Soot model from EPTL group
 Author-email: Mo Adib <moademic@gmail.com>
 Project-URL: Homepage, https://carleton.ca/eptl/people/336/
 Keywords: computational,soot
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

