# Comparing `tmp/ioddcomcheckergui-1.6.5-py3-none-any.whl.zip` & `tmp/ioddcomcheckergui-1.6.5.post1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5757 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     5517 b- defN 23-Apr-12 11:07 siogeen/tools/gui/IoddComChecker.py
--rw-rw-r--  2.0 unx      468 b- defN 23-Apr-12 11:07 siogeen/tools/gui/__init__.py
--rw-rw-r--  2.0 unx      732 b- defN 23-Apr-12 11:07 IoddComCheckerGui-1.6.5.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     5185 b- defN 23-Apr-12 11:07 IoddComCheckerGui-1.6.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 11:07 IoddComCheckerGui-1.6.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-12 11:07 IoddComCheckerGui-1.6.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      615 b- defN 23-Apr-12 11:07 IoddComCheckerGui-1.6.5.dist-info/RECORD
-7 files, 12617 bytes uncompressed, 4649 bytes compressed:  63.2%
+Zip file size: 5811 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     5468 b- defN 23-Apr-12 12:24 siogeen/tools/gui/IoddComChecker.py
+-rw-rw-r--  2.0 unx      468 b- defN 23-Apr-12 12:24 siogeen/tools/gui/__init__.py
+-rw-rw-r--  2.0 unx      732 b- defN 23-Apr-12 12:25 IoddComCheckerGui-1.6.5.post1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     5191 b- defN 23-Apr-12 12:25 IoddComCheckerGui-1.6.5.post1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 12:25 IoddComCheckerGui-1.6.5.post1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-12 12:25 IoddComCheckerGui-1.6.5.post1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      645 b- defN 23-Apr-12 12:25 IoddComCheckerGui-1.6.5.post1.dist-info/RECORD
+7 files, 12604 bytes uncompressed, 4643 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: siogeen/tools/gui/IoddComChecker.py
 Comment: 
 
 Filename: siogeen/tools/gui/__init__.py
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.dist-info/LICENSE.txt
+Filename: IoddComCheckerGui-1.6.5.post1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.dist-info/METADATA
+Filename: IoddComCheckerGui-1.6.5.post1.dist-info/METADATA
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.dist-info/WHEEL
+Filename: IoddComCheckerGui-1.6.5.post1.dist-info/WHEEL
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.dist-info/top_level.txt
+Filename: IoddComCheckerGui-1.6.5.post1.dist-info/top_level.txt
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.dist-info/RECORD
+Filename: IoddComCheckerGui-1.6.5.post1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## siogeen/tools/gui/IoddComChecker.py

```diff
@@ -106,15 +106,14 @@
         Clipboard.copy(self.scanText.text)
 
     def print(self, text=''):
         self.scanText.text += text + '\n'
 
     def updateTextSize(self, dt):
         self.scanText.height = self.scanText.texture_size[1]
-        print(f"height: {self.scanText.height}")
         if self.scanText.height > self.scrollView.height:
             self.scrollView.scroll_y = 0
 
     def runChecker(self, *args):
         self.scanBtn.disabled = True
         try:
             self.clock = Clock.schedule_interval(self.updateTextSize, 0.25)
```

## Comparing `IoddComCheckerGui-1.6.5.dist-info/LICENSE.txt` & `IoddComCheckerGui-1.6.5.post1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `IoddComCheckerGui-1.6.5.dist-info/METADATA` & `IoddComCheckerGui-1.6.5.post1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IoddComCheckerGui
-Version: 1.6.5
+Version: 1.6.5.post1
 Summary: IoddCom IO-Link master checker Gui
 Home-page: https://siogeen.com
 Author: Reimund Renner
 Author-email: reimund@siogeen.com
 License: proprietary and confidential
 Project-URL: Documentation, https://siogeen.com/doc/
 Project-URL: Help Desk, https://siogeen.com/helpdesk/
```

