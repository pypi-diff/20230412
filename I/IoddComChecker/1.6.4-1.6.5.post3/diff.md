# Comparing `tmp/ioddcomchecker-1.6.4-cp39-cp39-win_amd64.whl.zip` & `tmp/ioddcomchecker-1.6.5.post3-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 54802 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      732 b- defN 23-Mar-18 02:26 siogeen/LICENSE.txt
--rw-rw-rw-  2.0 fat   112640 b- defN 23-Mar-18 02:26 siogeen/tools/IoddComChecker.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      462 b- defN 23-Mar-18 02:26 siogeen/tools/__init__.py
--rw-rw-rw-  2.0 fat     1188 b- defN 23-Mar-18 02:26 siogeen/tools/cli/IoddComChecker.py
--rw-rw-rw-  2.0 fat      732 b- defN 23-Mar-18 02:26 IoddComChecker-1.6.4.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     5619 b- defN 23-Mar-18 02:26 IoddComChecker-1.6.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Mar-18 02:26 IoddComChecker-1.6.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-18 02:26 IoddComChecker-1.6.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      778 b- defN 23-Mar-18 02:26 IoddComChecker-1.6.4.dist-info/RECORD
-9 files, 122259 bytes uncompressed, 53448 bytes compressed:  56.3%
+Zip file size: 56236 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      732 b- defN 23-Apr-12 13:07 siogeen/LICENSE.txt
+-rw-rw-rw-  2.0 fat   115712 b- defN 23-Apr-12 13:08 siogeen/tools/IoddComChecker.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      462 b- defN 23-Apr-12 13:07 siogeen/tools/__init__.py
+-rw-rw-rw-  2.0 fat     1188 b- defN 23-Apr-12 13:07 siogeen/tools/cli/IoddComChecker.py
+-rw-rw-rw-  2.0 fat      732 b- defN 23-Apr-12 13:08 IoddComChecker-1.6.5.post3.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     5625 b- defN 23-Apr-12 13:08 IoddComChecker-1.6.5.post3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-12 13:08 IoddComChecker-1.6.5.post3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-12 13:08 IoddComChecker-1.6.5.post3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      808 b- defN 23-Apr-12 13:08 IoddComChecker-1.6.5.post3.dist-info/RECORD
+9 files, 125367 bytes uncompressed, 54822 bytes compressed:  56.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: siogeen/tools/__init__.py
 Comment: 
 
 Filename: siogeen/tools/cli/IoddComChecker.py
 Comment: 
 
-Filename: IoddComChecker-1.6.4.dist-info/LICENSE.txt
+Filename: IoddComChecker-1.6.5.post3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: IoddComChecker-1.6.4.dist-info/METADATA
+Filename: IoddComChecker-1.6.5.post3.dist-info/METADATA
 Comment: 
 
-Filename: IoddComChecker-1.6.4.dist-info/WHEEL
+Filename: IoddComChecker-1.6.5.post3.dist-info/WHEEL
 Comment: 
 
-Filename: IoddComChecker-1.6.4.dist-info/top_level.txt
+Filename: IoddComChecker-1.6.5.post3.dist-info/top_level.txt
 Comment: 
 
-Filename: IoddComChecker-1.6.4.dist-info/RECORD
+Filename: IoddComChecker-1.6.5.post3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `IoddComChecker-1.6.4.dist-info/LICENSE.txt` & `IoddComChecker-1.6.5.post3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `IoddComChecker-1.6.4.dist-info/METADATA` & `IoddComChecker-1.6.5.post3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IoddComChecker
-Version: 1.6.4
+Version: 1.6.5.post3
 Summary: IoddCom IO-Link master checker
 Home-page: https://siogeen.com
 Author: Reimund Renner
 Author-email: reimund@siogeen.com
 License: proprietary and confidential
 Project-URL: Documentation, https://siogeen.com/doc/
 Project-URL: Help Desk, https://siogeen.com/helpdesk/
@@ -28,15 +28,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: IoddComBase (==1.6.4)
+Requires-Dist: IoddComBase (>=1.6.4)
 Requires-Dist: dict2obj
 
 IoddComChecker - IoddCom Checker
 ================================
 
 .. _IoddComCheckerGui: /project/IoddComCheckerGui
```

## Comparing `IoddComChecker-1.6.4.dist-info/RECORD` & `IoddComChecker-1.6.5.post3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 siogeen/LICENSE.txt,sha256=mjUk_O3YPxAZeoS61zCys2pyShGDxR4ghwb55ItZ0lg,732
-siogeen/tools/IoddComChecker.cp39-win_amd64.pyd,sha256=HohMDYwnWcZd3aeOvJdd6icS4FAUxX1dkV2ZJ2cnBOA,112640
+siogeen/tools/IoddComChecker.cp39-win_amd64.pyd,sha256=m_ZY9_mHLLAbGcWhmior5O9fahbGxgjbTV_2C8TH1Kk,115712
 siogeen/tools/__init__.py,sha256=CCpWoKGerJjGcTDaC48F6skWG4rDZuBzIKxBIZqL74w,462
 siogeen/tools/cli/IoddComChecker.py,sha256=055FuCrKYio4xKOlE-uncCtc95w7P_7jqZbGEmgSncY,1188
-IoddComChecker-1.6.4.dist-info/LICENSE.txt,sha256=mjUk_O3YPxAZeoS61zCys2pyShGDxR4ghwb55ItZ0lg,732
-IoddComChecker-1.6.4.dist-info/METADATA,sha256=D_0di9F2nrR9VaDIiyPhkn5X13oPbXu1EekhdhlcHug,5619
-IoddComChecker-1.6.4.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
-IoddComChecker-1.6.4.dist-info/top_level.txt,sha256=vIFg0bLkihbkHyuCZUdHmA-50LP8LvTwDknGWir0T5o,8
-IoddComChecker-1.6.4.dist-info/RECORD,,
+IoddComChecker-1.6.5.post3.dist-info/LICENSE.txt,sha256=mjUk_O3YPxAZeoS61zCys2pyShGDxR4ghwb55ItZ0lg,732
+IoddComChecker-1.6.5.post3.dist-info/METADATA,sha256=K6E504_uguXIystXT3FbmsGykZ1VDIZO11I7f1wQshM,5625
+IoddComChecker-1.6.5.post3.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
+IoddComChecker-1.6.5.post3.dist-info/top_level.txt,sha256=vIFg0bLkihbkHyuCZUdHmA-50LP8LvTwDknGWir0T5o,8
+IoddComChecker-1.6.5.post3.dist-info/RECORD,,
```

