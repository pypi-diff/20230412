# Comparing `tmp/ioddcomcheckergui-1.6.5.post2-py3-none-any.whl.zip` & `tmp/ioddcomcheckergui-1.6.5.post3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5858 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     5662 b- defN 23-Apr-12 12:36 siogeen/tools/gui/IoddComChecker.py
--rw-rw-r--  2.0 unx      468 b- defN 23-Apr-12 12:36 siogeen/tools/gui/__init__.py
--rw-rw-r--  2.0 unx      732 b- defN 23-Apr-12 12:36 IoddComCheckerGui-1.6.5.post2.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     5191 b- defN 23-Apr-12 12:36 IoddComCheckerGui-1.6.5.post2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 12:36 IoddComCheckerGui-1.6.5.post2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-12 12:36 IoddComCheckerGui-1.6.5.post2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      645 b- defN 23-Apr-12 12:36 IoddComCheckerGui-1.6.5.post2.dist-info/RECORD
-7 files, 12798 bytes uncompressed, 4690 bytes compressed:  63.4%
+Zip file size: 5855 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     5663 b- defN 23-Apr-12 13:02 siogeen/tools/gui/IoddComChecker.py
+-rw-rw-r--  2.0 unx      468 b- defN 23-Apr-12 13:02 siogeen/tools/gui/__init__.py
+-rw-rw-r--  2.0 unx      732 b- defN 23-Apr-12 13:02 IoddComCheckerGui-1.6.5.post3.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     5191 b- defN 23-Apr-12 13:02 IoddComCheckerGui-1.6.5.post3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 13:02 IoddComCheckerGui-1.6.5.post3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-12 13:02 IoddComCheckerGui-1.6.5.post3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      645 b- defN 23-Apr-12 13:02 IoddComCheckerGui-1.6.5.post3.dist-info/RECORD
+7 files, 12799 bytes uncompressed, 4687 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: siogeen/tools/gui/IoddComChecker.py
 Comment: 
 
 Filename: siogeen/tools/gui/__init__.py
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post2.dist-info/LICENSE.txt
+Filename: IoddComCheckerGui-1.6.5.post3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post2.dist-info/METADATA
+Filename: IoddComCheckerGui-1.6.5.post3.dist-info/METADATA
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post2.dist-info/WHEEL
+Filename: IoddComCheckerGui-1.6.5.post3.dist-info/WHEEL
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post2.dist-info/top_level.txt
+Filename: IoddComCheckerGui-1.6.5.post3.dist-info/top_level.txt
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post2.dist-info/RECORD
+Filename: IoddComCheckerGui-1.6.5.post3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## siogeen/tools/gui/IoddComChecker.py

```diff
@@ -26,22 +26,22 @@
 from kivymd.uix.floatlayout import MDFloatLayout as FloatLayout
 from kivymd.uix.stacklayout import MDStackLayout as StackLayout
 from kivy.core.clipboard import Clipboard
 from kivy.clock import Clock
 
 from siogeen.tools import IoddComChecker
 
-__version__ = "1.6.5.post2"
+__version__ = "1.6.5.post3"
 
 class IoddComCheckerGui(App):
     def build(self):
         if __version__ == IoddComChecker.__version__:
             self.title = 'IoddComChecker ' + IoddComChecker.__version__
         else:
-            self.title = f'IoddComChecker {IoddComChecker.__version__} (Gui {__version__})'
+            self.title = f'IoddComChecker {IoddComChecker.__version__}  (Gui {__version__})'
 
         self.theme_cls.primary_palette = "Blue" # "Green"
         self.theme_cls.theme_style = "Dark"
 
         self.screenBox = FloatLayout()
         #self.mainBox = BoxLayout(orientation='horizontal', spacing=10)
         self.menuBox = BoxLayout(orientation='horizontal', spacing=20, size_hint=(0.88,None))
```

## Comparing `IoddComCheckerGui-1.6.5.post2.dist-info/LICENSE.txt` & `IoddComCheckerGui-1.6.5.post3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `IoddComCheckerGui-1.6.5.post2.dist-info/METADATA` & `IoddComCheckerGui-1.6.5.post3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IoddComCheckerGui
-Version: 1.6.5.post2
+Version: 1.6.5.post3
 Summary: IoddCom IO-Link master checker Gui
 Home-page: https://siogeen.com
 Author: Reimund Renner
 Author-email: reimund@siogeen.com
 License: proprietary and confidential
 Project-URL: Documentation, https://siogeen.com/doc/
 Project-URL: Help Desk, https://siogeen.com/helpdesk/
```

