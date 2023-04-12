# Comparing `tmp/ioddcomcheckergui-1.6.5.post1-py3-none-any.whl.zip` & `tmp/ioddcomcheckergui-1.6.5.post2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5811 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     5468 b- defN 23-Apr-12 12:24 siogeen/tools/gui/IoddComChecker.py
--rw-rw-r--  2.0 unx      468 b- defN 23-Apr-12 12:24 siogeen/tools/gui/__init__.py
--rw-rw-r--  2.0 unx      732 b- defN 23-Apr-12 12:25 IoddComCheckerGui-1.6.5.post1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     5191 b- defN 23-Apr-12 12:25 IoddComCheckerGui-1.6.5.post1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 12:25 IoddComCheckerGui-1.6.5.post1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-12 12:25 IoddComCheckerGui-1.6.5.post1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      645 b- defN 23-Apr-12 12:25 IoddComCheckerGui-1.6.5.post1.dist-info/RECORD
-7 files, 12604 bytes uncompressed, 4643 bytes compressed:  63.2%
+Zip file size: 5858 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     5662 b- defN 23-Apr-12 12:36 siogeen/tools/gui/IoddComChecker.py
+-rw-rw-r--  2.0 unx      468 b- defN 23-Apr-12 12:36 siogeen/tools/gui/__init__.py
+-rw-rw-r--  2.0 unx      732 b- defN 23-Apr-12 12:36 IoddComCheckerGui-1.6.5.post2.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     5191 b- defN 23-Apr-12 12:36 IoddComCheckerGui-1.6.5.post2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 12:36 IoddComCheckerGui-1.6.5.post2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-12 12:36 IoddComCheckerGui-1.6.5.post2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      645 b- defN 23-Apr-12 12:36 IoddComCheckerGui-1.6.5.post2.dist-info/RECORD
+7 files, 12798 bytes uncompressed, 4690 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: siogeen/tools/gui/IoddComChecker.py
 Comment: 
 
 Filename: siogeen/tools/gui/__init__.py
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post1.dist-info/LICENSE.txt
+Filename: IoddComCheckerGui-1.6.5.post2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post1.dist-info/METADATA
+Filename: IoddComCheckerGui-1.6.5.post2.dist-info/METADATA
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post1.dist-info/WHEEL
+Filename: IoddComCheckerGui-1.6.5.post2.dist-info/WHEEL
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post1.dist-info/top_level.txt
+Filename: IoddComCheckerGui-1.6.5.post2.dist-info/top_level.txt
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post1.dist-info/RECORD
+Filename: IoddComCheckerGui-1.6.5.post2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## siogeen/tools/gui/IoddComChecker.py

```diff
@@ -26,17 +26,23 @@
 from kivymd.uix.floatlayout import MDFloatLayout as FloatLayout
 from kivymd.uix.stacklayout import MDStackLayout as StackLayout
 from kivy.core.clipboard import Clipboard
 from kivy.clock import Clock
 
 from siogeen.tools import IoddComChecker
 
+__version__ = "1.6.5.post2"
+
 class IoddComCheckerGui(App):
     def build(self):
-        self.title = 'IoddComChecker ' + IoddComChecker.__version__
+        if __version__ == IoddComChecker.__version__:
+            self.title = 'IoddComChecker ' + IoddComChecker.__version__
+        else:
+            self.title = f'IoddComChecker {IoddComChecker.__version__} (Gui {__version__})'
+
         self.theme_cls.primary_palette = "Blue" # "Green"
         self.theme_cls.theme_style = "Dark"
 
         self.screenBox = FloatLayout()
         #self.mainBox = BoxLayout(orientation='horizontal', spacing=10)
         self.menuBox = BoxLayout(orientation='horizontal', spacing=20, size_hint=(0.88,None))
         self.autoBox = BoxLayout(orientation='horizontal', spacing=10)
```

## Comparing `IoddComCheckerGui-1.6.5.post1.dist-info/LICENSE.txt` & `IoddComCheckerGui-1.6.5.post2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `IoddComCheckerGui-1.6.5.post1.dist-info/METADATA` & `IoddComCheckerGui-1.6.5.post2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IoddComCheckerGui
-Version: 1.6.5.post1
+Version: 1.6.5.post2
 Summary: IoddCom IO-Link master checker Gui
 Home-page: https://siogeen.com
 Author: Reimund Renner
 Author-email: reimund@siogeen.com
 License: proprietary and confidential
 Project-URL: Documentation, https://siogeen.com/doc/
 Project-URL: Help Desk, https://siogeen.com/helpdesk/
```

## Comparing `IoddComCheckerGui-1.6.5.post1.dist-info/RECORD` & `IoddComCheckerGui-1.6.5.post2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-siogeen/tools/gui/IoddComChecker.py,sha256=wdYJ7o-_vs19S9sNPayJCeRTVESeS_vZr_YrMYlIv98,5468
+siogeen/tools/gui/IoddComChecker.py,sha256=iPBgNFXUltTBnaWiH6yFcngxMSWQ9htXP7JukoYQ5q4,5662
 siogeen/tools/gui/__init__.py,sha256=tWuQ0A2KTtCRBvTa4L0QAFljq4fz_vGLndYYDYpSLK4,468
-IoddComCheckerGui-1.6.5.post1.dist-info/LICENSE.txt,sha256=mjUk_O3YPxAZeoS61zCys2pyShGDxR4ghwb55ItZ0lg,732
-IoddComCheckerGui-1.6.5.post1.dist-info/METADATA,sha256=EuzEoUgH2d_x5t6MHCq0y_bjBbBuzfO-wPfiIQnZKcs,5191
-IoddComCheckerGui-1.6.5.post1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-IoddComCheckerGui-1.6.5.post1.dist-info/top_level.txt,sha256=vIFg0bLkihbkHyuCZUdHmA-50LP8LvTwDknGWir0T5o,8
-IoddComCheckerGui-1.6.5.post1.dist-info/RECORD,,
+IoddComCheckerGui-1.6.5.post2.dist-info/LICENSE.txt,sha256=mjUk_O3YPxAZeoS61zCys2pyShGDxR4ghwb55ItZ0lg,732
+IoddComCheckerGui-1.6.5.post2.dist-info/METADATA,sha256=WCO8Rg2T_KWwZx7DRX4RL5S4MbGSMDfpHHHESAvBppU,5191
+IoddComCheckerGui-1.6.5.post2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+IoddComCheckerGui-1.6.5.post2.dist-info/top_level.txt,sha256=vIFg0bLkihbkHyuCZUdHmA-50LP8LvTwDknGWir0T5o,8
+IoddComCheckerGui-1.6.5.post2.dist-info/RECORD,,
```

