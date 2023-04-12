# Comparing `tmp/ioddcomcheckergui-1.6.4-py3-none-any.whl.zip` & `tmp/ioddcomcheckergui-1.6.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5666 bytes, number of entries: 7
--rw-r--r--  2.0 unx     5180 b- defN 23-Mar-17 21:37 siogeen/tools/gui/IoddComChecker.py
--rw-r--r--  2.0 unx      468 b- defN 23-Mar-17 21:37 siogeen/tools/gui/__init__.py
--rw-rw-r--  2.0 unx      732 b- defN 23-Mar-17 21:45 IoddComCheckerGui-1.6.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     5185 b- defN 23-Mar-17 21:45 IoddComCheckerGui-1.6.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-17 21:45 IoddComCheckerGui-1.6.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Mar-17 21:45 IoddComCheckerGui-1.6.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      615 b- defN 23-Mar-17 21:45 IoddComCheckerGui-1.6.4.dist-info/RECORD
-7 files, 12280 bytes uncompressed, 4558 bytes compressed:  62.9%
+Zip file size: 5757 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     5517 b- defN 23-Apr-12 11:07 siogeen/tools/gui/IoddComChecker.py
+-rw-rw-r--  2.0 unx      468 b- defN 23-Apr-12 11:07 siogeen/tools/gui/__init__.py
+-rw-rw-r--  2.0 unx      732 b- defN 23-Apr-12 11:07 IoddComCheckerGui-1.6.5.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     5185 b- defN 23-Apr-12 11:07 IoddComCheckerGui-1.6.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 11:07 IoddComCheckerGui-1.6.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-12 11:07 IoddComCheckerGui-1.6.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      615 b- defN 23-Apr-12 11:07 IoddComCheckerGui-1.6.5.dist-info/RECORD
+7 files, 12617 bytes uncompressed, 4649 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: siogeen/tools/gui/IoddComChecker.py
 Comment: 
 
 Filename: siogeen/tools/gui/__init__.py
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.4.dist-info/LICENSE.txt
+Filename: IoddComCheckerGui-1.6.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.4.dist-info/METADATA
+Filename: IoddComCheckerGui-1.6.5.dist-info/METADATA
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.4.dist-info/WHEEL
+Filename: IoddComCheckerGui-1.6.5.dist-info/WHEEL
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.4.dist-info/top_level.txt
+Filename: IoddComCheckerGui-1.6.5.dist-info/top_level.txt
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.4.dist-info/RECORD
+Filename: IoddComCheckerGui-1.6.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## siogeen/tools/gui/IoddComChecker.py

```diff
@@ -22,14 +22,15 @@
 #from kivy.clock import Clock
 from kivymd.uix.scrollview import MDScrollView as ScrollView
 from kivy.properties import StringProperty
 from kivymd.uix.boxlayout import MDBoxLayout as BoxLayout
 from kivymd.uix.floatlayout import MDFloatLayout as FloatLayout
 from kivymd.uix.stacklayout import MDStackLayout as StackLayout
 from kivy.core.clipboard import Clipboard
+from kivy.clock import Clock
 
 from siogeen.tools import IoddComChecker
 
 class IoddComCheckerGui(App):
     def build(self):
         self.title = 'IoddComChecker ' + IoddComChecker.__version__
         self.theme_cls.primary_palette = "Blue" # "Green"
@@ -81,14 +82,16 @@
         self.autoBox.add_widget(self.floatMenu)
 
         self.screenBox.add_widget(self.scrollView)
         #self.screenBox.add_widget(self.mainBox)
         self.screenBox.add_widget(self.autoBox)
         self.screenBox.add_widget(self.menuBox)
 
+        self.clock = None
+
         return self.screenBox
 
     def contactSupport(self, *args):
         webbrowser.open("https://siogeen.com/#contact")
 
     def clearAddr(self, instance):
         self.addr.text = ''
@@ -98,26 +101,35 @@
 
     def clearText(self, instance):
         self.scanText.text = ''
 
     def copyText(self, instance):
         Clipboard.copy(self.scanText.text)
 
-    def print(self, text):
+    def print(self, text=''):
         self.scanText.text += text + '\n'
-        self.scanText.height = self.scanText.texture_size[1] + 70
+
+    def updateTextSize(self, dt):
+        self.scanText.height = self.scanText.texture_size[1]
+        print(f"height: {self.scanText.height}")
         if self.scanText.height > self.scrollView.height:
             self.scrollView.scroll_y = 0
 
     def runChecker(self, *args):
         self.scanBtn.disabled = True
         try:
+            self.clock = Clock.schedule_interval(self.updateTextSize, 0.25)
             IoddComChecker.check(*args)
         finally:
             self.scanText.text += '\n'
+
+            self.clock.cancel()
+            self.clock = None
+            Clock.schedule_once(self.updateTextSize, 0.25)
+
             self.scanBtn.disabled = False
 
     def scan(self, instance):
         addrs = self.addr.text
         if addrs:
             addrs = addrs.split(',')
         t = Thread(target=self.runChecker, args=(addrs, self.autoChk.active, self.print))
```

## Comparing `IoddComCheckerGui-1.6.4.dist-info/LICENSE.txt` & `IoddComCheckerGui-1.6.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `IoddComCheckerGui-1.6.4.dist-info/METADATA` & `IoddComCheckerGui-1.6.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IoddComCheckerGui
-Version: 1.6.4
+Version: 1.6.5
 Summary: IoddCom IO-Link master checker Gui
 Home-page: https://siogeen.com
 Author: Reimund Renner
 Author-email: reimund@siogeen.com
 License: proprietary and confidential
 Project-URL: Documentation, https://siogeen.com/doc/
 Project-URL: Help Desk, https://siogeen.com/helpdesk/
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: IoddComChecker (==1.6.4)
+Requires-Dist: IoddComChecker (>=1.6.4)
 Requires-Dist: kivymd
 
 IoddComCheckerGui - IoddComChecker GUI
 ======================================
 
 .. _IoddComChecker: /project/IoddComChecker
```

